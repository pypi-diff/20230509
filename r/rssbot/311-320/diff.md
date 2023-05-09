# Comparing `tmp/rssbot-311.tar.gz` & `tmp/rssbot-320.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssbot-311.tar", last modified: Wed Apr  5 19:18:08 2023, max compression
+gzip compressed data, was "rssbot-320.tar", last modified: Tue May  9 04:32:40 2023, max compression
```

## Comparing `rssbot-311.tar` & `rssbot-320.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.703632 rssbot-311/
--rw-r--r--   0 bart      (1000) bart      (1001)     3270 2023-04-05 19:18:08.703632 rssbot-311/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1801 2023-04-05 19:17:21.000000 rssbot-311/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.699632 rssbot-311/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     2633 2023-04-05 15:48:20.000000 rssbot-311/bin/rssbot
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1768 2023-04-05 16:46:27.000000 rssbot-311/bin/rssbotcmd
--rwxr-xr-x   0 bart      (1000) bart      (1001)      220 2023-04-05 15:50:01.000000 rssbot-311/bin/rssbotctl
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1533 2023-04-05 15:48:56.000000 rssbot-311/bin/rssbotd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.699632 rssbot-311/files/
--rw-r--r--   0 bart      (1000) bart      (1001)      317 2023-04-05 16:45:36.000000 rssbot-311/files/rssbot.service
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.699632 rssbot-311/rssbot/
--rw-r--r--   0 bart      (1000) bart      (1001)      550 2023-04-05 15:44:17.000000 rssbot-311/rssbot/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1259 2023-04-05 15:44:17.000000 rssbot-311/rssbot/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5733 2023-04-05 15:44:17.000000 rssbot-311/rssbot/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.703632 rssbot-311/rssbot/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       56 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      246 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      494 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18815 2023-04-05 15:53:41.000000 rssbot-311/rssbot/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      898 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7777 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      547 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1003 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1001 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      311 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1455 2023-04-05 15:44:28.000000 rssbot-311/rssbot/modules/utility.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5003 2023-04-05 15:44:17.000000 rssbot-311/rssbot/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3058 2023-04-05 17:26:44.000000 rssbot-311/rssbot/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1343 2023-04-05 15:44:17.000000 rssbot-311/rssbot/threads.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.699632 rssbot-311/rssbot.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     3270 2023-04-05 19:18:08.000000 rssbot-311/rssbot.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      701 2023-04-05 19:18:08.000000 rssbot-311/rssbot.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-05 19:18:08.000000 rssbot-311/rssbot.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        7 2023-04-05 19:18:08.000000 rssbot-311/rssbot.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-05 19:18:08.000000 rssbot-311/rssbot.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-05 19:18:08.703632 rssbot-311/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1081 2023-04-05 19:07:03.000000 rssbot-311/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-05 19:18:08.703632 rssbot-311/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      660 2023-04-05 17:33:06.000000 rssbot-311/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      355 2023-04-05 17:33:14.000000 rssbot-311/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      902 2023-04-05 17:33:26.000000 rssbot-311/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4596 2023-04-05 17:33:51.000000 rssbot-311/test/test_objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1072 2023-04-05 17:34:15.000000 rssbot-311/test/test_storage.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/
+-rw-r--r--   0 bart      (1000) bart      (1001)     3267 2023-05-09 04:32:40.166341 rssbot-320/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1798 2023-05-08 05:08:41.000000 rssbot-320/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     3174 2023-05-08 18:19:43.000000 rssbot-320/bin/rssbot
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1648 2023-05-08 20:27:09.000000 rssbot-320/bin/rssbotcmd
+-rwxr-xr-x   0 bart      (1000) bart      (1001)      244 2023-05-08 18:26:12.000000 rssbot-320/bin/rssbotctl
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1599 2023-05-09 04:26:44.000000 rssbot-320/bin/rssbotd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/files/
+-rw-r--r--   0 bart      (1000) bart      (1001)      317 2023-05-08 05:08:41.000000 rssbot-320/files/rssbot.service
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/rssbot/
+-rw-r--r--   0 bart      (1000) bart      (1001)      799 2023-05-08 18:20:05.000000 rssbot-320/rssbot/classes.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      625 2023-05-09 04:16:38.000000 rssbot-320/rssbot/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1166 2023-05-08 18:20:23.000000 rssbot-320/rssbot/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1076 2023-05-09 04:19:59.000000 rssbot-320/rssbot/command.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      761 2023-05-08 18:20:43.000000 rssbot-320/rssbot/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      527 2023-05-08 18:20:51.000000 rssbot-320/rssbot/default.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1151 2023-05-08 18:20:59.000000 rssbot-320/rssbot/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      579 2023-05-08 18:21:08.000000 rssbot-320/rssbot/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1853 2023-05-09 04:15:17.000000 rssbot-320/rssbot/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      981 2023-05-08 18:21:28.000000 rssbot-320/rssbot/listens.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2008 2023-05-08 18:21:36.000000 rssbot-320/rssbot/loggers.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2308 2023-05-09 04:16:01.000000 rssbot-320/rssbot/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/rssbot/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      306 2023-05-08 18:21:52.000000 rssbot-320/rssbot/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    20605 2023-05-08 18:24:06.000000 rssbot-320/rssbot/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7959 2023-05-08 18:22:05.000000 rssbot-320/rssbot/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3569 2023-05-08 18:32:28.000000 rssbot-320/rssbot/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4362 2023-05-08 18:22:22.000000 rssbot-320/rssbot/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      384 2023-05-08 18:22:31.000000 rssbot-320/rssbot/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      436 2023-05-08 18:22:38.000000 rssbot-320/rssbot/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2195 2023-05-09 04:15:38.000000 rssbot-320/rssbot/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      300 2023-05-08 18:35:03.000000 rssbot-320/rssbot/skipper.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1965 2023-05-08 18:30:37.000000 rssbot-320/rssbot/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1249 2023-05-08 18:23:18.000000 rssbot-320/rssbot/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-05-09 04:32:40.166341 rssbot-320/rssbot.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     3267 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      662 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-05-09 04:32:40.000000 rssbot-320/rssbot.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-05-09 04:32:40.166341 rssbot-320/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1081 2023-05-09 04:31:41.000000 rssbot-320/setup.py
```

### Comparing `rssbot-311/PKG-INFO` & `rssbot-320/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 311
+Version: 320
 Summary: feeding rss into your channel
 Home-page: http://github.com/thatebhj/rssbot
 Author: Bart Thate
 Author-email: thatebhj@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -86,15 +86,15 @@
         
         |
         
         **COMMANDS**
         
         |
         
-        here is a short description of ``rssbotctl`` commands::
+        here is a short description of ``rssctl`` commands::
         
         
          cfg - show the irc configuration, also edits the config
          cmd - show all commands
          dlt - remove a user
          dne - flag todo as done
          dpl - set display items for a rss feed
```

### Comparing `rssbot-311/README.rst` & `rssbot-320/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 |
 
 **COMMANDS**
 
 |
 
-here is a short description of ``rssbotctl`` commands::
+here is a short description of ``rssctl`` commands::
 
 
  cfg - show the irc configuration, also edits the config
  cmd - show all commands
  dlt - remove a user
  dne - flag todo as done
  dpl - set display items for a rss feed
```

### Comparing `rssbot-311/bin/rssbot` & `rssbot-320/bin/rssbotd`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,34 @@
 #!/usr/bin/env python3
 # This file is placed in the Public Domain.
+# pylint: disable=C,I,R,E0611,E0402,W0212
 
 
-'operator bot'
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
+import getpass
+import pwd
 import os
-import readline
 import sys
-import termios
 import time
 import traceback
 
 
 sys.path.insert(0, os.getcwd())
 
 
-from rssbot.handler import Client, Command, Event, Handler, Listens
-from rssbot.handler import command, parse, scan
-from rssbot.objects import update
+from rssbot.errored import Errors
+from rssbot.modules import irc, rss
 from rssbot.persist import Persist
-from rssbot.threads import launch
+from rssbot.runtime import Cfg
 
 
-from rssbot.modules import cmd, flt, irc, log, rss, tdo, thr
-
-
-Persist.workdir = os.path.expanduser('~/.rssbot')
-
-
-scan(cmd)
-scan(irc)
-scan(rss)
-
-
-class CLI(Client):
-
-    def announce(self, txt):
-        pass
-
-    def raw(self, txt):
-        print(txt)
-        sys.stdout.flush()
-
-
-class Console(CLI):
-
-    def handle(self, evt):
-        CLI.handle(self, evt)
-
-    def poll(self):
-        return self.event(input("> "))
+Persist.workdir = "/var/lib/rssbot/"
 
 
 def daemon():
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
@@ -63,67 +37,46 @@
     os.dup2(sis.fileno(), sys.stdin.fileno())
     sos = open('/dev/null', 'a+')
     ses = open('/dev/null', 'a+')
     os.dup2(sos.fileno(), sys.stdout.fileno())
     os.dup2(ses.fileno(), sys.stderr.fileno())
 
 
-def waiter():
-    got = []
-    for ex in Handler.errors:
-        traceback.print_exception(type(ex), ex, ex.__traceback__)
-        got.append(ex)
-    for exc in got:
-        Handler.errors.remove(exc)
-    got = []
-    for ex in Command.errors:
-        traceback.print_exception(type(ex), ex, ex.__traceback__)
-        got.append(ex)
-    for exc in got:
-        Command.errors.remove(exc)
+def main():
+    #daemon()
+    irc.start()
+    rss.start()
+    while 1:
+        time.sleep(1.0)
+        waiter()
 
 
-def wrap(func):
-    fds = sys.stdin.fileno()
-    gotterm = True
-    try:
-        old = termios.tcgetattr(fds)
-    except termios.error:
-        gotterm = False
+def privileges(username):
     try:
-        func()
-    except (EOFError, KeyboardInterrupt):
-        print('')
-    finally:
-        if gotterm:
-            termios.tcsetattr(fds, termios.TCSADRAIN, old)
-        waiter()
-      
+        pwnam = pwd.getpwnam(username)
+    except KeyError:
+        username = getpass.getuser()
+        try:
+            pwnam = pwd.getpwnam(username)
+        except KeyError:
+            return username
+    if os.getuid() != 0:
+        return username
+    os.setgroups([])
+    os.setgid(pwnam.pw_gid)
+    os.setuid(pwnam.pw_uid)
+    return username
 
-def main():
-    dowait = False
-    cfg = parse(' '.join(sys.argv[1:]))
-    if cfg.txt:
-        cli = CLI()
-        command(cli, cfg.otxt)
-    elif 'd' in cfg.opts:
-        daemon()
-        dowait = True
-    elif 'c' in cfg.opts:
-        date = time.ctime(time.time()).replace('  ', ' ')
-        print(f'RSSBOT started {date}')
-        csl = Console()
-        launch(csl.loop)
-        dowait = True
-    if dowait:
-        if os.path.exists("modules"):
-            from modules.scanner import importer, scandir
-            scandir("modules", importer, doall=True)
-        irc.start()
-        rss.start()
-        while 1:
-            time.sleep(1.0)
-            waiter()
+
+def waiter():
+    got = []
+    for ex in Errors.errors:
+        if not Cfg.silent:
+            traceback.print_exception(type(ex), ex, ex.__traceback__)
+        got.append(ex)
+    for exc in got:
+        Errors.errors.remove(exc)
 
 
-wrap(main)
-waiter()
+if __name__ == "__main__":
+    main()
+    waiter()
```

### Comparing `rssbot-311/rssbot/clocked.py` & `rssbot-320/rssbot/clocked.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,E0402
+# pylint: disable=C,I,R,E0402
 
 
-'clocked'
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import threading
 import time
 
 
 from .objects import Object
 from .threads import launch
 
 
 def __dir__():
     return (
-            'Repeater',
-            'Timer'
+            'Timer',
            )
 
 
 __all__ = __dir__()
 
 
 class Timer:
@@ -50,15 +50,7 @@
         timer.start()
         self.timer = timer
         return timer
 
     def stop(self):
         if self.timer:
             self.timer.cancel()
-
-
-class Repeater(Timer):
-
-    def run(self):
-        thr = launch(self.start)
-        super().run()
-        return thr
```

### Comparing `rssbot-311/rssbot/modules/irc.py` & `rssbot-320/rssbot/modules/irc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,125 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0902,R0903,W0613,E1101,R0912,R0904,R0915,E0402
+# pylint: disable=C,I,R,E0402,E1101,W0613
 
 
-'internet relay chat'
+"""internet relay chat
+
+IRC
+
+::
+
+ $ rssbot cfg server=<server> channel=<channel> nick=<nick>
+
+ (*) default channel/server is #opb on localhost
+
+
+SASL
+
+::
+
+ $ rssbot pwd <nickservnick> <nickservpass>
+ $ rssbot cfg password=<outputfrompwd>
+
+
+USERS
+
+as default the user's userhost is not checked when a user types a command in a
+channel. To enable userhost checking enable users with the ``cfg`` command::
+
+ $ rssbot cfg users=True
+
+
+To add a user to the bot use the met command::
+
+ $ rssbot  met <userhost>
+
+to delete a user use the del command with a substring of the userhost::
+
+ $ rssbot del <substring>
+
+"""
+
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
+
 
 
 import base64
 import os
 import queue
 import random
 import socket
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
-from ..handler import Client, Command, Event
-from ..objects import Default, Object, keys, printable, update
-from ..persist import find, fntime, last, write
-from ..threads import launch
-
-
-from .utility import elapsed
+from rssbot.classes import Classes
+from rssbot.clients import Client
+from rssbot.command import Command
+from rssbot.default import Default
+from rssbot.errored import Errors
+from rssbot.message import Message
+from rssbot.listens import Listens
+from rssbot.loggers import Logging
+from rssbot.objects import Object, copy, edit, keys, prt, update
+from rssbot.persist import find, fntime, last, write
+from rssbot.runtime import Cfg
+from rssbot.threads import launch
+from rssbot.utility import elapsed
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
             'NoUser',
             'Users',
             'User',
-            'dlt',
             'cfg',
-            'met',
+            'dlt',
+            'met'
             'mre',
             'pwd',
             'start'
            )
 
 
-NAME = "rssbot"
-
-
 saylock = _thread.allocate_lock()
 
 
 def start():
     irc = IRC()
     irc.start()
+    if "v" in Cfg.opts:
+        Logging.debug(prt(
+                          irc.cfg,
+                          ",".join(keys(irc.cfg)),
+                          skip='control,password,realname,sleep,username')
+                         )
+        irc.joined.wait()
     return irc
 
 
-class NoUser(Exception):
-
-    pass
-
-
 class Config(Default):
 
-    channel = '#%s' % NAME
+    channel = '#%s' % Cfg.name
     control = '!'
-    nick = NAME
+    nick = Cfg.name
     password = ''
     port = 6667
-    realname = NAME
+    realname = Cfg.name
     sasl = False
     server = 'localhost'
     servermodes = ''
     sleep = 60
-    username = NAME
+    username = Cfg.name
     users = False
 
     def __init__(self):
         Default.__init__(self)
         self.control = Config.control
         self.channel = Config.channel
         self.nick = Config.nick
@@ -86,14 +130,17 @@
         self.server = Config.server
         self.servermodes = Config.servermodes
         self.sleep = Config.sleep
         self.username = Config.username
         self.users = Config.users
 
 
+Classes.add(Config)
+
+
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = True
         self.fix_sentence_endings = True
@@ -106,14 +153,16 @@
 
     cache = Object()
 
     def __init__(self):
         Object.__init__(self)
         self.oqueue = queue.Queue()
         self.dostop = threading.Event()
+        self.state = Default()
+        self.state.starttime = time.time()
 
     def dosay(self, channel, txt):
         raise NotImplementedError
 
     def extend(self, channel, txtlist):
         if channel not in self.cache:
             setattr(self.cache, channel, [])
@@ -173,14 +222,15 @@
 class IRC(Client, Output):
 
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
+        self.authed = threading.Event()
         self.connected = threading.Event()
         self.channels = []
         self.joined = threading.Event()
         self.keeprunning = False
         self.outqueue = queue.Queue()
         self.sock = None
         self.speed = 'slow'
@@ -189,14 +239,15 @@
         self.state.errors = []
         self.state.last = 0
         self.state.lastline = ''
         self.state.nrconnect = 0
         self.state.nrerror = 0
         self.state.nrsend = 0
         self.state.pongcheck = False
+        self.state.starttime = time.time()
         self.threaded = False
         self.zelf = ''
         self.register('903', self.h903)
         self.register('904', self.h903)
         self.register('AUTHENTICATE', self.auth)
         self.register('CAP', self.cap)
         self.register('ERROR', self.error)
@@ -208,19 +259,18 @@
         self.target = 'type'
 
     def announce(self, txt):
         for channel in self.channels:
             self.say(channel, txt)
 
     def auth(self, event):
-        time.sleep(1.0)
+        assert self.cfg.password
         self.direct('AUTHENTICATE %s' % self.cfg.password)
 
     def cap(self, event):
-        time.sleep(1.0)
         if self.cfg.password and 'ACK' in event.arguments:
             self.direct('AUTHENTICATE PLAIN')
         else:
             self.direct('CAP REQ :sasl')
 
     def command(self, cmd, *args):
         with saylock:
@@ -253,52 +303,66 @@
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
             self.sock.connect((server, port))
             self.command('CAP LS 302')
         else:
             addr = socket.getaddrinfo(server, port, socket.AF_INET)[-1][-1]
             self.sock = socket.create_connection(addr)
+            self.authed.set()
         if self.sock:
             os.set_inheritable(self.fileno(), os.O_RDWR)
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.connected.set()
             return True
         return False
 
+
     def direct(self, txt):
-        self.sock.send(bytes(txt+'\n', 'utf-8'))
+        Logging.debug(txt)
+        self.sock.send(bytes(txt.rstrip()+'\r\n', 'utf-8'))
 
     def disconnect(self):
-        self.sock.shutdown(2)
+        try:
+            self.sock.shutdown(2)
+        except (
+                ssl.SSLError,
+                OSError,
+                BrokenPipeError
+               ) as ex:
+            Errors.errors.append(ex)
 
     def docommand(self, evt):
         evt.orig = repr(self)
         Command.handle(evt)
 
     def doconnect(self, server, nck, port=6667):
         while 1:
             try:
                 if self.connect(server, port):
                     break
-            except (ssl.SSLError, OSError, ConnectionResetError) as ex:
+            except (
+                    ssl.SSLError,
+                    OSError,
+                    ConnectionResetError
+                   ) as ex:
                 self.state.errors = str(ex)
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def dosay(self, channel, txt):
         self.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
         self.command('PRIVMSG', channel, txt)
 
     def error(self, event):
         self.state.nrerror += 1
         self.state.errors.append(event.txt)
-        self.stop()
+        #self.stop()
 
     def event(self, txt):
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
             self.command('PONG', evt.txt or '')
@@ -321,52 +385,49 @@
             self.command('NICK', nck)
         return evt
 
     def fileno(self):
         return self.sock.fileno()
 
     def h903(self, event):
-        time.sleep(1.0)
         self.command('CAP END')
+        self.authed.set()
 
     def h904(self, event):
-        time.sleep(1.0)
         self.command('CAP END')
+        self.authed.set()
 
     def joinall(self):
         for channel in self.channels:
             self.command('JOIN', channel)
 
     def keep(self):
         while 1:
             self.connected.wait()
             self.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
-            time.sleep(10.0)
             if self.state.pongcheck:
                 self.state.pongcheck = False
                 self.keeprunning = False
+                self.connected.clear()
                 self.stop()
-                launch(self.loop)
-                self.reconnect()
-
+                start()
+                break
 
     def logon(self, server, nck):
-        assert server
-        assert nck
-        assert self.cfg.username
-        assert self.cfg.realname
+        self.connected.wait()
+        self.authed.wait()
         self.direct('NICK %s' % nck)
         self.direct(
-                 'USER %s %s %s :%s' % (self.cfg.username,
+                 'USER %s %s %s :%s' % (self.cfg.username or Cfg.name,
                  server,
                  server,
-                 self.cfg.realname)
+                 self.cfg.realname or Cfg.name)
                 )
 
     def kill(self, event):
         pass
 
     def log(self, event):
         pass
@@ -380,15 +441,15 @@
             )
             self.command('NOTICE', event.channel, txt)
 
     def parsing(self, txt):
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        obj = Event()
+        obj = Message()
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
             obj.origin = arguments[0]
         else:
@@ -431,63 +492,77 @@
             obj.txt = arguments[1]
         spl = obj.txt.split()
         if len(spl) > 1:
             obj.args = spl[1:]
         obj.orig = repr(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
+        Logging.debug(rawstr)
         return obj
 
     def poll(self):
         self.connected.wait()
         if not self.buffer:
             try:
                 self.some()
-            except (ssl.SSLError, socket.timeout, ConnectionResetError) as ex:
-                self.joined.clear()
-                time.sleep(5.0)
-                evt = Event()
-                evt.txt = str(ex)
-                evt.orig = repr(self)
-                return evt
+            except BlockingIOError as ex:
+                time.sleep(1.0)
+                return self.event(str(ex))
+            except (
+                    socket.timeout,
+                    ssl.SSLError,
+                    ssl.SSLZeroReturnError,
+                    ConnectionResetError,
+                    BrokenPipeError
+                   ) as ex:
+                Errors.errors.append(ex)
+                #self.stop()
+                return self.event(str(ex))
         return self.event(self.buffer.pop(0))
 
     def privmsg(self, event):
         if event.txt:
             if event.txt[0] in [self.cfg.control, '!']:
                 event.txt = event.txt[1:]
             elif event.txt.startswith('%s:' % self.cfg.nick):
                 event.txt = event.txt[len(self.cfg.nick)+1:]
             else:
                 return
             if self.cfg.users and not Users.allowed(event.origin, 'USER'):
                 return
-            msg = Event(event)
+            msg = Message()
+            copy(msg, event)
             msg.type = 'command'
             msg.parse(event.txt)
             self.handle(msg)
 
     def quit(self, event):
         if event.orig and event.orig in self.zelf:
-            self.reconnect()
+            self.stop()
 
     def raw(self, txt):
         txt = txt.rstrip()
+        Logging.debug(txt)
         if not txt.endswith('\r\n'):
             txt += '\r\n'
         txt = txt[:512]
         txt += '\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
-            except (ssl.SSLError, ConnectionResetError, BrokenPipeError) as ex:
-                time.sleep(5.0)
-                self.errors.append(ex)
-                self.stop()
+            except (
+                    ssl.SSLError,
+                    ssl.SSLZeroReturnError,
+                    ConnectionResetError,
+                    BrokenPipeError
+                   ) as ex:
+                Errors.errors.append(ex)
+                #self.stop()
+                return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
@@ -510,38 +585,41 @@
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        assert self.cfg.nick
-        assert self.cfg.server
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.connected.clear()
         self.joined.clear()
         launch(Client.start, self)
         launch(Output.start, self)
         launch(
                self.doconnect,
-               self.cfg.server,
-               self.cfg.nick,
+               self.cfg.server or "localhost",
+               self.cfg.nick or Cfg.name,
                int(self.cfg.port or '6667')
               )
         if not self.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        try:
-            self.sock.shutdown(2)
-        except(ssl.SSLError,  OSError):
-            pass
+        Logging.debug("stopping")
+        Listens.remove(self)
         Client.stop(self)
+        Output.stop(self)
+        self.disconnect()
+
+
+class NoUser(Exception):
+
+    pass
 
 
 class Users(Object):
 
     @staticmethod
     def allowed(origin, perm):
         perm = perm.upper()
@@ -593,25 +671,28 @@
         Object.__init__(self)
         self.user = ''
         self.perms = []
         if val:
             update(self, val)
 
 
+Classes.add(User)
+
+
 def cfg(event):
     config = Config()
     last(config)
     if not event.sets:
-        event.reply(printable(
-                          config,
-                          keys(config),
-                          skip='control,password,realname,sleep,username')
-                         )
+        event.reply(prt(
+                        config,
+                        keys(config),
+                        skip='control,password,realname,sleep,username')
+                       )
     else:
-        update(config, event.sets)
+        edit(config, event.sets)
         write(config)
         event.reply('ok')
 
 
 def dlt(event):
     if not event.args:
         event.reply('dlt <username>')
@@ -624,31 +705,26 @@
         break
 
 
 def met(event):
     if not event.args:
         nmr = 0
         for obj in find('user'):
-            event.reply('%s %s %s %s' % (
-                                         nmr,
-                                         obj.user,
-                                         obj.perms,
-                                         elapsed(time.time() - fntime(obj.__fnm__)))
-                                        )
+            lap = elapsed(time.time() - fntime(obj.__fnm__))
+            event.reply(f'{nmr} {obj.user} {obj.perms} {lap}s')
             nmr += 1
         if not nmr:
-            event.reply('no users introduced yet')
+            event.reply('no user')
         return
     user = User()
     user.user = event.rest
     user.perms = ['USER']
     write(user)
     event.reply('ok')
 
-
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
         return
     bot = event.bot()
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
```

### Comparing `rssbot-311/rssbot/modules/rss.py` & `rssbot-320/rssbot/modules/rss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0903,E1101,E0402
+# pylint: disable=C,I,R,E0402,E1101
 
 
-'rich site syndicate'
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 import html.parser
 import re
 import threading
 import time
 import urllib
@@ -14,33 +15,32 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from ..clocked import Repeater
-from ..handler import Listens
-from ..objects import Object, printable, update
-from ..persist import find, fntime, last, write
-from ..threads import launch, threaded
-
-
-from .utility import elapsed, spl
+from rssbot.classes import Classes
+from rssbot.listens import Listens
+from rssbot.objects import Object, prt, update
+from rssbot.persist import find, fntime, last, write
+from rssbot.repeats import Repeater
+from rssbot.runtime import Cfg
+from rssbot.threads import launch, threaded
+from rssbot.utility import elapsed, spl
 
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
         'Rss',
         'Seen',
         'Timer',
-        'debug',
         'dpl',
         'ftc',
         'nme',
         'rem',
         'rss',
         'start'
     )
@@ -66,21 +66,27 @@
     def __init__(self):
         super().__init__()
         self.display_list = 'title,link,author'
         self.name = ''
         self.rss = ''
 
 
+Classes.add(Rss)
+
+
 class Seen(Object):
 
     def __init__(self):
         super().__init__()
         self.urls = []
 
 
+Classes.add(Seen)
+
+
 class Fetcher(Object):
 
     dosave = False
     seen = Seen()
 
     def __init__(self):
         super().__init__()
@@ -186,15 +192,15 @@
             for itm in spl(item):
                 setattr(obj, itm, Parser.getitem(line, itm))
             res.append(obj)
         return res
 
 
 def getfeed(url, item):
-    if DEBUG:
+    if Cfg.debug:
         return [Object(), Object()]
     try:
         result = geturl(url)
     except (ValueError, HTTPError, URLError):
         return [Object(), Object()]
     if not result:
         return [Object(), Object()]
@@ -206,29 +212,30 @@
         ('submit', 'submit'),
         ('url', url),
     ]
     postdata = urlencode(postarray, quote_via=quote_plus)
     req = Request('http://tinyurl.com/create.php',
                   data=bytes(postdata, 'UTF-8'))
     req.add_header('User-agent', useragent(url))
-    for txt in urlopen(req).readlines():
-        line = txt.decode('UTF-8').strip()
-        i = re.search('data-clipboard-text="(.*?)"', line, re.M)
-        if i:
-            return i.groups()
+    with urlopen(req) as htm:
+        for txt in htm.readlines():
+            line = txt.decode('UTF-8').strip()
+            i = re.search('data-clipboard-text="(.*?)"', line, re.M)
+            if i:
+                return i.groups()
     return []
 
 
 def geturl(url):
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
-    req.add_header('User-agent', useragent('OPB - object programming bot'))
-    response = urllib.request.urlopen(req)
-    response.data = response.read()
-    return response
+    req.add_header('User-agent', useragent(Cfg.name.upper()))
+    with urllib.request.urlopen(req) as response:
+        response.data = response.read()
+        return response
 
 
 def striphtml(text):
     clean = re.compile('<.*?>')
     return re.sub(clean, '', text)
 
 
@@ -293,15 +300,15 @@
 
 def rss(event):
     if not event.rest:
         nrs = 0
         for feed in find('rss'):
             event.reply('%s %s %s' % (
                                    nrs,
-                                   printable(feed),
+                                   prt(feed),
                                    elapsed(time.time()-fntime(feed.__oid__))
                                   )
                        )
             nrs += 1
         if not nrs:
             event.reply('no rss feed found.')
         return
```

### Comparing `rssbot-311/rssbot/modules/utility.py` & `rssbot-320/rssbot/utility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0116
+# pylint: disable=C,I,R,E0402
 
 
-'utilities'
-
-
-import os
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
 def __dir__():
     return (
             'elapsed',
-            'fnclass',
             'spl'
            )
 
 
 __all__ = __dir__()
 
 
@@ -54,23 +51,13 @@
         txt += "%sm" % minutes
     if sec:
         txt += "%ss" % sec
     txt = txt.strip()
     return txt
 
 
-def fnclass(pth):
-    try:
-        _rest, *path2 = pth.split('store')
-        splitted = path2[0].split(os.sep)
-        return splitted[1]
-    except (ValueError, IndexError):
-        return pth.split(os.sep)[0]
-    return None
-
-
 def spl(txt):
     try:
         res = txt.split(',')
     except (TypeError, ValueError):
         res = txt
     return [x for x in res if x]
```

### Comparing `rssbot-311/rssbot/persist.py` & `rssbot-320/rssbot/persist.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # Tihs file is placed in the Public Domain.
-# pylint: disable=C0115,C0116,R0903,E0402
+# pylint: disable=C,I,R,E0402
 
 
-"persistence"
+__author__ = "B.H.J. Thate <thatebhj@gmail.com>"
+__version__ = 1
 
 
+import json
 import os
 import pathlib
 import time
 import _thread
 
 
-from .objects import Object, dump, load, kind, search, update
+from .classes import Classes
+from .decoder import ObjectDecoder
+from .encoder import ObjectEncoder
+from .errored import NoClassError
+from .objects import Object, kind, search, update
+from .runtime import Cfg
 
 
 def __dir__():
     return (
             'Persist',
             'cdir',
             'last',
@@ -30,113 +37,163 @@
 
 
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
 
-    workdir = ""
+    workdir = Cfg.wd
+
+    @staticmethod
+    def logdir():
+        return os.path.join(Persist.workdir, "logs")
+
+    @staticmethod
+    def storedir():
+        return os.path.join(Persist.workdir, "store")
 
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
         pth = os.path.dirname(pth)
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
+def dump(*args, **kw) -> None:
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
 def files() -> []:
     return os.listdir(os.path.join(Persist.workdir, "store"))
 
 
-def fns(match) -> []:
+def find(mtc, selector=None) -> []:
+    if selector is None:
+        selector = {}
+    for fnm in fns(mtc):
+        obj = hook(fnm)
+        if '__deleted__' in obj:
+            continue
+        if selector and not search(obj, selector):
+            continue
+        yield obj
+
+
+def fnclass(pth):
+    try:
+        *_rest, mpth = pth.split("store")
+        splitted = mpth.split(os.sep)
+        return splitted[0]
+    except ValueError:
+        pass
+    return None
+
+
+def fns(mtc) -> []:
     assert Persist.workdir
     dname = ''
-    lst = match.lower().split(".")[-1]
+    lst = mtc.lower().split(".")[-1]
     for rootdir, dirs, _files in os.walk(Persist.workdir, topdown=False):
         if dirs:
             dname = sorted(dirs)[-1]
             if dname.count('-') == 2:
                 ddd = os.path.join(rootdir, dname)
                 fls = sorted(os.listdir(ddd))
                 if fls:
                     path2 = os.path.join(ddd, fls[-1])
-                    spl = strip(path2).split(os.sep)[0]
+                    spl = strip(path2).split(os.sep, maxsplit=1)[0]
                     if lst in spl.lower().split(".")[-1]:
                         yield strip(path2)
 
 
+def fntime(daystr):
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        tme += float('.' + rest)
+    else:
+        tme = 0
+    return tme
+
+
 def hook(otp) -> Object:
-    obj = Object()
-    read(obj, otp)
-    return obj
+    clz = fnclass(otp)
+    cls = Classes.get(clz)
+    if cls:
+        obj = cls()
+        read(obj, otp)
+        return obj
+    raise NoClassError(clz)
+
+
+def last(obj, selector=None) -> None:
+    if selector is None:
+        selector = {}
+    result = sorted(
+                    find(kind(obj), selector),
+                    key=lambda x: fntime(x.__oid__)
+                   )
+    if result:
+        inp = result[-1]
+        update(obj, inp)
+        obj.__oid__ = inp.__oid__
+    return obj.__oid__
+
+
+def match(mtc, selector=None) -> []:
+    if selector is None:
+        selector = {}
+    for tpe in Classes.match(mtc):
+        for fnm in fns(tpe):
+            obj = hook(fnm)
+            if '__deleted__' in obj:
+                continue
+            if selector and not search(obj, selector):
+                continue
+            yield obj
+
+
+def load(fpt, *args, **kw) -> Object:
+    return json.load(fpt, *args, cls=ObjectDecoder, **kw)
 
 
 def path(pth) -> str:
     return os.path.join(Persist.workdir, 'store', pth)
 
 
 def read(obj, pth) -> None:
     pth = path(pth)
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             data = load(ofile)
             update(obj, data)
     obj.__oid__ = strip(pth)
+    return obj.__oid__
 
 
 def setwd(pth) -> None:
     Persist.workdir = pth
 
 
 def strip(pth) -> str:
     return os.sep.join(pth.split(os.sep)[-4:])
 
 
+def touch(fname):
+    fds = os.open(fname, os.O_WRONLY | os.O_CREAT)
+    os.close(fds)
+
+
 def write(obj) -> str:
     pth = path(obj.__oid__)
     cdir(pth)
     with disklock:
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile)
     return strip(pth)
-
-
-def find(match, selector=None) -> []:
-    if selector is None:
-        selector = {}
-    for fnm in fns(match):
-        obj = hook(fnm)
-        if '__deleted__' in obj and obj.__deleted__:
-            continue
-        if selector and not search(obj, selector):
-            continue
-        yield obj
-
-
-def last(obj, selector=None) -> None:
-    if selector is None:
-        selector = {}
-    result = sorted(
-                    find(kind(obj), selector),
-                    key=lambda x: fntime(x.__oid__)
-                   )
-    if result:
-        inp = result[-1]
-        update(obj, inp)
-        obj.__oid__ = inp.__oid__
-    return obj.__oid__
-
-
-def fntime(daystr):
-    daystr = daystr.replace('_', ':')
-    datestr = ' '.join(daystr.split(os.sep)[-2:])
-    if '.' in datestr:
-        datestr, rest = datestr.rsplit('.', 1)
-    else:
-        rest = ''
-    tme = time.mktime(time.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
-    if rest:
-        tme += float('.' + rest)
-    else:
-        tme = 0
-    return tme
```

### Comparing `rssbot-311/rssbot.egg-info/PKG-INFO` & `rssbot-320/rssbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rssbot
-Version: 311
+Version: 320
 Summary: feeding rss into your channel
 Home-page: http://github.com/thatebhj/rssbot
 Author: Bart Thate
 Author-email: thatebhj@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -86,15 +86,15 @@
         
         |
         
         **COMMANDS**
         
         |
         
-        here is a short description of ``rssbotctl`` commands::
+        here is a short description of ``rssctl`` commands::
         
         
          cfg - show the irc configuration, also edits the config
          cmd - show all commands
          dlt - remove a user
          dne - flag todo as done
          dpl - set display items for a rss feed
```

### Comparing `rssbot-311/setup.py` & `rssbot-320/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="rssbot",
-    version="311",
+    version="320",
     author="Bart Thate",
     author_email="thatebhj@gmail.com",
     url="http://github.com/thatebhj/rssbot",
     description="feeding rss into your channel",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

