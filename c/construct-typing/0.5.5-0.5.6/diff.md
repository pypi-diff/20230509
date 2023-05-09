# Comparing `tmp/construct-typing-0.5.5.tar.gz` & `tmp/construct-typing-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "construct-typing-0.5.5.tar", last modified: Mon Jan  9 14:22:16 2023, max compression
+gzip compressed data, was "construct-typing-0.5.6.tar", last modified: Tue May  9 11:05:47 2023, max compression
```

## Comparing `construct-typing-0.5.5.tar` & `construct-typing-0.5.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:22:16.046483 construct-typing-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-09 14:22:04.000000 construct-typing-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-01-09 14:22:16.046483 construct-typing-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-01-09 14:22:04.000000 construct-typing-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:22:16.042483 construct-typing-0.5.5/construct-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    53655 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/expr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:22:16.042483 construct-typing-0.5.5/construct-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/lib/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/lib/bitstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/lib/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/lib/hex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/lib/py3compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:22:16.042483 construct-typing-0.5.5/construct_typed/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct_typed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct_typed/dataclass_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct_typed/generic_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct_typed/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct_typed/tenum.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-09 14:22:04.000000 construct-typing-0.5.5/construct_typed/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 14:22:16.046483 construct-typing-0.5.5/construct_typing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-01-09 14:22:15.000000 construct-typing-0.5.5/construct_typing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-09 14:22:15.000000 construct-typing-0.5.5/construct_typing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 14:22:15.000000 construct-typing-0.5.5/construct_typing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-09 14:22:15.000000 construct-typing-0.5.5/construct_typing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-09 14:22:15.000000 construct-typing-0.5.5/construct_typing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 14:22:16.046483 construct-typing-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-01-09 14:22:04.000000 construct-typing-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-09 11:05:33.000000 construct-typing-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-09 11:05:47.748647 construct-typing-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-09 11:05:33.000000 construct-typing-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    53656 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28346 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/expr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/bitstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/hex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/lib/py3compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct_typed/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/dataclass_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/generic_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/tenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 11:05:33.000000 construct-typing-0.5.6/construct_typed/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:05:47.748647 construct-typing-0.5.6/construct_typing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 11:05:47.000000 construct-typing-0.5.6/construct_typing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:05:47.748647 construct-typing-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-09 11:05:33.000000 construct-typing-0.5.6/setup.py
```

### Comparing `construct-typing-0.5.5/LICENSE` & `construct-typing-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/PKG-INFO` & `construct-typing-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-typing
-Version: 0.5.5
+Version: 0.5.6
 Summary: Extension for the python package 'construct' that adds typing features
 Home-page: https://github.com/timrid/construct-typing
 Author: Tim Riddermann
 License: MIT
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,annotation,type hint,typing,typed,bitstruct,PEP 561
 Platform: POSIX
 Platform: Windows
```

### Comparing `construct-typing-0.5.5/README.md` & `construct-typing-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/__init__.pyi` & `construct-typing-0.5.6/construct-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/core.pyi` & `construct-typing-0.5.6/construct-stubs/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #   - Higher Kinded Types: https://sobolevn.me/2020/10/higher-kinded-types-in-python
 
 # The type checkers mypy and pyright/pylance unfortunately work a little bit different with __init__ and __new__.
 # For supporting some constructs (eg. Enum, NamedTuple, Slicing) in mypy the __init__ self parameter has to have a
 # type hint. But for supporting pyright/pylance, the same type hint has to be used as the return type of __new__.
 # (see discussion here: https://github.com/python/typeshed/issues/4846).
 
-StreamType = t.BinaryIO
+StreamType = t.IO[bytes]
 FilenameType = t.Union[str, bytes, os.PathLike[str], os.PathLike[bytes]]
 PathType = str
 ContextKWType = t.Any
 
 # ===============================================================================
 # exceptions
 # ===============================================================================
@@ -71,26 +71,26 @@
 class ChecksumError(ConstructError): ...
 class CancelParsing(ConstructError): ...
 
 # ===============================================================================
 # used internally
 # ===============================================================================
 def stream_read(
-    stream: t.BinaryIO, length: int, path: t.Optional[PathType]
+    stream: StreamType, length: int, path: t.Optional[PathType]
 ) -> bytes: ...
-def stream_read_entire(stream: t.BinaryIO, path: t.Optional[PathType]) -> bytes: ...
+def stream_read_entire(stream: StreamType, path: t.Optional[PathType]) -> bytes: ...
 def stream_write(
-    stream: t.BinaryIO, data: bytes, length: int, path: t.Optional[PathType]
+    stream: StreamType, data: bytes, length: int, path: t.Optional[PathType]
 ) -> None: ...
 def stream_seek(
-    stream: t.BinaryIO, offset: int, whence: int, path: t.Optional[PathType]
+    stream: StreamType, offset: int, whence: int, path: t.Optional[PathType]
 ) -> int: ...
-def stream_tell(stream: t.BinaryIO, path: t.Optional[PathType]) -> int: ...
-def stream_size(stream: t.BinaryIO) -> int: ...
-def stream_iseof(stream: t.BinaryIO) -> bool: ...
+def stream_tell(stream: StreamType, path: t.Optional[PathType]) -> int: ...
+def stream_size(stream: StreamType) -> int: ...
+def stream_iseof(stream: StreamType) -> bool: ...
 def evaluate(param: ConstantOrContextLambda2[T], context: Context) -> T: ...
 
 # ===============================================================================
 # abstract constructs
 # ===============================================================================
 ParsedType = t.TypeVar("ParsedType", covariant=True)
 BuildTypes = t.TypeVar("BuildTypes", contravariant=True)
```

### Comparing `construct-typing-0.5.5/construct-stubs/expr.pyi` & `construct-typing-0.5.6/construct-stubs/expr.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/lib/__init__.pyi` & `construct-typing-0.5.6/construct-stubs/lib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/lib/binary.pyi` & `construct-typing-0.5.6/construct-stubs/lib/binary.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/lib/bitstream.pyi` & `construct-typing-0.5.6/construct-stubs/lib/bitstream.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/lib/containers.pyi` & `construct-typing-0.5.6/construct-stubs/lib/containers.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct-stubs/lib/py3compat.pyi` & `construct-typing-0.5.6/construct-stubs/lib/py3compat.pyi`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct_typed/__init__.py` & `construct-typing-0.5.6/construct_typed/__init__.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct_typed/dataclass_struct.py` & `construct-typing-0.5.6/construct_typed/dataclass_struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     library. In the original 'cs.Container' some names like "update", "keys", "items", ... can
     only accessed via key access (square brackets) and not via attribute access (dot operator),
     because they are also method names. This implementation is based on "dataclasses.dataclass"
     which only uses modul-level instead of instance-level helper methods.So no instance-level
     methods exists and every name can be used.
     """
 
+    __dataclass_fields__: "t.ClassVar[t.Dict[str, dataclasses.Field[t.Any]]]"
+
     def __getitem__(self, key: str) -> t.Any:
         return getattr(self, key)
 
     def __setitem__(self, key: str, value: t.Any) -> None:
         setattr(self, key, value)
 
     @recursion_lock()
@@ -206,15 +208,15 @@
 
         # extract all other values from the container, an pass it to the dataclass
         for field in fields:
             if not field.init:
                 value = obj[field.name]
                 setattr(dc, field.name, value)
 
-        return dc
+        return dc  # type: ignore
 
     def _encode(
         self, obj: DataclassType, context: Context, path: PathType
     ) -> t.Dict[str, t.Any]:
         if not isinstance(obj, self.dc_type):
             raise TypeError(f"'{repr(obj)}' has to be of type {repr(self.dc_type)}")
 
@@ -265,8 +267,8 @@
 
 # support legacy names
 TStruct = DataclassStruct
 TBitStruct = DataclassBitStruct
 TContainerMixin = DataclassMixin
 TContainerBase = DataclassMixin
 TStructField = csfield
-sfield = csfield
+sfield = csfield
```

### Comparing `construct-typing-0.5.5/construct_typed/generic_wrapper.py` & `construct-typing-0.5.6/construct_typed/generic_wrapper.py`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/construct_typed/tenum.py` & `construct-typing-0.5.6/construct_typed/tenum.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,14 +70,21 @@
                 new_member._name_ = str(value)
                 new_member._value_ = value
                 new_member.__doc__ = "missing value"
                 pseudo_member = cls._value2member_map_.setdefault(value, new_member)
             return pseudo_member
         return None  # will raise the ValueError in Enum.__new__
 
+    def __reduce_ex__(self, proto: t.Any) -> t.Tuple[t.Any, ...]:
+        """
+        Pickle enums by value instead of name (restores pre-3.11 behavior).
+        See https://github.com/python/cpython/pull/26658 for why this exists.
+        """
+        return self.__class__, (self._value_,)
+
 
 EnumType = t.TypeVar("EnumType", bound=EnumBase)
 
 
 class TEnum(Adapter[int, int, EnumType, EnumType]):
     """
     Typed enum.
@@ -167,14 +174,21 @@
         """
         Returns member (possibly creating it) if one can be found for value.
         """
         new_member = super()._missing_(value)
         new_member.__doc__ = "missing value"
         return new_member
 
+    def __reduce_ex__(self, proto: t.Any) -> t.Tuple[t.Any, ...]:
+        """
+        Pickle enums by value instead of name (restores pre-3.11 behavior).
+        See https://github.com/python/cpython/pull/26658 for why this exists.
+        """
+        return self.__class__, (self._value_,)
+
 
 FlagsEnumType = t.TypeVar("FlagsEnumType", bound=FlagsEnumBase)
 
 
 class TFlagsEnum(Adapter[int, int, FlagsEnumType, FlagsEnumType]):
     """
     Typed enum.
```

### Comparing `construct-typing-0.5.5/construct_typing.egg-info/PKG-INFO` & `construct-typing-0.5.6/construct_typing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: construct-typing
-Version: 0.5.5
+Version: 0.5.6
 Summary: Extension for the python package 'construct' that adds typing features
 Home-page: https://github.com/timrid/construct-typing
 Author: Tim Riddermann
 License: MIT
 Keywords: construct,kaitai,declarative,data structure,struct,binary,symmetric,parser,builder,parsing,building,pack,unpack,packer,unpacker,bitstring,bytestring,annotation,type hint,typing,typed,bitstruct,PEP 561
 Platform: POSIX
 Platform: Windows
```

### Comparing `construct-typing-0.5.5/construct_typing.egg-info/SOURCES.txt` & `construct-typing-0.5.6/construct_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `construct-typing-0.5.5/setup.py` & `construct-typing-0.5.6/setup.py`

 * *Files identical despite different names*

