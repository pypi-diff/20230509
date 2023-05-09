# Comparing `tmp/business_validator-1.0.2.tar.gz` & `tmp/business_validator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business_validator-1.0.2.tar", last modified: Tue Mar 28 15:24:03 2023, max compression
+gzip compressed data, was "business_validator-2.0.0.tar", last modified: Tue May  9 13:11:49 2023, max compression
```

## Comparing `business_validator-1.0.2.tar` & `business_validator-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-02-10 10:09:01.557162 business_validator-1.0.2/LICENSE
--rw-r--r--   0        0        0     1678 2023-02-16 20:58:03.025539 business_validator-1.0.2/README.md
--rw-r--r--   0        0        0      289 2023-03-28 12:00:54.186864 business_validator-1.0.2/business_validator/__init__.py
--rw-r--r--   0        0        0     1173 2023-03-07 08:22:20.954784 business_validator-1.0.2/business_validator/types.py
--rw-r--r--   0        0        0     2202 2023-03-28 14:47:56.947972 business_validator-1.0.2/business_validator/validator.py
--rw-r--r--   0        0        0        0 2023-02-10 09:47:42.224957 business_validator-1.0.2/examples/__init__.py
--rw-r--r--   0        0        0     2302 2023-03-28 14:50:36.100888 business_validator-1.0.2/examples/multiple_error.py
--rw-r--r--   0        0        0     1851 2023-03-28 14:33:02.906014 business_validator-1.0.2/examples/single_error.py
--rw-r--r--   0        0        0      389 2023-03-28 13:01:06.373484 business_validator-1.0.2/examples/types.py
--rw-r--r--   0        0        0      812 2023-03-28 15:24:03.880750 business_validator-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-28 12:31:25.057797 business_validator-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0      283 2023-03-28 14:33:43.674482 business_validator-1.0.2/tests/conftest.py
--rw-r--r--   0        0        0      239 2023-03-28 14:00:29.086043 business_validator-1.0.2/tests/factories.py
--rw-r--r--   0        0        0      300 2023-03-28 14:30:58.962078 business_validator-1.0.2/tests/test_multiple_error.py
--rw-r--r--   0        0        0      881 2023-03-28 14:36:51.591453 business_validator-1.0.2/tests/test_single_error.py
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 business_validator-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-02-10 10:09:01.557162 business_validator-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1674 2023-05-09 13:09:52.011288 business_validator-2.0.0/README.md
+-rw-r--r--   0        0        0      289 2023-03-28 12:00:54.186864 business_validator-2.0.0/business_validator/__init__.py
+-rw-r--r--   0        0        0     1285 2023-05-09 13:09:52.011746 business_validator-2.0.0/business_validator/types.py
+-rw-r--r--   0        0        0     3328 2023-05-09 13:09:52.012108 business_validator-2.0.0/business_validator/validator.py
+-rw-r--r--   0        0        0        0 2023-02-10 09:47:42.224957 business_validator-2.0.0/examples/__init__.py
+-rw-r--r--   0        0        0     2298 2023-05-09 13:09:52.012674 business_validator-2.0.0/examples/multiple_error.py
+-rw-r--r--   0        0        0     1847 2023-05-09 13:09:52.013100 business_validator-2.0.0/examples/single_error.py
+-rw-r--r--   0        0        0      389 2023-03-28 13:01:06.373484 business_validator-2.0.0/examples/types.py
+-rw-r--r--   0        0        0      812 2023-05-09 13:11:49.376154 business_validator-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-28 12:31:25.057797 business_validator-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      294 2023-05-09 13:09:52.014537 business_validator-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      239 2023-05-06 17:01:08.159610 business_validator-2.0.0/tests/factories.py
+-rw-r--r--   0        0        0      300 2023-03-28 14:30:58.962078 business_validator-2.0.0/tests/test_multiple_error.py
+-rw-r--r--   0        0        0      881 2023-05-06 16:57:39.505219 business_validator-2.0.0/tests/test_single_error.py
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 business_validator-2.0.0/PKG-INFO
```

### Comparing `business_validator-1.0.2/LICENSE` & `business_validator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `business_validator-1.0.2/README.md` & `business_validator-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 ### DTO Validator
 ```python
 @dataclasses.dataclass()
 class CommentValidator(Validator[ErrorSchema[Source]]):
     dto: CommentDto
 
-    @validate()
+    @validate
     async def test1(self):
         post_ids = list(range(1, 10))
 
         if self.dto.post_id not in post_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
@@ -38,15 +38,15 @@
                     detail=f"Post with id={self.dto.post_id} not found",
                     source=Source(
                         local="data/post_id",
                     ),
                 )
             )
 
-    @validate()
+    @validate
     async def test2(self):
         owner_ids = list(range(1, 10))
 
         if self.dto.owner_id not in owner_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
```

### Comparing `business_validator-1.0.2/business_validator/types.py` & `business_validator-2.0.0/business_validator/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 from enum import Enum
-from collections.abc import Callable, Coroutine
+from collections.abc import Callable, Coroutine, Sequence
 from typing import Any, Generic, TypeAlias, TypeVar
 
 from pydantic.generics import GenericModel
 
 
 _T = TypeVar("_T")
 _S = TypeVar("_S")
@@ -29,20 +29,24 @@
     messages: list[_T]
 
     def __init__(self, messages: list[_T], *args: object) -> None:
         super().__init__(*args)
         self.messages = messages
 
 
-@dataclasses.dataclass()
+@dataclasses.dataclass(frozen=True, slots=True)
 class ValidationContext(Generic[_T]):
     _errors: list[_T] = dataclasses.field(default_factory=list)
 
     def add_error(self, error: _T) -> None:
-        self._errors.append(error)
+        if error not in self._errors:
+            self._errors.append(error)
 
-    def extend_nested_error(self, errors: list[_T]) -> None:
+    def extend_error(self, errors: Sequence[_T]) -> None:
         self._errors.extend(errors)
 
     @property
     def errors(self) -> list[_T]:
         return self._errors
+
+
+SelfValidator: TypeAlias = Any  # heh
```

### Comparing `business_validator-1.0.2/examples/multiple_error.py` & `business_validator-2.0.0/examples/multiple_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class CommentValidator(Validator[ErrorSchema[SourceMultiple]]):
     dto_list: list[CommentDto]
 
     @functools.cached_property
     def context(self) -> CustomValidationContext:  # type: ignore[override]
         return CustomValidationContext()
 
-    @validate()
+    @validate
     async def test1(self):
         post_ids = range(1, 10)
         for i, dto in enumerate(self.dto_list):
             if dto.post_id not in post_ids:
                 self.context.add_error(
                     ErrorSchema(
                         code=ErrorCodeEnum.not_found.value,
@@ -32,15 +32,15 @@
                         source=SourceMultiple(
                             local="data/post_id",
                             position=i,
                         ),
                     )
                 )
 
-    @validate()
+    @validate
     async def test2(self):
         owner_ids = range(1, 10)
         for i, dto in enumerate(self.dto_list):
             if dto.owner_id not in owner_ids:
                 self.context.add_error(
                     ErrorSchema(
                         code=ErrorCodeEnum.not_found.value,
```

### Comparing `business_validator-1.0.2/examples/single_error.py` & `business_validator-2.0.0/examples/single_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,32 +21,31 @@
 )
 
 
 @dataclasses.dataclass()
 class CommentValidator(Validator[ErrorSchema[Source]]):
     dto: CommentDto
 
-    @validate()
+    @validate
     async def test1(self):
         post_ids = list(range(1, 10))
-
         if self.dto.post_id not in post_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
                     message="Id doen't not exists",
                     detail=f"Post with id={self.dto.post_id} not found",
                     source=Source(
                         local="data/post_id",
                     ),
                 )
             )
 
-    @validate()
-    @pre_state(lambda self: self.dto.post_id < 0, negative_id_error)
+    @validate
+    @pre_state(lambda self: self.dto.owner_id > 0, negative_id_error)
     async def test2(self):
         owner_ids = list(range(1, 10))
 
         if self.dto.owner_id not in owner_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
```

### Comparing `business_validator-1.0.2/pyproject.toml` & `business_validator-2.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "business-validator"
-version = "1.0.2"
+version = "2.0.0"
 authors = [
     { name = "maksyutov vlad", email = "maksyutov.vlad@gmail.com" },
 ]
 dependencies = [
     "pydantic>=1.10.4",
 ]
 requires-python = ">=3.11"
```

### Comparing `business_validator-1.0.2/tests/test_single_error.py` & `business_validator-2.0.0/tests/test_single_error.py`

 * *Files identical despite different names*

### Comparing `business_validator-1.0.2/PKG-INFO` & `business_validator-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: business-validator
-Version: 1.0.2
+Version: 2.0.0
 Author-Email: maksyutov vlad <maksyutov.vlad@gmail.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/1PaCHeK1/business-validator
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=1.10.4
 Description-Content-Type: text/markdown
 
@@ -32,15 +32,15 @@
 
 ### DTO Validator
 ```python
 @dataclasses.dataclass()
 class CommentValidator(Validator[ErrorSchema[Source]]):
     dto: CommentDto
 
-    @validate()
+    @validate
     async def test1(self):
         post_ids = list(range(1, 10))
 
         if self.dto.post_id not in post_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
@@ -48,15 +48,15 @@
                     detail=f"Post with id={self.dto.post_id} not found",
                     source=Source(
                         local="data/post_id",
                     ),
                 )
             )
 
-    @validate()
+    @validate
     async def test2(self):
         owner_ids = list(range(1, 10))
 
         if self.dto.owner_id not in owner_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
```

