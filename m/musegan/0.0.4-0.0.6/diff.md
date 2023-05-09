# Comparing `tmp/musegan-0.0.4.tar.gz` & `tmp/musegan-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musegan-0.0.4.tar", last modified: Mon May  8 13:50:33 2023, max compression
+gzip compressed data, was "musegan-0.0.6.tar", last modified: Tue May  9 05:37:31 2023, max compression
```

## Comparing `musegan-0.0.4.tar` & `musegan-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 13:50:33.874762 musegan-0.0.4/
--rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      884 2023-05-08 13:50:33.875316 musegan-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      782 2023-04-26 09:44:28.000000 musegan-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 13:50:33.862782 musegan-0.0.4/musegan/
--rw-rw-rw-   0        0        0      420 2023-05-08 13:44:09.000000 musegan-0.0.4/musegan/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-08 13:43:49.000000 musegan-0.0.4/musegan/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-08 13:50:33.873358 musegan-0.0.4/musegan.egg-info/
--rw-rw-rw-   0        0        0      884 2023-05-08 13:50:33.000000 musegan-0.0.4/musegan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-08 13:50:33.000000 musegan-0.0.4/musegan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 13:50:33.000000 musegan-0.0.4/musegan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-08 13:50:33.000000 musegan-0.0.4/musegan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 13:50:33.000000 musegan-0.0.4/musegan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-08 13:50:33.875316 musegan-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-08 13:48:23.000000 musegan-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 05:37:31.680496 musegan-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1040 2023-05-09 05:37:31.680496 musegan-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2023-05-09 05:17:56.000000 musegan-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 05:37:31.670491 musegan-0.0.6/musegan/
+-rw-rw-rw-   0        0        0      420 2023-05-08 14:02:00.000000 musegan-0.0.6/musegan/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-08 13:43:49.000000 musegan-0.0.6/musegan/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-09 05:37:31.678497 musegan-0.0.6/musegan.egg-info/
+-rw-rw-rw-   0        0        0     1040 2023-05-09 05:37:30.000000 musegan-0.0.6/musegan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-09 05:37:31.000000 musegan-0.0.6/musegan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 05:37:30.000000 musegan-0.0.6/musegan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-09 05:37:31.000000 musegan-0.0.6/musegan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 05:37:31.000000 musegan-0.0.6/musegan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-09 05:37:31.682490 musegan-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1935 2023-05-09 05:35:39.000000 musegan-0.0.6/setup.py
```

### Comparing `musegan-0.0.4/LICENSE` & `musegan-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `musegan-0.0.4/PKG-INFO` & `musegan-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.4
-Summary: A pytorch implimentation of musegan by https://github.com/salu133445
+Version: 0.0.6
+Summary: A pytorch implimentation of musegan by forked from: https://github.com/salu133445
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
-Download-URL: https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/latest.tar.gz
-Author: cliffordkleinsr
+Download-URL: https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/Alpha.tar.gz
+Author: clifford njoroge
 Author-email: cnjoroge925@gmail.com
 License: MIT
 Keywords: pytorch,music,generative adverserial networks
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `musegan-0.0.4/README.md` & `musegan-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 MuseGAN
 =========
 A Pytorch implementation of MuseGAN
-
-[Check out the generated piano music](#)
+Only linux BSD support due to SharedArray usage
 
 :star: Star this project on GitHub — it helps!
 
 [MuseGAN](https://arxiv.org/abs/1709.06298) is a generative model which allows to
 generate music.
 
 ## Table of content
 
 - [Training](#train)
 - [License](#license)
 - [Links](#links)
 
 ## Training 
 
-See this [colab](#)  notebook for more details of training process.
+See this [colab](https://colab.research.google.com/drive/1NF2t1dvqxeblZfd7BL4Gfn4SW-xEzgGg?authuser=3#scrollTo=9bj_FWvAArPI)  notebook for more details of training process.
 * The model components and utils are under `musegan/archs` folder.
 * The Midi `torch.utils.dataset` is under `musegan/dataset/data_utils.py`.
-* The training Functions and criterions can be found in the `musegan/trainner1 folder
+* The training Functions and criterions can be found in the `musegan/trainner` folder
 
 
 
 
 ## License
 
 This project is licensed under MIT.
```

### Comparing `musegan-0.0.4/musegan.egg-info/PKG-INFO` & `musegan-0.0.6/musegan.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.0.4
-Summary: A pytorch implimentation of musegan by https://github.com/salu133445
+Version: 0.0.6
+Summary: A pytorch implimentation of musegan by forked from: https://github.com/salu133445
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
-Download-URL: https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/latest.tar.gz
-Author: cliffordkleinsr
+Download-URL: https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/Alpha.tar.gz
+Author: clifford njoroge
 Author-email: cnjoroge925@gmail.com
 License: MIT
 Keywords: pytorch,music,generative adverserial networks
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `musegan-0.0.4/setup.py` & `musegan-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from distutils.core import setup
 setup(
   name = 'musegan',         # How you named your package folder (MyLib)
-  packages = ['musegan'],   # Chose the same as "name"
-  version = '0.0.4',      # Start with a small number and increase it with every change you make
+  packages = ['musegan'],   # Choose the same as "name"
+  version = '0.0.6',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'A pytorch implimentation of musegan by https://github.com/salu133445',   # Give a short description about your library
-  author = 'cliffordkleinsr',                   # Type in your name
+  description = 'A pytorch implimentation of musegan by forked from: https://github.com/salu133445',   # Give a short description about your library
+  author = 'clifford njoroge',                   # Type in your name
   author_email = 'cnjoroge925@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/cliffordkleinsr/musegan-pytorch',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/latest.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/cliffordkleinsr/musegan-pytorch/archive/refs/tags/Alpha.tar.gz',    # I explain this later on
   keywords = ['pytorch', 'music', 'generative adverserial networks'],   # Keywords that define your package best
-  install_requires=[            # I get to this in a second
+  install_requires=[            # SharedArray is needed but only works with linux
           'music21',
           'numpy',
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
+    'Operating System :: MacOS :: MacOS X',
+    'Operating System :: Microsoft :: Windows',
+    'Operating System :: POSIX',
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
   ],
 )
```

