# Comparing `tmp/pamai-1.0.3.tar.gz` & `tmp/pamai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pamai-1.0.3.tar", last modified: Mon May  8 12:47:46 2023, max compression
+gzip compressed data, was "pamai-1.0.4.tar", last modified: Tue May  9 06:23:42 2023, max compression
```

## Comparing `pamai-1.0.3.tar` & `pamai-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,53 @@
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:47:46.591180 pamai-1.0.3/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     1082 2023-05-08 12:08:14.000000 pamai-1.0.3/LICENSE.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       99 2023-05-08 12:06:00.000000 pamai-1.0.3/MANIFEST.in
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:47:46.591877 pamai-1.0.3/PKG-INFO
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     8509 2023-05-08 12:16:21.000000 pamai-1.0.3/README.md
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:47:46.586347 pamai-1.0.3/pamai/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      103 2023-05-08 12:04:24.000000 pamai-1.0.3/pamai/__init__.py
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       21 2023-05-08 12:47:24.000000 pamai-1.0.3/pamai/version.py
-drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-08 12:47:46.590656 pamai-1.0.3/pamai.egg-info/
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/PKG-INFO
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      246 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/SOURCES.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)        1 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/dependency_links.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)      323 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/requires.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)        6 2023-05-08 12:47:46.000000 pamai-1.0.3/pamai.egg-info/top_level.txt
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       76 2023-05-08 11:50:53.000000 pamai-1.0.3/pyproject.toml
--rw-r--r--   0 chrisrauch193   (501) staff       (20)     1158 2023-05-08 12:47:46.595519 pamai-1.0.3/setup.cfg
--rw-r--r--   0 chrisrauch193   (501) staff       (20)       97 2023-05-08 12:09:39.000000 pamai-1.0.3/setup.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.764404 pamai-1.0.4/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1082 2023-05-08 12:08:14.000000 pamai-1.0.4/LICENSE.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       99 2023-05-08 12:06:00.000000 pamai-1.0.4/MANIFEST.in
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-09 06:23:42.764723 pamai-1.0.4/PKG-INFO
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     8509 2023-05-08 12:16:21.000000 pamai-1.0.4/README.md
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.745342 pamai-1.0.4/pamai/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      114 2023-05-09 05:47:21.000000 pamai-1.0.4/pamai/__init__.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.749224 pamai-1.0.4/pamai/agents/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      393 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/agents/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1727 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/agents/base.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)    12859 2023-05-09 05:55:34.000000 pamai-1.0.4/pamai/agents/denet.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.750476 pamai-1.0.4/pamai/config/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 02:56:20.000000 pamai-1.0.4/pamai/config/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     4110 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/config/hparams.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.751961 pamai-1.0.4/pamai/datasets/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 03:11:50.000000 pamai-1.0.4/pamai/datasets/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1531 2023-05-09 05:47:53.000000 pamai-1.0.4/pamai/datasets/raw_audio.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1415 2023-05-09 05:51:43.000000 pamai-1.0.4/pamai/datasets/raw_audio_dataset.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.753049 pamai-1.0.4/pamai/graphs/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      394 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/graphs/__init__.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.755079 pamai-1.0.4/pamai/graphs/losses/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 03:12:07.000000 pamai-1.0.4/pamai/graphs/losses/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      611 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/graphs/losses/example.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1066 2023-05-09 05:56:26.000000 pamai-1.0.4/pamai/graphs/losses/utils.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.756797 pamai-1.0.4/pamai/graphs/models/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      394 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/graphs/models/__init__.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.760874 pamai-1.0.4/pamai/graphs/models/custom_layers/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     3419 2023-05-09 06:08:11.000000 pamai-1.0.4/pamai/graphs/models/custom_layers/MLP_sincnet.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        0 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/graphs/models/custom_layers/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     2613 2023-05-09 06:08:13.000000 pamai-1.0.4/pamai/graphs/models/custom_layers/de_layer.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      458 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/graphs/models/custom_layers/layer_norm.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     6815 2023-05-09 06:07:39.000000 pamai-1.0.4/pamai/graphs/models/custom_layers/sinc_conv.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1369 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/graphs/models/custom_layers/time_distributed.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     3202 2023-05-09 06:06:34.000000 pamai-1.0.4/pamai/graphs/models/denet.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     4117 2023-05-09 06:07:01.000000 pamai-1.0.4/pamai/graphs/models/sincnet.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1147 2023-05-09 06:06:05.000000 pamai-1.0.4/pamai/graphs/weights_initializer.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.764006 pamai-1.0.4/pamai/utils/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      394 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/utils/__init__.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     4262 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/utils/metrics.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1396 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/utils/misc.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     4647 2023-05-09 05:55:53.000000 pamai-1.0.4/pamai/utils/process_database.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1532 2023-04-13 05:03:09.000000 pamai-1.0.4/pamai/utils/signal_processing.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     3957 2023-05-09 06:22:40.000000 pamai-1.0.4/pamai/utils/train_utils.py
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       21 2023-05-09 06:23:28.000000 pamai-1.0.4/pamai/version.py
+drwxr-xr-x   0 chrisrauch193   (501) staff       (20)        0 2023-05-09 06:23:42.747638 pamai-1.0.4/pamai.egg-info/
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     9225 2023-05-09 06:23:42.000000 pamai-1.0.4/pamai.egg-info/PKG-INFO
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1148 2023-05-09 06:23:42.000000 pamai-1.0.4/pamai.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        1 2023-05-09 06:23:42.000000 pamai-1.0.4/pamai.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      323 2023-05-09 06:23:42.000000 pamai-1.0.4/pamai.egg-info/requires.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)        6 2023-05-09 06:23:42.000000 pamai-1.0.4/pamai.egg-info/top_level.txt
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)       76 2023-05-08 11:50:53.000000 pamai-1.0.4/pyproject.toml
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)     1158 2023-05-09 06:23:42.766026 pamai-1.0.4/setup.cfg
+-rw-r--r--   0 chrisrauch193   (501) staff       (20)      118 2023-05-09 03:08:05.000000 pamai-1.0.4/setup.py
```

### Comparing `pamai-1.0.3/LICENSE.txt` & `pamai-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pamai-1.0.3/PKG-INFO` & `pamai-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pamai
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for PAMAI written by Arthur Zucker and Chris Rauch.
 Home-page: https://github.com/ArthurZucker/PAMAI
-Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.3.tar.gz
+Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.4.tar.gz
 Author: Chris Rauch
 Author-email: chrisrauch193@gmail.com
 License: MIT
 Keywords: pamai,ai,audio,denet,arthur,zucker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ==3.8
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![wakatime](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661.svg)](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661)
 # DENet training code 
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pamai-1.0.3/README.md` & `pamai-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pamai-1.0.3/pamai.egg-info/PKG-INFO` & `pamai-1.0.4/pamai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pamai
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for PAMAI written by Arthur Zucker and Chris Rauch.
 Home-page: https://github.com/ArthurZucker/PAMAI
-Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.3.tar.gz
+Download-URL: https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.4.tar.gz
 Author: Chris Rauch
 Author-email: chrisrauch193@gmail.com
 License: MIT
 Keywords: pamai,ai,audio,denet,arthur,zucker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: ==3.8
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![wakatime](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661.svg)](https://wakatime.com/badge/user/57d887d6-525a-4214-a78c-21863f2f88f7/project/93d14295-7eb1-438b-b391-744be6d71661)
 # DENet training code 
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `pamai-1.0.3/setup.cfg` & `pamai-1.0.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Chris Rauch
 author_email = chrisrauch193@gmail.com
 keywords = pamai, ai, audio, denet, arthur, zucker
 description = Package for PAMAI written by Arthur Zucker and Chris Rauch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ArthurZucker/PAMAI
-download_url = https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.3.tar.gz
+download_url = https://github.com/ArthurZucker/PAMAI/archive/refs/tags/v1.0.4.tar.gz
 license = MIT
 license_files = LICENSE.txt
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Topic :: Software Development :: Build Tools
 	License :: OSI Approved :: MIT License
@@ -36,13 +36,13 @@
 	scikit-learn==1.2.2
 	scipy==1.10.1
 	simple-parsing==0.1.2
 	torch==2.0.0
 	torchaudio==2.0.1
 	tqdm==4.65.0
 	wandb==0.15.0
-python_requires = ==3.8
+python_requires = ~=3.8
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

