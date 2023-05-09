# Comparing `tmp/pylink-square-1.0.0.tar.gz` & `tmp/pylink-square-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylink-square-1.0.0.tar", last modified: Thu Dec  8 19:26:01 2022, max compression
+gzip compressed data, was "pylink-square-1.1.0.tar", last modified: Tue May  9 16:00:42 2023, max compression
```

## Comparing `pylink-square-1.0.0.tar` & `pylink-square-1.1.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.942315 pylink-square-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    13680 2022-12-08 19:25:26.000000 pylink-square-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2022-12-08 19:25:26.000000 pylink-square-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2022-12-08 19:25:26.000000 pylink-square-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2022-12-08 19:26:01.942315 pylink-square-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2022-12-08 19:25:26.000000 pylink-square-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.926314 pylink-square-1.0.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5562 2022-12-08 19:25:26.000000 pylink-square-1.0.0/examples/pylink-rtt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3202 2022-12-08 19:25:26.000000 pylink-square-1.0.0/examples/pylink-swv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/pylink/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20657 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/binpacker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    21561 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   168408 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/jlock.py
--rw-r--r--   0 runner    (1001) docker     (123)    21633 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/pylink/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/protocols/swd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)    38009 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/pylink/unlockers/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/unlockers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/unlockers/unlock_kinetis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2022-12-08 19:25:26.000000 pylink-square-1.0.0/pylink/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/pylink_square.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2022-12-08 19:26:01.000000 pylink-square-1.0.0/pylink_square.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2022-12-08 19:26:01.000000 pylink-square-1.0.0/pylink_square.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 19:26:01.000000 pylink-square-1.0.0/pylink_square.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-08 19:26:01.000000 pylink-square-1.0.0/pylink_square.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-08 19:26:01.000000 pylink-square-1.0.0/pylink_square.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-08 19:26:01.000000 pylink-square-1.0.0/pylink_square.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-08 19:26:01.942315 pylink-square-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2022-12-08 19:25:26.000000 pylink-square-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.930314 pylink-square-1.0.0/tests/functional/features/
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/features/jlink/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/canary.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/debugger.feature
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/emulator.feature
--rw-r--r--   0 runner    (1001) docker     (123)      629 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/flash.feature
--rw-r--r--   0 runner    (1001) docker     (123)      659 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/license.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/memory.feature
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/register.feature
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/rtt.feature
--rw-r--r--   0 runner    (1001) docker     (123)      583 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/swd.feature
--rw-r--r--   0 runner    (1001) docker     (123)      462 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/swo.feature
--rw-r--r--   0 runner    (1001) docker     (123)      381 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/unlock.feature
--rw-r--r--   0 runner    (1001) docker     (123)      403 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/jlink/update.feature
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/features/steps/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/registers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/rtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/swd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/swo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/steps/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/features/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.922315 pylink-square-1.0.0/tests/functional/firmware/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/firmware/k21-canary/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-canary/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-canary/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      766 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-canary/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/firmware/k21-canary/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-canary/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-canary/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/firmware/k21-canary/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-canary/src/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/firmware/k21-etm/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      559 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/firmware/k21-etm/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.934315 pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/etm.c
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/etm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/swo.c
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/swo.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-loop/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-loop/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-loop/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-loop/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-loop/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-loop/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-loop/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-loop/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-loop/src/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      661 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/src/main.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    53176 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h
--rw-r--r--   0 runner    (1001) docker     (123)    19789 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-swd/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swd/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swd/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swd/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/gcc.ld
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/main.s
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-swo/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/.gdbinit
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      577 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-swo/asm/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/asm/bootloader.s
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/asm/gcc.ld
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.938315 pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/swo.c
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/swo.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.942315 pylink-square-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.942315 pylink-square-1.0.0/tests/unit/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/protocols/test_swd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_binpacker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)   197978 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_jlock.py
--rw-r--r--   0 runner    (1001) docker     (123)    41451 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    25414 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 19:26:01.942315 pylink-square-1.0.0/tests/unit/unlockers/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/unlockers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/unlockers/test_unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2022-12-08 19:25:26.000000 pylink-square-1.0.0/tests/unit/unlockers/test_unlock_kinetis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-09 16:00:12.000000 pylink-square-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-09 16:00:12.000000 pylink-square-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-09 16:00:12.000000 pylink-square-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-09 16:00:42.781110 pylink-square-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-09 16:00:12.000000 pylink-square-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.769110 pylink-square-1.1.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5563 2023-05-09 16:00:12.000000 pylink-square-1.1.0/examples/pylink-rtt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3202 2023-05-09 16:00:12.000000 pylink-square-1.1.0/examples/pylink-swv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20657 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/binpacker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168513 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/jlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/protocols/swd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38009 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink/unlockers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/unlockers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/unlockers/unlock_kinetis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-09 16:00:12.000000 pylink-square-1.1.0/pylink/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/pylink_square.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 16:00:42.000000 pylink-square-1.1.0/pylink_square.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-09 16:00:42.781110 pylink-square-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-09 16:00:12.000000 pylink-square-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/functional/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.773110 pylink-square-1.1.0/tests/functional/features/jlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/canary.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/debugger.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/emulator.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/flash.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/license.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/memory.feature
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/register.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/rtt.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/swd.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/swo.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/unlock.feature
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/jlink/update.feature
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/features/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/registers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/rtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/swd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/swo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/unlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/steps/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/features/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.769110 pylink-square-1.1.0/tests/functional/firmware/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-canary/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-canary/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-canary/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-etm/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-loop/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-loop/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-loop/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/src/main.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    53176 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swd/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/gcc.ld
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/main.s
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swo/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/.gdbinit
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.777110 pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/bootloader.s
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/gcc.ld
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/unit/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/protocols/test_swd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_binpacker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197978 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_jlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_jlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41451 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25414 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:00:42.781110 pylink-square-1.1.0/tests/unit/unlockers/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/unlockers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/unlockers/test_unlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-09 16:00:12.000000 pylink-square-1.1.0/tests/unit/unlockers/test_unlock_kinetis.py
```

### Comparing `pylink-square-1.0.0/CHANGELOG.md` & `pylink-square-1.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
+## [1.1.0]
+### Added
+- @chanqueo: Added `use_tmpcpy` field to constructor for `JLink` and `Library`
+  instances to workaround temporary files not been cleaned up; a future patch
+  will change the default behaviour based on the version of the SDK. By
+  default, temporary files are used for the SDK binary.
+
+### Changed
+- @curtishx: Changed decorator on `set_reset_strategy()` from
+  `@connection_required` to `@open_required`.
+
+### Removed
+- @avi-jois: Removed dependency on `future`.
+
 ## [1.0.0]
 
 ### Changed
 - @boraozgen: Fixed installation error that prevented `setup.py install` when
   `six` was not installed.
 - @denravonska: Changed `.flash()` to no longer erase chip on flash; users will
   now need to ensure they call `.erase()` prior to flashing a non-erased region
```

### Comparing `pylink-square-1.0.0/LICENSE.md` & `pylink-square-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/PKG-INFO` & `pylink-square-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylink-square
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python interface for SEGGER J-Link.
 Home-page: http://www.github.com/Square/pylink
 Author: Square Embedded Software Team
 Author-email: esw-team@squareup.com
 License: Apache 2.0
 Keywords: SEGGER J-Link
 License-File: LICENSE.md
```

### Comparing `pylink-square-1.0.0/README.md` & `pylink-square-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/examples/pylink-rtt` & `pylink-square-1.1.0/examples/pylink-rtt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Date: October 11, 2017
 # Copyright: 2017 Square, Inc.
 
 import pylink
 import argparse
 import sys
 import time
-from builtins import input
+from six.moves import input
 
 try:
     import thread
 except ImportError:
     import _thread as thread
```

### Comparing `pylink-square-1.0.0/examples/pylink-swv` & `pylink-square-1.1.0/examples/pylink-swv`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/__init__.py` & `pylink-square-1.1.0/pylink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __title__ = 'pylink'
 __author__ = 'Square Embedded Software Team'
 __author_email__ = 'esw-team@squareup.com'
 __copyright__ = 'Copyright 2017 Square, Inc.'
 __license__ = 'Apache 2.0'
 __url__ = 'http://www.github.com/Square/pylink'
 __description__ = 'Python interface for SEGGER J-Link.'
```

### Comparing `pylink-square-1.0.0/pylink/__main__.py` & `pylink-square-1.1.0/pylink/__main__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/binpacker.py` & `pylink-square-1.1.0/pylink/binpacker.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/decorators.py` & `pylink-square-1.1.0/pylink/decorators.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/enums.py` & `pylink-square-1.1.0/pylink/enums.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/errors.py` & `pylink-square-1.1.0/pylink/errors.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/jlink.py` & `pylink-square-1.1.0/pylink/jlink.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
                 if self.tif != interface:
                     raise errors.JLinkException('Unsupported for current interface.')
                 return func(self, *args, **kwargs)
             return wrapper
         return _interface_required
 
     def __init__(self, lib=None, log=None, detailed_log=None, error=None, warn=None, unsecure_hook=None,
-                 serial_no=None, ip_addr=None, open_tunnel=False):
+                 serial_no=None, ip_addr=None, open_tunnel=False, use_tmpcpy=True):
         """Initializes the J-Link interface object.
 
         Note:
           By default, the unsecure dialog will reject unsecuring the device on
           connection.  If you wish to change this behaviour (to have the device
           be unsecured and erased), pass a callback that returns
           ``JLinkFlags.DLG_BUTTON_YES`` as its return value.
@@ -275,25 +275,26 @@
           open_tunnel (bool, None): If ``False`` (default), the ``open``
             method will be called when entering the context manager using
             the ``serial_no`` and ``ip_addr`` provided here.
             If ``True`` ``open_tunnel`` method will be called instead
             of ``open`` method.
             If ``None``, the driver will not be opened automatically
             (however, it is still closed when exiting the context manager).
+          use_tmpcpy (bool): True to load a temporary copy of J-Link DLL
 
         Returns:
           ``None``
 
         Raises:
           TypeError: if lib's DLL is ``None``
         """
         self._initialized = False
 
         if lib is None:
-            lib = library.Library()
+            lib = library.Library(use_tmpcpy=use_tmpcpy)
 
         if lib.dll() is None:
             raise TypeError('Expected to be given a valid DLL.')
 
         self._library = lib
         self._dll = lib.dll()
         self._tif = enums.JLinkInterfaces.JTAG
@@ -1957,15 +1958,15 @@
           self (JLink): the ``JLink`` instance.
 
         Returns:
           ``None``
         """
         return self.set_trace_source(enums.JLinkTraceSource.ETM)
 
-    @connection_required
+    @open_required
     def set_reset_strategy(self, strategy):
         """Sets the reset strategy for the target.
 
         The reset strategy defines what happens when the target is reset.
 
         Args:
           self (JLink): the ``JLink`` instance
```

### Comparing `pylink-square-1.0.0/pylink/jlock.py` & `pylink-square-1.1.0/pylink/jlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/library.py` & `pylink-square-1.1.0/pylink/library.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,32 +256,34 @@
 
                 # For versions >= 5.0.0 and < 6.0.0, there is no strictly
                 # linked library file, so try and find the versioned one.
                 for f in files:
                     if f.startswith(dll):
                         yield os.path.join(dir_path, f)
 
-    def __init__(self, dllpath=None):
+    def __init__(self, dllpath=None, use_tmpcpy=True):
         """Initializes an instance of a ``Library``.
 
         Loads the default J-Link DLL if ``dllpath`` is ``None``, otherwise
         loads the DLL specified by the given ``dllpath``.
 
         Args:
           self (Library): the ``Library`` instance
           dllpath (str): the DLL to load into the library
+          use_tmpcpy (bool): True to load a temporary copy of J-Link DLL
 
         Returns:
           ``None``
         """
         self._lib = None
         self._winlib = None
         self._path = None
         self._windows = sys.platform.startswith('win')
         self._cygwin = sys.platform.startswith('cygwin')
+        self._use_tmpcpy = use_tmpcpy
         self._temp = None
 
         if self._windows or self._cygwin:
             self._sdk = self.get_appropriate_windows_sdk_name()
         else:
             self._sdk = self.JLINK_SDK_OBJECT
 
@@ -383,36 +385,41 @@
         if self._windows or self._cygwin:
             suffix = '.dll'
         elif sys.platform.startswith('darwin'):
             suffix = '.dylib'
         else:
             suffix = '.so'
 
-        # Copy the J-Link DLL to a temporary file.  This will be cleaned up the
-        # next time we load a DLL using this library or if this library is
-        # cleaned up.
-        tf = tempfile.NamedTemporaryFile(delete=False, suffix=suffix)
-        with open(tf.name, 'wb') as outputfile:
-            with open(self._path, 'rb') as inputfile:
-                outputfile.write(inputfile.read())
-
-        # This is needed to work around a WindowsError where the file is not
-        # being properly cleaned up after exiting the with statement.
-        tf.close()
+        lib_path = self._path
 
-        self._temp = tf
-        self._lib = ctypes.cdll.LoadLibrary(tf.name)
+        if self._use_tmpcpy:
+            # Copy the J-Link DLL to a temporary file.  This will be cleaned up the
+            # next time we load a DLL using this library or if this library is
+            # cleaned up.
+            tf = tempfile.NamedTemporaryFile(delete=False, suffix=suffix)
+            with open(tf.name, 'wb') as outputfile:
+                with open(self._path, 'rb') as inputfile:
+                    outputfile.write(inputfile.read())
+
+            # This is needed to work around a WindowsError where the file is not
+            # being properly cleaned up after exiting the with statement.
+            tf.close()
+
+            lib_path = tf.name
+            self._temp = tf
+
+        self._lib = ctypes.cdll.LoadLibrary(lib_path)
 
         if self._windows:
             # The J-Link library uses a mix of __cdecl and __stdcall function
             # calls.  While this is fine on a nix platform or in cygwin, this
             # causes issues with Windows, where it expects the __stdcall
             # methods to follow the standard calling convention.  As a result,
             # we have to convert them to windows function calls.
-            self._winlib = ctypes.windll.LoadLibrary(tf.name)
+            self._winlib = ctypes.windll.LoadLibrary(lib_path)
             for stdcall in self._standard_calls_:
                 if hasattr(self._winlib, stdcall):
                     # Backwards compatibility.  Some methods do not exist on
                     # older versions of the J-Link firmware, so ignore them in
                     # these cases.
                     setattr(self._lib, stdcall, getattr(self._winlib, stdcall))
         return True
```

### Comparing `pylink-square-1.0.0/pylink/protocols/__init__.py` & `pylink-square-1.1.0/pylink/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/protocols/swd.py` & `pylink-square-1.1.0/pylink/protocols/swd.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/registers.py` & `pylink-square-1.1.0/pylink/registers.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/structs.py` & `pylink-square-1.1.0/pylink/structs.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/threads.py` & `pylink-square-1.1.0/pylink/threads.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/unlockers/__init__.py` & `pylink-square-1.1.0/pylink/unlockers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/unlockers/unlock_kinetis.py` & `pylink-square-1.1.0/pylink/unlockers/unlock_kinetis.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink/util.py` & `pylink-square-1.1.0/pylink/util.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/pylink_square.egg-info/PKG-INFO` & `pylink-square-1.1.0/pylink_square.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylink-square
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python interface for SEGGER J-Link.
 Home-page: http://www.github.com/Square/pylink
 Author: Square Embedded Software Team
 Author-email: esw-team@squareup.com
 License: Apache 2.0
 Keywords: SEGGER J-Link
 License-File: LICENSE.md
```

### Comparing `pylink-square-1.0.0/pylink_square.egg-info/SOURCES.txt` & `pylink-square-1.1.0/pylink_square.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/setup.py` & `pylink-square-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,14 @@
         'pylink': [
         ]
     },
 
     # Dependencies.
     install_requires=[
         'psutil >= 5.2.2',
-        'future',
         'six'
     ],
 
     # Tests
     test_suite='tests',
 
     # Test requirements
```

### Comparing `pylink-square-1.0.0/tests/README.md` & `pylink-square-1.1.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/__init__.py` & `pylink-square-1.1.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/__init__.py` & `pylink-square-1.1.0/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/environment.py` & `pylink-square-1.1.0/tests/functional/features/environment.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/debugger.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/debugger.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/emulator.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/emulator.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/flash.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/flash.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/license.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/license.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/memory.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/memory.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/register.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/register.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/rtt.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/rtt.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/jlink/swd.feature` & `pylink-square-1.1.0/tests/functional/features/jlink/swd.feature`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/__init__.py` & `pylink-square-1.1.0/tests/functional/features/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/common.py` & `pylink-square-1.1.0/tests/functional/features/steps/common.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/debug.py` & `pylink-square-1.1.0/tests/functional/features/steps/debug.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/licenses.py` & `pylink-square-1.1.0/tests/functional/features/steps/licenses.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/memory.py` & `pylink-square-1.1.0/tests/functional/features/steps/memory.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/registers.py` & `pylink-square-1.1.0/tests/functional/features/steps/registers.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/rtt.py` & `pylink-square-1.1.0/tests/functional/features/steps/rtt.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/swd.py` & `pylink-square-1.1.0/tests/functional/features/steps/swd.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/swo.py` & `pylink-square-1.1.0/tests/functional/features/steps/swo.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/unlock.py` & `pylink-square-1.1.0/tests/functional/features/steps/unlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/steps/update.py` & `pylink-square-1.1.0/tests/functional/features/steps/update.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/features/utility.py` & `pylink-square-1.1.0/tests/functional/features/utility.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-canary/Makefile` & `pylink-square-1.1.0/tests/functional/firmware/k21-canary/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-canary/README.md` & `pylink-square-1.1.0/tests/functional/firmware/k21-canary/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-canary/asm/bootloader.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-canary/asm/gcc.ld` & `pylink-square-1.1.0/tests/functional/firmware/k21-canary/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-canary/src/main.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-canary/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/Makefile` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/README.md` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/asm/bootloader.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/asm/gcc.ld` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/etm.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/etm.h` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/etm.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/main.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/swo.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-etm/src/swo.h` & `pylink-square-1.1.0/tests/functional/firmware/k21-etm/src/swo.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-loop/Makefile` & `pylink-square-1.1.0/tests/functional/firmware/k21-loop/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-loop/asm/bootloader.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-loop/asm/gcc.ld` & `pylink-square-1.1.0/tests/functional/firmware/k21-loop/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-loop/src/main.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-loop/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/Makefile` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/README.md` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/asm/bootloader.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/asm/gcc.ld` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/src/main.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_Conf.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-rtt/vendor/SEGGER_RTT_printf.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swd/Makefile` & `pylink-square-1.1.0/tests/functional/firmware/k21-swd/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swd/README.md` & `pylink-square-1.1.0/tests/functional/firmware/k21-swd/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/bootloader.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/gcc.ld` & `pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swd/asm/main.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-swd/asm/main.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/Makefile` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/Makefile`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/README.md` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/README.md`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/asm/bootloader.s` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/bootloader.s`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/asm/gcc.ld` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/asm/gcc.ld`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/main.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/main.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/swo.c` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.c`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/functional/firmware/k21-swo/src/swo.h` & `pylink-square-1.1.0/tests/functional/firmware/k21-swo/src/swo.h`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/__init__.py` & `pylink-square-1.1.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/protocols/__init__.py` & `pylink-square-1.1.0/tests/unit/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/protocols/test_swd.py` & `pylink-square-1.1.0/tests/unit/protocols/test_swd.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_binpacker.py` & `pylink-square-1.1.0/tests/unit/test_binpacker.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_decorators.py` & `pylink-square-1.1.0/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_enums.py` & `pylink-square-1.1.0/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_errors.py` & `pylink-square-1.1.0/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_jlink.py` & `pylink-square-1.1.0/tests/unit/test_jlink.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_jlock.py` & `pylink-square-1.1.0/tests/unit/test_jlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_library.py` & `pylink-square-1.1.0/tests/unit/test_library.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_main.py` & `pylink-square-1.1.0/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_structs.py` & `pylink-square-1.1.0/tests/unit/test_structs.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_threads.py` & `pylink-square-1.1.0/tests/unit/test_threads.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/test_util.py` & `pylink-square-1.1.0/tests/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/unlockers/__init__.py` & `pylink-square-1.1.0/tests/unit/unlockers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/unlockers/test_unlock.py` & `pylink-square-1.1.0/tests/unit/unlockers/test_unlock.py`

 * *Files identical despite different names*

### Comparing `pylink-square-1.0.0/tests/unit/unlockers/test_unlock_kinetis.py` & `pylink-square-1.1.0/tests/unit/unlockers/test_unlock_kinetis.py`

 * *Files identical despite different names*

