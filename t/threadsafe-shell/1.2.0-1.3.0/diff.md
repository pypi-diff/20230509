# Comparing `tmp/threadsafe_shell-1.2.0.tar.gz` & `tmp/threadsafe_shell-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsafe_shell-1.2.0.tar", last modified: Mon May  8 20:16:43 2023, max compression
+gzip compressed data, was "threadsafe_shell-1.3.0.tar", last modified: Tue May  9 19:38:55 2023, max compression
```

## Comparing `threadsafe_shell-1.2.0.tar` & `threadsafe_shell-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-08 20:16:43.406706 threadsafe_shell-1.2.0/
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)     1071 2022-11-05 20:17:37.000000 threadsafe_shell-1.2.0/LICENSE
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-08 20:16:43.406706 threadsafe_shell-1.2.0/PKG-INFO
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       88 2022-11-05 20:23:15.000000 threadsafe_shell-1.2.0/README.md
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      565 2023-05-08 20:16:32.000000 threadsafe_shell-1.2.0/pyproject.toml
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       38 2023-05-08 20:16:43.406706 threadsafe_shell-1.2.0/setup.cfg
-drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-08 20:16:43.406706 threadsafe_shell-1.2.0/threadsafe_shell.egg-info/
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-08 20:16:43.000000 threadsafe_shell-1.2.0/threadsafe_shell.egg-info/PKG-INFO
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      212 2023-05-08 20:16:43.000000 threadsafe_shell-1.2.0/threadsafe_shell.egg-info/SOURCES.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)        1 2023-05-08 20:16:43.000000 threadsafe_shell-1.2.0/threadsafe_shell.egg-info/dependency_links.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       17 2023-05-08 20:16:43.000000 threadsafe_shell-1.2.0/threadsafe_shell.egg-info/top_level.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)     6423 2023-05-08 20:03:07.000000 threadsafe_shell-1.2.0/threadsafe_shell.py
+drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-09 19:38:55.914741 threadsafe_shell-1.3.0/
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)     1071 2022-11-05 20:17:37.000000 threadsafe_shell-1.3.0/LICENSE
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-09 19:38:55.914741 threadsafe_shell-1.3.0/PKG-INFO
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       88 2022-11-05 20:23:15.000000 threadsafe_shell-1.3.0/README.md
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      565 2023-05-09 19:38:48.000000 threadsafe_shell-1.3.0/pyproject.toml
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       38 2023-05-09 19:38:55.914741 threadsafe_shell-1.3.0/setup.cfg
+drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-09 19:38:55.914741 threadsafe_shell-1.3.0/threadsafe_shell.egg-info/
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-09 19:38:55.000000 threadsafe_shell-1.3.0/threadsafe_shell.egg-info/PKG-INFO
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      212 2023-05-09 19:38:55.000000 threadsafe_shell-1.3.0/threadsafe_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)        1 2023-05-09 19:38:55.000000 threadsafe_shell-1.3.0/threadsafe_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       17 2023-05-09 19:38:55.000000 threadsafe_shell-1.3.0/threadsafe_shell.egg-info/top_level.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)     6548 2023-05-09 19:38:07.000000 threadsafe_shell-1.3.0/threadsafe_shell.py
```

### Comparing `threadsafe_shell-1.2.0/LICENSE` & `threadsafe_shell-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsafe_shell-1.2.0/PKG-INFO` & `threadsafe_shell-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe_shell
-Version: 1.2.0
+Version: 1.3.0
 Summary: A pure-python, thread-safe, queue-based logging and user input module
 Author-email: Calico Kalamari <kalamariking@proton.me>
 Project-URL: Homepage, https://github.com/KalamariKing/threadsafe-shell
 Project-URL: Bug Tracker, https://github.com/KalamariKing/threadsafe-shell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `threadsafe_shell-1.2.0/pyproject.toml` & `threadsafe_shell-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "threadsafe_shell"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name="Calico Kalamari", email="kalamariking@proton.me" },
 ]
 description = "A pure-python, thread-safe, queue-based logging and user input module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `threadsafe_shell-1.2.0/threadsafe_shell.egg-info/PKG-INFO` & `threadsafe_shell-1.3.0/threadsafe_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe-shell
-Version: 1.2.0
+Version: 1.3.0
 Summary: A pure-python, thread-safe, queue-based logging and user input module
 Author-email: Calico Kalamari <kalamariking@proton.me>
 Project-URL: Homepage, https://github.com/KalamariKing/threadsafe-shell
 Project-URL: Bug Tracker, https://github.com/KalamariKing/threadsafe-shell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `threadsafe_shell-1.2.0/threadsafe_shell.py` & `threadsafe_shell-1.3.0/threadsafe_shell.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import readline # adds up/down arrow support in shell
 import threading
 from queue import deque
+import io
 
 class Shell:
     class colors:
         GREY   = "\033[30m"
         GRAY   = "\033[30m"
         RED    = "\033[31m"
         GREEN  = "\033[32m"
@@ -23,53 +24,60 @@
         BLUE   = "\033[44m"
         PURPLE = "\033[45m"
         CYAN   = "\033[46m"
         WHITE  = "\033[47m"
         RESET  = "\033[0m"
     
     
-    def __init__(self, log_file=None, error_file=None, debug_level=3):
-        # io
+    def __init__(self, log_file:io.IOBase=None, error_file:io.IOBase=None, debug_level=3):
+        # stream and file io
         self.__log_file = log_file
+        self.__write_to_log_file = log_file is not None
         self.__error_file = error_file
+        self.__write_to_error_file = error_file is not None
+        # debug info
         self.DEBUG_LEVEL = debug_level
         self.__is_debug_active = True
         # threading
         self.__queue = deque()
         self.__get_write_loop_thread().start()
         self.__queue_lock = threading.Lock()
         self.__file_lock = threading.Lock()
         self.__input_lock = threading.Lock()
+    
+    def set_log_output_file(self, file: io.IOBase):
+        self.__log_file = file
+        self.__write_to_log_file = file is not None
+    
+    def set_error_output_file(self, file: io.IOBase):
+        self.__error_file = file
+        self.__write_to_error_file = file is not None        
 
     
     def __handle_to_file(self, data:dict={}) -> None:
         if "text" not in data: raise KeyError("Key 'text' not found")
         if "is_error" not in data: raise KeyError("Key 'is_error' not found")
-        if "only" not in data: raise KeyError("Key 'only' not found")
         with self.__file_lock:
             # print to console
-            if data["only"] != "file":
-                print(data["text"], end='', flush=True, file=sys.stderr if data["is_error"] else sys.stdout)
+            print(data["text"], end='', flush=True, file=sys.stderr if data["is_error"] else sys.stdout)
             # print to file
-            if data["only"] != "console":
-                file = self.__error_file if data["is_error"] else self.__log_file
-                if not (self.__log_file is None):
-                    print(data["text"], end='', flush=True, file=self.__log_file)
-                if data["is_error"] and not (self.__error_file is None):
-                    print(data["text"], end='', flush=True, file=self.__error_file)
+            if self.__write_to_log_file:
+                print(data["text"], end='', flush=True, file=self.__log_file)
+            if self.__write_to_error_file and data["is_error"]:
+                print(data["text"], end='', flush=True, file=self.__error_file)
+
 
     def __add_to_queue(self, header:str, *args, is_error:bool=False, console_only:bool=False, file_only:bool=False, end='\n', sep=' ') -> None:
         if console_only and file_only: raise AttributeError("console_only and file_only cannot both be True")
         header += "\033[0m"
         end += "\033[0m"
         out = header + sep.join(str(arg) for arg in args) + end
         out.replace('\n', '\n'+header)
-        only = "console" if console_only else "file" if file_only else None
         with self.__queue_lock:
-            self.__queue.append({ "text": out, "is_error": is_error, "only": only })
+            self.__queue.append({ "text": out, "is_error": is_error })
      
     def __write_loop(self):
         while True:
             if len(self.__queue):
                 with self.__queue_lock: val = self.__queue.popleft()
                 self.__handle_to_file(val)
```

