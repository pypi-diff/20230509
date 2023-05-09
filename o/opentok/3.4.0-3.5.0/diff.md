# Comparing `tmp/opentok-3.4.0.tar.gz` & `tmp/opentok-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opentok-3.4.0.tar", last modified: Tue Mar 14 18:17:18 2023, max compression
+gzip compressed data, was "dist/opentok-3.5.0.tar", last modified: Tue May  9 16:58:21 2023, max compression
```

## Comparing `opentok-3.4.0.tar` & `opentok-3.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-03-14 18:17:18.000000 opentok-3.4.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.4.0/LICENSE.txt
--rw-r--r--   0 mkahan     (503) staff       (20)    25662 2023-03-14 18:17:18.000000 opentok-3.4.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)    24357 2023-03-14 18:17:01.000000 opentok-3.4.0/README.rst
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok/
--rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:17:01.000000 opentok-3.4.0/opentok/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.4.0/opentok/archives.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3754 2022-10-12 15:29:40.000000 opentok-3.4.0/opentok/broadcast.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6229 2023-03-14 18:17:01.000000 opentok-3.4.0/opentok/endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3270 2023-03-14 18:17:01.000000 opentok-3.4.0/opentok/exceptions.py
--rw-r--r--   0 mkahan     (503) staff       (20)    92594 2023-03-14 18:17:01.000000 opentok-3.4.0/opentok/opentok.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.4.0/opentok/render.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.4.0/opentok/session.py
--rw-r--r--   0 mkahan     (503) staff       (20)      446 2022-09-05 18:13:07.000000 opentok-3.4.0/opentok/sip_call.py
--rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.4.0/opentok/stream.py
--rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.4.0/opentok/streamlist.py
--rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-03-14 18:17:01.000000 opentok-3.4.0/opentok/version.py
--rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:17:01.000000 opentok-3.4.0/opentok/websocket_audio_connection.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)    25662 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      472 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-03-14 18:17:18.000000 opentok-3.4.0/opentok.egg-info/top_level.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-03-14 18:17:18.000000 opentok-3.4.0/setup.cfg
--rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.4.0/setup.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-05-09 16:58:21.000000 opentok-3.5.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1079 2022-09-05 18:13:07.000000 opentok-3.5.0/LICENSE.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)    25836 2023-05-09 16:58:21.000000 opentok-3.5.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)    24531 2023-05-09 16:58:09.000000 opentok-3.5.0/README.rst
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok/
+-rw-r--r--   0 mkahan     (503) staff       (20)      605 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     7369 2022-10-12 15:29:40.000000 opentok-3.5.0/opentok/archives.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3754 2023-05-09 16:40:54.000000 opentok-3.5.0/opentok/broadcast.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     6229 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/endpoints.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3270 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/exceptions.py
+-rw-r--r--   0 mkahan     (503) staff       (20)    92855 2023-05-09 16:49:47.000000 opentok-3.5.0/opentok/opentok.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1360 2022-10-12 15:29:40.000000 opentok-3.5.0/opentok/render.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2165 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/session.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      446 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/sip_call.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      899 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/stream.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      809 2022-09-05 18:13:07.000000 opentok-3.5.0/opentok/streamlist.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      101 2023-05-09 16:49:47.000000 opentok-3.5.0/opentok/version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      680 2023-03-14 18:39:57.000000 opentok-3.5.0/opentok/websocket_audio_connection.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)    25836 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      472 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       39 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        8 2023-05-09 16:58:21.000000 opentok-3.5.0/opentok.egg-info/top_level.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      103 2023-05-09 16:58:21.000000 opentok-3.5.0/setup.cfg
+-rw-r--r--   0 mkahan     (503) staff       (20)     2630 2022-10-12 15:29:40.000000 opentok-3.5.0/setup.py
```

### Comparing `opentok-3.4.0/LICENSE.txt` & `opentok-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/PKG-INFO` & `opentok-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.4.0
+Version: 3.5.0
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
@@ -74,28 +74,32 @@
   from opentok import Client
 
   opentok = Client(api_key, api_secret)
 
 Creating Sessions
 ~~~~~~~~~~~~~~~~~
 
-To create an OpenTok Session, use the ``opentok.create_session()`` method. There are three optional
+To create an OpenTok Session, use the ``opentok.create_session()`` method. There are optional
 keyword parameters for this method:
 
 * ``location`` which can be set to a string containing an IP address.
 
 * ``media_mode`` which is a String (defined by the MediaModes class).
   This determines whether the session will use the
   `OpenTok Media Router <https://tokbox.com/developer/guides/create-session/#media-mode>`_
   or attempt to send streams directly between clients. A routed session is required for some
   OpenTok features (such as archiving).
 
 * ``archive_mode`` which specifies whether the session will be automatically archived (``always``)
   or not (``manual``).
 
+* ``e2ee`` which is a boolean. This specifies whether to enable
+  `end-to-end encryption <https://tokbox.com/developer/guides/end-to-end-encryption/>`_
+  for the OpenTok session.
+
 This method returns a ``Session`` object. Its ``session_id`` attribute is useful when saving to a persistent
 store (such as a database).
 
 .. code:: python
 
   # Create a session that attempts to send streams directly between clients (falling back
   # to use the OpenTok TURN server to relay streams if the clients cannot connect):
```

### Comparing `opentok-3.4.0/README.rst` & `opentok-3.5.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,28 +44,32 @@
   from opentok import Client
 
   opentok = Client(api_key, api_secret)
 
 Creating Sessions
 ~~~~~~~~~~~~~~~~~
 
-To create an OpenTok Session, use the ``opentok.create_session()`` method. There are three optional
+To create an OpenTok Session, use the ``opentok.create_session()`` method. There are optional
 keyword parameters for this method:
 
 * ``location`` which can be set to a string containing an IP address.
 
 * ``media_mode`` which is a String (defined by the MediaModes class).
   This determines whether the session will use the
   `OpenTok Media Router <https://tokbox.com/developer/guides/create-session/#media-mode>`_
   or attempt to send streams directly between clients. A routed session is required for some
   OpenTok features (such as archiving).
 
 * ``archive_mode`` which specifies whether the session will be automatically archived (``always``)
   or not (``manual``).
 
+* ``e2ee`` which is a boolean. This specifies whether to enable
+  `end-to-end encryption <https://tokbox.com/developer/guides/end-to-end-encryption/>`_
+  for the OpenTok session.
+
 This method returns a ``Session`` object. Its ``session_id`` attribute is useful when saving to a persistent
 store (such as a database).
 
 .. code:: python
 
   # Create a session that attempts to send streams directly between clients (falling back
   # to use the OpenTok TURN server to relay streams if the clients cannot connect):
```

### Comparing `opentok-3.4.0/opentok/__init__.py` & `opentok-3.5.0/opentok/__init__.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/archives.py` & `opentok-3.5.0/opentok/archives.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/broadcast.py` & `opentok-3.5.0/opentok/broadcast.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/endpoints.py` & `opentok-3.5.0/opentok/endpoints.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/exceptions.py` & `opentok-3.5.0/opentok/exceptions.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/opentok.py` & `opentok-3.5.0/opentok/opentok.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,15 @@
         return token
 
     def create_session(
         self,
         location=None,
         media_mode=MediaModes.relayed,
         archive_mode=ArchiveModes.manual,
+        e2ee=False,
     ):
         """
         Creates a new OpenTok session and returns the session ID, which uniquely identifies
         the session.
 
         For example, when using the OpenTok JavaScript library, use the session ID when calling the
         OT.initSession() method (to initialize an OpenTok session).
@@ -355,14 +356,17 @@
             (either automatically or not), you must set the media_mode parameter to
             MediaModes.routed.
 
         :param String location: An IP address that the OpenTok servers will use to
             situate the session in its global network. If you do not set a location hint,
             the OpenTok servers will be based on the first client connecting to the session.
 
+         :param Boolean e2ee: Whether to enable end-to-end encryption for a routed session
+             (see https://tokbox.com/developer/guides/end-to-end-encryption/).
+
         :rtype: The Session object. The session_id property of the object is the session ID.
         """
 
         # build options
         options = {}
         if not isinstance(media_mode, MediaModes):
             raise OpenTokException(
@@ -391,14 +395,15 @@
             except:
                 raise OpenTokException(
                     u(
                         "Cannot create session. Location must be either None or a valid IPv4 address {0}"
                     ).format(location)
                 )
             options[u("location")] = location
+        options["e2ee"] = e2ee
 
         try:
             logger.debug(
                 "POST to %r with params %r, headers %r, proxies %r",
                 self.endpoints.session_url(),
                 options,
                 self.headers(),
@@ -432,21 +437,22 @@
                         error.attributes["code"].value,
                         error.firstChild.attributes["message"].value,
                     )
                 )
 
             session_id = (
                 dom.getElementsByTagName("session_id")[0].childNodes[0].nodeValue
-            )
+            )            
             return Session(
                 self,
                 session_id,
                 location=location,
                 media_mode=media_mode,
                 archive_mode=archive_mode,
+                e2ee=e2ee,
             )
         except Exception as e:
             raise OpenTokException("Failed to generate session: %s" % str(e))
 
     def get_headers(self):
         """For internal use."""
         return {
```

### Comparing `opentok-3.4.0/opentok/render.py` & `opentok-3.5.0/opentok/render.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/session.py` & `opentok-3.5.0/opentok/session.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/stream.py` & `opentok-3.5.0/opentok/stream.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/streamlist.py` & `opentok-3.5.0/opentok/streamlist.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok/websocket_audio_connection.py` & `opentok-3.5.0/opentok/websocket_audio_connection.py`

 * *Files identical despite different names*

### Comparing `opentok-3.4.0/opentok.egg-info/PKG-INFO` & `opentok-3.5.0/opentok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentok
-Version: 3.4.0
+Version: 3.5.0
 Summary: OpenTok server-side SDK
 Home-page: https://github.com/opentok/Opentok-Python-SDK/
 Author: TokBox, Inc.
 Author-email: support@tokbox.com
 License: LICENSE.txt
 Keywords: video chat tokbox tok opentok python media webrtc archiving realtime
 Classifier: Development Status :: 5 - Production/Stable
@@ -74,28 +74,32 @@
   from opentok import Client
 
   opentok = Client(api_key, api_secret)
 
 Creating Sessions
 ~~~~~~~~~~~~~~~~~
 
-To create an OpenTok Session, use the ``opentok.create_session()`` method. There are three optional
+To create an OpenTok Session, use the ``opentok.create_session()`` method. There are optional
 keyword parameters for this method:
 
 * ``location`` which can be set to a string containing an IP address.
 
 * ``media_mode`` which is a String (defined by the MediaModes class).
   This determines whether the session will use the
   `OpenTok Media Router <https://tokbox.com/developer/guides/create-session/#media-mode>`_
   or attempt to send streams directly between clients. A routed session is required for some
   OpenTok features (such as archiving).
 
 * ``archive_mode`` which specifies whether the session will be automatically archived (``always``)
   or not (``manual``).
 
+* ``e2ee`` which is a boolean. This specifies whether to enable
+  `end-to-end encryption <https://tokbox.com/developer/guides/end-to-end-encryption/>`_
+  for the OpenTok session.
+
 This method returns a ``Session`` object. Its ``session_id`` attribute is useful when saving to a persistent
 store (such as a database).
 
 .. code:: python
 
   # Create a session that attempts to send streams directly between clients (falling back
   # to use the OpenTok TURN server to relay streams if the clients cannot connect):
```

### Comparing `opentok-3.4.0/setup.py` & `opentok-3.5.0/setup.py`

 * *Files identical despite different names*

