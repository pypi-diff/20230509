# Comparing `tmp/arithmetica-py-1.0.186.tar.gz` & `tmp/arithmetica-py-1.0.189.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.186.tar", last modified: Mon May  8 21:56:02 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.189.tar", last modified: Tue May  9 08:09:01 2023, max compression
```

## Comparing `arithmetica-py-1.0.186.tar` & `arithmetica-py-1.0.189.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.331936 arithmetica-py-1.0.186/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.331936 arithmetica-py-1.0.186/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:56:02.335936 arithmetica-py-1.0.186/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   166980 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    66430 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-08 21:55:40.000000 arithmetica-py-1.0.186/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 21:56:02.000000 arithmetica-py-1.0.186/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:09:01.525327 arithmetica-py-1.0.189/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-09 08:08:46.000000 arithmetica-py-1.0.189/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 08:09:01.525327 arithmetica-py-1.0.189/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-05-09 08:08:46.000000 arithmetica-py-1.0.189/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:09:01.525327 arithmetica-py-1.0.189/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 08:09:01.525327 arithmetica-py-1.0.189/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-09 08:08:46.000000 arithmetica-py-1.0.189/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:09:01.525327 arithmetica-py-1.0.189/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 08:09:01.525327 arithmetica-py-1.0.189/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   182664 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75112 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-05-09 08:08:46.000000 arithmetica-py-1.0.189/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 08:09:01.000000 arithmetica-py-1.0.189/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.186/LICENSE` & `arithmetica-py-1.0.189/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.186/README.md` & `arithmetica-py-1.0.189/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.186/setup.py` & `arithmetica-py-1.0.189/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.186/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.189/src/python-module/libarithmetica.a`

 * *Files 4% similar despite different names*

#### nm -s {}

```diff
@@ -20,17 +20,22 @@
 _ZN11arithmetica9to_stringB5cxx11ERKNS_8FractionE in arithmetica.cpp.o
 _ZNSt6vectorINSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEESaIS5_EE17_M_realloc_insertIJS5_EEEvN9__gnu_cxx17__normal_iteratorIPS5_S7_EEDpOT_ in arithmetica.cpp.o
 _ZN11arithmetica30fraction_to_continued_fractionENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ in arithmetica.cpp.o
 arccos in arccos.c.o
 arcsin in arcsin.c.o
 arctan in arctan.c.o
 check_accuracy in check_accuracy.c.o
+continued_fraction_to_fraction in continued_fraction_to_fraction.c.o
 cosine in cosine.c.o
 exponential in exponential.c.o
 factorial in factorial.c.o
+find_roots_of_polynomial_substitute in find_roots_of_polynomial.c.o
+find_roots_of_polynomial_substitute_fraction in find_roots_of_polynomial.c.o
+find_roots_of_polynomial_divide_polynomial in find_roots_of_polynomial.c.o
+find_roots_of_polynomial in find_roots_of_polynomial.c.o
 fraction_to_continued_fraction in fraction_to_continued_fraction.c.o
 igcd in igcd.c.o
 ilcm in ilcm.c.o
 natural_logarithm in natural_logarithm.c.o
 power in power.c.o
 power_integer in power_integer.c.o
 repeating_decimal_to_fraction in repeating_decimal_to_fraction.c.o
@@ -63,14 +68,15 @@
 delete_fraction in fraction.c.o
 add_fraction in add_fraction.c.o
 multiply_fraction in multiply_fraction.c.o
 parse_fraction in parse_fraction.c.o
 power_fraction in power_fraction.c.o
 simplify_parsed_fraction in simplify_parsed_fraction.c.o
 subtract_fraction in subtract_fraction.c.o
+equal_fraction in equal_fraction.c.o
 create_complex_number in complex_arithmetica.c.o
 delete_complex_number in complex_arithmetica.c.o
 add_complex in add_complex.c.o
 divide_complex in divide_complex.c.o
 exponential_complex in exponential_complex.c.o
 multiply_complex in multiply_complex.c.o
 square_root_complex in square_root_complex.c.o
@@ -204,14 +210,25 @@
 
 check_accuracy.c.o:
 0000000000000000 T check_accuracy
                  U strchr
                  U strcmp
                  U strlen
 
+continued_fraction_to_fraction.c.o:
+                 U add
+                 U calloc
+0000000000000000 T continued_fraction_to_fraction
+                 U free
+                 U malloc
+                 U memcpy
+                 U multiply
+                 U strcpy
+                 U strlen
+
 cosine.c.o:
                  U __stack_chk_fail
                  U add
                  U calloc
                  U check_accuracy
 0000000000000000 T cosine
                  U divide
@@ -255,14 +272,49 @@
                  U free
                  U log10
                  U memset
                  U multiply
                  U strcpy
                  U strlen
 
+find_roots_of_polynomial.c.o:
+0000000000000000 r .LC0
+0000000000000004 r .LC1
+0000000000000000 r .LC2
+                 U __stack_chk_fail
+                 U abs_mod
+                 U add
+                 U add_fraction
+                 U calloc
+                 U continued_fraction_to_fraction
+                 U delete_fraction
+                 U divide
+                 U equal_fraction
+00000000000003f0 T find_roots_of_polynomial
+00000000000002b0 T find_roots_of_polynomial_divide_polynomial
+0000000000000000 T find_roots_of_polynomial_substitute
+0000000000000180 T find_roots_of_polynomial_substitute_fraction
+                 U fraction_to_continued_fraction
+                 U free
+                 U increment_whole
+                 U log2
+                 U malloc
+                 U memcpy
+                 U memmove
+                 U memset
+                 U multiply
+                 U multiply_fraction
+                 U parse_fraction
+                 U realloc
+                 U stpcpy
+                 U strcpy
+                 U strlen
+                 U subtract
+                 U terminating_decimal_to_fraction
+
 fraction_to_continued_fraction.c.o:
                  U calloc
                  U divide_whole_with_remainder
 0000000000000000 T fraction_to_continued_fraction
                  U free
                  U malloc
                  U memcpy
@@ -457,15 +509,14 @@
                  U calloc
                  U divide
                  U free
                  U igcd
                  U malloc
                  U memcpy
                  U memmove
-                 U realloc
                  U strlen
 0000000000000000 T terminating_decimal_to_fraction
 
 Fraction.cpp.o:
 0000000000000003 r .LC10
 0000000000000000 r .LC4
 0000000000000000 r .LC9
@@ -596,14 +647,18 @@
                  U free
                  U multiply
                  U simplify_parsed_fraction
                  U strlen
                  U subtract
 0000000000000000 T subtract_fraction
 
+equal_fraction.c.o:
+0000000000000000 T equal_fraction
+                 U strcmp
+
 complex_arithmetica.c.o:
                  U calloc
 0000000000000000 T create_complex_number
 0000000000000080 T delete_complex_number
                  U free
                  U memcpy
                  U strlen
```

#### file list

```diff
@@ -1,37 +1,40 @@
-----------   0        0        0     3432 1970-01-01 00:00:00.000000 /
+----------   0        0        0     3650 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0    22216 1970-01-01 00:00:00.000000 arithmetica.cpp.o
 ?rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 arccos.c.o
 ?rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 arcsin.c.o
 ?rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 arctan.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 check_accuracy.c.o
+?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 continued_fraction_to_fraction.c.o
 ?rw-r--r--   0        0        0     3968 1970-01-01 00:00:00.000000 cosine.c.o
 ?rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 exponential.c.o
 ?rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 factorial.c.o
+?rw-r--r--   0        0        0    11200 1970-01-01 00:00:00.000000 find_roots_of_polynomial.c.o
 ?rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 fraction_to_continued_fraction.c.o
 ?rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 igcd.c.o
 ?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 ilcm.c.o
 ?rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 natural_logarithm.c.o
 ?rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 power.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18192 1970-01-01 00:00:00.000000 simplify_arithmetic_expression.c.o
 ?rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 sine.c.o
 ?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 square_root.c.o
 ?rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 tangent.c.o
-?rw-r--r--   0        0        0     2952 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
+?rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18288 1970-01-01 00:00:00.000000 Fraction.cpp.o
 ?rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 fraction.c.o
 ?rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 add_fraction.c.o
 ?rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 multiply_fraction.c.o
 ?rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 parse_fraction.c.o
 ?rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 power_fraction.c.o
 ?rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 simplify_parsed_fraction.c.o
 ?rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 subtract_fraction.c.o
+?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 equal_fraction.c.o
 ?rw-r--r--   0        0        0     1920 1970-01-01 00:00:00.000000 complex_arithmetica.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 add_complex.c.o
 ?rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 divide_complex.c.o
 ?rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 exponential_complex.c.o
 ?rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 multiply_complex.c.o
 ?rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 square_root_complex.c.o
 ?rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 subtract_complex.c.o
```

#### terminating_decimal_to_fraction.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          2056 (bytes into file)
+  Start of section headers:          1960 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         14
   Section header string table index: 13
```

##### readelf --wide --sections {}

```diff
@@ -1,23 +1,23 @@
-There are 14 section headers, starting at offset 0x808:
+There are 14 section headers, starting at offset 0x7a8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 0002b5 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 0005c0 0001b0 18   I 11   1  8
-  [ 3] .data             PROGBITS        0000000000000000 0002f5 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 0002f5 000000 00  WA  0   0  1
-  [ 5] .rodata.cst16     PROGBITS        0000000000000000 000300 000010 10  AM  0   0 16
-  [ 6] .comment          PROGBITS        0000000000000000 000310 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00033c 000000 00      0   0  1
-  [ 8] .note.gnu.property NOTE            0000000000000000 000340 000020 00   A  0   0  8
-  [ 9] .eh_frame         PROGBITS        0000000000000000 000360 000068 00   A  0   0  8
-  [10] .rela.eh_frame    RELA            0000000000000000 000770 000018 18   I 11   9  8
-  [11] .symtab           SYMTAB          0000000000000000 0003c8 000168 18     12   5  8
-  [12] .strtab           STRTAB          0000000000000000 000530 00008a 00      0   0  1
-  [13] .shstrtab         STRTAB          0000000000000000 000788 00007a 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 0002a5 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000590 000180 18   I 11   1  8
+  [ 3] .data             PROGBITS        0000000000000000 0002e5 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 0002e5 000000 00  WA  0   0  1
+  [ 5] .rodata.cst16     PROGBITS        0000000000000000 0002f0 000010 10  AM  0   0 16
+  [ 6] .comment          PROGBITS        0000000000000000 000300 00002c 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00032c 000000 00      0   0  1
+  [ 8] .note.gnu.property NOTE            0000000000000000 000330 000020 00   A  0   0  8
+  [ 9] .eh_frame         PROGBITS        0000000000000000 000350 000068 00   A  0   0  8
+  [10] .rela.eh_frame    RELA            0000000000000000 000710 000018 18   I 11   9  8
+  [11] .symtab           SYMTAB          0000000000000000 0003b8 000150 18     12   5  8
+  [12] .strtab           STRTAB          0000000000000000 000508 000082 00      0   0  1
+  [13] .shstrtab         STRTAB          0000000000000000 000728 00007a 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,18 +1,17 @@
 
-Symbol table '.symtab' contains 15 entries:
+Symbol table '.symtab' contains 14 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS terminating_decimal_to_fraction.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
      3: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    5 .LC1
      4: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    5 .LC0
-     5: 0000000000000000   693 FUNC    GLOBAL DEFAULT    1 terminating_decimal_to_fraction
+     5: 0000000000000000   677 FUNC    GLOBAL DEFAULT    1 terminating_decimal_to_fraction
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND malloc
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
      9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
     10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND igcd
     11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
     12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
-    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND realloc
-    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
+    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x5c0 contains 18 entries:
+Relocation section '.rela.text' at offset 0x590 contains 16 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000000003c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000004d  0000000700000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 000000000000005d  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 000000000000006e  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
 00000000000000c9  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 0000000000000109  0000000400000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
@@ -11,15 +11,13 @@
 00000000000001ce  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000001df  0000000a00000004 R_X86_64_PLT32         0000000000000000 igcd - 4
 00000000000001ef  0000000b00000004 R_X86_64_PLT32         0000000000000000 divide - 4
 0000000000000201  0000000b00000004 R_X86_64_PLT32         0000000000000000 divide - 4
 0000000000000211  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
 0000000000000219  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
 000000000000024c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000258  0000000d00000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-0000000000000263  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000274  0000000e00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+000000000000025d  0000000d00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 000000000000022f  0000000c00000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x770 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x710 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,15 +9,15 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..00000000000002b5
+00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..00000000000002a5
   DW_CFA_advance_loc: 6 to 0000000000000006
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 2 to 0000000000000008
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 2 to 000000000000000a
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -41,15 +41,15 @@
 	mov    %rax,%rbp
 	call   72 <terminating_decimal_to_fraction+0x72>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x18(%rsp),%r9
 	xor    %eax,%eax
 	xor    %edx,%edx
 	test   %r9,%r9
-	je     2a0 <terminating_decimal_to_fraction+0x2a0>
+	je     290 <terminating_decimal_to_fraction+0x290>
 	nopl   0x0(%rax)
 	cmpb   $0x2e,0x0(%r13,%rax,1)
 	je     bc <terminating_decimal_to_fraction+0xbc>
 	add    $0x1,%rax
 	cmp    %rax,%r9
 	jbe    238 <terminating_decimal_to_fraction+0x238>
 	test   %dl,%dl
@@ -68,20 +68,20 @@
  R_X86_64_PLT32	strlen-0x4
 	movb   $0x0,-0x1(%r15,%rax,1)
 	movb   $0x31,0x0(%rbp)
 	test   %rbx,%rbx
 	je     1c5 <terminating_decimal_to_fraction+0x1c5>
 	lea    -0x1(%rbx),%rax
 	cmp    $0xffffffffffffffff,%rbx
-	je     280 <terminating_decimal_to_fraction+0x280>
+	je     270 <terminating_decimal_to_fraction+0x270>
 	cmp    $0x6,%rax
-	jbe    280 <terminating_decimal_to_fraction+0x280>
+	jbe    270 <terminating_decimal_to_fraction+0x270>
 	mov    %rbx,%rcx
 	cmp    $0xe,%rax
-	jbe    2a9 <terminating_decimal_to_fraction+0x2a9>
+	jbe    299 <terminating_decimal_to_fraction+0x299>
 	movdqa 0x0(%rip),%xmm0        
  R_X86_64_PC32	.LC0-0x4
 	shr    $0x4,%rcx
 	xor    %eax,%eax
 	nopl   0x0(%rax,%rax,1)
 	mov    %rax,%rdx
 	add    $0x1,%rax
@@ -177,36 +177,28 @@
 	test   %dl,%dl
 	je     d3 <terminating_decimal_to_fraction+0xd3>
 	jmp    c5 <terminating_decimal_to_fraction+0xc5>
 	nopl   (%rax)
 	mov    %r12,%rdi
 	call   250 <terminating_decimal_to_fraction+0x250>
  R_X86_64_PLT32	strlen-0x4
-	mov    %r12,%rdi
-	lea    0x2(%rax),%rsi
-	call   25c <terminating_decimal_to_fraction+0x25c>
- R_X86_64_PLT32	realloc-0x4
-	mov    %rax,%rdi
-	mov    %rax,%r12
-	call   267 <terminating_decimal_to_fraction+0x267>
- R_X86_64_PLT32	strlen-0x4
 	lea    0x1(%r12),%rdi
 	mov    %r12,%rsi
 	lea    0x1(%rax),%rdx
-	call   278 <terminating_decimal_to_fraction+0x278>
+	call   261 <terminating_decimal_to_fraction+0x261>
  R_X86_64_PLT32	memmove-0x4
 	movb   $0x2d,(%r12)
 	jmp    20d <terminating_decimal_to_fraction+0x20d>
-	nop
+	nopl   0x0(%rax,%rax,1)
 	mov    $0x1,%eax
 	nopl   (%rax)
 	movb   $0x30,0x0(%rbp,%rax,1)
 	add    $0x1,%rax
 	cmp    %rax,%rbx
-	jae    288 <terminating_decimal_to_fraction+0x288>
+	jae    278 <terminating_decimal_to_fraction+0x278>
 	jmp    1c5 <terminating_decimal_to_fraction+0x1c5>
 	nopl   0x0(%rax,%rax,1)
 	movb   $0x31,0x0(%rbp)
 	jmp    1c5 <terminating_decimal_to_fraction+0x1c5>
 	xor    %edx,%edx
 	mov    $0x1,%eax
 	jmp    151 <terminating_decimal_to_fraction+0x151>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,11 +1,11 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
-  0x00000020 00000000 b5020000 00460e10 8f02420e .........F....B.
+  0x00000020 00000000 a5020000 00460e10 8f02420e .........F....B.
   0x00000030 188e0342 0e208d04 450e288c 05440e30 ...B. ..E.(..D.0
   0x00000040 8606410e 38830744 0e600309 020a0e38 ..A.8..D.`.....8
   0x00000050 440e3041 0e28420e 20420e18 420e1042 D.0A.(B. B..B..B
   0x00000060 0e084a0b 00000000                   ..J.....
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -3,10 +3,10 @@
   0x00000000 00746572 6d696e61 74696e67 5f646563 .terminating_dec
   0x00000010 696d616c 5f746f5f 66726163 74696f6e imal_to_fraction
   0x00000020 2e63002e 4c433100 2e4c4330 00746572 .c..LC1..LC0.ter
   0x00000030 6d696e61 74696e67 5f646563 696d616c minating_decimal
   0x00000040 5f746f5f 66726163 74696f6e 00737472 _to_fraction.str
   0x00000050 6c656e00 6d616c6c 6f630063 616c6c6f len.malloc.callo
   0x00000060 63006d65 6d637079 00696763 64006469 c.memcpy.igcd.di
-  0x00000070 76696465 00667265 65007265 616c6c6f vide.free.reallo
-  0x00000080 63006d65 6d6d6f76 6500              c.memmove.
+  0x00000070 76696465 00667265 65006d65 6d6d6f76 vide.free.memmov
+  0x00000080 6500                                e.
```

### Comparing `arithmetica-py-1.0.186/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.189/src/python-module/libbasic_math_operations.a`

 * *Files 11% similar despite different names*

#### nm -s {}

```diff
@@ -18,14 +18,17 @@
 _ZN21basic_math_operations6BMONumdvES0_ in basic_math_operations.cpp.o
 _ZN21basic_math_operations17DIVISION_ACCURACYE in basic_math_operations.cpp.o
 _ZN21basic_math_operations6BMONumrmES0_ in basic_math_operations.cpp.o
 _ZN21basic_math_operations6BMONumltES0_ in basic_math_operations.cpp.o
 _ZN21basic_math_operations6BMONumgtES0_ in basic_math_operations.cpp.o
 _ZN21basic_math_operations6BMONumeqES0_ in basic_math_operations.cpp.o
 _ZN21basic_math_operations6BMONumgeES0_ in basic_math_operations.cpp.o
+_ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv in basic_math_operations.cpp.o
+_ZN21basic_math_operations6randomEy in basic_math_operations.cpp.o
+_ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits in basic_math_operations.cpp.o
 strlen_asm in strlen_asm.asm.o
 remove_leading_zeroes in remove_leading_zeroes.asm.o
 remove_leading_zeroes_inplace in remove_leading_zeroes.asm.o
 add_whole in add_whole.asm.o
 add_whole_same_length in add_whole_same_length.asm.o
 add in add.c.o
 subtract_whole in subtract_whole.asm.o
@@ -36,25 +39,29 @@
 multiplyp in multiplyp.c.o
 multiply in multiply.c.o
 _divide_whole_with_remainder in _divide_whole_with_remainder.asm.o
 divide_whole_with_remainder in divide_whole_with_remainder.c.o
 divide_whole in divide_whole.c.o
 dividep in dividep.c.o
 divide in divide.c.o
+abs_mod in abs_mod.c.o
 asmalloc in asmalloc.asm.o
 multiply_whole in multiply_whole.asm.o
 addp in addp.c.o
 remove_zeroes in remove_zeroes.c.o
 increment_whole in increment_whole.c.o
 
 basic_math_operations.c.o:
 
 basic_math_operations.cpp.o:
 0000000000000000 r .LC0
 0000000000000000 r .LC1
+0000000000000002 r .LC12
+0000000000000005 r .LC14
+000000000000001a r .LC15
 0000000000000000 V DW.ref.__gxx_personality_v0
                  U _GLOBAL_OFFSET_TABLE_
                  U _Unwind_Resume
 0000000000000000 u _ZN21basic_math_operations17DIVISION_ACCURACYE
 0000000000000000 T _ZN21basic_math_operations3addENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
 0000000000000480 T _ZN21basic_math_operations3modENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
 0000000000000610 T _ZN21basic_math_operations6BMONumC1ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
@@ -65,35 +72,48 @@
 0000000000000650 T _ZN21basic_math_operations6BMONumC2EPKc
 000000000000003c t _ZN21basic_math_operations6BMONumC2EPKc.cold
 00000000000005c0 T _ZN21basic_math_operations6BMONumC2Ev
 0000000000000000 t _ZN21basic_math_operations6BMONumC2Ev.cold
 0000000000001060 T _ZN21basic_math_operations6BMONumdvES0_
 0000000000000168 t _ZN21basic_math_operations6BMONumdvES0_.cold
 0000000000001aa0 T _ZN21basic_math_operations6BMONumeqES0_
-0000000000001ae0 T _ZN21basic_math_operations6BMONumgeES0_
+0000000000001b50 T _ZN21basic_math_operations6BMONumgeES0_
 0000000000000274 t _ZN21basic_math_operations6BMONumgeES0_.cold
 0000000000001960 T _ZN21basic_math_operations6BMONumgtES0_
 0000000000000254 t _ZN21basic_math_operations6BMONumgtES0_.cold
 0000000000001700 T _ZN21basic_math_operations6BMONumltES0_
 000000000000021c t _ZN21basic_math_operations6BMONumltES0_.cold
 00000000000009e0 T _ZN21basic_math_operations6BMONummiES0_
 00000000000000b4 t _ZN21basic_math_operations6BMONummiES0_.cold
 0000000000000d20 T _ZN21basic_math_operations6BMONummlES0_
 000000000000010e t _ZN21basic_math_operations6BMONummlES0_.cold
 00000000000006a0 T _ZN21basic_math_operations6BMONumplES0_
 000000000000005a t _ZN21basic_math_operations6BMONumplES0_.cold
 00000000000013c0 T _ZN21basic_math_operations6BMONumrmES0_
 00000000000001c2 t _ZN21basic_math_operations6BMONumrmES0_.cold
 0000000000000360 T _ZN21basic_math_operations6divideENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_m
+0000000000002040 T _ZN21basic_math_operations6randomEy
+00000000000002ac t _ZN21basic_math_operations6randomEy.cold
 0000000000000240 T _ZN21basic_math_operations8multiplyENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
 0000000000000120 T _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
+                 U _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
+                 U _ZNSt13random_device7_M_finiEv
+                 U _ZNSt13random_device7_M_initERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+                 U _ZNSt13random_device9_M_getvalEv
+0000000000000000 W _ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv
+0000000000001dc0 t _ZNSt24uniform_int_distributionIiEclISt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EEEEiRT_RKNS0_10param_typeE.isra.0
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
+                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE12_M_constructEmc
+                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm
+                 U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
                  U _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
                  U _ZSt19__throw_logic_errorPKc
+                 U _ZSt20__throw_length_errorPKc
+0000000000000000 u _ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits
                  U _ZdlPvm
                  U __gxx_personality_v0
                  U __stack_chk_fail
                  U add
                  U calloc
                  U divide
                  U divide_whole_with_remainder
@@ -272,14 +292,21 @@
 divide.c.o:
 0000000000000000 T divide
                  U dividep
                  U memmove
                  U remove_zeroes
                  U strlen_asm
 
+abs_mod.c.o:
+0000000000000000 T abs_mod
+                 U calloc
+                 U divide_whole_with_remainder
+                 U free
+                 U strlen
+
 asmalloc.asm.o:
 0000000000000000 T asmalloc
 
 multiply_whole.asm.o:
                  U _multiply_whole
                  U asmalloc
 0000000000000000 T multiply_whole
```

#### file list

```diff
@@ -1,26 +1,27 @@
-----------   0        0        0     1742 1970-01-01 00:00:00.000000 /
+----------   0        0        0     2012 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 basic_math_operations.c.o
-?rw-r--r--   0        0        0    22352 1970-01-01 00:00:00.000000 basic_math_operations.cpp.o
+?rw-r--r--   0        0        0    28944 1970-01-01 00:00:00.000000 basic_math_operations.cpp.o
 ?rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 strlen_asm.asm.o
 ?rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 remove_leading_zeroes.asm.o
 ?rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 add_whole.asm.o
 ?rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 add_whole_same_length.asm.o
 ?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 add.c.o
 ?rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 subtract_whole.asm.o
 ?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 subtract_whole_same_length.asm.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 subtractp.c.o
 ?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 subtract.c.o
 ?rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 _multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 multiplyp.c.o
 ?rw-r--r--   0        0        0     2016 1970-01-01 00:00:00.000000 multiply.c.o
 ?rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
 ?rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
-?rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 divide_whole.c.o
+?rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 divide_whole.c.o
 ?rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 dividep.c.o
 ?rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 divide.c.o
+?rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 abs_mod.c.o
 ?rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 asmalloc.asm.o
 ?rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 multiply_whole.asm.o
 ?rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 addp.c.o
 ?rw-r--r--   0        0        0     1824 1970-01-01 00:00:00.000000 remove_zeroes.c.o
 ?rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 increment_whole.c.o
```

#### basic_math_operations.cpp.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - GNU
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          20880 (bytes into file)
+  Start of section headers:          27216 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
-  Number of section headers:         23
-  Section header string table index: 22
+  Number of section headers:         27
+  Section header string table index: 26
```

##### readelf --wide --sections {}

```diff
@@ -1,32 +1,36 @@
-There are 23 section headers, starting at offset 0x5190:
+There are 27 section headers, starting at offset 0x6a50:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .group            GROUP           0000000000000000 000040 000008 04     20  52  4
-  [ 2] .group            GROUP           0000000000000000 000048 00000c 04     20  36  4
-  [ 3] .text             PROGBITS        0000000000000000 000060 001d4c 00  AX  0   0 16
-  [ 4] .rela.text        RELA            0000000000000000 0036d8 001188 18   I 20   3  8
-  [ 5] .data             PROGBITS        0000000000000000 001dac 000000 00  WA  0   0  1
-  [ 6] .bss              NOBITS          0000000000000000 001dac 000000 00  WA  0   0  1
-  [ 7] .rodata.str1.8    PROGBITS        0000000000000000 001db0 00002a 01 AMS  0   0  8
-  [ 8] .rodata.str1.1    PROGBITS        0000000000000000 001dda 000002 01 AMS  0   0  1
-  [ 9] .text.unlikely    PROGBITS        0000000000000000 001ddc 0002ac 00  AX  0   0  2
-  [10] .rela.text.unlikely RELA            0000000000000000 004860 000330 18   I 20   9  8
-  [11] .gcc_except_table PROGBITS        0000000000000000 002088 000183 00   A  0   0  1
-  [12] .data._ZN21basic_math_operations17DIVISION_ACCURACYE PROGBITS        0000000000000000 002210 000008 00 WAG  0   0  8
-  [13] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 002218 000008 00 WAG  0   0  8
-  [14] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 004b90 000018 18  IG 20  13  8
-  [15] .comment          PROGBITS        0000000000000000 002220 00002c 01  MS  0   0  1
-  [16] .note.GNU-stack   PROGBITS        0000000000000000 00224c 000000 00      0   0  1
-  [17] .note.gnu.property NOTE            0000000000000000 002250 000020 00   A  0   0  8
-  [18] .eh_frame         PROGBITS        0000000000000000 002270 000650 00   A  0   0  8
-  [19] .rela.eh_frame    RELA            0000000000000000 004ba8 0004c8 18   I 20  18  8
-  [20] .symtab           SYMTAB          0000000000000000 0028c0 000588 18     21  18  8
-  [21] .strtab           STRTAB          0000000000000000 002e48 00088d 00      0   0  1
-  [22] .shstrtab         STRTAB          0000000000000000 005070 00011d 00      0   0  1
+  [ 1] .group            GROUP           0000000000000000 000040 000008 04     24  66  4
+  [ 2] .group            GROUP           0000000000000000 000048 000008 04     24  71  4
+  [ 3] .group            GROUP           0000000000000000 000050 000008 04     24  58  4
+  [ 4] .group            GROUP           0000000000000000 000058 00000c 04     24  42  4
+  [ 5] .text             PROGBITS        0000000000000000 000070 0026a1 00  AX  0   0 16
+  [ 6] .rela.text        RELA            0000000000000000 004990 001560 18   I 24   5  8
+  [ 7] .data             PROGBITS        0000000000000000 002711 000000 00  WA  0   0  1
+  [ 8] .bss              NOBITS          0000000000000000 002711 000000 00  WA  0   0  1
+  [ 9] .rodata.str1.8    PROGBITS        0000000000000000 002718 00002a 01 AMS  0   0  8
+  [10] .rodata.str1.1    PROGBITS        0000000000000000 002742 00001c 01 AMS  0   0  1
+  [11] .text.unlikely    PROGBITS        0000000000000000 00275e 00034d 00  AX  0   0  2
+  [12] .rela.text.unlikely RELA            0000000000000000 005ef0 0003f0 18   I 24  11  8
+  [13] .gcc_except_table PROGBITS        0000000000000000 002aab 0001c5 00   A  0   0  1
+  [14] .text._ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv PROGBITS        0000000000000000 002c70 0000f3 00 AXG  0   0 16
+  [15] .rodata._ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits PROGBITS        0000000000000000 002d80 0000c9 00  AG  0   0 32
+  [16] .data._ZN21basic_math_operations17DIVISION_ACCURACYE PROGBITS        0000000000000000 002e50 000008 00 WAG  0   0  8
+  [17] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 002e58 000008 00 WAG  0   0  8
+  [18] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 0062e0 000018 18  IG 24  17  8
+  [19] .comment          PROGBITS        0000000000000000 002e60 00002c 01  MS  0   0  1
+  [20] .note.GNU-stack   PROGBITS        0000000000000000 002e8c 000000 00      0   0  1
+  [21] .note.gnu.property NOTE            0000000000000000 002e90 000020 00   A  0   0  8
+  [22] .eh_frame         PROGBITS        0000000000000000 002eb0 000770 00   A  0   0  8
+  [23] .rela.eh_frame    RELA            0000000000000000 0062f8 000558 18   I 24  22  8
+  [24] .symtab           SYMTAB          0000000000000000 003620 000720 18     25  24  8
+  [25] .strtab           STRTAB          0000000000000000 003d40 000c4e 00      0   0  1
+  [26] .shstrtab         STRTAB          0000000000000000 006850 0001fe 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   R (retain), D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,62 +1,79 @@
 
-Symbol table '.symtab' contains 59 entries:
+Symbol table '.symtab' contains 76 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS basic_math_operations.cpp
-     2: 0000000000000000     0 SECTION LOCAL  DEFAULT    3 .text
-     3: 0000000000000000     0 SECTION LOCAL  DEFAULT    9 .text.unlikely
-     4: 0000000000000000     0 SECTION LOCAL  DEFAULT   11 .gcc_except_table
-     5: 0000000000000000    29 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumC2Ev.cold
-     6: 000000000000001e    29 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumC2ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
-     7: 000000000000003c    29 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumC2EPKc.cold
-     8: 000000000000005a    89 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumplES0_.cold
-     9: 00000000000000b4    89 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONummiES0_.cold
-    10: 000000000000010e    89 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONummlES0_.cold
-    11: 0000000000000168    89 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumdvES0_.cold
-    12: 00000000000001c2    89 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumrmES0_.cold
-    13: 000000000000021c    56 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumltES0_.cold
-    14: 0000000000000254    32 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumgtES0_.cold
-    15: 0000000000000274    56 FUNC    LOCAL  DEFAULT    9 _ZN21basic_math_operations6BMONumgeES0_.cold
-    16: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    7 .LC0
-    17: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    8 .LC1
-    18: 0000000000000000   278 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations3addENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
-    19: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
-    20: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add
-    21: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
-    22: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
-    23: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
-    24: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
-    25: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
-    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt19__throw_logic_errorPKc
-    27: 0000000000000120   278 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
-    28: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract
-    29: 0000000000000240   278 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations8multiplyENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
-    30: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply
-    31: 0000000000000360   278 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6divideENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_m
-    32: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
-    33: 0000000000000480   310 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations3modENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
-    34: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide_whole_with_remainder
-    35: 00000000000005c0    69 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumC2Ev
-    36: 0000000000000000     8 OBJECT  WEAK   HIDDEN    13 DW.ref.__gxx_personality_v0
-    37: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
-    38: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __gxx_personality_v0
-    39: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZdlPvm
-    40: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Unwind_Resume
-    41: 00000000000005c0    69 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumC1Ev
-    42: 0000000000000610    52 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumC2ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-    43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
-    44: 0000000000000610    52 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumC1ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
-    45: 0000000000000650    76 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumC2EPKc
-    46: 0000000000000650    76 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumC1EPKc
-    47: 00000000000006a0   828 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumplES0_
-    48: 00000000000009e0   828 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONummiES0_
-    49: 0000000000000d20   828 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONummlES0_
-    50: 0000000000001060   860 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumdvES0_
-    51: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _GLOBAL_OFFSET_TABLE_
-    52: 0000000000000000     8 OBJECT  UNIQUE DEFAULT   12 _ZN21basic_math_operations17DIVISION_ACCURACYE
-    53: 00000000000013c0   828 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumrmES0_
-    54: 0000000000001700   599 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumltES0_
-    55: 0000000000001960   311 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumgtES0_
-    56: 0000000000001aa0    59 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumeqES0_
-    57: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcmp
-    58: 0000000000001ae0   620 FUNC    GLOBAL DEFAULT    3 _ZN21basic_math_operations6BMONumgeES0_
+     2: 0000000000000000     0 SECTION LOCAL  DEFAULT    5 .text
+     3: 0000000000000000     0 SECTION LOCAL  DEFAULT   11 .text.unlikely
+     4: 0000000000000000     0 SECTION LOCAL  DEFAULT   13 .gcc_except_table
+     5: 0000000000000000    29 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumC2Ev.cold
+     6: 000000000000001e    29 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumC2ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
+     7: 000000000000003c    29 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumC2EPKc.cold
+     8: 000000000000005a    89 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumplES0_.cold
+     9: 00000000000000b4    89 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONummiES0_.cold
+    10: 000000000000010e    89 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONummlES0_.cold
+    11: 0000000000000168    89 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumdvES0_.cold
+    12: 00000000000001c2    89 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumrmES0_.cold
+    13: 000000000000021c    56 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumltES0_.cold
+    14: 0000000000000254    32 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumgtES0_.cold
+    15: 0000000000000274    56 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6BMONumgeES0_.cold
+    16: 0000000000000000     0 SECTION LOCAL  DEFAULT   14 .text._ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv
+    17: 0000000000001dc0   631 FUNC    LOCAL  DEFAULT    5 _ZNSt24uniform_int_distributionIiEclISt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EEEEiRT_RKNS0_10param_typeE.isra.0
+    18: 00000000000002ac   161 FUNC    LOCAL  DEFAULT   11 _ZN21basic_math_operations6randomEy.cold
+    19: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    9 .LC0
+    20: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT   10 .LC1
+    21: 0000000000000002     0 NOTYPE  LOCAL  DEFAULT   10 .LC12
+    22: 000000000000001a     0 NOTYPE  LOCAL  DEFAULT   10 .LC15
+    23: 0000000000000005     0 NOTYPE  LOCAL  DEFAULT   10 .LC14
+    24: 0000000000000000   278 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations3addENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
+    25: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
+    26: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND add
+    27: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
+    28: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    29: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
+    30: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
+    31: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
+    32: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt19__throw_logic_errorPKc
+    33: 0000000000000120   278 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
+    34: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND subtract
+    35: 0000000000000240   278 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations8multiplyENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
+    36: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND multiply
+    37: 0000000000000360   278 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6divideENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_m
+    38: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
+    39: 0000000000000480   310 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations3modENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
+    40: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide_whole_with_remainder
+    41: 00000000000005c0    69 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumC2Ev
+    42: 0000000000000000     8 OBJECT  WEAK   HIDDEN    17 DW.ref.__gxx_personality_v0
+    43: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm
+    44: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __gxx_personality_v0
+    45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZdlPvm
+    46: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _Unwind_Resume
+    47: 00000000000005c0    69 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumC1Ev
+    48: 0000000000000610    52 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumC2ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    49: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_
+    50: 0000000000000610    52 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumC1ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    51: 0000000000000650    76 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumC2EPKc
+    52: 0000000000000650    76 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumC1EPKc
+    53: 00000000000006a0   828 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumplES0_
+    54: 00000000000009e0   828 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONummiES0_
+    55: 0000000000000d20   828 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONummlES0_
+    56: 0000000000001060   860 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumdvES0_
+    57: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _GLOBAL_OFFSET_TABLE_
+    58: 0000000000000000     8 OBJECT  UNIQUE DEFAULT   16 _ZN21basic_math_operations17DIVISION_ACCURACYE
+    59: 00000000000013c0   828 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumrmES0_
+    60: 0000000000001700   599 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumltES0_
+    61: 0000000000001960   311 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumgtES0_
+    62: 0000000000001aa0   175 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumeqES0_
+    63: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
+    64: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcmp
+    65: 0000000000001b50   620 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6BMONumgeES0_
+    66: 0000000000000000   243 FUNC    WEAK   DEFAULT   14 _ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv
+    67: 0000000000002040  1633 FUNC    GLOBAL DEFAULT    5 _ZN21basic_math_operations6randomEy
+    68: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt13random_device7_M_initERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+    69: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt13random_device9_M_getvalEv
+    70: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE12_M_constructEmc
+    71: 0000000000000000   201 OBJECT  UNIQUE DEFAULT   15 _ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits
+    72: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
+    73: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm
+    74: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZNSt13random_device7_M_finiEv
+    75: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _ZSt20__throw_length_errorPKc
```

##### readelf --wide --relocs {}

```diff
@@ -1,172 +1,207 @@
 
-Relocation section '.rela.text' at offset 0x36d8 contains 187 entries:
+Relocation section '.rela.text' at offset 0x4990 contains 228 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-000000000000003c  0000001300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000053  0000001400000004 R_X86_64_PLT32         0000000000000000 add - 4
-0000000000000068  0000001500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000097  0000001600000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000000d9  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000000f7  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000106  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000010d  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000112  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-000000000000015c  0000001300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000173  0000001c00000004 R_X86_64_PLT32         0000000000000000 subtract - 4
-0000000000000188  0000001500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001b7  0000001600000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000001f9  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000217  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000226  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000022d  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000232  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-000000000000027c  0000001300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000293  0000001e00000004 R_X86_64_PLT32         0000000000000000 multiply - 4
-00000000000002a8  0000001500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000002d7  0000001600000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000319  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000337  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000346  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000034d  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000352  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-000000000000039d  0000001300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000003b6  0000002000000004 R_X86_64_PLT32         0000000000000000 divide - 4
-00000000000003cb  0000001500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000003fa  0000001600000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000439  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000457  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000466  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000046d  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000472  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000004be  0000001300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000004d9  0000001300000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000004ed  0000002200000004 R_X86_64_PLT32         0000000000000000 divide_whole_with_remainder - 4
-00000000000004fa  0000001600000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000050f  0000001500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000053e  0000001600000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000579  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000597  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000005a6  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-00000000000005ad  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-00000000000005b2  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000005d8  0000001100000002 R_X86_64_PC32          0000000000000000 .LC1 - 4
-00000000000005f0  0000002500000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-000000000000062f  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
-0000000000000675  0000001500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000687  0000002500000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
-00000000000006d4  0000002900000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
-0000000000000787  0000001200000004 R_X86_64_PLT32         0000000000000000 _ZN21basic_math_operations3addENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
-000000000000080e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000826  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000083e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000008ad  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000008ca  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000008f0  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000090d  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000092f  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000096f  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000974  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000993  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000099a  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-000000000000099f  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000a14  0000002900000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
-0000000000000ac7  0000001b00000004 R_X86_64_PLT32         0000000000000120 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
-0000000000000b4e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000b66  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000b7e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000bed  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000c0a  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000c30  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000c4d  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000c6f  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000caf  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000cb4  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000cd3  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000000cda  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000cdf  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000000d54  0000002900000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
-0000000000000e07  0000001d00000004 R_X86_64_PLT32         0000000000000240 _ZN21basic_math_operations8multiplyENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
-0000000000000e8e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000ea6  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000ebe  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000f2d  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000f4a  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000f70  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000000f8d  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000faf  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000fef  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000000ff4  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000001013  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000101a  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-000000000000101f  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000001097  0000002900000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
-000000000000109e  000000340000002a R_X86_64_REX_GOTPCRELX 0000000000000000 _ZN21basic_math_operations17DIVISION_ACCURACYE - 4
-000000000000115e  0000001f00000004 R_X86_64_PLT32         0000000000000360 _ZN21basic_math_operations6divideENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_m - 4
-00000000000011e5  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000011fd  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001215  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000128d  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000012aa  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000012d0  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000012ed  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000130f  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000134f  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001354  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000001373  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-000000000000137a  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-000000000000137f  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000013f4  0000002900000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
-00000000000014a7  0000002100000004 R_X86_64_PLT32         0000000000000480 _ZN21basic_math_operations3modENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
-000000000000152e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001546  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000155e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000015cd  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000015ea  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000001610  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-000000000000162d  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000164f  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000168f  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001694  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000016b3  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-00000000000016ba  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-00000000000016bf  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000017dc  0000001b00000004 R_X86_64_PLT32         0000000000000120 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
-00000000000017f4  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000180c  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001830  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000189d  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000018ba  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000018e0  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-00000000000018fd  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000001913  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001918  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-000000000000191d  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000001924  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001929  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-00000000000019db  0000003600000004 R_X86_64_PLT32         0000000000001700 _ZN21basic_math_operations6BMONumltES0_ - 4
-00000000000019f6  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001a40  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000001a5d  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000001a73  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001a78  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000001a7d  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000001acd  0000003900000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
-0000000000001b60  0000003700000004 R_X86_64_PLT32         0000000000001960 _ZN21basic_math_operations6BMONumgtES0_ - 4
-0000000000001b7f  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001c24  0000003800000004 R_X86_64_PLT32         0000000000001aa0 _ZN21basic_math_operations6BMONumeqES0_ - 4
-0000000000001c43  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000001c60  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000001c7d  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000001cb8  0000001700000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
-0000000000001cd5  0000001800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000001ceb  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001cf0  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
-0000000000001cf5  0000001900000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
-0000000000001d13  0000001000000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
-0000000000001d18  0000001a00000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000003c  0000001900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000053  0000001a00000004 R_X86_64_PLT32         0000000000000000 add - 4
+0000000000000068  0000001b00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000097  0000001c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000000d9  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000000f7  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000106  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000010d  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000112  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000015c  0000001900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000173  0000002200000004 R_X86_64_PLT32         0000000000000000 subtract - 4
+0000000000000188  0000001b00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000001b7  0000001c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000001f9  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000217  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000226  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000022d  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000232  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000027c  0000001900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000293  0000002400000004 R_X86_64_PLT32         0000000000000000 multiply - 4
+00000000000002a8  0000001b00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000002d7  0000001c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000319  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000337  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000346  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000034d  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000352  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000039d  0000001900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000003b6  0000002600000004 R_X86_64_PLT32         0000000000000000 divide - 4
+00000000000003cb  0000001b00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000003fa  0000001c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000439  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000457  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000466  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000046d  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000472  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000004be  0000001900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004d9  0000001900000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004ed  0000002800000004 R_X86_64_PLT32         0000000000000000 divide_whole_with_remainder - 4
+00000000000004fa  0000001c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000050f  0000001b00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000053e  0000001c00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000579  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000597  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000005a6  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+00000000000005ad  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+00000000000005b2  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000005d8  0000001400000002 R_X86_64_PC32          0000000000000000 .LC1 - 4
+00000000000005f0  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+000000000000062f  0000003100000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_assignERKS4_ - 4
+0000000000000675  0000001b00000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000687  0000002b00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE10_M_replaceEmmPKcm - 4
+00000000000006d4  0000002f00000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
+0000000000000787  0000001800000004 R_X86_64_PLT32         0000000000000000 _ZN21basic_math_operations3addENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
+000000000000080e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000826  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000083e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000008ad  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000008ca  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000008f0  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000090d  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000092f  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000096f  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000974  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000993  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000099a  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+000000000000099f  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000a14  0000002f00000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
+0000000000000ac7  0000002100000004 R_X86_64_PLT32         0000000000000120 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
+0000000000000b4e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000b66  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000b7e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000bed  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000c0a  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000c30  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000c4d  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000c6f  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000caf  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000cb4  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000cd3  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000cda  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000cdf  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000000d54  0000002f00000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
+0000000000000e07  0000002300000004 R_X86_64_PLT32         0000000000000240 _ZN21basic_math_operations8multiplyENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
+0000000000000e8e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000ea6  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000ebe  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000f2d  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000f4a  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000f70  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000000f8d  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000faf  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000fef  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000000ff4  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000001013  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000101a  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+000000000000101f  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000001097  0000002f00000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
+000000000000109e  0000003a0000002a R_X86_64_REX_GOTPCRELX 0000000000000000 _ZN21basic_math_operations17DIVISION_ACCURACYE - 4
+000000000000115e  0000002500000004 R_X86_64_PLT32         0000000000000360 _ZN21basic_math_operations6divideENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_m - 4
+00000000000011e5  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000011fd  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001215  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000128d  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000012aa  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000012d0  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000012ed  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000130f  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000134f  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001354  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000001373  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+000000000000137a  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+000000000000137f  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000013f4  0000002f00000004 R_X86_64_PLT32         00000000000005c0 _ZN21basic_math_operations6BMONumC1Ev - 4
+00000000000014a7  0000002700000004 R_X86_64_PLT32         0000000000000480 _ZN21basic_math_operations3modENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
+000000000000152e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001546  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000155e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000015cd  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000015ea  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000001610  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+000000000000162d  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000164f  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000168f  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001694  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000016b3  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+00000000000016ba  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+00000000000016bf  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000017dc  0000002100000004 R_X86_64_PLT32         0000000000000120 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_ - 4
+00000000000017f4  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000180c  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001830  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000189d  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000018ba  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000018e0  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+00000000000018fd  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000001913  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001918  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+000000000000191d  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000001924  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001929  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+00000000000019db  0000003c00000004 R_X86_64_PLT32         0000000000001700 _ZN21basic_math_operations6BMONumltES0_ - 4
+00000000000019f6  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001a40  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000001a5d  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000001a73  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001a78  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000001a7d  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000001aa9  0000001400000002 R_X86_64_PC32          0000000000000000 .LC1 - 4
+0000000000001ab2  0000001500000002 R_X86_64_PC32          0000000000000002 .LC12 - 4
+0000000000001ac6  0000003f00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001ad5  0000003f00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001ae4  0000003f00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001b15  0000004000000004 R_X86_64_PLT32         0000000000000000 memcmp - 4
+0000000000001b37  0000003f00000004 R_X86_64_PLT32         0000000000000000 _ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc - 4
+0000000000001bd0  0000003d00000004 R_X86_64_PLT32         0000000000001960 _ZN21basic_math_operations6BMONumgtES0_ - 4
+0000000000001bef  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001c94  0000003e00000004 R_X86_64_PLT32         0000000000001aa0 _ZN21basic_math_operations6BMONumeqES0_ - 4
+0000000000001cb3  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000001cd0  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000001ced  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000001d28  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000001d45  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000001d5b  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001d60  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000001d65  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000001d83  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000001d88  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000001e23  0000004200000004 R_X86_64_PLT32         0000000000000000 _ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv - 4
+0000000000001f8d  0000004200000004 R_X86_64_PLT32         0000000000000000 _ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv - 4
+0000000000002011  0000004200000004 R_X86_64_PLT32         0000000000000000 _ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv - 4
+0000000000002029  0000004200000004 R_X86_64_PLT32         0000000000000000 _ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv - 4
+00000000000020ea  0000004400000004 R_X86_64_PLT32         0000000000000000 _ZNSt13random_device7_M_initERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE - 4
+0000000000002108  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000002112  0000004500000004 R_X86_64_PLT32         0000000000000000 _ZNSt13random_device9_M_getvalEv - 4
+0000000000002254  0000004600000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE12_M_constructEmc - 4
+000000000000226c  000000470000002a R_X86_64_REX_GOTPCRELX 0000000000000000 _ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits - 4
+00000000000022b8  000000470000002a R_X86_64_REX_GOTPCRELX 0000000000000000 _ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits - 4
+00000000000022e2  0000004800000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+0000000000002303  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000002354  0000004900000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm - 4
+000000000000237a  0000001600000002 R_X86_64_PC32          000000000000001a .LC15 - 4
+0000000000002382  0000004800000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+0000000000002394  0000004800000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm - 4
+0000000000002417  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000002483  0000003200000004 R_X86_64_PLT32         0000000000000610 _ZN21basic_math_operations6BMONumC1ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE - 4
+000000000000249c  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000024b6  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000024c0  0000004a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt13random_device7_M_finiEv - 4
+0000000000002569  0000001d00000004 R_X86_64_PLT32         0000000000000000 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm - 4
+0000000000002586  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000025d1  0000001e00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000263f  0000001700000002 R_X86_64_PC32          0000000000000005 .LC14 - 4
+0000000000002644  0000004b00000004 R_X86_64_PLT32         0000000000000000 _ZSt20__throw_length_errorPKc - 4
+000000000000264b  0000001300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+0000000000002650  0000002000000004 R_X86_64_PLT32         0000000000000000 _ZSt19__throw_logic_errorPKc - 4
+0000000000002655  0000001f00000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
 0000000000000601  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely - 4
 0000000000000640  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1a
 0000000000000698  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 38
 00000000000009c0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 7b
 00000000000009cc  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 6e
 00000000000009d8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 56
 0000000000000d00  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + d5
@@ -180,68 +215,82 @@
 00000000000013b8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 164
 00000000000016e0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1e3
 00000000000016ec  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1d6
 00000000000016f8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1be
 0000000000001947  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 230
 0000000000001953  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 218
 0000000000001a93  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 250
-0000000000001d24  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 270
-0000000000001d30  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2a0
-0000000000001d3c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 288
-0000000000001d48  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 288
+0000000000001d94  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 270
+0000000000001da0  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2a0
+0000000000001dac  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 288
+0000000000001db8  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 288
+0000000000002661  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2c1
+000000000000266d  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2a8
+0000000000002679  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2ed
+0000000000002685  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 308
+0000000000002691  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 323
+000000000000269d  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2db
 
-Relocation section '.rela.text.unlikely' at offset 0x4860 contains 34 entries:
+Relocation section '.rela.text.unlikely' at offset 0x5ef0 contains 42 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000011  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000019  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000002f  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000037  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000004d  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000055  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-000000000000006e  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000097  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000009f  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000000ad  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000c8  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000f1  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000000f9  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000107  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000122  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-000000000000014b  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000153  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000161  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000189  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001a5  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001ad  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-00000000000001bb  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001d6  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000001ff  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000207  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000215  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000230  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000248  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000250  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000268  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-0000000000000270  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
-0000000000000288  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000002a0  0000002700000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
-00000000000002a8  0000002800000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000011  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000019  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000002f  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000037  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000004d  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000055  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+000000000000006e  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000097  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000009f  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000000ad  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000c8  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000f1  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000000f9  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000107  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000122  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+000000000000014b  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000153  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000161  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000189  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001a5  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001ad  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000001bb  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001d6  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000001ff  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000207  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000215  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000230  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000248  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000250  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000268  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000270  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000288  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000002a0  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000002a8  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+00000000000002c1  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000002db  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+00000000000002e5  0000004a00000004 R_X86_64_PLT32         0000000000000000 _ZNSt13random_device7_M_finiEv - 4
+00000000000002ed  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
+0000000000000306  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000321  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000341  0000002d00000004 R_X86_64_PLT32         0000000000000000 _ZdlPvm - 4
+0000000000000349  0000002e00000004 R_X86_64_PLT32         0000000000000000 _Unwind_Resume - 4
 
-Relocation section '.rela.data.rel.local.DW.ref.__gxx_personality_v0' at offset 0x4b90 contains 1 entry:
+Relocation section '.rela.data.rel.local.DW.ref.__gxx_personality_v0' at offset 0x62e0 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000000  0000002600000001 R_X86_64_64            0000000000000000 __gxx_personality_v0 + 0
+0000000000000000  0000002c00000001 R_X86_64_64            0000000000000000 __gxx_personality_v0 + 0
 
-Relocation section '.rela.eh_frame' at offset 0x4ba8 contains 51 entries:
+Relocation section '.rela.eh_frame' at offset 0x62f8 contains 57 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
 0000000000000064  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 120
 00000000000000a8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 240
 00000000000000ec  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 360
 0000000000000130  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 480
-0000000000000187  0000002400000002 R_X86_64_PC32          0000000000000000 DW.ref.__gxx_personality_v0 + 0
+0000000000000187  0000002a00000002 R_X86_64_PC32          0000000000000000 DW.ref.__gxx_personality_v0 + 0
 000000000000019c  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 5c0
 00000000000001a5  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 0
 00000000000001cc  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 0
 00000000000001d5  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 8
 00000000000001ec  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 610
 00000000000001f5  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 10
 000000000000021c  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 1e
@@ -275,11 +324,17 @@
 0000000000000538  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 21c
 0000000000000541  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 136
 000000000000055c  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1960
 0000000000000565  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 13e
 00000000000005a4  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 254
 00000000000005ad  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 14c
 00000000000005c8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1aa0
-00000000000005e0  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1ae0
-00000000000005e9  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 154
-0000000000000630  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 274
-0000000000000639  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 17b
+0000000000000624  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1b50
+000000000000062d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 154
+0000000000000674  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 274
+000000000000067d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 17b
+0000000000000698  0000001000000002 R_X86_64_PC32          0000000000000000 .text._ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv + 0
+00000000000006ac  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 1dc0
+00000000000006f8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 2040
+0000000000000701  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 183
+0000000000000754  0000000300000002 R_X86_64_PC32          0000000000000000 .text.unlikely + 2ac
+000000000000075d  0000000400000002 R_X86_64_PC32          0000000000000000 .gcc_except_table + 1bd
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -660,68 +660,212 @@
   DW_CFA_offset: r12 (r12) at cfa-32
   DW_CFA_offset: r13 (r13) at cfa-24
   DW_CFA_offset: r14 (r14) at cfa-16
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000005c0 0000000000000014 000005c4 FDE cie=00000000 pc=0000000000001aa0..0000000000001adb
-  DW_CFA_advance_loc: 38 to 0000000000001ac6
+000005c0 0000000000000058 000005c4 FDE cie=00000000 pc=0000000000001aa0..0000000000001b4f
+  DW_CFA_advance_loc: 6 to 0000000000001aa6
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 20 to 0000000000001ada
+  DW_CFA_offset: r13 (r13) at cfa-16
+  DW_CFA_advance_loc: 9 to 0000000000001aaf
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r12 (r12) at cfa-24
+  DW_CFA_advance_loc: 8 to 0000000000001ab7
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r6 (rbp) at cfa-32
+  DW_CFA_advance_loc: 7 to 0000000000001abe
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r3 (rbx) at cfa-40
+  DW_CFA_advance_loc: 7 to 0000000000001ac5
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 55 to 0000000000001afc
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 1 to 0000000000001afd
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 0000000000001afe
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000001b00
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000001b02
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 6 to 0000000000001b08
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 26 to 0000000000001b22
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 1 to 0000000000001b23
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 0000000000001b24
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000001b26
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000001b28
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 8 to 0000000000001b30
+  DW_CFA_restore_state
+  DW_CFA_advance_loc: 19 to 0000000000001b43
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 6 to 0000000000001b49
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 1 to 0000000000001b4a
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000001b4c
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000001b4e
   DW_CFA_def_cfa_offset: 8
   DW_CFA_nop
 
-000005d8 000000000000004c 00000468 FDE cie=00000174 pc=0000000000001ae0..0000000000001d4c
-  Augmentation data:     6b fb ff ff
-  DW_CFA_advance_loc: 6 to 0000000000001ae6
+0000061c 000000000000004c 000004ac FDE cie=00000174 pc=0000000000001b50..0000000000001dbc
+  Augmentation data:     27 fb ff ff
+  DW_CFA_advance_loc: 6 to 0000000000001b56
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
-  DW_CFA_advance_loc: 2 to 0000000000001ae8
+  DW_CFA_advance_loc: 2 to 0000000000001b58
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
-  DW_CFA_advance_loc: 2 to 0000000000001aea
+  DW_CFA_advance_loc: 2 to 0000000000001b5a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 5 to 0000000000001aef
+  DW_CFA_advance_loc: 5 to 0000000000001b5f
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000001af0
+  DW_CFA_advance_loc: 1 to 0000000000001b60
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 1 to 0000000000001af1
+  DW_CFA_advance_loc: 1 to 0000000000001b61
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 0000000000001af8
+  DW_CFA_advance_loc: 7 to 0000000000001b68
   DW_CFA_def_cfa_offset: 160
-  DW_CFA_advance_loc1: 163 to 0000000000001b9b
+  DW_CFA_advance_loc1: 163 to 0000000000001c0b
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 0000000000001b9f
+  DW_CFA_advance_loc: 4 to 0000000000001c0f
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001ba0
+  DW_CFA_advance_loc: 1 to 0000000000001c10
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001ba2
+  DW_CFA_advance_loc: 2 to 0000000000001c12
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001ba4
+  DW_CFA_advance_loc: 2 to 0000000000001c14
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001ba6
+  DW_CFA_advance_loc: 2 to 0000000000001c16
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001ba8
+  DW_CFA_advance_loc: 2 to 0000000000001c18
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 8 to 0000000000001bb0
+  DW_CFA_advance_loc: 8 to 0000000000001c20
   DW_CFA_restore_state
 
-00000628 0000000000000024 000004b8 FDE cie=00000174 pc=0000000000000274..00000000000002ac
-  Augmentation data:     42 fb ff ff
+0000066c 0000000000000020 000004fc FDE cie=00000174 pc=0000000000000274..00000000000002ac
+  Augmentation data:     fe fa ff ff
   DW_CFA_def_cfa_offset: 160
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_offset: r12 (r12) at cfa-40
   DW_CFA_offset: r13 (r13) at cfa-32
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_offset: r15 (r15) at cfa-16
+
+00000690 0000000000000010 00000694 FDE cie=00000000 pc=0000000000000000..00000000000000f3
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
+
+000006a4 0000000000000048 000006a8 FDE cie=00000000 pc=0000000000001dc0..0000000000002037
+  DW_CFA_advance_loc: 2 to 0000000000001dc2
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r15 (r15) at cfa-16
+  DW_CFA_advance_loc: 5 to 0000000000001dc7
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r14 (r14) at cfa-24
+  DW_CFA_advance_loc: 2 to 0000000000001dc9
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r13 (r13) at cfa-32
+  DW_CFA_advance_loc: 5 to 0000000000001dce
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r12 (r12) at cfa-40
+  DW_CFA_advance_loc: 7 to 0000000000001dd5
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_offset: r6 (rbp) at cfa-48
+  DW_CFA_advance_loc: 9 to 0000000000001dde
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_offset: r3 (rbx) at cfa-56
+  DW_CFA_advance_loc: 4 to 0000000000001de2
+  DW_CFA_def_cfa_offset: 64
+  DW_CFA_advance_loc1: 178 to 0000000000001e94
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_advance_loc: 5 to 0000000000001e99
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 1 to 0000000000001e9a
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 2 to 0000000000001e9c
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 0000000000001e9e
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 0000000000001ea0
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 0000000000001ea2
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 6 to 0000000000001ea8
+  DW_CFA_restore_state
+  DW_CFA_nop
+
+000006f0 0000000000000058 00000580 FDE cie=00000174 pc=0000000000002040..00000000000026a1
+  Augmentation data:     82 fa ff ff
+  DW_CFA_advance_loc: 6 to 0000000000002046
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_offset: r15 (r15) at cfa-16
+  DW_CFA_advance_loc: 2 to 0000000000002048
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_offset: r14 (r14) at cfa-24
+  DW_CFA_advance_loc: 2 to 000000000000204a
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_offset: r13 (r13) at cfa-32
+  DW_CFA_advance_loc: 2 to 000000000000204c
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_offset: r12 (r12) at cfa-40
+  DW_CFA_advance_loc: 1 to 000000000000204d
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_offset: r6 (rbp) at cfa-48
+  DW_CFA_advance_loc: 1 to 000000000000204e
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_offset: r3 (rbx) at cfa-56
+  DW_CFA_advance_loc: 7 to 0000000000002055
+  DW_CFA_def_cfa_offset: 4152
+  DW_CFA_advance_loc: 12 to 0000000000002061
+  DW_CFA_def_cfa_offset: 8248
+  DW_CFA_advance_loc: 12 to 000000000000206d
+  DW_CFA_def_cfa_offset: 10208
+  DW_CFA_advance_loc2: 1146 to 00000000000024e7
+  DW_CFA_remember_state
+  DW_CFA_def_cfa_offset: 56
+  DW_CFA_advance_loc: 1 to 00000000000024e8
+  DW_CFA_def_cfa_offset: 48
+  DW_CFA_advance_loc: 1 to 00000000000024e9
+  DW_CFA_def_cfa_offset: 40
+  DW_CFA_advance_loc: 2 to 00000000000024eb
+  DW_CFA_def_cfa_offset: 32
+  DW_CFA_advance_loc: 2 to 00000000000024ed
+  DW_CFA_def_cfa_offset: 24
+  DW_CFA_advance_loc: 2 to 00000000000024ef
+  DW_CFA_def_cfa_offset: 16
+  DW_CFA_advance_loc: 2 to 00000000000024f1
+  DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 7 to 00000000000024f8
+  DW_CFA_restore_state
   DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
+0000074c 0000000000000020 000005dc FDE cie=00000174 pc=00000000000002ac..000000000000034d
+  Augmentation data:     60 fa ff ff
+  DW_CFA_def_cfa_offset: 10208
+  DW_CFA_offset: r3 (rbx) at cfa-56
+  DW_CFA_offset: r6 (rbp) at cfa-48
+  DW_CFA_offset: r12 (r12) at cfa-40
+  DW_CFA_offset: r13 (r13) at cfa-32
+  DW_CFA_offset: r14 (r14) at cfa-24
+  DW_CFA_offset: r15 (r15) at cfa-16
```

##### strings --all --bytes=8 {}

```diff
@@ -8,28 +8,42 @@
 []A\A]A^A_
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATUSH
 []A\A]A^A_
 []A\A]A^
 []A\A]A^A_
+[]A\A]A^A_
+AWAVAUATUSH
+|$`H;<$t
+|$`H;<$t
+|$@H;|$(t
+[]A\A]A^A_
 basic_string::_M_construct null not valid
+basic_string::append
+|$`H;<$t
+|$@H;|$(t
+|$`H;<$t
+|$`H;<$t
+00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
 GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
 basic_math_operations.cpp
 _ZN21basic_math_operations6BMONumC2Ev.cold
 _ZN21basic_math_operations6BMONumC2ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 _ZN21basic_math_operations6BMONumC2EPKc.cold
 _ZN21basic_math_operations6BMONumplES0_.cold
 _ZN21basic_math_operations6BMONummiES0_.cold
 _ZN21basic_math_operations6BMONummlES0_.cold
 _ZN21basic_math_operations6BMONumdvES0_.cold
 _ZN21basic_math_operations6BMONumrmES0_.cold
 _ZN21basic_math_operations6BMONumltES0_.cold
 _ZN21basic_math_operations6BMONumgtES0_.cold
 _ZN21basic_math_operations6BMONumgeES0_.cold
+_ZNSt24uniform_int_distributionIiEclISt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EEEEiRT_RKNS0_10param_typeE.isra.0
+_ZN21basic_math_operations6randomEy.cold
 _ZN21basic_math_operations3addENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
 _ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_createERmm
 __stack_chk_fail
 _ZSt19__throw_logic_errorPKc
 _ZN21basic_math_operations8subtractENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
 subtract
 _ZN21basic_math_operations8multiplyENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_
@@ -53,20 +67,33 @@
 _ZN21basic_math_operations6BMONumdvES0_
 _GLOBAL_OFFSET_TABLE_
 _ZN21basic_math_operations17DIVISION_ACCURACYE
 _ZN21basic_math_operations6BMONumrmES0_
 _ZN21basic_math_operations6BMONumltES0_
 _ZN21basic_math_operations6BMONumgtES0_
 _ZN21basic_math_operations6BMONumeqES0_
+_ZNKSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7compareEPKc
 _ZN21basic_math_operations6BMONumgeES0_
+_ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv
+_ZN21basic_math_operations6randomEy
+_ZNSt13random_device7_M_initERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE
+_ZNSt13random_device9_M_getvalEv
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE12_M_constructEmc
+_ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE9_M_appendEPKcm
+_ZNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEE7reserveEm
+_ZNSt13random_device7_M_finiEv
+_ZSt20__throw_length_errorPKc
 .shstrtab
 .rela.text
 .rodata.str1.8
 .rodata.str1.1
 .rela.text.unlikely
 .gcc_except_table
+.text._ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv
+.rodata._ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits
 .data._ZN21basic_math_operations17DIVISION_ACCURACYE
 .rela.data.rel.local.DW.ref.__gxx_personality_v0
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### readelf --wide --decompress --hex-dump=.group {}

```diff
@@ -1,8 +1,16 @@
 
 Hex dump of section '.group':
-  0x00000000 01000000 0c000000                   ........
+  0x00000000 01000000 0e000000                   ........
 
 
 Hex dump of section '.group':
-  0x00000000 01000000 0d000000 0e000000          ............
+  0x00000000 01000000 0f000000                   ........
+
+
+Hex dump of section '.group':
+  0x00000000 01000000 10000000                   ........
+
+
+Hex dump of section '.group':
+  0x00000000 01000000 11000000 12000000          ............
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1904,36 +1904,84 @@
  R_X86_64_PC32	.text.unlikely+0x250
 	nop
 	nopl   0x0(%rax,%rax,1)
 
 0000000000001aa0 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)>:
 basic_math_operations::BMONum::operator==(basic_math_operations::BMONum):
 	endbr64
-	mov    0x8(%rdi),%rdx
+	push   %r13
+	lea    0x0(%rip),%r13        
+ R_X86_64_PC32	.LC1-0x4
+	push   %r12
+	lea    0x0(%rip),%r12        
+ R_X86_64_PC32	.LC12-0x4
+	push   %rbp
+	mov    %rsi,%rbp
+	mov    %r13,%rsi
+	push   %rbx
+	mov    %rdi,%rbx
+	sub    $0x8,%rsp
+	call   1aca <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x2a>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
+	test   %eax,%eax
+	jne    1add <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x3d>
+	mov    %r12,%rsi
+	mov    %rbp,%rdi
+	call   1ad9 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x39>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
+	test   %eax,%eax
+	je     1b3f <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x9f>
+	mov    %r12,%rsi
+	mov    %rbx,%rdi
+	call   1ae8 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x48>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
+	test   %eax,%eax
+	je     1b30 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x90>
+	mov    0x8(%rbx),%rdx
 	xor    %eax,%eax
-	cmp    0x8(%rsi),%rdx
-	je     1ab8 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x18>
+	cmp    0x8(%rbp),%rdx
+	je     1b08 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x68>
+	add    $0x8,%rsp
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
 	ret
-	nopl   0x0(%rax)
-	mov    $0x1,%eax
+	nopl   0x0(%rax,%rax,1)
+	mov    (%rbx),%rdi
+	mov    0x0(%rbp),%rsi
 	test   %rdx,%rdx
-	je     1ab0 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x10>
-	sub    $0x8,%rsp
-	mov    (%rsi),%rsi
-	mov    (%rdi),%rdi
-	call   1ad1 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x31>
+	je     1b3f <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x9f>
+	call   1b19 <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x79>
  R_X86_64_PLT32	memcmp-0x4
 	test   %eax,%eax
 	sete   %al
 	add    $0x8,%rsp
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
 	ret
-	nop
 	nopl   0x0(%rax)
+	mov    %r13,%rsi
+	mov    %rbp,%rdi
+	call   1b3b <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x9b>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::compare(char const*) const-0x4
+	test   %eax,%eax
+	jne    1aec <basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)+0x4c>
+	add    $0x8,%rsp
+	mov    $0x1,%eax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	ret
+	nop
 
-0000000000001ae0 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)>:
+0000000000001b50 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)>:
 basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum):
 	endbr64
 	push   %r15
 	push   %r14
 	push   %r13
 	mov    %rdi,%r13
 	push   %r12
@@ -1946,160 +1994,721 @@
 	mov    %fs:0x28,%rax
 	mov    %rax,0x58(%rsp)
 	xor    %eax,%eax
 	lea    0x20(%rsp),%rbp
 	mov    %r14,%rax
 	mov    %rbp,0x10(%rsp)
 	add    %r12,%rax
-	je     1b2a <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x4a>
+	je     1b9a <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x4a>
 	test   %r14,%r14
-	je     1ce8 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x208>
+	je     1d58 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x208>
 	mov    %r12,0x8(%rsp)
 	cmp    $0xf,%r12
-	ja     1c50 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x170>
+	ja     1cc0 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x170>
 	cmp    $0x1,%r12
-	jne    1bb0 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xd0>
+	jne    1c20 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xd0>
 	movzbl (%r14),%eax
 	lea    0x10(%rsp),%r15
 	mov    %al,0x20(%rsp)
 	mov    %rbp,%rax
 	mov    %r12,0x18(%rsp)
 	mov    %r15,%rsi
 	mov    %r13,%rdi
 	movb   $0x0,(%rax,%r12,1)
-	call   1b64 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x84>
+	call   1bd4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x84>
  R_X86_64_PLT32	basic_math_operations::BMONum::operator>(basic_math_operations::BMONum)-0x4
 	mov    %eax,%r12d
 	test   %al,%al
-	je     1bc8 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xe8>
+	je     1c38 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xe8>
 	mov    0x10(%rsp),%rdi
 	cmp    %rbp,%rdi
-	je     1b83 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xa3>
+	je     1bf3 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xa3>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1b83 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xa3>
+	call   1bf3 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0xa3>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    0x58(%rsp),%rax
 	sub    %fs:0x28,%rax
-	jne    1cf4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x214>
+	jne    1d64 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x214>
 	add    $0x68,%rsp
 	mov    %r12d,%eax
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	nopl   0x0(%rax)
 	test   %r12,%r12
-	jne    1cf9 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x219>
+	jne    1d69 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x219>
 	mov    %rbp,%rax
 	lea    0x10(%rsp),%r15
-	jmp    1b4f <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x6f>
+	jmp    1bbf <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x6f>
 	nopl   0x0(%rax,%rax,1)
 	mov    (%rbx),%r15
 	mov    0x8(%rbx),%r12
 	lea    0x40(%rsp),%r14
 	mov    %r14,0x30(%rsp)
 	mov    %r15,%rax
 	add    %r12,%rax
-	je     1bea <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x10a>
+	je     1c5a <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x10a>
 	test   %r15,%r15
-	je     1d10 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x230>
+	je     1d80 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x230>
 	mov    %r12,0x8(%rsp)
 	cmp    $0xf,%r12
-	ja     1ca8 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1c8>
+	ja     1d18 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1c8>
 	cmp    $0x1,%r12
-	jne    1c90 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1b0>
+	jne    1d00 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1b0>
 	movzbl (%r15),%eax
 	lea    0x30(%rsp),%rbx
 	mov    %al,0x40(%rsp)
 	mov    %r14,%rax
 	mov    %r12,0x38(%rsp)
 	mov    %rbx,%rsi
 	mov    %r13,%rdi
 	movb   $0x0,(%rax,%r12,1)
-	call   1c28 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x148>
+	call   1c98 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x148>
  R_X86_64_PLT32	basic_math_operations::BMONum::operator==(basic_math_operations::BMONum)-0x4
 	mov    0x30(%rsp),%rdi
 	mov    %eax,%r12d
 	cmp    %r14,%rdi
-	je     1b6b <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x8b>
+	je     1bdb <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x8b>
 	mov    0x40(%rsp),%rax
 	lea    0x1(%rax),%rsi
-	call   1c47 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x167>
+	call   1cb7 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x167>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
-	jmp    1b6b <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x8b>
+	jmp    1bdb <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x8b>
 	nopl   0x0(%rax)
 	lea    0x10(%rsp),%r15
 	lea    0x8(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %r15,%rdi
-	call   1c64 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x184>
+	call   1cd4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x184>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x10(%rsp)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x20(%rsp)
 	mov    %r12,%rdx
 	mov    %r14,%rsi
-	call   1c81 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1a1>
+	call   1cf1 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1a1>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r12
 	mov    0x10(%rsp),%rax
-	jmp    1b4f <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x6f>
+	jmp    1bbf <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x6f>
 	test   %r12,%r12
-	jne    1d06 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x226>
+	jne    1d76 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x226>
 	mov    %r14,%rax
 	lea    0x30(%rsp),%rbx
-	jmp    1c13 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x133>
+	jmp    1c83 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x133>
 	nopw   0x0(%rax,%rax,1)
 	lea    0x30(%rsp),%rbx
 	lea    0x8(%rsp),%rsi
 	xor    %edx,%edx
 	mov    %rbx,%rdi
-	call   1cbc <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1dc>
+	call   1d2c <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1dc>
  R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
 	mov    %rax,0x30(%rsp)
 	mov    %rax,%rdi
 	mov    0x8(%rsp),%rax
 	mov    %rax,0x40(%rsp)
 	mov    %r12,%rdx
 	mov    %r15,%rsi
-	call   1cd9 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1f9>
+	call   1d49 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1f9>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x8(%rsp),%r12
 	mov    0x30(%rsp),%rax
-	jmp    1c13 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x133>
-	lea    0x0(%rip),%rdi        # 1cef <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x20f>
+	jmp    1c83 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x133>
+	lea    0x0(%rip),%rdi        # 1d5f <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x20f>
  R_X86_64_PC32	.LC0-0x4
-	call   1cf4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x214>
+	call   1d64 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x214>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
-	call   1cf9 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x219>
+	call   1d69 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x219>
  R_X86_64_PLT32	__stack_chk_fail-0x4
 	mov    %rbp,%rdi
 	lea    0x10(%rsp),%r15
-	jmp    1c76 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x196>
+	jmp    1ce6 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x196>
 	mov    %r14,%rdi
 	lea    0x30(%rsp),%rbx
-	jmp    1cce <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1ee>
-	lea    0x0(%rip),%rdi        # 1d17 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x237>
+	jmp    1d3e <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x1ee>
+	lea    0x0(%rip),%rdi        # 1d87 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x237>
  R_X86_64_PC32	.LC0-0x4
-	call   1d1c <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x23c>
+	call   1d8c <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x23c>
  R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
 	endbr64
 	mov    %rax,%r12
-	jmp    1d28 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x248>
+	jmp    1d98 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x248>
  R_X86_64_PC32	.text.unlikely+0x270
 	endbr64
 	mov    %rax,%r12
-	jmp    1d34 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x254>
+	jmp    1da4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x254>
  R_X86_64_PC32	.text.unlikely+0x2a0
 	endbr64
 	mov    %rax,%r12
-	jmp    1d40 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x260>
+	jmp    1db0 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x260>
  R_X86_64_PC32	.text.unlikely+0x288
 	endbr64
 	mov    %rax,%r12
-	jmp    1d4c <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x26c>
+	jmp    1dbc <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum)+0x26c>
  R_X86_64_PC32	.text.unlikely+0x288
+	nopl   0x0(%rax)
+
+0000000000001dc0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]>:
+int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]:
+	push   %r15
+	movslq %esi,%rax
+	push   %r14
+	push   %r13
+	movslq %edx,%r13
+	push   %r12
+	sub    %rax,%r13
+	mov    %rdi,%r12
+	push   %rbp
+	mov    %rax,%rbp
+	mov    $0xfffffffe,%eax
+	push   %rbx
+	sub    $0x8,%rsp
+	cmp    %rax,%r13
+	jbe    1ea8 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0xe8>
+	mov    $0xffffffff,%eax
+	cmp    %rax,%r13
+	je     1fb0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1f0>
+	mov    $0xffffffff,%edx
+	xor    %esi,%esi
+	mov    %r12,%rdi
+	call   1dc0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]>
+	mov    %rax,%rbx
+	mov    0x1380(%r12),%rax
+	shl    $0x20,%rbx
+	cmp    $0x26f,%rax
+	jbe    1e2f <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x6f>
+	mov    %r12,%rdi
+	call   1e27 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x67>
+ R_X86_64_PLT32	std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>::_M_gen_rand()-0x4
+	mov    0x1380(%r12),%rax
+	lea    0x1(%rax),%rdx
+	mov    (%r12,%rax,8),%rax
+	mov    %rdx,0x1380(%r12)
+	mov    %rax,%rdx
+	shr    $0xb,%rdx
+	mov    %edx,%edx
+	xor    %rdx,%rax
+	mov    %rax,%rdx
+	shl    $0x7,%rdx
+	and    $0x9d2c5680,%edx
+	xor    %rdx,%rax
+	mov    %rax,%rdx
+	shl    $0xf,%rdx
+	and    $0xefc60000,%edx
+	xor    %rdx,%rax
+	mov    %rax,%rdx
+	shr    $0x12,%rdx
+	xor    %rdx,%rax
+	add    %rax,%rbx
+	setb   %al
+	movzbl %al,%eax
+	cmp    %rbx,%r13
+	jb     1df9 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x39>
+	test   %rax,%rax
+	jne    1df9 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x39>
+	add    $0x8,%rsp
+	lea    0x0(%rbp,%rbx,1),%eax
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	pop    %r15
+	ret
+	nopl   0x0(%rax,%rax,1)
+	mov    0x1380(%rdi),%rax
+	add    $0x1,%r13
+	mov    %r13d,%r15d
+	cmp    $0x26f,%rax
+	ja     2010 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x250>
+	mov    (%r12,%rax,8),%rbx
+	lea    0x1(%rax),%rcx
+	mov    %rcx,0x1380(%r12)
+	mov    %rbx,%rax
+	shr    $0xb,%rax
+	mov    %eax,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shl    $0x7,%rax
+	and    $0x9d2c5680,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shl    $0xf,%rax
+	and    $0xefc60000,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shr    $0x12,%rax
+	xor    %rax,%rbx
+	imul   %r13,%rbx
+	cmp    %ebx,%r13d
+	jbe    1fa0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1e0>
+	mov    %r13d,%eax
+	xor    %edx,%edx
+	neg    %eax
+	div    %r15d
+	mov    %edx,%r14d
+	cmp    %edx,%ebx
+	jb     1f7d <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1bd>
+	jmp    1fa0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1e0>
+	cs nopw 0x0(%rax,%rax,1)
+	mov    (%r12,%rax,8),%rbx
+	lea    0x1(%rax),%rcx
+	mov    %rcx,0x1380(%r12)
+	mov    %rbx,%rax
+	shr    $0xb,%rax
+	mov    %eax,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shl    $0x7,%rax
+	and    $0x9d2c5680,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shl    $0xf,%rax
+	and    $0xefc60000,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shr    $0x12,%rax
+	xor    %rax,%rbx
+	imul   %r13,%rbx
+	cmp    %ebx,%r14d
+	jbe    1fa0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1e0>
+	mov    %rcx,%rax
+	cmp    $0x26f,%rcx
+	jbe    1f30 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x170>
+	mov    %r12,%rdi
+	call   1f91 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1d1>
+ R_X86_64_PLT32	std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>::_M_gen_rand()-0x4
+	mov    0x1380(%r12),%rax
+	jmp    1f30 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x170>
+	nopl   0x0(%rax,%rax,1)
+	shr    $0x20,%rbx
+	jmp    1e90 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0xd0>
+	nopl   0x0(%rax)
+	mov    0x1380(%rdi),%rax
+	cmp    $0x26f,%rax
+	ja     2028 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x268>
+	mov    (%r12,%rax,8),%rbx
+	lea    0x1(%rax),%rdx
+	mov    %rdx,0x1380(%r12)
+	mov    %rbx,%rax
+	shr    $0xb,%rax
+	mov    %eax,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shl    $0x7,%rax
+	and    $0x9d2c5680,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shl    $0xf,%rax
+	and    $0xefc60000,%eax
+	xor    %rax,%rbx
+	mov    %rbx,%rax
+	shr    $0x12,%rax
+	xor    %rax,%rbx
+	jmp    1e90 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0xd0>
+	nopl   0x0(%rax,%rax,1)
+	call   2015 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x255>
+ R_X86_64_PLT32	std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>::_M_gen_rand()-0x4
+	mov    0x1380(%r12),%rax
+	jmp    1ec2 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x102>
+	nopw   0x0(%rax,%rax,1)
+	call   202d <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x26d>
+ R_X86_64_PLT32	std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>::_M_gen_rand()-0x4
+	mov    0x1380(%r12),%rax
+	jmp    1fbf <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]+0x1ff>
+	nopw   0x0(%rax,%rax,1)
+
+0000000000002040 <basic_math_operations::random(unsigned long long)>:
+basic_math_operations::random(unsigned long long):
+	endbr64
+	push   %r15
+	push   %r14
+	push   %r13
+	push   %r12
+	push   %rbp
+	push   %rbx
+	sub    $0x1000,%rsp
+	orq    $0x0,(%rsp)
+	sub    $0x1000,%rsp
+	orq    $0x0,(%rsp)
+	sub    $0x7a8,%rsp
+	mov    %rdi,0x20(%rsp)
+	lea    0x1410(%rsp),%r13
+	lea    0x1420(%rsp),%rbx
+	mov    %rsi,0x10(%rsp)
+	mov    %r13,%rsi
+	mov    %fs:0x28,%rax
+	mov    %rax,0x2798(%rsp)
+	xor    %eax,%eax
+	mov    $0x6c75,%eax
+	mov    %rbx,0x1410(%rsp)
+	mov    %ax,0x1424(%rsp)
+	lea    0x80(%rsp),%rax
+	mov    %rax,%rdi
+	movl   $0x61666564,0x1420(%rsp)
+	movb   $0x74,0x1426(%rsp)
+	movq   $0x7,0x1418(%rsp)
+	movb   $0x0,0x1427(%rsp)
+	mov    %rax,0x18(%rsp)
+	call   20ee <basic_math_operations::random(unsigned long long)+0xae>
+ R_X86_64_PLT32	std::random_device::_M_init(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> > const&)-0x4
+	mov    0x1410(%rsp),%rdi
+	cmp    %rbx,%rdi
+	je     210c <basic_math_operations::random(unsigned long long)+0xcc>
+	mov    0x1420(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   210c <basic_math_operations::random(unsigned long long)+0xcc>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    0x18(%rsp),%rdi
+	call   2116 <basic_math_operations::random(unsigned long long)+0xd6>
+ R_X86_64_PLT32	std::random_device::_M_getval()-0x4
+	mov    %eax,%eax
+	mov    $0x1,%ecx
+	mov    %rax,0x1410(%rsp)
+	mov    %rax,%rdx
+	nopl   0x0(%rax,%rax,1)
+	mov    %rdx,%rax
+	shr    $0x1e,%rax
+	xor    %rdx,%rax
+	imul   $0x6c078965,%rax,%rax
+	lea    (%rax,%rcx,1),%edx
+	mov    %rdx,0x0(%r13,%rcx,8)
+	add    $0x1,%rcx
+	cmp    $0x270,%rcx
+	jne    2130 <basic_math_operations::random(unsigned long long)+0xf0>
+	lea    0x50(%rsp),%rax
+	xor    %r15d,%r15d
+	cmpq   $0x0,0x10(%rsp)
+	movq   $0x270,0x2790(%rsp)
+	mov    %rax,0x28(%rsp)
+	movabs $0x346dc5d63886594b,%r14
+	mov    %rax,0x40(%rsp)
+	lea    0x60(%rsp),%rax
+	mov    %rax,0x8(%rsp)
+	lea    0x70(%rsp),%rax
+	movq   $0x0,0x48(%rsp)
+	movb   $0x0,0x50(%rsp)
+	mov    %rax,(%rsp)
+	je     2312 <basic_math_operations::random(unsigned long long)+0x2d2>
+	nopl   0x0(%rax,%rax,1)
+	xor    %esi,%esi
+	mov    $0x9,%edx
+	mov    %r13,%rdi
+	call   1dc0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]>
+	mov    %eax,%r12d
+	mov    %eax,%ebp
+	shr    $0x1f,%r12d
+	neg    %ebp
+	cmovs  %eax,%ebp
+	cmp    $0x9,%ebp
+	jbe    25a3 <basic_math_operations::random(unsigned long long)+0x563>
+	cmp    $0x63,%ebp
+	jbe    2599 <basic_math_operations::random(unsigned long long)+0x559>
+	cmp    $0x3e7,%ebp
+	jbe    25ad <basic_math_operations::random(unsigned long long)+0x56d>
+	mov    %ebp,%edx
+	cmp    $0x270f,%ebp
+	jbe    25b7 <basic_math_operations::random(unsigned long long)+0x577>
+	mov    $0x1,%ebx
+	jmp    2221 <basic_math_operations::random(unsigned long long)+0x1e1>
+	cmp    $0x63,%edx
+	jbe    2510 <basic_math_operations::random(unsigned long long)+0x4d0>
+	cmp    $0x3e7,%edx
+	jbe    2520 <basic_math_operations::random(unsigned long long)+0x4e0>
+	cmp    $0x270f,%edx
+	jbe    2530 <basic_math_operations::random(unsigned long long)+0x4f0>
+	mov    %rdx,%rax
+	mov    %rdx,%rcx
+	mul    %r14
+	mov    %ebx,%eax
+	add    $0x4,%ebx
+	shr    $0xb,%rdx
+	cmp    $0x1869f,%rcx
+	ja     2200 <basic_math_operations::random(unsigned long long)+0x1c0>
+	mov    (%rsp),%rax
+	mov    0x8(%rsp),%rdi
+	lea    (%r12,%rbx,1),%esi
+	mov    $0x2d,%edx
+	mov    %rax,0x60(%rsp)
+	call   2258 <basic_math_operations::random(unsigned long long)+0x218>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_construct(unsigned long, char)-0x4
+	movzbl %r12b,%r12d
+	sub    $0x1,%ebx
+	add    0x60(%rsp),%r12
+	cmp    $0x63,%ebp
+	jbe    22ad <basic_math_operations::random(unsigned long long)+0x26d>
+	mov    0x0(%rip),%rcx        
+ R_X86_64_REX_GOTPCRELX	std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits-0x4
+	mov    %ebp,%edx
+	mov    %ebp,%eax
+	imul   $0x51eb851f,%rdx,%rdx
+	shr    $0x25,%rdx
+	imul   $0x64,%edx,%esi
+	sub    %esi,%eax
+	mov    %ebp,%esi
+	mov    %edx,%ebp
+	mov    %ebx,%edx
+	add    %eax,%eax
+	lea    0x1(%rax),%edi
+	movzbl (%rcx,%rax,1),%eax
+	movzbl (%rcx,%rdi,1),%edi
+	mov    %dil,(%r12,%rdx,1)
+	lea    -0x1(%rbx),%edx
+	sub    $0x2,%ebx
+	mov    %al,(%r12,%rdx,1)
+	cmp    $0x270f,%esi
+	ja     2270 <basic_math_operations::random(unsigned long long)+0x230>
+	lea    0x30(%rbp),%eax
+	cmp    $0x9,%ebp
+	jbe    22ce <basic_math_operations::random(unsigned long long)+0x28e>
+	mov    0x0(%rip),%rcx        
+ R_X86_64_REX_GOTPCRELX	std::__detail::__to_chars_10_impl<unsigned int>(char*, unsigned int, unsigned int)::__digits-0x4
+	add    %ebp,%ebp
+	lea    0x1(%rbp),%eax
+	movzbl (%rcx,%rax,1),%eax
+	mov    %al,0x1(%r12)
+	movzbl (%rcx,%rbp,1),%eax
+	mov    %al,(%r12)
+	mov    0x68(%rsp),%rdx
+	lea    0x40(%rsp),%rdi
+	mov    0x60(%rsp),%rsi
+	call   22e6 <basic_math_operations::random(unsigned long long)+0x2a6>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x60(%rsp),%rdi
+	cmp    (%rsp),%rdi
+	je     24f8 <basic_math_operations::random(unsigned long long)+0x4b8>
+	mov    0x70(%rsp),%rax
+	add    $0x1,%r15
+	lea    0x1(%rax),%rsi
+	call   2307 <basic_math_operations::random(unsigned long long)+0x2c7>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	cmp    %r15,0x10(%rsp)
+	jne    21b0 <basic_math_operations::random(unsigned long long)+0x170>
+	xor    %esi,%esi
+	mov    $0x9,%edx
+	mov    %r13,%rdi
+	call   1dc0 <int std::uniform_int_distribution<int>::operator()<std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul> >(std::mersenne_twister_engine<unsigned long, 32ul, 624ul, 397ul, 31ul, 2567483615ul, 11ul, 4294967295ul, 7ul, 2636928640ul, 15ul, 4022730752ul, 18ul, 1812433253ul>&, std::uniform_int_distribution<int>::param_type const&) [clone .isra.0]>
+	test   $0x1,%al
+	jne    241b <basic_math_operations::random(unsigned long long)+0x3db>
+	mov    (%rsp),%rax
+	lea    0x60(%rsp),%rdi
+	movb   $0x0,0x70(%rsp)
+	mov    %rdi,0x8(%rsp)
+	mov    %rax,0x60(%rsp)
+	mov    0x48(%rsp),%rax
+	movq   $0x0,0x68(%rsp)
+	lea    0x1(%rax),%rsi
+	call   2358 <basic_math_operations::random(unsigned long long)+0x318>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::reserve(unsigned long)-0x4
+	movabs $0x3fffffffffffffff,%rax
+	cmp    %rax,0x68(%rsp)
+	je     263c <basic_math_operations::random(unsigned long long)+0x5fc>
+	mov    0x8(%rsp),%rbx
+	mov    $0x1,%edx
+	lea    0x0(%rip),%rsi        
+ R_X86_64_PC32	.LC15-0x4
+	mov    %rbx,%rdi
+	call   2386 <basic_math_operations::random(unsigned long long)+0x346>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x48(%rsp),%rdx
+	mov    0x40(%rsp),%rsi
+	mov    %rbx,%rdi
+	call   2398 <basic_math_operations::random(unsigned long long)+0x358>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_append(char const*, unsigned long)-0x4
+	mov    0x40(%rsp),%rdi
+	mov    0x60(%rsp),%rax
+	mov    0x68(%rsp),%rdx
+	cmp    (%rsp),%rax
+	je     25c1 <basic_math_operations::random(unsigned long long)+0x581>
+	mov    0x70(%rsp),%rcx
+	movq   %rdx,%xmm0
+	movq   %rcx,%xmm1
+	punpcklqdq %xmm1,%xmm0
+	cmp    0x28(%rsp),%rdi
+	je     25f2 <basic_math_operations::random(unsigned long long)+0x5b2>
+	mov    0x50(%rsp),%rsi
+	mov    %rax,0x40(%rsp)
+	mov    %rdx,0x48(%rsp)
+	mov    %rcx,0x50(%rsp)
+	test   %rdi,%rdi
+	je     25fc <basic_math_operations::random(unsigned long long)+0x5bc>
+	mov    %rdi,0x60(%rsp)
+	mov    %rsi,0x70(%rsp)
+	movq   $0x0,0x68(%rsp)
+	movb   $0x0,(%rdi)
+	mov    0x60(%rsp),%rdi
+	cmp    (%rsp),%rdi
+	je     241b <basic_math_operations::random(unsigned long long)+0x3db>
+	mov    0x70(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   241b <basic_math_operations::random(unsigned long long)+0x3db>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    (%rsp),%rax
+	mov    0x40(%rsp),%rbp
+	mov    0x48(%rsp),%r12
+	mov    %rax,0x60(%rsp)
+	mov    %rbp,%rax
+	add    %r12,%rax
+	je     243f <basic_math_operations::random(unsigned long long)+0x3ff>
+	test   %rbp,%rbp
+	je     2648 <basic_math_operations::random(unsigned long long)+0x608>
+	mov    %r12,0x38(%rsp)
+	cmp    $0xf,%r12
+	ja     2554 <basic_math_operations::random(unsigned long long)+0x514>
+	cmp    $0x1,%r12
+	jne    2538 <basic_math_operations::random(unsigned long long)+0x4f8>
+	movzbl 0x0(%rbp),%eax
+	lea    0x60(%rsp),%rsi
+	mov    %rsi,0x8(%rsp)
+	mov    %al,0x70(%rsp)
+	mov    (%rsp),%rax
+	mov    0x8(%rsp),%rsi
+	mov    0x20(%rsp),%rdi
+	mov    %r12,0x68(%rsp)
+	movb   $0x0,(%rax,%r12,1)
+	call   2487 <basic_math_operations::random(unsigned long long)+0x447>
+ R_X86_64_PLT32	basic_math_operations::BMONum::BMONum(std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >)-0x4
+	mov    0x60(%rsp),%rdi
+	cmp    (%rsp),%rdi
+	je     24a0 <basic_math_operations::random(unsigned long long)+0x460>
+	mov    0x70(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   24a0 <basic_math_operations::random(unsigned long long)+0x460>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    0x40(%rsp),%rdi
+	cmp    0x28(%rsp),%rdi
+	je     24ba <basic_math_operations::random(unsigned long long)+0x47a>
+	mov    0x50(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   24ba <basic_math_operations::random(unsigned long long)+0x47a>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    0x18(%rsp),%rdi
+	call   24c4 <basic_math_operations::random(unsigned long long)+0x484>
+ R_X86_64_PLT32	std::random_device::_M_fini()-0x4
+	mov    0x2798(%rsp),%rax
+	sub    %fs:0x28,%rax
+	jne    2654 <basic_math_operations::random(unsigned long long)+0x614>
+	mov    0x20(%rsp),%rax
+	add    $0x27a8,%rsp
+	pop    %rbx
+	pop    %rbp
+	pop    %r12
+	pop    %r13
+	pop    %r14
+	pop    %r15
+	ret
+	nopw   0x0(%rax,%rax,1)
+	add    $0x1,%r15
+	cmp    %r15,0x10(%rsp)
+	jne    21b0 <basic_math_operations::random(unsigned long long)+0x170>
+	jmp    2312 <basic_math_operations::random(unsigned long long)+0x2d2>
+	nopl   0x0(%rax)
+	lea    0x5(%rax),%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	nopl   0x0(%rax,%rax,1)
+	lea    0x6(%rax),%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	nopl   0x0(%rax,%rax,1)
+	lea    0x7(%rax),%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	test   %r12,%r12
+	jne    2629 <basic_math_operations::random(unsigned long long)+0x5e9>
+	lea    0x60(%rsp),%rsi
+	mov    (%rsp),%rax
+	mov    %rsi,0x8(%rsp)
+	jmp    246e <basic_math_operations::random(unsigned long long)+0x42e>
+	lea    0x60(%rsp),%rax
+	lea    0x38(%rsp),%rsi
+	xor    %edx,%edx
+	mov    %rax,%rdi
+	mov    %rax,0x8(%rsp)
+	call   256d <basic_math_operations::random(unsigned long long)+0x52d>
+ R_X86_64_PLT32	std::__cxx11::basic_string<char, std::char_traits<char>, std::allocator<char> >::_M_create(unsigned long&, unsigned long)-0x4
+	mov    %rax,0x60(%rsp)
+	mov    %rax,%rdi
+	mov    0x38(%rsp),%rax
+	mov    %rax,0x70(%rsp)
+	mov    %r12,%rdx
+	mov    %rbp,%rsi
+	call   258a <basic_math_operations::random(unsigned long long)+0x54a>
+ R_X86_64_PLT32	memcpy-0x4
+	mov    0x38(%rsp),%r12
+	mov    0x60(%rsp),%rax
+	jmp    246e <basic_math_operations::random(unsigned long long)+0x42e>
+	mov    $0x2,%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	mov    $0x1,%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	mov    $0x3,%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	mov    $0x4,%ebx
+	jmp    223c <basic_math_operations::random(unsigned long long)+0x1fc>
+	test   %rdx,%rdx
+	je     25df <basic_math_operations::random(unsigned long long)+0x59f>
+	cmp    $0x1,%rdx
+	je     2616 <basic_math_operations::random(unsigned long long)+0x5d6>
+	mov    (%rsp),%rsi
+	call   25d5 <basic_math_operations::random(unsigned long long)+0x595>
+ R_X86_64_PLT32	memcpy-0x4
+	mov    0x68(%rsp),%rdx
+	mov    0x40(%rsp),%rdi
+	mov    %rdx,0x48(%rsp)
+	movb   $0x0,(%rdi,%rdx,1)
+	mov    0x60(%rsp),%rdi
+	jmp    23f6 <basic_math_operations::random(unsigned long long)+0x3b6>
+	mov    %rax,0x40(%rsp)
+	movups %xmm0,0x48(%rsp)
+	mov    (%rsp),%rax
+	mov    %rax,0x60(%rsp)
+	lea    0x70(%rsp),%rax
+	mov    %rax,(%rsp)
+	mov    %rax,%rdi
+	jmp    23f6 <basic_math_operations::random(unsigned long long)+0x3b6>
+	movzbl 0x70(%rsp),%eax
+	mov    %al,(%rdi)
+	mov    0x68(%rsp),%rdx
+	mov    0x40(%rsp),%rdi
+	jmp    25df <basic_math_operations::random(unsigned long long)+0x59f>
+	lea    0x60(%rsp),%rax
+	mov    (%rsp),%rdi
+	mov    %rax,0x8(%rsp)
+	jmp    257f <basic_math_operations::random(unsigned long long)+0x53f>
+	lea    0x0(%rip),%rdi        
+ R_X86_64_PC32	.LC14-0x4
+	call   2648 <basic_math_operations::random(unsigned long long)+0x608>
+ R_X86_64_PLT32	std::__throw_length_error(char const*)-0x4
+	lea    0x0(%rip),%rdi        
+ R_X86_64_PC32	.LC0-0x4
+	call   2654 <basic_math_operations::random(unsigned long long)+0x614>
+ R_X86_64_PLT32	std::__throw_logic_error(char const*)-0x4
+	call   2659 <basic_math_operations::random(unsigned long long)+0x619>
+ R_X86_64_PLT32	__stack_chk_fail-0x4
+	endbr64
+	mov    %rax,%rbx
+	jmp    2665 <basic_math_operations::random(unsigned long long)+0x625>
+ R_X86_64_PC32	.text.unlikely+0x2c1
+	endbr64
+	mov    %rax,%rbx
+	jmp    2671 <basic_math_operations::random(unsigned long long)+0x631>
+ R_X86_64_PC32	.text.unlikely+0x2a8
+	endbr64
+	mov    %rax,%rbx
+	jmp    267d <basic_math_operations::random(unsigned long long)+0x63d>
+ R_X86_64_PC32	.text.unlikely+0x2ed
+	endbr64
+	mov    %rax,%rbx
+	jmp    2689 <basic_math_operations::random(unsigned long long)+0x649>
+ R_X86_64_PC32	.text.unlikely+0x308
+	endbr64
+	mov    %rax,%rbp
+	jmp    2695 <basic_math_operations::random(unsigned long long)+0x655>
+ R_X86_64_PC32	.text.unlikely+0x323
+	endbr64
+	mov    %rax,%rbx
+	jmp    26a1 <basic_math_operations::random(unsigned long long)+0x661>
+ R_X86_64_PC32	.text.unlikely+0x2db
```

##### readelf --wide --decompress --string-dump=.rodata.str1.1 {}

```diff
@@ -1,4 +1,7 @@
 
 String dump of section '.rodata.str1.1':
   [     0]  0
+  [     2]  -0
+  [     5]  basic_string::append
+  [    1a]  -
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text.unlikely {}

```diff
@@ -246,9 +246,58 @@
 	cmp    %rbp,%rdi
 	je     2a4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum) [clone .cold]+0x30>
 	mov    0x20(%rsp),%rax
 	lea    0x1(%rax),%rsi
 	call   2a4 <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum) [clone .cold]+0x30>
  R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
 	mov    %r12,%rdi
-	call   2ac <basic_math_operations::BMONum::operator>=(basic_math_operations::BMONum) [clone .cold]+0x38>
+	call   2ac <basic_math_operations::random(unsigned long long) [clone .cold]>
+ R_X86_64_PLT32	_Unwind_Resume-0x4
+
+00000000000002ac <basic_math_operations::random(unsigned long long) [clone .cold]>:
+basic_math_operations::random(unsigned long long) [clone .cold]:
+	mov    0x60(%rsp),%rdi
+	cmp    (%rsp),%rdi
+	je     2c5 <basic_math_operations::random(unsigned long long) [clone .cold]+0x19>
+	mov    0x70(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   2c5 <basic_math_operations::random(unsigned long long) [clone .cold]+0x19>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    0x40(%rsp),%rdi
+	cmp    0x28(%rsp),%rdi
+	je     2df <basic_math_operations::random(unsigned long long) [clone .cold]+0x33>
+	mov    0x50(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   2df <basic_math_operations::random(unsigned long long) [clone .cold]+0x33>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    0x18(%rsp),%rdi
+	call   2e9 <basic_math_operations::random(unsigned long long) [clone .cold]+0x3d>
+ R_X86_64_PLT32	std::random_device::_M_fini()-0x4
+	mov    %rbx,%rdi
+	call   2f1 <basic_math_operations::random(unsigned long long) [clone .cold]+0x45>
+ R_X86_64_PLT32	_Unwind_Resume-0x4
+	mov    0x60(%rsp),%rdi
+	cmp    (%rsp),%rdi
+	je     2c5 <basic_math_operations::random(unsigned long long) [clone .cold]+0x19>
+	mov    0x70(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   30a <basic_math_operations::random(unsigned long long) [clone .cold]+0x5e>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	jmp    2c5 <basic_math_operations::random(unsigned long long) [clone .cold]+0x19>
+	mov    0x60(%rsp),%rdi
+	cmp    (%rsp),%rdi
+	je     2c5 <basic_math_operations::random(unsigned long long) [clone .cold]+0x19>
+	mov    0x70(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   325 <basic_math_operations::random(unsigned long long) [clone .cold]+0x79>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	jmp    2c5 <basic_math_operations::random(unsigned long long) [clone .cold]+0x19>
+	mov    0x1410(%rsp),%rdi
+	cmp    %rbx,%rdi
+	je     345 <basic_math_operations::random(unsigned long long) [clone .cold]+0x99>
+	mov    0x1420(%rsp),%rax
+	lea    0x1(%rax),%rsi
+	call   345 <basic_math_operations::random(unsigned long long) [clone .cold]+0x99>
+ R_X86_64_PLT32	operator delete(void*, unsigned long)-0x4
+	mov    %rbp,%rdi
+	call   34d <basic_math_operations::random(unsigned long long) [clone .cold]+0xa1>
  R_X86_64_PLT32	_Unwind_Resume-0x4
```

##### readelf --wide --decompress --hex-dump=.gcc_except_table {}

```diff
@@ -20,9 +20,13 @@
   0x00000110 01044405 0000ffff 011cdb01 05cb0400 ..D.............
   0x00000120 9c030500 00df0305 bf040097 04050000 ................
   0x00000130 a80405bf 0400ffff 01043305 0000ffff ..........3.....
   0x00000140 010a7a05 ab0200df 013d0000 ffff0104 ..z......=......
   0x00000150 1b050000 ffff0123 7f05e004 00c30205 .......#........
   0x00000160 bc0400ff 0205c804 00d70305 d404008f ................
   0x00000170 0405c804 00b70405 d40400ff ff010433 ...............3
-  0x00000180 050000                              ...
+  0x00000180 050000ff ff0136a9 0105c90c 00d10105 ......6.........
+  0x00000190 d50c0093 0405990c 00a10505 b10c0093 ................
+  0x000001a0 0645a50c 00c20805 bd0c00a8 0a05990c .E..............
+  0x000001b0 00830c05 a50c008f 0c05990c 00ffff01 ................
+  0x000001c0 04406100 00                         .@a..
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -89,17 +89,35 @@
   0x00000550 8e038f02 44000000 e4030000 00000000 ....D...........
   0x00000560 37010000 04000000 00460e10 8e02450e 7........F....E.
   0x00000570 188d0342 0e208c04 410e2886 05410e30 ...B. ..A.(..A.0
   0x00000580 8306440e 70029b0a 0e30440e 28410e20 ..D.p....0D.(A. 
   0x00000590 420e1842 0e10420e 08470b00 20000000 B..B..B..G.. ...
   0x000005a0 2c040000 00000000 20000000 04000000 ,....... .......
   0x000005b0 000e7083 0686058c 048d038e 02000000 ..p.............
-  0x000005c0 14000000 c4050000 00000000 3b000000 ............;...
-  0x000005d0 00660e10 540e0800 4c000000 68040000 .f..T...L...h...
-  0x000005e0 00000000 6c020000 04000000 00460e10 ....l........F..
-  0x000005f0 8f02420e 188e0342 0e208d04 450e288c ..B....B. ..E.(.
-  0x00000600 05410e30 8606410e 38830747 0ea00102 .A.0..A.8..G....
-  0x00000610 a30a0e38 440e3041 0e28420e 20420e18 ...8D.0A.(B. B..
-  0x00000620 420e1042 0e08480b 24000000 b8040000 B..B..H.$.......
-  0x00000630 00000000 38000000 04000000 000ea001 ....8...........
-  0x00000640 83078606 8c058d04 8e038f02 00000000 ................
+  0x000005c0 58000000 c4050000 00000000 af000000 X...............
+  0x000005d0 00460e10 8d02490e 188c0348 0e208604 .F....I....H. ..
+  0x000005e0 470e2883 05470e30 770a0e28 410e2041 G.(..G.0w..(A. A
+  0x000005f0 0e18420e 10420e08 460b5a0a 0e28410e ..B..B..F.Z..(A.
+  0x00000600 20410e18 420e1042 0e08480b 530e2846  A..B..B..H.S.(F
+  0x00000610 0e20410e 18420e10 420e0800 4c000000 . A..B..B...L...
+  0x00000620 ac040000 00000000 6c020000 04000000 ........l.......
+  0x00000630 00460e10 8f02420e 188e0342 0e208d04 .F....B....B. ..
+  0x00000640 450e288c 05410e30 8606410e 38830747 E.(..A.0..A.8..G
+  0x00000650 0ea00102 a30a0e38 440e3041 0e28420e .......8D.0A.(B.
+  0x00000660 20420e18 420e1042 0e08480b 20000000  B..B..B..H. ...
+  0x00000670 fc040000 00000000 38000000 04000000 ........8.......
+  0x00000680 000ea001 83078606 8c058d04 8e038f02 ................
+  0x00000690 10000000 94060000 00000000 f3000000 ................
+  0x000006a0 00000000 48000000 a8060000 00000000 ....H...........
+  0x000006b0 77020000 00420e10 8f02450e 188e0342 w....B....E....B
+  0x000006c0 0e208d04 450e288c 05470e30 8606490e . ..E.(..G.0..I.
+  0x000006d0 38830744 0e4002b2 0a0e3845 0e30410e 8..D.@....8E.0A.
+  0x000006e0 28420e20 420e1842 0e10420e 08460b00 (B. B..B..B..F..
+  0x000006f0 58000000 80050000 00000000 61060000 X...........a...
+  0x00000700 04000000 00460e10 8f02420e 188e0342 .....F....B....B
+  0x00000710 0e208d04 420e288c 05410e30 8606410e . ..B.(..A.0..A.
+  0x00000720 38830747 0eb8204c 0eb8404c 0ee04f03 8..G.. L..@L..O.
+  0x00000730 7a040a0e 38410e30 410e2842 0e20420e z...8A.0A.(B. B.
+  0x00000740 18420e10 420e0847 0b000000 20000000 .B..B..G.... ...
+  0x00000750 dc050000 00000000 a1000000 04000000 ................
+  0x00000760 000ee04f 83078606 8c058d04 8e038f02 ...O............
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -31,110 +31,170 @@
   0x000001c0 685f6f70 65726174 696f6e73 36424d4f h_operations6BMO
   0x000001d0 4e756d6c 74455330 5f2e636f 6c64005f NumltES0_.cold._
   0x000001e0 5a4e3231 62617369 635f6d61 74685f6f ZN21basic_math_o
   0x000001f0 70657261 74696f6e 7336424d 4f4e756d perations6BMONum
   0x00000200 67744553 305f2e63 6f6c6400 5f5a4e32 gtES0_.cold._ZN2
   0x00000210 31626173 69635f6d 6174685f 6f706572 1basic_math_oper
   0x00000220 6174696f 6e733642 4d4f4e75 6d676545 ations6BMONumgeE
-  0x00000230 53305f2e 636f6c64 002e4c43 30002e4c S0_.cold..LC0..L
-  0x00000240 4331005f 5a4e3231 62617369 635f6d61 C1._ZN21basic_ma
-  0x00000250 74685f6f 70657261 74696f6e 73336164 th_operations3ad
-  0x00000260 64454e53 74375f5f 63787831 31313262 dENSt7__cxx1112b
-  0x00000270 61736963 5f737472 696e6749 63537431 asic_stringIcSt1
-  0x00000280 31636861 725f7472 61697473 49634553 1char_traitsIcES
-  0x00000290 61496345 45455335 5f006361 6c6c6f63 aIcEEES5_.calloc
-  0x000002a0 00616464 00737472 6c656e00 66726565 .add.strlen.free
-  0x000002b0 005f5a4e 5374375f 5f637878 31313132 ._ZNSt7__cxx1112
-  0x000002c0 62617369 635f7374 72696e67 49635374 basic_stringIcSt
-  0x000002d0 31316368 61725f74 72616974 73496345 11char_traitsIcE
-  0x000002e0 53614963 4545395f 4d5f6372 65617465 SaIcEE9_M_create
-  0x000002f0 45526d6d 006d656d 63707900 5f5f7374 ERmm.memcpy.__st
-  0x00000300 61636b5f 63686b5f 6661696c 005f5a53 ack_chk_fail._ZS
-  0x00000310 7431395f 5f746872 6f775f6c 6f676963 t19__throw_logic
-  0x00000320 5f657272 6f72504b 63005f5a 4e323162 _errorPKc._ZN21b
-  0x00000330 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
-  0x00000340 696f6e73 38737562 74726163 74454e53 ions8subtractENS
-  0x00000350 74375f5f 63787831 31313262 61736963 t7__cxx1112basic
-  0x00000360 5f737472 696e6749 63537431 31636861 _stringIcSt11cha
-  0x00000370 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
-  0x00000380 45455335 5f007375 62747261 6374005f EES5_.subtract._
-  0x00000390 5a4e3231 62617369 635f6d61 74685f6f ZN21basic_math_o
-  0x000003a0 70657261 74696f6e 73386d75 6c746970 perations8multip
-  0x000003b0 6c79454e 5374375f 5f637878 31313132 lyENSt7__cxx1112
-  0x000003c0 62617369 635f7374 72696e67 49635374 basic_stringIcSt
-  0x000003d0 31316368 61725f74 72616974 73496345 11char_traitsIcE
-  0x000003e0 53614963 45454553 355f006d 756c7469 SaIcEEES5_.multi
-  0x000003f0 706c7900 5f5a4e32 31626173 69635f6d ply._ZN21basic_m
-  0x00000400 6174685f 6f706572 6174696f 6e733664 ath_operations6d
-  0x00000410 69766964 65454e53 74375f5f 63787831 ivideENSt7__cxx1
-  0x00000420 31313262 61736963 5f737472 696e6749 112basic_stringI
-  0x00000430 63537431 31636861 725f7472 61697473 cSt11char_traits
-  0x00000440 49634553 61496345 45455335 5f6d0064 IcESaIcEEES5_m.d
-  0x00000450 69766964 65005f5a 4e323162 61736963 ivide._ZN21basic
-  0x00000460 5f6d6174 685f6f70 65726174 696f6e73 _math_operations
-  0x00000470 336d6f64 454e5374 375f5f63 78783131 3modENSt7__cxx11
-  0x00000480 31326261 7369635f 73747269 6e674963 12basic_stringIc
-  0x00000490 53743131 63686172 5f747261 69747349 St11char_traitsI
-  0x000004a0 63455361 49634545 4553355f 00646976 cESaIcEEES5_.div
-  0x000004b0 6964655f 77686f6c 655f7769 74685f72 ide_whole_with_r
-  0x000004c0 656d6169 6e646572 005f5a4e 32316261 emainder._ZN21ba
-  0x000004d0 7369635f 6d617468 5f6f7065 72617469 sic_math_operati
-  0x000004e0 6f6e7336 424d4f4e 756d4332 45760044 ons6BMONumC2Ev.D
-  0x000004f0 572e7265 662e5f5f 6778785f 70657273 W.ref.__gxx_pers
-  0x00000500 6f6e616c 6974795f 7630005f 5a4e5374 onality_v0._ZNSt
-  0x00000510 375f5f63 78783131 31326261 7369635f 7__cxx1112basic_
-  0x00000520 73747269 6e674963 53743131 63686172 stringIcSt11char
-  0x00000530 5f747261 69747349 63455361 49634545 _traitsIcESaIcEE
-  0x00000540 31305f4d 5f726570 6c616365 456d6d50 10_M_replaceEmmP
-  0x00000550 4b636d00 5f5a646c 50766d00 5f556e77 Kcm._ZdlPvm._Unw
-  0x00000560 696e645f 52657375 6d65005f 5a4e3231 ind_Resume._ZN21
-  0x00000570 62617369 635f6d61 74685f6f 70657261 basic_math_opera
-  0x00000580 74696f6e 7336424d 4f4e756d 43314576 tions6BMONumC1Ev
-  0x00000590 005f5a4e 32316261 7369635f 6d617468 ._ZN21basic_math
-  0x000005a0 5f6f7065 72617469 6f6e7336 424d4f4e _operations6BMON
-  0x000005b0 756d4332 454e5374 375f5f63 78783131 umC2ENSt7__cxx11
-  0x000005c0 31326261 7369635f 73747269 6e674963 12basic_stringIc
-  0x000005d0 53743131 63686172 5f747261 69747349 St11char_traitsI
-  0x000005e0 63455361 49634545 45005f5a 4e537437 cESaIcEEE._ZNSt7
-  0x000005f0 5f5f6378 78313131 32626173 69635f73 __cxx1112basic_s
-  0x00000600 7472696e 67496353 74313163 6861725f tringIcSt11char_
-  0x00000610 74726169 74734963 45536149 63454539 traitsIcESaIcEE9
-  0x00000620 5f4d5f61 73736967 6e45524b 53345f00 _M_assignERKS4_.
-  0x00000630 5f5a4e32 31626173 69635f6d 6174685f _ZN21basic_math_
-  0x00000640 6f706572 6174696f 6e733642 4d4f4e75 operations6BMONu
-  0x00000650 6d433145 4e537437 5f5f6378 78313131 mC1ENSt7__cxx111
-  0x00000660 32626173 69635f73 7472696e 67496353 2basic_stringIcS
-  0x00000670 74313163 6861725f 74726169 74734963 t11char_traitsIc
-  0x00000680 45536149 63454545 005f5a4e 32316261 ESaIcEEE._ZN21ba
-  0x00000690 7369635f 6d617468 5f6f7065 72617469 sic_math_operati
-  0x000006a0 6f6e7336 424d4f4e 756d4332 45504b63 ons6BMONumC2EPKc
-  0x000006b0 005f5a4e 32316261 7369635f 6d617468 ._ZN21basic_math
-  0x000006c0 5f6f7065 72617469 6f6e7336 424d4f4e _operations6BMON
-  0x000006d0 756d4331 45504b63 005f5a4e 32316261 umC1EPKc._ZN21ba
-  0x000006e0 7369635f 6d617468 5f6f7065 72617469 sic_math_operati
-  0x000006f0 6f6e7336 424d4f4e 756d706c 4553305f ons6BMONumplES0_
-  0x00000700 005f5a4e 32316261 7369635f 6d617468 ._ZN21basic_math
-  0x00000710 5f6f7065 72617469 6f6e7336 424d4f4e _operations6BMON
-  0x00000720 756d6d69 4553305f 005f5a4e 32316261 ummiES0_._ZN21ba
-  0x00000730 7369635f 6d617468 5f6f7065 72617469 sic_math_operati
-  0x00000740 6f6e7336 424d4f4e 756d6d6c 4553305f ons6BMONummlES0_
-  0x00000750 005f5a4e 32316261 7369635f 6d617468 ._ZN21basic_math
-  0x00000760 5f6f7065 72617469 6f6e7336 424d4f4e _operations6BMON
-  0x00000770 756d6476 4553305f 005f474c 4f42414c umdvES0_._GLOBAL
-  0x00000780 5f4f4646 5345545f 5441424c 455f005f _OFFSET_TABLE_._
-  0x00000790 5a4e3231 62617369 635f6d61 74685f6f ZN21basic_math_o
-  0x000007a0 70657261 74696f6e 73313744 49564953 perations17DIVIS
-  0x000007b0 494f4e5f 41434355 52414359 45005f5a ION_ACCURACYE._Z
-  0x000007c0 4e323162 61736963 5f6d6174 685f6f70 N21basic_math_op
-  0x000007d0 65726174 696f6e73 36424d4f 4e756d72 erations6BMONumr
-  0x000007e0 6d455330 5f005f5a 4e323162 61736963 mES0_._ZN21basic
-  0x000007f0 5f6d6174 685f6f70 65726174 696f6e73 _math_operations
-  0x00000800 36424d4f 4e756d6c 74455330 5f005f5a 6BMONumltES0_._Z
-  0x00000810 4e323162 61736963 5f6d6174 685f6f70 N21basic_math_op
-  0x00000820 65726174 696f6e73 36424d4f 4e756d67 erations6BMONumg
-  0x00000830 74455330 5f005f5a 4e323162 61736963 tES0_._ZN21basic
-  0x00000840 5f6d6174 685f6f70 65726174 696f6e73 _math_operations
-  0x00000850 36424d4f 4e756d65 71455330 5f006d65 6BMONumeqES0_.me
-  0x00000860 6d636d70 005f5a4e 32316261 7369635f mcmp._ZN21basic_
-  0x00000870 6d617468 5f6f7065 72617469 6f6e7336 math_operations6
-  0x00000880 424d4f4e 756d6765 4553305f 00       BMONumgeES0_.
+  0x00000230 53305f2e 636f6c64 005f5a4e 53743234 S0_.cold._ZNSt24
+  0x00000240 756e6966 6f726d5f 696e745f 64697374 uniform_int_dist
+  0x00000250 72696275 74696f6e 49694563 6c495374 ributionIiEclISt
+  0x00000260 32336d65 7273656e 6e655f74 77697374 23mersenne_twist
+  0x00000270 65725f65 6e67696e 65496d4c 6d333245 er_engineImLm32E
+  0x00000280 4c6d3632 34454c6d 33393745 4c6d3331 Lm624ELm397ELm31
+  0x00000290 454c6d32 35363734 38333631 35454c6d ELm2567483615ELm
+  0x000002a0 3131454c 6d343239 34393637 32393545 11ELm4294967295E
+  0x000002b0 4c6d3745 4c6d3236 33363932 38363430 Lm7ELm2636928640
+  0x000002c0 454c6d31 35454c6d 34303232 37333037 ELm15ELm40227307
+  0x000002d0 3532454c 6d313845 4c6d3138 31323433 52ELm18ELm181243
+  0x000002e0 33323533 45454545 6952545f 524b4e53 3253EEEEiRT_RKNS
+  0x000002f0 305f3130 70617261 6d5f7479 7065452e 0_10param_typeE.
+  0x00000300 69737261 2e30005f 5a4e3231 62617369 isra.0._ZN21basi
+  0x00000310 635f6d61 74685f6f 70657261 74696f6e c_math_operation
+  0x00000320 73367261 6e646f6d 45792e63 6f6c6400 s6randomEy.cold.
+  0x00000330 2e4c4330 002e4c43 31002e4c 43313200 .LC0..LC1..LC12.
+  0x00000340 2e4c4331 35002e4c 43313400 5f5a4e32 .LC15..LC14._ZN2
+  0x00000350 31626173 69635f6d 6174685f 6f706572 1basic_math_oper
+  0x00000360 6174696f 6e733361 6464454e 5374375f ations3addENSt7_
+  0x00000370 5f637878 31313132 62617369 635f7374 _cxx1112basic_st
+  0x00000380 72696e67 49635374 31316368 61725f74 ringIcSt11char_t
+  0x00000390 72616974 73496345 53614963 45454553 raitsIcESaIcEEES
+  0x000003a0 355f0063 616c6c6f 63006164 64007374 5_.calloc.add.st
+  0x000003b0 726c656e 00667265 65005f5a 4e537437 rlen.free._ZNSt7
+  0x000003c0 5f5f6378 78313131 32626173 69635f73 __cxx1112basic_s
+  0x000003d0 7472696e 67496353 74313163 6861725f tringIcSt11char_
+  0x000003e0 74726169 74734963 45536149 63454539 traitsIcESaIcEE9
+  0x000003f0 5f4d5f63 72656174 6545526d 6d006d65 _M_createERmm.me
+  0x00000400 6d637079 005f5f73 7461636b 5f63686b mcpy.__stack_chk
+  0x00000410 5f666169 6c005f5a 53743139 5f5f7468 _fail._ZSt19__th
+  0x00000420 726f775f 6c6f6769 635f6572 726f7250 row_logic_errorP
+  0x00000430 4b63005f 5a4e3231 62617369 635f6d61 Kc._ZN21basic_ma
+  0x00000440 74685f6f 70657261 74696f6e 73387375 th_operations8su
+  0x00000450 62747261 6374454e 5374375f 5f637878 btractENSt7__cxx
+  0x00000460 31313132 62617369 635f7374 72696e67 1112basic_string
+  0x00000470 49635374 31316368 61725f74 72616974 IcSt11char_trait
+  0x00000480 73496345 53614963 45454553 355f0073 sIcESaIcEEES5_.s
+  0x00000490 75627472 61637400 5f5a4e32 31626173 ubtract._ZN21bas
+  0x000004a0 69635f6d 6174685f 6f706572 6174696f ic_math_operatio
+  0x000004b0 6e73386d 756c7469 706c7945 4e537437 ns8multiplyENSt7
+  0x000004c0 5f5f6378 78313131 32626173 69635f73 __cxx1112basic_s
+  0x000004d0 7472696e 67496353 74313163 6861725f tringIcSt11char_
+  0x000004e0 74726169 74734963 45536149 63454545 traitsIcESaIcEEE
+  0x000004f0 53355f00 6d756c74 69706c79 005f5a4e S5_.multiply._ZN
+  0x00000500 32316261 7369635f 6d617468 5f6f7065 21basic_math_ope
+  0x00000510 72617469 6f6e7336 64697669 6465454e rations6divideEN
+  0x00000520 5374375f 5f637878 31313132 62617369 St7__cxx1112basi
+  0x00000530 635f7374 72696e67 49635374 31316368 c_stringIcSt11ch
+  0x00000540 61725f74 72616974 73496345 53614963 ar_traitsIcESaIc
+  0x00000550 45454553 355f6d00 64697669 6465005f EEES5_m.divide._
+  0x00000560 5a4e3231 62617369 635f6d61 74685f6f ZN21basic_math_o
+  0x00000570 70657261 74696f6e 73336d6f 64454e53 perations3modENS
+  0x00000580 74375f5f 63787831 31313262 61736963 t7__cxx1112basic
+  0x00000590 5f737472 696e6749 63537431 31636861 _stringIcSt11cha
+  0x000005a0 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
+  0x000005b0 45455335 5f006469 76696465 5f77686f EES5_.divide_who
+  0x000005c0 6c655f77 6974685f 72656d61 696e6465 le_with_remainde
+  0x000005d0 72005f5a 4e323162 61736963 5f6d6174 r._ZN21basic_mat
+  0x000005e0 685f6f70 65726174 696f6e73 36424d4f h_operations6BMO
+  0x000005f0 4e756d43 32457600 44572e72 65662e5f NumC2Ev.DW.ref._
+  0x00000600 5f677878 5f706572 736f6e61 6c697479 _gxx_personality
+  0x00000610 5f763000 5f5a4e53 74375f5f 63787831 _v0._ZNSt7__cxx1
+  0x00000620 31313262 61736963 5f737472 696e6749 112basic_stringI
+  0x00000630 63537431 31636861 725f7472 61697473 cSt11char_traits
+  0x00000640 49634553 61496345 4531305f 4d5f7265 IcESaIcEE10_M_re
+  0x00000650 706c6163 65456d6d 504b636d 005f5a64 placeEmmPKcm._Zd
+  0x00000660 6c50766d 005f556e 77696e64 5f526573 lPvm._Unwind_Res
+  0x00000670 756d6500 5f5a4e32 31626173 69635f6d ume._ZN21basic_m
+  0x00000680 6174685f 6f706572 6174696f 6e733642 ath_operations6B
+  0x00000690 4d4f4e75 6d433145 76005f5a 4e323162 MONumC1Ev._ZN21b
+  0x000006a0 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
+  0x000006b0 696f6e73 36424d4f 4e756d43 32454e53 ions6BMONumC2ENS
+  0x000006c0 74375f5f 63787831 31313262 61736963 t7__cxx1112basic
+  0x000006d0 5f737472 696e6749 63537431 31636861 _stringIcSt11cha
+  0x000006e0 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
+  0x000006f0 4545005f 5a4e5374 375f5f63 78783131 EE._ZNSt7__cxx11
+  0x00000700 31326261 7369635f 73747269 6e674963 12basic_stringIc
+  0x00000710 53743131 63686172 5f747261 69747349 St11char_traitsI
+  0x00000720 63455361 49634545 395f4d5f 61737369 cESaIcEE9_M_assi
+  0x00000730 676e4552 4b53345f 005f5a4e 32316261 gnERKS4_._ZN21ba
+  0x00000740 7369635f 6d617468 5f6f7065 72617469 sic_math_operati
+  0x00000750 6f6e7336 424d4f4e 756d4331 454e5374 ons6BMONumC1ENSt
+  0x00000760 375f5f63 78783131 31326261 7369635f 7__cxx1112basic_
+  0x00000770 73747269 6e674963 53743131 63686172 stringIcSt11char
+  0x00000780 5f747261 69747349 63455361 49634545 _traitsIcESaIcEE
+  0x00000790 45005f5a 4e323162 61736963 5f6d6174 E._ZN21basic_mat
+  0x000007a0 685f6f70 65726174 696f6e73 36424d4f h_operations6BMO
+  0x000007b0 4e756d43 3245504b 63005f5a 4e323162 NumC2EPKc._ZN21b
+  0x000007c0 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
+  0x000007d0 696f6e73 36424d4f 4e756d43 3145504b ions6BMONumC1EPK
+  0x000007e0 63005f5a 4e323162 61736963 5f6d6174 c._ZN21basic_mat
+  0x000007f0 685f6f70 65726174 696f6e73 36424d4f h_operations6BMO
+  0x00000800 4e756d70 6c455330 5f005f5a 4e323162 NumplES0_._ZN21b
+  0x00000810 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
+  0x00000820 696f6e73 36424d4f 4e756d6d 69455330 ions6BMONummiES0
+  0x00000830 5f005f5a 4e323162 61736963 5f6d6174 _._ZN21basic_mat
+  0x00000840 685f6f70 65726174 696f6e73 36424d4f h_operations6BMO
+  0x00000850 4e756d6d 6c455330 5f005f5a 4e323162 NummlES0_._ZN21b
+  0x00000860 61736963 5f6d6174 685f6f70 65726174 asic_math_operat
+  0x00000870 696f6e73 36424d4f 4e756d64 76455330 ions6BMONumdvES0
+  0x00000880 5f005f47 4c4f4241 4c5f4f46 46534554 _._GLOBAL_OFFSET
+  0x00000890 5f544142 4c455f00 5f5a4e32 31626173 _TABLE_._ZN21bas
+  0x000008a0 69635f6d 6174685f 6f706572 6174696f ic_math_operatio
+  0x000008b0 6e733137 44495649 53494f4e 5f414343 ns17DIVISION_ACC
+  0x000008c0 55524143 5945005f 5a4e3231 62617369 URACYE._ZN21basi
+  0x000008d0 635f6d61 74685f6f 70657261 74696f6e c_math_operation
+  0x000008e0 7336424d 4f4e756d 726d4553 305f005f s6BMONumrmES0_._
+  0x000008f0 5a4e3231 62617369 635f6d61 74685f6f ZN21basic_math_o
+  0x00000900 70657261 74696f6e 7336424d 4f4e756d perations6BMONum
+  0x00000910 6c744553 305f005f 5a4e3231 62617369 ltES0_._ZN21basi
+  0x00000920 635f6d61 74685f6f 70657261 74696f6e c_math_operation
+  0x00000930 7336424d 4f4e756d 67744553 305f005f s6BMONumgtES0_._
+  0x00000940 5a4e3231 62617369 635f6d61 74685f6f ZN21basic_math_o
+  0x00000950 70657261 74696f6e 7336424d 4f4e756d perations6BMONum
+  0x00000960 65714553 305f005f 5a4e4b53 74375f5f eqES0_._ZNKSt7__
+  0x00000970 63787831 31313262 61736963 5f737472 cxx1112basic_str
+  0x00000980 696e6749 63537431 31636861 725f7472 ingIcSt11char_tr
+  0x00000990 61697473 49634553 61496345 4537636f aitsIcESaIcEE7co
+  0x000009a0 6d706172 6545504b 63006d65 6d636d70 mpareEPKc.memcmp
+  0x000009b0 005f5a4e 32316261 7369635f 6d617468 ._ZN21basic_math
+  0x000009c0 5f6f7065 72617469 6f6e7336 424d4f4e _operations6BMON
+  0x000009d0 756d6765 4553305f 005f5a4e 53743233 umgeES0_._ZNSt23
+  0x000009e0 6d657273 656e6e65 5f747769 73746572 mersenne_twister
+  0x000009f0 5f656e67 696e6549 6d4c6d33 32454c6d _engineImLm32ELm
+  0x00000a00 36323445 4c6d3339 37454c6d 3331454c 624ELm397ELm31EL
+  0x00000a10 6d323536 37343833 36313545 4c6d3131 m2567483615ELm11
+  0x00000a20 454c6d34 32393439 36373239 35454c6d ELm4294967295ELm
+  0x00000a30 37454c6d 32363336 39323836 3430454c 7ELm2636928640EL
+  0x00000a40 6d313545 4c6d3430 32323733 30373532 m15ELm4022730752
+  0x00000a50 454c6d31 38454c6d 31383132 34333332 ELm18ELm18124332
+  0x00000a60 35334545 31315f4d 5f67656e 5f72616e 53EE11_M_gen_ran
+  0x00000a70 64457600 5f5a4e32 31626173 69635f6d dEv._ZN21basic_m
+  0x00000a80 6174685f 6f706572 6174696f 6e733672 ath_operations6r
+  0x00000a90 616e646f 6d457900 5f5a4e53 74313372 andomEy._ZNSt13r
+  0x00000aa0 616e646f 6d5f6465 76696365 375f4d5f andom_device7_M_
+  0x00000ab0 696e6974 45524b4e 5374375f 5f637878 initERKNSt7__cxx
+  0x00000ac0 31313132 62617369 635f7374 72696e67 1112basic_string
+  0x00000ad0 49635374 31316368 61725f74 72616974 IcSt11char_trait
+  0x00000ae0 73496345 53614963 45454500 5f5a4e53 sIcESaIcEEE._ZNS
+  0x00000af0 74313372 616e646f 6d5f6465 76696365 t13random_device
+  0x00000b00 395f4d5f 67657476 616c4576 005f5a4e 9_M_getvalEv._ZN
+  0x00000b10 5374375f 5f637878 31313132 62617369 St7__cxx1112basi
+  0x00000b20 635f7374 72696e67 49635374 31316368 c_stringIcSt11ch
+  0x00000b30 61725f74 72616974 73496345 53614963 ar_traitsIcESaIc
+  0x00000b40 45453132 5f4d5f63 6f6e7374 72756374 EE12_M_construct
+  0x00000b50 456d6300 5f5a5a4e 5374385f 5f646574 Emc._ZZNSt8__det
+  0x00000b60 61696c31 385f5f74 6f5f6368 6172735f ail18__to_chars_
+  0x00000b70 31305f69 6d706c49 6a454576 50636a54 10_implIjEEvPcjT
+  0x00000b80 5f45385f 5f646967 69747300 5f5a4e53 _E8__digits._ZNS
+  0x00000b90 74375f5f 63787831 31313262 61736963 t7__cxx1112basic
+  0x00000ba0 5f737472 696e6749 63537431 31636861 _stringIcSt11cha
+  0x00000bb0 725f7472 61697473 49634553 61496345 r_traitsIcESaIcE
+  0x00000bc0 45395f4d 5f617070 656e6445 504b636d E9_M_appendEPKcm
+  0x00000bd0 005f5a4e 5374375f 5f637878 31313132 ._ZNSt7__cxx1112
+  0x00000be0 62617369 635f7374 72696e67 49635374 basic_stringIcSt
+  0x00000bf0 31316368 61725f74 72616974 73496345 11char_traitsIcE
+  0x00000c00 53614963 45453772 65736572 7665456d SaIcEE7reserveEm
+  0x00000c10 005f5a4e 53743133 72616e64 6f6d5f64 ._ZNSt13random_d
+  0x00000c20 65766963 65375f4d 5f66696e 69457600 evice7_M_finiEv.
+  0x00000c30 5f5a5374 32305f5f 7468726f 775f6c65 _ZSt20__throw_le
+  0x00000c40 6e677468 5f657272 6f72504b 6300     ngth_errorPKc.
```

##### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -3,19 +3,33 @@
   0x00000000 002e7379 6d746162 002e7374 72746162 ..symtab..strtab
   0x00000010 002e7368 73747274 6162002e 72656c61 ..shstrtab..rela
   0x00000020 2e746578 74002e64 61746100 2e627373 .text..data..bss
   0x00000030 002e726f 64617461 2e737472 312e3800 ..rodata.str1.8.
   0x00000040 2e726f64 6174612e 73747231 2e31002e .rodata.str1.1..
   0x00000050 72656c61 2e746578 742e756e 6c696b65 rela.text.unlike
   0x00000060 6c79002e 6763635f 65786365 70745f74 ly..gcc_except_t
-  0x00000070 61626c65 002e6461 74612e5f 5a4e3231 able..data._ZN21
-  0x00000080 62617369 635f6d61 74685f6f 70657261 basic_math_opera
-  0x00000090 74696f6e 73313744 49564953 494f4e5f tions17DIVISION_
-  0x000000a0 41434355 52414359 45002e72 656c612e ACCURACYE..rela.
-  0x000000b0 64617461 2e72656c 2e6c6f63 616c2e44 data.rel.local.D
-  0x000000c0 572e7265 662e5f5f 6778785f 70657273 W.ref.__gxx_pers
-  0x000000d0 6f6e616c 6974795f 7630002e 636f6d6d onality_v0..comm
-  0x000000e0 656e7400 2e6e6f74 652e474e 552d7374 ent..note.GNU-st
-  0x000000f0 61636b00 2e6e6f74 652e676e 752e7072 ack..note.gnu.pr
-  0x00000100 6f706572 7479002e 72656c61 2e65685f operty..rela.eh_
-  0x00000110 6672616d 65002e67 726f7570 00       frame..group.
+  0x00000070 61626c65 002e7465 78742e5f 5a4e5374 able..text._ZNSt
+  0x00000080 32336d65 7273656e 6e655f74 77697374 23mersenne_twist
+  0x00000090 65725f65 6e67696e 65496d4c 6d333245 er_engineImLm32E
+  0x000000a0 4c6d3632 34454c6d 33393745 4c6d3331 Lm624ELm397ELm31
+  0x000000b0 454c6d32 35363734 38333631 35454c6d ELm2567483615ELm
+  0x000000c0 3131454c 6d343239 34393637 32393545 11ELm4294967295E
+  0x000000d0 4c6d3745 4c6d3236 33363932 38363430 Lm7ELm2636928640
+  0x000000e0 454c6d31 35454c6d 34303232 37333037 ELm15ELm40227307
+  0x000000f0 3532454c 6d313845 4c6d3138 31323433 52ELm18ELm181243
+  0x00000100 33323533 45453131 5f4d5f67 656e5f72 3253EE11_M_gen_r
+  0x00000110 616e6445 76002e72 6f646174 612e5f5a andEv..rodata._Z
+  0x00000120 5a4e5374 385f5f64 65746169 6c31385f ZNSt8__detail18_
+  0x00000130 5f746f5f 63686172 735f3130 5f696d70 _to_chars_10_imp
+  0x00000140 6c496a45 45765063 6a545f45 385f5f64 lIjEEvPcjT_E8__d
+  0x00000150 69676974 73002e64 6174612e 5f5a4e32 igits..data._ZN2
+  0x00000160 31626173 69635f6d 6174685f 6f706572 1basic_math_oper
+  0x00000170 6174696f 6e733137 44495649 53494f4e ations17DIVISION
+  0x00000180 5f414343 55524143 5945002e 72656c61 _ACCURACYE..rela
+  0x00000190 2e646174 612e7265 6c2e6c6f 63616c2e .data.rel.local.
+  0x000001a0 44572e72 65662e5f 5f677878 5f706572 DW.ref.__gxx_per
+  0x000001b0 736f6e61 6c697479 5f763000 2e636f6d sonality_v0..com
+  0x000001c0 6d656e74 002e6e6f 74652e47 4e552d73 ment..note.GNU-s
+  0x000001d0 7461636b 002e6e6f 74652e67 6e752e70 tack..note.gnu.p
+  0x000001e0 726f7065 72747900 2e72656c 612e6568 roperty..rela.eh
+  0x000001f0 5f667261 6d65002e 67726f75 7000     _frame..group.
```

#### divide_whole.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1272 (bytes into file)
+  Start of section headers:          1280 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x4f8:
+There are 13 section headers, starting at offset 0x500:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 000105 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000368 000108 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 000145 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 000145 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000145 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000171 000000 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 000109 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000370 000108 18   I 10   1  8
+  [ 3] .data             PROGBITS        0000000000000000 000149 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 000149 000000 00  WA  0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000149 00002c 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000175 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000178 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000198 000060 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000470 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0001f8 000108 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000300 000067 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000488 00006c 00      0   0  1
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000198 000068 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000478 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000200 000108 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000308 000067 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000490 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,14 +1,14 @@
 
 Symbol table '.symtab' contains 11 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS divide_whole.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   261 FUNC    GLOBAL DEFAULT    1 divide_whole
+     3: 0000000000000000   265 FUNC    GLOBAL DEFAULT    1 divide_whole
      4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen_asm
      5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
      6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memset
      8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND _divide_whole_with_remainder
-     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
-    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
```

##### readelf --wide --relocs {}

```diff
@@ -1,18 +1,18 @@
 
-Relocation section '.rela.text' at offset 0x368 contains 11 entries:
+Relocation section '.rela.text' at offset 0x370 contains 11 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000021  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 000000000000002c  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000045  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 000000000000005d  0000000600000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000074  0000000700000004 R_X86_64_PLT32         0000000000000000 memset - 4
+0000000000000075  0000000700000004 R_X86_64_PLT32         0000000000000000 memset - 4
 0000000000000099  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000000b1  0000000800000004 R_X86_64_PLT32         0000000000000000 _divide_whole_with_remainder - 4
-00000000000000b9  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
-00000000000000da  0000000900000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000000eb  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000101  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000000be  0000000900000004 R_X86_64_PLT32         0000000000000000 free - 4
+00000000000000e4  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
+0000000000000100  0000000a00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+00000000000000d4  0000000900000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x470 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x478 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -9,43 +9,51 @@
   Return address column: 16
   Augmentation data:     1b
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_offset: r16 (rip) at cfa-8
   DW_CFA_nop
   DW_CFA_nop
 
-00000018 0000000000000044 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000105
+00000018 000000000000004c 0000001c FDE cie=00000000 pc=0000000000000000..0000000000000109
   DW_CFA_advance_loc: 6 to 0000000000000006
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 2 to 0000000000000008
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 5 to 000000000000000d
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r13 (r13) at cfa-32
-  DW_CFA_advance_loc: 2 to 000000000000000f
+  DW_CFA_advance_loc: 5 to 0000000000000012
   DW_CFA_def_cfa_offset: 40
   DW_CFA_offset: r12 (r12) at cfa-40
-  DW_CFA_advance_loc: 1 to 0000000000000010
+  DW_CFA_advance_loc: 4 to 0000000000000016
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
-  DW_CFA_advance_loc: 4 to 0000000000000014
+  DW_CFA_advance_loc: 1 to 0000000000000017
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
-  DW_CFA_advance_loc: 7 to 000000000000001b
+  DW_CFA_advance_loc: 4 to 000000000000001b
   DW_CFA_def_cfa_offset: 80
-  DW_CFA_advance_loc1: 216 to 00000000000000f3
+  DW_CFA_advance_loc1: 171 to 00000000000000c6
+  DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 4 to 00000000000000f7
+  DW_CFA_advance_loc: 4 to 00000000000000ca
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 00000000000000f8
+  DW_CFA_advance_loc: 1 to 00000000000000cb
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 00000000000000fa
+  DW_CFA_advance_loc: 2 to 00000000000000cd
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 00000000000000fc
+  DW_CFA_advance_loc: 2 to 00000000000000cf
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 00000000000000fe
+  DW_CFA_advance_loc: 2 to 00000000000000d1
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000000100
+  DW_CFA_advance_loc: 2 to 00000000000000d3
   DW_CFA_def_cfa_offset: 8
+  DW_CFA_advance_loc: 13 to 00000000000000e0
+  DW_CFA_restore_state
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -4,90 +4,91 @@
 Disassembly of section .text:
 
 0000000000000000 <divide_whole>:
 divide_whole():
 	endbr64
 	push   %r15
 	push   %r14
-	mov    %rsi,%r14
+	mov    %rdx,%r14
 	push   %r13
+	mov    %rsi,%r13
 	push   %r12
+	mov    %rcx,%r12
 	push   %rbp
-	mov    %rdx,%rbp
 	push   %rbx
-	mov    %rcx,%rbx
 	sub    $0x18,%rsp
 	mov    %rdi,0x8(%rsp)
 	call   25 <divide_whole+0x25>
  R_X86_64_PLT32	strlen_asm-0x4
-	mov    %r14,%rdi
+	mov    %r13,%rdi
 	mov    %rax,%r15
 	call   30 <divide_whole+0x30>
  R_X86_64_PLT32	strlen_asm-0x4
 	mov    $0x1,%esi
-	mov    %rax,%r13
-	lea    (%r15,%rbx,1),%rax
+	mov    %rax,%rbx
+	lea    (%r15,%r12,1),%rax
 	lea    0x1(%rax),%rdi
 	mov    %rax,(%rsp)
 	call   49 <divide_whole+0x49>
  R_X86_64_PLT32	calloc-0x4
-	mov    %rax,%r12
+	mov    %rax,%rbp
 	test   %r15,%r15
 	je     61 <divide_whole+0x61>
 	mov    0x8(%rsp),%rsi
 	mov    %r15,%rdx
 	mov    %rax,%rdi
 	call   61 <divide_whole+0x61>
  R_X86_64_PLT32	memcpy-0x4
 	cmp    (%rsp),%r15
-	jae    78 <divide_whole+0x78>
-	lea    (%r12,%r15,1),%rdi
-	mov    %rbx,%rdx
+	jae    79 <divide_whole+0x79>
+	lea    0x0(%rbp,%r15,1),%rdi
+	mov    %r12,%rdx
 	mov    $0x30,%esi
-	call   78 <divide_whole+0x78>
+	call   79 <divide_whole+0x79>
  R_X86_64_PLT32	memset-0x4
 	mov    (%rsp),%rax
-	lea    0x0(%r13,%r13,4),%rdx
+	lea    (%rbx,%rbx,4),%rdx
 	mov    $0x1,%esi
-	lea    0x2(%r13,%rax,1),%rcx
+	lea    0x2(%rbx,%rax,1),%rcx
 	lea    (%rcx,%rcx,4),%rax
 	mov    %rcx,(%rsp)
 	lea    0x17(%rax,%rdx,2),%rdi
 	call   9d <divide_whole+0x9d>
  R_X86_64_PLT32	calloc-0x4
 	mov    (%rsp),%rcx
-	mov    %rbp,%rdx
-	mov    %r14,%rsi
+	mov    %r14,%rdx
+	mov    %r13,%rsi
 	mov    %rax,%r8
-	mov    %r12,%rdi
+	mov    %rbp,%rdi
 	mov    %rax,%r15
 	call   b5 <divide_whole+0xb5>
  R_X86_64_PLT32	_divide_whole_with_remainder-0x4
-	mov    %rbp,%rdi
-	call   bd <divide_whole+0xbd>
- R_X86_64_PLT32	strlen_asm-0x4
-	mov    %rax,%r13
-	test   %rbx,%rbx
-	je     de <divide_whole+0xde>
-	mov    %rax,%rsi
-	sub    %rbx,%rax
-	mov    %rbx,%rdx
-	sub    %rbx,%rsi
-	lea    0x1(%rbp,%rax,1),%rdi
-	add    %rbp,%rsi
-	call   de <divide_whole+0xde>
- R_X86_64_PLT32	memmove-0x4
-	sub    %rbx,%r13
+	test   %r12,%r12
+	jne    e0 <divide_whole+0xe0>
 	mov    %r15,%rdi
-	movb   $0x2e,0x0(%rbp,%r13,1)
-	call   ef <divide_whole+0xef>
+	call   c2 <divide_whole+0xc2>
  R_X86_64_PLT32	free-0x4
 	add    $0x18,%rsp
-	mov    %r12,%rdi
+	mov    %rbp,%rdi
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
-	jmp    105 <divide_whole+0x105>
+	jmp    d8 <divide_whole+0xd8>
  R_X86_64_PLT32	free-0x4
+	nopl   0x0(%rax,%rax,1)
+	mov    %r14,%rdi
+	call   e8 <divide_whole+0xe8>
+ R_X86_64_PLT32	strlen_asm-0x4
+	mov    %r12,%rdx
+	mov    %rax,%rbx
+	sub    %r12,%rax
+	sub    %r12,%rbx
+	lea    0x1(%r14,%rax,1),%rdi
+	add    %r14,%rbx
+	mov    %rbx,%rsi
+	call   104 <divide_whole+0x104>
+ R_X86_64_PLT32	memmove-0x4
+	movb   $0x2e,(%rbx)
+	jmp    ba <divide_whole+0xba>
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,10 +1,11 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00000010 1b0c0708 90010000 44000000 1c000000 ........D.......
-  0x00000020 00000000 05010000 00460e10 8f02420e .........F....B.
-  0x00000030 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
-  0x00000040 8606440e 38830747 0e5002d8 0e38440e ..D.8..G.P...8D.
-  0x00000050 30410e28 420e2042 0e18420e 10420e08 0A.(B. B..B..B..
+  0x00000010 1b0c0708 90010000 4c000000 1c000000 ........L.......
+  0x00000020 00000000 09010000 00460e10 8f02420e .........F....B.
+  0x00000030 188e0345 0e208d04 450e288c 05440e30 ...E. ..E.(..D.0
+  0x00000040 8606410e 38830744 0e5002ab 0a0e3844 ..A.8..D.P....8D
+  0x00000050 0e30410e 28420e20 420e1842 0e10420e .0A.(B. B..B..B.
+  0x00000060 084d0b00 00000000                   .M......
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.strtab':
   0x00000000 00646976 6964655f 77686f6c 652e6300 .divide_whole.c.
   0x00000010 64697669 64655f77 686f6c65 00737472 divide_whole.str
   0x00000020 6c656e5f 61736d00 63616c6c 6f63006d len_asm.calloc.m
   0x00000030 656d6370 79006d65 6d736574 005f6469 emcpy.memset._di
   0x00000040 76696465 5f77686f 6c655f77 6974685f vide_whole_with_
-  0x00000050 72656d61 696e6465 72006d65 6d6d6f76 remainder.memmov
-  0x00000060 65006672 656500                     e.free.
+  0x00000050 72656d61 696e6465 72006672 6565006d remainder.free.m
+  0x00000060 656d6d6f 766500                     emmove.
```

### Comparing `arithmetica-py-1.0.186/src/python-module/module.c` & `arithmetica-py-1.0.189/src/python-module/module.c`

 * *Files identical despite different names*

