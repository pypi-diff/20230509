# Comparing `tmp/git3Client-0.2.5.tar.gz` & `tmp/git3Client-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git3Client-0.2.5.tar", last modified: Mon Sep 12 09:03:31 2022, max compression
+gzip compressed data, was "git3Client-0.2.6.tar", last modified: Tue May  9 11:49:58 2023, max compression
```

## Comparing `git3Client-0.2.5.tar` & `git3Client-0.2.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.827612 git3Client-0.2.5/
--rw-r--r--   0 jacek.varky   (501) staff       (20)     1068 2022-03-18 05:45:10.000000 git3Client-0.2.5/LICENSE
--rw-r--r--   0 jacek.varky   (501) staff       (20)       48 2022-06-28 07:27:15.000000 git3Client-0.2.5/MANIFEST.in
--rw-r--r--   0 jacek.varky   (501) staff       (20)     6362 2022-09-12 09:03:31.827348 git3Client-0.2.5/PKG-INFO
--rw-r--r--   0 jacek.varky   (501) staff       (20)     6175 2022-09-01 18:08:07.000000 git3Client-0.2.5/README.md
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.773141 git3Client-0.2.5/git3Client/
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      132 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/__main__.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.757904 git3Client-0.2.5/git3Client/artifacts/
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.758901 git3Client-0.2.5/git3Client/artifacts/contracts/
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.758509 git3Client-0.2.5/git3Client/artifacts/contracts/factory_facets/
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.781245 git3Client-0.2.5/git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/
--rw-r--r--   0 jacek.varky   (501) staff       (20)    64291 2022-09-01 17:25:50.000000 git3Client-0.2.5/git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/RepositoryManagement.json
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.759444 git3Client-0.2.5/git3Client/artifacts/contracts/repo_facets/
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.783527 git3Client-0.2.5/git3Client/artifacts/contracts/repo_facets/GitBranch.sol/
--rw-r--r--   0 jacek.varky   (501) staff       (20)    23255 2022-09-01 17:23:11.000000 git3Client-0.2.5/git3Client/artifacts/contracts/repo_facets/GitBranch.sol/GitBranch.json
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.787405 git3Client-0.2.5/git3Client/config/
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/config/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      665 2022-09-09 09:31:03.000000 git3Client-0.2.5/git3Client/config/config.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.797591 git3Client-0.2.5/git3Client/dlt/
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/dlt/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     2012 2022-09-01 17:47:22.000000 git3Client-0.2.5/git3Client/dlt/contract.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      546 2022-05-19 11:27:10.000000 git3Client-0.2.5/git3Client/dlt/provider.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)    10252 2022-09-09 09:19:53.000000 git3Client-0.2.5/git3Client/dlt/repository.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     1367 2022-09-02 10:50:16.000000 git3Client-0.2.5/git3Client/dlt/storageClient.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      264 2022-03-21 10:46:08.000000 git3Client-0.2.5/git3Client/dlt/user.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.799375 git3Client-0.2.5/git3Client/exceptions/
--rw-r--r--   0 jacek.varky   (501) staff       (20)      266 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/exceptions/NoABIFoundError.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      259 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/exceptions/NoRepositoryError.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/exceptions/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     8217 2022-05-19 11:27:10.000000 git3Client-0.2.5/git3Client/git3.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.819387 git3Client-0.2.5/git3Client/gitCommands/
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     3177 2022-05-19 11:27:15.000000 git3Client-0.2.5/git3Client/gitCommands/add.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     3038 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/branch.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     1376 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/catFile.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     4937 2022-09-01 18:01:56.000000 git3Client-0.2.5/git3Client/gitCommands/checkout.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     3609 2022-09-06 17:12:42.000000 git3Client-0.2.5/git3Client/gitCommands/clone.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     3597 2022-05-19 11:27:15.000000 git3Client-0.2.5/git3Client/gitCommands/commit.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     2484 2022-09-09 09:18:56.000000 git3Client-0.2.5/git3Client/gitCommands/create.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     3554 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/diff.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     4062 2022-05-19 11:27:10.000000 git3Client-0.2.5/git3Client/gitCommands/fetch.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      161 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/getAddress.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      584 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/hashObject.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     1213 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/init.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      451 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/lsFiles.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)    11561 2022-05-19 11:27:10.000000 git3Client-0.2.5/git3Client/gitCommands/merge.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     4182 2022-05-19 11:27:10.000000 git3Client-0.2.5/git3Client/gitCommands/pull.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     2231 2022-09-06 12:31:55.000000 git3Client-0.2.5/git3Client/gitCommands/push.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      482 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitCommands/status.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.823851 git3Client-0.2.5/git3Client/gitInternals/
--rw-r--r--   0 jacek.varky   (501) staff       (20)      195 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitInternals/IndexEntry.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitInternals/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)      120 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitInternals/fileMode.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     4826 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitInternals/gitCommit.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     5631 2022-05-19 11:27:15.000000 git3Client-0.2.5/git3Client/gitInternals/gitIndex.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     4401 2022-05-19 11:27:15.000000 git3Client-0.2.5/git3Client/gitInternals/gitObject.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     6477 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/gitInternals/gitTree.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.826379 git3Client-0.2.5/git3Client/utils/
--rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.5/git3Client/utils/__init__.py
--rw-r--r--   0 jacek.varky   (501) staff       (20)     6731 2022-09-09 09:31:16.000000 git3Client-0.2.5/git3Client/utils/utils.py
-drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2022-09-12 09:03:31.777990 git3Client-0.2.5/git3Client.egg-info/
--rw-r--r--   0 jacek.varky   (501) staff       (20)     6362 2022-09-12 09:03:31.000000 git3Client-0.2.5/git3Client.egg-info/PKG-INFO
--rw-r--r--   0 jacek.varky   (501) staff       (20)     1723 2022-09-12 09:03:31.000000 git3Client-0.2.5/git3Client.egg-info/SOURCES.txt
--rw-r--r--   0 jacek.varky   (501) staff       (20)        1 2022-09-12 09:03:31.000000 git3Client-0.2.5/git3Client.egg-info/dependency_links.txt
--rw-r--r--   0 jacek.varky   (501) staff       (20)       49 2022-09-12 09:03:31.000000 git3Client-0.2.5/git3Client.egg-info/entry_points.txt
--rw-r--r--   0 jacek.varky   (501) staff       (20)     1007 2022-09-12 09:03:31.000000 git3Client-0.2.5/git3Client.egg-info/requires.txt
--rw-r--r--   0 jacek.varky   (501) staff       (20)       11 2022-09-12 09:03:31.000000 git3Client-0.2.5/git3Client.egg-info/top_level.txt
--rw-r--r--   0 jacek.varky   (501) staff       (20)       38 2022-09-12 09:03:31.827719 git3Client-0.2.5/setup.cfg
--rw-r--r--   0 jacek.varky   (501) staff       (20)     2729 2022-09-12 09:03:07.000000 git3Client-0.2.5/setup.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.626839 git3Client-0.2.6/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     1068 2022-03-18 05:45:10.000000 git3Client-0.2.6/LICENSE
+-rw-r--r--   0 jacek.varky   (501) staff       (20)       48 2022-06-28 07:27:15.000000 git3Client-0.2.6/MANIFEST.in
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     6496 2023-05-09 11:49:58.626510 git3Client-0.2.6/PKG-INFO
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     6348 2023-05-09 11:43:18.000000 git3Client-0.2.6/README.md
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.596833 git3Client-0.2.6/git3Client/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      132 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/__main__.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.590218 git3Client-0.2.6/git3Client/artifacts/
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.591284 git3Client-0.2.6/git3Client/artifacts/contracts/
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.591025 git3Client-0.2.6/git3Client/artifacts/contracts/factory_facets/
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.599822 git3Client-0.2.6/git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)    64291 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/RepositoryManagement.json
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.591542 git3Client-0.2.6/git3Client/artifacts/contracts/repo_facets/
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.600573 git3Client-0.2.6/git3Client/artifacts/contracts/repo_facets/GitBranch.sol/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)    23255 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/artifacts/contracts/repo_facets/GitBranch.sol/GitBranch.json
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.601390 git3Client-0.2.6/git3Client/config/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/config/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      393 2023-05-08 12:24:26.000000 git3Client-0.2.6/git3Client/config/config.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.604704 git3Client-0.2.6/git3Client/dlt/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/dlt/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     2012 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/dlt/contract.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      546 2022-05-19 11:27:10.000000 git3Client-0.2.6/git3Client/dlt/provider.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)    10252 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/dlt/repository.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     1450 2023-05-09 11:37:51.000000 git3Client-0.2.6/git3Client/dlt/storageClient.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      264 2022-03-21 10:46:08.000000 git3Client-0.2.6/git3Client/dlt/user.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.606222 git3Client-0.2.6/git3Client/exceptions/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      266 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/exceptions/NoABIFoundError.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      259 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/exceptions/NoRepositoryError.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/exceptions/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     8217 2022-05-19 11:27:10.000000 git3Client-0.2.6/git3Client/git3.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.616210 git3Client-0.2.6/git3Client/gitCommands/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     3177 2022-05-19 11:27:15.000000 git3Client-0.2.6/git3Client/gitCommands/add.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     3038 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/branch.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     1376 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/catFile.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     4937 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/gitCommands/checkout.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     3609 2022-09-06 17:12:42.000000 git3Client-0.2.6/git3Client/gitCommands/clone.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     3597 2022-05-19 11:27:15.000000 git3Client-0.2.6/git3Client/gitCommands/commit.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     2484 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/gitCommands/create.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     3554 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/diff.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     4062 2022-05-19 11:27:10.000000 git3Client-0.2.6/git3Client/gitCommands/fetch.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      161 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/getAddress.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      584 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/hashObject.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     1213 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/init.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      451 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/lsFiles.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)    11561 2022-05-19 11:27:10.000000 git3Client-0.2.6/git3Client/gitCommands/merge.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     4182 2022-05-19 11:27:10.000000 git3Client-0.2.6/git3Client/gitCommands/pull.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     2231 2022-09-12 09:10:24.000000 git3Client-0.2.6/git3Client/gitCommands/push.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      482 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitCommands/status.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.623437 git3Client-0.2.6/git3Client/gitInternals/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      195 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitInternals/IndexEntry.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitInternals/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)      120 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitInternals/fileMode.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     4826 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitInternals/gitCommit.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     5631 2022-05-19 11:27:15.000000 git3Client-0.2.6/git3Client/gitInternals/gitIndex.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     4401 2022-05-19 11:27:15.000000 git3Client-0.2.6/git3Client/gitInternals/gitObject.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     6477 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/gitInternals/gitTree.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.625404 git3Client-0.2.6/git3Client/utils/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        0 2022-03-18 05:45:10.000000 git3Client-0.2.6/git3Client/utils/__init__.py
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     6731 2023-05-09 11:37:42.000000 git3Client-0.2.6/git3Client/utils/utils.py
+drwxr-xr-x   0 jacek.varky   (501) staff       (20)        0 2023-05-09 11:49:58.599392 git3Client-0.2.6/git3Client.egg-info/
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     6496 2023-05-09 11:49:58.000000 git3Client-0.2.6/git3Client.egg-info/PKG-INFO
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     1723 2023-05-09 11:49:58.000000 git3Client-0.2.6/git3Client.egg-info/SOURCES.txt
+-rw-r--r--   0 jacek.varky   (501) staff       (20)        1 2023-05-09 11:49:58.000000 git3Client-0.2.6/git3Client.egg-info/dependency_links.txt
+-rw-r--r--   0 jacek.varky   (501) staff       (20)       49 2023-05-09 11:49:58.000000 git3Client-0.2.6/git3Client.egg-info/entry_points.txt
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     1007 2023-05-09 11:49:58.000000 git3Client-0.2.6/git3Client.egg-info/requires.txt
+-rw-r--r--   0 jacek.varky   (501) staff       (20)       11 2023-05-09 11:49:58.000000 git3Client-0.2.6/git3Client.egg-info/top_level.txt
+-rw-r--r--   0 jacek.varky   (501) staff       (20)       38 2023-05-09 11:49:58.626965 git3Client-0.2.6/setup.cfg
+-rw-r--r--   0 jacek.varky   (501) staff       (20)     2729 2023-05-09 11:49:32.000000 git3Client-0.2.6/setup.py
```

### Comparing `git3Client-0.2.5/LICENSE` & `git3Client-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/PKG-INFO` & `git3Client-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: git3Client
-Version: 0.2.5
+Version: 0.2.6
 Summary: Git3 Python client
 Home-page: https://github.com/varkiwi/git3-client
 Author: Jacek Varky
 Author-email: jaca347@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Stake to support us](https://badge.devprotocol.xyz/0xc6286Fc480Ba4d15981664a3350ABF12b0b7Feda/descriptive)](https://stakes.social/0xc6286Fc480Ba4d15981664a3350ABF12b0b7Feda)
 
 # GIT 3
@@ -61,16 +59,18 @@
 #### Gitconfig
 Here is how the contant of the `~/.gitconfig` file looks like
 ```bash
 [user]
         email = author email
         name = author name
         IdentityFile = path to private key in pem format. It has to be the absolute path! No $HOME or similar stuff in it
+        Web3StorageApiKey = APIKey
 ```
 Set the values according to your needs.
+The `Web3StorageApiKey` can be obtained from https://web3.storage/. Just create an account and copy the API key from the settings page.
 
 #### Repository config
 If you want to use a different configuration for each repository, just add a `config` file into the `.git/` in your repository and add the same entries as in the `~/.gitconfig` file.
 
 # Git Commands
 
 ## Git init
@@ -148,9 +148,7 @@
 ## How to push to PyPi
 
 In the active virtual env, execute the following: `python setup.py sdist bdist_wheel`
 This will create a dist folder. Once done, you can publish to Pypi using twine (pip3 install twine)
 `twine upload dist/*` - enter credentials and that's it. After that you should be able to install your package 
 using pip3 install [name]
 
-
-
```

### Comparing `git3Client-0.2.5/README.md` & `git3Client-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,18 @@
 #### Gitconfig
 Here is how the contant of the `~/.gitconfig` file looks like
 ```bash
 [user]
         email = author email
         name = author name
         IdentityFile = path to private key in pem format. It has to be the absolute path! No $HOME or similar stuff in it
+        Web3StorageApiKey = APIKey
 ```
 Set the values according to your needs.
+The `Web3StorageApiKey` can be obtained from https://web3.storage/. Just create an account and copy the API key from the settings page.
 
 #### Repository config
 If you want to use a different configuration for each repository, just add a `config` file into the `.git/` in your repository and add the same entries as in the `~/.gitconfig` file.
 
 # Git Commands
 
 ## Git init
```

### Comparing `git3Client-0.2.5/git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/RepositoryManagement.json` & `git3Client-0.2.6/git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/RepositoryManagement.json`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/artifacts/contracts/repo_facets/GitBranch.sol/GitBranch.json` & `git3Client-0.2.6/git3Client/artifacts/contracts/repo_facets/GitBranch.sol/GitBranch.json`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/dlt/contract.py` & `git3Client-0.2.6/git3Client/dlt/contract.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/dlt/provider.py` & `git3Client-0.2.6/git3Client/dlt/provider.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/dlt/repository.py` & `git3Client-0.2.6/git3Client/dlt/repository.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/dlt/storageClient.py` & `git3Client-0.2.6/git3Client/dlt/storageClient.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import ipfshttpclient
 import json
 import requests
 
-from git3Client.config.config import WEB3_STORAGE_API_KEY
+from git3Client.utils.utils import get_value_from_config_file
 
 client = None
 
 def getStorageClient():
     """
     The getStorageClient function returns an Web3Storage object which can be used to upload and download
     files from ipfs.
 
     Returns:
         Web3Storage
     """
     global client
     if client is None:
-        client = Web3Storage(WEB3_STORAGE_API_KEY)
+        web3_storage_api_key = get_value_from_config_file('Web3StorageApiKey')
+        client = Web3Storage(web3_storage_api_key)
     return client
 
 
 class Web3Storage:
     upload_endpoint = "https://api.web3.storage/"
     retrieve_endpoint = ".ipfs.w3s.link"
```

### Comparing `git3Client-0.2.5/git3Client/git3.py` & `git3Client-0.2.6/git3Client/git3.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/add.py` & `git3Client-0.2.6/git3Client/gitCommands/add.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/branch.py` & `git3Client-0.2.6/git3Client/gitCommands/branch.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/catFile.py` & `git3Client-0.2.6/git3Client/gitCommands/catFile.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/checkout.py` & `git3Client-0.2.6/git3Client/gitCommands/checkout.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/clone.py` & `git3Client-0.2.6/git3Client/gitCommands/clone.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/commit.py` & `git3Client-0.2.6/git3Client/gitCommands/commit.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/create.py` & `git3Client-0.2.6/git3Client/gitCommands/create.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/diff.py` & `git3Client-0.2.6/git3Client/gitCommands/diff.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/fetch.py` & `git3Client-0.2.6/git3Client/gitCommands/fetch.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/hashObject.py` & `git3Client-0.2.6/git3Client/gitCommands/hashObject.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/init.py` & `git3Client-0.2.6/git3Client/gitCommands/init.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/merge.py` & `git3Client-0.2.6/git3Client/gitCommands/merge.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/pull.py` & `git3Client-0.2.6/git3Client/gitCommands/pull.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitCommands/push.py` & `git3Client-0.2.6/git3Client/gitCommands/push.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitInternals/gitCommit.py` & `git3Client-0.2.6/git3Client/gitInternals/gitCommit.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitInternals/gitIndex.py` & `git3Client-0.2.6/git3Client/gitInternals/gitIndex.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitInternals/gitObject.py` & `git3Client-0.2.6/git3Client/gitInternals/gitObject.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/gitInternals/gitTree.py` & `git3Client-0.2.6/git3Client/gitInternals/gitTree.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client/utils/utils.py` & `git3Client-0.2.6/git3Client/utils/utils.py`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client.egg-info/PKG-INFO` & `git3Client-0.2.6/git3Client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: git3Client
-Version: 0.2.5
+Version: 0.2.6
 Summary: Git3 Python client
 Home-page: https://github.com/varkiwi/git3-client
 Author: Jacek Varky
 Author-email: jaca347@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Stake to support us](https://badge.devprotocol.xyz/0xc6286Fc480Ba4d15981664a3350ABF12b0b7Feda/descriptive)](https://stakes.social/0xc6286Fc480Ba4d15981664a3350ABF12b0b7Feda)
 
 # GIT 3
@@ -61,16 +59,18 @@
 #### Gitconfig
 Here is how the contant of the `~/.gitconfig` file looks like
 ```bash
 [user]
         email = author email
         name = author name
         IdentityFile = path to private key in pem format. It has to be the absolute path! No $HOME or similar stuff in it
+        Web3StorageApiKey = APIKey
 ```
 Set the values according to your needs.
+The `Web3StorageApiKey` can be obtained from https://web3.storage/. Just create an account and copy the API key from the settings page.
 
 #### Repository config
 If you want to use a different configuration for each repository, just add a `config` file into the `.git/` in your repository and add the same entries as in the `~/.gitconfig` file.
 
 # Git Commands
 
 ## Git init
@@ -148,9 +148,7 @@
 ## How to push to PyPi
 
 In the active virtual env, execute the following: `python setup.py sdist bdist_wheel`
 This will create a dist folder. Once done, you can publish to Pypi using twine (pip3 install twine)
 `twine upload dist/*` - enter credentials and that's it. After that you should be able to install your package 
 using pip3 install [name]
 
-
-
```

### Comparing `git3Client-0.2.5/git3Client.egg-info/SOURCES.txt` & `git3Client-0.2.6/git3Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git3Client-0.2.5/git3Client.egg-info/requires.txt` & `git3Client-0.2.6/git3Client.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 bleach==5.0.0
 certifi==2020.6.20
 cffi==1.15.0
 chardet==3.0.4
 charset-normalizer==2.0.12
 commonmark==0.9.1
 cryptography==36.0.2
-cytoolz==0.11.0
+cytoolz==0.12.1
 docutils==0.18.1
 eth-abi==2.1.1
 eth-account==0.5.5
 eth-hash==0.2.0
 eth-keyfile==0.5.1
 eth-keys==0.3.3
 eth-rlp==0.2.1
```

### Comparing `git3Client-0.2.5/setup.py` & `git3Client-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     },
     data_files=[
         ('contractAbi', [
             'git3Client/artifacts/contracts/repo_facets/GitBranch.sol/GitBranch.json',
             'git3Client/artifacts/contracts/factory_facets/RepositoryManagement.sol/RepositoryManagement.json',
             ])
     ],
-    version = "0.2.5",
+    version = "0.2.6",
     description = "Git3 Python client",
     long_description = content,
     long_description_content_type="text/markdown",
     author = "Jacek Varky",
     author_email = "jaca347@gmail.com",
     install_requires=[
         'aiohttp==3.8.1',
@@ -35,15 +35,15 @@
         'bleach==5.0.0',
         'certifi==2020.6.20',
         'cffi==1.15.0',
         'chardet==3.0.4',
         'charset-normalizer==2.0.12',
         'commonmark==0.9.1',
         'cryptography==36.0.2',
-        'cytoolz==0.11.0',
+        'cytoolz==0.12.1',
         'docutils==0.18.1',
         'eth-abi==2.1.1',
         'eth-account==0.5.5',
         'eth-hash==0.2.0',
         'eth-keyfile==0.5.1',
         'eth-keys==0.3.3',
         'eth-rlp==0.2.1',
```

