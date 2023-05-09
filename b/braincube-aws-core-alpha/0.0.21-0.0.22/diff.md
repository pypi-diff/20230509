# Comparing `tmp/braincube-aws-core-alpha-0.0.21.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.21.tar", last modified: Mon May  8 13:09:23 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.22.tar", last modified: Mon May  8 14:19:41 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.21.tar` & `braincube-aws-core-alpha-0.0.22.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.212328 braincube-aws-core-alpha-0.0.21/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.21/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 13:09:23.213256 braincube-aws-core-alpha-0.0.21/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.21/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.21/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 13:09:23.217686 braincube-aws-core-alpha-0.0.21/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.21/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.191462 braincube-aws-core-alpha-0.0.21/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.196745 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 13:09:23.000000 braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.197131 braincube-aws-core-alpha-0.0.21/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.200358 braincube-aws-core-alpha-0.0.21/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1289 2023-05-05 18:31:34.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      281 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2434 2023-05-08 10:25:13.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    30110 2023-05-08 12:48:30.000000 braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.203434 braincube-aws-core-alpha-0.0.21/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      623 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4099 2023-05-08 13:07:54.000000 braincube-aws-core-alpha-0.0.21/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.206872 braincube-aws-core-alpha-0.0.21/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3741 2023-05-08 10:21:48.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3631 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 13:09:23.210346 braincube-aws-core-alpha-0.0.21/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.21/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.21/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1437 2023-05-04 08:51:42.000000 braincube-aws-core-alpha-0.0.21/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.910251 braincube-aws-core-alpha-0.0.22/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-02 13:41:49.000000 braincube-aws-core-alpha-0.0.22/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 14:19:41.910528 braincube-aws-core-alpha-0.0.22/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8348 2023-05-03 19:09:10.000000 braincube-aws-core-alpha-0.0.22/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-02 13:42:37.000000 braincube-aws-core-alpha-0.0.22/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      933 2023-05-08 14:19:41.912641 braincube-aws-core-alpha-0.0.22/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-02 13:44:20.000000 braincube-aws-core-alpha-0.0.22/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.895884 braincube-aws-core-alpha-0.0.22/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.901380 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     9101 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      733 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       48 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-05-08 14:19:41.000000 braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.901767 braincube-aws-core-alpha-0.0.22/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.904018 braincube-aws-core-alpha-0.0.22/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1243 2023-05-08 14:04:48.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      248 2023-05-08 13:56:23.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2434 2023-05-08 10:25:13.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    30110 2023-05-08 12:48:30.000000 braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.905482 braincube-aws-core-alpha-0.0.22/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      575 2023-05-08 13:58:47.000000 braincube-aws-core-alpha-0.0.22/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4059 2023-05-08 14:00:15.000000 braincube-aws-core-alpha-0.0.22/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.907900 braincube-aws-core-alpha-0.0.22/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2835 2023-05-08 12:13:01.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3700 2023-05-08 14:01:38.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3597 2023-05-08 14:02:55.000000 braincube-aws-core-alpha-0.0.22/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-05-08 14:19:41.909738 braincube-aws-core-alpha-0.0.22/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-03 05:49:13.000000 braincube-aws-core-alpha-0.0.22/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      580 2023-05-07 19:45:48.000000 braincube-aws-core-alpha-0.0.22/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1391 2023-05-08 14:03:54.000000 braincube-aws-core-alpha-0.0.22/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.21/LICENSE` & `braincube-aws-core-alpha-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/PKG-INFO` & `braincube-aws-core-alpha-0.0.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.21
+Version: 0.0.22
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.21/README.md` & `braincube-aws-core-alpha-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/setup.cfg` & `braincube-aws-core-alpha-0.0.22/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.21
+version = 0.0.22
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.21
+Version: 0.0.22
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-alpha-0.0.21/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.22/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_connection.py` & `braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.22/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.22/src/core/di/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Dict, Tuple, Optional, Generic, TypeVar, Type
+from typing import Generic, TypeVar, Type
 from dataclasses import dataclass
 
 
 class Scope(Enum):
     request = "REQUEST"
     singleton = "SINGLETON"
 
@@ -11,19 +11,19 @@
 T = TypeVar("T")
 
 
 @dataclass()
 class Dependency(Generic[T]):
     scope: Scope
     cls: Type[T]
-    params: List[Tuple[type, Optional[str]]] = None
-    name: Optional[str] = None
-    instance: Optional[T] = None
-    factory: Optional[callable] = None
+    params: list[tuple[type, str | None]] = None
+    name: str | None = None
+    instance: T | None = None
+    factory: callable = None
 
 
-def qualifier_to_data(qualifier: str) -> Dict[str, str]:
+def qualifier_to_data(qualifier: str) -> dict[str, str]:
     d = dict()
     for s in qualifier.split(","):
         q = s.split(":")
         d[q[0]] = q[1]
     return d
```

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.22/src/core/di/injector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import List, Optional, TypeVar, Type
+from typing import TypeVar, Type
 from inspect import signature, isfunction, iscoroutinefunction
 from .data import Dependency, Scope, qualifier_to_data
 
 from ..dal.postgres_connection import Pool, get_pool
 
 T = TypeVar("T")
 
 
 class _Injector:
     """Module that used in order to resolve dependencies from components or route functions."""
 
-    dependencies: List[Dependency] = list()
+    dependencies: list[Dependency] = list()
 
     @staticmethod
-    def inject(name: Optional[str] = None, scope: Scope = Scope.singleton, qualifier: Optional[str] = None):
+    def inject(name: str | None = None, scope: Scope = Scope.singleton, qualifier: str | None = None):
         def _inject(component):
             data = qualifier_to_data(qualifier) if qualifier else dict()
             if isfunction(component):
                 cls = component.__annotations__.get("return")
                 if not cls:
                     raise ValueError(f"injected function '{component.__name__}' must specify return type.")
 
@@ -28,15 +28,15 @@
                 params = [(v.annotation, data.get(k)) for k, v in items_.items()]
                 _Injector.dependencies.append(Dependency(scope, component, params, name))
             return component
 
         return _inject
 
     @staticmethod
-    async def provide(cls: Type[T], name: Optional[str] = None) -> T:
+    async def provide(cls: Type[T], name: str | None = None) -> T:
 
         matched = list(filter(lambda d: (d.cls is cls or issubclass(d.cls, cls)) and
                                         (d.name == name if name else d.name is None), _Injector.dependencies))
 
         if not matched and cls is Pool:
             instance = await get_pool()
             _Injector.dependencies.append(Dependency(Scope.singleton, Pool, instance=instance))
@@ -58,39 +58,39 @@
                 instance = matched[0].cls(*nested)
             if matched[0].scope is Scope.request:
                 return instance
             matched[0].instance = instance
         return matched[0].instance
 
     @staticmethod
-    def register_instance(cls: Type[T], instance: T, name: Optional[str] = None):
+    def register_instance(cls: Type[T], instance: T, name: str | None = None):
         _Injector.dependencies.append(Dependency(Scope.singleton, cls, name=name, instance=instance))
 
 
-def inject(name: Optional[str] = None, scope: Scope = Scope.singleton, qualifier: Optional[str] = None):
+def inject(name: str | None = None, scope: Scope = Scope.singleton, qualifier: str | None = None):
     """Inject a class or function.
     :param name: Component name.
     :param scope: Class of the Scope in which to resolve.
     :param qualifier: Comma separated string, used to specify components by name in case of multiple implementations.
     """
 
     return _Injector.inject(name, scope, qualifier)
 
 
-async def provide(cls: Type[T], name: Optional[str] = None) -> T:
+async def provide(cls: Type[T], name: str | None = None) -> T:
     """Get an instance of the given type.
     :param cls: Interface whose implementation we want.
     :param name: Name of a specific component that implements the interface.
     :returns: An implementation of interface.
     """
 
     return await _Injector.provide(cls, name)
 
 
-def register_instance(cls: Type[T], instance: T, name: Optional[str] = None):
+def register_instance(cls: Type[T], instance: T, name: str | None = None):
     """Create manually and register an instance of a specific type.
     :param cls: Component type.
     :param instance: Component instance.
     :param name: Component name.
     """
 
     return _Injector.register_instance(cls, instance, name)
```

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.22/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.22/src/core/rest/app_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import os
 import time
 import json
 from http import HTTPStatus
 from inspect import signature
 from dataclasses import dataclass
-from typing import List, Tuple, Optional, get_args, get_origin
+from typing import get_args, get_origin
 
 from ..utils.convert import JSONEncoder
 from ..utils.data import import_modules, import_directories
 from ..di.data import qualifier_to_data
 from ..di.injector import provide
 from .data import HTTPRequest, HTTPResponse, http_event_to_request
 from .app_controller import AppController
 
 
 @dataclass()
 class _Route:
     func: callable
-    request_type: Optional[type]
-    dependencies: List[Tuple[type, Optional[str]]]
+    request_type: type | None
+    dependencies: list[tuple[type, str | None]]
 
 
 class AppModule:
     """AWS lambda application main entry point.
     :param controllers: Application controllers.
     :param modules: Modules to force import.
     :param directories: Directories to force import.
     """
 
-    def __init__(self, controllers: List[AppController],
-                 modules: Optional[List[str]] = None,
-                 directories: Optional[List[str]] = None):
+    def __init__(self, controllers: list[AppController],
+                 modules: list[str] | None = None,
+                 directories: list[str] | None = None):
 
         if modules:
             import_modules(modules)
         elif os.environ.get("IMPORT_MODULES"):
             import_modules(os.environ["IMPORT_MODULES"].split(","))
 
         root = os.environ["ROOT_DIRECTORY"] if os.environ.get("ROOT_DIRECTORY") else "/var/task/"
@@ -48,16 +48,16 @@
 
         for c in controllers:
             routes.update(c.routes)
 
         for resource, methods in routes.items():
             for method, handler in methods.items():
 
-                request_type: Optional[type] = None
-                dependencies: List[Tuple[type, Optional[str]]] = list()
+                request_type: type | None = None
+                dependencies: list[tuple[type, str | None]] = list()
                 data = qualifier_to_data(handler[1]) if handler[1] else dict()
 
                 for key, value in signature(handler[0]).parameters.items():
                     origin = get_origin(value.annotation)
                     cls = origin if origin else value.annotation
                     if cls is HTTPRequest:
                         args = get_args(value.annotation)
```

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.22/src/core/rest/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import json
 from dataclasses import dataclass
-from typing import Optional, Dict, List, Generic, TypeVar, Type
+from typing import Generic, TypeVar, Type
 from http import HTTPStatus
 
 from ..utils.convert import try_str_to_float
 from ..utils.data import Order, OrderType, Condition, ConditionType, Pageable
 
 reserved_keys = ["fields", "pageNo", "pageSize", "topSize", "order"]
 
 T = TypeVar("T")
 
 
 @dataclass()
 class HTTPResponse:
     status: HTTPStatus
     body: any = None
-    headers: Dict[str, any] = None
+    headers: dict[str, any] = None
 
 
 @dataclass()
 class QueryParameters:
-    fields: List[str] = None
-    conditions: List[Condition] = None
+    fields: list[str] = None
+    conditions: list[Condition] = None
     page: Pageable = Pageable()
-    order: Optional[List[Order]] = None
+    order: list[Order] | None = None
 
 
 @dataclass()
 class HTTPRequest(Generic[T]):
     query_parameters: QueryParameters = QueryParameters()
-    body: Optional[T] = None
-    headers: Dict[str, any] = None
-    path_parameters: Dict[str, any] = None
+    body: T | None = None
+    headers: dict[str, any] = None
+    path_parameters: dict[str, any] = None
 
 
-def http_event_to_request(cls: Type[T], event: Dict[str, any], context) -> HTTPRequest[T]:
+def http_event_to_request(cls: Type[T], event: dict[str, any], context) -> HTTPRequest[T]:
     data = json.loads(event["body"]) if event.get("body") else None
 
     request = HTTPRequest(QueryParameters(),
                           cls(**data) if cls is not dict else data,
                           event.get("headers"),
                           event.get("pathParameters"))
 
-    params: Optional[Dict[str, any]] = event.get("queryStringParameters")
+    params: dict[str, any] | None = event.get("queryStringParameters")
 
     if params:
         fields = params["fields"].replace(" ", "").split(",") if params.get("fields") else list()
         pageable = Pageable(page_param(params, alias="pageNo", default=0),
                             page_param(params, alias="pageSize", default=20, max_=50),
                             page_param(params, alias="topSize", default=0, max_=1000))
 
@@ -84,15 +84,15 @@
             order.append(Order(order_type, alias=o[0]))
 
         request.query_parameters = QueryParameters(fields, conditions, pageable, order)
 
     return request
 
 
-def page_param(params: Dict[str, any], alias: str, default: int, max_: Optional[int] = None) -> int:
+def page_param(params: dict[str, any], alias: str, default: int, max_: int | None = None) -> int:
     try:
         if not params.get(alias):
             return default
         value_ = int(params[alias])
         return value_ if (max_ >= value_ > 0 if max_ else value_ > 0) else default
     except ValueError:
         return default
```

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.22/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.21/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.22/src/core/utils/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import glob
 import importlib
 from os.path import basename, isfile, join
 
-from typing import Optional, List, Dict
 from enum import Enum
 from dataclasses import dataclass
 
 
 class OrderType(Enum):
     asc = "ASC"
     desc = "DESC"
@@ -31,51 +30,51 @@
     value: any
 
 
 @dataclass()
 class Paging:
     pageNo: int
     pageSize: int
-    totalPages: Optional[int] = None
-    totalCount: Optional[int] = None
+    totalPages: int | None = None
+    totalCount: int | None = None
 
 
 @dataclass
 class Metadata:
     dataElapsed: int
 
 
 @dataclass()
 class Page:
-    data: List[Dict[str, any]]
+    data: list[dict[str, any]]
     paging: Paging
     meta: Metadata = None
 
 
 @dataclass()
 class Top:
-    data: List[Dict[str, any]]
+    data: list[dict[str, any]]
     topSize: int
     hasMore: bool
 
 
 @dataclass
 class Pageable:
     page_no: int = 0
     page_size: int = 20
     top_size: int = 0
 
 
-def import_directories(root: str, paths: List[str]):
+def import_directories(root: str, paths: list[str]):
     for path in paths:
         for module_name in get_module_names(f"{root}{path.replace('.', '/')}"):
             importlib.import_module(f"{path}.{module_name}")
 
 
-def import_modules(paths: List[str]):
+def import_modules(paths: list[str]):
     for path in paths:
         importlib.import_module(path)
 
 
 def get_module_names(path: str):
     modules = glob.glob(join(path, "*.py"))
     return [basename(f)[:-3] for f in modules if isfile(f) and not f.endswith("__init__.py")]
```

