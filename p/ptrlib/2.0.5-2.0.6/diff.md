# Comparing `tmp/ptrlib-2.0.5-py3-none-any.whl.zip` & `tmp/ptrlib-2.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,35 +1,36 @@
-Zip file size: 114547 bytes, number of entries: 152
+Zip file size: 121875 bytes, number of entries: 158
 -rw-rw-r--  2.0 unx      422 b- defN 23-Jan-21 06:41 ptrlib/__init__.py
 -rw-rw-r--  2.0 unx       28 b- defN 23-Jan-21 06:41 ptrlib/algorithm/__init__.py
 -rw-rw-r--  2.0 unx      116 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/__init__.py
 -rw-rw-r--  2.0 unx      287 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/base.py
 -rw-rw-r--  2.0 unx     1360 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/shortestpath.py
 -rw-rw-r--  2.0 unx      941 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/types.py
 -rw-rw-r--  2.0 unx      102 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/algorithms/__init__.py
 -rw-rw-r--  2.0 unx     3367 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/algorithms/astar.py
 -rw-rw-r--  2.0 unx     1712 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/algorithms/bulkdijkstra.py
 -rw-rw-r--  2.0 unx     2397 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/algorithms/dijkstra.py
 -rw-rw-r--  2.0 unx     2138 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/algorithms/floydwarshall.py
 -rw-rw-r--  2.0 unx       24 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/utils/__init__.py
 -rw-rw-r--  2.0 unx     1021 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/utils/lazylist.py
--rw-rw-r--  2.0 unx       43 b- defN 23-Jan-21 06:41 ptrlib/arch/__init__.py
+-rw-rw-r--  2.0 unx       64 b- defN 23-May-09 08:12 ptrlib/arch/__init__.py
 -rw-rw-r--  2.0 unx      100 b- defN 23-Jan-21 06:41 ptrlib/arch/arm/__init__.py
 -rw-rw-r--  2.0 unx      828 b- defN 23-Jan-21 06:41 ptrlib/arch/arm/archname.py
 -rw-rw-r--  2.0 unx     2964 b- defN 23-Mar-12 15:00 ptrlib/arch/arm/assembler.py
 -rw-rw-r--  2.0 unx     2497 b- defN 23-Mar-12 14:59 ptrlib/arch/arm/disassembler.py
 -rw-rw-r--  2.0 unx    14668 b- defN 23-Jan-21 06:41 ptrlib/arch/arm/syscall.py
 -rw-rw-r--  2.0 unx       75 b- defN 23-Jan-21 06:41 ptrlib/arch/common/__init__.py
 -rw-rw-r--  2.0 unx     3383 b- defN 23-Mar-12 14:53 ptrlib/arch/common/assembler.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-Mar-12 14:44 ptrlib/arch/common/disassembler.py
+-rw-rw-r--  2.0 unx     1860 b- defN 23-Apr-14 22:10 ptrlib/arch/common/disassembler.py
 -rw-rw-r--  2.0 unx      181 b- defN 23-Mar-12 14:55 ptrlib/arch/common/ospath.py
--rw-rw-r--  2.0 unx      100 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/__init__.py
+-rw-rw-r--  2.0 unx      120 b- defN 23-May-09 07:33 ptrlib/arch/intel/__init__.py
 -rw-rw-r--  2.0 unx      853 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/archname.py
 -rw-rw-r--  2.0 unx     2107 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/assembler.py
 -rw-rw-r--  2.0 unx     2072 b- defN 23-Mar-12 14:36 ptrlib/arch/intel/disassembler.py
+-rw-rw-r--  2.0 unx     7138 b- defN 23-May-09 08:00 ptrlib/arch/intel/simd.py
 -rw-rw-r--  2.0 unx    14542 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/syscall.py
 -rw-rw-r--  2.0 unx       45 b- defN 23-Jan-21 06:41 ptrlib/arch/linux/__init__.py
 -rw-rw-r--  2.0 unx      465 b- defN 23-Mar-12 14:56 ptrlib/arch/linux/ospath.py
 -rw-rw-r--  2.0 unx      723 b- defN 23-Jan-21 06:41 ptrlib/arch/linux/syscall.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Jan-21 06:41 ptrlib/binary/__init__.py
 -rw-rw-r--  2.0 unx       67 b- defN 23-Jan-21 06:41 ptrlib/binary/encoding/__init__.py
 -rw-rw-r--  2.0 unx      524 b- defN 23-Jan-21 06:41 ptrlib/binary/encoding/byteconv.py
@@ -72,34 +73,39 @@
 -rw-rw-r--  2.0 unx       26 b- defN 23-Jan-21 06:41 ptrlib/crypto/password/__init__.py
 -rw-rw-r--  2.0 unx     1231 b- defN 23-Jan-21 06:41 ptrlib/crypto/password/bruteforce.py
 -rw-rw-r--  2.0 unx       87 b- defN 23-Jan-21 06:41 ptrlib/crypto/rsa/__init__.py
 -rw-rw-r--  2.0 unx      828 b- defN 23-Jan-21 06:41 ptrlib/crypto/rsa/common_modulus.py
 -rw-rw-r--  2.0 unx      618 b- defN 23-Jan-21 06:41 ptrlib/crypto/rsa/hastads_broadcast.py
 -rw-rw-r--  2.0 unx     1405 b- defN 23-Jan-21 06:41 ptrlib/crypto/rsa/lsb_leak.py
 -rw-rw-r--  2.0 unx       37 b- defN 23-Jan-21 06:41 ptrlib/filestruct/__init__.py
--rw-rw-r--  2.0 unx     7807 b- defN 23-Jan-21 06:41 ptrlib/filestruct/bunkai.py
+-rw-rw-r--  2.0 unx     8785 b- defN 23-Apr-14 23:21 ptrlib/filestruct/bunkai.py
 -rw-rw-r--  2.0 unx       19 b- defN 23-Jan-21 06:41 ptrlib/filestruct/elf/__init__.py
 -rw-rw-r--  2.0 unx    14938 b- defN 23-Apr-01 03:57 ptrlib/filestruct/elf/elf.py
 -rw-rw-r--  2.0 unx    35234 b- defN 23-Jan-21 06:41 ptrlib/filestruct/elf/enums.py
 -rw-rw-r--  2.0 unx     6418 b- defN 23-Jan-21 06:41 ptrlib/filestruct/elf/parser.py
 -rw-rw-r--  2.0 unx     5410 b- defN 23-Jan-21 06:41 ptrlib/filestruct/elf/structs.py
--rw-rw-r--  2.0 unx        7 b- defN 23-Jan-21 06:41 ptrlib/filestruct/pe/__init__.py
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-14 22:24 ptrlib/filestruct/pe/__init__.py
+-rw-rw-r--  2.0 unx      607 b- defN 23-Apr-15 06:18 ptrlib/filestruct/pe/enums.py
+-rw-rw-r--  2.0 unx     6348 b- defN 23-Apr-16 08:05 ptrlib/filestruct/pe/parser.py
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Apr-16 08:17 ptrlib/filestruct/pe/pe.py
+-rw-rw-r--  2.0 unx     8162 b- defN 23-Apr-16 08:04 ptrlib/filestruct/pe/structs.py
 -rw-rw-r--  2.0 unx       62 b- defN 23-Jan-21 06:41 ptrlib/pwn/__init__.py
 -rw-rw-r--  2.0 unx       39 b- defN 23-Jan-21 06:41 ptrlib/pwn/dynlink/__init__.py
 -rw-rw-r--  2.0 unx     1979 b- defN 23-Jan-21 06:41 ptrlib/pwn/dynlink/dl.py
 -rw-rw-r--  2.0 unx     2769 b- defN 23-Jan-21 06:41 ptrlib/pwn/dynlink/robot.py
 -rw-rw-r--  2.0 unx       19 b- defN 23-Jan-21 06:41 ptrlib/pwn/fsb/__init__.py
 -rw-rw-r--  2.0 unx     4546 b- defN 23-Jan-21 06:41 ptrlib/pwn/fsb/fsb.py
 -rw-rw-r--  2.0 unx       23 b- defN 23-Jan-21 06:41 ptrlib/pwn/fuzz/__init__.py
 -rw-rw-r--  2.0 unx     5613 b- defN 23-Jan-21 06:41 ptrlib/pwn/fuzz/randgen.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/algorithm/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/algorithm/shortestpath/__init__.py
 -rw-rw-r--  2.0 unx     3389 b- defN 23-Jan-21 06:41 tests/algorithm/shortestpath/test_shortestpath.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/arch/__init__.py
--rw-rw-r--  2.0 unx     1118 b- defN 23-Jan-21 06:41 tests/arch/test_syscall.py
+-rw-rw-r--  2.0 unx      985 b- defN 23-May-09 08:07 tests/arch/test_simd.py
+-rw-rw-r--  2.0 unx     1120 b- defN 23-May-09 08:02 tests/arch/test_syscall.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/binary/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/binary/encoding/__init__.py
 -rw-rw-r--  2.0 unx      596 b- defN 23-Jan-21 06:41 tests/binary/encoding/test_byteconv.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Jan-21 06:41 tests/binary/encoding/test_locale.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/binary/operation/__init__.py
 -rw-rw-r--  2.0 unx     1273 b- defN 23-Jan-21 06:41 tests/binary/operation/test_rotate.py
 -rw-rw-r--  2.0 unx      654 b- defN 23-Jan-21 06:41 tests/binary/operation/test_xor.py
@@ -113,15 +119,15 @@
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/connection/__init__.py
 -rw-rw-r--  2.0 unx     1414 b- defN 23-Jan-21 06:41 tests/connection/test_proc.py
 -rw-rw-r--  2.0 unx      943 b- defN 23-Jan-21 06:41 tests/connection/test_sock.py
 -rw-rw-r--  2.0 unx     1586 b- defN 23-Feb-16 07:43 tests/connection/test_windows_proc.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/crypto/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/crypto/blockcipher/__init__.py
 -rw-rw-r--  2.0 unx      731 b- defN 23-Jan-21 06:41 tests/crypto/blockcipher/test_ecb.py
--rw-rw-r--  2.0 unx     1652 b- defN 23-Jan-21 06:41 tests/crypto/blockcipher/test_padcbc.py
+-rw-rw-r--  2.0 unx     1809 b- defN 23-May-09 08:15 tests/crypto/blockcipher/test_padcbc.py
 -rw-rw-r--  2.0 unx     1811 b- defN 23-Jan-21 06:41 tests/crypto/blockcipher/test_padding.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/crypto/hash/__init__.py
 -rw-rw-r--  2.0 unx      589 b- defN 23-Jan-21 06:41 tests/crypto/hash/test_crc.py
 -rw-rw-r--  2.0 unx     1862 b- defN 23-Jan-21 06:41 tests/crypto/hash/test_hash.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/crypto/number/__init__.py
 -rw-rw-r--  2.0 unx      696 b- defN 23-Jan-21 06:41 tests/crypto/number/test_crt.py
 -rw-rw-r--  2.0 unx      768 b- defN 23-Jan-21 06:41 tests/crypto/number/test_gcd.py
@@ -141,14 +147,14 @@
 -rw-rw-r--  2.0 unx     1613 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_5.py
 -rw-rw-r--  2.0 unx     1124 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_6.py
 -rw-rw-r--  2.0 unx     1108 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_7.py
 -rw-rw-r--  2.0 unx      574 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_8.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/pwn/__init__.py
 -rw-rw-r--  2.0 unx     1877 b- defN 23-Jan-21 06:41 tests/pwn/test_fsb.py
 -rw-rw-r--  2.0 unx     1988 b- defN 23-Jan-21 06:41 tests/pwn/test_fuzz.py
--rw-rw-r--  2.0 unx     1069 b- defN 23-Apr-01 04:02 ptrlib-2.0.5.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     3535 b- defN 23-Apr-01 04:02 ptrlib-2.0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-01 04:02 ptrlib-2.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Apr-01 04:02 ptrlib-2.0.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-Apr-01 04:02 ptrlib-2.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13318 b- defN 23-Apr-01 04:02 ptrlib-2.0.5.dist-info/RECORD
-152 files, 297808 bytes uncompressed, 93281 bytes compressed:  68.7%
+-rw-rw-r--  2.0 unx     1069 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     3535 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13823 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/RECORD
+158 files, 323978 bytes uncompressed, 99825 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -75,14 +75,17 @@
 
 Filename: ptrlib/arch/intel/assembler.py
 Comment: 
 
 Filename: ptrlib/arch/intel/disassembler.py
 Comment: 
 
+Filename: ptrlib/arch/intel/simd.py
+Comment: 
+
 Filename: ptrlib/arch/intel/syscall.py
 Comment: 
 
 Filename: ptrlib/arch/linux/__init__.py
 Comment: 
 
 Filename: ptrlib/arch/linux/ospath.py
@@ -246,14 +249,26 @@
 
 Filename: ptrlib/filestruct/elf/structs.py
 Comment: 
 
 Filename: ptrlib/filestruct/pe/__init__.py
 Comment: 
 
+Filename: ptrlib/filestruct/pe/enums.py
+Comment: 
+
+Filename: ptrlib/filestruct/pe/parser.py
+Comment: 
+
+Filename: ptrlib/filestruct/pe/pe.py
+Comment: 
+
+Filename: ptrlib/filestruct/pe/structs.py
+Comment: 
+
 Filename: ptrlib/pwn/__init__.py
 Comment: 
 
 Filename: ptrlib/pwn/dynlink/__init__.py
 Comment: 
 
 Filename: ptrlib/pwn/dynlink/dl.py
@@ -282,14 +297,17 @@
 
 Filename: tests/algorithm/shortestpath/test_shortestpath.py
 Comment: 
 
 Filename: tests/arch/__init__.py
 Comment: 
 
+Filename: tests/arch/test_simd.py
+Comment: 
+
 Filename: tests/arch/test_syscall.py
 Comment: 
 
 Filename: tests/binary/__init__.py
 Comment: 
 
 Filename: tests/binary/encoding/__init__.py
@@ -432,26 +450,26 @@
 
 Filename: tests/pwn/test_fsb.py
 Comment: 
 
 Filename: tests/pwn/test_fuzz.py
 Comment: 
 
-Filename: ptrlib-2.0.5.dist-info/LICENSE.txt
+Filename: ptrlib-2.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: ptrlib-2.0.5.dist-info/METADATA
+Filename: ptrlib-2.0.6.dist-info/METADATA
 Comment: 
 
-Filename: ptrlib-2.0.5.dist-info/WHEEL
+Filename: ptrlib-2.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: ptrlib-2.0.5.dist-info/entry_points.txt
+Filename: ptrlib-2.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ptrlib-2.0.5.dist-info/top_level.txt
+Filename: ptrlib-2.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ptrlib-2.0.5.dist-info/RECORD
+Filename: ptrlib-2.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ptrlib/arch/__init__.py

```diff
@@ -1,2 +1,3 @@
+from .intel import *
 from .common import *
 from .linux import *
```

## ptrlib/arch/common/disassembler.py

```diff
@@ -39,18 +39,17 @@
         raise ValueError("Unknown architecture '{}'".format(arch))
 
     if returns == str:
         return '\n'.join(map(lambda v: v[1], l))
     else:
         return l
 
-def disasm(code: bytes,
-           arch: str='x86',
-           mode: str='64',
-           endian: str='little',
+def disasm(code: Union[str, bytes],
            address: int=0,
-           micro: bool=False,
-           mclass: bool=False,
-           v8: bool=False,
-           v9: bool=False,
-           returns: type=list):
-    raise NotImplementedError()
+           bits: Optional[int]=None,
+           arch: Optional[str]='x86-64',
+           syntax: Optional[str]='intel',
+           thumb: Optional[bool]=False,
+           returns: Optional[type]=list,
+           objdump_path: str=None) -> Union[list, str]:
+    return disassemble(code, address, bits, arch, syntax,
+                       thumb, returns, objdump_path)
```

## ptrlib/arch/intel/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .archname import *
 from .assembler import *
 from .disassembler import *
 from .syscall import *
+from .simd import *
```

## ptrlib/filestruct/bunkai.py

```diff
@@ -1,18 +1,20 @@
+# https://github.com/ptr-yudai/bunkai_struct (1559ca2)
 import ctypes
 import io
 from collections import OrderedDict
 
 class BunkaiMember(object):
     def __init__(self, name, struct):
         assert isinstance(struct, Struct) \
             or isinstance(struct, BitStruct) \
             or isinstance(struct, BitInt) \
             or isinstance(struct, Array) \
             or isinstance(struct, VariableArray) \
+            or isinstance(struct, Union) \
             or isinstance(struct, Enum) \
             or isinstance(struct, BunkaiPrimitive)
         self.name = name
         self.struct = struct
 
     def __getattr__(self, key):
         return getattr(self.struct, key)
@@ -67,15 +69,15 @@
     def size(self):
         return (self.bitlen + 7 & ~7) // 8
 
     def __getattr__(self, key):
         return self._members[key]
 
     def __ge__(self, other):
-        assert isinstance(other, str), "Usage: 'name' <= Struct(...)"
+        assert isinstance(other, str), "Usage: 'name' <= BitStruct(...)"
         return BunkaiMember(other, self)
 
     def _parse_stream(self, stream):
         res = {}
         data = stream.read((self.bitlen + 7 & ~7) // 8)
         offset = 0
         for name in self._members:
@@ -90,15 +92,15 @@
         return res
 
 class BitInt(object):
     def __init__(self, bitlen):
         self.bitlen = bitlen
 
     def __ge__(self, other):
-        assert isinstance(other, str), "Usage: 'name' <= Struct(...)"
+        assert isinstance(other, str), "Usage: 'name' <= BitInt(...)"
         return BunkaiMember(other, self)
 
     @property
     def size(self):
         return (self.bitlen + 7 & ~7) // 8
 
     def _parse(self, data):
@@ -142,14 +144,34 @@
             newval = self._ty._parse_stream(stream)
             if not self._repeat_until(newval, res):
                 break
             else:
                 res.append(newval)
         return res
 
+class Union(object):
+    def __init__(self, *args):
+        self._members = args
+        self._size = max(map(lambda member: member.size, self._members))
+
+    def __ge__(self, other):
+        assert isinstance(other, str), "Usage: 'name' <= Union(...)"
+        return BunkaiMember(other, self)
+
+    @property
+    def size(self):
+        return self._size
+
+    def _parse_stream(self, stream):
+        res = {}
+        data = stream.read(self.size)
+        for member in self._members:
+            res[member.name] = member.parse(data)
+        return res
+
 class Enum(object):
     def __init__(self, ty, members=None, startsfrom=None, **kwargs):
         self._ty = ty
         self._items = {}
 
         if members is not None:
             if startsfrom is None:
@@ -224,27 +246,38 @@
 s16be = BunkaiPrimitive(ctypes.c_short, True)
 s32be = BunkaiPrimitive(ctypes.c_int, True)
 s64be = BunkaiPrimitive(ctypes.c_long, True)
 
 if __name__ == '__main__':
     data  = b'\xde\xad\xbe\xef' # magic
     data += b'fizzbuzz\0'       # name
-    data += b'\x01\x27'             # version
+    data += b'\x72\x01'         # version
     data += b'\x11\xf0' + b'\x33\xf1' # children
+    data += b'\xff\xff\xff\xff\xff\xff\xff\xff' + b'\x01' # v1_data
     my_struct = 'MyStruct' <= Struct(
         'magic' <= u32be,
         'name' <= VariableArray(lambda c,_: c!=0, s8),
         'version' <= BitStruct(
             'major' <= BitInt(4),
             'minor' <= BitInt(4),
             'is_beta' <= BitInt(1),
         ),
         'children' <= Array(
             2,
             Struct(
                 'x' <= Enum(u8, CHILD_X1=0x11, CHILD_X2=0x22, CHILD_X3=0x33),
                 'y' <= Enum(u8, ['CHILD_Y1', 'CHILD_Y2'], startsfrom=0xf0),
             )
+        ),
+        'data' <= Union(
+            'v1_data' <= Struct(
+                'value' <= s32,
+                'flag'  <= u8,
+            ),
+            'v2_data' <= Struct(
+                'value' <= s64,
+                'flag'  <= u8,
+            ),
         )
     )
 
     print(my_struct.parse(data))
```

## ptrlib/filestruct/pe/__init__.py

```diff
@@ -1 +1 @@
-# TODO
+from .pe import *
```

## tests/arch/test_syscall.py

```diff
@@ -1,13 +1,13 @@
 import unittest
 from ptrlib import syscall
 from logging import getLogger, FATAL
 
 
-class TestBytes(unittest.TestCase):
+class TestSyscall(unittest.TestCase):
     def setUp(self):
         getLogger("ptrlib").setLevel(FATAL)
 
     def test_syscall(self):
         self.assertEqual(syscall['x86']['read'], 3)
         self.assertEqual(syscall['i386']['read'], 3)
         self.assertEqual(syscall['x86-64']['read'], 0)
```

## tests/crypto/blockcipher/test_padcbc.py

```diff
@@ -8,39 +8,48 @@
 
 
 class TestPaddingOracle(unittest.TestCase):
     def setUp(self):
         getLogger("ptrlib").setLevel(FATAL)
 
     def test_padding_oracle(self):
+        ok_count = 0
         for _ in range(10):
             iv = os.urandom(AES.block_size)
             key = os.urandom(AES.block_size)
             aes = AES.new(key, AES.MODE_CBC, iv=iv)
             m = pad(os.urandom(50), AES.block_size)
             c = aes.encrypt(m)
 
             def try_decrypt(c):
                 try:
                     aes = AES.new(key, AES.MODE_CBC, iv=c[:AES.block_size])
                     unpad(aes.decrypt(c[AES.block_size:]), AES.block_size)
                     return True
                 except:
                     return False
-            self.assertEqual(m, padding_oracle(try_decrypt, c, iv=iv, bs=AES.block_size))
+
+            if m == padding_oracle(try_decrypt, c, iv=iv, bs=AES.block_size):
+                ok_count += 1
+
+        self.assertTrue(ok_count > 7)
 
     def test_padding_oracle_attack(self):
+        ok_count = 0
         for _ in range(10):
             key = os.urandom(AES.block_size)
 
             def try_decrypt(c):
                 try:
                     aes = AES.new(key, AES.MODE_CBC, iv=c[:AES.block_size])
                     unpad(aes.decrypt(c[AES.block_size:]), AES.block_size)
                     return True
                 except:
                     return False
 
             m = pad(os.urandom(50), AES.block_size)
             iv, c = padding_oracle_encrypt(try_decrypt, m, bs=AES.block_size)
             aes = AES.new(key, AES.MODE_CBC, iv=iv)
-            self.assertEqual(m, aes.decrypt(c))
+            if m == aes.decrypt(c):
+                ok_count += 1
+
+        self.assertTrue(ok_count > 7)
```

## Comparing `ptrlib-2.0.5.dist-info/LICENSE.txt` & `ptrlib-2.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `ptrlib-2.0.5.dist-info/METADATA` & `ptrlib-2.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptrlib
-Version: 2.0.5
+Version: 2.0.6
 Summary: CTF library
 Home-page: https://github.com/ptr-yudai/ptrlib/
 Author: ptr-yudai
 Author-email: ptr.yudai+dev@gmail.com
 Keywords: pwn crypto algorithm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
```

## Comparing `ptrlib-2.0.5.dist-info/RECORD` & `ptrlib-2.0.6.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 ptrlib/algorithm/shortestpath/algorithms/__init__.py,sha256=-WGB-FYQD5BP3x5nx9o22iGL195w16CyC0phxv-C6zM,102
 ptrlib/algorithm/shortestpath/algorithms/astar.py,sha256=OQBy7G2AjItRq_3r2Rpl7ZCWy1xY7z_RoOnQuQMVtP8,3367
 ptrlib/algorithm/shortestpath/algorithms/bulkdijkstra.py,sha256=ycZRw-KfsVXxyUh-LElgz0GW0zw8l_wfT3Vxm1AE3bA,1712
 ptrlib/algorithm/shortestpath/algorithms/dijkstra.py,sha256=sMgeyzSy73x_9aaU4EnN3O9nNOvdh24t-TAh3AuOzrg,2397
 ptrlib/algorithm/shortestpath/algorithms/floydwarshall.py,sha256=_X9XwkD7JnqV7WbnN3kewf5aqUryk_mlQ4_eUdBQROw,2138
 ptrlib/algorithm/shortestpath/utils/__init__.py,sha256=qq45vtKASyaZwseOQ2yA3vIO0kCPeVhOp_g2G77dz8c,24
 ptrlib/algorithm/shortestpath/utils/lazylist.py,sha256=tn4i1FV9GY5vthS3DsgomxVFjvVy5DVJpy4rzFkxtQg,1021
-ptrlib/arch/__init__.py,sha256=H0fWFZsXM3lO2p9GuY1W9x4PHLsbIjNZRvptPG5oOnU,43
+ptrlib/arch/__init__.py,sha256=L1Hlv4VYioKNCy2gmx5twUA2VWDzj1pYuCgSvedQbB0,64
 ptrlib/arch/arm/__init__.py,sha256=YQHW2FOm4G_T48qo-u-hBKcCKPbVEMoyb9ob4MWS828,100
 ptrlib/arch/arm/archname.py,sha256=02zPQPpOjBDs8_2SRj9HeZrgS_AcxOPMGAbx_rIUK64,828
 ptrlib/arch/arm/assembler.py,sha256=CXsOuWyLVBK3sFYX95f3UQZ7IuvLP1NR2y9mhgJu3BQ,2964
 ptrlib/arch/arm/disassembler.py,sha256=D3U8E0EhiV1SnZ5karVEeedgbf665q40yZ9iFo-wdXw,2497
 ptrlib/arch/arm/syscall.py,sha256=p8dqUdp2Yk7TnOXAzY11he-vcDhnlRKxBA0IuyXlQBU,14668
 ptrlib/arch/common/__init__.py,sha256=FFz48QFj-90sKaJSYAcnk2IaM5aY7LQmMsK5IgrKryc,75
 ptrlib/arch/common/assembler.py,sha256=IINg5eHILqYd_frtFzTecdoD2qKNTdMy21ym14Zuruw,3383
-ptrlib/arch/common/disassembler.py,sha256=fFDs_elR8lXrUIkrkeEJyOyOg0apXcOMJcO0xoSdugU,1747
+ptrlib/arch/common/disassembler.py,sha256=PwhIw2yTuZ06rDbFwHs-M0tokzqocn5Tan7wAo7dGXM,1860
 ptrlib/arch/common/ospath.py,sha256=Um5rSp8IhNH78ZYUnj3b0DXdSxU-vJbfuC_XjLKva78,181
-ptrlib/arch/intel/__init__.py,sha256=YQHW2FOm4G_T48qo-u-hBKcCKPbVEMoyb9ob4MWS828,100
+ptrlib/arch/intel/__init__.py,sha256=nDKSz9M52xIiwBcEqmnV2s64mPAyg17NLwsX96pCPbo,120
 ptrlib/arch/intel/archname.py,sha256=eAIB2r7eHKow4U5oZtnY6CPsGdN78S5f1UGeJFE2XZs,853
 ptrlib/arch/intel/assembler.py,sha256=n4ri2jH22LJMPHf4LMCeKZC-b3gL_nN3jovTyEsYH-Q,2107
 ptrlib/arch/intel/disassembler.py,sha256=bGR24AGqu7Xh5CCHy2Quw0AqEQZLgO6yd79WKWPFovE,2072
+ptrlib/arch/intel/simd.py,sha256=tgpqur-sY1hQEV1wqTUdZ78TU57W5pTI0sFTMx0l514,7138
 ptrlib/arch/intel/syscall.py,sha256=kgAoR1WAhqsfeJ4BGchrCqZb_nrsnnJ_g3u5loehatY,14542
 ptrlib/arch/linux/__init__.py,sha256=MxDaHplYTwY16ma16lsigtP2a433xLPZe5QdmSdTZMo,45
 ptrlib/arch/linux/ospath.py,sha256=MekrAU-UCw7HDEmMAe4rTPGI-H6nbQTgmXFUIxMuGIw,465
 ptrlib/arch/linux/syscall.py,sha256=g-_eE5xc98rRL1NluKgI00sDUTBdQ2Qb7_dukkONL3M,723
 ptrlib/binary/__init__.py,sha256=Yq7lZzjQbkGObgBhkc4EyxUQNqoSzq8Upy8aAzcqMmY,98
 ptrlib/binary/encoding/__init__.py,sha256=-6TbyfyvxhCcEtvC1C8jJ5guR7xobwUQ3bh3m-duUSM,67
 ptrlib/binary/encoding/byteconv.py,sha256=-kkf6GF4dXm7P3VC3iXXahT0e05xNDOW7wVT1KAXRKQ,524
@@ -71,34 +72,39 @@
 ptrlib/crypto/password/__init__.py,sha256=b1TAaiZNNm_4Ula1XcWpEz0gYVK1GHl9THE1iwm2gSs,26
 ptrlib/crypto/password/bruteforce.py,sha256=Be7fx5TW5x74OsTdRmK2TStOh6BydbsrSV8mWj28BFw,1231
 ptrlib/crypto/rsa/__init__.py,sha256=lif8P5DyVvkRr9w7sULzoKYP4Ow18qG09CmmiZgZ8SI,87
 ptrlib/crypto/rsa/common_modulus.py,sha256=9CBDyh82YL5aN5GqbqtCKu0TC3Fh0TmmwoTnOcW_2Ws,828
 ptrlib/crypto/rsa/hastads_broadcast.py,sha256=FsNChP-s0eCNMLq73wnPEJ1g0Bhy--fmdFPSyxQ6NwQ,618
 ptrlib/crypto/rsa/lsb_leak.py,sha256=mAdebgX_f3EPJwGVB5RvQTR6si1S13O9cFHNsZ3T_BM,1405
 ptrlib/filestruct/__init__.py,sha256=Wy6eJQr-7hORd8vseesNuAzO12Ibx5aparBkJzkQNZY,37
-ptrlib/filestruct/bunkai.py,sha256=lFNg0uERFuxaLv0eU3keaVI5vQQdsJEq5tk90V3OPCU,7807
+ptrlib/filestruct/bunkai.py,sha256=Mng1KawYC4FoQqcRzCftBWBBUKkHvsnzeyqzLP_rCzk,8785
 ptrlib/filestruct/elf/__init__.py,sha256=Qyr5FFu6Las5QoN69F7QOv3dMrfln2UmxpYjcqYovRk,19
 ptrlib/filestruct/elf/elf.py,sha256=pvv9ocZ0pmUzIg1bFBG5MYkZNQJtV7zFBgFPvvftwxc,14938
 ptrlib/filestruct/elf/enums.py,sha256=TMzLlZmQ4CETO8znNQVVbjY5xOkU3gno3DFBC1v__Gg,35234
 ptrlib/filestruct/elf/parser.py,sha256=TMy7XjRqB5UsGwCaSjcq8gQTqSKxWa05AW2t1_dz_YA,6418
 ptrlib/filestruct/elf/structs.py,sha256=lA4C-6KV4oPsfkkxGyH6Ne8QUvopGbSPJ5O-_6pHDW0,5410
-ptrlib/filestruct/pe/__init__.py,sha256=DkeLUlrb7rGx3nZ04aADU9HXXu5mZTf_DBwT0xhzIv4,7
+ptrlib/filestruct/pe/__init__.py,sha256=reIZyIl_6_xja8EiDABCxppz-SIubFmsKqSJ6w88Ld0,18
+ptrlib/filestruct/pe/enums.py,sha256=oMDeE1fXR0UyLzffcNzoeUrX9MPearp_LAZffzzZbb0,607
+ptrlib/filestruct/pe/parser.py,sha256=FBvAitE2jNqDM9m5N5io2mEhd3HXvMo3I4o6UBjbsQg,6348
+ptrlib/filestruct/pe/pe.py,sha256=IV_SbwyB18byEx9VCM84FEGQDqgmrlwpfc824GyiNh0,1123
+ptrlib/filestruct/pe/structs.py,sha256=4ewriZKm_v6bDJrspe9HM731rdt9gAm_vrGU7KbNAzg,8162
 ptrlib/pwn/__init__.py,sha256=_vVnpUu3aXU7v0QlWS0efjg0axTeXtu8dVqiE91EJaM,62
 ptrlib/pwn/dynlink/__init__.py,sha256=VqDqQOGkTHms2jVM37CDYjPLi13Xyvd9PlQBuMoncAc,39
 ptrlib/pwn/dynlink/dl.py,sha256=qCv2Vq9csQ0cYiNXhkazHiVuAGUEamW3-wT9zush6no,1979
 ptrlib/pwn/dynlink/robot.py,sha256=b0K8pGxQoChVPZsX2-3jOTrCFTqlM30hYvq6APQ9SWk,2769
 ptrlib/pwn/fsb/__init__.py,sha256=nlUQAALUrr976oxR3iznuZuSM11vfw1MfOe3tc066uA,19
 ptrlib/pwn/fsb/fsb.py,sha256=OsMPeHXD20NV820D3oMJSNIRIZJmUMuaNTwpqLTfOPA,4546
 ptrlib/pwn/fuzz/__init__.py,sha256=RjOf2xiJg09IktbnSn5CNylxhetu7eoMg8QpUfMFpd4,23
 ptrlib/pwn/fuzz/randgen.py,sha256=v1-SwGR3NfrKAOzXrEzlXmTzVwlfuD08Erpkm9hTXJE,5613
 tests/algorithm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/algorithm/shortestpath/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/algorithm/shortestpath/test_shortestpath.py,sha256=uYKYhsE3K_1FYzuRdhmFFKJulV5qPmIDWN9qVX3fHAk,3389
 tests/arch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/arch/test_syscall.py,sha256=tNFFrZCAnuDEPF9an1wC9jy78-zRWagH3iAulMAvgkM,1118
+tests/arch/test_simd.py,sha256=k43CxIQVCVu6wc_5mHdmWC7vuQCyOyqxxS-sG_8kG98,985
+tests/arch/test_syscall.py,sha256=9D-rplpqv80u80zjDRseufnvjP2vyRDerggoOe1NpmM,1120
 tests/binary/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/binary/encoding/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/binary/encoding/test_byteconv.py,sha256=7EeO-3l1mMGr2lpE2y6VHoFFo49peQT-xRX6R138uTY,596
 tests/binary/encoding/test_locale.py,sha256=ipVE8agDaOABSUBdXhGIRDrKg2SOmVEF8ntaDHYFy84,2787
 tests/binary/operation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/binary/operation/test_rotate.py,sha256=ppoWXsBskZsvmNtT7MlLU65roOq9NKhvzfHAUApD7yU,1273
 tests/binary/operation/test_xor.py,sha256=lw8-DCfeIM9zSZwjM6lTuRrcQiL7qsBKzv2w10O1MyA,654
@@ -112,15 +118,15 @@
 tests/connection/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/connection/test_proc.py,sha256=Zql-0PJXcfWGA6A-VKGnYL2LRHV47PCORvnRfa6U5Qc,1414
 tests/connection/test_sock.py,sha256=YHfBIPRuHdMJWxditwTPV7HNE6gWMBjPAvNej9wCgQQ,943
 tests/connection/test_windows_proc.py,sha256=40pG5-yiteGYkHv3INGQBb_4TCGmfnELoTbp6K7sCMM,1586
 tests/crypto/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/crypto/blockcipher/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/crypto/blockcipher/test_ecb.py,sha256=t90btTdrOX7yjHnfFOp-NDU6znYm__1ETU36j49WLcc,731
-tests/crypto/blockcipher/test_padcbc.py,sha256=-g4FeN-DLjnEnDMJqJiHYFtHTlC6y-kqZfAdshqWqdQ,1652
+tests/crypto/blockcipher/test_padcbc.py,sha256=JRglGsedIlyS7BNQyvGCRTVQr0N5noKfuWgpL1N8ITE,1809
 tests/crypto/blockcipher/test_padding.py,sha256=lvPadMx39yHiX7u2sFp1_ORzedUNa8Axy7v9TygQj28,1811
 tests/crypto/hash/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/crypto/hash/test_crc.py,sha256=OBXpnxL8GJGFVHUy81oIXFxa8umexQMk953mc1ZZlxQ,589
 tests/crypto/hash/test_hash.py,sha256=ef3F93cf2mVFYcgZmRxBCsmWRS4MfYxKeOSNN6iyNXg,1862
 tests/crypto/number/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/crypto/number/test_crt.py,sha256=laSTFs325tBslOKuGvCGOZ30NFwjvogAZczhixkWq5c,696
 tests/crypto/number/test_gcd.py,sha256=o3Bpj6WCmKT7_z0dMUbGkKHx3HeEVDcmSGfke625ipA,768
@@ -140,13 +146,13 @@
 tests/filestruct/elf/test_elf_5.py,sha256=LEi8_R6uog7U3LLkrYAdfrdJH3JJXH8Olv77xPFBIgQ,1613
 tests/filestruct/elf/test_elf_6.py,sha256=XJ7pRu9whJq4wdgfk8ere4q4QbcgONtV-e2ZBo4S544,1124
 tests/filestruct/elf/test_elf_7.py,sha256=uwkPsovbAdZFUJNWZ5XySf0kYtaaPJNs1YDzjYce0-Q,1108
 tests/filestruct/elf/test_elf_8.py,sha256=C1Gnylu5lOqPFo8NfJBo5YyUULe026uKL-hvwWprON0,574
 tests/pwn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/pwn/test_fsb.py,sha256=VC_0csTXIS1_PIGUBJmy2uN7hllr4kXJ0mibNYN5d_A,1877
 tests/pwn/test_fuzz.py,sha256=ARnTx48YnuV-awKeFhjsPAyCYJDn9M80q4DyVj5pvOA,1988
-ptrlib-2.0.5.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-ptrlib-2.0.5.dist-info/METADATA,sha256=OfE8r6FFBfK0M57J_C2JcbbfXodJXB5I-h_vAUftzfc,3535
-ptrlib-2.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ptrlib-2.0.5.dist-info/entry_points.txt,sha256=xJ7v7w7uhxUeAzagSodmQhexYh_8GjCTPDCKMFse9T0,48
-ptrlib-2.0.5.dist-info/top_level.txt,sha256=A_zqZPqp9QidhyWj2_hpnC7wz0tTQ2nbR8D6vOnhzYk,13
-ptrlib-2.0.5.dist-info/RECORD,,
+ptrlib-2.0.6.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+ptrlib-2.0.6.dist-info/METADATA,sha256=yZyByzBSHbQaAitPzHjyrtf-xEY-B0Yv7UpV7cC2sL4,3535
+ptrlib-2.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ptrlib-2.0.6.dist-info/entry_points.txt,sha256=xJ7v7w7uhxUeAzagSodmQhexYh_8GjCTPDCKMFse9T0,48
+ptrlib-2.0.6.dist-info/top_level.txt,sha256=A_zqZPqp9QidhyWj2_hpnC7wz0tTQ2nbR8D6vOnhzYk,13
+ptrlib-2.0.6.dist-info/RECORD,,
```

