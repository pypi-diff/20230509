# Comparing `tmp/ptrlib-2.0.6-py3-none-any.whl.zip` & `tmp/ptrlib-2.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 121875 bytes, number of entries: 158
+Zip file size: 123294 bytes, number of entries: 161
 -rw-rw-r--  2.0 unx      422 b- defN 23-Jan-21 06:41 ptrlib/__init__.py
 -rw-rw-r--  2.0 unx       28 b- defN 23-Jan-21 06:41 ptrlib/algorithm/__init__.py
 -rw-rw-r--  2.0 unx      116 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/__init__.py
 -rw-rw-r--  2.0 unx      287 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/base.py
 -rw-rw-r--  2.0 unx     1360 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/shortestpath.py
 -rw-rw-r--  2.0 unx      941 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/types.py
 -rw-rw-r--  2.0 unx      102 b- defN 23-Jan-21 06:41 ptrlib/algorithm/shortestpath/algorithms/__init__.py
@@ -18,25 +18,27 @@
 -rw-rw-r--  2.0 unx     2964 b- defN 23-Mar-12 15:00 ptrlib/arch/arm/assembler.py
 -rw-rw-r--  2.0 unx     2497 b- defN 23-Mar-12 14:59 ptrlib/arch/arm/disassembler.py
 -rw-rw-r--  2.0 unx    14668 b- defN 23-Jan-21 06:41 ptrlib/arch/arm/syscall.py
 -rw-rw-r--  2.0 unx       75 b- defN 23-Jan-21 06:41 ptrlib/arch/common/__init__.py
 -rw-rw-r--  2.0 unx     3383 b- defN 23-Mar-12 14:53 ptrlib/arch/common/assembler.py
 -rw-rw-r--  2.0 unx     1860 b- defN 23-Apr-14 22:10 ptrlib/arch/common/disassembler.py
 -rw-rw-r--  2.0 unx      181 b- defN 23-Mar-12 14:55 ptrlib/arch/common/ospath.py
--rw-rw-r--  2.0 unx      120 b- defN 23-May-09 07:33 ptrlib/arch/intel/__init__.py
+-rw-rw-r--  2.0 unx      139 b- defN 23-May-09 08:24 ptrlib/arch/intel/__init__.py
 -rw-rw-r--  2.0 unx      853 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/archname.py
 -rw-rw-r--  2.0 unx     2107 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/assembler.py
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-09 12:08 ptrlib/arch/intel/cpu.py
 -rw-rw-r--  2.0 unx     2072 b- defN 23-Mar-12 14:36 ptrlib/arch/intel/disassembler.py
--rw-rw-r--  2.0 unx     7138 b- defN 23-May-09 08:00 ptrlib/arch/intel/simd.py
+-rw-rw-r--  2.0 unx     7142 b- defN 23-May-09 08:24 ptrlib/arch/intel/simd.py
 -rw-rw-r--  2.0 unx    14542 b- defN 23-Jan-21 06:41 ptrlib/arch/intel/syscall.py
 -rw-rw-r--  2.0 unx       45 b- defN 23-Jan-21 06:41 ptrlib/arch/linux/__init__.py
 -rw-rw-r--  2.0 unx      465 b- defN 23-Mar-12 14:56 ptrlib/arch/linux/ospath.py
 -rw-rw-r--  2.0 unx      723 b- defN 23-Jan-21 06:41 ptrlib/arch/linux/syscall.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Jan-21 06:41 ptrlib/binary/__init__.py
--rw-rw-r--  2.0 unx       67 b- defN 23-Jan-21 06:41 ptrlib/binary/encoding/__init__.py
+-rw-rw-r--  2.0 unx       90 b- defN 23-May-09 11:53 ptrlib/binary/encoding/__init__.py
+-rw-rw-r--  2.0 unx      220 b- defN 23-May-09 11:55 ptrlib/binary/encoding/bitconv.py
 -rw-rw-r--  2.0 unx      524 b- defN 23-Jan-21 06:41 ptrlib/binary/encoding/byteconv.py
 -rw-rw-r--  2.0 unx     1552 b- defN 23-Jan-21 06:41 ptrlib/binary/encoding/locale.py
 -rw-rw-r--  2.0 unx      520 b- defN 23-Jan-21 06:41 ptrlib/binary/encoding/table.py
 -rw-rw-r--  2.0 unx       41 b- defN 23-Jan-21 06:41 ptrlib/binary/operation/__init__.py
 -rw-rw-r--  2.0 unx     1374 b- defN 23-Jan-21 06:41 ptrlib/binary/operation/rotate.py
 -rw-rw-r--  2.0 unx     1048 b- defN 23-Jan-21 06:41 ptrlib/binary/operation/xor.py
 -rw-rw-r--  2.0 unx       84 b- defN 23-Jan-21 06:41 ptrlib/binary/packing/__init__.py
@@ -96,15 +98,16 @@
 -rw-rw-r--  2.0 unx     4546 b- defN 23-Jan-21 06:41 ptrlib/pwn/fsb/fsb.py
 -rw-rw-r--  2.0 unx       23 b- defN 23-Jan-21 06:41 ptrlib/pwn/fuzz/__init__.py
 -rw-rw-r--  2.0 unx     5613 b- defN 23-Jan-21 06:41 ptrlib/pwn/fuzz/randgen.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/algorithm/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/algorithm/shortestpath/__init__.py
 -rw-rw-r--  2.0 unx     3389 b- defN 23-Jan-21 06:41 tests/algorithm/shortestpath/test_shortestpath.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/arch/__init__.py
--rw-rw-r--  2.0 unx      985 b- defN 23-May-09 08:07 tests/arch/test_simd.py
+-rw-rw-r--  2.0 unx     1252 b- defN 23-May-09 12:16 tests/arch/test_cpu.py
+-rw-rw-r--  2.0 unx      988 b- defN 23-May-09 08:25 tests/arch/test_simd.py
 -rw-rw-r--  2.0 unx     1120 b- defN 23-May-09 08:02 tests/arch/test_syscall.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/binary/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/binary/encoding/__init__.py
 -rw-rw-r--  2.0 unx      596 b- defN 23-Jan-21 06:41 tests/binary/encoding/test_byteconv.py
 -rw-rw-r--  2.0 unx     2787 b- defN 23-Jan-21 06:41 tests/binary/encoding/test_locale.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/binary/operation/__init__.py
 -rw-rw-r--  2.0 unx     1273 b- defN 23-Jan-21 06:41 tests/binary/operation/test_rotate.py
@@ -147,14 +150,14 @@
 -rw-rw-r--  2.0 unx     1613 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_5.py
 -rw-rw-r--  2.0 unx     1124 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_6.py
 -rw-rw-r--  2.0 unx     1108 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_7.py
 -rw-rw-r--  2.0 unx      574 b- defN 23-Jan-21 06:41 tests/filestruct/elf/test_elf_8.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-21 06:41 tests/pwn/__init__.py
 -rw-rw-r--  2.0 unx     1877 b- defN 23-Jan-21 06:41 tests/pwn/test_fsb.py
 -rw-rw-r--  2.0 unx     1988 b- defN 23-Jan-21 06:41 tests/pwn/test_fuzz.py
--rw-rw-r--  2.0 unx     1069 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx     3535 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       13 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13823 b- defN 23-May-09 08:16 ptrlib-2.0.6.dist-info/RECORD
-158 files, 323978 bytes uncompressed, 99825 bytes compressed:  69.2%
+-rw-rw-r--  2.0 unx     1069 b- defN 23-May-09 12:18 ptrlib-2.0.7.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx     3535 b- defN 23-May-09 12:18 ptrlib-2.0.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-09 12:18 ptrlib-2.0.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       48 b- defN 23-May-09 12:18 ptrlib-2.0.7.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       13 b- defN 23-May-09 12:18 ptrlib-2.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    14071 b- defN 23-May-09 12:18 ptrlib-2.0.7.dist-info/RECORD
+161 files, 326615 bytes uncompressed, 100858 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -72,14 +72,17 @@
 
 Filename: ptrlib/arch/intel/archname.py
 Comment: 
 
 Filename: ptrlib/arch/intel/assembler.py
 Comment: 
 
+Filename: ptrlib/arch/intel/cpu.py
+Comment: 
+
 Filename: ptrlib/arch/intel/disassembler.py
 Comment: 
 
 Filename: ptrlib/arch/intel/simd.py
 Comment: 
 
 Filename: ptrlib/arch/intel/syscall.py
@@ -96,14 +99,17 @@
 
 Filename: ptrlib/binary/__init__.py
 Comment: 
 
 Filename: ptrlib/binary/encoding/__init__.py
 Comment: 
 
+Filename: ptrlib/binary/encoding/bitconv.py
+Comment: 
+
 Filename: ptrlib/binary/encoding/byteconv.py
 Comment: 
 
 Filename: ptrlib/binary/encoding/locale.py
 Comment: 
 
 Filename: ptrlib/binary/encoding/table.py
@@ -297,14 +303,17 @@
 
 Filename: tests/algorithm/shortestpath/test_shortestpath.py
 Comment: 
 
 Filename: tests/arch/__init__.py
 Comment: 
 
+Filename: tests/arch/test_cpu.py
+Comment: 
+
 Filename: tests/arch/test_simd.py
 Comment: 
 
 Filename: tests/arch/test_syscall.py
 Comment: 
 
 Filename: tests/binary/__init__.py
@@ -450,26 +459,26 @@
 
 Filename: tests/pwn/test_fsb.py
 Comment: 
 
 Filename: tests/pwn/test_fuzz.py
 Comment: 
 
-Filename: ptrlib-2.0.6.dist-info/LICENSE.txt
+Filename: ptrlib-2.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: ptrlib-2.0.6.dist-info/METADATA
+Filename: ptrlib-2.0.7.dist-info/METADATA
 Comment: 
 
-Filename: ptrlib-2.0.6.dist-info/WHEEL
+Filename: ptrlib-2.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: ptrlib-2.0.6.dist-info/entry_points.txt
+Filename: ptrlib-2.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ptrlib-2.0.6.dist-info/top_level.txt
+Filename: ptrlib-2.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ptrlib-2.0.6.dist-info/RECORD
+Filename: ptrlib-2.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ptrlib/arch/intel/__init__.py

```diff
@@ -1,5 +1,6 @@
 from .archname import *
 from .assembler import *
+from .cpu import *
 from .disassembler import *
-from .syscall import *
 from .simd import *
+from .syscall import *
```

## ptrlib/arch/intel/simd.py

```diff
@@ -88,15 +88,15 @@
         v = xtime(xtime(s[i][1] ^ s[i][3]))
         s[i][0] ^= u
         s[i][1] ^= v
         s[i][2] ^= u
         s[i][3] ^= v
     _aes_mix_columns(s)
 
-def simd_aesenc(state, round_key):
+def intel_aesenc(state, round_key):
     """Emulate AESENC instruction
     """
     if len(state) != 16:
         raise ValueError("'state' must be 16-byte long")
     if len(round_key) != 16:
         raise ValueError("'round_key' must be 16-byte long")
 
@@ -104,15 +104,15 @@
     round_key = _aes_bytes_to_matrix(round_key)
     _aes_shift_rows(state)
     _aes_sub_bytes(state)
     _aes_mix_columns(state)
     _aes_add_round_key(state, round_key)
     return _aes_matrix_to_bytes(state)
 
-def simd_aesenc_inv(state, round_key):
+def intel_aesenc_inv(state, round_key):
     """Emulate the inverse of AESENC instruction
     """
     if len(state) != 16:
         raise ValueError("'state' must be 16-byte long")
     if len(round_key) != 16:
         raise ValueError("'round_key' must be 16-byte long")
 
@@ -120,15 +120,15 @@
     round_key = _aes_bytes_to_matrix(round_key)
     _aes_add_round_key(state, round_key)
     _aes_inv_mix_columns(state)
     _aes_inv_sub_bytes(state)
     _aes_inv_shift_rows(state)
     return _aes_matrix_to_bytes(state)
 
-def simd_aesdec(state, round_key):
+def intel_aesdec(state, round_key):
     """Emulate AESDEC instruction
     """
     if len(state) != 16:
         raise ValueError("'state' must be 16-byte long")
     if len(round_key) != 16:
         raise ValueError("'round_key' must be 16-byte long")
 
@@ -136,15 +136,15 @@
     round_key = _aes_bytes_to_matrix(round_key)
     _aes_inv_shift_rows(state)
     _aes_inv_sub_bytes(state)
     _aes_inv_mix_columns(state)
     _aes_add_round_key(state, round_key)
     return _aes_matrix_to_bytes(state)
 
-def simd_aesdec_inv(state, round_key):
+def intel_aesdec_inv(state, round_key):
     """Emulate the inverse of AESENC instruction
     """
     if len(state) != 16:
         raise ValueError("'state' must be 16-byte long")
     if len(round_key) != 16:
         raise ValueError("'round_key' must be 16-byte long")
```

## ptrlib/binary/encoding/__init__.py

```diff
@@ -1,3 +1,4 @@
+from .bitconv import *
 from .byteconv import *
 from .locale import *
 from .table import *
```

## tests/arch/test_simd.py

```diff
@@ -1,27 +1,27 @@
 import os
 import unittest
 from ptrlib.arch.intel.simd import *
 from logging import getLogger, FATAL
 
 
-class TestSyscall(unittest.TestCase):
+class TestSIMD(unittest.TestCase):
     def setUp(self):
         getLogger("ptrlib").setLevel(FATAL)
 
     def test_aes(self):
         dat = b'\x00\xff\xee\xdd\xcc\xbb\xaa\x99'\
             b'\x88\x77\x66\x55\x44\x33\x22\x11'
         key = b'\x0f\x0e\x0d\x0c\x0b\x0a\x09\x08'\
             b'\x07\x06\x05\x04\x03\x02\x01\x00'
         enc = b'\x5d\x75\x7f\x6f\xcb\xdf\xd2\x2a'\
             b'\x0c\xc9\x7b\x7f\x5f\x26\x50\x74'
         dec = b'\xe9\xbd\x56\x1c\x42\xe8\xb5\x3c'\
             b'\xf1\xc9\xdb\xf0\x67\x8d\xdf\x1a'
 
-        self.assertEqual(simd_aesenc(dat, key), enc)
-        self.assertEqual(simd_aesdec(dat, key), dec)
+        self.assertEqual(intel_aesenc(dat, key), enc)
+        self.assertEqual(intel_aesdec(dat, key), dec)
         for _ in range(10):
             dat = os.urandom(16)
             key = os.urandom(16)
-            self.assertEqual(simd_aesenc_inv(simd_aesenc(dat, key), key), dat)
-            self.assertEqual(simd_aesdec_inv(simd_aesdec(dat, key), key), dat)
+            self.assertEqual(intel_aesenc_inv(intel_aesenc(dat, key), key), dat)
+            self.assertEqual(intel_aesdec_inv(intel_aesdec(dat, key), key), dat)
```

## Comparing `ptrlib-2.0.6.dist-info/LICENSE.txt` & `ptrlib-2.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `ptrlib-2.0.6.dist-info/METADATA` & `ptrlib-2.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptrlib
-Version: 2.0.6
+Version: 2.0.7
 Summary: CTF library
 Home-page: https://github.com/ptr-yudai/ptrlib/
 Author: ptr-yudai
 Author-email: ptr.yudai+dev@gmail.com
 Keywords: pwn crypto algorithm
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.5
```

## Comparing `ptrlib-2.0.6.dist-info/RECORD` & `ptrlib-2.0.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 ptrlib/arch/arm/assembler.py,sha256=CXsOuWyLVBK3sFYX95f3UQZ7IuvLP1NR2y9mhgJu3BQ,2964
 ptrlib/arch/arm/disassembler.py,sha256=D3U8E0EhiV1SnZ5karVEeedgbf665q40yZ9iFo-wdXw,2497
 ptrlib/arch/arm/syscall.py,sha256=p8dqUdp2Yk7TnOXAzY11he-vcDhnlRKxBA0IuyXlQBU,14668
 ptrlib/arch/common/__init__.py,sha256=FFz48QFj-90sKaJSYAcnk2IaM5aY7LQmMsK5IgrKryc,75
 ptrlib/arch/common/assembler.py,sha256=IINg5eHILqYd_frtFzTecdoD2qKNTdMy21ym14Zuruw,3383
 ptrlib/arch/common/disassembler.py,sha256=PwhIw2yTuZ06rDbFwHs-M0tokzqocn5Tan7wAo7dGXM,1860
 ptrlib/arch/common/ospath.py,sha256=Um5rSp8IhNH78ZYUnj3b0DXdSxU-vJbfuC_XjLKva78,181
-ptrlib/arch/intel/__init__.py,sha256=nDKSz9M52xIiwBcEqmnV2s64mPAyg17NLwsX96pCPbo,120
+ptrlib/arch/intel/__init__.py,sha256=XSP8yO8gZhcfEd3ygcZKlcKsGe2Rq9KlvP1JzyMDAUs,139
 ptrlib/arch/intel/archname.py,sha256=eAIB2r7eHKow4U5oZtnY6CPsGdN78S5f1UGeJFE2XZs,853
 ptrlib/arch/intel/assembler.py,sha256=n4ri2jH22LJMPHf4LMCeKZC-b3gL_nN3jovTyEsYH-Q,2107
+ptrlib/arch/intel/cpu.py,sha256=EgBIQKp7uztH75A_luU7Oi5l_LVFu0AErXqoMP0fRXo,868
 ptrlib/arch/intel/disassembler.py,sha256=bGR24AGqu7Xh5CCHy2Quw0AqEQZLgO6yd79WKWPFovE,2072
-ptrlib/arch/intel/simd.py,sha256=tgpqur-sY1hQEV1wqTUdZ78TU57W5pTI0sFTMx0l514,7138
+ptrlib/arch/intel/simd.py,sha256=0Oc5ht36hF032WK_hA1j9Cz0k-j8rcnr7QLeELbBQCg,7142
 ptrlib/arch/intel/syscall.py,sha256=kgAoR1WAhqsfeJ4BGchrCqZb_nrsnnJ_g3u5loehatY,14542
 ptrlib/arch/linux/__init__.py,sha256=MxDaHplYTwY16ma16lsigtP2a433xLPZe5QdmSdTZMo,45
 ptrlib/arch/linux/ospath.py,sha256=MekrAU-UCw7HDEmMAe4rTPGI-H6nbQTgmXFUIxMuGIw,465
 ptrlib/arch/linux/syscall.py,sha256=g-_eE5xc98rRL1NluKgI00sDUTBdQ2Qb7_dukkONL3M,723
 ptrlib/binary/__init__.py,sha256=Yq7lZzjQbkGObgBhkc4EyxUQNqoSzq8Upy8aAzcqMmY,98
-ptrlib/binary/encoding/__init__.py,sha256=-6TbyfyvxhCcEtvC1C8jJ5guR7xobwUQ3bh3m-duUSM,67
+ptrlib/binary/encoding/__init__.py,sha256=fQgp0SEFRN-2KBUKUH5AxqsXV3hgxYcT1o7eqT548Rc,90
+ptrlib/binary/encoding/bitconv.py,sha256=Y9p95RbBi4lDqnbeuC0N0MeTkSuVowjtX95-Dnqu2OU,220
 ptrlib/binary/encoding/byteconv.py,sha256=-kkf6GF4dXm7P3VC3iXXahT0e05xNDOW7wVT1KAXRKQ,524
 ptrlib/binary/encoding/locale.py,sha256=JZALRWQWLDHYkPuYAf8llAGAFmhgR1mDGcCTfz9-Ebc,1552
 ptrlib/binary/encoding/table.py,sha256=0G3-e_GQnHIilV5N9QbyCOelVxnwfE5uVvVXr5h3gMc,520
 ptrlib/binary/operation/__init__.py,sha256=A7OOwayygfMwVev-HJoazt4ryq15xqSXjni1RK5Q7cM,41
 ptrlib/binary/operation/rotate.py,sha256=1K4Z1rtoaqJ-Q7uJkp5LzAoqFbg07IzgKDrN5Rx1XEI,1374
 ptrlib/binary/operation/xor.py,sha256=wa99k4etfCzZHIjkaf5vdLiPxFPEQuIvAkL6GdO_51o,1048
 ptrlib/binary/packing/__init__.py,sha256=2wYJJGaQ_9vEMvdGeSvex4dRsxVziEuwl416yh8w2-o,84
@@ -95,15 +97,16 @@
 ptrlib/pwn/fsb/fsb.py,sha256=OsMPeHXD20NV820D3oMJSNIRIZJmUMuaNTwpqLTfOPA,4546
 ptrlib/pwn/fuzz/__init__.py,sha256=RjOf2xiJg09IktbnSn5CNylxhetu7eoMg8QpUfMFpd4,23
 ptrlib/pwn/fuzz/randgen.py,sha256=v1-SwGR3NfrKAOzXrEzlXmTzVwlfuD08Erpkm9hTXJE,5613
 tests/algorithm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/algorithm/shortestpath/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/algorithm/shortestpath/test_shortestpath.py,sha256=uYKYhsE3K_1FYzuRdhmFFKJulV5qPmIDWN9qVX3fHAk,3389
 tests/arch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/arch/test_simd.py,sha256=k43CxIQVCVu6wc_5mHdmWC7vuQCyOyqxxS-sG_8kG98,985
+tests/arch/test_cpu.py,sha256=VnZ03jKE64Oi2X-0asnfR9uCrt4UtCxUe-W9yvzWN6Y,1252
+tests/arch/test_simd.py,sha256=kEWsAkxsY6R3Nq_9lDM_clsgucsC8aabw3IcQ5V4POM,988
 tests/arch/test_syscall.py,sha256=9D-rplpqv80u80zjDRseufnvjP2vyRDerggoOe1NpmM,1120
 tests/binary/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/binary/encoding/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/binary/encoding/test_byteconv.py,sha256=7EeO-3l1mMGr2lpE2y6VHoFFo49peQT-xRX6R138uTY,596
 tests/binary/encoding/test_locale.py,sha256=ipVE8agDaOABSUBdXhGIRDrKg2SOmVEF8ntaDHYFy84,2787
 tests/binary/operation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/binary/operation/test_rotate.py,sha256=ppoWXsBskZsvmNtT7MlLU65roOq9NKhvzfHAUApD7yU,1273
@@ -146,13 +149,13 @@
 tests/filestruct/elf/test_elf_5.py,sha256=LEi8_R6uog7U3LLkrYAdfrdJH3JJXH8Olv77xPFBIgQ,1613
 tests/filestruct/elf/test_elf_6.py,sha256=XJ7pRu9whJq4wdgfk8ere4q4QbcgONtV-e2ZBo4S544,1124
 tests/filestruct/elf/test_elf_7.py,sha256=uwkPsovbAdZFUJNWZ5XySf0kYtaaPJNs1YDzjYce0-Q,1108
 tests/filestruct/elf/test_elf_8.py,sha256=C1Gnylu5lOqPFo8NfJBo5YyUULe026uKL-hvwWprON0,574
 tests/pwn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/pwn/test_fsb.py,sha256=VC_0csTXIS1_PIGUBJmy2uN7hllr4kXJ0mibNYN5d_A,1877
 tests/pwn/test_fuzz.py,sha256=ARnTx48YnuV-awKeFhjsPAyCYJDn9M80q4DyVj5pvOA,1988
-ptrlib-2.0.6.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-ptrlib-2.0.6.dist-info/METADATA,sha256=yZyByzBSHbQaAitPzHjyrtf-xEY-B0Yv7UpV7cC2sL4,3535
-ptrlib-2.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ptrlib-2.0.6.dist-info/entry_points.txt,sha256=xJ7v7w7uhxUeAzagSodmQhexYh_8GjCTPDCKMFse9T0,48
-ptrlib-2.0.6.dist-info/top_level.txt,sha256=A_zqZPqp9QidhyWj2_hpnC7wz0tTQ2nbR8D6vOnhzYk,13
-ptrlib-2.0.6.dist-info/RECORD,,
+ptrlib-2.0.7.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+ptrlib-2.0.7.dist-info/METADATA,sha256=z0uTxn_iHK9g8BKHqMc3N2beiu0mcgDvaM_JGb6cLb0,3535
+ptrlib-2.0.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ptrlib-2.0.7.dist-info/entry_points.txt,sha256=xJ7v7w7uhxUeAzagSodmQhexYh_8GjCTPDCKMFse9T0,48
+ptrlib-2.0.7.dist-info/top_level.txt,sha256=A_zqZPqp9QidhyWj2_hpnC7wz0tTQ2nbR8D6vOnhzYk,13
+ptrlib-2.0.7.dist-info/RECORD,,
```

