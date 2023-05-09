# Comparing `tmp/muffin_rest-4.9.0.tar.gz` & `tmp/muffin_rest-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-4.9.0.tar", max compression
+gzip compressed data, was "muffin_rest-5.0.0.tar", max compression
```

## Comparing `muffin_rest-4.9.0.tar` & `muffin_rest-5.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1082 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/LICENSE
--rw-r--r--   0        0        0     2616 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/README.rst
--rw-r--r--   0        0        0     1242 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-05-05 06:47:12.394818 muffin_rest-4.9.0/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/errors.py
--rw-r--r--   0        0        0     5212 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/filters.py
--rw-r--r--   0        0        0    10372 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/handler.py
--rw-r--r--   0        0        0     4842 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8808 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/options.py
--rw-r--r--   0        0        0     5372 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2418 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     1111 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1780 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2813 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6397 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     4058 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/swagger.html
--rw-r--r--   0        0        0      455 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/types.py
--rw-r--r--   0        0        0     2081 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/muffin_rest/utils.py
--rw-r--r--   0        0        0     2670 2023-05-05 06:47:12.398818 muffin_rest-4.9.0/pyproject.toml
--rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-4.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/LICENSE
+-rw-r--r--   0        0        0     2616 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/README.rst
+-rw-r--r--   0        0        0     1242 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5212 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10730 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4971 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8808 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/options.py
+-rw-r--r--   0        0        0     5508 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2418 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     1111 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1780 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2813 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6572 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     4058 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/types.py
+-rw-r--r--   0        0        0     2081 2023-05-09 07:27:39.431963 muffin_rest-5.0.0/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2670 2023-05-09 07:27:39.435962 muffin_rest-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 muffin_rest-5.0.0/PKG-INFO
```

### Comparing `muffin_rest-4.9.0/LICENSE` & `muffin_rest-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/README.rst` & `muffin_rest-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/__init__.py` & `muffin_rest-5.0.0/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/api.py` & `muffin_rest-5.0.0/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/errors.py` & `muffin_rest-5.0.0/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/filters.py` & `muffin_rest-5.0.0/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/handler.py` & `muffin_rest-5.0.0/muffin_rest/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from muffin.handler import Handler, HandlerMeta
 
 from muffin_rest import LIMIT_PARAM, OFFSET_PARAM, openapi
 from muffin_rest.errors import APIError
 
 from .errors import HandlerNotBindedError
 from .options import RESTOptions
-from .types import TVResource
+from .types import TVData, TVResource
 
 if TYPE_CHECKING:
     import marshmallow as ma
     from muffin import Request
 
     from muffin_rest.api import API
     from muffin_rest.filters import Filter
@@ -204,18 +204,34 @@
         offset: int = 0,
     ) -> Tuple[Any, int]:
         """Paginate the results."""
         raise NotImplementedError
 
     # Manage data
     # -----------
+    @overload
+    @abc.abstractmethod
+    async def save(
+        self, request: Request, data: TVResource, *, update=False
+    ) -> TVResource:
+        ...
+
+    @overload
+    @abc.abstractmethod
+    async def save(
+        self, request: Request, data: List[TVResource], *, update=False
+    ) -> List[TVResource]:
+        ...
+
     @abc.abstractmethod
-    async def save(self, request: Request, resource: TVResource) -> TVResource:
+    async def save(
+        self, request: Request, data: TVData[TVResource], *, update=False
+    ) -> TVData[TVResource]:
         """Save the given resource."""
-        return resource
+        return data
 
     @abc.abstractmethod
     async def remove(self, request: Request, resource):
         """Remove the given resource."""
         raise NotImplementedError
 
     # Parse data
@@ -233,38 +249,41 @@
         """Parse data from the given request."""
         try:
             return await request.data(raise_errors=True)
         except (ValueError, TypeError) as exc:
             raise APIError.BAD_REQUEST(str(exc)) from exc
 
     async def load(
-        self,
-        request: Request,
-        resource: Optional[TVResource] = None,
-    ) -> Any:
+        self, request: Request, resource: Optional[TVResource] = None
+    ) -> TVData[TVResource]:
         """Load data from request and create/update a resource."""
         data = await self.parse(request)
         schema = await self.get_schema(request, resource=resource)
         if not schema:
-            return data
+            return cast(TVData[TVResource], data)
 
-        return schema.load(
-            cast(Union[dict, list], data),
-            partial=resource is not None,
-            many=isinstance(data, list),
+        return cast(
+            TVData[TVResource],
+            schema.load(
+                cast(Union[dict, list], data),
+                partial=resource is not None,
+                many=isinstance(data, list),
+            ),
         )
 
     @overload
     async def dump(  # type: ignore[misc]
-        self, request, data, *, many: Literal[True], **opts
+        self, request, data: TVData, *, many: Literal[True], **opts
     ) -> List[TSchemaRes]:
         ...
 
     @overload
-    async def dump(self, request, data, *, many: bool = False, **opts) -> TSchemaRes:
+    async def dump(
+        self, request, data: TVData, *, many: bool = False, **opts
+    ) -> TSchemaRes:
         ...
 
     async def dump(
         self,
         request: Request,
         data: Union[TVResource, Iterable[TVResource]],
         *,
@@ -288,23 +307,16 @@
 
     async def post(self, request: Request, *, resource: Optional[TVResource] = None):
         """Create a resource.
 
         The method accepts a single resource's data or a list of resources to create.
         """
         data = await self.load(request, resource)
-        if isinstance(data, list):
-            return await self.dump(
-                request,
-                data=[await self.save(request, res) for res in data],
-                many=True,
-            )
-
-        res = await self.save(request, data)
-        return await self.dump(request, res)
+        data = await self.save(request, data, update=resource is not None)
+        return await self.dump(request, data, many=isinstance(data, list))
 
     async def put(self, request: Request, *, resource: Optional[TVResource] = None):
         """Update a resource."""
         if resource is None:
             raise APIError.NOT_FOUND()
 
         return await self.post(request, resource=resource)
```

### Comparing `muffin_rest-4.9.0/muffin_rest/mongo/__init__.py` & `muffin_rest-5.0.0/muffin_rest/mongo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 from .types import TVResource
 
 if TYPE_CHECKING:
     import marshmallow as ma
     from motor import motor_asyncio as motor
     from muffin import Request
 
+    from muffin_rest.types import TVData
+
 
 class MongoRESTOptions(RESTOptions):
     """Support Mongo DB."""
 
     filters_cls: Type[MongoFilters] = MongoFilters
     sorting_cls: Type[MongoSorting] = MongoSorting
     schema_base: Type[MongoSchema] = MongoSchema
@@ -107,26 +109,27 @@
         """Initialize marshmallow schema for serialization/deserialization."""
         return self.meta.Schema(
             instance=resource,
             only=request.url.query.get("schema_only"),
             exclude=request.url.query.get("schema_exclude", ()),
         )
 
-    async def save(self, _: Request, resource: TVResource) -> TVResource:
+    async def save(self, _: Request, resource: TVData[TVResource], *, update=False):
         """Save the given resource."""
         meta = self.meta
-        if resource.get(meta.collection_id):
-            await self.collection.replace_one(
-                {meta.collection_id: resource[meta.collection_id]},
-                resource,
-            )
-
-        else:
-            res = await meta.collection.insert_one(resource)
-            resource[meta.collection_id] = res.inserted_id
+        collection_id = meta.collection_id
+        for res in resource if isinstance(resource, list) else [resource]:
+            if update:
+                await self.collection.replace_one(
+                    {collection_id: res[collection_id]}, res
+                )
+
+            else:
+                updated = await meta.collection.insert_one(res)
+                res[collection_id] = updated.inserted_id
 
         return resource
 
     async def remove(self, request: Request, resource: Optional[TVResource] = None):
         """Remove the given resource(s)."""
         meta = self.meta
         oids = (
```

### Comparing `muffin_rest-4.9.0/muffin_rest/mongo/filters.py` & `muffin_rest-5.0.0/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/mongo/schema.py` & `muffin_rest-5.0.0/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/mongo/sorting.py` & `muffin_rest-5.0.0/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/mongo/utils.py` & `muffin_rest-5.0.0/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/openapi.py` & `muffin_rest-5.0.0/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/options.py` & `muffin_rest-5.0.0/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/peewee/__init__.py` & `muffin_rest-5.0.0/muffin_rest/peewee/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 """Support for Peewee ORM (https://github.com/coleifer/peewee)."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Optional, Tuple, Type, Union, cast, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+    overload,
+)
 
 import marshmallow as ma
 import peewee as pw
 from apispec.ext.marshmallow import MarshmallowPlugin
 from marshmallow_peewee import ForeignKey
 from peewee_aio.model import AIOModel, AIOModelSelect
 
@@ -76,29 +86,21 @@
         if resource is None:
             raise APIError.NOT_FOUND("Resource not found")
 
         return resource
 
     @overload
     async def paginate(
-        self: PWRESTBase[TVAIOModel],
-        _: Request,
-        *,
-        limit: int = 0,
-        offset: int = 0,
+        self: PWRESTBase[TVAIOModel], _: Request, *, limit: int = 0, offset: int = 0
     ) -> Tuple[AIOModelSelect[TVAIOModel], int]:
         ...
 
     @overload
     async def paginate(
-        self: PWRESTBase[pw.Model],
-        _: Request,
-        *,
-        limit: int = 0,
-        offset: int = 0,
+        self: PWRESTBase[pw.Model], _: Request, *, limit: int = 0, offset: int = 0
     ) -> Tuple[pw.ModelSelect, int]:
         ...
 
     async def paginate(self, _: Request, *, limit: int = 0, offset: int = 0):
         """Paginate the collection."""
         cqs = cast(pw.ModelSelect, self.collection.order_by())
         if cqs._group_by:  # type: ignore[misc]
@@ -114,21 +116,25 @@
         """Get resource or collection of resources."""
         if resource:
             return await self.dump(request, resource)
 
         resources = await self.meta.manager.fetchall(self.collection)
         return await self.dump(request, resources, many=True)
 
-    async def save(self, _: Request, resource: TVModel) -> TVModel:
+    async def save(
+        self, request: Request, resource: Union[TVModel, List[TVModel]], *, update=False
+    ):
         """Save the given resource."""
         meta = self.meta
-        if issubclass(meta.model, AIOModel):
-            await resource.save()
-        else:
-            await meta.manager.save(resource)
+        manager = meta.manager
+        for res in resource if isinstance(resource, list) else [resource]:
+            if issubclass(meta.model, AIOModel):
+                await res.save()
+            else:
+                await manager.save(res)
 
         return resource
 
     async def remove(self, request: Request, resource: TVModel | None = None):
         """Remove the given resource."""
         meta = self.meta
         if resource:
```

### Comparing `muffin_rest-4.9.0/muffin_rest/peewee/filters.py` & `muffin_rest-5.0.0/muffin_rest/peewee/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/peewee/openapi.py` & `muffin_rest-5.0.0/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/peewee/options.py` & `muffin_rest-5.0.0/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/peewee/schemas.py` & `muffin_rest-5.0.0/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/peewee/sorting.py` & `muffin_rest-5.0.0/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/redoc.html` & `muffin_rest-5.0.0/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/sorting.py` & `muffin_rest-5.0.0/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.0.0/muffin_rest/sqlalchemy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from muffin_rest.sqlalchemy.filters import SAFilters
 from muffin_rest.sqlalchemy.sorting import SASorting
 
 if TYPE_CHECKING:
     from muffin import Request
     from muffin_databases import Plugin as Database
 
+    from muffin_rest.types import TVData
+
 from .types import TVResource
 
 # XXX: Monkey patch ModelConverter
 ModelConverter._get_field_name = lambda _, prop_or_column: str(prop_or_column.key)  # type: ignore[assignment]  # noqa:
 
 
 class SQLAlchemyAutoSchema(BaseSQLAlchemyAutoSchema):
@@ -163,24 +165,28 @@
         """Initialize marshmallow schema for serialization/deserialization."""
         return self.meta.Schema(
             instance=resource,
             only=request.url.query.get("schema_only"),
             exclude=request.url.query.get("schema_exclude", ()),
         )
 
-    async def save(self, _: Request, resource: TVResource) -> TVResource:
+    async def save(self, _: Request, resource: TVData[TVResource], *, update=False):
         """Save the given resource."""
-        table_pk = cast(sa.Column, self.meta.table_pk)
-        if resource.get(table_pk.name):
-            update = self.meta.table.update().where(table_pk == resource[table_pk.name])
-            await self.meta.database.execute(update, resource)
-
-        else:
-            insert = self.meta.table.insert()
-            resource[table_pk.name] = await self.meta.database.execute(insert, resource)
+        meta = self.meta
+        insert_query = meta.table.insert()
+        table_pk = cast(sa.Column, meta.table_pk)
+        for res in resource if isinstance(resource, list) else [resource]:
+            if update:
+                update_query = self.meta.table.update().where(
+                    table_pk == res[table_pk.name]
+                )
+                await meta.database.execute(update_query, res)
+
+            else:
+                res[table_pk.name] = await meta.database.execute(insert_query, resource)
 
         return resource
 
     async def remove(self, request: Request, resource: Optional[TVResource] = None):
         """Remove the given resource."""
         table_pk = cast(sa.Column, self.meta.table_pk)
         pks = [resource[table_pk.name]] if resource else await request.data()
```

### Comparing `muffin_rest-4.9.0/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.0.0/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.0.0/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/swagger.html` & `muffin_rest-5.0.0/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/muffin_rest/utils.py` & `muffin_rest-5.0.0/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-4.9.0/pyproject.toml` & `muffin_rest-5.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "4.9.0"
+version = "5.0.0"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-4.9.0/PKG-INFO` & `muffin_rest-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 4.9.0
+Version: 5.0.0
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

