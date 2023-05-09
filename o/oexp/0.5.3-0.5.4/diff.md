# Comparing `tmp/oexp-0.5.3.tar.gz` & `tmp/oexp-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.5.3.tar", last modified: Tue May  9 01:49:50 2023, max compression
+gzip compressed data, was "oexp-0.5.4.tar", last modified: Tue May  9 02:15:52 2023, max compression
```

## Comparing `oexp-0.5.3.tar` & `oexp-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 01:49:50.836171 oexp-0.5.3/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 01:49:50.835983 oexp-0.5.3/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.5.3/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 01:49:50.834938 oexp-0.5.3/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.5.3/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    71381 2023-05-09 01:49:35.000000 oexp-0.5.3/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 01:49:19.000000 oexp-0.5.3/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     5375 2023-05-09 01:14:01.000000 oexp-0.5.3/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 01:49:50.835803 oexp-0.5.3/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 01:49:50.000000 oexp-0.5.3/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 01:49:50.000000 oexp-0.5.3/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 01:49:50.000000 oexp-0.5.3/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 01:49:50.000000 oexp-0.5.3/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 01:49:50.000000 oexp-0.5.3/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 01:49:46.000000 oexp-0.5.3/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 01:49:50.836216 oexp-0.5.3/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:15:52.766267 oexp-0.5.4/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:15:52.766049 oexp-0.5.4/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.5.4/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:15:52.764995 oexp-0.5.4/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.5.4/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    71656 2023-05-09 02:15:37.000000 oexp-0.5.4/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 02:15:20.000000 oexp-0.5.4/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     5375 2023-05-09 01:14:01.000000 oexp-0.5.4/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:15:52.765840 oexp-0.5.4/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 02:15:47.000000 oexp-0.5.4/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 02:15:52.766316 oexp-0.5.4/setup.cfg
```

### Comparing `oexp-0.5.3/oexp/access.py` & `oexp-0.5.4/oexp/access.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/365/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/366/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -473,41 +473,50 @@
         _ensure_synchronized()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(5)
         _recv_exception_check()
         return _recv_confirmation()
 
+    # [[matt.oexp.front.api.Experiment#sessionUrl]]
+    def session_url(self) -> str:
+        _ensure_synchronized()
+        _sendall(CALL_FUN)
+        _send_long(self._id._id)
+        _send_int(6)
+        _recv_exception_check()
+        return _recv_string(nullable=False)
+
     # [[matt.oexp.front.api.Experiment#subjectData]]
     def subject_data(self) -> SubjectData:
         _ensure_synchronized()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(6)
+        _send_int(7)
         _recv_exception_check()
         return _recv_object(SubjectData, nullable=False)
 
     # [[matt.oexp.front.api.Experiment#uploadImages]]
     def upload_images(self, root_dir) -> List[str]:
         _ensure_synchronized()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(7)
+        _send_int(8)
         _send_string(root_dir)
         _recv_exception_check()
         return _recv_list(
             elementReceiveFun=lambda: _recv_string(nullable=False), nullable=False
         )
 
     # [[matt.oexp.front.api.Experiment#viewImage]]
     def view_image(self, path):
         _ensure_synchronized()
         _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(8)
+        _send_int(9)
         _send_string(path)
         _recv_exception_check()
         return _recv_confirmation()
 
     # [[matt.oexp.front.api.Experiment]]
     def __eq__(self, other):
         _ensure_synchronized()
```

### Comparing `oexp-0.5.3/oexp/jbridge.py` & `oexp-0.5.4/oexp/jbridge.py`

 * *Files identical despite different names*

