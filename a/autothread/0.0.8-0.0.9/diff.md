# Comparing `tmp/autothread-0.0.8.tar.gz` & `tmp/autothread-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autothread-0.0.8.tar", last modified: Tue Jan 10 01:18:14 2023, max compression
+gzip compressed data, was "autothread-0.0.9.tar", last modified: Fri Feb 10 20:03:44 2023, max compression
```

## Comparing `autothread-0.0.8.tar` & `autothread-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bas       (1000) bas       (1000)        0 2023-01-10 01:18:14.772951 autothread-0.0.8/
--rw-rw-r--   0 bas       (1000) bas       (1000)     1070 2023-01-07 22:46:53.000000 autothread-0.0.8/LICENSE.txt
--rw-rw-r--   0 bas       (1000) bas       (1000)     3448 2023-01-10 01:18:14.772951 autothread-0.0.8/PKG-INFO
--rw-rw-r--   0 bas       (1000) bas       (1000)     2666 2023-01-10 01:11:01.000000 autothread-0.0.8/README.md
-drwxrwxr-x   0 bas       (1000) bas       (1000)        0 2023-01-10 01:18:14.772951 autothread-0.0.8/autothread/
--rw-rw-r--   0 bas       (1000) bas       (1000)     8664 2023-01-10 01:11:01.000000 autothread-0.0.8/autothread/__init__.py
--rw-rw-r--   0 bas       (1000) bas       (1000)    12192 2023-01-07 22:46:53.000000 autothread-0.0.8/autothread/blocking.py
--rw-rw-r--   0 bas       (1000) bas       (1000)     1133 2023-01-07 22:46:53.000000 autothread-0.0.8/autothread/common.py
--rw-rw-r--   0 bas       (1000) bas       (1000)     3538 2023-01-09 14:46:34.000000 autothread-0.0.8/autothread/non_blocking.py
-drwxrwxr-x   0 bas       (1000) bas       (1000)        0 2023-01-10 01:18:14.772951 autothread-0.0.8/autothread.egg-info/
--rw-rw-r--   0 bas       (1000) bas       (1000)     3448 2023-01-10 01:18:14.000000 autothread-0.0.8/autothread.egg-info/PKG-INFO
--rw-rw-r--   0 bas       (1000) bas       (1000)      303 2023-01-10 01:18:14.000000 autothread-0.0.8/autothread.egg-info/SOURCES.txt
--rw-rw-r--   0 bas       (1000) bas       (1000)        1 2023-01-10 01:18:14.000000 autothread-0.0.8/autothread.egg-info/dependency_links.txt
--rw-rw-r--   0 bas       (1000) bas       (1000)       42 2023-01-10 01:18:14.000000 autothread-0.0.8/autothread.egg-info/requires.txt
--rw-rw-r--   0 bas       (1000) bas       (1000)       11 2023-01-10 01:18:14.000000 autothread-0.0.8/autothread.egg-info/top_level.txt
--rw-rw-r--   0 bas       (1000) bas       (1000)      107 2023-01-10 01:18:14.772951 autothread-0.0.8/setup.cfg
--rw-rw-r--   0 bas       (1000) bas       (1000)     1396 2023-01-10 01:11:01.000000 autothread-0.0.8/setup.py
+drwxrwxr-x   0 bas       (1000) bas       (1000)        0 2023-02-10 20:03:44.158714 autothread-0.0.9/
+-rw-rw-r--   0 bas       (1000) bas       (1000)     1070 2023-01-07 22:46:53.000000 autothread-0.0.9/LICENSE.txt
+-rw-rw-r--   0 bas       (1000) bas       (1000)     3448 2023-02-10 20:03:44.158714 autothread-0.0.9/PKG-INFO
+-rw-rw-r--   0 bas       (1000) bas       (1000)     2666 2023-01-10 01:11:01.000000 autothread-0.0.9/README.md
+drwxrwxr-x   0 bas       (1000) bas       (1000)        0 2023-02-10 20:03:44.158714 autothread-0.0.9/autothread/
+-rw-rw-r--   0 bas       (1000) bas       (1000)     9068 2023-02-10 20:03:30.000000 autothread-0.0.9/autothread/__init__.py
+-rw-rw-r--   0 bas       (1000) bas       (1000)    12557 2023-02-05 19:21:34.000000 autothread-0.0.9/autothread/blocking.py
+-rw-rw-r--   0 bas       (1000) bas       (1000)     1133 2023-01-07 22:46:53.000000 autothread-0.0.9/autothread/common.py
+-rw-rw-r--   0 bas       (1000) bas       (1000)     3694 2023-01-21 22:34:39.000000 autothread-0.0.9/autothread/non_blocking.py
+drwxrwxr-x   0 bas       (1000) bas       (1000)        0 2023-02-10 20:03:44.158714 autothread-0.0.9/autothread.egg-info/
+-rw-rw-r--   0 bas       (1000) bas       (1000)     3448 2023-02-10 20:03:44.000000 autothread-0.0.9/autothread.egg-info/PKG-INFO
+-rw-rw-r--   0 bas       (1000) bas       (1000)      303 2023-02-10 20:03:44.000000 autothread-0.0.9/autothread.egg-info/SOURCES.txt
+-rw-rw-r--   0 bas       (1000) bas       (1000)        1 2023-02-10 20:03:44.000000 autothread-0.0.9/autothread.egg-info/dependency_links.txt
+-rw-rw-r--   0 bas       (1000) bas       (1000)       42 2023-02-10 20:03:44.000000 autothread-0.0.9/autothread.egg-info/requires.txt
+-rw-rw-r--   0 bas       (1000) bas       (1000)       11 2023-02-10 20:03:44.000000 autothread-0.0.9/autothread.egg-info/top_level.txt
+-rw-rw-r--   0 bas       (1000) bas       (1000)      107 2023-02-10 20:03:44.162714 autothread-0.0.9/setup.cfg
+-rw-rw-r--   0 bas       (1000) bas       (1000)     1396 2023-01-21 22:04:45.000000 autothread-0.0.9/setup.py
```

### Comparing `autothread-0.0.8/LICENSE.txt` & `autothread-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autothread-0.0.8/PKG-INFO` & `autothread-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autothread
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/Basdbruijne/autothread
 Author: Bas de Bruijne
 Author-email: basdbruijne@gmail.com
 License: MIT
 Keywords: multithreading,multiprocessing,decorator
 Platform: UNKNOWN
```

### Comparing `autothread-0.0.8/README.md` & `autothread-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `autothread-0.0.8/autothread/__init__.py` & `autothread-0.0.9/autothread/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022 by Bas de Bruijne
 # All rights reserved.
 # autothread comes with ABSOLUTELY NO WARRANTY, the writer can not be
 # held responsible for any problems caused by the use of this module.
 
 __author__ = "Bas de Bruijne"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import functools
 import inspect
 import multiprocess as mp
 import psutil
 import queue
 import threading
@@ -48,41 +48,45 @@
 
     def __init__(
         self,
         n_workers: int = None,
         mb_mem: int = None,
         workers_per_core: int = None,
         progress_bar: bool = False,
+        ignore_errors: bool = False,
     ):
         """Initialize the autothread decorator
 
         :param n_workers: Total number of workers to run in parallel (0 for unlimited,
         (default) None for the amount of cores).
         :param mb_mem: Minimum megabytes of memory for each worker.
         :param workers_per_core: Number of workers to run per core.
         :param progress_bar: Visualize how many of the tasks are completed
+        :param ignore_errors: Return `None` when an error is encountered
         """
         if callable(n_workers):
             raise SyntaxError(
                 f"{self.__class__.__name__} received an unexpected value."
                 f"\n@autothread.{self.__class__.__name__}() <- Did you forget the ()?"
                 f"\n{' '*(len(self.__class__.__name__)+12)}~~"
             )
 
         self.n_workers = self._get_workers(n_workers, mb_mem, workers_per_core)
         self.process_bar = progress_bar
+        self.ignore_errors = ignore_errors
 
     def __call__(self, function: Callable):
         decorator = _Autothread(
             function=function,
             Process=self.Process,
             Queue=self.Queue,
             Semaphore=self.Semaphore,
             n_workers=self.n_workers,
             progress_bar=self.process_bar,
+            ignore_errors=self.ignore_errors,
         )
 
         @functools.wraps(function)
         def wrapper(*args, **kwargs):
             return decorator(*args, **kwargs)
 
         wrapper.__doc__ = decorator.__doc__
@@ -172,27 +176,30 @@
     Semaphore = threading.Semaphore
 
     def __init__(
         self,
         n_workers: int = None,
         mb_mem: int = None,
         workers_per_core: int = None,
+        ignore_errors: int = False,
     ):
         """Initialize the autothread decorator
 
         :param n_workers: Total number of workers to run in parallel (0 for unlimited,
         (default) None for the amount of cores).
         :param mb_mem: Minimum megabytes of memory for each worker.
         :param workers_per_core: Number of workers to run per core.
+        :param ignore_errors: Return `None` when an error is encountered
         """
 
         super().__init__(n_workers, mb_mem, workers_per_core)
         self.semaphore = self.Semaphore(
             self.n_workers if self.n_workers > 0 else int(1e9)
         )
+        self.ignore_errors = ignore_errors
 
     def __call__(self, function):
         return_type = inspect.signature(function).return_annotation
         if return_type == inspect._empty:
             warnings.warn(
                 "The designed return type of this function could not be verified, which"
                 " will result in a placeholder that does not act identially to the"
@@ -200,14 +207,15 @@
             )
             return_type = None
 
         class Placeholder(_Placeholder):
             ___semaphore___ = self.semaphore
             ___Queue___ = self.Queue
             ___Process___ = self.Process
+            ___ignore_errors___ = self.ignore_errors
             if not return_type is None:
                 __type__ = return_type
                 __metaclass__ = return_type
             if hasattr(return_type, "__name__"):
                 __name__ = return_type.__name__
             if hasattr(return_type, "__qualname__"):
                 __qualname__ = return_type.__qualname__
```

### Comparing `autothread-0.0.8/autothread/blocking.py` & `autothread-0.0.9/autothread/blocking.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,35 @@
         self,
         function: Callable,
         Process: Union[Type[threading.Thread], Type[mp.Process]],
         Queue: Union[Type[queue.Queue], Type[mp.Queue]],
         Semaphore: Union[Type[threading.Semaphore], Type[mp.Semaphore]],
         n_workers: int,
         progress_bar: bool,
+        ignore_errors: bool,
     ):
         """Initialize the decorator
 
         :param function: function to decorate
         :param Process: Process/thread class
         :param Queue: Queue class
         :param Semaphore: Semaphore class
         :param n_workers: Total number of workers to use
-        :oaram progress_bar: Whether to show a progress bar
+        :param progress_bar: Whether to show a progress bar
+        :param ignore_errors: Return `None` when an error is encountered
         """
         self._Process = Process
         self._Queue = Queue
         self._Semaphore = Semaphore
         self._function = function
         self.n_workers = n_workers
         self._params = inspect.signature(self._function).parameters
         self._progress_bar = progress_bar
         self._is_listy = lambda x: isinstance(x, list) or isinstance(x, tuple)
+        self._ignore_errors = ignore_errors
 
     @property
     def __signature__(self):
         """Updates the __signature__ to match the received function"""
         signature = inspect.signature(self._function)
         new_params = []
         for k in self._params:
@@ -288,25 +291,31 @@
                     content, "autothread_intercepted", False
                 ):
                     try:
                         self._kill_all()
                     except KeyboardInterrupt:
                         # The main thread can accidentally be killed on some platforms
                         pass
-                    raise content
+                    if self._ignore_errors:
+                        return {list(res)[0]: None}
+                    else:
+                        raise content
                 return res
 
     def _kill_all(self):
         """Terminates all running processes by sending them a keyboard interrupt"""
         if self._Process == threading.Thread:
             p_names = [p.name for p in self._processes]
             for id, thread in threading._active.copy().items():
                 if thread.name in p_names:
                     ctypes.pythonapi.PyThreadState_SetAsyncExc(
                         ctypes.c_long(id),
                         ctypes.py_object(KeyboardInterrupt),
                     )
         else:
             for process in self._processes:
-                os.kill(process.pid, getattr(signal, "CTRL_C_EVENT", signal.SIGINT))
+                try:
+                    os.kill(process.pid, getattr(signal, "CTRL_C_EVENT", signal.SIGINT))
+                except ProcessLookupError:
+                    pass
         for process in self._processes:
             process.join()
```

### Comparing `autothread-0.0.8/autothread/common.py` & `autothread-0.0.9/autothread/common.py`

 * *Files identical despite different names*

### Comparing `autothread-0.0.8/autothread/non_blocking.py` & `autothread-0.0.9/autothread/non_blocking.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class _Placeholder:
     """Base class for a non-blocking decorator that makes any function threaded"""
 
     ___semaphore___: Union[threading.Semaphore, mp.Semaphore] = None
     ___Queue___: Union[Type[queue.Queue], Type[mp.Queue]] = None
     ___Process___: Union[Type[threading.Thread], Type[mp.Process]] = None
+    ___ignore_errors___: bool = False
 
     @classmethod
     def ___forwarder___(cls, attr: str) -> Callable:
         """Returns function to forward dunders to the original type
 
         Dunders are not processed through __getattribute__, so we need to inspect the
         originional return type and add all the dunders that are present there.
@@ -47,15 +48,18 @@
         if not self.___response_collected___:
             self.___process___.join()
             self.___response___ = list(self.___queue___.get().values())[0]
             self.___response_collected___ = True
             if isinstance(self.___response___, Exception) and getattr(
                 self.___response___, "autothread_intercepted", False
             ):
-                raise self.___response___
+                if self.___ignore_errors___:
+                    self.___response___ = None
+                else:
+                    raise self.___response___
         return self.___response___
 
     def __getattribute__(self, __name: str) -> Any:
         """Forwards attribute request to function response
 
         The placeholder itself uses thrunders ("___attr___") as internal attributed. If
         the attribute is not a thrunder, wait for the response and forward it there.
```

### Comparing `autothread-0.0.8/autothread.egg-info/PKG-INFO` & `autothread-0.0.9/autothread.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autothread
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/Basdbruijne/autothread
 Author: Bas de Bruijne
 Author-email: basdbruijne@gmail.com
 License: MIT
 Keywords: multithreading,multiprocessing,decorator
 Platform: UNKNOWN
```

### Comparing `autothread-0.0.8/setup.py` & `autothread-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'autothread',
   packages = ['autothread'],
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Bas de Bruijne',
   author_email = 'basdbruijne@gmail.com',
   url = 'https://github.com/Basdbruijne/autothread',
   keywords = ['multithreading', 'multiprocessing', 'decorator'],
```

