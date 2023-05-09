# Comparing `tmp/spotlight-dev-0.0.1b5.tar.gz` & `tmp/spotlight-dev-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-dev-0.0.1b5.tar", last modified: Fri May  5 22:35:30 2023, max compression
+gzip compressed data, was "spotlight-dev-0.0.1b6.tar", last modified: Tue May  9 17:15:56 2023, max compression
```

## Comparing `spotlight-dev-0.0.1b5.tar` & `spotlight-dev-0.0.1b6.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.877600 spotlight-dev-0.0.1b5/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 22:35:30.877600 spotlight-dev-0.0.1b5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 22:35:30.877600 spotlight-dev-0.0.1b5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.833597 spotlight-dev-0.0.1b5/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.834597 spotlight-dev-0.0.1b5/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.835597 spotlight-dev-0.0.1b5/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.837597 spotlight-dev-0.0.1b5/spotlight/api/job/
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.839597 spotlight-dev-0.0.1b5/spotlight/api/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/job/view/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.841597 spotlight-dev-0.0.1b5/spotlight/api/organization/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.843598 spotlight-dev-0.0.1b5/spotlight/api/organization/user/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/user/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.845598 spotlight-dev-0.0.1b5/spotlight/api/organization/view/
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/organization/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.847598 spotlight-dev-0.0.1b5/spotlight/api/rule/
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.849598 spotlight-dev-0.0.1b5/spotlight/api/tag/
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.851598 spotlight-dev-0.0.1b5/spotlight/api/tag/view/
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/api/tag/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.851598 spotlight-dev-0.0.1b5/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.854598 spotlight-dev-0.0.1b5/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.855598 spotlight-dev-0.0.1b5/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.855598 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.857599 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.858599 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.858599 spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.860599 spotlight-dev-0.0.1b5/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.861599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/decorator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.862599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.864599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/sql_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.866599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/rule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.866599 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/
--rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.871600 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.872600 spotlight-dev-0.0.1b5/spotlight/pandas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-05-05 22:35:04.000000 spotlight-dev-0.0.1b5/spotlight/pandas/runners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 22:35:30.876600 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1413 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3859 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-05 22:35:30.000000 spotlight-dev-0.0.1b5/spotlight_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.026770 spotlight-dev-0.0.1b6/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 17:15:56.026770 spotlight-dev-0.0.1b6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      852 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 17:15:56.026770 spotlight-dev-0.0.1b6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.964765 spotlight-dev-0.0.1b6/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.965765 spotlight-dev-0.0.1b6/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.967765 spotlight-dev-0.0.1b6/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1726 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.972766 spotlight-dev-0.0.1b6/spotlight/api/job/
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.976766 spotlight-dev-0.0.1b6/spotlight/api/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/job/view/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.979766 spotlight-dev-0.0.1b6/spotlight/api/organization/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2805 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2503 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.983766 spotlight-dev-0.0.1b6/spotlight/api/organization/user/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/user/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.986767 spotlight-dev-0.0.1b6/spotlight/api/organization/view/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/organization/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.990767 spotlight-dev-0.0.1b6/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3667 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      962 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.993767 spotlight-dev-0.0.1b6/spotlight/api/tag/
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1297 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.997767 spotlight-dev-0.0.1b6/spotlight/api/tag/view/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/api/tag/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:55.998767 spotlight-dev-0.0.1b6/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.003768 spotlight-dev-0.0.1b6/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.004768 spotlight-dev-0.0.1b6/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.005768 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.007768 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3898 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.009768 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.010769 spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.011768 spotlight-dev-0.0.1b6/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.013769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5958 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.014769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.016769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2154 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/sql_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     3413 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.018769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/rule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.019769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/
+-rw-rw-rw-   0 root         (0) root         (0)     6327 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.020769 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.022769 spotlight-dev-0.0.1b6/spotlight/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-09 17:15:39.000000 spotlight-dev-0.0.1b6/spotlight/pandas/runners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 17:15:56.025770 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3859 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 17:15:55.000000 spotlight-dev-0.0.1b6/spotlight_dev.egg-info/top_level.txt
```

### Comparing `spotlight-dev-0.0.1b5/PKG-INFO` & `spotlight-dev-0.0.1b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b5/README.md` & `spotlight-dev-0.0.1b6/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/setup.py` & `spotlight-dev-0.0.1b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="spotlight-dev",
-    version="0.0.1b5",
+    version="0.0.1b6",
     author="Spotlight",
     author_email="hello@spotlight.dev",
     description="Spotlight Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/auth/__util.py` & `spotlight-dev-0.0.1b6/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/auth/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/auth/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/job/__util.py` & `spotlight-dev-0.0.1b6/spotlight/api/job/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/job/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/job/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/job/model.py` & `spotlight-dev-0.0.1b6/spotlight/api/job/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/job/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/job/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/job/view/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/__util.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/user/__util.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/user/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/user/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/user/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/user/model.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/user/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/user/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/user/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/view/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/organization/view/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/organization/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/rule/__util.py` & `spotlight-dev-0.0.1b6/spotlight/api/rule/__util.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def _get_all_rules_by_tags_request_info(request: LookupRequest) -> dict:
     return {"endpoint": f"dq/rule", "json": request.request_dict()}
 
 
 def _search_rules_request_info(request: SearchRequest) -> dict:
-    return {"endpoint": f"dq/rule", "json": request.request_dict()}
+    return {"endpoint": f"dq/rule/search", "json": request.request_dict()}
 
 
 def _create_rule_request_info(request: RuleRequest) -> dict:
     return {"endpoint": f"dq/rule", "json": request.request_dict()}
 
 
 def _update_rule_request_info(id: str, request: RuleRequest) -> dict:
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/rule/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/rule/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/rule/model.py` & `spotlight-dev-0.0.1b6/spotlight/api/rule/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from typing import Optional, List
 
 from pydantic import Field
 
 from spotlight.core.common.base import Base
-from spotlight.core.common.enum import Severity
+from spotlight.core.common.enum import Severity, ThresholdType
 
 
 class RuleRequest(Base):
     name: str
     predicate: str
     description: Optional[str] = Field(default=None)
-    threshold: Optional[int] = Field(default=None)
+    threshold: Optional[float] = Field(default=None)
+    threshold_type: Optional[ThresholdType] = Field(default=ThresholdType.TOTAL)
     severity: Optional[Severity] = Field(default=Severity.ERROR)
     sampling_fields: Optional[List[str]] = Field(default=None)
 
 
 class RuleResponse(Base):
     id: str
     name: str
     description: Optional[str]
     predicate: str
-    threshold: int
+    threshold: float
+    threshold_type: ThresholdType
     severity: Severity
     sampling_fields: List[str]
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/rule/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/rule/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/tag/__util.py` & `spotlight-dev-0.0.1b6/spotlight/api/tag/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/tag/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/tag/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/tag/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/tag/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/tag/view/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/tag/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/api/tag/view/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/api/tag/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/base.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/config.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -60,22 +60,22 @@
         env = os.getenv("SPOTLIGHT_ENV", "production")
         return env
 
     @property
     def urls(self) -> dict:
         env_url_map = {
             "production": {
-                "spotlight": "https://api.algoralabs.com",
-                "keycloak_admin": "https://auth.algoralabs.com/auth/admin/realms/production",
-                "keycloak": "https://auth.algoralabs.com/auth/realms/production",
+                "spotlight": "https://api.spotlight.dev",
+                "keycloak_admin": "https://auth.spotlight.dev/auth/admin/realms/production",
+                "keycloak": "https://auth.spotlight.dev/auth/realms/production",
             },
             "development": {
-                "spotlight": "https://api.dev.algoralabs.com",
-                "keycloak_admin": "https://auth.dev.algoralabs.com/auth/admin/realms/production",
-                "keycloak": "https://auth.dev.algoralabs.com/auth/realms/production",
+                "spotlight": "https://api.dev.spotlight.dev",
+                "keycloak_admin": "https://auth.dev.spotlight.dev/auth/admin/realms/production",
+                "keycloak": "https://auth.dev.spotlight.dev/auth/realms/production",
             },
         }
         return env_url_map.get(self.environment, env_url_map["production"])
 
     def get_url(self, key: str = "spotlight") -> str:
         """
         Get base URL given key.
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/date/function.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/__util.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/decorators/timeit.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/errors.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/function.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/metaclass/singleton.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/requests/asynchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/common/requests/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/abstract.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/abstract.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/decorator.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/decorator.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/abstract.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from abc import ABC, abstractmethod
 from typing import Any, List, Optional
 
-from spotlight.core.common.enum import Severity
+from spotlight.core.common.enum import Severity, ThresholdType
 from spotlight.core.pipeline.execution.rule.enum import RuleTypes
 
 
 class AbstractRule(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
         """
         Name of the rule
         """
         pass
 
     @property
     @abstractmethod
-    def threshold(self) -> int:
+    def threshold(self) -> float:
+        """
+        Threshold for the number of flagged results to cause a rule to fail with the specified severity
+        """
+        pass
+
+    @property
+    @abstractmethod
+    def threshold_type(self) -> ThresholdType:
         """
         Threshold for the number of flagged results to cause a rule to fail with the specified severity
         """
         pass
 
     @property
     @abstractmethod
@@ -61,14 +69,18 @@
     def name(self) -> str:
         return self.__class__.__name__
 
     @property
     def sampling_fields(self) -> Optional[List[str]]:
         return []
 
+    @property
+    def threshold_type(self) -> ThresholdType:
+        return ThresholdType.TOTAL
+
     def to_dict(self):
         props = self._properties()
         props.update({"type": RuleTypes.CUSTOM_CODE.value})
         return props
 
     @abstractmethod
     def test(self, data: Any) -> Any:
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/rule/sql_rule.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/rule/sql_rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 from typing import Optional, List
 
 from spotlight.api.rule.model import RuleResponse
-from spotlight.core.common.enum import Severity
+from spotlight.core.common.enum import Severity, ThresholdType
 from spotlight.core.pipeline.execution.rule.abstract import AbstractRule
 from spotlight.core.pipeline.execution.rule.enum import RuleTypes
 
 
 class SQLRule(AbstractRule):
     def __init__(
         self,
         name: str,
         predicate: str,
-        threshold: int,
+        threshold: float,
+        threshold_type: ThresholdType,
         severity: Severity,
         sampling_fields: Optional[List[str]] = None,
     ):
         self._name = name
         self.predicate = predicate
         self._threshold = threshold
+        self._threshold_type = threshold_type
         self._severity = severity
         self._sampling_fields = sampling_fields
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def threshold(self) -> int:
+    def threshold(self) -> float:
         return self._threshold
 
     @property
+    def threshold_type(self) -> ThresholdType:
+        return self._threshold_type
+
+    @property
     def severity(self) -> Severity:
         return self._severity
 
     @property
     def sampling_fields(self) -> Optional[List[str]]:
         return self._sampling_fields
 
@@ -44,10 +50,11 @@
 
     @classmethod
     def from_rule_response(cls, rule: RuleResponse) -> "SQLRule":
         return cls(
             name=rule.name,
             predicate=rule.predicate,
             threshold=rule.threshold,
+            threshold_type=rule.threshold_type,
             severity=Severity(rule.severity),
             sampling_fields=rule.sampling_fields,
         )
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/execution/synchronous.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/execution/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,10 +89,11 @@
 
     Returns:
         RuleResult: The result of the rule
     """
     logger.debug(f"Running rule {rule.name}")
     result = apply_rule(data, rule)
     logger.info(
-        f"Rule completed [name={rule.name}, flagged_results={result.flagged_results}, threshold={rule.threshold}]: {result.status}"
+        f"Rule completed [name={rule.name}, flagged_results={result.flagged_results}, threshold={rule.threshold}, "
+        f"threshold_type={rule.threshold_type}]: {result.status}"
     )
     return result
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/model/pipeline.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/__init__.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/asynchronously.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/asynchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/core/pipeline/runner/utils/synchronously.py` & `spotlight-dev-0.0.1b6/spotlight/core/pipeline/runner/utils/synchronously.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/pandas/__util.py` & `spotlight-dev-0.0.1b6/spotlight/pandas/__util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,100 @@
 import logging
 from typing import List
 
 import pandas as pd
 
 from spotlight.api.rule.model import RuleResponse
-from spotlight.core.common.enum import Severity, Status
+from spotlight.core.common.enum import Severity, Status, ThresholdType
 from spotlight.core.pipeline.execution.rule import AbstractRule
 from spotlight.core.pipeline.model.rule import RuleResult
 
 logger = logging.getLogger(__name__)
 
 
 def build_rule_result(
-    rule: AbstractRule, start_time: int, end_time: int, result: pd.DataFrame
+    rule: AbstractRule,
+    start_time: int,
+    end_time: int,
+    data: pd.DataFrame,
+    result: pd.DataFrame,
 ) -> RuleResult:
     """
     Helper method for building the rule result.
 
     Args:
         rule (RuleResponse): The rule being applied to the data
         start_time (int): The timestamp from when the job started
         end_time (int): The timestamp from when the job ended
+        data (pd.DataFrame): The raw dataset being tested
         result (pd.DataFrame): All the rules that failed the test
 
     Result:
         RuleResult: The result of the rule
     """
-    status = get_rule_status(result, rule.threshold, rule.severity)
+    status = get_rule_status(rule, data, result)
     samples = construct_samples(rule, result) if status != Status.SUCCESS else []
     return RuleResult(
         start_time=start_time,
         end_time=end_time,
         status=status,
         flagged_results=len(result),
         rule=rule.to_dict(),
         samples=samples,
     )
 
 
-def get_rule_status(result: pd.DataFrame, threshold: int, severity: Severity) -> Status:
+def get_rule_status(
+    rule: AbstractRule,
+    data: pd.DataFrame,
+    result: pd.DataFrame,
+) -> Status:
     """
     Helper method for determining the Status of the rule.
 
     Args:
-        result (pd.DataFrame): All the rows that failed the rule
-        threshold (int): The number of results needed to cause the rule to fail
-        severity (Severity): The severity level of the rule
+        rule (RuleResponse): The rule applied to the data
+        data (pd.DataFrame): The raw dataset being tested
+        result (pd.DataFrame): All the rules that failed the test
 
     Returns:
         Status: The status of the rule
     """
-    success = len(result) < threshold
+    success = is_successful(len(result), len(data), rule)
     if success:
         return Status.SUCCESS
-    elif severity == Severity.WARN:
+    elif rule.severity == Severity.WARN:
         return Status.WARNING
     else:
         return Status.FAILURE
 
 
+def is_successful(failure_count: int, total_count: int, rule: AbstractRule) -> bool:
+    """
+    Helper method for determining the success of a rule
+
+    Args:
+        failure_count (int): The number of flagged results
+        total_count (int): The total number of data points tested
+        rule (AbstractRule): The rule run on the data
+
+    Returns:
+        bool: A flag representing the success of a job
+    """
+    if rule.threshold_type == ThresholdType.TOTAL:
+        return failure_count < rule.threshold
+    elif rule.threshold_type == ThresholdType.PERCENTAGE:
+        failure_percentage = (failure_count / total_count) * 100
+        return failure_percentage < rule.threshold
+
+
 def construct_samples(rule: AbstractRule, results: pd.DataFrame) -> List[dict]:
-    """ """
+    """
+    Helper method for extracting a sample from the failed results
+    """
     fields = set(rule.sampling_fields) if rule.sampling_fields else set()
     if fields == set():
         return []
 
     schema = list(results.columns)
     fields = schema if fields == {"*"} else fields.intersection(set(schema))
     sample = results[fields][:10]
```

### Comparing `spotlight-dev-0.0.1b5/spotlight/pandas/pipeline.py` & `spotlight-dev-0.0.1b6/spotlight/pandas/pipeline.py`

 * *Files identical despite different names*

### Comparing `spotlight-dev-0.0.1b5/spotlight/pandas/runners.py` & `spotlight-dev-0.0.1b6/spotlight/pandas/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         FROM data
         WHERE {rule.predicate}
     """
     start_time = current_timestamp()
     result = duckdb.query(query).to_df()
     end_time = current_timestamp()
     logger.debug(f"Pandas sql rule {rule.name} completed")
-    result = build_rule_result(rule, start_time, end_time, result)
+    result = build_rule_result(rule, start_time, end_time, data, result)
     return result
 
 
 def pandas_custom_code_rule_runner(
     data: pd.DataFrame, rule: AbstractCustomCodeRule
 ) -> RuleResult:
     """
@@ -48,10 +48,10 @@
     Result:
         RuleResult: The result of the rule
     """
     logger.debug(f"Running pandas custom code rule {rule.name}")
     start_time = current_timestamp()
     result = rule.test(data)
     end_time = current_timestamp()
-    result = build_rule_result(rule, start_time, end_time, result)
+    result = build_rule_result(rule, start_time, end_time, data, result)
     logger.debug(f"Pandas custom code rule {rule.name} completed")
     return result
```

### Comparing `spotlight-dev-0.0.1b5/spotlight_dev.egg-info/PKG-INFO` & `spotlight-dev-0.0.1b6/spotlight_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-dev
-Version: 0.0.1b5
+Version: 0.0.1b6
 Summary: Spotlight Python SDK
 Home-page: https://alpha.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The data quality platform for developers
```

### Comparing `spotlight-dev-0.0.1b5/spotlight_dev.egg-info/SOURCES.txt` & `spotlight-dev-0.0.1b6/spotlight_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

