# Comparing `tmp/openpgpcard-x25519-agent-1.0.0.tar.gz` & `tmp/openpgpcard-x25519-agent-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpgpcard-x25519-agent-1.0.0.tar", last modified: Mon Mar 13 21:15:23 2023, max compression
+gzip compressed data, was "openpgpcard-x25519-agent-1.0.1.tar", last modified: Tue May  9 21:27:03 2023, max compression
```

## Comparing `openpgpcard-x25519-agent-1.0.0.tar` & `openpgpcard-x25519-agent-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-13 21:15:23.964481 openpgpcard-x25519-agent-1.0.0/
--rw-rw-r--   0 justin    (1000) justin    (1000)      260 2023-03-13 21:13:13.000000 openpgpcard-x25519-agent-1.0.0/.build.yml
--rw-r--r--   0 justin    (1000) justin    (1000)      420 2023-02-08 06:25:10.000000 openpgpcard-x25519-agent-1.0.0/.editorconfig
--rw-rw-r--   0 justin    (1000) justin    (1000)      566 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.0/.gitignore
--rw-rw-r--   0 justin    (1000) justin    (1000)     1771 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 justin    (1000) justin    (1000)    32473 2023-02-08 06:26:50.000000 openpgpcard-x25519-agent-1.0.0/LICENSE
--rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-03-13 21:15:23.964481 openpgpcard-x25519-agent-1.0.0/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     3679 2023-03-13 20:44:52.000000 openpgpcard-x25519-agent-1.0.0/README.md
--rw-rw-r--   0 justin    (1000) justin    (1000)      607 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.0/coveragerc
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-13 21:15:23.956475 openpgpcard-x25519-agent-1.0.0/etc/
--rw-rw-r--   0 justin    (1000) justin    (1000)     2356 2023-03-04 23:50:44.000000 openpgpcard-x25519-agent-1.0.0/etc/openpgpcard-x25519-agent.service
--rw-rw-r--   0 justin    (1000) justin    (1000)      246 2023-03-05 02:52:53.000000 openpgpcard-x25519-agent-1.0.0/etc/openpgpcard-x25519-agent.socket
--rwxrwxr-x   0 justin    (1000) justin    (1000)     1435 2023-03-05 03:10:33.000000 openpgpcard-x25519-agent-1.0.0/install.sh
--rw-rw-r--   0 justin    (1000) justin    (1000)      254 2023-02-08 01:50:04.000000 openpgpcard-x25519-agent-1.0.0/pyproject.toml
--rw-rw-r--   0 justin    (1000) justin    (1000)     2157 2023-03-13 21:15:23.964481 openpgpcard-x25519-agent-1.0.0/setup.cfg
--rw-rw-r--   0 justin    (1000) justin    (1000)      557 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.0/setup.py
--rw-rw-r--   0 justin    (1000) justin    (1000)      400 2023-02-28 02:25:14.000000 openpgpcard-x25519-agent-1.0.0/spellcheck-dictionary.txt
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-13 21:15:23.952471 openpgpcard-x25519-agent-1.0.0/src/
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-13 21:15:23.960478 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/
--rw-rw-r--   0 justin    (1000) justin    (1000)      466 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/__init__.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    13632 2023-03-08 00:13:39.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/card.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     2487 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    11252 2023-02-28 02:42:11.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/client.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     4980 2023-02-28 02:56:43.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/client_cli.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1748 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    28646 2023-03-03 23:17:32.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/msg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    12987 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/server.py
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-13 21:15:23.960478 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/
--rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-03-13 21:15:23.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1000) justin    (1000)     1027 2023-03-13 21:15:23.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-03-13 21:15:23.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)      148 2023-03-13 21:15:23.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/entry_points.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-02-08 01:29:53.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/not-zip-safe
--rw-rw-r--   0 justin    (1000) justin    (1000)      141 2023-03-13 21:15:23.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/requires.txt
--rw-rw-r--   0 justin    (1000) justin    (1000)       25 2023-03-13 21:15:23.000000 openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/top_level.txt
-drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-03-13 21:15:23.964481 openpgpcard-x25519-agent-1.0.0/tests/
--rw-rw-r--   0 justin    (1000) justin    (1000)     1332 2023-02-16 05:43:01.000000 openpgpcard-x25519-agent-1.0.0/tests/conftest.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    13586 2023-03-08 00:13:42.000000 openpgpcard-x25519-agent-1.0.0/tests/test_card.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    17671 2023-02-28 02:36:18.000000 openpgpcard-x25519-agent-1.0.0/tests/test_client.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     3225 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.0/tests/test_cnf.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    23775 2023-02-28 02:10:34.000000 openpgpcard-x25519-agent-1.0.0/tests/test_msg.py
--rw-rw-r--   0 justin    (1000) justin    (1000)    16878 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.0/tests/test_server.py
--rw-rw-r--   0 justin    (1000) justin    (1000)     1885 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.0/tox.ini
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.568908 openpgpcard-x25519-agent-1.0.1/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      260 2023-05-09 21:16:06.000000 openpgpcard-x25519-agent-1.0.1/.build.yml
+-rw-r--r--   0 justin    (1000) justin    (1000)      420 2023-02-08 06:25:10.000000 openpgpcard-x25519-agent-1.0.1/.editorconfig
+-rw-rw-r--   0 justin    (1000) justin    (1000)      566 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.1/.gitignore
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1771 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.1/.pre-commit-config.yaml
+-rw-rw-r--   0 justin    (1000) justin    (1000)    32473 2023-02-08 06:26:50.000000 openpgpcard-x25519-agent-1.0.1/LICENSE
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-05-09 21:27:03.568908 openpgpcard-x25519-agent-1.0.1/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3679 2023-03-13 20:44:52.000000 openpgpcard-x25519-agent-1.0.1/README.md
+-rw-rw-r--   0 justin    (1000) justin    (1000)      607 2023-02-07 22:50:35.000000 openpgpcard-x25519-agent-1.0.1/coveragerc
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.560903 openpgpcard-x25519-agent-1.0.1/etc/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2356 2023-03-04 23:50:44.000000 openpgpcard-x25519-agent-1.0.1/etc/openpgpcard-x25519-agent.service
+-rw-rw-r--   0 justin    (1000) justin    (1000)      246 2023-03-05 02:52:53.000000 openpgpcard-x25519-agent-1.0.1/etc/openpgpcard-x25519-agent.socket
+-rwxrwxr-x   0 justin    (1000) justin    (1000)     1435 2023-03-05 03:10:33.000000 openpgpcard-x25519-agent-1.0.1/install.sh
+-rw-rw-r--   0 justin    (1000) justin    (1000)      254 2023-02-08 01:50:04.000000 openpgpcard-x25519-agent-1.0.1/pyproject.toml
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2157 2023-05-09 21:27:03.568908 openpgpcard-x25519-agent-1.0.1/setup.cfg
+-rw-rw-r--   0 justin    (1000) justin    (1000)      557 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.1/setup.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)      404 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.1/spellcheck-dictionary.txt
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.556900 openpgpcard-x25519-agent-1.0.1/src/
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.564905 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/
+-rw-rw-r--   0 justin    (1000) justin    (1000)      466 2023-02-08 05:47:24.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/__init__.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    14520 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/card.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     2487 2023-02-28 02:10:35.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    11252 2023-02-28 02:42:11.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4980 2023-02-28 02:56:43.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client_cli.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1748 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    28646 2023-03-03 23:17:32.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/msg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    12987 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/server.py
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.564905 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     4692 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1027 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)      148 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)        1 2023-02-08 01:29:53.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 justin    (1000) justin    (1000)      141 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1000) justin    (1000)       25 2023-05-09 21:27:03.000000 openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/top_level.txt
+drwxrwxr-x   0 justin    (1000) justin    (1000)        0 2023-05-09 21:27:03.564905 openpgpcard-x25519-agent-1.0.1/tests/
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1332 2023-02-16 05:43:01.000000 openpgpcard-x25519-agent-1.0.1/tests/conftest.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    15254 2023-05-09 21:16:23.000000 openpgpcard-x25519-agent-1.0.1/tests/test_card.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    17671 2023-02-28 02:36:18.000000 openpgpcard-x25519-agent-1.0.1/tests/test_client.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     3225 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/tests/test_cnf.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    23775 2023-02-28 02:10:34.000000 openpgpcard-x25519-agent-1.0.1/tests/test_msg.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)    16878 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/tests/test_server.py
+-rw-rw-r--   0 justin    (1000) justin    (1000)     1885 2023-02-28 02:10:36.000000 openpgpcard-x25519-agent-1.0.1/tox.ini
```

### Comparing `openpgpcard-x25519-agent-1.0.0/.gitignore` & `openpgpcard-x25519-agent-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/.pre-commit-config.yaml` & `openpgpcard-x25519-agent-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/LICENSE` & `openpgpcard-x25519-agent-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/PKG-INFO` & `openpgpcard-x25519-agent-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpgpcard-x25519-agent
-Version: 1.0.0
+Version: 1.0.1
 Summary: Socket interface to Curve25519 ECDH from an OpenPGP card.
 Home-page: https://git.sr.ht/~arx10/openpgpcard-x25519-agent
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: GPL-3.0-or-later
 Project-URL: Mailing List, https://lists.sr.ht/~arx10/openpgpcard-x25519-agent
 Project-URL: Source, https://git.sr.ht/~arx10/openpgpcard-x25519-agent
```

### Comparing `openpgpcard-x25519-agent-1.0.0/README.md` & `openpgpcard-x25519-agent-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/coveragerc` & `openpgpcard-x25519-agent-1.0.1/coveragerc`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/etc/openpgpcard-x25519-agent.service` & `openpgpcard-x25519-agent-1.0.1/etc/openpgpcard-x25519-agent.service`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/install.sh` & `openpgpcard-x25519-agent-1.0.1/install.sh`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/setup.cfg` & `openpgpcard-x25519-agent-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/setup.py` & `openpgpcard-x25519-agent-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/card.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/card.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,20 +195,24 @@
         PGPCardException: If the command fails.
     """
     length = len(data) if data else 0
     command = [class_byte, instruction, parameter_1, parameter_2, length]
     if data:
         command[6:] = data
 
-    _log_command(class_byte, instruction, parameter_1, parameter_2, length)
     result, status_1, status_2 = _send_command_and_zero(card, command)
-    _log_response(status_1, status_2, len(result))
+    while status_1 == 0x61 and status_2 != 0x00:
+        result, status_1, status_2 = _append_get_response(
+            card, class_byte, result, status_2
+        )
 
-    if status_1 != 0x90 or status_2 != 0x00:
+    if status_1 not in (0x61, 0x90) or status_2 != 0x00:
+        result[:] = bytearray(len(result))
         raise PGPCardException(status_1, status_2)
+
     return result
 
 
 def _log_command(cla, ins, p1, p2, lc):  # noqa: SC200
     s = "sending command to card: %x %x %x %x + %x bytes"
     getLogger(__name__).debug(s, cla, ins, p1, p2, lc)  # noqa: SC200
 
@@ -216,19 +220,40 @@
 def _log_response(sw1, sw2, length):  # noqa: SC200
     s = "received response from card: %x %x + %x bytes"
     getLogger(__name__).debug(s, sw1, sw2, length)  # noqa: SC200
 
 
 def _send_command_and_zero(card, command):
     try:
-        return card.connection.transmit(command)
+        _log_command(*command[:5])
+        result, status_1, status_2 = card.connection.transmit(command)
+        _log_response(status_1, status_2, len(result))
+        return result, status_1, status_2
     finally:
         command[:] = [0] * len(command)
 
 
+def _append_get_response(card, class_byte, previous_result, expected_length):
+    command = [class_byte, 0xC0, 0x00, 0x00, expected_length]
+    result, status_1, status_2 = _send_command_and_zero(card, command)
+
+    previous_result_length = len(previous_result)
+    if previous_result_length == 0:
+        return result, status_1, status_2
+
+    result_length = len(result)
+    if result_length == 0:
+        return previous_result, status_1, status_2
+
+    full_result = previous_result + result
+    previous_result[:] = bytearray(previous_result_length)
+    result[:] = bytearray(result_length)
+    return full_result, status_1, status_2
+
+
 def verify_pin(card, pin, slot=ENCRYPTION_PIN):
     """Submits the specified pin to the specified card for verification.
 
     If the PIN is valid, succeeds. If the PIN is invalid (or blocked),
     will raise a `PinException` with the number of retries left for the PIN.
 
     Arguments:
```

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/cli.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cli.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/client.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/client_cli.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/client_cli.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/cnf.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/cnf.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/msg.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/msg.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent/server.py` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent/server.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/PKG-INFO` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpgpcard-x25519-agent
-Version: 1.0.0
+Version: 1.0.1
 Summary: Socket interface to Curve25519 ECDH from an OpenPGP card.
 Home-page: https://git.sr.ht/~arx10/openpgpcard-x25519-agent
 Author: Arcem Tene
 Author-email: dev@arcemtene.com
 License: GPL-3.0-or-later
 Project-URL: Mailing List, https://lists.sr.ht/~arx10/openpgpcard-x25519-agent
 Project-URL: Source, https://git.sr.ht/~arx10/openpgpcard-x25519-agent
```

### Comparing `openpgpcard-x25519-agent-1.0.0/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt` & `openpgpcard-x25519-agent-1.0.1/src/openpgpcard_x25519_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/tests/conftest.py` & `openpgpcard-x25519-agent-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/tests/test_card.py` & `openpgpcard-x25519-agent-1.0.1/tests/test_card.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for card utilities."""
 
+from logging import DEBUG
 from unittest.mock import MagicMock
 
 import pytest
 from OpenPGPpy import ConnectionException, DataException, PGPCardException, PinException
 
 from openpgpcard_x25519_agent.card import (
     _send_command_and_zero,
@@ -107,33 +108,92 @@
 def test_send_simple_command_when_failure():
     card, sent = mock_card_and_command([], 0x12, 0x34)
     with pytest.raises(PGPCardException) as e:
         send_simple_command(card, 1, 2, 3, 4, b"foo")
     assert e.value.sw_code == 0x1234
 
 
-def test_send_command_and_zero_when_success():
-    card, sent = mock_card_and_command([5, 6, 7], 8, 9)
-    command = [1, 2, 3, 4]
+def test_send_simple_command_when_get_response_empty():
+    card = MagicMock()
+    sent = mock_card_commands(
+        card,
+        (bytearray(b"bar"), 0x61, 0x03),
+        (bytearray(0), 0x61, 0x00),
+    )
+
+    assert send_simple_command(card, 1, 2, 3, 4, b"foo") == b"bar"
 
-    assert _send_command_and_zero(card, command) == ([5, 6, 7], 8, 9)
+    assert sent == [
+        [1, 2, 3, 4, 3, 0x66, 0x6F, 0x6F],
+        [1, 0xC0, 0, 0, 3],
+    ]
+
+
+def test_send_simple_command_when_get_response_once():
+    card = MagicMock()
+    sent = mock_card_commands(
+        card,
+        (bytearray(0), 0x61, 0x03),
+        (bytearray(b"bar"), 0x90, 0x00),
+    )
 
-    assert sent == [[1, 2, 3, 4]]
-    assert command == [0, 0, 0, 0]
+    assert send_simple_command(card, 1, 2, 3, 4, b"foo") == b"bar"
+
+    assert sent == [
+        [1, 2, 3, 4, 3, 0x66, 0x6F, 0x6F],
+        [1, 0xC0, 0, 0, 3],
+    ]
+
+
+def test_send_simple_command_when_get_response_multiple():
+    card = MagicMock()
+    foo = bytearray(b"foo")
+    bar = bytearray(b"bar")
+    baz = bytearray(b"baz")
+    sent = mock_card_commands(
+        card,
+        (foo, 0x61, 0x06),
+        (bar, 0x61, 0x03),
+        (baz, 0x90, 0x00),
+    )
+
+    assert send_simple_command(card, 1, 2, 3, 4, b"foo") == b"foobarbaz"
+
+    assert sent == [
+        [1, 2, 3, 4, 3, 0x66, 0x6F, 0x6F],
+        [1, 0xC0, 0, 0, 6],
+        [1, 0xC0, 0, 0, 3],
+    ]
+    assert foo == b"\0\0\0"
+    assert bar == b"\0\0\0"
+    assert baz == b"\0\0\0"
+
+
+def test_send_command_and_zero_when_success(caplog):
+    card, sent = mock_card_and_command([6, 7, 8], 9, 0)
+    command = [1, 2, 3, 4, 5, 11, 12, 13, 14, 15]
+
+    with caplog.at_level(DEBUG):
+        assert _send_command_and_zero(card, command) == ([6, 7, 8], 9, 0)
+
+    assert sent == [[1, 2, 3, 4, 5, 11, 12, 13, 14, 15]]
+    assert command == [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+    assert caplog.text.find("sending command to card: 1 2 3 4 + 5 bytes") >= 0
+    assert caplog.text.find("received response from card: 9 0 + 3 bytes") >= 0
 
 
 def test_send_command_and_zero_when_failure():
     card = MagicMock()
     card.connection.transmit.side_effect = ConnectionException("test")
-    command = [1, 2, 3, 4]
+    command = [1, 2, 3, 4, 5, 11, 12, 13, 14, 15]
 
     with pytest.raises(ConnectionException):
         _send_command_and_zero(card, command)
 
-    assert command == [0, 0, 0, 0]
+    assert command == [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
 
 
 def test_verify_pin_when_success():
     card, sent = mock_card_and_command([])
     verify_pin(card, bytearray(b"foo"))
     assert sent == [[0, 0x20, 0, 0x82, 3, 0x66, 0x6F, 0x6F]]
```

### Comparing `openpgpcard-x25519-agent-1.0.0/tests/test_client.py` & `openpgpcard-x25519-agent-1.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/tests/test_cnf.py` & `openpgpcard-x25519-agent-1.0.1/tests/test_cnf.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/tests/test_msg.py` & `openpgpcard-x25519-agent-1.0.1/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/tests/test_server.py` & `openpgpcard-x25519-agent-1.0.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `openpgpcard-x25519-agent-1.0.0/tox.ini` & `openpgpcard-x25519-agent-1.0.1/tox.ini`

 * *Files identical despite different names*

