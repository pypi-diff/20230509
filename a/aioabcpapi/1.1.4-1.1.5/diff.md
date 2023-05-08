# Comparing `tmp/aioabcpapi-1.1.4.tar.gz` & `tmp/aioabcpapi-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-1.1.4.tar", last modified: Sun Apr 16 16:41:09 2023, max compression
+gzip compressed data, was "aioabcpapi-1.1.5.tar", last modified: Mon May  8 23:13:24 2023, max compression
```

## Comparing `aioabcpapi-1.1.4.tar` & `aioabcpapi-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.414548 aioabcpapi-1.1.4/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     5341 2023-04-16 16:41:09.414548 aioabcpapi-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4519 2022-11-22 13:00:19.000000 aioabcpapi-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.273688 aioabcpapi-1.1.4/aioabcpapi/
--rw-rw-rw-   0        0        0      584 2023-04-16 16:40:20.000000 aioabcpapi-1.1.4/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      680 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    18863 2023-04-11 16:46:29.000000 aioabcpapi-1.1.4/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4799 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.342685 aioabcpapi-1.1.4/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-1.1.4/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   113231 2023-04-11 17:21:52.000000 aioabcpapi-1.1.4/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      767 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60152 2022-12-13 07:07:31.000000 aioabcpapi-1.1.4/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-1.1.4/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.379550 aioabcpapi-1.1.4/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-1.1.4/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   113383 2023-04-11 17:37:33.000000 aioabcpapi-1.1.4/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      784 2023-04-11 17:25:28.000000 aioabcpapi-1.1.4/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    45010 2023-04-11 16:56:32.000000 aioabcpapi-1.1.4/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.399548 aioabcpapi-1.1.4/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-1.1.4/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-1.1.4/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9025 2023-04-11 17:30:01.000000 aioabcpapi-1.1.4/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.303685 aioabcpapi-1.1.4/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5341 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-04-16 16:41:09.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-04-16 16:41:08.000000 aioabcpapi-1.1.4/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-04-16 16:41:09.416548 aioabcpapi-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-04-16 16:40:20.000000 aioabcpapi-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:41:09.413549 aioabcpapi-1.1.4/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-1.1.4/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.097699 aioabcpapi-1.1.5/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     5341 2023-05-08 23:13:24.097699 aioabcpapi-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4519 2022-11-22 13:00:19.000000 aioabcpapi-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:23.969668 aioabcpapi-1.1.5/aioabcpapi/
+-rw-rw-rw-   0        0        0      584 2023-05-08 23:12:15.000000 aioabcpapi-1.1.5/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    18959 2023-05-08 23:10:24.000000 aioabcpapi-1.1.5/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4799 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.028683 aioabcpapi-1.1.5/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-1.1.5/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   113231 2023-04-11 17:21:52.000000 aioabcpapi-1.1.5/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      767 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60138 2023-04-16 16:54:48.000000 aioabcpapi-1.1.5/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-1.1.5/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.065691 aioabcpapi-1.1.5/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-1.1.5/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   113383 2023-04-11 17:37:33.000000 aioabcpapi-1.1.5/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      784 2023-04-11 17:25:28.000000 aioabcpapi-1.1.5/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    45010 2023-04-11 16:56:32.000000 aioabcpapi-1.1.5/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.083694 aioabcpapi-1.1.5/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-1.1.5/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-1.1.5/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9025 2023-04-11 17:30:01.000000 aioabcpapi-1.1.5/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:23.993675 aioabcpapi-1.1.5/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5341 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-05-08 23:13:23.000000 aioabcpapi-1.1.5/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-05-08 23:13:24.099700 aioabcpapi-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-05-08 23:12:15.000000 aioabcpapi-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 23:13:24.095699 aioabcpapi-1.1.5/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-1.1.5/test/test_payload.py
```

### Comparing `aioabcpapi-1.1.4/LICENSE` & `aioabcpapi-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/PKG-INFO` & `aioabcpapi-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 1.1.4
+Version: 1.1.5
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-1.1.4/README.md` & `aioabcpapi-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/__init__.py` & `aioabcpapi-1.1.5/aioabcpapi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,9 +6,9 @@
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '1.1.4'
+__version__ = '1.1.5'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-1.1.4/aioabcpapi/abcp.py` & `aioabcpapi-1.1.5/aioabcpapi/abcp.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/api.py` & `aioabcpapi-1.1.5/aioabcpapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,16 @@
                 email = re.match('^[\w.]+@([\w-]+\.)+[\w-]{2,6}$', login, flags=re.IGNORECASE)
                 if email:
                     return False
                 else:
                     raise UnsupportedLogin('Недопустимый логин')
             else:
                 raise UnsupportedLogin('Недопустимый логин')
+        elif host[:4] == 'abcp' and host.split('.')[0][4:].isdigit():
+            return True
         else:
             raise UnsupportedHost(f'Имя хоста {host} не поддерживается\n'
                                   f'Допустимые имена id200.public.api.abcp.ru')
     else:
         raise PasswordType('Допускаются пароли только в md5 hash')
```

### Comparing `aioabcpapi-1.1.4/aioabcpapi/base.py` & `aioabcpapi-1.1.5/aioabcpapi/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/cp/admin.py` & `aioabcpapi-1.1.5/aioabcpapi/cp/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/cp/base.py` & `aioabcpapi-1.1.5/aioabcpapi/cp/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/cp/client.py` & `aioabcpapi-1.1.5/aioabcpapi/cp/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,15 @@
     async def set_client_params(self,
                                 payment_method_index: int,
                                 shipment_address_index: int,
                                 shipment_method_index: int = None,
                                 shipment_office_index: int = None):
         """
         Устанавливает параметры для метода order.
-        Если все индексы переданы верно в методы <b>api.cp.client.order.order_by_basket</b> и <b>api.cp.client.order.order_instant</b> не требуется передавать аргументы:
+        Если все индексы переданы верно в методы api.cp.client.order.order_by_basket и api.cp.client.order.order_instant не требуется передавать аргументы:
         'payment_method', 'shipment_address', 'shipment_method', 'shipment_office'.
 
         :param payment_method_index: Обязательный параметр для любого типа отгрузки. Индекс типа оплаты полученный методом payment_method
         :type payment_method_index: int
         :param shipment_address_index: Обязательный параметр для любого типа отгрузки. Индекс адреса доставки полученный методом shipment_address
         :type shipment_address_index: int
         :param shipment_method_index: Не обязательный параметр, если используется самовывоз. Индекс типа доставки полученный методом payment_method
```

### Comparing `aioabcpapi-1.1.4/aioabcpapi/exceptions.py` & `aioabcpapi-1.1.5/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/ts/admin.py` & `aioabcpapi-1.1.5/aioabcpapi/ts/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/ts/base.py` & `aioabcpapi-1.1.5/aioabcpapi/ts/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/ts/client.py` & `aioabcpapi-1.1.5/aioabcpapi/ts/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-1.1.5/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi/utils/payload.py` & `aioabcpapi-1.1.5/aioabcpapi/utils/payload.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-1.1.5/aioabcpapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 1.1.4
+Version: 1.1.5
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-1.1.4/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-1.1.5/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-1.1.4/setup.py` & `aioabcpapi-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
 
 setup(
     name='aioabcpapi',
-    version='1.1.4',
+    version='1.1.5',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-1.1.4/test/test_payload.py` & `aioabcpapi-1.1.5/test/test_payload.py`

 * *Files identical despite different names*

