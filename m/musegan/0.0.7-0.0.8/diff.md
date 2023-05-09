# Comparing `tmp/musegan-0.0.7.tar.gz` & `tmp/musegan-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musegan-0.0.7.tar", last modified: Tue May  9 06:15:34 2023, max compression
+gzip compressed data, was "musegan-0.0.8.tar", last modified: Tue May  9 06:52:58 2023, max compression
```

## Comparing `musegan-0.0.7.tar` & `musegan-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 06:15:34.660471 musegan-0.0.7/
--rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1691 2023-05-09 06:15:34.660471 musegan-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      892 2023-05-09 05:17:56.000000 musegan-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 06:15:34.644845 musegan-0.0.7/musegan/
-drwxrwxrwx   0        0        0        0 2023-05-09 06:15:34.644845 musegan-0.0.7/musegan/archs/
--rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.0.7/musegan/archs/__init__.py
--rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.0.7/musegan/archs/bar_generator.py
--rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.0.7/musegan/archs/critic.py
--rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.0.7/musegan/archs/generator.py
--rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.0.7/musegan/archs/temp_network.py
--rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.0.7/musegan/archs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:15:34.644845 musegan-0.0.7/musegan/dataset/
--rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.0.7/musegan/dataset/__init__.py
--rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.0.7/musegan/dataset/data_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-09 06:15:34.660471 musegan-0.0.7/musegan/musegan.egg-info/
--rw-rw-rw-   0        0        0     1691 2023-05-09 06:15:34.000000 musegan-0.0.7/musegan/musegan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-05-09 06:15:34.000000 musegan-0.0.7/musegan/musegan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 06:15:34.000000 musegan-0.0.7/musegan/musegan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-09 06:15:34.000000 musegan-0.0.7/musegan/musegan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-09 06:15:34.000000 musegan-0.0.7/musegan/musegan.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 06:15:34.660471 musegan-0.0.7/musegan/trainner/
--rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.0.7/musegan/trainner/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.0.7/musegan/trainner/criterion.py
--rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.0.7/musegan/trainner/trainer.py
--rw-rw-rw-   0        0        0       86 2023-05-09 06:15:34.660471 musegan-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2092 2023-05-09 06:15:19.000000 musegan-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:52:58.638457 musegan-0.0.8/
+-rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1507 2023-05-09 06:52:58.638457 musegan-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2023-05-09 05:17:56.000000 musegan-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 06:52:58.613404 musegan-0.0.8/musegan/
+drwxrwxrwx   0        0        0        0 2023-05-09 06:52:58.627456 musegan-0.0.8/musegan/archs/
+-rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.0.8/musegan/archs/__init__.py
+-rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.0.8/musegan/archs/bar_generator.py
+-rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.0.8/musegan/archs/critic.py
+-rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.0.8/musegan/archs/generator.py
+-rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.0.8/musegan/archs/temp_network.py
+-rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.0.8/musegan/archs/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:52:58.629458 musegan-0.0.8/musegan/dataset/
+-rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.0.8/musegan/dataset/__init__.py
+-rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.0.8/musegan/dataset/data_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:52:58.633520 musegan-0.0.8/musegan/musegan.egg-info/
+-rw-rw-rw-   0        0        0     1507 2023-05-09 06:52:58.000000 musegan-0.0.8/musegan/musegan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-05-09 06:52:58.000000 musegan-0.0.8/musegan/musegan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 06:52:58.000000 musegan-0.0.8/musegan/musegan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-09 06:52:58.000000 musegan-0.0.8/musegan/musegan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 06:52:58.637458 musegan-0.0.8/musegan/trainner/
+-rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.0.8/musegan/trainner/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.0.8/musegan/trainner/criterion.py
+-rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.0.8/musegan/trainner/trainer.py
+-rw-rw-rw-   0        0        0       86 2023-05-09 06:31:55.000000 musegan-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      736 2023-05-09 06:52:58.639456 musegan-0.0.8/setup.cfg
```

### Comparing `musegan-0.0.7/LICENSE` & `musegan-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/PKG-INFO` & `musegan-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.7
-Author: clifford njoroge
-Author-email: cnjoroge925@gmail.com
-License: MIT
-Keywords: pytorch,music,generative adverserial networks
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
+Version: 0.0.8
+Summary: A pytorch implementation of musegan
+Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
+Author: Clifford Njoroge
+Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MuseGAN
 =========
 A Pytorch implementation of MuseGAN
 Only linux BSD support due to SharedArray usage
```

### Comparing `musegan-0.0.7/README.md` & `musegan-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/archs/bar_generator.py` & `musegan-0.0.8/musegan/archs/bar_generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/archs/critic.py` & `musegan-0.0.8/musegan/archs/critic.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/archs/generator.py` & `musegan-0.0.8/musegan/archs/generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/archs/temp_network.py` & `musegan-0.0.8/musegan/archs/temp_network.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/archs/utils.py` & `musegan-0.0.8/musegan/archs/utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/dataset/data_utils.py` & `musegan-0.0.8/musegan/dataset/data_utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/musegan.egg-info/PKG-INFO` & `musegan-0.0.8/musegan/musegan.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.7
-Author: clifford njoroge
-Author-email: cnjoroge925@gmail.com
-License: MIT
-Keywords: pytorch,music,generative adverserial networks
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
+Version: 0.0.8
+Summary: A pytorch implementation of musegan
+Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
+Author: Clifford Njoroge
+Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MuseGAN
 =========
 A Pytorch implementation of MuseGAN
 Only linux BSD support due to SharedArray usage
```

### Comparing `musegan-0.0.7/musegan/trainner/criterion.py` & `musegan-0.0.8/musegan/trainner/criterion.py`

 * *Files identical despite different names*

### Comparing `musegan-0.0.7/musegan/trainner/trainer.py` & `musegan-0.0.8/musegan/trainner/trainer.py`

 * *Files identical despite different names*

