# Comparing `tmp/oexp-0.5.4.tar.gz` & `tmp/oexp-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.5.4.tar", last modified: Tue May  9 02:15:52 2023, max compression
+gzip compressed data, was "oexp-0.6.0.tar", last modified: Tue May  9 02:37:50 2023, max compression
```

## Comparing `oexp-0.5.4.tar` & `oexp-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:15:52.766267 oexp-0.5.4/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:15:52.766049 oexp-0.5.4/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.5.4/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:15:52.764995 oexp-0.5.4/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.5.4/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    71656 2023-05-09 02:15:37.000000 oexp-0.5.4/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 02:15:20.000000 oexp-0.5.4/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     5375 2023-05-09 01:14:01.000000 oexp-0.5.4/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:15:52.765840 oexp-0.5.4/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 02:15:52.000000 oexp-0.5.4/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 02:15:47.000000 oexp-0.5.4/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 02:15:52.766316 oexp-0.5.4/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:37:50.245425 oexp-0.6.0/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:37:50.245232 oexp-0.6.0/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.6.0/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:37:50.244340 oexp-0.6.0/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      173 2023-05-07 20:52:51.000000 oexp-0.6.0/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    79528 2023-05-09 02:37:35.000000 oexp-0.6.0/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-05-09 02:37:20.000000 oexp-0.6.0/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     5375 2023-05-09 01:14:01.000000 oexp-0.6.0/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-05-09 02:37:50.245068 oexp-0.6.0/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      224 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-05-09 02:37:50.000000 oexp-0.6.0/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-05-09 02:37:45.000000 oexp-0.6.0/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-05-09 02:37:50.245472 oexp-0.6.0/setup.cfg
```

### Comparing `oexp-0.5.4/oexp/access.py` & `oexp-0.6.0/oexp/access.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,45 +3,47 @@
 import sys
 import weakref
 from multiprocessing import current_process
 from threading import current_thread
 import abc
 from typing import List, Optional, Dict, TypeVar, Generic
 from enum import Enum, auto
+import json
 
 _SAFE_PROCESS = current_process().pid
 _SAFE_THREAD = current_thread().ident
 
 
 def _ensure_synchronized():
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/366/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/367/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
 SET_EXIT_PORT = b"\x01"
 CALL_GLOBAL_FUN = b"\x02"
 CREATE_OBJECT = b"\x03"
 INIT_OBJECT = b"\x04"
 CHECK_EQUALITY = b"\x05"
 STR = b"\x06"
 CALL_FUN = b"\x07"
-GET_VAL = b"\x08"
-SET_VAR = b"\x09"
-GC = b"\x0A"
+GET_JSON = b"\x08"
+GET_VAL = b"\x09"
+SET_VAR = b"\x0A"
+GC = b"\x0B"
 
 
 def _sendall(b):
     jbridge._java_conn.sendall(b)
 
 
 def _send_short(arg):
@@ -768,14 +770,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(6)
         temp = _recv_bool(nullable=False)
         return temp
 
     # [[matt.oexp.olang.lab.model.ExperimentConfig]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.ExperimentConfig]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.lab.model.ExperimentConfig]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -862,14 +875,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(2)
         temp = _recv_object(ProlificParticipantUid, nullable=False)
         return temp
 
     # [[matt.oexp.olang.lab.model.Subject]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.Subject]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.lab.model.Subject]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -925,14 +949,25 @@
         temp = _recv_list(
             elementReceiveFun=lambda: _recv_object(Subject, nullable=False),
             nullable=False,
         )
         return temp
 
     # [[matt.oexp.olang.lab.model.SubjectData]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.SubjectData]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.lab.model.SubjectData]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1059,14 +1094,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(5)
         temp = _recv_object(ProlificSessionId, nullable=True)
         return temp
 
     # [[matt.oexp.olang.lab.model.SubjectDemographicData]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.SubjectDemographicData]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.lab.model.SubjectDemographicData]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1119,14 +1165,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.lab.model.Trial]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.Trial]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.lab.model.Trial]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1183,14 +1240,25 @@
         temp = _recv_list(
             elementReceiveFun=lambda: _recv_object(Trial, nullable=False),
             nullable=False,
         )
         return temp
 
     # [[matt.oexp.olang.lab.model.TrialManifest]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.lab.model.TrialManifest]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.lab.model.TrialManifest]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1226,14 +1294,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedStimulusPath]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.EncryptedStimulusPath]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.EncryptedStimulusPath]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.cipher_path == self.cipher_path
 
 
 # [[matt.oexp.olang.model.ExperimentEvent]]
 class ExperimentEvent(KBClass, abc.ABC):
@@ -1257,14 +1336,25 @@
 
     # [[matt.oexp.olang.model.ExperimentEvent#sessionNumber]]
     @property
     @abc.abstractmethod
     def session_number(self) -> SessionNumber:
         pass
 
+    # [[matt.oexp.olang.model.ExperimentEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ExperimentEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
 
 def experiment_start(
     pid=NO_DEFAULT,
     session_id=NO_DEFAULT,
     unix_time_millis=NO_DEFAULT,
     session_number=NO_DEFAULT,
     exp_uid=NO_DEFAULT,
@@ -1352,14 +1442,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(4)
         temp = _recv_long(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExperimentStart]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ExperimentStart]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ExperimentStart]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1393,14 +1494,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_long(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExperimentUID]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ExperimentUID]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ExperimentUID]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.uid == self.uid
 
 
 def manifest_number(num=NO_DEFAULT):
     if num == NO_DEFAULT:
@@ -1428,14 +1540,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_int(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ManifestNumber]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ManifestNumber]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ManifestNumber]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.num == self.num
 
 
 def prolific_participant_uid(pid=NO_DEFAULT):
     if pid == NO_DEFAULT:
@@ -1481,14 +1604,25 @@
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(1)
         _recv_exception_check()
         return _recv_bool(nullable=False)
 
     # [[matt.oexp.olang.model.ProlificParticipantUid]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ProlificParticipantUid]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ProlificParticipantUid]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.pid == self.pid
 
 
 def prolific_session_id(id=NO_DEFAULT):
     if id == NO_DEFAULT:
@@ -1534,14 +1668,25 @@
         _sendall(CALL_FUN)
         _send_long(self._id._id)
         _send_int(1)
         _recv_exception_check()
         return _recv_bool(nullable=False)
 
     # [[matt.oexp.olang.model.ProlificSessionId]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ProlificSessionId]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ProlificSessionId]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.id == self.id
 
 
 def prolific_study_id(id=NO_DEFAULT):
     if id == NO_DEFAULT:
@@ -1569,14 +1714,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ProlificStudyID]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ProlificStudyID]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ProlificStudyID]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.id == self.id
 
 
 def session_number(num=NO_DEFAULT):
     if num == NO_DEFAULT:
@@ -1604,27 +1760,49 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_long(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.SessionNumber]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.SessionNumber]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.SessionNumber]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.num == self.num
 
 
 # [[matt.oexp.olang.model.SubjectTrialEvent]]
 class SubjectTrialEvent(KBClass, abc.ABC):
     # [[matt.oexp.olang.model.SubjectTrialEvent#timeMillis]]
     @property
     @abc.abstractmethod
     def time_millis(self) -> int:
         pass
 
+    # [[matt.oexp.olang.model.SubjectTrialEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.SubjectTrialEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
 
 def temporary_encrypted_stimulus(path=NO_DEFAULT, temp_url=NO_DEFAULT):
     if path == NO_DEFAULT:
         raise Exception(f"there is no default value for path, so it must be defined")
     if temp_url == NO_DEFAULT:
         raise Exception(
             f"there is no default value for temp_url, so it must be defined"
@@ -1673,14 +1851,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(2)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1822,14 +2011,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(2)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.prolific.CompletionCode]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.prolific.CompletionCode]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.prolific.CompletionCode]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1837,14 +2037,24 @@
             return False
 
 
 # [[matt.oexp.olang.model.prolific.CompletionOption]]
 class CompletionOption(Enum):
     url = 0
     code = 1
+    # [[matt.oexp.olang.model.prolific.CompletionOption]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.prolific.CompletionOption]]
+    def to_dict(self):
+        return json.loads(self.to_json())
 
 
 def prolific_study_data(
     external_study_url=NO_DEFAULT,
     completion_option=NO_DEFAULT,
     completion_codes=NO_DEFAULT,
 ):
@@ -1910,14 +2120,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(2)
         temp = _recv_string(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -1966,14 +2187,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
         temp = _recv_int(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ButtonEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ButtonEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ButtonEvent]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -2185,14 +2417,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(9)
         temp = _recv_int(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.EncryptedSubjectTrialData]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.EncryptedSubjectTrialData]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -2292,14 +2535,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(4)
         temp = _recv_long(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.ExitFullScreenEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.ExitFullScreenEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.ExitFullScreenEvent]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -2367,14 +2621,25 @@
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(2)
         temp = _recv_int(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.SelectionEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.SelectionEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.SelectionEvent]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
```

### Comparing `oexp-0.5.4/oexp/jbridge.py` & `oexp-0.6.0/oexp/jbridge.py`

 * *Files identical despite different names*

