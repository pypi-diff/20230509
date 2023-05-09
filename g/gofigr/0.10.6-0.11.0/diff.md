# Comparing `tmp/gofigr-0.10.6.tar.gz` & `tmp/gofigr-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofigr-0.10.6.tar", last modified: Sun Apr 16 22:56:38 2023, max compression
+gzip compressed data, was "gofigr-0.11.0.tar", last modified: Tue May  9 19:07:11 2023, max compression
```

## Comparing `gofigr-0.10.6.tar` & `gofigr-0.11.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.213648 gofigr-0.10.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-04-16 22:39:06.000000 gofigr-0.10.6/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-04-16 22:39:06.000000 gofigr-0.10.6/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-04-16 22:56:38.213648 gofigr-0.10.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-04-16 22:39:06.000000 gofigr-0.10.6/README.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.209648 gofigr-0.10.6/gofigr/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12625 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/gfconfig.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18297 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/jupyter.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41605 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.213648 gofigr-0.10.6/gofigr/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/resources/FreeMono.ttf
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-04-16 22:39:06.000000 gofigr-0.10.6/gofigr/watermarks.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.209648 gofigr-0.10.6/gofigr.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      447 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-04-16 22:56:38.000000 gofigr-0.10.6/gofigr.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-04-16 22:39:06.000000 gofigr-0.10.6/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-16 22:56:38.213648 gofigr-0.10.6/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-16 22:56:38.213648 gofigr-0.10.6/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40797 2023-04-16 22:39:06.000000 gofigr-0.10.6/tests/test_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-04-16 22:39:06.000000 gofigr-0.10.6/tests/test_models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-04-16 22:39:06.000000 gofigr-0.10.6/tests/test_watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1078 2023-05-09 18:47:57.000000 gofigr-0.11.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-05-09 18:47:57.000000 gofigr-0.11.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-09 19:07:11.155597 gofigr-0.11.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6023 2023-05-09 18:47:57.000000 gofigr-0.11.0/README.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.151597 gofigr-0.11.0/gofigr/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12625 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4991 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/gfconfig.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18303 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/jupyter.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42702 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/models.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/gofigr/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   584424 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/resources/FreeMono.ttf
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3097 2023-05-09 18:47:57.000000 gofigr-0.11.0/gofigr/watermarks.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/gofigr.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      466 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2023-05-09 19:07:11.000000 gofigr-0.11.0/gofigr.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1546 2023-05-09 18:47:57.000000 gofigr-0.11.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-09 19:07:11.155597 gofigr-0.11.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 19:07:11.155597 gofigr-0.11.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    40823 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1967 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_logs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2698 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_models.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1007 2023-05-09 18:47:57.000000 gofigr-0.11.0/tests/test_watermarks.py
```

### Comparing `gofigr-0.10.6/LICENSE` & `gofigr-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.6/PKG-INFO` & `gofigr-0.11.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.10.6
+Version: 0.11.0
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.10.6/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.0/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.10.6)
+GoFigr - Python Client (0.11.0)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.10.6/README.rst` & `gofigr-0.11.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.10.6)
+GoFigr - Python Client (0.11.0)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.10.6/gofigr/__init__.py` & `gofigr-0.11.0/gofigr/__init__.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.6/gofigr/gfconfig.py` & `gofigr-0.11.0/gofigr/gfconfig.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.6/gofigr/jupyter.py` & `gofigr-0.11.0/gofigr/jupyter.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     return bio.read()
 
 
 class Publisher:
     """\
     Publishes revisions to the GoFigr server.
     """
-    def __init__(self, gf, watermark=None, annotators=DEFAULT_ANNOTATORS, image_formats=("png",),
+    def __init__(self, gf, watermark=None, annotators=DEFAULT_ANNOTATORS, image_formats=("png", "eps"),
                  default_metadata=None, clear=True):
         """
 
         :param gf: GoFigr instance
         :param watermark: watermark generator, e.g. QRWatermark()
         :param annotators: revision annotators
         :param image_formats: image formats to save by default
```

### Comparing `gofigr-0.10.6/gofigr/models.py` & `gofigr-0.11.0/gofigr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -559,68 +559,101 @@
     """
     def __init__(self, username, timestamp, action, target_id, target_type,
                  deleted_sentinel=None,
                  deleted=False,
                  thumbnail=None,
                  target_name=None,
                  analysis_id=None,
-                 analysis_name=None):
+                 analysis_name=None,
+                 api_id=None,
+                 gf=None,
+                 parent=None):
         """\
 
         :param username: user who performed the activity
         :param timestamp: time the activity was performed
         :param action: Type of action (a string): create, create_child, view, update, move, delete
         :param target_id: API ID of the target object
         :param target_type: type of the target object
         :param deleted_sentinel: if this is a delete action (target no longer exists), this field captures the name of
         the entity that was deleted
         :param deleted: True if target was deleted
         :param thumbnail: base-64 encoded thumbnail image of the target object
         :param target_name: not used
         :param analysis_id: ID of the parent analysis
         :param analysis_name: name of the parent analysis
+        :param api_id: API ID for this activity
+        :param gf: GoFigr client instance
+        :param parent: parent object, e.g. Workspace or Analysis
         """
         self.username, self.timestamp, self.action = username, timestamp, action
         self.target_id, self.target_type = target_id, target_type
         self.deleted, self.deleted_sentinel = deleted, deleted_sentinel
         self.thumbnail = thumbnail
         self.target_name = target_name
         self.analysis_id = analysis_id
         self.analysis_name = analysis_name
+        self.api_id = api_id
+        self.gf = gf
+        self.parent = parent
+
+    def fetch(self):
+        """Fetches information about this log item from the server. API ID and parent have to be set."""
+        if self.api_id is None:
+            raise ValueError("API ID is None")
+        elif self.parent is None:
+            raise ValueError("Parent is None")
+        elif self.parent.api_id is None:
+            raise ValueError("Parent API ID is None")
+
+        # pylint: disable=protected-access
+        obj = self.gf._get(urljoin(self.parent.endpoint + "/" + self.parent.api_id + "/log/", self.api_id + "/")).json()
+
+        if 'timestamp' in obj.keys():
+            obj['timestamp'] = dateutil.parser.parse(obj['timestamp'])
+
+        for name, value in obj.items():
+            setattr(self, name, value)
+
+        return self
 
     @classmethod
-    def from_json(cls, data):
+    def from_json(cls, data, gf=None, parent=None):
         timestamp = data.get('timestamp')
         if timestamp:
             timestamp = dateutil.parser.parse(timestamp)
 
         return LogItem(username=data.get('username'),
                        timestamp=timestamp,
                        action=data.get('action'),
                        target_id=data.get('target_id'),
                        target_type=data.get('target_type'),
                        target_name=data.get('target_name'),
                        deleted_sentinel=data.get('deleted_sentinel'),
                        deleted=data.get('deleted'),
                        thumbnail=data.get('thumbnail'),
                        analysis_id=data.get('analysis_id'),
-                       analysis_name=data.get('analysis_name'))
+                       analysis_name=data.get('analysis_name'),
+                       api_id=data.get('api_id'),
+                       gf=gf,
+                       parent=parent)
 
     def to_json(self):
         return {'username': self.username,
                 'timestamp': self.timestamp,
                 'action': self.action,
                 'target_id': self.target_id,
                 'target_type': self.target_type,
                 'target_name': self.target_name,
                 'deleted_sentinel': self.deleted_sentinel,
                 'thumbnail': self.thumbnail,
                 'deleted': self.deleted,
                 'analysis_id': self.analysis_id,
-                'analysis_name': self.analysis_name}
+                'analysis_name': self.analysis_name,
+                'api_id': self.api_id}
 
     def __repr__(self):
         return str(self.to_json())
 
 
 class ShareableModelMixin(ModelMixin):
     """\
@@ -710,15 +743,32 @@
 
     ALL_LEVELS = [OWNER, ADMIN, CREATOR, VIEWER]
 
 
 Recents = namedtuple("Recents", ["analyses", "figures"])
 
 
-class gf_Workspace(ModelMixin):
+class LogsMixin:
+    """\
+    Mixin for entities which support the /log/ endpoint.
+
+    """
+    def get_logs(self):
+        """\
+        Retrieves the activity log.
+
+        :return: list of LogItem objects.
+        """
+        # pylint: disable=protected-access
+        response = self._gf._get(urljoin(self.endpoint, f'{self.api_id}/log/'),
+                                 expected_status=HTTPStatus.OK)
+        return [LogItem.from_json(datum, gf=self._gf, parent=self) for datum in response.json()]
+
+
+class gf_Workspace(ModelMixin, LogsMixin):
     """Represents a workspace"""
     # pylint: disable=protected-access
 
     fields = ["api_id",
               "name",
               "description",
               "workspace_type",
@@ -787,24 +837,14 @@
         """
         response = self._gf._post(urljoin(self.endpoint, f'{self.api_id}/members/remove/'),
                                   json=WorkspaceMember(username=username, membership_type=None).to_json(),
                                   expected_status=HTTPStatus.OK)
 
         return WorkspaceMember.from_json(response.json())
 
-    def get_logs(self):
-        """\
-        Retrieves the activity log.
-
-        :return: list of LogItem objects.
-        """
-        response = self._gf._get(urljoin(self.endpoint, f'{self.api_id}/log/'),
-                                 expected_status=HTTPStatus.OK)
-        return [LogItem.from_json(datum) for datum in response.json()]
-
     def get_recents(self, limit=100):
         """\
         Gets the most recently created or modified analyses & figures.
 
         :param limit: maximum number of elements to retrieve.
         :return: Instance of the Recents object
         """
@@ -812,15 +852,15 @@
                                          expected_status=HTTPStatus.OK)
         data = response.json()
         analyses = [self._gf.Analysis(**datum) for datum in data.get("analyses", [])]
         figures = [self._gf.Figure(**datum) for datum in data.get("figures", [])]
         return Recents(analyses, figures)
 
 
-class gf_Analysis(ShareableModelMixin):
+class gf_Analysis(ShareableModelMixin, LogsMixin):
     """Represents an analysis"""
     # pylint: disable=protected-access
 
     fields = ["api_id",
               "name",
               "description",
               LinkedEntityField("workspace", lambda gf: gf.Workspace, lazy=True, many=False),
@@ -837,24 +877,14 @@
         :param kwargs: parameters to Figure (e.g. description) if it needs to be created
         :return: Figure instance
 
         """
         return self.figures.find_or_create(name=name,
                                            default_obj=self._gf.Figure(name=name, **kwargs) if create else None)
 
-    def get_logs(self):
-        """\
-        Retrieves the activity log.
-
-        :return: list of LogItem objects.
-        """
-        response = self._gf._get(urljoin(self.endpoint, f'{self.api_id}/log/'),
-                                 expected_status=HTTPStatus.OK)
-        return [LogItem.from_json(datum) for datum in response.json()]
-
 
 class gf_Figure(ShareableModelMixin):
     """Represents a figure"""
     fields = ["api_id",
               "name",
               "description",
               LinkedEntityField("analysis", lambda gf: gf.Analysis, lazy=True, many=False),
```

### Comparing `gofigr-0.10.6/gofigr/resources/FreeMono.ttf` & `gofigr-0.11.0/gofigr/resources/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.6/gofigr/watermarks.py` & `gofigr-0.11.0/gofigr/watermarks.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.6/gofigr.egg-info/PKG-INFO` & `gofigr-0.11.0/gofigr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gofigr
-Version: 0.10.6
+Version: 0.11.0
 Summary: GoFigr client library
 Author-email: Maciej Pacula <maciej@gofigr.io>
 License: Copyright 2022-2023 Flagstaff Solutions, LLC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the “Software”), to deal in
         the Software without restriction, including without limitation the rights to
@@ -20,28 +20,28 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Homepage, https://www.gofigr.io
-Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.10.6/
+Project-URL: Documentation, https://gofigr.io/docs/gofigr-python/0.11.0/
 Keywords: science,visualization,version control,plotting,data,reproducibility
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 .. figure:: docs/source/images/logo_wide_light.png
   :alt: GoFigr.io logo
 
-GoFigr - Python Client (0.10.6)
+GoFigr - Python Client (0.11.0)
 ====================================
 GoFigr (https://www.gofigr.io) is a service which provides sophisticated version control for figures.
 
 This repository contains the Python client for GoFigr.
 
 Account registration
 ********************
```

### Comparing `gofigr-0.10.6/pyproject.toml` & `gofigr-0.11.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gofigr"
-version = "0.10.6"
+version = "0.11.0"
 description = "GoFigr client library"
 readme = "README.rst"
 authors = [{ name = "Maciej Pacula", email = "maciej@gofigr.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,21 +24,21 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["pip-tools", "bumpver", "build", "twine", "pylint", "flake8", "sphinx", "sphinx_rtd_theme", "sphinxcontrib-jquery"]
 
 [project.urls]
 Homepage = "https://www.gofigr.io"
-Documentation = "https://gofigr.io/docs/gofigr-python/0.10.6/"
+Documentation = "https://gofigr.io/docs/gofigr-python/0.11.0/"
 
 [project.scripts]
 gfconfig = "gofigr.gfconfig:main"
 
 [tool.bumpver]
-current_version = "0.10.6"
+current_version = "0.11.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gofigr-0.10.6/tests/test_client.py` & `gofigr-0.11.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         obj.save()
 
         server_obj = obj.__class__(api_id=obj.api_id).fetch()
 
         # We're not too strict about creation time, but all these objects are created
         # in the unit test and should be fairly recent (~1min)
         test_case.assertLess(datetime.now().astimezone() - obj.created_on,
-                             timedelta(seconds=60))
+                             timedelta(seconds=120))
         test_case.assertEqual(obj.created_by, gf.username)
 
         test_case.assertEqual(server_obj.updated_by, gf.username)
         test_case.assertGreaterEqual(server_obj.updated_on - last_update, timedelta(seconds=delay_seconds))
         test_case.assertLess(server_obj.updated_on - last_update, timedelta(seconds=delay_seconds + 20))
         last_update = server_obj.updated_on
 
@@ -487,15 +487,15 @@
 
             for parent in [fig, ana, workspace]:
                 parent.fetch()
                 self.assertGreaterEqual(parent.child_updated_on, deletion_time)
                 self.assertEqual(parent.child_updated_by, gf.username)
 
         # Check logs
-        logs = workspace.get_logs()
+        logs = [log.fetch() for log in workspace.get_logs()]
         self.assertEqual(len(logs), 18)  # 18 = create x3 (workspace+analysis+fig) + (create, update, delete) x 5 revisions
         for item in logs:
             self.assertIn(item.action, ["create", "update", "delete"])
             self.assertLessEqual((datetime.now().astimezone() - item.timestamp).total_seconds(), 120)
 
     def test_revisions(self):
         gf = make_gf()
```

### Comparing `gofigr-0.10.6/tests/test_models.py` & `gofigr-0.11.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `gofigr-0.10.6/tests/test_watermarks.py` & `gofigr-0.11.0/tests/test_watermarks.py`

 * *Files identical despite different names*

