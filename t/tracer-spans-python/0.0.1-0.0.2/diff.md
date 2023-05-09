# Comparing `tmp/tracer_spans_python-0.0.1.tar.gz` & `tmp/tracer_spans_python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracer_spans_python-0.0.1.tar", last modified: Tue May  9 01:44:27 2023, max compression
+gzip compressed data, was "tracer_spans_python-0.0.2.tar", last modified: Tue May  9 01:59:09 2023, max compression
```

## Comparing `tracer_spans_python-0.0.1.tar` & `tracer_spans_python-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-09 01:44:27.582653 tracer_spans_python-0.0.1/
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      729 2023-05-09 01:44:27.584653 tracer_spans_python-0.0.1/PKG-INFO
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      106 2023-05-09 01:44:27.588653 tracer_spans_python-0.0.1/setup.cfg
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      803 2023-05-09 01:36:30.000000 tracer_spans_python-0.0.1/setup.py
-drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-09 01:44:27.572653 tracer_spans_python-0.0.1/tracer_spans_python.egg-info/
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      729 2023-05-09 01:44:27.000000 tracer_spans_python-0.0.1/tracer_spans_python.egg-info/PKG-INFO
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      221 2023-05-09 01:44:27.000000 tracer_spans_python-0.0.1/tracer_spans_python.egg-info/SOURCES.txt
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)        1 2023-05-09 01:44:27.000000 tracer_spans_python-0.0.1/tracer_spans_python.egg-info/dependency_links.txt
--rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       14 2023-05-09 01:44:27.000000 tracer_spans_python-0.0.1/tracer_spans_python.egg-info/top_level.txt
-drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-09 01:44:27.557653 tracer_spans_python-0.0.1/tracers_spans/
+drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-09 01:59:09.559654 tracer_spans_python-0.0.2/
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)     1092 2023-05-09 01:25:16.000000 tracer_spans_python-0.0.2/LICENSE
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      729 2023-05-09 01:59:09.559654 tracer_spans_python-0.0.2/PKG-INFO
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      102 2023-05-09 01:59:09.561654 tracer_spans_python-0.0.2/setup.cfg
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      839 2023-05-09 01:54:06.000000 tracer_spans_python-0.0.2/setup.py
+drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-09 01:59:09.558654 tracer_spans_python-0.0.2/tracer_spans_python.egg-info/
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      729 2023-05-09 01:59:09.000000 tracer_spans_python-0.0.2/tracer_spans_python.egg-info/PKG-INFO
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)      271 2023-05-09 01:59:09.000000 tracer_spans_python-0.0.2/tracer_spans_python.egg-info/SOURCES.txt
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)        1 2023-05-09 01:59:09.000000 tracer_spans_python-0.0.2/tracer_spans_python.egg-info/dependency_links.txt
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       10 2023-05-09 01:59:09.000000 tracer_spans_python-0.0.2/tracer_spans_python.egg-info/requires.txt
+-rw-r--r--   0 mascarenhas  (1000) mascarenhas  (1000)       14 2023-05-09 01:59:09.000000 tracer_spans_python-0.0.2/tracer_spans_python.egg-info/top_level.txt
+drwxr-xr-x   0 mascarenhas  (1000) mascarenhas  (1000)        0 2023-05-09 01:59:09.552654 tracer_spans_python-0.0.2/tracers_spans/
```

### Comparing `tracer_spans_python-0.0.1/PKG-INFO` & `tracer_spans_python-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tracer_spans_python
-Version: 0.0.1
+Version: 0.0.2
 Summary: Projeto para facilitar a criação e envios de tracers e spans.
 Home-page: UNKNOWN
 Author: Otávio Mascarenhas
 Author-email: otaviomascarenhaspessoal@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: Tracers Spans tracers spans tracer span OpenTelemetry Zipkin
```

### Comparing `tracer_spans_python-0.0.1/setup.py` & `tracer_spans_python-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup
 
 setup(
     name = 'tracer_spans_python',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Otávio Mascarenhas',
     author_email = 'otaviomascarenhaspessoal@gmail.com',
     packages = ['tracers_spans'],
     description = 'Projeto para facilitar a criação e envios de tracers e spans.',
     license = 'MIT',
     keywords = 'Tracers Spans tracers spans tracer span OpenTelemetry Zipkin',
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: Portuguese (Brazilian)',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Internationalization',
         'Topic :: Scientific/Engineering :: Physics'
-    ]
+    ],
+    install_requires=['aiozipkin']
     )
```

### Comparing `tracer_spans_python-0.0.1/tracer_spans_python.egg-info/PKG-INFO` & `tracer_spans_python-0.0.2/tracer_spans_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tracer-spans-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: Projeto para facilitar a criação e envios de tracers e spans.
 Home-page: UNKNOWN
 Author: Otávio Mascarenhas
 Author-email: otaviomascarenhaspessoal@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: Tracers Spans tracers spans tracer span OpenTelemetry Zipkin
```

