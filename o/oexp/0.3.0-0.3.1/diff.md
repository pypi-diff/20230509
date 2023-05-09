# Comparing `tmp/oexp-0.3.0.tar.gz` & `tmp/oexp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.3.0.tar", last modified: Mon May  8 23:04:19 2023, max compression
+gzip compressed data, was "oexp-0.3.1.tar", last modified: Tue May  9 00:13:28 2023, max compression
```

## Comparing `oexp-0.3.0.tar` & `oexp-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-08 23:04:19.975768 oexp-0.3.0/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-08 23:04:19.975582 oexp-0.3.0/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.3.0/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-08 23:04:19.974447 oexp-0.3.0/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.3.0/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    71050 2023-05-08 23:03:51.000000 oexp-0.3.0/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-08 23:03:35.000000 oexp-0.3.0/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     4740 2023-05-08 19:15:04.000000 oexp-0.3.0/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-08 23:04:19.975369 oexp-0.3.0/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-08 23:04:19.000000 oexp-0.3.0/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-08 23:04:14.000000 oexp-0.3.0/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-08 23:04:19.975816 oexp-0.3.0/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:13:28.597553 oexp-0.3.1/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:13:28.597394 oexp-0.3.1/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.3.1/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:13:28.596526 oexp-0.3.1/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.3.1/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    71075 2023-05-09 00:10:01.000000 oexp-0.3.1/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 00:09:40.000000 oexp-0.3.1/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     4740 2023-05-08 19:15:04.000000 oexp-0.3.1/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 00:13:28.597224 oexp-0.3.1/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 00:13:28.000000 oexp-0.3.1/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 00:13:28.000000 oexp-0.3.1/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 00:13:28.000000 oexp-0.3.1/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 00:13:28.000000 oexp-0.3.1/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 00:13:28.000000 oexp-0.3.1/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 00:13:24.000000 oexp-0.3.1/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 00:13:28.597597 oexp-0.3.1/setup.cfg
```

### Comparing `oexp-0.3.0/oexp/access.py` & `oexp-0.3.1/oexp/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/359/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/362/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -219,14 +219,15 @@
 def _exit_server():
     _sendall(EXIT)
 
 
 # [[matt.oexp.front.api.ApiKt#login]]
 def login(username, password) -> OnlineExperiments:
     _ensure_synchronized()
+    jbridge._init_java()
     _sendall(CALL_GLOBAL_FUN)
     _send_string(f"matt.oexp.front.api.ApiKt")
     _send_string(f"login")
     _send_string(username)
     _send_string(password)
     _recv_exception_check()
     return _recv_object(OnlineExperiments, nullable=False)
```

### Comparing `oexp-0.3.0/oexp/jbridge.py` & `oexp-0.3.1/oexp/jbridge.py`

 * *Files identical despite different names*

