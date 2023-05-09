# Comparing `tmp/plone.recipe.zeoserver-2.0.3.tar.gz` & `tmp/plone.recipe.zeoserver-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.recipe.zeoserver-2.0.3.tar", last modified: Thu Aug 13 23:18:56 2020, max compression
+gzip compressed data, was "plone.recipe.zeoserver-3.0.0.tar", last modified: Tue May  9 19:33:33 2023, max compression
```

## Comparing `plone.recipe.zeoserver-2.0.3.tar` & `plone.recipe.zeoserver-3.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/
--rw-r--r--   0 maurits    (501) staff       (20)    19304 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      193 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     2122 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      129 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     7589 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6101 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/CHANGES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    19304 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       19 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      911 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       62 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       92 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/dependency_links.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/src/plone/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/
--rw-r--r--   0 maurits    (501) staff       (20)      268 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/
--rw-r--r--   0 maurits    (501) staff       (20)     2177 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/pack.py
--rw-r--r--   0 maurits    (501) staff       (20)      287 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/runzeo.bat
--rw-r--r--   0 maurits    (501) staff       (20)     1119 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/ctl.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:56.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     1586 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/tests/test_docs.py
--rw-r--r--   0 maurits    (501) staff       (20)       26 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    15957 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/tests/zeoserver.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4217 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/zeoservice.py.in
--rw-r--r--   0 maurits    (501) staff       (20)    20489 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/recipe.py
--rw-r--r--   0 maurits    (501) staff       (20)      268 2020-08-13 23:18:55.000000 plone.recipe.zeoserver-2.0.3/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.121877 plone.recipe.zeoserver-3.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     6383 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      193 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    15149 2023-05-09 19:33:33.121994 plone.recipe.zeoserver-3.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     7707 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2858 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-05-09 19:33:33.122458 plone.recipe.zeoserver-3.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1768 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.113240 plone.recipe.zeoserver-3.0.0/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.116044 plone.recipe.zeoserver-3.0.0/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.118986 plone.recipe.zeoserver-3.0.0/src/plone/recipe/
+-rw-r--r--   0 maurits    (501) staff       (20)      245 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.120761 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1057 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/ctl.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2259 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/pack.py
+-rw-r--r--   0 maurits    (501) staff       (20)    20249 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/recipe.py
+-rw-r--r--   0 maurits    (501) staff       (20)      287 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/runzeo.bat
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.121559 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1435 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/tests/test_docs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    16620 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/tests/zeoserver.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4217 2023-05-09 19:33:32.000000 plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/zeoservice.py.in
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-09 19:33:33.118550 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    15149 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      911 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       19 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       98 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-05-09 19:33:33.000000 plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.recipe.zeoserver-2.0.3/setup.py` & `plone.recipe.zeoserver-3.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,54 @@
-# -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
-import sys
 
-
-version = '2.0.3'
-
-additional_install_requires = []
-
-if sys.platform[:3].lower() == 'win':
-    additional_install_requires += ['nt_svcutils']
+version = "3.0.0"
 
 
 setup(
     name="plone.recipe.zeoserver",
     version=version,
-    author='Hanno Schlichting',
-    author_email='hannosch@plone.org',
-    description='ZC Buildout recipe for installing a ZEO server',
-    long_description=(
-        open('README.rst').read() +
-        '\n' +
-        open('CHANGES.rst').read()
-    ),
-    license='ZPL 2.1',
-    keywords='zope2 zeo zodb buildout',
-    url='https://github.com/plone/plone.recipe.zeoserver',
-    download_url='https://pypi.org/project/plone.recipe.zeoserver',
+    author="Hanno Schlichting",
+    author_email="hannosch@plone.org",
+    description="ZC Buildout recipe for installing a ZEO server",
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
+    license="ZPL 2.1",
+    keywords="zope2 zeo zodb buildout",
+    url="https://github.com/plone/plone.recipe.zeoserver",
+    download_url="https://pypi.org/project/plone.recipe.zeoserver",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: Zope Public License',
-        'Framework :: Buildout',
-        'Framework :: Plone',
-        'Framework :: Plone :: 5.1',
-        'Framework :: Plone :: 5.2',
-        'Framework :: Plone :: Core',
-        'Framework :: Zope',
-        'Framework :: Zope :: 4',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: Implementation',
-        'Programming Language :: Python :: Implementation :: CPython',
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: Zope Public License",
+        "Framework :: Buildout",
+        "Framework :: Plone",
+        "Framework :: Plone :: 6.0",
+        "Framework :: Zope",
+        "Framework :: Zope :: 5",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: Implementation",
+        "Programming Language :: Python :: Implementation :: CPython",
     ],
-    packages=find_packages('src'),
+    python_requires=">=3.8",
+    packages=find_packages("src"),
     include_package_data=True,
-    package_dir={'': 'src'},
-    namespace_packages=['plone', 'plone.recipe'],
+    package_dir={"": "src"},
+    namespace_packages=["plone", "plone.recipe"],
     install_requires=[
-        'setuptools',
-        'zc.buildout',
-        'zc.recipe.egg',
-        'ZODB >= 5',
-        'zope.mkzeoinstance >=4.1',
-        'ZopeUndo',
-    ] + additional_install_requires,
-    extras_require={
-        'zrs': ['zc.zrs']
-    },
+        "setuptools",
+        "zc.buildout",
+        "zc.recipe.egg",
+        "ZEO",
+        "ZODB >= 5",
+        "zope.mkzeoinstance >= 5.1.1",
+        "ZopeUndo",
+    ],
+    extras_require={"zrs": ["zc.zrs"]},
     zip_safe=False,
     entry_points={
-        'zc.buildout': ['default = plone.recipe.zeoserver.recipe:Recipe'],
+        "zc.buildout": ["default = plone.recipe.zeoserver.recipe:Recipe"],
     },
 )
```

### Comparing `plone.recipe.zeoserver-2.0.3/README.rst` & `plone.recipe.zeoserver-3.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -235,12 +235,19 @@
   will be called the name you specify. If you'd like to use this script to pack
   a different mount point, you'll need to specify `-S mount_name`. You can also
   specify a `-B` option to not use the default blob directory.
   You may override the pack-days by adding "-D #" to the command line where
   "#" is the number of days to keep.
 
 
+Version Information
+-------------------
+
+- 3.x -> Plone 6, Zope 5, Python 3.8+
+- 2.x -> Plone 5, Zope 4, Python 2.7
+
+
 Reporting bugs or asking questions
 ----------------------------------
 
 We have a bugtracker and help desk on Github:
 https://github.com/plone/plone.recipe.zeoserver/issues
```

### Comparing `plone.recipe.zeoserver-2.0.3/CHANGES.rst` & `plone.recipe.zeoserver-3.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.0 (2023-05-09)
+------------------
+
+Breaking changes:
+
+
+- Update Codebase to python 3.8+.
+  Update required version ``zope.mkzeoinstance = 5.1.1``.
+  [petschki] (#45)
+
+
+Bug fixes:
+
+
+- Fix lost dependencies when defining additional ``eggs`` in buildout part.
+  [petschki] (#45)
+
+
 2.0.3 (2020-08-14)
 ------------------
 
 Bug fixes:
 
 
 - Removing ZODB3_HOME variable from runzeo.bat and zeoservice.py.in files, Fix for windows machine (#41)
```

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone.recipe.zeoserver.egg-info/SOURCES.txt` & `plone.recipe.zeoserver-3.0.0/src/plone.recipe.zeoserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/pack.py` & `plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/pack.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-# -*- coding: utf-8 -*-
 from ZEO.ClientStorage import ClientStorage
 from ZEO.Exceptions import ClientDisconnected
 
 import logging
 import os
 import socket
 import sys
 import time
 
 
-def _main(host, port, unix=None, days=1, username=None, password=None,
-          realm=None, blob_dir=None, storage='1', shared_blob_dir=True):
+def _main(
+    host,
+    port,
+    unix=None,
+    days=1,
+    username=None,
+    password=None,
+    realm=None,
+    blob_dir=None,
+    storage="1",
+    shared_blob_dir=True,
+):
     if unix is not None:
         addr = unix
     else:
         if host is None:
             host = socket.gethostname()
         addr = host, int(port)
 
@@ -23,47 +32,54 @@
 
     cs = None
     logger = logging.getLogger(__name__)
     try:
         # We do not want to wait until a zeoserver is up and running; it
         # should already be running, so wait=False
         cs = ClientStorage(
-            addr, storage=storage, wait=False, read_only=True,
-            username=username, password=password, realm=realm,
-            blob_dir=blob_dir, shared_blob_dir=shared_blob_dir,
+            addr,
+            storage=storage,
+            wait=False,
+            read_only=True,
+            username=username,
+            password=password,
+            realm=realm,
+            blob_dir=blob_dir,
+            shared_blob_dir=shared_blob_dir,
         )
         for i in range(60):
             if cs.is_connected():
                 break
             time.sleep(1)
         else:
-            logger.error("Could not connect to zeoserver. Please make sure it "
-                         "is running.")
+            logger.error(
+                "Could not connect to zeoserver. Please make sure it " "is running."
+            )
             cs.close()
             sys.exit(1)
         try:
             # The script should not exit until the packing is done.
             # => wait=True
             cs.pack(wait=True, days=int(days))
         except ClientDisconnected:
-            logger.error("Disconnected from zeoserver. Please make sure it "
-                         "is still running.")
+            logger.error(
+                "Disconnected from zeoserver. Please make sure it " "is still running."
+            )
             sys.exit(1)
     finally:
         if cs is not None:
             cs.close()
 
 
 def main(*args, **kw):
     root_logger = logging.getLogger()
     old_level = root_logger.getEffectiveLevel()
     logging.getLogger().setLevel(logging.WARNING)
     handler = logging.StreamHandler(sys.stdout)
-    handler.setFormatter(logging.Formatter(
-        "%(name)s %(levelname)s %(message)s"))
+    handler.setFormatter(logging.Formatter("%(name)s %(levelname)s %(message)s"))
     logging.getLogger().addHandler(handler)
     try:
         _main(*args, **kw)
     finally:
         logging.getLogger().setLevel(old_level)
         logging.getLogger().removeHandler(handler)
```

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/ctl.py` & `plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/ctl.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# -*- coding: utf-8 -*-
 """zeocltl -- control a ZEO server using zdaemon.
 
 Usage: zeocltl [options] [action [arguments]]
 
 Options:
 -h/--help -- print usage message and exit
 
 Actions are commands like "start", "stop" and "status". If -i is specified or
 no action is specified on the command line, a "shell" interpreting actions
 typed interactively is started. Use the action "help" to find out about
 available actions. """
-from __future__ import print_function
 
 from ZEO import runzeo
 from ZEO import zeoctl
 
 import os
 import sys
 
 
 if sys.platform[:3].lower() == "win":
-    print('For win32 platforms, runzeo.bat or zeoservice.exe should be used')
-    print('%s is based on zdaemon, which is Linux specific' % sys.argv[0])
-    print('Aborting...')
+    print("For win32 platforms, runzeo.bat or zeoservice.exe should be used")
+    print("%s is based on zdaemon, which is Linux specific" % sys.argv[0])
+    print("Aborting...")
     sys.exit(0)
 
 
 def main(args=None):
     # When we detect Supervisord we need to make sure we do not fork a
     # sub process since Supervisord does not like that
-    if 'SUPERVISOR_ENABLED' in os.environ:
+    if "SUPERVISOR_ENABLED" in os.environ:
         # We will ignore any command sent and always start in foreground mode
         args = args[:2]
         runzeo.main(args)
     else:
         zeoctl.main(args)
```

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/tests/test_docs.py` & `plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/tests/test_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,52 @@
-# -*- coding: utf-8 -*-
-
 from zc.buildout.testing import buildoutSetUp
 from zc.buildout.testing import buildoutTearDown
 from zc.buildout.testing import install
 from zc.buildout.testing import install_develop
 
 import doctest
 import pkg_resources
 import shutil
-import sys
 import unittest
 
 
 def setUp(test):
     buildoutSetUp(test)
-    install_develop('plone.recipe.zeoserver', test)
-    install('zc.recipe.egg', test)
-    if sys.platform[:3].lower() == "win":
-        install('nt_svcutils', test)
-    install('zope.mkzeoinstance', test)
-    install('ZopeUndo', test)
-    install('zc.zrs', test)
-    install('Automat', test)
-    install('incremental', test)
-    install('constantly', test)
-    install('attrs', test)
-    install('Twisted', test)
-    install('hyperlink', test)
-    install('idna', test)
-    install('PyHamcrest', test)
-    dependencies = pkg_resources.working_set.require('ZODB')
+    install_develop("plone.recipe.zeoserver", test)
+    install("zc.recipe.egg", test)
+    install("zope.mkzeoinstance", test)
+    install("ZopeUndo", test)
+    install("zc.zrs", test)
+    install("Automat", test)
+    install("incremental", test)
+    install("constantly", test)
+    install("attrs", test)
+    install("Twisted", test)
+    install("hyperlink", test)
+    install("idna", test)
+    dependencies = pkg_resources.working_set.require("ZODB")
     for dep in dependencies:
         try:
             install(dep.project_name, test)
         except OSError:
             # Some distributions are installed multiple times, and the
             # underlying API doesn't check for it
             pass
 
 
 def tearDown(test):
     buildoutTearDown(test)
-    sample_buildout = test.globs['sample_buildout']
+    sample_buildout = test.globs["sample_buildout"]
     shutil.rmtree(sample_buildout, ignore_errors=True)
 
 
 def test_suite():
     suite = []
-    flags = (doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE)
+    flags = doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
 
-    suite.append(doctest.DocFileSuite('zeoserver.txt', optionflags=flags,
-                                      setUp=setUp, tearDown=buildoutTearDown))
+    suite.append(
+        doctest.DocFileSuite(
+            "zeoserver.txt", optionflags=flags, setUp=setUp, tearDown=buildoutTearDown
+        )
+    )
 
     return unittest.TestSuite(suite)
```

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/tests/zeoserver.txt` & `plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/tests/zeoserver.txt`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,16 @@
     Uninstalling zeo.
     Installing zeo...
 
 We should have a zeo.conf with log file rotation enabled::
 
     >>> zeo = os.path.join(sample_buildout, 'parts', 'zeo')
     >>> with open(os.path.join(zeo, 'etc', 'zeo.conf')) as f:
-    ...     print(f.read())
+    ...     output = f.read()
+    >>> print(output.replace('\\', '/'))
     %define INSTANCE ...
     ...
     <eventlog>
       level info
       <logfile>
         path .../sample-buildout/var/log/zeo.log
         format %(asctime)s %(message)s
@@ -470,15 +471,15 @@
 
 Check the files are actually different by comparing different settings. The given usernames should
 be different and correspond as the buildout specified::
 
     >>> zeopack_scripts = ('first-zeopack', 'second-zeopack')
     >>> zeopack_paths = [os.path.join(sample_buildout, 'bin', script) for script in zeopack_scripts]
     >>> if WINDOWS:
-    ...     zeopack_paths =  [zeopack + '-script.py' for zeopack in zeopacks]
+    ...     zeopack_paths =  [zeopack + '-script.py' for zeopack in zeopack_paths]
     >>> with open(zeopack_paths[0], 'r') as f:
     ...     first_zeopack = f.read()
     >>> with open(zeopack_paths[1], 'r') as f:
     ...     second_zeopack = f.read()
     >>> 'username = "firstuser"' in first_zeopack
     True
     >>> 'username = "seconduser"' in first_zeopack
@@ -628,7 +629,34 @@
     ...     suffix = '-script.py'
     ... else:
     ...     suffix = ''
 
     >>> with open(join('bin', 'zeo' + suffix)) as f:
     ...     'foo = 1' in f.read()
     True
+
+Additional eggs
+===============
+
+The recipe support additional eggs.
+
+    >>> write('buildout.cfg',
+    ... '''
+    ... [buildout]
+    ... parts = zeo
+    ... find-links = %(sample_buildout)s/eggs
+    ...
+    ... [zeo]
+    ... recipe = plone.recipe.zeoserver
+    ... zeo-address = /path/to/zeo.socket
+    ... eggs = ZEO
+    ... ''' % globals())
+    >>> print(system(join('bin', 'buildout'))),
+    Uninstalling zeo.
+    Installing zeo.
+    ...
+
+The main script should have the initialization.
+
+    >>> with open(join('parts', 'zeo', 'bin', 'zeoctl')) as f:
+    ...     'plone.recipe.zeoserver' in f.read()
+    True
```

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/zeoservice.py.in` & `plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/zeoservice.py.in`

 * *Files identical despite different names*

### Comparing `plone.recipe.zeoserver-2.0.3/src/plone/recipe/zeoserver/recipe.py` & `plone.recipe.zeoserver-3.0.0/src/plone/recipe/zeoserver/recipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,499 +1,512 @@
-# -*- coding: utf-8 -*-
 import logging
 import os
 import shutil
 import sys
 import zc.buildout
 import zc.recipe.egg
 
 
 try:
     import zc.zrs
+
     HAS_ZRS = True
 except ImportError:
     HAS_ZRS = False
 join = os.path.join
 
 curdir = os.path.dirname(__file__)
 
 
-class Recipe(object):
-
+class Recipe:
     def __init__(self, buildout, name, options):
-        self.egg = zc.recipe.egg.Egg(buildout, options['recipe'], options)
+        self.egg = zc.recipe.egg.Egg(buildout, options["recipe"], options)
         self.buildout, self.options, self.name = buildout, options, name
 
-        options['location'] = os.path.join(
-            buildout['buildout']['parts-directory'],
+        if self.options.get("eggs") and options["recipe"] not in self.options["eggs"]:
+            # make sure we do not loose our own dependencies if additional eggs are provided
+            self.options["eggs"] += "\n%s" % options["recipe"]
+
+        options["location"] = os.path.join(
+            buildout["buildout"]["parts-directory"],
             self.name,
         )
-        options['bin-directory'] = buildout['buildout']['bin-directory']
-        options['scripts'] = ''  # suppress script generation.
+        options["bin-directory"] = buildout["buildout"]["bin-directory"]
+        options["scripts"] = ""  # suppress script generation.
 
         # Relative path support for the generated scripts
         relative_paths = options.get(
-            'relative-paths',
-            buildout['buildout'].get('relative-paths', 'false'))
-        if relative_paths == 'true':
-            options['buildout-directory'] = buildout['buildout']['directory']
-            self._relative_paths = options['buildout-directory']
+            "relative-paths", buildout["buildout"].get("relative-paths", "false")
+        )
+        if relative_paths == "true":
+            options["buildout-directory"] = buildout["buildout"]["directory"]
+            self._relative_paths = options["buildout-directory"]
         else:
-            self._relative_paths = ''
-            assert relative_paths == 'false'
+            self._relative_paths = ""
+            assert relative_paths == "false"
 
     _ws_locations = None
 
+    @property
     def ws_locations(self):
         if self._ws_locations is None:
-            self._ws_locations = [d.location for d in self.zodb_ws]
+            self._ws_locations = {d.location for d in self.zodb_ws}
         return self._ws_locations
-    ws_locations = property(ws_locations)
 
     def install(self):
         _, self.zodb_ws = self.egg.working_set()
 
         options = self.options
-        location = options['location']
+        location = options["location"]
 
         if os.path.exists(location):
             shutil.rmtree(location)
 
-        self.module_paths = self.options.get('extra-paths', [])
+        self.module_paths = self.options.get("extra-paths", [])
         if self.module_paths:
             # Filter out empty directories
-            self.module_paths = [p for p in self.module_paths.split('\n') if p]
+            self.module_paths = [p for p in self.module_paths.split("\n") if p]
 
         # this was taken from mkzeoinstance.py
         import zdaemon
+
         zdaemon_home = os.path.split(zdaemon.__path__[0])[0]
 
         import ZEO
+
         self.zodb_home = os.path.dirname(os.path.dirname(ZEO.__file__))
         params = {
             "package": "zeo",
             "PACKAGE": "ZEO",
             "zodb_home": self.zodb_home,
-            'zdaemon_home': zdaemon_home,
+            "zdaemon_home": zdaemon_home,
             "instance_home": location,
-            "address": '8100',  # will be overwritten later
-            "python": options['executable'],
+            "address": "8100",  # will be overwritten later
+            "python": options["executable"],
         }
         from zope.mkzeoinstance import ZEOInstanceBuilder
+
         ZEOInstanceBuilder().create(location, params)
 
         try:
             # Save the working set:
-            open(os.path.join(location, 'etc', '.eggs'), 'w').write(
-                '\n'.join(self.ws_locations))
+            open(os.path.join(location, "etc", ".eggs"), "w").write(
+                "\n".join(self.ws_locations)
+            )
 
             # Make a new zeo.conf based on options in buildout.cfg
             self.build_zeo_conf()
 
             # Patch extra paths into binaries
             self.patch_binaries()
 
             # Install extra scripts
             self.install_scripts()
 
-        except Exception:            # clean up
+        except Exception:  # clean up
             shutil.rmtree(location)
             raise
 
         return location
 
     def update(self):
         _, self.zodb_ws = self.egg.working_set()
 
         options = self.options
-        location = options['location']
+        location = options["location"]
 
         if os.path.exists(location):
             # See if we can stop. We need to see if the working set path
             # has changed.
-            saved_path = os.path.join(location, 'etc', '.eggs')
+            saved_path = os.path.join(location, "etc", ".eggs")
             if os.path.isfile(saved_path):
-                if (open(saved_path).read() != '\n'.join(self.ws_locations)):
+                if open(saved_path).read() != "\n".join(self.ws_locations):
                     # Something has changed. Blow away the instance.
                     self.install()
 
             # Nothing has changed.
             return location
 
         else:
             self.install()
 
         return location
 
     def build_zeo_conf(self):
-        """Create a zeo.conf file
-        """
+        """Create a zeo.conf file"""
         options = self.options
-        location = options['location']
+        location = options["location"]
         instance_home = location
 
-        base_dir = self.buildout['buildout']['directory']
-        var_dir = options.get('var', os.path.join(base_dir, 'var'))
+        base_dir = self.buildout["buildout"]["directory"]
+        var_dir = options.get("var", os.path.join(base_dir, "var"))
         if not os.path.exists(var_dir):
             os.makedirs(var_dir)
 
         self.pid_file = options.get(
-            'pid-file',
-            os.path.join(var_dir, self.name + '.pid'))
+            "pid-file", os.path.join(var_dir, self.name + ".pid")
+        )
 
-        zeo_conf_path = options.get('zeo-conf', None)
+        zeo_conf_path = options.get("zeo-conf", None)
         if zeo_conf_path is not None:
             zeo_conf = "%%include %s" % os.path.abspath(zeo_conf_path)
         else:
-            zeo_address = options.get('zeo-address', '8100')
-            zeo_conf_additional = options.get('zeo-conf-additional', '')
-            storage_number = options.get('storage-number', '1')
+            zeo_address = options.get("zeo-address", "8100")
+            zeo_conf_additional = options.get("zeo-conf-additional", "")
+            storage_number = options.get("storage-number", "1")
 
-            monitor_address = options.get('monitor-address', '')
+            monitor_address = options.get("monitor-address", "")
             if monitor_address:
-                monitor_address = 'monitor-address %s' % monitor_address
+                monitor_address = "monitor-address %s" % monitor_address
 
-            effective_user = options.get('effective-user', '')
+            effective_user = options.get("effective-user", "")
             if effective_user:
-                effective_user = 'user %s' % effective_user
+                effective_user = "user %s" % effective_user
 
-            invalidation_queue_size = options.get('invalidation-queue-size',
-                                                  '100')
+            invalidation_queue_size = options.get("invalidation-queue-size", "100")
 
-            socket_name = options.get('socket-name',
-                                      '%s/zeo.zdsock' % var_dir)
+            socket_name = options.get("socket-name", "%s/zeo.zdsock" % var_dir)
             socket_dir = os.path.dirname(socket_name)
             if not os.path.exists(socket_dir):
                 os.makedirs(socket_dir)
 
-            z_log_name = os.path.sep.join(('log', self.name + '.log'))
-            zeo_log_level = options.get('zeo-log-level', 'info')
-            zeo_log_custom = options.get('zeo-log-custom', None)
+            z_log_name = os.path.sep.join(("log", self.name + ".log"))
+            zeo_log_level = options.get("zeo-log-level", "info")
+            zeo_log_custom = options.get("zeo-log-custom", None)
 
             # if zeo-log is given, we use it to set the runner
             # logfile value in any case
-            z_log_filename = options.get('zeo-log', z_log_name)
+            z_log_filename = options.get("zeo-log", z_log_name)
             z_log_filename = os.path.join(var_dir, z_log_filename)
             z_log_dir = os.path.dirname(z_log_filename)
             if not os.path.exists(z_log_dir):
                 os.makedirs(z_log_dir)
 
             # zeo-log-custom superseeds zeo-log
-            logformat = options.get(
-                'zeo-log-format', '%(asctime)s %(message)s')
+            logformat = options.get("zeo-log-format", "%(asctime)s %(message)s")
             if zeo_log_custom is None:
-                zeo_log_rotate = ''
-                zeo_log_max_size = options.get('zeo-log-max-size', None)
+                zeo_log_rotate = ""
+                zeo_log_max_size = options.get("zeo-log-max-size", None)
                 if zeo_log_max_size:
-                    zeo_log_old_files = options.get('zeo-log-old-files', 1)
-                    zeo_log_rotate = '\n'.join((
-                        "max-size %s" % zeo_log_max_size,
-                        "      old-files %s" % zeo_log_old_files))
+                    zeo_log_old_files = options.get("zeo-log-old-files", 1)
+                    zeo_log_rotate = "\n".join(
+                        (
+                            "max-size %s" % zeo_log_max_size,
+                            "      old-files %s" % zeo_log_old_files,
+                        )
+                    )
                 z_log = z_log_file % {
-                    'filename': z_log_filename,
-                    'logformat': logformat,
-                    'zeo_log_rotate': zeo_log_rotate}
+                    "filename": z_log_filename,
+                    "logformat": logformat,
+                    "zeo_log_rotate": zeo_log_rotate,
+                }
             else:
                 z_log = zeo_log_custom
 
-            file_storage = os.path.sep.join(('filestorage', 'Data.fs'))
-            file_storage = options.get('file-storage', file_storage)
+            file_storage = os.path.sep.join(("filestorage", "Data.fs"))
+            file_storage = options.get("file-storage", file_storage)
             file_storage = os.path.join(var_dir, file_storage)
             file_storage_dir = os.path.dirname(file_storage)
             if not os.path.exists(file_storage_dir):
                 os.makedirs(file_storage_dir)
 
-            if options.get('authentication-database', ''):
-                authentication = authentication_template % \
-                    dict(database=options.get('authentication-database'),
-                         realm=options.get('authentication-realm', 'ZEO'))
+            if options.get("authentication-database", ""):
+                authentication = authentication_template % dict(
+                    database=options.get("authentication-database"),
+                    realm=options.get("authentication-realm", "ZEO"),
+                )
             else:
-                authentication = ''
+                authentication = ""
 
-            blob_storage = options.get('blob-storage', 'blobstorage')
+            blob_storage = options.get("blob-storage", "blobstorage")
             if blob_storage:
                 blob_storage = os.path.join(var_dir, blob_storage)
                 storage_template = blob_storage_template
             else:
                 storage_template = file_storage_template
 
-            effective_user = options.get('effective-user', '')
+            effective_user = options.get("effective-user", "")
             if effective_user:
-                effective_user = 'user %s' % effective_user
+                effective_user = "user %s" % effective_user
 
-            pack_gc = options.get('pack-gc', '')
-            if pack_gc.lower() == 'false':
-                pack_gc = 'pack-gc false'
-
-            pack_keep_old = options.get('pack-keep-old', '')
-            if pack_keep_old.lower() == 'false':
-                pack_keep_old = 'pack-keep-old false'
+            pack_gc = options.get("pack-gc", "")
+            if pack_gc.lower() == "false":
+                pack_gc = "pack-gc false"
+
+            pack_keep_old = options.get("pack-keep-old", "")
+            if pack_keep_old.lower() == "false":
+                pack_keep_old = "pack-keep-old false"
 
             storage = storage_template % dict(
                 storage_number=storage_number,
                 file_storage=file_storage,
                 blob_storage=blob_storage,
                 pack_gc=pack_gc,
                 pack_keep_old=pack_keep_old,
             )
 
             # ZRS config
-            rfrom = options.get('replicate-from')
-            rto = options.get('replicate-to')
+            rfrom = options.get("replicate-from")
+            rto = options.get("replicate-to")
             if HAS_ZRS and (rfrom or rto):
-                replicate = ''
+                replicate = ""
                 if rfrom:
                     replicate += "\nreplicate-from %s" % rfrom
                 if rto:
                     replicate += "\nreplicate-to %s" % rto
-                keep_alive = options.get('keep-alive-delay', '60')
+                keep_alive = options.get("keep-alive-delay", "60")
                 storage = zrs_template % dict(
                     storage=storage,
                     keep_alive=keep_alive,
                     replicate=replicate,
-                    storage_number=storage_number
+                    storage_number=storage_number,
                 )
 
-            read_only = options.get('read-only', 'false')
+            read_only = options.get("read-only", "false")
             zeo_conf = zeo_conf_template % dict(
                 instance_home=instance_home,
                 effective_user=effective_user,
                 invalidation_queue_size=invalidation_queue_size,
                 socket_name=socket_name,
                 z_log=z_log,
                 z_log_filename=z_log_filename,
                 authentication=authentication,
                 storage=storage,
                 zeo_address=zeo_address,
                 pid_file=self.pid_file,
                 zeo_conf_additional=zeo_conf_additional,
                 monitor_address=monitor_address,
                 zeo_log_level=zeo_log_level,
-                read_only=read_only
+                read_only=read_only,
             )
 
-        zeo_conf_path = os.path.join(location, 'etc', 'zeo.conf')
-        open(zeo_conf_path, 'w').write(zeo_conf)
+        zeo_conf_path = os.path.join(location, "etc", "zeo.conf")
+        open(zeo_conf_path, "w").write(zeo_conf)
 
     def patch_binaries(self):
-        location = self.options['location']
+        location = self.options["location"]
         # XXX We need to patch the windows specific batch scripts
-        # and they need a different path seperator
+        # and they need a different path separator
         path = (
-            os.path.pathsep.join(self.ws_locations) +
-            os.path.pathsep +
-            os.path.pathsep.join(self.module_paths)
+            os.path.pathsep.join(self.ws_locations)
+            + os.path.pathsep
+            + os.path.pathsep.join(self.module_paths)
         )
-
-        for script_name in ('runzeo', 'zeoctl'):
-            script_path = os.path.join(location, 'bin', script_name)
+        for script_name in ("runzeo", "zeoctl"):
+            script_path = os.path.join(location, "bin", script_name)
             script = open(script_path).read()
-            script = script.replace('PYTHONPATH="$ZODB3_HOME"',
-                                    'PYTHONPATH="%s"' % path)
-            f = open(script_path, 'w')
+            script = script.replace(
+                'PYTHONPATH="$ZODB3_HOME"', 'PYTHONPATH="%s"' % path
+            )
+            f = open(script_path, "w")
             f.write(script)
             f.close()
 
     def install_scripts(self):
         options = self.options
-        location = options['location']
+        location = options["location"]
 
-        self.zeo_conf = options.get('zeo-conf', None)
+        self.zeo_conf = options.get("zeo-conf", None)
         if self.zeo_conf is None:
-            self.zeo_conf = os.path.join(location, 'etc', 'zeo.conf')
+            self.zeo_conf = os.path.join(location, "etc", "zeo.conf")
 
-        _, ws = self.egg.working_set(['plone.recipe.zeoserver'])
+        _, ws = self.egg.working_set(["plone.recipe.zeoserver"])
 
-        path = (
-            os.path.pathsep.join(self.ws_locations) +
-            os.path.pathsep +
-            os.path.pathsep.join(self.module_paths)
-        )
-        initialization = """
-        import os; os.environ['PYTHONPATH'] = %r
-        """.strip() % path
         zc.buildout.easy_install.scripts(
-            [(self.name, 'plone.recipe.zeoserver.ctl', 'main')],
-            ws, options['executable'], options['bin-directory'],
-            initialization='\n'.join(
-                [initialization, options.get('initialization', ''), '']),
-            arguments=('\n        ["-C", %r]'
-                       '\n        + sys.argv[1:]'
-                       % self.zeo_conf),
+            [(self.name, "plone.recipe.zeoserver.ctl", "main")],
+            ws,
+            options["executable"],
+            options["bin-directory"],
+            initialization=options.get("initialization", ""),
+            arguments=(
+                '\n        ["-C", %r]' "\n        + sys.argv[1:]" % self.zeo_conf
+            ),
             extra_paths=self.module_paths,
-            relative_paths=self._relative_paths)
+            relative_paths=self._relative_paths,
+        )
 
         # zeopack.py
-        zeopack = options.get('zeopack', None)
-        zeopack_script_name = options.get('zeopack-script-name', 'zeopack')
+        zeopack = options.get("zeopack", None)
+        zeopack_script_name = options.get("zeopack-script-name", "zeopack")
         zeopack_scripts = dict(zeopack=zeopack_script_name)
         if zeopack is not None:
             directory, filename = os.path.split(zeopack)
             if zeopack and os.path.exists(zeopack):
                 zc.buildout.easy_install.scripts(
-                    [('zeopack', os.path.splitext(filename)[0], 'main')],
-                    ws, options['executable'], options['bin-directory'],
+                    [("zeopack", os.path.splitext(filename)[0], "main")],
+                    ws,
+                    options["executable"],
+                    options["bin-directory"],
                     scripts=zeopack_scripts,
                     extra_paths=ws + [directory] + self.module_paths,
                     relative_paths=self._relative_paths,
                 )
         else:
-            host = port = socket_path = ''
-            zeo_address = options.get('zeo-address', '8100')
-            parts = zeo_address.split(':')
+            host = port = socket_path = ""
+            zeo_address = options.get("zeo-address", "8100")
+            parts = zeo_address.split(":")
 
             if len(parts) == 1:
                 try:
                     # if the only argument is a port, which must be an int,
                     # we use 127.0.0.1 as the host by default
                     port = int(zeo_address)
                 except ValueError:
                     # The address is a simple string, we now assume it is
                     # a path to a Unix socket file
                     socket_path = zeo_address
                 else:
-                    host = '127.0.0.1'
+                    host = "127.0.0.1"
                     port = zeo_address
             else:
                 host, port = parts
 
-            username = options.get('pack-user', None)
-            password = options.get('pack-password', None)
+            username = options.get("pack-user", None)
+            password = options.get("pack-password", None)
             if username is not None:
-                realm = options.get('authentication-realm', 'ZEO')
+                realm = options.get("authentication-realm", "ZEO")
             else:
                 realm = None
-            storage = options.get('storage-number', '1')
+            storage = options.get("storage-number", "1")
 
             arg_list = [
-                'host', 'port', 'unix', 'days',
-                'username', 'password', 'realm', 'blob_dir', 'storage',
+                "host",
+                "port",
+                "unix",
+                "days",
+                "username",
+                "password",
+                "realm",
+                "blob_dir",
+                "storage",
             ]
             arguments = dict(
                 address=zeo_address,
                 host=host,
                 port=port,
                 unix=socket_path,
-                days=options.get('pack-days', 1),
+                days=options.get("pack-days", 1),
                 username=username,
                 password=password,
                 realm=realm,
                 storage=storage,
-                blob_dir=options.get('blob-storage', None),
+                blob_dir=options.get("blob-storage", None),
             )
-            arguments_info = ''
+            arguments_info = ""
             for k, v in arguments.items():
                 if not v:
-                    arguments_info += '%s = None\n' % k
+                    arguments_info += "%s = None\n" % k
                 else:
-                    arguments_info += '%s = "%s"\n' % (k, v)
+                    arguments_info += f'{k} = "{v}"\n'
 
-            arguments_info += ("import getopt; opts = "
-                               "getopt.getopt(sys.argv[1:], 'S:B:D:W1')[0];\n"
-                               "opts = dict(opts)\n"
-                               "storage = opts.get('-S') and "
-                               "opts['-S'] or storage\n"
-                               "blob_dir = opts.get('-B') and "
-                               "opts['-B'] or blob_dir\n"
-                               "days = opts.get('-D') and "
-                               "opts['-D'] or days\n"
-                               )
+            arguments_info += (
+                "import getopt; opts = "
+                "getopt.getopt(sys.argv[1:], 'S:B:D:W1')[0];\n"
+                "opts = dict(opts)\n"
+                "storage = opts.get('-S') and "
+                "opts['-S'] or storage\n"
+                "blob_dir = opts.get('-B') and "
+                "opts['-B'] or blob_dir\n"
+                "days = opts.get('-D') and "
+                "opts['-D'] or days\n"
+            )
 
             # Make sure the recipe itself and its dependencies are on the path
-            extra_paths = [
-                ws.by_key[options['recipe'].replace('[zrs]', '')].location]
+            extra_paths = [ws.by_key[options["recipe"].replace("[zrs]", "")].location]
             try:
-                extra_paths.append(ws.by_key['zc.buildout'].location)
+                extra_paths.append(ws.by_key["zc.buildout"].location)
             except KeyError:
                 # XXX Buildout installed with Pip?
                 pass
-            extra_paths.append(ws.by_key['zc.recipe.egg'].location)
+            extra_paths.append(ws.by_key["zc.recipe.egg"].location)
             zc.buildout.easy_install.scripts(
-                [('zeopack', 'plone.recipe.zeoserver.pack', 'main')],
-                self.zodb_ws, options['executable'], options['bin-directory'],
+                [("zeopack", "plone.recipe.zeoserver.pack", "main")],
+                self.zodb_ws,
+                options["executable"],
+                options["bin-directory"],
                 scripts=zeopack_scripts,
                 initialization=arguments_info,
-                arguments=', '.join(arg_list),
+                arguments=", ".join(arg_list),
                 relative_paths=self._relative_paths,
                 extra_paths=extra_paths + self.module_paths,
             )
 
         # The backup script, pointing to repozo.py
-        repozo = options.get('repozo', None)
-        repozo_script_name = options.get('repozo-script-name', 'repozo')
+        repozo = options.get("repozo", None)
+        repozo_script_name = options.get("repozo-script-name", "repozo")
         repozo_scripts = dict(repozo=repozo_script_name)
         if repozo is None:
-            repozo = 'ZODB.scripts.repozo'
+            repozo = "ZODB.scripts.repozo"
             extra_paths = []
         else:
             if not os.path.exists(repozo):
-                raise AssertionError(
-                    'Custom repozo script not found: %s' % repozo)
+                raise AssertionError("Custom repozo script not found: %s" % repozo)
             directory, filename = os.path.split(repozo)
             repozo = os.path.splitext(filename)[0]
             extra_paths = [directory]
         zc.buildout.easy_install.scripts(
-            [('repozo', repozo, 'main')],
-            self.zodb_ws, options['executable'], options['bin-directory'],
+            [("repozo", repozo, "main")],
+            self.zodb_ws,
+            options["executable"],
+            options["bin-directory"],
             scripts=repozo_scripts,
             extra_paths=extra_paths + self.module_paths,
             relative_paths=self._relative_paths,
         )
 
-        if sys.platform == 'win32':
+        if sys.platform == "win32":
             self.install_win32_scripts()
 
     def install_win32_scripts(self):
-        path = self.ws_locations + self.module_paths
-        location = self.options['location']
+        path = list(self.ws_locations) + self.module_paths
+        location = self.options["location"]
 
-        arguments = {'PYTHON': self.options['executable'],
-                     'zodb_home': self.zodb_home,
-                     'INSTANCE_HOME': location,
-                     'PYTHONPATH': os.path.pathsep.join(path),
-                     'PACKAGE': 'zeo',
-                     'PID_FILENAME': self.pid_file}
+        arguments = {
+            "PYTHON": self.options["executable"],
+            "zodb_home": self.zodb_home,
+            "INSTANCE_HOME": location,
+            "PYTHONPATH": os.path.pathsep.join(path),
+            "PACKAGE": "zeo",
+            "PID_FILENAME": self.pid_file,
+        }
 
         # runzeo.bat
-        runzeo_filename = '%s_runzeo.bat' % self.name
-        runzeo = open(join(curdir, 'runzeo.bat')).read()
-        self._write_file(os.path.join(self.options['bin-directory'],
-                                      runzeo_filename), runzeo % arguments)
+        runzeo_filename = "%s_runzeo.bat" % self.name
+        runzeo = open(join(curdir, "runzeo.bat")).read()
+        self._write_file(
+            os.path.join(self.options["bin-directory"], runzeo_filename),
+            runzeo % arguments,
+        )
 
         # zeoservice.py
-        zeo_filename = '%s_service' % self.name
-        zeo_service = open(join(curdir, 'zeoservice.py.in')).read()
-        zeo_file = os.path.join(self.options['bin-directory'],
-                                '%s.py' % zeo_filename)
+        zeo_filename = "%s_service" % self.name
+        zeo_service = open(join(curdir, "zeoservice.py.in")).read()
+        zeo_file = os.path.join(self.options["bin-directory"], "%s.py" % zeo_filename)
         self._write_file(zeo_file, zeo_service % arguments)
 
-        initialization = """
-        import os; os.environ['PYTHONPATH'] = %r
-        """.strip() % os.path.pathsep.join(path)
-
         zc.buildout.easy_install.scripts(
-            [(zeo_filename, zeo_filename, 'main')],
+            [(zeo_filename, zeo_filename, "main")],
             self.zodb_ws,
-            self.options['executable'],
-            self.options['bin-directory'],
+            self.options["executable"],
+            self.options["bin-directory"],
             extra_paths=path,
             relative_paths=self._relative_paths,
-            initialization=initialization,
+            initialization=self.options.get("initialization", ""),
         )
 
     def _write_file(self, path, content):
-        logger = logging.getLogger('zc.buildout.easy_install')
-        f = open(path, 'w')
+        logger = logging.getLogger("zc.buildout.easy_install")
+        f = open(path, "w")
         try:
             f.write(content)
         finally:
             f.close()
-        logger.debug('Wrote file %s' % path)
+        logger.debug("Wrote file %s" % path)
         os.chmod(path, 0o755)
-        logger.warning('Changed mode for %s to 755' % path)
+        logger.warning("Changed mode for %s to 755" % path)
 
 
 # the template used to build a regular file storage entry for zeo.conf
 file_storage_template = """
 <filestorage %(storage_number)s>
   path %(file_storage)s
   %(pack_gc)s
```

