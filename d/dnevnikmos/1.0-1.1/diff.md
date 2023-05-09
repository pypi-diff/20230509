# Comparing `tmp/dnevnikmos-1.0.tar.gz` & `tmp/dnevnikmos-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnevnikmos-1.0.tar", last modified: Tue May  9 10:14:39 2023, max compression
+gzip compressed data, was "dnevnikmos-1.1.tar", last modified: Tue May  9 13:31:12 2023, max compression
```

## Comparing `dnevnikmos-1.0.tar` & `dnevnikmos-1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 10:14:39.398185 dnevnikmos-1.0/
--rw-rw-rw-   0        0        0     4197 2023-05-09 10:14:39.398185 dnevnikmos-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3759 2023-05-09 10:11:52.000000 dnevnikmos-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 10:14:39.379859 dnevnikmos-1.0/dnevniklib/
--rw-rw-rw-   0        0        0      255 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/__init__.py
--rw-rw-rw-   0        0        0      303 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/errors.py
--rw-rw-rw-   0        0        0     1223 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/homeworks.py
--rw-rw-rw-   0        0        0      277 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/lessons.py
--rw-rw-rw-   0        0        0     2107 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/marks.py
--rw-rw-rw-   0        0        0      292 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/school.py
--rw-rw-rw-   0        0        0     3442 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/user.py
--rw-rw-rw-   0        0        0     1314 2023-05-09 10:11:52.000000 dnevnikmos-1.0/dnevniklib/user_token_getter.py
-drwxrwxrwx   0        0        0        0 2023-05-09 10:14:39.397176 dnevnikmos-1.0/dnevnikmos.egg-info/
--rw-rw-rw-   0        0        0     4197 2023-05-09 10:14:39.000000 dnevnikmos-1.0/dnevnikmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-09 10:14:39.000000 dnevnikmos-1.0/dnevnikmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 10:14:39.000000 dnevnikmos-1.0/dnevnikmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-09 10:14:39.000000 dnevnikmos-1.0/dnevnikmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 10:14:39.399183 dnevnikmos-1.0/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-05-09 10:14:34.000000 dnevnikmos-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:31:12.851673 dnevnikmos-1.1/
+-rw-rw-rw-   0        0        0      290 2023-05-09 13:31:12.850673 dnevnikmos-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-09 13:29:41.000000 dnevnikmos-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 13:31:12.837634 dnevnikmos-1.1/dnevnikmos/
+-rw-rw-rw-   0        0        0      255 2023-05-09 13:26:53.000000 dnevnikmos-1.1/dnevnikmos/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-05-09 13:26:52.000000 dnevnikmos-1.1/dnevnikmos/errors.py
+-rw-rw-rw-   0        0        0     1223 2023-05-09 13:27:24.000000 dnevnikmos-1.1/dnevnikmos/homeworks.py
+-rw-rw-rw-   0        0        0      277 2023-05-09 10:11:52.000000 dnevnikmos-1.1/dnevnikmos/lessons.py
+-rw-rw-rw-   0        0        0     2107 2023-05-09 13:28:01.000000 dnevnikmos-1.1/dnevnikmos/marks.py
+-rw-rw-rw-   0        0        0      292 2023-05-09 10:11:52.000000 dnevnikmos-1.1/dnevnikmos/school.py
+-rw-rw-rw-   0        0        0     3442 2023-05-09 13:28:44.000000 dnevnikmos-1.1/dnevnikmos/user.py
+-rw-rw-rw-   0        0        0     1314 2023-05-09 13:28:59.000000 dnevnikmos-1.1/dnevnikmos/user_token_getter.py
+drwxrwxrwx   0        0        0        0 2023-05-09 13:31:12.849675 dnevnikmos-1.1/dnevnikmos.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-05-09 13:31:12.000000 dnevnikmos-1.1/dnevnikmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-09 13:31:12.000000 dnevnikmos-1.1/dnevnikmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 13:31:12.000000 dnevnikmos-1.1/dnevnikmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-09 13:31:12.000000 dnevnikmos-1.1/dnevnikmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 13:31:12.851673 dnevnikmos-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-05-09 13:30:58.000000 dnevnikmos-1.1/setup.py
```

### Comparing `dnevnikmos-1.0/dnevniklib/homeworks.py` & `dnevnikmos-1.1/dnevnikmos/homeworks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import json
-from dnevniklib.errors import *
+from dnevnikmos.errors import *
 
 
 class Homeworks:
     def __init__(self, user) -> None:
         self.session = user.session
         self.token = user.token
         self.id = user.id
@@ -28,9 +28,9 @@
                         homeworks.append(
                             {
                                 "name": str(lesson_),
                                 "homework": str(homework)
                             }
                         )
         except KeyError:
-            raise DnevnikLibError("Неверная дата")
+            raise DnevnikMosError("Неверная дата")
         return homeworks
```

### Comparing `dnevnikmos-1.0/dnevniklib/marks.py` & `dnevnikmos-1.1/dnevnikmos/marks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dnevniklib.errors import *
+from dnevnikmos.errors import *
 
 
 class Marks:
     def __init__(self, user) -> None:
         self.session = user.session
         self.token = user.token
         self.id = user.id
@@ -23,15 +23,15 @@
                     if activity["lesson"]["marks"]:
                         lesson_ = activity["lesson"]["subject_name"]
                         mark = activity["lesson"]["marks"][0]["value"]
                         marks.append(
                             {"name": lesson_, "mark": mark}
                         )
         except KeyError:
-            raise DnevnikLibError("Скорее всего, неверная дата")
+            raise DnevnikMosError("Скорее всего, неверная дата")
         return marks
 
     def get_trimester_marks(self, trimester: int, academic_year_id: int = 10):
         """
         Триместр вводим в последовательности 0 - 1 триместр, 1 - 2 триместр, 2 - 3 триместр
         ID года вводим 10
         """
```

### Comparing `dnevnikmos-1.0/dnevniklib/user.py` & `dnevnikmos-1.1/dnevnikmos/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from requests import Session
-from dnevniklib.errors import DnevnikLibError
+from dnevnikmos.errors import DnevnikMosError
 
 
 class User:
     def __init__(self, token=None) -> None:
         # Init function
         self.default_api_url = "https://dnevnik.mos.ru/mobile/api"
         self.token = token
@@ -22,23 +22,23 @@
             self.birth_date = self.data_about_user["children"][0]["birth_date"]
             self.sex = self.data_about_user["children"][0]["sex"]
             self.class_name = self.data_about_user["children"][0]["class_name"]
             self.contract_id = self.data_about_user["children"][0]["contract_id"]
             self.parents = self.data_about_user["children"][0]["representatives"]
         else:
             if self.data_about_user == 403:
-                raise DnevnikLibError("non-existent token")
+                raise DnevnikMosError("non-existent token")
             elif self.data_about_user == 400:
-                raise DnevnikLibError("Bad Request")
+                raise DnevnikMosError("Bad Request")
             elif self.data_about_user == 402:
-                raise DnevnikLibError("Non-existent token")
+                raise DnevnikMosError("Non-existent token")
             elif self.data_about_user == 401:
-                raise DnevnikLibError("Your token expired")
+                raise DnevnikMosError("Your token expired")
             else:
-                raise DnevnikLibError()
+                raise DnevnikMosError()
 
 
     def login(self):
         """
         Сюда ничего не задаем
         :return:
         """
```

### Comparing `dnevnikmos-1.0/dnevniklib/user_token_getter.py` & `dnevnikmos-1.1/dnevnikmos/user_token_getter.py`

 * *Files identical despite different names*

### Comparing `dnevnikmos-1.0/setup.py` & `dnevnikmos-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Определение requests как requirements для того, чтобы этот пакет работал. Зависимости проекта.
 requirements = ["requests<=2.21.0", "selenium"]
 
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setuptools.setup(
 	name="dnevnikmos",
-	version="1.0",
+	version="1.1",
 	author="Boiko Arseniy",
 	author_email="ars254642@gmail.com",
 	description="Library for automated work with dnevnik.mos.ru",
 
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/CyberBars1k/dnevnikmos/",
```

