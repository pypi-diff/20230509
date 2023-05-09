# Comparing `tmp/toolforge-weld-0.1.tar.gz` & `tmp/toolforge-weld-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge-weld-0.1.tar", last modified: Tue May  9 08:55:04 2023, max compression
+gzip compressed data, was "toolforge-weld-0.1.0.1.tar", last modified: Tue May  9 08:59:02 2023, max compression
```

## Comparing `toolforge-weld-0.1.tar` & `toolforge-weld-0.1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:55:04.664418 toolforge-weld-0.1/
--rw-r--r--   0 taavi     (1000) taavi     (1000)    34524 2023-05-05 13:07:36.000000 toolforge-weld-0.1/LICENSE
--rw-r--r--   0 taavi     (1000) taavi     (1000)      249 2023-05-09 08:55:04.664418 toolforge-weld-0.1/PKG-INFO
--rw-r--r--   0 taavi     (1000) taavi     (1000)       78 2023-05-08 15:26:37.000000 toolforge-weld-0.1/README.md
--rw-r--r--   0 taavi     (1000) taavi     (1000)      449 2023-05-08 15:26:37.000000 toolforge-weld-0.1/pyproject.toml
--rw-r--r--   0 taavi     (1000) taavi     (1000)       38 2023-05-09 08:55:04.664418 toolforge-weld-0.1/setup.cfg
--rw-r--r--   0 taavi     (1000) taavi     (1000)      452 2023-05-09 08:54:16.000000 toolforge-weld-0.1/setup.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:55:04.660417 toolforge-weld-0.1/tests/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      385 2023-05-08 15:26:37.000000 toolforge-weld-0.1/tests/test_kubernetes.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)      418 2023-05-08 15:26:37.000000 toolforge-weld-0.1/tests/test_utils.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:55:04.664418 toolforge-weld-0.1/toolforge_weld/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      176 2023-05-08 15:26:37.000000 toolforge-weld-0.1/toolforge_weld/__init__.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)     1590 2023-05-08 15:26:37.000000 toolforge-weld-0.1/toolforge_weld/errors.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)     9744 2023-05-09 08:54:16.000000 toolforge-weld-0.1/toolforge_weld/kubernetes.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:55:04.664418 toolforge-weld-0.1/toolforge_weld/logs/
--rw-r--r--   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:54:16.000000 toolforge-weld-0.1/toolforge_weld/logs/__init__.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)     2466 2023-05-09 08:54:16.000000 toolforge-weld-0.1/toolforge_weld/logs/kubernetes.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)      441 2023-05-09 08:54:16.000000 toolforge-weld-0.1/toolforge_weld/logs/source.py
--rw-r--r--   0 taavi     (1000) taavi     (1000)        0 2023-05-08 15:26:37.000000 toolforge-weld-0.1/toolforge_weld/py.typed
--rw-r--r--   0 taavi     (1000) taavi     (1000)      182 2023-05-08 15:26:37.000000 toolforge-weld-0.1/toolforge_weld/utils.py
-drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:55:04.664418 toolforge-weld-0.1/toolforge_weld.egg-info/
--rw-r--r--   0 taavi     (1000) taavi     (1000)      249 2023-05-09 08:55:04.000000 toolforge-weld-0.1/toolforge_weld.egg-info/PKG-INFO
--rw-r--r--   0 taavi     (1000) taavi     (1000)      500 2023-05-09 08:55:04.000000 toolforge-weld-0.1/toolforge_weld.egg-info/SOURCES.txt
--rw-r--r--   0 taavi     (1000) taavi     (1000)        1 2023-05-09 08:55:04.000000 toolforge-weld-0.1/toolforge_weld.egg-info/dependency_links.txt
--rw-r--r--   0 taavi     (1000) taavi     (1000)       32 2023-05-09 08:55:04.000000 toolforge-weld-0.1/toolforge_weld.egg-info/requires.txt
--rw-r--r--   0 taavi     (1000) taavi     (1000)       15 2023-05-09 08:55:04.000000 toolforge-weld-0.1/toolforge_weld.egg-info/top_level.txt
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)    34524 2023-05-05 13:07:36.000000 toolforge-weld-0.1.0.1/LICENSE
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      253 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/PKG-INFO
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       78 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/README.md
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      449 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/pyproject.toml
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       38 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/setup.cfg
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      454 2023-05-09 08:58:57.000000 toolforge-weld-0.1.0.1/setup.py
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/tests/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      385 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/tests/test_kubernetes.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      418 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/tests/test_utils.py
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/toolforge_weld/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      176 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/__init__.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)     1590 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/errors.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)    10043 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/kubernetes.py
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/toolforge_weld/logs/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      535 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/logs/__init__.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)     2457 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/logs/kubernetes.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      544 2023-05-09 08:56:46.000000 toolforge-weld-0.1.0.1/toolforge_weld/logs/source.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)        0 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/py.typed
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      182 2023-05-08 15:26:37.000000 toolforge-weld-0.1.0.1/toolforge_weld/utils.py
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2023-05-09 08:59:02.677255 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      253 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/PKG-INFO
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      500 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/SOURCES.txt
+-rw-r--r--   0 taavi     (1000) taavi     (1000)        1 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/dependency_links.txt
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       32 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/requires.txt
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       15 2023-05-09 08:59:02.000000 toolforge-weld-0.1.0.1/toolforge_weld.egg-info/top_level.txt
```

### Comparing `toolforge-weld-0.1/LICENSE` & `toolforge-weld-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.1/toolforge_weld/errors.py` & `toolforge-weld-0.1.0.1/toolforge_weld/errors.py`

 * *Files identical despite different names*

### Comparing `toolforge-weld-0.1/toolforge_weld/kubernetes.py` & `toolforge-weld-0.1.0.1/toolforge_weld/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,25 +114,33 @@
     def _make_kwargs(self, url: str, **kwargs):
         """Setup kwargs for a Requests request."""
         version = kwargs.pop("version", "v1")
         if version == "v1":
             root = "api"
         else:
             root = "apis"
+
+        # use "or" syntax in case namespace is present but set as None
+        namespace = kwargs.pop("namespace", None) or self.namespace
+
         kwargs["url"] = "{}/{}/{}/namespaces/{}/{}".format(
-            self.server, root, version, self.namespace, url
+            self.server, root, version, namespace, url
         )
+
         name = kwargs.pop("name", None)
         if name is not None:
             kwargs["url"] = "{}/{}".format(kwargs["url"], name)
+
         subpath = kwargs.pop("subpath", None)
         if subpath is not None:
             kwargs["url"] = "{}{}".format(kwargs["url"], subpath)
+
         if "timeout" not in kwargs:
             kwargs["timeout"] = self.timeout
+
         return kwargs
 
     def _get(self, url, **kwargs):
         """GET request."""
         r = self.session.get(**self._make_kwargs(url, **kwargs))
         r.raise_for_status()
         return r.json()
@@ -155,28 +163,32 @@
         r.raise_for_status()
         return r.status_code
 
     def get_object(
         self,
         kind: str,
         name: str,
+        *,
+        namespace: Optional[str] = None,
     ) -> Dict[str, Any]:
         """Get the object with the specified name and of the given kind in the namespace."""
         return self._get(
             kind,
             name=name,
             version=K8sClient.VERSIONS[kind],
+            namespace=namespace,
         )
 
     def get_objects(
         self,
         kind: str,
         *,
         label_selector: Optional[Dict[str, str]] = None,
         field_selector: Optional[Dict[str, Any]] = None,
+        namespace: Optional[str] = None,
     ) -> List[Dict[str, Any]]:
         """Get list of objects of the given kind in the namespace."""
         params: Dict[str, Any] = {}
 
         if label_selector:
             params["labelSelector"] = ",".join(
                 [f"{k}={v}" for k, v in label_selector.items()]
@@ -184,14 +196,15 @@
         if field_selector:
             params["fieldSelector"] = field_selector
 
         return self._get(
             kind,
             params=params,
             version=K8sClient.VERSIONS[kind],
+            namespace=namespace,
         )["items"]
 
     def delete_objects(
         self,
         kind: str,
         *,
         label_selector: Optional[Dict[str, str]] = None,
```

### Comparing `toolforge-weld-0.1/toolforge_weld/logs/kubernetes.py` & `toolforge-weld-0.1.0.1/toolforge_weld/logs/kubernetes.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,14 @@
             "follow": follow,
             "pretty": True,
             "timestamps": True,
         }
         if lines:
             params["tailLines"] = lines
         timeout = None if follow else self.client.timeout
-        instance = f"{pod_name}/{container_name}"
 
         with self.client.session.get(
             **self.client._make_kwargs(
                 "pods",
                 name=pod_name,
                 subpath="/log",
                 params=params,
@@ -45,15 +44,16 @@
             stream=True,
         ) as r:
             r.raise_for_status()
             for line in r.iter_lines():
                 content = line.decode("utf-8")
                 datetime, message = content.split(" ", 1)
                 yield LogEntry(
-                    instance=instance,
+                    pod=pod_name,
+                    container=container_name,
                     datetime=parse_date(datetime),
                     message=message,
                 )
 
     def query(
         self, *, selector: Dict[str, str], follow: bool, lines: Optional[int]
     ) -> Iterator[LogEntry]:
```

