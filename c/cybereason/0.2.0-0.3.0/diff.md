# Comparing `tmp/cybereason-0.2.0.tar.gz` & `tmp/cybereason-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybereason-0.2.0.tar", last modified: Fri Apr 14 00:37:04 2023, max compression
+gzip compressed data, was "cybereason-0.3.0.tar", last modified: Tue May  9 19:47:29 2023, max compression
```

## Comparing `cybereason-0.2.0.tar` & `cybereason-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.941291 cybereason-0.2.0/
--rw-rw-rw-   0        0        0     1481 2023-04-12 17:30:28.000000 cybereason-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2986 2023-04-14 00:37:04.942615 cybereason-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2078 2023-04-14 00:37:04.943954 cybereason-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0       60 2023-04-12 17:30:28.000000 cybereason-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.838613 cybereason-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.903251 cybereason-0.2.0/src/cybereason/
--rw-rw-rw-   0        0        0      198 2023-04-13 22:34:20.000000 cybereason-0.2.0/src/cybereason/__init__.py
--rw-rw-rw-   0        0        0     3023 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/_patch.py
--rw-rw-rw-   0        0        0     1306 2023-04-13 17:53:18.000000 cybereason-0.2.0/src/cybereason/_typing.py
--rw-rw-rw-   0        0        0    15785 2023-04-14 00:09:11.000000 cybereason-0.2.0/src/cybereason/client.py
--rw-rw-rw-   0        0        0     2640 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/custom_rules.py
--rw-rw-rw-   0        0        0     4573 2023-04-13 17:48:23.000000 cybereason-0.2.0/src/cybereason/exceptions.py
--rw-rw-rw-   0        0        0     3531 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/incident_reponse.py
--rw-rw-rw-   0        0        0     5373 2023-04-13 22:25:58.000000 cybereason-0.2.0/src/cybereason/malops.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.929885 cybereason-0.2.0/src/cybereason/parse/
--rw-rw-rw-   0        0        0      147 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/parse/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/parse/cef.py
--rw-rw-rw-   0        0        0     2846 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/parse/server.py
--rw-rw-rw-   0        0        0        0 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/py.typed
--rw-rw-rw-   0        0        0    16783 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/sensors.py
--rw-rw-rw-   0        0        0     4477 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/system.py
--rw-rw-rw-   0        0        0     6444 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/threat_intel.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.938555 cybereason-0.2.0/src/cybereason/utils/
--rw-rw-rw-   0        0        0     4642 2023-04-14 00:07:58.000000 cybereason-0.2.0/src/cybereason/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/utils/guid.py
-drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.918827 cybereason-0.2.0/src/cybereason.egg-info/
--rw-rw-rw-   0        0        0     2986 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      229 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 19:47:29.869994 cybereason-0.3.0/
+-rw-rw-rw-   0        0        0     1481 2023-04-12 17:30:28.000000 cybereason-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2986 2023-05-09 19:47:29.870991 cybereason-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2085 2023-05-09 19:47:29.873996 cybereason-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       60 2023-04-12 17:30:28.000000 cybereason-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:47:29.758282 cybereason-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 19:47:29.820740 cybereason-0.3.0/src/cybereason/
+-rw-rw-rw-   0        0        0      198 2023-05-09 19:40:36.000000 cybereason-0.3.0/src/cybereason/__init__.py
+-rw-rw-rw-   0        0        0     1839 2023-04-18 14:24:10.000000 cybereason-0.3.0/src/cybereason/_typing.py
+-rw-rw-rw-   0        0        0    15614 2023-05-09 19:39:34.000000 cybereason-0.3.0/src/cybereason/client.py
+-rw-rw-rw-   0        0        0     4619 2023-04-14 19:14:27.000000 cybereason-0.3.0/src/cybereason/exceptions.py
+-rw-rw-rw-   0        0        0     3531 2023-04-12 17:30:28.000000 cybereason-0.3.0/src/cybereason/incident_reponse.py
+-rw-rw-rw-   0        0        0     5386 2023-04-19 18:25:11.000000 cybereason-0.3.0/src/cybereason/malops.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:47:29.852910 cybereason-0.3.0/src/cybereason/parse/
+-rw-rw-rw-   0        0        0      147 2023-04-12 17:30:28.000000 cybereason-0.3.0/src/cybereason/parse/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-04-12 17:30:28.000000 cybereason-0.3.0/src/cybereason/parse/cef.py
+-rw-rw-rw-   0        0        0     2846 2023-04-12 17:30:28.000000 cybereason-0.3.0/src/cybereason/parse/server.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:30:28.000000 cybereason-0.3.0/src/cybereason/py.typed
+-rw-rw-rw-   0        0        0     5175 2023-04-18 17:55:56.000000 cybereason-0.3.0/src/cybereason/rules.py
+-rw-rw-rw-   0        0        0    16794 2023-05-09 19:34:26.000000 cybereason-0.3.0/src/cybereason/sensors.py
+-rw-rw-rw-   0        0        0     4391 2023-04-15 11:32:54.000000 cybereason-0.3.0/src/cybereason/system.py
+-rw-rw-rw-   0        0        0     7617 2023-04-21 00:32:29.000000 cybereason-0.3.0/src/cybereason/threat_intel.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:47:29.866938 cybereason-0.3.0/src/cybereason/utils/
+-rw-rw-rw-   0        0        0     4515 2023-04-17 23:20:46.000000 cybereason-0.3.0/src/cybereason/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-12 17:30:28.000000 cybereason-0.3.0/src/cybereason/utils/guid.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:47:29.840042 cybereason-0.3.0/src/cybereason.egg-info/
+-rw-rw-rw-   0        0        0     2986 2023-05-09 19:47:29.000000 cybereason-0.3.0/src/cybereason.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-05-09 19:47:29.000000 cybereason-0.3.0/src/cybereason.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:47:29.000000 cybereason-0.3.0/src/cybereason.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-09 19:47:29.000000 cybereason-0.3.0/src/cybereason.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      236 2023-05-09 19:47:29.000000 cybereason-0.3.0/src/cybereason.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 19:47:29.000000 cybereason-0.3.0/src/cybereason.egg-info/top_level.txt
```

### Comparing `cybereason-0.2.0/LICENSE` & `cybereason-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybereason-0.2.0/PKG-INFO` & `cybereason-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.2.0
+Version: 0.3.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.2.0 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.3.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
```

### Comparing `cybereason-0.2.0/setup.cfg` & `cybereason-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -76,55 +76,56 @@
 000004b0: 6765 5f64 6972 203d 200d 0a09 3d73 7263  ge_dir = ...=src
 000004c0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 000004d0: 643a 0d0a 7365 7475 705f 7265 7175 6972  d:..setup_requir
 000004e0: 6573 203d 200d 0a09 7365 7475 7074 6f6f  es = ...setuptoo
 000004f0: 6c73 203e 3d20 3430 2e39 2e30 0d0a 0977  ls >= 40.9.0...w
 00000500: 6865 656c 203e 3d20 302e 3332 0d0a 696e  heel >= 0.32..in
 00000510: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-00000520: 200d 0a09 6874 7470 783e 3d30 2e32 322e   ...httpx>=0.22.
-00000530: 300d 0a09 6e65 7374 2d61 7379 6e63 696f  0...nest-asyncio
-00000540: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000550: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000560: 7265 203d 2073 7263 0d0a 0d0a 5b6f 7074  re = src....[opt
-00000570: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-00000580: 615d 0d0a 6379 6265 7265 6173 6f6e 203d  a]..cybereason =
-00000590: 200d 0a09 7079 2e74 7970 6564 0d0a 0d0a   ...py.typed....
-000005a0: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
-000005b0: 7265 7175 6972 655d 0d0a 7a69 7020 3d20  require]..zip = 
-000005c0: 0d0a 0970 797a 6970 7065 720d 0a73 6f63  ...pyzipper..soc
-000005d0: 6b73 203d 200d 0a09 6874 7470 782d 736f  ks = ...httpx-so
-000005e0: 636b 735b 6173 796e 6369 6f5d 0d0a 6465  cks[asyncio]..de
-000005f0: 7620 3d20 0d0a 096d 7970 790d 0a09 666c  v = ...mypy...fl
-00000600: 616b 6538 0d0a 0970 7974 6573 740d 0a09  ake8...pytest...
-00000610: 7079 7961 6d6c 0d0a 0970 7974 6573 742d  pyyaml...pytest-
-00000620: 6173 796e 6369 6f0d 0a09 7079 7465 7374  asyncio...pytest
-00000630: 2d64 6174 6166 696c 6573 0d0a 096a 736f  -datafiles...jso
-00000640: 6e73 6368 656d 610d 0a09 6671 646e 0d0a  nschema...fqdn..
-00000650: 0972 6663 3333 3339 2d76 616c 6964 6174  .rfc3339-validat
-00000660: 6f72 0d0a 0969 736f 6475 7261 7469 6f6e  or...isoduration
-00000670: 0d0a 0969 646e 610d 0a09 7266 6333 3938  ...idna...rfc398
-00000680: 370d 0a64 6f63 7320 3d20 0d0a 0973 7068  7..docs = ...sph
-00000690: 696e 780d 0a09 7370 6869 6e78 2d72 7464  inx...sphinx-rtd
-000006a0: 2d74 6865 6d65 0d0a 0d0a 5b66 6c61 6b65  -theme....[flake
-000006b0: 385d 0d0a 6967 6e6f 7265 203d 2045 3131  8]..ignore = E11
-000006c0: 352c 2045 3232 312c 2045 3234 312c 2045  5, E221, E241, E
-000006d0: 3430 322c 2045 3733 310d 0a65 7863 6c75  402, E731..exclu
-000006e0: 6465 203d 200d 0a09 2e67 6974 2c0d 0a09  de = ....git,...
-000006f0: 5f5f 7079 6361 6368 655f 5f2c 0d0a 092e  __pycache__,....
-00000700: 6d79 7079 5f63 6163 6865 2c0d 0a09 2e70  mypy_cache,....p
-00000710: 7974 6573 745f 6361 6368 652c 0d0a 092e  ytest_cache,....
-00000720: 7665 6e76 2c0d 0a09 2e65 6767 732c 0d0a  venv,....eggs,..
-00000730: 0962 7569 6c64 2c0d 0a09 7465 7374 2e2a  .build,...test.*
-00000740: 2c0d 0a09 5f74 7970 696e 672e 7079 0d0a  ,..._typing.py..
-00000750: 696e 6c69 6e65 2d71 756f 7465 7320 3d20  inline-quotes = 
-00000760: 7369 6e67 6c65 0d0a 6d61 782d 636f 6d70  single..max-comp
-00000770: 6c65 7869 7479 203d 2031 330d 0a6d 6178  lexity = 13..max
-00000780: 2d6c 696e 652d 6c65 6e67 7468 203d 2039  -line-length = 9
-00000790: 390d 0a6d 756c 7469 6c69 6e65 2d71 756f  9..multiline-quo
-000007a0: 7465 7320 3d20 7369 6e67 6c65 0d0a 646f  tes = single..do
-000007b0: 6373 7472 696e 672d 7175 6f74 6573 203d  cstring-quotes =
-000007c0: 2073 696e 676c 650d 0a0d 0a5b 6d79 7079   single....[mypy
-000007d0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
-000007e0: 675f 696d 706f 7274 7320 3d20 5472 7565  g_imports = True
-000007f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000800: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000810: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000520: 200d 0a09 6874 7470 785b 6874 7470 325d   ...httpx[http2]
+00000530: 3e3d 302e 3232 2e30 0d0a 096e 6573 742d  >=0.22.0...nest-
+00000540: 6173 796e 6369 6f0d 0a0d 0a5b 6f70 7469  asyncio....[opti
+00000550: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000560: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000570: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000580: 6167 655f 6461 7461 5d0d 0a63 7962 6572  age_data]..cyber
+00000590: 6561 736f 6e20 3d20 0d0a 0970 792e 7479  eason = ...py.ty
+000005a0: 7065 640d 0a0d 0a5b 6f70 7469 6f6e 732e  ped....[options.
+000005b0: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
+000005c0: 0a7a 6970 203d 200d 0a09 7079 7a69 7070  .zip = ...pyzipp
+000005d0: 6572 0d0a 736f 636b 7320 3d20 0d0a 0968  er..socks = ...h
+000005e0: 7474 7078 2d73 6f63 6b73 5b61 7379 6e63  ttpx-socks[async
+000005f0: 696f 5d0d 0a64 6576 203d 200d 0a09 6d79  io]..dev = ...my
+00000600: 7079 0d0a 0966 6c61 6b65 380d 0a09 7079  py...flake8...py
+00000610: 7465 7374 0d0a 0970 7979 616d 6c0d 0a09  test...pyyaml...
+00000620: 7079 7465 7374 2d61 7379 6e63 696f 0d0a  pytest-asyncio..
+00000630: 0970 7974 6573 742d 6461 7461 6669 6c65  .pytest-datafile
+00000640: 730d 0a09 6a73 6f6e 7363 6865 6d61 0d0a  s...jsonschema..
+00000650: 0966 7164 6e0d 0a09 7266 6333 3333 392d  .fqdn...rfc3339-
+00000660: 7661 6c69 6461 746f 720d 0a09 6973 6f64  validator...isod
+00000670: 7572 6174 696f 6e0d 0a09 6964 6e61 0d0a  uration...idna..
+00000680: 0972 6663 3339 3837 0d0a 646f 6373 203d  .rfc3987..docs =
+00000690: 200d 0a09 7370 6869 6e78 0d0a 0973 7068   ...sphinx...sph
+000006a0: 696e 782d 7274 642d 7468 656d 650d 0a0d  inx-rtd-theme...
+000006b0: 0a5b 666c 616b 6538 5d0d 0a69 676e 6f72  .[flake8]..ignor
+000006c0: 6520 3d20 4531 3135 2c20 4532 3231 2c20  e = E115, E221, 
+000006d0: 4532 3431 2c20 4534 3032 2c20 4537 3331  E241, E402, E731
+000006e0: 0d0a 6578 636c 7564 6520 3d20 0d0a 092e  ..exclude = ....
+000006f0: 6769 742c 0d0a 095f 5f70 7963 6163 6865  git,...__pycache
+00000700: 5f5f 2c0d 0a09 2e6d 7970 795f 6361 6368  __,....mypy_cach
+00000710: 652c 0d0a 092e 7079 7465 7374 5f63 6163  e,....pytest_cac
+00000720: 6865 2c0d 0a09 2e76 656e 762c 0d0a 092e  he,....venv,....
+00000730: 6567 6773 2c0d 0a09 6275 696c 642c 0d0a  eggs,...build,..
+00000740: 0974 6573 742e 2a2c 0d0a 095f 7479 7069  .test.*,..._typi
+00000750: 6e67 2e70 790d 0a69 6e6c 696e 652d 7175  ng.py..inline-qu
+00000760: 6f74 6573 203d 2073 696e 676c 650d 0a6d  otes = single..m
+00000770: 6178 2d63 6f6d 706c 6578 6974 7920 3d20  ax-complexity = 
+00000780: 3135 0d0a 6d61 782d 6c69 6e65 2d6c 656e  15..max-line-len
+00000790: 6774 6820 3d20 3939 0d0a 6d75 6c74 696c  gth = 99..multil
+000007a0: 696e 652d 7175 6f74 6573 203d 2073 696e  ine-quotes = sin
+000007b0: 676c 650d 0a64 6f63 7374 7269 6e67 2d71  gle..docstring-q
+000007c0: 756f 7465 7320 3d20 7369 6e67 6c65 0d0a  uotes = single..
+000007d0: 0d0a 5b6d 7970 795d 0d0a 6967 6e6f 7265  ..[mypy]..ignore
+000007e0: 5f6d 6973 7369 6e67 5f69 6d70 6f72 7473  _missing_imports
+000007f0: 203d 2054 7275 650d 0a0d 0a5b 6567 675f   = True....[egg_
+00000800: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+00000810: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000820: 300d 0a0d 0a                             0....
```

### Comparing `cybereason-0.2.0/src/cybereason/client.py` & `cybereason-0.3.0/src/cybereason/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 from typing import Any, Optional, TYPE_CHECKING, cast
 from json.decoder import JSONDecodeError
 from functools import cached_property
 from pathlib import Path
 from io import BytesIO
 import logging
+import asyncio
 
-# monkey-patch to allow multiple {'file-encoding': 'chunked'} headers
-import httpx
-from ._patch import normalize_and_validate
-httpx._transports.default.httpcore._async.http11.h11._headers.normalize_and_validate = normalize_and_validate  # noqa: E501
 from httpx import AsyncClient, HTTPStatusError, ConnectError
 
 from .exceptions import (
-    AccessDenied, AuthenticationError, ResourceNotFoundError,
-    UnauthorizedRequest, ServerError, ClientError,
+    AccessDenied, AuthenticationError, UnauthorizedRequest,
+    ServerError, ClientError, CybereasonException, TooManyRequests,
     get_response_error,
 )
 from .utils import get_filename, to_list, get_config_from_env, parse_query_response
-from .custom_rules import CustomRulesMixin
+from .rules import CustomRulesMixin, IsolationRulesMixin
 from .incident_reponse import IncidentResponseMixin
 from .malops import MalopsMixin
 from .sensors import SensorsMixin
 from .system import SystemMixin
 from .threat_intel import ThreatIntelligenceMixin
 
 if TYPE_CHECKING:
-    from typing import AsyncIterator, Callable, Dict, List, Literal, Tuple, Union
+    from typing import AsyncIterator, Callable, Dict, Literal, Tuple, Union
     from io import BufferedIOBase
     from tarfile import TarFile
     from zipfile import ZipFile
     from os import PathLike
     from ._typing import Query, UrlPath, URL
 
 DEFAULT_TIMEOUT = 30.0
 DEFAULT_PAGE_SIZE = 50
 
 log = logging.getLogger(__name__)
 
 
 class Cybereason(
     CustomRulesMixin,
+    IsolationRulesMixin,
     IncidentResponseMixin,
     MalopsMixin,
     SensorsMixin,
     SystemMixin,
     ThreatIntelligenceMixin,
 ):
     def __init__(
@@ -70,35 +68,37 @@
         headers  = {
             'content-type': 'application/json',
             'user-agent': f'python-cybereason/{".".join(map(str, __version__))}',
         }
 
         if self.proxy and self.proxy.startswith('socks'):
             # https://github.com/encode/httpx/discussions/2305
-            # TODO: go back to socksio when ^ it's resolved
+            # TODO: go back to socksio when ^ is resolved
             # see: commit f439393
             try:
                 from httpx_socks import AsyncProxyTransport
             except ImportError:
                 msg = 'Install SOCKS proxy support using `pip install cybereason[socks]`.'
                 raise ImportError(msg) from None
 
             return AsyncClient(
                 base_url=base_url,
                 headers=headers,
                 transport=AsyncProxyTransport.from_url(self.proxy),
                 timeout=self.timeout,
+                http2=True,
             )
 
         else:
             return AsyncClient(
                 base_url=base_url,
                 headers=headers,
                 proxies=self.proxy,
                 timeout=self.timeout,
+                http2=True,
             )
 
     @cached_property
     def session_sage(self) -> AsyncClient:
         return AsyncClient(
             base_url='https://sage.cybereason.com/rest',
             headers={'content-type': 'application/json'},
@@ -183,29 +183,40 @@
         async def run_task(task):
             async with semaphore:
                 return await task
 
         return await asyncio.gather(*(run_task(task) for task in tasks))
 
     def check_resp(self, resp):
-        if resp['status'] == 'SUCCESS':
-            return resp['data']
+        if 'status' in resp:
+            if resp['status'] == 'SUCCESS':
+                return resp['data']
+            else:
+                exc = get_response_error(resp['status'])
+                raise exc(resp.get('message'))
+        elif 'outcome' in resp:
+            if resp['outcome'] == 'success':
+                return resp['data']
+            else:
+                # TODO: same model?
+                exc = get_response_error(resp['outcome'].upper())
+                raise exc(resp['outcome'])
         else:
-            exc = get_response_error(resp['status'])
-            raise exc(resp.get('message'))
+            raise CybereasonException(resp)
 
     async def _request(
         self,
         method:   str,
         path:     'UrlPath',
         data:     Any = None,
         query:    'Query' = None,
         files:    'Query' = None,
         raw:      bool = False,
         raw_data: bool = False,
+        retried:  bool = False,
     ) -> Any:
         if raw_data:
             kwargs = dict(data=data, params=query, files=files)
         else:
             kwargs = dict(json=data, params=query, files=files)
 
         resp = await self.session.request(method, path, **kwargs)
@@ -219,15 +230,32 @@
                 raise ClientError(e.response.text) from None
             elif e.response.status_code == 412:
                 raise AccessDenied(e.response.text) from None
             elif e.response.status_code == 500:
                 raise ServerError(e.response.text) from None
             elif e.response.status_code == 302:
                 raise AuthenticationError from None
-            raise
+            elif e.response.status_code == 429:
+                # throttling
+                if retried is False:
+                    WAIT = 60
+
+                    log.warning('Too many requests. Waiting %i seconds...', WAIT)
+                    await asyncio.sleep(WAIT)
+
+                    if 'json' in kwargs:
+                        kwargs['data'] = kwargs.pop('json')
+                    kwargs['query'] = kwargs.pop('params')
+                    return await self._request(
+                        method, path, **kwargs, raw=raw, raw_data=raw_data, retried=True
+                    )
+                else:
+                    raise TooManyRequests(e.response.text) from None
+            else:
+                raise
 
         if raw:
             return resp.content
         else:
             try:
                 return resp.json()
             except JSONDecodeError:
@@ -314,136 +342,110 @@
             destpath.write_bytes(buffer.read())
             log.info('%s saved as %s', filename, destpath)
 
         return destpath.resolve()
 
     async def aiter_pages(
         self,
-        path:          'UrlPath',
-        data:          Any,
-        key:           str,
-        page_size:     int = DEFAULT_PAGE_SIZE,
-        sort:          'Literal["ASC", "DESC"]' = 'ASC',
+        path:         'UrlPath',
+        data:         'Dict[str, Any]',
+        key:          str,
+        *, page_size: int = DEFAULT_PAGE_SIZE,
+        check_resp:   bool = False,
+        sort:         'Literal["ASC", "DESC"]' = 'ASC',
     ) -> 'AsyncIterator[Dict[str, Any]]':
+        '''
+        Args:
+            check_resp: ``True`` if the response returns either a
+                {status, data} or a {outcome, data} schema.
+        '''
         data = {**data, 'limit': page_size, 'offset': 0, 'sortDirection': sort}
 
         while True:
             resp = await self.post(path, data)
-            # XXX: not all results have the same schema
-            items = resp[key] if key in resp else resp['data'][key]
+            if check_resp is True:
+                resp = self.check_resp(resp)
 
-            for item in items:
+            for item in resp[key]:
                 yield item
 
-            # XXX: ditto
-            if 'hasMoreResults' in resp:
-                if not resp['hasMoreResults']:
-                    break
-            elif not resp['data']['hasMoreResults']:
+            if not resp['hasMoreResults']:
                 break
 
-            data['offset'] += 1  # XXX: page number
-
-    async def post_sage(self, path, data):
-        resp = await self.session_sage.post(path, json=data)
-        resp.raise_for_status()
-        return resp.json()
-
-# region ISOLATION RULES
-    async def get_isolation_rules(self) -> 'List[Dict[str, Any]]':
-        '''Retrieve a list of isolation rules.
-        '''
-        return await self.get('settings/isolation-rule')
-
-    async def get_isolation_rule(self, id) -> 'Dict[str, Any]':
-        rules = await self.get_isolation_rules()
-        try:
-            return [r for r in rules if r['ruleId'] == id][0]
-        except IndexError:
-            raise ResourceNotFoundError(id) from None
+            data['offset'] += 1  # page number
 
-    async def create_isolation_rule(
+    # some endpoints use a different pagination schema than `aiter_pages()``
+    async def aiter_items(
         self,
-        direction: str,
-        blocking:  bool,
-        ip:        str,  # TODO: validate
-        port:      Optional[int] = None,
-    ) -> 'Dict[str, Any]':
+        path:           'UrlPath',
+        data:           'Dict[str, Any]',
+        key:            str,
+        *, page_size:   int = DEFAULT_PAGE_SIZE,
+        check_resp:     bool = False,
+        pagination:     bool = False,
+    ) -> 'AsyncIterator[Dict[str, Any]]':
         '''
         Args:
-            direction: The direction of the allowed communication.
-                {'ALL', 'OUTGOING', 'INCOMING'}
-            blocking: States whether communication with the given IP or
-                port is allowed. If ``True`` communication is blocked.
-            ip: The IP address of the machine to which the rule applies.
-            port: The port by which Cybereason communicates with an
-                isolated machine, according to the rule.
+            check_resp: ``True`` if the response returns either a
+                {status, data} or a {outcome, data} schema.
+            pagination: ``True`` if ``size`` and ``page`` go inside a
+                ``pagination`` object.
         '''
-        rule = {
-            'ruleId':          None,
-            'port':            port or '',
-            'ipAddressString': ip,
-            'blocking':        blocking,
-            'direction':       direction,
-        }
-        return await self.post('settings/isolation-rule', rule)
+        if pagination:
+            data = {**data, 'pagination': {'size': page_size}}
+        else:
+            data = {**data, 'size': page_size}
 
-    async def update_isolation_rule(
-        self,
-        id:           str,
-        *, direction: Optional[str] = None,
-        blocking:     Optional[bool] = None,
-        ip:           Optional[str] = None,
-        port:         Optional[int] = None,
-    ) -> 'Dict[str, Any]':
-        '''
-        Args:
-            id: rule ID.
-            port: ``0`` means any port.
-        '''
-        rule = await self.get_isolation_rule(id)
-        if direction is not None:
-            rule['direction'] = direction
-        if blocking is not None:
-            rule['blocking'] = blocking
-        if ip is not None:
-            rule['ipAddressString'] = ip or ''
-        if port is not None:
-            rule['port'] = port
+        page = 0
+
+        while True:
+            if pagination:
+                data['pagination']['page'] = page
+            else:
+                data['page'] = page
 
-        return await self.put('settings/isolation-rule', rule)
+            resp = await self.post(path, data)
+            if check_resp is True:
+                resp = self.check_resp(resp)
 
-    async def delete_isolation_rule(self, id: str) -> None:
-        '''Deletes an isolation exception rule.
-        '''
-        rule = await self.get_isolation_rule(id)
-        await self.post('settings/isolation-rule/delete', rule)
-# endregion
+            for item in resp[key]:
+                yield item
+
+            if len(resp[key]) < page_size:
+                break
+
+            page += 1
+
+    async def post_sage(self, path, data):
+        resp = await self.session_sage.post(path, json=data)
+        resp.raise_for_status()
+        return resp.json()
 
     @cached_property
     def features_map(self) -> 'Dict[str, Dict[str, Any]]':
         import asyncio
 
         async def func():
             return await self.get('translate/features/all/')
 
         return asyncio.run(func())
 
-    async def get_user_audit_logs(self, rotated: bool = True) -> 'AsyncIterator[Dict]':
+    async def get_user_audit_logs(self, rotated: bool = True) -> 'AsyncIterator[Dict[str, Any]]':
         '''The User Audit log (aka Actions log) displays all user
         activity on the platform.
         '''
         from .utils import extract_logfiles
         from .parse import cefparse
 
         _, archive = await self.raw_download('monitor/global/userAuditLog')
         async for content in extract_logfiles(archive, 'userAuditSyslog', rotated):
             # yield latest logs first
             for line in content.splitlines()[::-1]:
-                yield cefparse(line.decode())
+                if line is not None:
+                    yield cefparse(line.decode())  # type: ignore
 
     # https://nest.cybereason.com/documentation/api-documentation/all-versions/how-build-queries
     async def query(self, query: 'Dict[str, Any]', parsed: bool = True) -> 'Dict[str, Any]':
         # default since version 20.1.381
         query.setdefault('perGroupLimit', 100)
         if query['perGroupLimit'] > 1000:
             query['perGroupLimit'] = 1000
```

### Comparing `cybereason-0.2.0/src/cybereason/exceptions.py` & `cybereason-0.3.0/src/cybereason/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 log = logging.getLogger(__name__)
 
 
 class CybereasonException(Exception):
     ...
 
 
+class ClientError(CybereasonException):
+    ...
+
+
 class UnauthorizedRequest(CybereasonException):
     def __init__(self, url: str, role: Optional[str] = None) -> None:
         if role:
             msg = f'You must have the {role} role'
         else:
             msg = 'You don\'t have the role required'
 
@@ -30,15 +34,15 @@
     ...
 
 
 class ServerError(CybereasonException):
     ...
 
 
-class ClientError(CybereasonException):
+class TooManyRequests(ClientError):
     ...
 
 
 class ResourceNotFoundError(CybereasonException):
     ...
```

### Comparing `cybereason-0.2.0/src/cybereason/incident_reponse.py` & `cybereason-0.3.0/src/cybereason/incident_reponse.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.2.0/src/cybereason/malops.py` & `cybereason-0.3.0/src/cybereason/malops.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         }
 
         return (await self.post('detection/inbox', data))['malops']
 
     async def get_active_malops(self, logon: bool = False) -> 'AsyncIterator[Dict[str, Any]]':
         '''Get all malops currently active.
         '''
-
         payload = {
             'totalResultLimit': 10000,
             'perGroupLimit':    10000,
             'perFeatureLimit':  100,
             'templateContext':  'OVERVIEW',
             'customFields':     [],
             'queryPath':        [{'result': True, 'filters': None}],
@@ -92,15 +91,15 @@
             msg['message'] = unescape(msg['message'])
         return resp
 
     @min_version(17, 5)
     @authz('Analyst L1')
     async def get_malware_alerts(self, filters=None) -> 'AsyncIterator[Any]':
         data = {'filters': filters or [], 'sortingFieldName': 'timestamp'}
-        async for alert in self.aiter_pages('malware/query', data, key='malwares'):
+        async for alert in self.aiter_pages('malware/query', data, 'malwares', check_resp=True):
             yield alert
 
 # region LABELS
     @min_version(20, 1, 43)
     async def get_malops_labels(
         self, malops_ids: 'Optional[List[MalopId]]' = None
     ) -> 'List[Label]':
@@ -109,16 +108,16 @@
         Args:
             malops_ids: You can add specific Malop GUID identifiers.
         '''
         return await self.post('detection/labels', malops_ids or [])
 
     @min_version(20, 1, 43)
     async def add_malops_label(self, label: str) -> 'Label':
-        '''Add a new malop label to the list of labels available for use
-        to add to malops.
+        '''Adds a new malop label to the list of labels available for
+        use to add to malops.
         '''
         return await self.post('detection/add-label', {'labelText': label})
 
     @min_version(20, 1, 43)
     async def update_malops_labels(
         self,
         malops_ids:     'List[MalopId]',
```

### Comparing `cybereason-0.2.0/src/cybereason/parse/cef.py` & `cybereason-0.3.0/src/cybereason/parse/cef.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.2.0/src/cybereason/parse/server.py` & `cybereason-0.3.0/src/cybereason/parse/server.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.2.0/src/cybereason/sensors.py` & `cybereason-0.3.0/src/cybereason/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 from typing import Optional, Union, Any, TYPE_CHECKING, cast
 from pathlib import Path
 from os import PathLike
 import logging
 import asyncio
 
-from .utils import to_list, unset, get_filename
+from .utils import to_list, get_filename
 from .exceptions import (
     AccessDenied, ServerError, ClientError,
     ResourceExistsError, ResourceNotFoundError,
     authz, min_version,
 )
-from ._typing import CybereasonProtocol
+from ._typing import CybereasonProtocol, unset
 
 if TYPE_CHECKING:
     from typing import AsyncIterator, Dict, List
-    from ._typing import SensorId
-    from .utils import Unset
+    from ._typing import SensorId, Unset, Unforced
 
 
 log = logging.getLogger(__name__)
 
 
 class SensorsMixin(CybereasonProtocol):
     @authz('System Admin')
     async def get_sensors(
         self,
         *, archived: bool = True,
         filters:     'Optional[List[Any]]' = None,
-        page_size:   Optional[int] = None,  # TODO
     ) -> 'AsyncIterator[Dict[str, Any]]':
         '''Returns details on all or a selected group of sensors.
 
         Args:
             archived: show archived sensors.
         '''
-        filters = filters or []
+        data = {'filters': filters or []}
+
         if not archived:
-            filters.append({
+            data['filters'].append({
                 'fieldName': 'status',
-                'operator': 'NotEquals',
-                'values': ['Archived'],
+                'operator':  'NotEquals',
+                'values':    ['Archived'],
             })
 
-        async for sensor in self.aiter_pages(
-            'sensors/query',
-            data={'filters': filters},
-            key='sensors',
-            # page_size=page_size,
-        ):
+        async for sensor in self.aiter_pages('sensors/query', data, 'sensors'):
             yield sensor
 
     @authz('System Admin')
     async def get_sensors_actions(self) -> 'Any':
         '''Returns a list of all the current or queued actions on sensors.
         '''
         return await self.get('sensors/allActions')
@@ -171,18 +165,18 @@
         return resp['groupId']
 
     @min_version(20, 2, 2)
     @authz('System Admin')
     async def edit_group(
         self,
         group_id:    str,
-        name:        'Union[Unset, str]' = unset,
-        description: 'Union[Unset, str]' = unset,
-        rules:       'Union[Unset, List[Dict[str, Any]]]' = unset,
-        policy_id:   'Union[Unset, str]' = unset,
+        name:        'Unforced[str]' = unset,
+        description: 'Unforced[str]' = unset,
+        rules:       'Unforced[List[Dict[str, Any]]]' = unset,
+        policy_id:   'Unforced[str]' = unset,
     ) -> 'Any':
         '''Edits the details of an existing sensor group.
         '''
         group = await self.get_group_by_id(group_id)
         data = {
             'name': group['name'] if name is unset else name,
             'description': group['description'] if description is unset else description,
@@ -425,15 +419,19 @@
         self,
         pylum_id: str,
         filepath: PathLike,
         destdir:  Optional[PathLike] = None,
         extract:  bool = False,
     ) -> Path:
         '''
-        Returns the folder where the archive was downloaded or extracted.
+        Downloads a file from a sensor.
+
+        If ``extract`` is ``True`` returns the folder where the archive
+        was extracted. Otherwise returns the path where the archive was
+        downloaded.
         '''
         from io import BytesIO
 
         destdir = Path('.').resolve() if not destdir else Path(destdir)
 
         if not destdir.exists():
             destdir.mkdir(parents=True)
@@ -461,12 +459,14 @@
             except ImportError:
                 raise RuntimeError('Install as `pip install cybereason[zip]` to'
                                    'allow file extraction.')
 
             with AESZipFile(buffer, mode='r') as archive:
                 # TODO: add drive to target
                 archive.extractall(path=destdir, pwd=b'cautionhandlewithcare')
+
+            return destdir
         else:
             with open(destdir / filename, 'wb') as archive:
                 archive.write(buffer.read())
 
-        return destdir
+            return destdir / filename
```

### Comparing `cybereason-0.2.0/src/cybereason/system.py` & `cybereason-0.3.0/src/cybereason/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,15 @@
 
     async def get_detection_servers(self):
         return await self.get('settings/get-detection-servers')
 
     async def get_registration_config(self):
         # XXX: returns detection servers
         resp = await self.get('settings/configuration/general/get-registration-config')
-        if resp['outcome'] == 'success':
-            return resp['data']
-        else:
-            raise ServerError(resp)
+        return self.check_resp(resp)
 
     async def get_investigation_config(
         self
     ) -> Dict[str, Dict[str, List[Dict[str, Union[str, List[str]]]]]]:
         resp = await self.get('investigation/configuration')
         return resp['configurationModel']
```

### Comparing `cybereason-0.2.0/src/cybereason/threat_intel.py` & `cybereason-0.3.0/src/cybereason/threat_intel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,76 @@
 from typing import TYPE_CHECKING, Any
+from functools import cached_property
 from ipaddress import ip_address
+from datetime import datetime
 from pathlib import Path
 from os import PathLike
 import hashlib
+import asyncio
 
 from ._typing import CybereasonProtocol
 
 if TYPE_CHECKING:
-    from typing import AsyncIterator, Dict, List, Optional
+    from typing import AsyncIterator, Dict, List, Optional, Literal
 
 
 class ThreatIntelligenceMixin(CybereasonProtocol):
 
 # region QUERIES
+    @cached_property
+    def reputation_list(self):
+        async def replist():
+            url = 'dynamic/v1/ti-reputation/api/v1/entity/lists/default'
+            return await self.get(url)
+        return asyncio.run(replist())
+
+    # async def get_custom_reputations(
+    #     self,
+    #     included_expired: bool = False,
+    # ) -> 'AsyncIterator[Dict[str, Any]]':
+    #     '''Returns a list of custom reputations for files, IP addresses,
+    #     and domain names.
+    #     '''
+    #     url = 'classification/reputations/list'
+    #     data = {'filter': {'includeExpired': included_expired}}
+    #     async for x in self.aiter_items(url, data, 'reputations', check_resp=True):
+    #         yield x
+
+    async def get_reputations(self) -> 'AsyncIterator[Dict[str, Any]]':
+        url = f'dynamic/v1/ti-reputation/api/v1/lists/{self.reputation_list}/reputations/search'
+        async for x in self.aiter_items(url, {}, 'reputations', pagination=True):
+            yield x
+
+    async def update_reputation(
+        self,
+        id:         int,
+        *, comment: str,
+        action:     'Literal["ALLOW", "DENY"]',
+        keys:       'List[Dict[str, str]]',
+        groups:     'Optional[List[str]]' = None,
+        expiration: 'Optional[datetime]' = None,
+    ) -> 'Dict[str, Any]':
+        '''
+        Args:
+            groups: ``None`` means "Global".
+        '''
+        data = {
+            'comment':          comment,
+            'action':           action,
+            'keys':             keys,
+            'groupIds':         groups,
+            'reputationListId': self.reputation_list,
+        }
+        # TODO: remove expiration?
+        if expiration is not None:
+            data['expiresAt'] = int(expiration.timestamp() * 1000)
+
+        url = f'dynamic/v1/ti-reputation/api/v1/lists/{self.reputation_list}/reputations/{id}'
+        return await self.put(url, data)
+
     async def get_file_reputation(self, path: PathLike, use_sha1: bool = True) -> Any:
         '''Returns details on a file’s reputation based on the threat
         intelligence service.
 
         Args:
             path: path to the file.
             use_sha1: if ``True`` uses SHA-1 to hash the file. Otherwise
@@ -129,34 +183,8 @@
     async def get_domain_reputations(self) -> Any:
         '''Returns a list of all domain reputations used by the threat
         intelligence service.
         '''
         from warnings import warn
         warn("'get_domain_reputations' is deprecated", DeprecationWarning)
         return await self.post_sage('download_v1/domain_reputation', {})
-
-    # XXX: broken: commas not escaped, `None` and `` in boolean fields...
-    async def get_reputations(
-        self,
-        reputation: 'Optional[str]' = None,
-    ) -> 'AsyncIterator[Dict[str, Any]]':
-        '''Returns a list of custom reputations for files, IP addresses,
-        and domain names.
-
-        Args:
-            reputation: 'blacklist' or 'whitelist'.
-        '''
-        from .utils import parse_csv
-
-        # TODO: could be reputation filtered in the query?
-        csv = await self.get('classification/download')
-
-        for item in parse_csv(
-            csv,
-            boolean=['prevent execution', 'remove'],
-            optional=['comment'],
-        ):
-            if not reputation:
-                yield item
-            elif item['reputation'] == reputation:
-                yield item
 # endregion
```

### Comparing `cybereason-0.2.0/src/cybereason/utils/__init__.py` & `cybereason-0.3.0/src/cybereason/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,14 @@
     from httpx import Response
 
 
 BOOL = {'true': True, 'false': False}
 NONE = {'null': None}
 
 
-class Unset:
-    def __bool__(self):
-        return False
-
-    def __contains__(self, o):
-        return False
-
-
-unset = Unset()
-
-
 def parse_csv(
     text:       str,
     *, boolean: 'List[str]' = [],
     optional:   'List[str]' = [],
 ) -> 'Iterator[Dict[str, Any]]':
     csv = text.splitlines()
 
@@ -38,15 +27,15 @@
         for key in boolean:
             item[key] = BOOL[item[key]]  # type: ignore
         for key in optional:
             item[key] = NONE.get(item[key], item[key])  # type: ignore
         yield item
 
 
-def to_list(obj: 'Any') -> 'List[Any]':
+def to_list(obj: 'Any') -> 'Iterable[Any]':
     if isinstance(obj, Iterator):
         return list(obj)
     elif isinstance(obj, Iterable):
         if not isinstance(obj, (str, bytes)):
             return obj
     return [obj]
```

### Comparing `cybereason-0.2.0/src/cybereason/utils/guid.py` & `cybereason-0.3.0/src/cybereason/utils/guid.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.2.0/src/cybereason.egg-info/PKG-INFO` & `cybereason-0.3.0/src/cybereason.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.2.0
+Version: 0.3.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.2.0 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.3.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
```

### Comparing `cybereason-0.2.0/src/cybereason.egg-info/SOURCES.txt` & `cybereason-0.3.0/src/cybereason.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 LICENSE
 setup.cfg
 setup.py
 src/cybereason/__init__.py
-src/cybereason/_patch.py
 src/cybereason/_typing.py
 src/cybereason/client.py
-src/cybereason/custom_rules.py
 src/cybereason/exceptions.py
 src/cybereason/incident_reponse.py
 src/cybereason/malops.py
 src/cybereason/py.typed
+src/cybereason/rules.py
 src/cybereason/sensors.py
 src/cybereason/system.py
 src/cybereason/threat_intel.py
 src/cybereason.egg-info/PKG-INFO
 src/cybereason.egg-info/SOURCES.txt
 src/cybereason.egg-info/dependency_links.txt
 src/cybereason.egg-info/not-zip-safe
```

