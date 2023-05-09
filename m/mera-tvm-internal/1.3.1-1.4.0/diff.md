# Comparing `tmp/mera_tvm_internal-1.3.1-cp38-cp38-manylinux_2_27_x86_64.whl.zip` & `tmp/mera_tvm_internal-1.4.0-cp38-cp38-manylinux_2_27_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 288257 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx    23544 b- defN 23-Feb-22 08:59 meratvm_internal/__init__.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    59656 b- defN 23-Feb-22 08:59 meratvm_internal/_cpp_lib_load.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    23416 b- defN 23-Feb-22 08:59 meratvm_internal/_version.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   143056 b- defN 23-Feb-22 08:59 meratvm_internal/multi_networks.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx   424360 b- defN 23-Feb-22 08:59 meratvm_internal/patterns.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    67688 b- defN 23-Feb-22 08:59 meratvm_internal/query_arch.cpython-38-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      181 b- defN 23-Feb-22 08:59 mera_tvm_internal-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 23-Feb-22 08:59 mera_tvm_internal-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Feb-22 08:59 mera_tvm_internal-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1037 b- defN 23-Feb-22 08:59 mera_tvm_internal-1.3.1.dist-info/RECORD
-10 files, 743067 bytes uncompressed, 286441 bytes compressed:  61.5%
+Zip file size: 370619 bytes, number of entries: 11
+-rwxr-xr-x  2.0 unx    23544 b- defN 23-May-09 08:05 meratvm_internal/__init__.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    59656 b- defN 23-May-09 08:05 meratvm_internal/_cpp_lib_load.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    23416 b- defN 23-May-09 08:05 meratvm_internal/_version.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   143056 b- defN 23-May-09 08:05 meratvm_internal/multi_networks.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   424360 b- defN 23-May-09 08:05 meratvm_internal/patterns.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   212200 b- defN 23-May-09 08:06 meratvm_internal/patterns_mera_blocks.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    67688 b- defN 23-May-09 08:06 meratvm_internal/query_arch.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      181 b- defN 23-May-09 08:06 mera_tvm_internal-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-May-09 08:06 mera_tvm_internal-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-09 08:06 mera_tvm_internal-1.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1164 b- defN 23-May-09 08:06 mera_tvm_internal-1.4.0.dist-info/RECORD
+11 files, 955394 bytes uncompressed, 368591 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -9,23 +9,26 @@
 
 Filename: meratvm_internal/multi_networks.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
 Filename: meratvm_internal/patterns.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
+Filename: meratvm_internal/patterns_mera_blocks.cpython-38-x86_64-linux-gnu.so
+Comment: 
+
 Filename: meratvm_internal/query_arch.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: mera_tvm_internal-1.3.1.dist-info/METADATA
+Filename: mera_tvm_internal-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: mera_tvm_internal-1.3.1.dist-info/WHEEL
+Filename: mera_tvm_internal-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: mera_tvm_internal-1.3.1.dist-info/top_level.txt
+Filename: mera_tvm_internal-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mera_tvm_internal-1.3.1.dist-info/RECORD
+Filename: mera_tvm_internal-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## meratvm_internal/_cpp_lib_load.cpython-38-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0215c2bc4f78c338a001db9a86f719f9ad40cc81
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: cc476d1499a6587497ddb7a20ebb10eecd184568
```

### strings --all --bytes=8 {}

```diff
@@ -128,15 +128,15 @@
 __file__
 __package__
 __path__
 submodule_search_locations
 cannot import name %S
 name '%U' is not defined
 %s (%s:%d)
-_cython_0_29_32
+_cython_0_29_34
 builtins
 cython_runtime
 __builtins__
 cython_function_or_method
 __reduce__
 __module__
 func_doc
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -7,15 +7,15 @@
   0x0000b040 655f5f00 70617265 6e74005f 5f706174 e__.parent.__pat
   0x0000b050 685f5f00 7375626d 6f64756c 655f7365 h__.submodule_se
   0x0000b060 61726368 5f6c6f63 6174696f 6e730063 arch_locations.c
   0x0000b070 616e6e6f 7420696d 706f7274 206e616d annot import nam
   0x0000b080 65202553 006e616d 65202725 55272069 e %S.name '%U' i
   0x0000b090 73206e6f 74206465 66696e65 64002573 s not defined.%s
   0x0000b0a0 20282573 3a256429 0025642e 2564005f  (%s:%d).%d.%d._
-  0x0000b0b0 63797468 6f6e5f30 5f32395f 33320062 cython_0_29_32.b
+  0x0000b0b0 63797468 6f6e5f30 5f32395f 33340062 cython_0_29_34.b
   0x0000b0c0 75696c74 696e7300 63797468 6f6e5f72 uiltins.cython_r
   0x0000b0d0 756e7469 6d65005f 5f627569 6c74696e untime.__builtin
   0x0000b0e0 735f5f00 63797468 6f6e5f66 756e6374 s__.cython_funct
   0x0000b0f0 696f6e5f 6f725f6d 6574686f 64005f5f ion_or_method.__
   0x0000b100 72656475 63655f5f 005f5f6d 6f64756c reduce__.__modul
   0x0000b110 655f5f00 66756e63 5f646f63 005f5f64 e__.func_doc.__d
   0x0000b120 6f635f5f 0066756e 635f6e61 6d65005f oc__.func_name._
```

## meratvm_internal/_version.cpython-38-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 7f3f05384fe14c2f5aa2c1ecb336426d756471b8
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a9bdb2832ba01efc1d57183da8a376abc7476c99
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -32,12 +32,12 @@
   0x000041d0 6174766d 5f696e74 65726e61 6c2e5f76 atvm_internal._v
   0x000041e0 65727369 6f6e0062 75696c74 696e7300 ersion.builtins.
   0x000041f0 63797468 6f6e5f72 756e7469 6d65005f cython_runtime._
   0x00004200 5f627569 6c74696e 735f5f00 25732028 _builtins__.%s (
   0x00004210 25733a25 64290000 00000000 00000000 %s:%d)..........
   0x00004220 636c696e 655f696e 5f747261 63656261 cline_in_traceba
   0x00004230 636b0000 00000000 5f5f7665 7273696f ck......__versio
-  0x00004240 6e5f5f00 312e332e 31000000 00000000 n__.1.3.1.......
+  0x00004240 6e5f5f00 312e342e 30000000 00000000 n__.1.4.0.......
   0x00004250 5f5f7465 73745f5f 00000000 00000000 __test__........
   0x00004260 5f5f6e61 6d655f5f 00000000 00000000 __name__........
   0x00004270 5f5f6d61 696e5f5f 00                __main__.
```

## meratvm_internal/multi_networks.cpython-38-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 52ce7ecc6fe59aa8d26c1c52623eda8b8dd1f76a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 7dbd6f806d3cb12cf25341252c22009d90a085aa
```

### strings --all --bytes=8 {}

```diff
@@ -170,15 +170,15 @@
 cannot import name %S
 name '%U' is not defined
 %s (%s:%d)
 __init__
 _var_is_input
 _func_has_attr
 _is_mera_quantized
-_cython_0_29_32
+_cython_0_29_34
 builtins
 cython_runtime
 __builtins__
 transform_function
 _update_params
 visit_var
 at least
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -11,15 +11,15 @@
   0x0001d080 65202553 006e616d 65202725 55272069 e %S.name '%U' i
   0x0001d090 73206e6f 74206465 66696e65 64002573 s not defined.%s
   0x0001d0a0 20282573 3a256429 00657861 63746c79  (%s:%d).exactly
   0x0001d0b0 005f5f69 6e69745f 5f005f76 61725f69 .__init__._var_i
   0x0001d0c0 735f696e 70757400 5f66756e 635f6861 s_input._func_ha
   0x0001d0d0 735f6174 7472005f 69735f6d 6572615f s_attr._is_mera_
   0x0001d0e0 7175616e 74697a65 64002564 2e256400 quantized.%d.%d.
-  0x0001d0f0 5f637974 686f6e5f 305f3239 5f333200 _cython_0_29_32.
+  0x0001d0f0 5f637974 686f6e5f 305f3239 5f333400 _cython_0_29_34.
   0x0001d100 6275696c 74696e73 00637974 686f6e5f builtins.cython_
   0x0001d110 72756e74 696d6500 5f5f6275 696c7469 runtime.__builti
   0x0001d120 6e735f5f 00747261 6e73666f 726d5f66 ns__.transform_f
   0x0001d130 756e6374 696f6e00 5f757064 6174655f unction._update_
   0x0001d140 70617261 6d730076 69736974 5f766172 params.visit_var
   0x0001d150 006f626a 00617420 6c656173 74006174 .obj.at least.at
   0x0001d160 206d6f73 74006675 73655f6d 756c7469  most.fuse_multi
```

## meratvm_internal/patterns.cpython-38-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 89ebf516c3d3248d28f49ee91e5ff7beb760062a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 782b0ac3131f75488f61df060d6efda1bf694dcf
```

### strings --all --bytes=8 {}

```diff
@@ -263,15 +263,15 @@
 __package__
 __path__
 submodule_search_locations
 cannot import name %S
 name '%U' is not defined
 %s (%s:%d)
 meratvm_internal.patterns
-_cython_0_29_32
+_cython_0_29_34
 builtins
 cython_runtime
 __builtins__
 at least
 make_qnn_mul_pattern
 make_qnn_add_pattern
 tuple_multi_input_pattern
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -10,15 +10,15 @@
   0x0005d070 616e6e6f 7420696d 706f7274 206e616d annot import nam
   0x0005d080 65202553 006e616d 65202725 55272069 e %S.name '%U' i
   0x0005d090 73206e6f 74206465 66696e65 64002573 s not defined.%s
   0x0005d0a0 20282573 3a256429 00657861 63746c79  (%s:%d).exactly
   0x0005d0b0 006c616d 62646131 0025642e 2564006d .lambda1.%d.%d.m
   0x0005d0c0 65726174 766d5f69 6e746572 6e616c2e eratvm_internal.
   0x0005d0d0 70617474 65726e73 005f6379 74686f6e patterns._cython
-  0x0005d0e0 5f305f32 395f3332 00627569 6c74696e _0_29_32.builtin
+  0x0005d0e0 5f305f32 395f3334 00627569 6c74696e _0_29_34.builtin
   0x0005d0f0 73006379 74686f6e 5f72756e 74696d65 s.cython_runtime
   0x0005d100 005f5f62 75696c74 696e735f 5f006174 .__builtins__.at
   0x0005d110 206c6561 73740061 74206d6f 7374006d  least.at most.m
   0x0005d120 616b655f 716e6e5f 6d756c5f 70617474 ake_qnn_mul_patt
   0x0005d130 65726e00 6d616b65 5f716e6e 5f616464 ern.make_qnn_add
   0x0005d140 5f706174 7465726e 00747570 6c655f6d _pattern.tuple_m
   0x0005d150 756c7469 5f696e70 75745f70 61747465 ulti_input_patte
```

## meratvm_internal/query_arch.cpython-38-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 95e7005f3d7b5a7f7aacc158e10694f8fb2a36c4
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ca7178d42238b7f00e2f4faf665d706dfda13412
```

### strings --all --bytes=8 {}

```diff
@@ -128,15 +128,15 @@
 __file__
 __package__
 __path__
 submodule_search_locations
 name '%U' is not defined
 %s (%s:%d)
 meratvm_internal.query_arch
-_cython_0_29_32
+_cython_0_29_34
 builtins
 cython_runtime
 __builtins__
 cannot import name %S
 arch_val
 operator_id
 _arch_supports_operator
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -8,15 +8,15 @@
   0x0000d050 685f5f00 7375626d 6f64756c 655f7365 h__.submodule_se
   0x0000d060 61726368 5f6c6f63 6174696f 6e73006e arch_locations.n
   0x0000d070 616d6520 27255527 20697320 6e6f7420 ame '%U' is not 
   0x0000d080 64656669 6e656400 25732028 25733a25 defined.%s (%s:%
   0x0000d090 64290025 642e2564 006d6572 6174766d d).%d.%d.meratvm
   0x0000d0a0 5f696e74 65726e61 6c2e7175 6572795f _internal.query_
   0x0000d0b0 61726368 005f6379 74686f6e 5f305f32 arch._cython_0_2
-  0x0000d0c0 395f3332 00627569 6c74696e 73006379 9_32.builtins.cy
+  0x0000d0c0 395f3334 00627569 6c74696e 73006379 9_34.builtins.cy
   0x0000d0d0 74686f6e 5f72756e 74696d65 005f5f62 thon_runtime.__b
   0x0000d0e0 75696c74 696e735f 5f006361 6e6e6f74 uiltins__.cannot
   0x0000d0f0 20696d70 6f727420 6e616d65 20255300  import name %S.
   0x0000d100 65786163 746c7900 61726368 5f76616c exactly.arch_val
   0x0000d110 006f7065 7261746f 725f6964 005f6172 .operator_id._ar
   0x0000d120 63685f73 7570706f 7274735f 6f706572 ch_supports_oper
   0x0000d130 61746f72 00706172 616d5f6e 616d6500 ator.param_name.
```

## Comparing `mera_tvm_internal-1.3.1.dist-info/RECORD` & `mera_tvm_internal-1.4.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 meratvm_internal/__init__.cpython-38-x86_64-linux-gnu.so,sha256=V7QF0Eo-edq_Ki6jetYQAU3D6oLdcTgyvuZmlcax1DM,23544
-meratvm_internal/_cpp_lib_load.cpython-38-x86_64-linux-gnu.so,sha256=wO_N3xmpLbnrq60BpUQOVUE-A7vVV4SXwTvUt5Ss-R8,59656
-meratvm_internal/_version.cpython-38-x86_64-linux-gnu.so,sha256=ud6cJt-yHdGewpO5PohMwlSl0tT6t_iIeMAHvgcRUBM,23416
-meratvm_internal/multi_networks.cpython-38-x86_64-linux-gnu.so,sha256=-y2rZaa0W8JEmGAJGHABIt3SaWvx34dilmNprb6905A,143056
-meratvm_internal/patterns.cpython-38-x86_64-linux-gnu.so,sha256=I4u6Rt4WWNb1pxSmtCmQ29LN0gZX1WR7HZ7EeHQB4Cg,424360
-meratvm_internal/query_arch.cpython-38-x86_64-linux-gnu.so,sha256=W5UkXEuqgOkGp5KMAs_qc33ESiuT9g655lq8xTckye4,67688
-mera_tvm_internal-1.3.1.dist-info/METADATA,sha256=zD3ucohjy0x1iAQi_8sK-Tl4gmzIzvcusA97SI7mpPE,181
-mera_tvm_internal-1.3.1.dist-info/WHEEL,sha256=dmF1FikMDTF1FaZ4r0VXJMTFfO94TPfcDS3SzW-yeAk,112
-mera_tvm_internal-1.3.1.dist-info/top_level.txt,sha256=JrkwbbHZpDLqdXgiuMWSh3sDRjmxbWTDm_MqMEgpjUk,17
-mera_tvm_internal-1.3.1.dist-info/RECORD,,
+meratvm_internal/_cpp_lib_load.cpython-38-x86_64-linux-gnu.so,sha256=zhUk7bybR3duxZXKsSPmRnv50pzcWojj8pd4uZakMKg,59656
+meratvm_internal/_version.cpython-38-x86_64-linux-gnu.so,sha256=7G-ZL8PA20Afhq7qRyCHoqYkHCGMS23mh4Npm2icOdw,23416
+meratvm_internal/multi_networks.cpython-38-x86_64-linux-gnu.so,sha256=SFS1bMs6HcpDZNey24S-2GL8tteNAlyr5WUozIEBAiQ,143056
+meratvm_internal/patterns.cpython-38-x86_64-linux-gnu.so,sha256=Zk8U7S_suPIzgOOnKScnDqcE5TxyuE4wkmg1JfKE2f0,424360
+meratvm_internal/patterns_mera_blocks.cpython-38-x86_64-linux-gnu.so,sha256=UO-Z0NjEqYry06cwh0Jl7AvRU_GQEOEql995q4XG2WU,212200
+meratvm_internal/query_arch.cpython-38-x86_64-linux-gnu.so,sha256=P2q6dx2dXPXGM0SxrU8VP1ZyQuikvNywersP5kLagGA,67688
+mera_tvm_internal-1.4.0.dist-info/METADATA,sha256=eXU1ShfRuNP1SQIcGakTHXxJVmGETmw9qgKMo_JMMvo,181
+mera_tvm_internal-1.4.0.dist-info/WHEEL,sha256=dmF1FikMDTF1FaZ4r0VXJMTFfO94TPfcDS3SzW-yeAk,112
+mera_tvm_internal-1.4.0.dist-info/top_level.txt,sha256=JrkwbbHZpDLqdXgiuMWSh3sDRjmxbWTDm_MqMEgpjUk,17
+mera_tvm_internal-1.4.0.dist-info/RECORD,,
```

