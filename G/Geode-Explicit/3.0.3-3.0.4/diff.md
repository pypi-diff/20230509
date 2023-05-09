# Comparing `tmp/Geode_Explicit-3.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-3.0.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2193655 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-May-03 10:06 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-May-03 10:06 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-May-03 10:06 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2155008 b- defN 23-May-03 10:07 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    19968 b- defN 23-May-03 10:07 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2069504 b- defN 23-May-03 10:07 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   146432 b- defN 23-May-03 10:07 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-May-03 10:07 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2379 b- defN 23-May-03 10:07 Geode_Explicit-3.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 10:07 Geode_Explicit-3.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-03 10:07 Geode_Explicit-3.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 23-May-03 10:07 Geode_Explicit-3.0.3.dist-info/RECORD
-12 files, 4537062 bytes uncompressed, 2191755 bytes compressed:  51.7%
+Zip file size: 2193659 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 23-May-09 15:08 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-May-09 15:08 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-May-09 15:08 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  2155008 b- defN 23-May-09 15:09 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    19968 b- defN 23-May-09 15:09 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  2069504 b- defN 23-May-09 15:09 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   146432 b- defN 23-May-09 15:09 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   141824 b- defN 23-May-09 15:09 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2380 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1118 b- defN 23-May-09 15:09 Geode_Explicit-3.0.4.dist-info/RECORD
+12 files, 4537063 bytes uncompressed, 2191759 bytes compressed:  51.7%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-3.0.3.dist-info/METADATA
+Filename: Geode_Explicit-3.0.4.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-3.0.3.dist-info/WHEEL
+Filename: Geode_Explicit-3.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-3.0.3.dist-info/top_level.txt
+Filename: Geode_Explicit-3.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-3.0.3.dist-info/RECORD
+Filename: Geode_Explicit-3.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180175510
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  3 10:07:11 2023
+Time/Date		Tue May  9 15:09:14 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000177800
 SizeOfInitializedData	0000000000096600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000175510
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00216000
 SizeOfHeaders		00000400
-CheckSum		002141f8
+CheckSum		0021a1a1
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -277,15 +277,15 @@
  001f2d98	001f3618 00000000 00000000 001f7322 00179678
 
 	DLL Name: OpenGeode_geometry.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	1f72e6	  171  ??0?$InfiniteLine@$02@geode@@QEAA@AEBV?$Segment@$02@1@@Z
 	1f7290	   21  ??$point_line_distance@$02@geode@@YANAEBV?$Point@$02@0@AEBV?$InfiniteLine@$02@0@@Z
 	1f725a	  248  ??0?$Segment@$02@geode@@QEAA@AEBV?$Point@$02@1@0@Z
-	1f71ae	  649  ?vertices@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@std@@XZ
+	1f71ae	  652  ?vertices@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBAAEBV?$array@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@std@@XZ
 	1f7170	  489  ?diagonal@?$BoundingBox@$02@geode@@QEBA?AV?$Vector@$02@2@XZ
 	1f7136	  541  ?min@?$BoundingBox@$02@geode@@QEBAAEBV?$Point@$02@2@XZ
 	1f7110	  300  ??1?$BoundingBox@$02@geode@@QEAA@XZ
 	1f70e0	   71  ??0?$BoundingBox@$02@geode@@QEAA@$$QEAV01@@Z
 
  001f2dac	001f35a0 00000000 00000000 001f763c 00179600
 
@@ -37951,15 +37951,15 @@
 	  4dc0: 40 3f 24 42 6f 75 6e 64 69 6e 67 42 6f 78 40 24
 	  4dd0: 30 32 40 67 65 6f 64 65 40 40 51 45 42 41 41 45
 	  4de0: 42 56 3f 24 50 6f 69 6e 74 40 24 30 32 40 32 40
 	  4df0: 58 5a 00 00 e9 01 3f 64 69 61 67 6f 6e 61 6c 40
 	  4e00: 3f 24 42 6f 75 6e 64 69 6e 67 42 6f 78 40 24 30
 	  4e10: 32 40 67 65 6f 64 65 40 40 51 45 42 41 3f 41 56
 	  4e20: 3f 24 56 65 63 74 6f 72 40 24 30 32 40 32 40 58
-	  4e30: 5a 00 89 02 3f 76 65 72 74 69 63 65 73 40 3f 24
+	  4e30: 5a 00 8c 02 3f 76 65 72 74 69 63 65 73 40 3f 24
 	  4e40: 47 65 6e 65 72 69 63 54 72 69 61 6e 67 6c 65 40
 	  4e50: 56 3f 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61
 	  4e60: 70 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e
 	  4e70: 74 40 24 30 32 40 67 65 6f 64 65 40 40 40 73 74
 	  4e80: 64 40 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  4e90: 42 41 41 45 42 56 3f 24 61 72 72 61 79 40 56 3f
 	  4ea0: 24 72 65 66 65 72 65 6e 63 65 5f 77 72 61 70 70
@@ -643415,16 +643415,16 @@
    1801e03f8:	(bad)
    1801e03fd:	insb   (%dx),%es:(%rdi)
    1801e03fe:	insb   (%dx),%es:(%rdi)
    1801e03ff:	outsl  %ds:(%rsi),(%dx)
    1801e0400:	movsxd 0x74(%rcx),%esp
    1801e0403:	imul   $0x0,0x6e(%rdi),%ebp
    1801e040a:	add    %al,(%rax)
-   1801e040c:	rex.WRXB xor 0x64(%r10),%r10b
-   1801e0410:	add    %al,(%rax)
+   1801e040c:	sbb    0x5a(%rdx),%ah
+   1801e040f:	add    %al,%fs:(%rax)
    1801e0412:	add    %al,(%rax)
    1801e0414:	or     $0x60000000,%eax
    1801e0419:	add    (%rax),%eax
    1801e041b:	add    %cl,(%rax,%riz,1)
    1801e041e:	(bad)
    1801e041f:	add    %cl,(%rsp,%rcx,1)
    1801e0422:	(bad)
@@ -681720,18 +681720,19 @@
    1801f719c:	(bad)
    1801f719d:	and    $0x56,%al
    1801f719f:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
    1801f71a4:	rex and $0x30,%al
    1801f71a7:	xor    0x32(%rax),%al
    1801f71aa:	rex pop %rax
    1801f71ac:	pop    %rdx
-   1801f71ad:	add    %cl,0x65763f02(%rcx)
-   1801f71b3:	jb     0x1801f7229
-   1801f71b5:	imul   $0x243f4073,0x65(%rbx),%esp
-   1801f71bc:	rex.RXB
+   1801f71ad:	add    %cl,0x7265763f(%rdx,%rax,1)
+   1801f71b4:	je     0x1801f721f
+   1801f71b6:	movsxd 0x73(%rbp),%esp
+   1801f71b9:	rex (bad)
+   1801f71bb:	and    $0x47,%al
    1801f71bd:	outsb  %gs:(%rsi),(%dx)
    1801f71bf:	gs jb  0x1801f722b
    1801f71c2:	movsxd 0x69(%rdx,%rsi,2),%edx
    1801f71c6:	(bad)
    1801f71c7:	outsb  %ds:(%rsi),(%dx)
    1801f71c8:	insb   (%dx),%es:(%edi)
    1801f71ca:	gs rex push %rsi
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800020b0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  3 10:07:02 2023
+Time/Date		Tue May  9 15:09:04 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000002000
 SizeOfInitializedData	0000000000002a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000020b0
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00009000
 SizeOfHeaders		00000400
-CheckSum		0000cb03
+CheckSum		00012aa7
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -3586,16 +3586,17 @@
    1800033da:	(bad)
    1800033db:	(bad)
    1800033dc:	(bad)
    1800033dd:	(bad)
    1800033de:	(bad)
    1800033df:	incl   (%rax)
    1800033e1:	add    %al,(%rax)
-   1800033e3:	add    %al,0x32(%rsi)
-   1800033e6:	push   %rdx
+   1800033e3:	add    %dl,(%rax)
+   1800033e5:	(bad)
+   1800033e6:	pop    %rdx
    1800033e7:	add    %al,%fs:(%rax)
    1800033ea:	add    %al,(%rax)
    1800033ec:	or     $0x7c000000,%eax
    1800033f1:	add    (%rax),%al
    1800033f3:	add    %cl,%ah
    1800033f5:	cmp    %al,(%rax)
    1800033f7:	add    %cl,%ah
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180165ef0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  3 10:07:05 2023
+Time/Date		Tue May  9 15:09:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000167a00
 SizeOfInitializedData	0000000000091600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000165ef0
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00200000
 SizeOfHeaders		00000400
-CheckSum		001fc7a6
+CheckSum		0020274c
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -622494,16 +622494,17 @@
    1801cfeb8:	(bad)
    1801cfebd:	insb   (%dx),%es:(%rdi)
    1801cfebe:	insb   (%dx),%es:(%rdi)
    1801cfebf:	outsl  %ds:(%rsi),(%dx)
    1801cfec0:	movsxd 0x74(%rcx),%esp
    1801cfec3:	imul   $0x0,0x6e(%rdi),%ebp
    1801cfeca:	add    %al,(%rax)
-   1801cfecc:	rex.WB xor 0x64(%r10),%dl
-   1801cfed0:	add    %al,(%rax)
+   1801cfecc:	adc    $0x62,%al
+   1801cfece:	pop    %rdx
+   1801cfecf:	add    %al,%fs:(%rax)
    1801cfed2:	add    %al,(%rax)
    1801cfed4:	or     $0x60000000,%eax
    1801cfed9:	add    (%rax),%eax
    1801cfedb:	add    %ch,0x8ac001d(%rdx,%rbx,1)
    1801cfee2:	sbb    $0x0,%eax
 	...
    1801cfeef:	add    %bh,(%rax)
```

## Comparing `Geode_Explicit-3.0.3.dist-info/METADATA` & `Geode_Explicit-3.0.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 3.0.3
+Version: 3.0.4
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background (==7.*,>=7.1.0)
-Requires-Dist: geode-common (==25.*,>=25.0.2)
-Requires-Dist: geode-conversion (==5.*,>=5.0.1)
-Requires-Dist: opengeode-core (==14.*,>=14.0.7)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.4)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.0)
-Requires-Dist: opengeode-inspector (==3.*,>=3.0.1)
-Requires-Dist: opengeode-io (==6.*,>=6.0.1)
+Requires-Dist: geode-background (==7.*,>=7.1.2)
+Requires-Dist: geode-common (==25.*,>=25.0.6)
+Requires-Dist: geode-conversion (==5.*,>=5.0.4)
+Requires-Dist: opengeode-core (==14.*,>=14.0.14)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.6)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.2)
+Requires-Dist: opengeode-inspector (==3.*,>=3.0.3)
+Requires-Dist: opengeode-io (==6.*,>=6.0.4)
 
 <h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 3.0.3 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 3.0.4 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.1.0)
-Requires-Dist: geode-common (==25.*,>=25.0.2) Requires-Dist: geode-conversion
-(==5.*,>=5.0.1) Requires-Dist: opengeode-core (==14.*,>=14.0.7) Requires-Dist:
-opengeode-geosciences (==7.*,>=7.0.4) Requires-Dist: opengeode-geosciencesio
-(==4.*,>=4.1.0) Requires-Dist: opengeode-inspector (==3.*,>=3.0.1) Requires-
-Dist: opengeode-io (==6.*,>=6.0.1)
+Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.1.2)
+Requires-Dist: geode-common (==25.*,>=25.0.6) Requires-Dist: geode-conversion
+(==5.*,>=5.0.4) Requires-Dist: opengeode-core (==14.*,>=14.0.14) Requires-Dist:
+opengeode-geosciences (==7.*,>=7.0.6) Requires-Dist: opengeode-geosciencesio
+(==4.*,>=4.1.2) Requires-Dist: opengeode-inspector (==3.*,>=3.0.3) Requires-
+Dist: opengeode-io (==6.*,>=6.0.4)
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Explicit-3.0.3.dist-info/RECORD` & `Geode_Explicit-3.0.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 geode_explicit/__init__.py,sha256=-1Ma-Q_qKho5-HJywdEjGH_v91Dp0h8zchFCzKp7ADk,194
 geode_explicit/brep.py,sha256=5gXUGyujJVK7W7i2Zoqb5_9Mb5jPPZLiYZX9piVVUGY,271
 geode_explicit/section.py,sha256=diHY0-G0OXfICdOX3HSTnwrdrW3WOsct7GAT4rECQb4,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=zC0eFdLg5maTUpnNnBC51vSHULrMoGF84Qn6lcEqG7c,2155008
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=S0ckA_YcnpbdU-WtAtNRIm4S4GtLaiMxJTyFZK-njQk,19968
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=z6Mde-TefmVw-zyPeYL0vJx1rzfYvHxEEHwhhc2O0Z0,2069504
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=vMUgm_YZnVZDZpwZUSjjzIa3DANfeFNh2CINvnBlLw0,146432
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=vMK-q9PxRLAF-vWMYaRyd9bbkxowcY5B84O4BBGL9N0,141824
-Geode_Explicit-3.0.3.dist-info/METADATA,sha256=ESYacd0c-t51HW5OP2ghmNBOCsvOYUucP8sTF9xtt5U,2379
-Geode_Explicit-3.0.3.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Explicit-3.0.3.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-3.0.3.dist-info/RECORD,,
+geode_explicit/bin/Geode-Explicit_brep.dll,sha256=yeD_fRqFa6NCF2O29prDdPZOkqfdnycoryUWWIIm0qs,2155008
+geode_explicit/bin/Geode-Explicit_common.dll,sha256=VaacN2TeboPe5LR-qysRvYjs9XdZArPdz3PEKpzCt6I,19968
+geode_explicit/bin/Geode-Explicit_section.dll,sha256=eXgdAirqGMN2mMAQL76j2_LB3pFAKWGxfE9Aom63EEc,2069504
+geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=AKIwiqb0ZRN3PxTsXy84SMnqGpIYT_jF2xIG5hzBI5E,146432
+geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=IoJ5w0qJValYQTt1uFheuhw1yFyUq9m_plOjM1vgB4o,141824
+Geode_Explicit-3.0.4.dist-info/METADATA,sha256=M0VXiFqpuGZd6j_HZp_-tkHQGCgD18PlTYed1Y2yU7M,2380
+Geode_Explicit-3.0.4.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Explicit-3.0.4.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-3.0.4.dist-info/RECORD,,
```

