# Comparing `tmp/stormware-1.1.0.tar.gz` & `tmp/stormware-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormware-1.1.0.tar", last modified: Thu Jan 26 17:47:30 2023, max compression
+gzip compressed data, was "stormware-1.2.0.tar", last modified: Tue May  9 14:58:54 2023, max compression
```

## Comparing `stormware-1.1.0.tar` & `stormware-1.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.656366 stormware-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-01-26 17:47:09.000000 stormware-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-26 17:47:09.000000 stormware-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-01-26 17:47:30.656366 stormware-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-01-26 17:47:09.000000 stormware-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-01-26 17:47:09.000000 stormware-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.652366 stormware-1.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3013 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.656366 stormware-1.1.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/extras/amazon.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/extras/facebook.txt
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-01-26 17:47:09.000000 stormware-1.1.0/requirements/extras/google.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-26 17:47:30.656366 stormware-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.656366 stormware-1.1.0/stormware/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.656366 stormware-1.1.0/stormware/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/amazon/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/amazon/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/client_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     5781 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/facebook.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.656366 stormware-1.1.0/stormware/google/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/google/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/google/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/google/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     7780 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/google/sheets.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      237 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-01-26 17:47:09.000000 stormware-1.1.0/stormware/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 17:47:30.656366 stormware-1.1.0/stormware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2405 2023-01-26 17:47:30.000000 stormware-1.1.0/stormware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-01-26 17:47:30.000000 stormware-1.1.0/stormware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-26 17:47:30.000000 stormware-1.1.0/stormware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-01-26 17:47:30.000000 stormware-1.1.0/stormware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-01-26 17:47:30.000000 stormware-1.1.0/stormware.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.975688 stormware-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-09 14:58:23.000000 stormware-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-09 14:58:23.000000 stormware-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2433 2023-05-09 14:58:54.975688 stormware-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-05-09 14:58:23.000000 stormware-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-09 14:58:23.000000 stormware-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.971688 stormware-1.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4060 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.971688 stormware-1.2.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/extras/amazon.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/extras/facebook.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-09 14:58:23.000000 stormware-1.2.0/requirements/extras/google.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 14:58:54.975688 stormware-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.975688 stormware-1.2.0/stormware/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.975688 stormware-1.2.0/stormware/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1649 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/amazon/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/amazon/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1294 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/client_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5833 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/facebook.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.975688 stormware-1.2.0/stormware/google/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/google/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/google/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/google/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/google/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-05-09 14:58:23.000000 stormware-1.2.0/stormware/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 14:58:54.975688 stormware-1.2.0/stormware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2433 2023-05-09 14:58:54.000000 stormware-1.2.0/stormware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-05-09 14:58:54.000000 stormware-1.2.0/stormware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 14:58:54.000000 stormware-1.2.0/stormware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      371 2023-05-09 14:58:54.000000 stormware-1.2.0/stormware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-09 14:58:54.000000 stormware-1.2.0/stormware.egg-info/top_level.txt
```

### Comparing `stormware-1.1.0/LICENSE.txt` & `stormware-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/PKG-INFO` & `stormware-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormware
-Version: 1.1.0
+Version: 1.2.0
 Summary: API connectors for data analysis and task automation
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -28,14 +28,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: google
 Provides-Extra: amazon
 Provides-Extra: facebook
 License-File: LICENSE.txt
```

### Comparing `stormware-1.1.0/requirements/build.txt.lock` & `stormware-1.2.0/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/requirements/dev.txt.lock` & `stormware-1.2.0/requirements/dev.txt.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,195 +1,203 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 7ed7778fe719d3f6290cc15919469dbcbf0df47a994e5c1ed5221af0b8505846
+##  Requirements hash: 9697b3785f2b249702c9e8de101b5bad7ecf8555a506cbc6df72167654d83c88
 ##
 ###################################################################################################
 -e .
-aiohttp==3.8.3
+aiohttp==3.8.4
 aiosignal==1.3.1
 alabaster==0.7.13
-astroid==2.13.3
+astroid==2.15.4
 asttokens==2.2.1
 async-timeout==4.0.2
-attrs==22.2.0
-Babel==2.11.0
+attrs==23.1.0
+Babel==2.12.1
 backcall==0.2.0
-bandit==1.7.4
-beautifulsoup4==4.11.1
+bandit==1.7.5
+beautifulsoup4==4.12.2
 bleach==6.0.0
-boto3==1.26.57
-boto3-stubs==1.26.57
-botocore==1.29.57
-botocore-stubs==1.29.57
+boto3==1.26.130
+boto3-stubs==1.26.130
+botocore==1.29.130
+botocore-stubs==1.29.130
+Bottleneck==1.3.7
 build==0.10.0
 cachetools==5.3.0
-certifi==2022.12.7
+certifi==2023.5.7
 cffi==1.15.1
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
 colorama==0.4.6
-comm==0.1.2
-coverage==7.1.0
-cryptography==39.0.0
+comm==0.1.3
+coverage==7.2.5
+cryptography==40.0.2
 curlify==2.2.1
-db-dtypes==1.0.5
-debugpy==1.6.6
+db-dtypes==1.1.1
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 dill==0.3.6
+docker==6.1.1
 docutils==0.17.1
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
 execnet==1.9.0
 executing==1.2.0
-facebook-business==15.0.2
-fastjsonschema==2.16.2
-filelock==3.9.0
+facebook-business==16.0.2
+fastjsonschema==2.16.3
+filelock==3.12.0
 frozenlist==1.3.3
 gitdb==4.0.10
-GitPython==3.1.30
+GitPython==3.1.31
 google-api-core==2.11.0
-google-api-python-client==2.74.0
-google-api-python-client-stubs==1.15.0
-google-auth==2.15.0
+google-api-python-client==2.86.0
+google-api-python-client-stubs==1.16.0
+google-auth==2.17.3
 google-auth-httplib2==0.1.0
 google-auth-stubs==0.2.0
-google-cloud-bigquery==3.4.2
+google-cloud-bigquery==3.10.0
 google-cloud-core==2.3.2
-google-cloud-secret-manager==2.15.1
+google-cloud-secret-manager==2.16.1
 google-crc32c==1.5.0
-google-resumable-media==2.4.1
-googleapis-common-protos==1.58.0
+google-resumable-media==2.5.0
+googleapis-common-protos==1.59.0
 grpc-google-iam-v1==0.12.6
-grpc-stubs==1.24.12
-grpcio==1.51.1
-grpcio-status==1.51.1
-httplib2==0.21.0
+grpc-stubs==1.53.0.2
+grpcio==1.54.0
+grpcio-status==1.54.0
+httplib2==0.22.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
-importlib-resources==5.10.2
+importlib-metadata==6.6.0
+importlib-resources==5.12.0
 iniconfig==2.0.0
-ipykernel==6.20.2
-ipython==8.8.0
-ipywidgets==8.0.4
-isort==5.11.4
+ipykernel==6.23.0
+ipython==8.12.2
+ipywidgets==8.0.6
+isort==5.12.0
 jaraco.classes==3.2.3
 jedi==0.18.2
 jeepney==0.8.0
 Jinja2==3.1.2
 jmespath==1.0.1
 jsonschema==4.17.3
 jupyter-sphinx==0.4.0
-jupyter_client==8.0.0
-jupyter_core==5.1.5
+jupyter_client==8.2.0
+jupyter_core==5.3.0
 jupyterlab-pygments==0.2.2
-jupyterlab-widgets==3.0.5
+jupyterlab-widgets==3.0.7
 keyring==23.13.1
 lazy-object-proxy==1.9.0
+llvmlite==0.40.0
 logikal-docs==1.1.3
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 matplotlib-inline==0.1.6
 mccabe==0.7.0
 mdurl==0.1.2
-mistune==2.0.4
-more-itertools==9.0.0
+mistune==2.0.5
+more-itertools==9.1.0
 multidict==6.0.4
-mypy==0.991
-mypy-extensions==0.4.3
-nbclient==0.7.2
-nbconvert==7.2.9
-nbformat==5.7.3
+mypy==1.2.0
+mypy-extensions==1.0.0
+nbclient==0.7.4
+nbconvert==7.4.0
+nbformat==5.8.0
 nest-asyncio==1.5.6
-numpy==1.24.1
-packaging==23.0
-pandas==1.5.3
-pandas-stubs==1.5.2.230105
+numba==0.57.0
+numexpr==2.8.4
+numpy==1.24.3
+packaging==23.1
+pandas==2.0.1
+pandas-stubs==2.0.1.230501
 pandocfilters==1.5.0
 parso==0.8.3
 pbr==5.11.1
 pexpect==4.8.0
 pickleshare==0.7.5
-Pillow==9.4.0
-pip==22.3.1
-pip-licenses==4.0.3
+Pillow==9.5.0
+pip==23.1.2
+pip-licenses==4.3.1
 pkginfo==1.9.6
 pkgutil_resolve_name==1.3.10
-platformdirs==2.6.2
+platformdirs==3.5.0
 pluggy==1.0.0
-prettytable==3.6.0
-prompt-toolkit==3.0.36
+prettytable==3.7.0
+prompt-toolkit==3.0.38
 proto-plus==1.22.2
-protobuf==4.21.12
-psutil==5.9.4
+protobuf==4.23.0
+psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pyarrow==10.0.1
-pyasn1==0.4.8
-pyasn1-modules==0.2.8
+pyarrow==12.0.0
+pyasn1==0.5.0
+pyasn1-modules==0.3.0
 pycodestyle==2.10.0
 pycountry==22.3.5
 pycparser==2.21
 pydocstyle==6.3.0
-Pygments==2.14.0
-pylint==2.15.10
-pyorbs==1.6.1
+Pygments==2.15.1
+pylint==2.17.4
+pyorbs==2.0.0
 pyparsing==3.0.9
 pyproject_hooks==1.0.0
 pyrsistent==0.19.3
-pytest==7.2.1
+pytest==7.3.1
 pytest-cov==4.0.0
-pytest-logikal==1.4.0
+pytest-logikal==1.8.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.1.0
+pytest-xdist==3.2.1
 python-dateutil==2.8.2
-pytz==2022.7.1
+pytz==2023.3
 PyYAML==6.0
-pyzmq==25.0.0
+pyzmq==25.0.2
 readme-renderer==37.3
-requests==2.28.2
-requests-toolbelt==0.10.1
+requests==2.30.0
+requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.2.0
+rich==13.3.5
 rsa==4.9
-s3transfer==0.6.0
+s3transfer==0.6.1
 SecretStorage==3.3.3
-setuptools==44.0.0
+setuptools==67.7.2
 six==1.16.0
 smmap==5.0.0
 snowballstemmer==2.2.0
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.2
-stevedore==4.1.1
+stevedore==5.0.0
+termcolor==2.3.0
 tinycss2==1.2.1
 tomli==2.0.1
-tomlkit==0.11.6
-tornado==6.2
-traitlets==5.8.1
+tomlkit==0.11.8
+tornado==6.3.1
+traitlets==5.9.0
 twine==4.0.2
-types-awscrt==0.16.4
-types-pytz==2022.7.1.0
-types-requests==2.28.11.8
-types-s3transfer==0.6.0.post5
-types-urllib3==1.26.25.4
-typing_extensions==4.4.0
+types-awscrt==0.16.17
+types-pytz==2023.3.0.0
+types-requests==2.30.0.0
+types-s3transfer==0.6.1
+types-urllib3==1.26.25.12
+typing_extensions==4.5.0
+tzdata==2023.3
 uritemplate==4.1.1
-urllib3==1.26.14
+urllib3==1.26.15
 wcwidth==0.2.6
 webencodings==0.5.1
-wheel==0.38.4
-widgetsnbextension==4.0.5
-wrapt==1.14.1
+websocket-client==1.5.1
+wheel==0.40.0
+widgetsnbextension==4.0.7
+wrapt==1.15.0
 xdg==5.1.1
-yarl==1.8.2
-zipp==3.11.0
+yarl==1.9.2
+zipp==3.15.0
```

### Comparing `stormware-1.1.0/requirements/docs.txt.lock` & `stormware-1.2.0/requirements/docs.txt.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,141 +1,146 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: d743aaa3580df6a8e5da9bff340e968afa3b91428493ff28f748bba48df156ef
+##  Requirements hash: 51ecc1433b894dec2e1e8881da55c84989d5f0b8ea0549d2262e1158e19920a4
 ##
 ###################################################################################################
 -e .
-aiohttp==3.8.3
+aiohttp==3.8.4
 aiosignal==1.3.1
 alabaster==0.7.13
 asttokens==2.2.1
 async-timeout==4.0.2
-attrs==22.2.0
-Babel==2.11.0
+attrs==23.1.0
+Babel==2.12.1
 backcall==0.2.0
-beautifulsoup4==4.11.1
+beautifulsoup4==4.12.2
 bleach==6.0.0
-boto3==1.26.57
-boto3-stubs==1.26.57
-botocore==1.29.57
-botocore-stubs==1.29.57
+boto3==1.26.130
+boto3-stubs==1.26.130
+botocore==1.29.130
+botocore-stubs==1.29.130
+Bottleneck==1.3.7
 cachetools==5.3.0
-certifi==2022.12.7
-charset-normalizer==2.1.1
-comm==0.1.2
+certifi==2023.5.7
+charset-normalizer==3.1.0
+comm==0.1.3
 curlify==2.2.1
-db-dtypes==1.0.5
-debugpy==1.6.6
+db-dtypes==1.1.1
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 docutils==0.17.1
 executing==1.2.0
-facebook-business==15.0.2
-fastjsonschema==2.16.2
+facebook-business==16.0.2
+fastjsonschema==2.16.3
 frozenlist==1.3.3
 google-api-core==2.11.0
-google-api-python-client==2.74.0
-google-api-python-client-stubs==1.15.0
-google-auth==2.15.0
+google-api-python-client==2.86.0
+google-api-python-client-stubs==1.16.0
+google-auth==2.17.3
 google-auth-httplib2==0.1.0
 google-auth-stubs==0.2.0
-google-cloud-bigquery==3.4.2
+google-cloud-bigquery==3.10.0
 google-cloud-core==2.3.2
-google-cloud-secret-manager==2.15.1
+google-cloud-secret-manager==2.16.1
 google-crc32c==1.5.0
-google-resumable-media==2.4.1
-googleapis-common-protos==1.58.0
+google-resumable-media==2.5.0
+googleapis-common-protos==1.59.0
 grpc-google-iam-v1==0.12.6
-grpc-stubs==1.24.12
-grpcio==1.51.1
-grpcio-status==1.51.1
-httplib2==0.21.0
+grpc-stubs==1.53.0.2
+grpcio==1.54.0
+grpcio-status==1.54.0
+httplib2==0.22.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
-importlib-resources==5.10.2
-ipykernel==6.20.2
-ipython==8.8.0
-ipywidgets==8.0.4
+importlib-metadata==6.6.0
+importlib-resources==5.12.0
+ipykernel==6.23.0
+ipython==8.12.2
+ipywidgets==8.0.6
 jedi==0.18.2
 Jinja2==3.1.2
 jmespath==1.0.1
 jsonschema==4.17.3
 jupyter-sphinx==0.4.0
-jupyter_client==8.0.0
-jupyter_core==5.1.5
+jupyter_client==8.2.0
+jupyter_core==5.3.0
 jupyterlab-pygments==0.2.2
-jupyterlab-widgets==3.0.5
+jupyterlab-widgets==3.0.7
+llvmlite==0.40.0
 logikal-docs==1.1.3
 MarkupSafe==2.1.2
 matplotlib-inline==0.1.6
-mistune==2.0.4
+mistune==2.0.5
 multidict==6.0.4
-nbclient==0.7.2
-nbconvert==7.2.9
-nbformat==5.7.3
+nbclient==0.7.4
+nbconvert==7.4.0
+nbformat==5.8.0
 nest-asyncio==1.5.6
-numpy==1.24.1
-packaging==23.0
-pandas==1.5.3
-pandas-stubs==1.5.2.230105
+numba==0.57.0
+numexpr==2.8.4
+numpy==1.24.3
+packaging==23.1
+pandas==2.0.1
+pandas-stubs==2.0.1.230501
 pandocfilters==1.5.0
 parso==0.8.3
 pexpect==4.8.0
 pickleshare==0.7.5
-pip==22.3.1
+pip==23.1.2
 pkgutil_resolve_name==1.3.10
-platformdirs==2.6.2
-prompt-toolkit==3.0.36
+platformdirs==3.5.0
+prompt-toolkit==3.0.38
 proto-plus==1.22.2
-protobuf==4.21.12
-psutil==5.9.4
+protobuf==4.23.0
+psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pyarrow==10.0.1
-pyasn1==0.4.8
-pyasn1-modules==0.2.8
+pyarrow==12.0.0
+pyasn1==0.5.0
+pyasn1-modules==0.3.0
 pycountry==22.3.5
-Pygments==2.14.0
+Pygments==2.15.1
 pyparsing==3.0.9
 pyrsistent==0.19.3
 python-dateutil==2.8.2
-pytz==2022.7.1
-pyzmq==25.0.0
-requests==2.28.2
+pytz==2023.3
+pyzmq==25.0.2
+requests==2.30.0
 rsa==4.9
-s3transfer==0.6.0
-setuptools==44.0.0
+s3transfer==0.6.1
+setuptools==67.7.2
 six==1.16.0
 snowballstemmer==2.2.0
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.2
 tinycss2==1.2.1
 tomli==2.0.1
-tornado==6.2
-traitlets==5.8.1
-types-awscrt==0.16.4
-types-pytz==2022.7.1.0
-types-requests==2.28.11.8
-types-s3transfer==0.6.0.post5
-types-urllib3==1.26.25.4
-typing_extensions==4.4.0
+tornado==6.3.1
+traitlets==5.9.0
+types-awscrt==0.16.17
+types-pytz==2023.3.0.0
+types-requests==2.30.0.0
+types-s3transfer==0.6.1
+types-urllib3==1.26.25.12
+typing_extensions==4.5.0
+tzdata==2023.3
 uritemplate==4.1.1
-urllib3==1.26.14
+urllib3==1.26.15
 wcwidth==0.2.6
 webencodings==0.5.1
-wheel==0.38.4
-widgetsnbextension==4.0.5
+wheel==0.40.0
+widgetsnbextension==4.0.7
 xdg==5.1.1
-yarl==1.8.2
-zipp==3.11.0
+yarl==1.9.2
+zipp==3.15.0
```

### Comparing `stormware-1.1.0/stormware/amazon/auth.py` & `stormware-1.2.0/stormware/amazon/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,21 @@
         if credentials.exists():
             config = ConfigParser()
             config.read(credentials)
             self.profiles = set(config.sections())
         else:
             logger.debug(f'Named profile credentials file "{credentials}" does not exist')
 
-    def session(self, organization: Optional[str] = None, region: Optional[str] = None) -> Session:
+    def profile(self, organization: Optional[str] = None) -> Optional[str]:
         """
-        Return a session that uses the organization ID named profile credentials (if it exists).
+        Return the profile name (same as the organization ID) or :data:`None` if it does not exist.
         """
         organization_id = self.organization_id(organization=organization)
-        profile = organization_id if organization_id in self.profiles else None
-        if profile:
+        if (profile := organization_id if organization_id in self.profiles else None):
             logger.debug(f'Using named profile "{profile}"')
-        return Session(profile_name=profile, region_name=region)
+        return profile
+
+    def session(self, organization: Optional[str] = None, region: Optional[str] = None) -> Session:
+        """
+        Return a session that uses named profile credentials (if it exists).
+        """
+        return Session(profile_name=self.profile(organization=organization), region_name=region)
```

### Comparing `stormware-1.1.0/stormware/amazon/secrets.py` & `stormware-1.2.0/stormware/amazon/secrets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/stormware/auth.py` & `stormware-1.2.0/stormware/auth.py`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/stormware/client_manager.py` & `stormware-1.2.0/stormware/client_manager.py`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/stormware/facebook.py` & `stormware-1.2.0/stormware/facebook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Facebook API connector.
 
 Documentation:
 - Python Business SDK: https://github.com/facebook/facebook-python-business-sdk
 - Marketing API: https://developers.facebook.com/docs/marketing-apis
+- Changelog: https://developers.facebook.com/docs/graph-api/changelog
 
 """
 import json
 from logging import getLogger
 from typing import Any, Dict, List, Mapping, Optional
 
 import pandas as pd
@@ -57,16 +58,15 @@
         accounts = user.get_assigned_ad_accounts(fields=['id', 'name'])
         self.ad_accounts: Dict[str, str] = {account['name']: account['id'] for account in accounts}
 
     def account_id(self, account_name: Optional[str] = None) -> str:
         """
         Return the account ID for a given account name.
         """
-        account_name = account_name or self.account_name
-        if not account_name:
+        if not (account_name := account_name or self.account_name):
             raise ValueError('You must specify the account')
         if account_name not in self.ad_accounts:
             raise RuntimeError(f'Account "{account_name}" not found in your accounts')
         return self.ad_accounts[account_name]
 
     def report(  # pylint: disable=too-many-arguments
         self, metrics: List[str], dimensions: Optional[List[str]] = None,
```

### Comparing `stormware-1.1.0/stormware/google/auth.py` & `stormware-1.2.0/stormware/google/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     def project(self, project: Optional[str] = None) -> str:
         """
         Return the project name.
 
         Defaults to the ``project`` value set in ``pyproject.toml`` under the ``tool.stormware``
         section.
         """
-        project = project or self._project or STORMWARE_CONFIG.get('project')
-        if not project:
+        if not (project := project or self._project or STORMWARE_CONFIG.get('project')):
             raise ValueError('You must provide a project')
         return project
 
     def project_id(self, organization: Optional[str] = None, project: Optional[str] = None) -> str:
         """
         Return the project ID.
```

### Comparing `stormware-1.1.0/stormware/google/bigquery.py` & `stormware-1.2.0/stormware/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/stormware/google/secrets.py` & `stormware-1.2.0/stormware/google/secrets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/stormware/google/sheets.py` & `stormware-1.2.0/stormware/google/sheets.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,15 +110,16 @@
         updates.append(self._format(
             {'textFormat': {'bold': True}, 'wrapStrategy': 'WRAP'},
             sheet_id=sheet_id, start_row=0, end_row=1,
         ))
 
         # Data formatting and update
         for index, (column, data_type) in enumerate(data.dtypes.items()):
-            column = cast(str, column)  # looks like the type is derived incorrectly, we must cast
+            # Type is derived incorrectly, we must cast
+            column = cast(str, column)  # pylint: disable=redefined-loop-name
             sheet_range = {'sheet_id': sheet_id, 'start_column': index, 'end_column': index + 1}
             updates.append(self._format(
                 {'horizontalAlignment': 'RIGHT' if types.is_numeric_dtype(data_type) else 'LEFT'},
                 **sheet_range,
             ))
             if types.is_integer_dtype(data_type):
                 updates.append(self._format(
@@ -127,23 +128,24 @@
             elif types.is_float_dtype(data_type):
                 updates.append(self._format(
                     {'numberFormat': {'pattern': '#,##0.00', 'type': 'NUMBER'}}, **sheet_range,
                 ))
             elif types.is_object_dtype(data_type):
                 first_index = data[column].first_valid_index()
                 first_value = data[column].loc[first_index] if first_index is not None else None
-                if isinstance(first_value, date):
-                    data[column] = data[column].apply(
-                        lambda value: value.strftime('%Y-%m-%d')  # type: ignore[no-any-return]
-                    )
+                data[column] = data[column].apply(
+                    lambda value: value.strftime('%Y-%m-%d')  # type: ignore[no-any-return]
+                ) if isinstance(first_value, date) else data[column]
             elif types.is_datetime64_ns_dtype(data_type):
-                if ((data[column].dt.microsecond == 0) | (data[column].isnull())).all():
-                    data[column] = data[column].dt.strftime('%Y-%m-%d %H:%M:%S')
-                else:
-                    data[column] = data[column].dt.strftime('%Y-%m-%d %H:%M:%S.%f')
+                no_microseconds = (
+                    (data[column].dt.microsecond == 0)  # pylint: disable=compare-to-zero
+                    | (data[column].isnull())
+                )
+                microseconds = '.%f' if not no_microseconds.all() else ''
+                data[column] = data[column].dt.strftime(f'%Y-%m-%d %H:%M:%S{microseconds}')
 
         logger.info(f'Updating sheet "{name}"')
         self.update(updates)
         self.update_values(name, data)
 
         # Resizing columns
         # Note: the header row text sometimes overflows due to the bold formatting
```

### Comparing `stormware-1.1.0/stormware/secrets.py` & `stormware-1.2.0/stormware/secrets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.1.0/stormware.egg-info/PKG-INFO` & `stormware-1.2.0/stormware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormware
-Version: 1.1.0
+Version: 1.2.0
 Summary: API connectors for data analysis and task automation
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -28,14 +28,15 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: google
 Provides-Extra: amazon
 Provides-Extra: facebook
 License-File: LICENSE.txt
```

### Comparing `stormware-1.1.0/stormware.egg-info/SOURCES.txt` & `stormware-1.2.0/stormware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

