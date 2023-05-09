# Comparing `tmp/pyjourney-0.1.4.tar.gz` & `tmp/pyjourney-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjourney-0.1.4.tar", max compression
+gzip compressed data, was "pyjourney-0.1.7.tar", max compression
```

## Comparing `pyjourney-0.1.4.tar` & `pyjourney-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      285 2023-05-08 18:47:43.793002 pyjourney-0.1.4/pyjourney/__init__.py
--rw-r--r--   0        0        0     3915 2023-05-08 19:37:06.751509 pyjourney-0.1.4/pyjourney/api.py
--rw-r--r--   0        0        0      421 2023-05-08 18:47:43.703228 pyjourney-0.1.4/pyjourney/exceptions.py
--rw-r--r--   0        0        0     2095 2023-05-08 19:32:20.598400 pyjourney-0.1.4/pyjourney/models.py
--rw-r--r--   0        0        0      651 2023-05-08 19:37:15.002859 pyjourney-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1332 2023-05-08 19:15:06.713347 pyjourney-0.1.4/README.md
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 pyjourney-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      285 2023-05-08 18:47:43.793002 pyjourney-0.1.7/pyjourney/__init__.py
+-rw-r--r--   0        0        0     5375 2023-05-08 23:59:18.962927 pyjourney-0.1.7/pyjourney/api.py
+-rw-r--r--   0        0        0      421 2023-05-08 18:47:43.703228 pyjourney-0.1.7/pyjourney/exceptions.py
+-rw-r--r--   0        0        0     2089 2023-05-09 00:28:32.193037 pyjourney-0.1.7/pyjourney/models.py
+-rw-r--r--   0        0        0      651 2023-05-09 00:32:07.469689 pyjourney-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1332 2023-05-08 19:15:06.713347 pyjourney-0.1.7/README.md
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 pyjourney-0.1.7/PKG-INFO
```

### Comparing `pyjourney-0.1.4/pyjourney/models.py` & `pyjourney-0.1.7/pyjourney/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # TODO:: Use pydantic to validate the data
 # This is a class to hold the values for the get_jobs api call
 class GetJobsArgs:
 
     def __init__(
             self,
-            amount=35,
+            amount=1,
             dedupe=True,
             jobStatus="completed",
             orderBy="new",
             prompt="undefined",
             refreshApi="0",
             searchType="advanced",
             service="null",
             type="all",
-            user_id="",
+            userId="",
             user_id_ranked_score="null",
             _ql="todo",
             _qurl="https://www.midjourney.com/app/"):
         self.amount = amount
         self.dedupe = dedupe
         self.jobStatus = jobStatus
         self.orderBy = orderBy
         self.prompt = prompt
         self.refreshApi = refreshApi
         self.searchType = searchType
         self.service = service
         self.type = type
-        self.user_id = user_id
+        self.userId = userId
         self.user_id_ranked_score = user_id_ranked_score
         self._ql = _ql
         self._qurl = _qurl
         self._dict = self.to_dict()
 
     def __repr__(self) -> str:
         return str(self._dict)
@@ -52,12 +52,12 @@
             "jobStatus": self.jobStatus,
             "orderBy": self.orderBy,
             "prompt": self.prompt,
             "refreshApi": self.refreshApi,
             "searchType": self.searchType,
             "service": self.service,
             "type": self.type,
-            "user_id": self.user_id,
+            "userId": self.userId,
             "user_id_ranked_score": self.user_id_ranked_score,
             "_ql": self._ql,
             "_qurl": self._qurl
         }
```

### Comparing `pyjourney-0.1.4/pyproject.toml` & `pyjourney-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyjourney"
-version = "0.1.4"
+version = "0.1.7"
 description = "Python module for interacting with the MidJourney API"
 authors = ["agentd00nut <agentd00nut@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/agentd00nut/pyjourney"
 repository = "https://github.com/agentd00nut/pyjourney"
 keywords = ["journey", "midjourney", "api", "python"]
```

### Comparing `pyjourney-0.1.4/README.md` & `pyjourney-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyjourney-0.1.4/PKG-INFO` & `pyjourney-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjourney
-Version: 0.1.4
+Version: 0.1.7
 Summary: Python module for interacting with the MidJourney API
 Home-page: https://github.com/agentd00nut/pyjourney
 License: MIT
 Keywords: journey,midjourney,api,python
 Author: agentd00nut
 Author-email: agentd00nut@gmail.com
 Requires-Python: >=3.10,<4.0
```

