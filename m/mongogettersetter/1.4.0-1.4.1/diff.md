# Comparing `tmp/mongogettersetter-1.4.0.tar.gz` & `tmp/mongogettersetter-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.4.0.tar", last modified: Mon May  8 17:58:29 2023, max compression
+gzip compressed data, was "mongogettersetter-1.4.1.tar", last modified: Tue May  9 05:23:47 2023, max compression
```

## Comparing `mongogettersetter-1.4.0.tar` & `mongogettersetter-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 17:58:29.635655 mongogettersetter-1.4.0/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29861 2023-05-08 17:58:29.635655 mongogettersetter-1.4.0/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29264 2023-05-08 17:48:48.000000 mongogettersetter-1.4.0/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 17:58:29.635655 mongogettersetter-1.4.0/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26957 2023-05-08 17:56:16.000000 mongogettersetter-1.4.0/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-08 17:58:29.635655 mongogettersetter-1.4.0/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29861 2023-05-08 17:58:29.000000 mongogettersetter-1.4.0/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-08 17:58:29.000000 mongogettersetter-1.4.0/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-08 17:58:29.000000 mongogettersetter-1.4.0/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-08 17:58:29.000000 mongogettersetter-1.4.0/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-08 17:58:29.000000 mongogettersetter-1.4.0/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-08 17:58:29.635655 mongogettersetter-1.4.0/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-08 17:49:08.000000 mongogettersetter-1.4.0/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30181 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29584 2023-05-08 19:25:09.000000 mongogettersetter-1.4.1/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    26957 2023-05-08 19:15:12.000000 mongogettersetter-1.4.1/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    30181 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-09 05:23:47.000000 mongogettersetter-1.4.1/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-09 05:23:47.672491 mongogettersetter-1.4.1/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-08 19:15:30.000000 mongogettersetter-1.4.1/setup.py
```

### Comparing `mongogettersetter-1.4.0/PKG-INFO` & `mongogettersetter-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.0
+Version: 1.4.1
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -67,15 +67,136 @@
 ```
 $ python3 -i employee.py
 ```
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `EmployeeCollection` in `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
-{'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
+{
+  "_id": "640311ab0469a9c4eaf3d2bd",
+  "id": 4051,
+  "email": "manoj123@gmail.com",
+  "password": "SomeNew SecurePassword",
+  "about": null,
+  "token": "7f471974-ae46-4ac0-a882-1980c300c4d6",
+  "country": "India",
+  "location": null,
+  "lng": 0,
+  "lat": 0,
+  "dob": null,
+  "gender": 0,
+  "userType": 1,
+  "userStatus": 1,
+  "profilePicture": "Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png",
+  "coverPicture": "Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png",
+  "enablefollowme": false,
+  "sendmenotifications": false,
+  "sendTextmessages": false,
+  "enabletagging": false,
+  "createdAt": "2020-01-01T11:13:27.1107739",
+  "updatedAt": "2020-01-02T09:16:49.284864",
+  "livelng": 77.389849,
+  "livelat": 28.6282231,
+  "liveLocation": "Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India",
+  "creditBalance": 130,
+  "myCash": 0,
+  "data": {
+    "name": "array_test",
+    "arr": [
+      1,
+      2,
+      3,
+      4,
+      5,
+      6,
+      7,
+      8
+    ],
+    "hobies": {
+      "composer": [
+        "anirudh",
+        {
+          "co_singer": [
+            "rakshitha",
+            "divagar",
+            "sibi"
+          ]
+        },
+        "yuvan"
+      ],
+      "music": "helo"
+    }
+  },
+  "scores": [
+    {
+      "subject": "math",
+      "score": 100
+    },
+    {
+      "subject": "physics",
+      "score": 85
+    },
+    {
+      "subject": "chemistry",
+      "score": 95
+    }
+  ],
+  "fix": 1,
+  "hello": 1,
+  "recent_views": [
+    200
+  ],
+  "exam": "",
+  "subject": "",
+  "arr": {
+    "name": "sibidharan",
+    "pass": "hello",
+    "score": {
+      "subject": {
+        "minor": "zoology",
+        "major": "biology",
+        "others": [
+          "evs",
+          {
+            "name": "shiro",
+            "inarr": [
+              200,
+              2,
+              3,
+              {
+                "sub": "testsub",
+                "newsu": "aksjdad",
+                "secret": "skdjfnsdkfjnsdfsdf"
+              },
+              4,
+              12
+            ]
+          }
+        ]
+      },
+      "score": 40,
+      "new": "not7",
+      "hello": {
+        "arr": [
+          5,
+          2
+        ]
+      }
+    }
+  },
+  "name": "ManojKumar",
+  "d": [
+    1,
+    3,
+    4,
+    5
+  ],
+  "score": {},
+  "hgf": 5
+}
 ```
 
 This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, `Employee` class will create a new document with the given `id` when initialized. `EmployeeCollection` is designed to replace your MongoDB collection object, so you can use it as a drop-in replacement for your MongoDB collection object inside any class, and perform operations in it according to this documentation.
 
 For example:
 
 ```
@@ -86,23 +207,19 @@
 
 ```
 >>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
->>> e.id.get()
-4051
 >>> e.name
 ManojKumar
->>> e.name.get()
-ManojKumar
 ```
 
-The MongoDB Document's root level attributes are directly accessible as the attributes of the `MongoGetterSetter` object. For example, `e.id` can also be accessible as `e['id']` and `e.name` can also be accessible as `e['name']`. The `e.id.get()` and `e.name.get()` methods are used to get the original datatype of the MongoDB document's root level attributes. For example, `e.id` is an `int` datatype, so `e.id.get()` will return the original `int` datatype. Similarly, `e.data` is a `dict` datatype wrapped in `MongoDictWrapper`, `e.data.get()` will return the original `dict` datatype.
+The MongoDB Document's root level attributes are directly accessible as the attributes of the `MongoGetterSetter` object. For example, `e.id` can also be accessible as `e['id']` and `e.name` can also be accessible as `e['name']`.
 
 For Example:
 
 ```
 >>> e.name = "S. Manoj Kumar"
 >>> e.name
 S. Manoj Kumar
@@ -114,15 +231,15 @@
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> 
 ```
 
 The `MongoDataWrapper` class is used to wrap the MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection.
 
-You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array. You can also use `e.data.arr[0].get()` to get the original datatype of the first element of the `arr` array.
+You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array.
 
 ```
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> type(e.data)
 <class 'mongogettersetter.MongoDataWrapper'>
 >>> type(e.data.get())
@@ -133,15 +250,16 @@
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8, 9], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> e.data.arr[1] = 100
 >>> e.data.arr
 [1, 100, 3, 4, 5, 6, 7, 8, 9]
 >>> e.data.arr[1]
 100
 ```
-Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
+
+All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
 
 ```
 >>> e.data.hobies
 {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}
 >>> e.data.hobies.composer
 ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan']
 >>> e.data.hobies.composer.push('rahman')
@@ -636,14 +754,15 @@
    - `__repr__`
    - `__getattr__`
    - `__getitem__`
    - `__setattr__`
    - `__setitem__`
    - `__delitem__`
    - `__delattr__`
+   - `__contains__`
 
 3. `MongoGetterSetter`: A metaclass that provides a way to override the default behavior of `__getattr__`, `__setattr__`, `__contains__`, `__str__`, `__repr__`, and `__delattr__` to work with MongoDB documents.
 
    Nested class: `PyMongoGetterSetter`
 
    Methods:
    - `__getattr__`
```

### Comparing `mongogettersetter-1.4.0/README.md` & `mongogettersetter-1.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,136 @@
 ```
 $ python3 -i employee.py
 ```
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `EmployeeCollection` in `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
-{'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
+{
+  "_id": "640311ab0469a9c4eaf3d2bd",
+  "id": 4051,
+  "email": "manoj123@gmail.com",
+  "password": "SomeNew SecurePassword",
+  "about": null,
+  "token": "7f471974-ae46-4ac0-a882-1980c300c4d6",
+  "country": "India",
+  "location": null,
+  "lng": 0,
+  "lat": 0,
+  "dob": null,
+  "gender": 0,
+  "userType": 1,
+  "userStatus": 1,
+  "profilePicture": "Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png",
+  "coverPicture": "Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png",
+  "enablefollowme": false,
+  "sendmenotifications": false,
+  "sendTextmessages": false,
+  "enabletagging": false,
+  "createdAt": "2020-01-01T11:13:27.1107739",
+  "updatedAt": "2020-01-02T09:16:49.284864",
+  "livelng": 77.389849,
+  "livelat": 28.6282231,
+  "liveLocation": "Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India",
+  "creditBalance": 130,
+  "myCash": 0,
+  "data": {
+    "name": "array_test",
+    "arr": [
+      1,
+      2,
+      3,
+      4,
+      5,
+      6,
+      7,
+      8
+    ],
+    "hobies": {
+      "composer": [
+        "anirudh",
+        {
+          "co_singer": [
+            "rakshitha",
+            "divagar",
+            "sibi"
+          ]
+        },
+        "yuvan"
+      ],
+      "music": "helo"
+    }
+  },
+  "scores": [
+    {
+      "subject": "math",
+      "score": 100
+    },
+    {
+      "subject": "physics",
+      "score": 85
+    },
+    {
+      "subject": "chemistry",
+      "score": 95
+    }
+  ],
+  "fix": 1,
+  "hello": 1,
+  "recent_views": [
+    200
+  ],
+  "exam": "",
+  "subject": "",
+  "arr": {
+    "name": "sibidharan",
+    "pass": "hello",
+    "score": {
+      "subject": {
+        "minor": "zoology",
+        "major": "biology",
+        "others": [
+          "evs",
+          {
+            "name": "shiro",
+            "inarr": [
+              200,
+              2,
+              3,
+              {
+                "sub": "testsub",
+                "newsu": "aksjdad",
+                "secret": "skdjfnsdkfjnsdfsdf"
+              },
+              4,
+              12
+            ]
+          }
+        ]
+      },
+      "score": 40,
+      "new": "not7",
+      "hello": {
+        "arr": [
+          5,
+          2
+        ]
+      }
+    }
+  },
+  "name": "ManojKumar",
+  "d": [
+    1,
+    3,
+    4,
+    5
+  ],
+  "score": {},
+  "hgf": 5
+}
 ```
 
 This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, `Employee` class will create a new document with the given `id` when initialized. `EmployeeCollection` is designed to replace your MongoDB collection object, so you can use it as a drop-in replacement for your MongoDB collection object inside any class, and perform operations in it according to this documentation.
 
 For example:
 
 ```
@@ -70,23 +191,19 @@
 
 ```
 >>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
->>> e.id.get()
-4051
 >>> e.name
 ManojKumar
->>> e.name.get()
-ManojKumar
 ```
 
-The MongoDB Document's root level attributes are directly accessible as the attributes of the `MongoGetterSetter` object. For example, `e.id` can also be accessible as `e['id']` and `e.name` can also be accessible as `e['name']`. The `e.id.get()` and `e.name.get()` methods are used to get the original datatype of the MongoDB document's root level attributes. For example, `e.id` is an `int` datatype, so `e.id.get()` will return the original `int` datatype. Similarly, `e.data` is a `dict` datatype wrapped in `MongoDictWrapper`, `e.data.get()` will return the original `dict` datatype.
+The MongoDB Document's root level attributes are directly accessible as the attributes of the `MongoGetterSetter` object. For example, `e.id` can also be accessible as `e['id']` and `e.name` can also be accessible as `e['name']`.
 
 For Example:
 
 ```
 >>> e.name = "S. Manoj Kumar"
 >>> e.name
 S. Manoj Kumar
@@ -98,15 +215,15 @@
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> 
 ```
 
 The `MongoDataWrapper` class is used to wrap the MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection.
 
-You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array. You can also use `e.data.arr[0].get()` to get the original datatype of the first element of the `arr` array.
+You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array.
 
 ```
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> type(e.data)
 <class 'mongogettersetter.MongoDataWrapper'>
 >>> type(e.data.get())
@@ -117,15 +234,16 @@
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8, 9], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> e.data.arr[1] = 100
 >>> e.data.arr
 [1, 100, 3, 4, 5, 6, 7, 8, 9]
 >>> e.data.arr[1]
 100
 ```
-Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
+
+All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
 
 ```
 >>> e.data.hobies
 {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}
 >>> e.data.hobies.composer
 ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan']
 >>> e.data.hobies.composer.push('rahman')
@@ -620,14 +738,15 @@
    - `__repr__`
    - `__getattr__`
    - `__getitem__`
    - `__setattr__`
    - `__setitem__`
    - `__delitem__`
    - `__delattr__`
+   - `__contains__`
 
 3. `MongoGetterSetter`: A metaclass that provides a way to override the default behavior of `__getattr__`, `__setattr__`, `__contains__`, `__str__`, `__repr__`, and `__delattr__` to work with MongoDB documents.
 
    Nested class: `PyMongoGetterSetter`
 
    Methods:
    - `__getattr__`
```

### Comparing `mongogettersetter-1.4.0/mongogettersetter/__init__.py` & `mongogettersetter-1.4.1/mongogettersetter/__init__.py`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.4.0/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.4.1/mongogettersetter.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.4.0
+Version: 1.4.1
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
@@ -67,15 +67,136 @@
 ```
 $ python3 -i employee.py
 ```
 This will run the contents of employee.py in interactive mode. Now, you can create an instance of `EmployeeCollection` in `Employee` class and do operations on it. 
 
 Before that, assume you have a MongoDB Collection called `employee` with an object like this:
 ```json
-{'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
+{
+  "_id": "640311ab0469a9c4eaf3d2bd",
+  "id": 4051,
+  "email": "manoj123@gmail.com",
+  "password": "SomeNew SecurePassword",
+  "about": null,
+  "token": "7f471974-ae46-4ac0-a882-1980c300c4d6",
+  "country": "India",
+  "location": null,
+  "lng": 0,
+  "lat": 0,
+  "dob": null,
+  "gender": 0,
+  "userType": 1,
+  "userStatus": 1,
+  "profilePicture": "Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png",
+  "coverPicture": "Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png",
+  "enablefollowme": false,
+  "sendmenotifications": false,
+  "sendTextmessages": false,
+  "enabletagging": false,
+  "createdAt": "2020-01-01T11:13:27.1107739",
+  "updatedAt": "2020-01-02T09:16:49.284864",
+  "livelng": 77.389849,
+  "livelat": 28.6282231,
+  "liveLocation": "Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India",
+  "creditBalance": 130,
+  "myCash": 0,
+  "data": {
+    "name": "array_test",
+    "arr": [
+      1,
+      2,
+      3,
+      4,
+      5,
+      6,
+      7,
+      8
+    ],
+    "hobies": {
+      "composer": [
+        "anirudh",
+        {
+          "co_singer": [
+            "rakshitha",
+            "divagar",
+            "sibi"
+          ]
+        },
+        "yuvan"
+      ],
+      "music": "helo"
+    }
+  },
+  "scores": [
+    {
+      "subject": "math",
+      "score": 100
+    },
+    {
+      "subject": "physics",
+      "score": 85
+    },
+    {
+      "subject": "chemistry",
+      "score": 95
+    }
+  ],
+  "fix": 1,
+  "hello": 1,
+  "recent_views": [
+    200
+  ],
+  "exam": "",
+  "subject": "",
+  "arr": {
+    "name": "sibidharan",
+    "pass": "hello",
+    "score": {
+      "subject": {
+        "minor": "zoology",
+        "major": "biology",
+        "others": [
+          "evs",
+          {
+            "name": "shiro",
+            "inarr": [
+              200,
+              2,
+              3,
+              {
+                "sub": "testsub",
+                "newsu": "aksjdad",
+                "secret": "skdjfnsdkfjnsdfsdf"
+              },
+              4,
+              12
+            ]
+          }
+        ]
+      },
+      "score": 40,
+      "new": "not7",
+      "hello": {
+        "arr": [
+          5,
+          2
+        ]
+      }
+    }
+  },
+  "name": "ManojKumar",
+  "d": [
+    1,
+    3,
+    4,
+    5
+  ],
+  "score": {},
+  "hgf": 5
+}
 ```
 
 This can be accessed by creating an instance of `EmployeeCollection` class with the proper `id` as given in the `self._filter_query`. If such ID doesn't exist, `Employee` class will create a new document with the given `id` when initialized. `EmployeeCollection` is designed to replace your MongoDB collection object, so you can use it as a drop-in replacement for your MongoDB collection object inside any class, and perform operations in it according to this documentation.
 
 For example:
 
 ```
@@ -86,23 +207,19 @@
 
 ```
 >>> e = EmployeeCollection(4051)
 >>> e
 {'_id': ObjectId('640311ab0469a9c4eaf3d2bd'), 'id': 4051, 'email': 'manoj123@gmail.com', 'password': 'SomeNew SecurePassword', 'about': None, 'token': '7f471974-ae46-4ac0-a882-1980c300c4d6', 'country': 'India', 'location': None, 'lng': 0, 'lat': 0, 'dob': None, 'gender': 0, 'userType': 1, 'userStatus': 1, 'profilePicture': 'Images/9b291404-bc2e-4806-88c5-08d29e65a5ad.png', 'coverPicture': 'Images/44af97d9-b8c9-4ec1-a099-010671db25b7.png', 'enablefollowme': False, 'sendmenotifications': False, 'sendTextmessages': False, 'enabletagging': False, 'createdAt': '2020-01-01T11:13:27.1107739', 'updatedAt': '2020-01-02T09:16:49.284864', 'livelng': 77.389849, 'livelat': 28.6282231, 'liveLocation': 'Unnamed Road, Chhijarsi, Sector 63, Noida, Uttar Pradesh 201307, India', 'creditBalance': 130, 'myCash': 0, 'data': {'name': 'array_test', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}, 'scores': [{'subject': 'math', 'score': 100}, {'subject': 'physics', 'score': 85}, {'subject': 'chemistry', 'score': 95}], 'fix': 1, 'hello': 1, 'recent_views': [200], 'exam': '', 'subject': '', 'arr': {'name': 'sibidharan', 'pass': 'hello', 'score': {'subject': {'minor': 'zoology', 'major': 'biology', 'others': ['evs', {'name': 'shiro', 'inarr': [200, 2, 3, {'sub': 'testsub', 'newsu': 'aksjdad', 'secret': 'skdjfnsdkfjnsdfsdf'}, 4, 12]}]}, 'score': 40, 'new': 'not7', 'hello': {'arr': [5, 2]}}}, 'name': 'ManojKumar', 'd': [1, 3, 4, 5], 'score': {}, 'hgf': 5}
 >>> e.id
 4051
->>> e.id.get()
-4051
 >>> e.name
 ManojKumar
->>> e.name.get()
-ManojKumar
 ```
 
-The MongoDB Document's root level attributes are directly accessible as the attributes of the `MongoGetterSetter` object. For example, `e.id` can also be accessible as `e['id']` and `e.name` can also be accessible as `e['name']`. The `e.id.get()` and `e.name.get()` methods are used to get the original datatype of the MongoDB document's root level attributes. For example, `e.id` is an `int` datatype, so `e.id.get()` will return the original `int` datatype. Similarly, `e.data` is a `dict` datatype wrapped in `MongoDictWrapper`, `e.data.get()` will return the original `dict` datatype.
+The MongoDB Document's root level attributes are directly accessible as the attributes of the `MongoGetterSetter` object. For example, `e.id` can also be accessible as `e['id']` and `e.name` can also be accessible as `e['name']`.
 
 For Example:
 
 ```
 >>> e.name = "S. Manoj Kumar"
 >>> e.name
 S. Manoj Kumar
@@ -114,15 +231,15 @@
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> 
 ```
 
 The `MongoDataWrapper` class is used to wrap the MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection.
 
-You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array. You can also use `e.data.arr[0].get()` to get the original datatype of the first element of the `arr` array.
+You can perform almost all basic array operations MongoDB supports. For example, you can use `e.data.arr.push(9)` to append a new element to the `arr` array. Similarly, you can use `e.data.arr.pop()` to pop the last element from the `arr` array. You can also use `e.data.arr.remove(2)` to remove the element `2` from the `arr` array. You can also use `e.data.arr.insert(0, [1,2,3])` to insert the element `[1,2,3]` at the beginning of the `arr` array. You can also use `e.data.arr[0] = 0` to set the first element of the `arr` array to `0`. You can also use `e.data.arr[0]` to get the first element of the `arr` array.
 
 ```
 >>> e.data
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> type(e.data)
 <class 'mongogettersetter.MongoDataWrapper'>
 >>> type(e.data.get())
@@ -133,15 +250,16 @@
 {'name': 'ThisIsAwesmoe', 'arr': [1, 2, 3, 4, 5, 6, 7, 8, 9], 'hobies': {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}}
 >>> e.data.arr[1] = 100
 >>> e.data.arr
 [1, 100, 3, 4, 5, 6, 7, 8, 9]
 >>> e.data.arr[1]
 100
 ```
-Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
+
+All List/Array are wrapped with `MongoDataWrapper` and all dictionary are wrapped with `MongoDictWrapper`. Access documents in any depth, either as attributes or as keys, to access nested data. For example, `e.data.hobies` is a nested dictionary, so you can access the `hobies` dictionary as `e.data.hobies` or `e.data['hobies']`. Similarly, `e.data.hobies.composer` is a nested list, so you can access the `composer` list as `e.data.hobies.composer` or `e.data.hobies['composer']`. Similarly, `e.data.hobies.composer[1]` is a nested dictionary, so you can access the `co_singer` list as `e.data.hobies.composer[1].co_singer` or `e.data.hobies.composer[1]['co_singer']`. Perform all possible operations on all the nested data, limited to the MongoDB supported operations.
 
 ```
 >>> e.data.hobies
 {'composer': ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan'], 'music': 'helo'}
 >>> e.data.hobies.composer
 ['anirudh', {'co_singer': ['rakshitha', 'divagar', 'sibi']}, 'yuvan']
 >>> e.data.hobies.composer.push('rahman')
@@ -636,14 +754,15 @@
    - `__repr__`
    - `__getattr__`
    - `__getitem__`
    - `__setattr__`
    - `__setitem__`
    - `__delitem__`
    - `__delattr__`
+   - `__contains__`
 
 3. `MongoGetterSetter`: A metaclass that provides a way to override the default behavior of `__getattr__`, `__setattr__`, `__contains__`, `__str__`, `__repr__`, and `__delattr__` to work with MongoDB documents.
 
    Nested class: `PyMongoGetterSetter`
 
    Methods:
    - `__getattr__`
```

### Comparing `mongogettersetter-1.4.0/setup.py` & `mongogettersetter-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.4.0',
+    version='1.4.1',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

