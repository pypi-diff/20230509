# Comparing `tmp/pulumi_kafka-3.5.0a1683325558.tar.gz` & `tmp/pulumi_kafka-3.5.0a1683612894.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.5.0a1683325558.tar", last modified: Fri May  5 22:29:58 2023, max compression
+gzip compressed data, was "pulumi_kafka-3.5.0a1683612894.tar", last modified: Tue May  9 06:24:53 2023, max compression
```

## Comparing `pulumi_kafka-3.5.0a1683325558.tar` & `pulumi_kafka-3.5.0a1683612894.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:29:58.765177 pulumi_kafka-3.5.0a1683325558/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-05 22:29:58.765177 pulumi_kafka-3.5.0a1683325558/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:29:58.765177 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:29:58.765177 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 22:29:58.765177 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 22:29:58.765177 pulumi_kafka-3.5.0a1683325558/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-05 22:29:58.000000 pulumi_kafka-3.5.0a1683325558/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:53.950840 pulumi_kafka-3.5.0a1683612894/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-09 06:24:53.950840 pulumi_kafka-3.5.0a1683612894/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:53.950840 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23125 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:53.950840 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:24:53.950840 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 06:24:53.950840 pulumi_kafka-3.5.0a1683612894/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-09 06:24:53.000000 pulumi_kafka-3.5.0a1683612894/setup.py
```

### Comparing `pulumi_kafka-3.5.0a1683325558/PKG-INFO` & `pulumi_kafka-3.5.0a1683612894/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.5.0a1683325558
+Version: 3.5.0a1683612894
 Summary: A Pulumi package for creating and managing Kafka.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi kafka
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.5.0a1683325558/README.md` & `pulumi_kafka-3.5.0a1683612894/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/__init__.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/acl.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/provider.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/quota.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka/topic.py` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-kafka
-Version: 3.5.0a1683325558
+Version: 3.5.0a1683612894
 Summary: A Pulumi package for creating and managing Kafka.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi kafka
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.5.0a1683325558/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.5.0a1683612894/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.5.0a1683325558/setup.py` & `pulumi_kafka-3.5.0a1683612894/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.5.0a1683325558"
-PLUGIN_VERSION = "3.5.0-alpha.1683325558+c246514b"
+VERSION = "3.5.0a1683612894"
+PLUGIN_VERSION = "3.5.0-alpha.1683612894+9a6dc941"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'kafka', PLUGIN_VERSION])
         except OSError as error:
```

