# Comparing `tmp/swiftshadow-0.2.3.tar.gz` & `tmp/swiftshadow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftshadow-0.2.3.tar", last modified: Thu May  4 07:58:38 2023, max compression
+gzip compressed data, was "swiftshadow-1.0.0.tar", last modified: Tue May  9 08:39:03 2023, max compression
```

## Comparing `swiftshadow-0.2.3.tar` & `swiftshadow-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:38.225992 swiftshadow-0.2.3/swiftshadow/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-04 07:58:25.000000 swiftshadow-0.2.3/swiftshadow/swiftshadow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:58:38.229992 swiftshadow-0.2.3/swiftshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 07:58:38.000000 swiftshadow-0.2.3/swiftshadow.egg-info/top_level.txt
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 08:39:03.934757 swiftshadow-1.0.0/
+-rw-rw----   0 root         (0) everybody  (9997)    35149 2023-04-25 06:53:34.000000 swiftshadow-1.0.0/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     2640 2023-05-09 08:39:03.922757 swiftshadow-1.0.0/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2275 2023-05-04 09:07:57.000000 swiftshadow-1.0.0/README.md
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-09 08:39:03.938757 swiftshadow-1.0.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1022 2023-05-08 07:45:36.000000 swiftshadow-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 08:39:03.802757 swiftshadow-1.0.0/swiftshadow/
+-rw-rw----   0 root         (0) everybody  (9997)      630 2023-05-09 08:30:11.000000 swiftshadow-1.0.0/swiftshadow/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)      434 2023-05-02 07:02:57.000000 swiftshadow-1.0.0/swiftshadow/cache.py
+-rw-rw----   0 root         (0) everybody  (9997)     5826 2023-05-09 08:30:11.000000 swiftshadow-1.0.0/swiftshadow/classes.py
+-rw-rw----   0 root         (0) everybody  (9997)     6303 2023-04-25 06:53:34.000000 swiftshadow-1.0.0/swiftshadow/constants.py
+-rw-rw----   0 root         (0) everybody  (9997)      917 2023-05-04 09:19:08.000000 swiftshadow-1.0.0/swiftshadow/helpers.py
+-rw-rw----   0 root         (0) everybody  (9997)     1495 2023-05-04 09:19:08.000000 swiftshadow-1.0.0/swiftshadow/providers.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-09 08:39:03.902757 swiftshadow-1.0.0/swiftshadow.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2640 2023-05-09 08:39:03.000000 swiftshadow-1.0.0/swiftshadow.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      341 2023-05-09 08:39:03.000000 swiftshadow-1.0.0/swiftshadow.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-09 08:39:03.000000 swiftshadow-1.0.0/swiftshadow.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        9 2023-05-09 08:39:03.000000 swiftshadow-1.0.0/swiftshadow.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       12 2023-05-09 08:39:03.000000 swiftshadow-1.0.0/swiftshadow.egg-info/top_level.txt
```

### Comparing `swiftshadow-0.2.3/LICENSE` & `swiftshadow-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.3/PKG-INFO` & `swiftshadow-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.3
+Version: 1.0.0
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Swiftshadow
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/swiftshadow) ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/sachin-sankar/swiftshadow?include_prereleases&style=flat)
 ## About
@@ -26,17 +28,17 @@
 ``` py
 pip install swiftshadow
 ```
 
 ## One class rules all
 Everything in swiftshadow is under one class for ease of use and minimal code.
 
-Get a proxy using just 3 lines of code!
+Get a proxy using just 2 lines of code!
 ``` py
-from swiftshadow.swiftshadow import Proxy
+from swiftshadow.swiftshadow import QuickProxy
 
-swift = Proxy()
-print(swift.proxy())
+print(QuickProxy())
 ```
 That was easy. 
 
 Head to [Documentation](https://sachin-sankar.github.io/swiftshadow/) to get started.
+
```

### Comparing `swiftshadow-0.2.3/README.md` & `swiftshadow-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 ``` py
 pip install swiftshadow
 ```
 
 ## One class rules all
 Everything in swiftshadow is under one class for ease of use and minimal code.
 
-Get a proxy using just 3 lines of code!
+Get a proxy using just 2 lines of code!
 ``` py
-from swiftshadow.swiftshadow import Proxy
+from swiftshadow.swiftshadow import QuickProxy
 
-swift = Proxy()
-print(swift.proxy())
+print(QuickProxy())
 ```
 That was easy. 
 
 Head to [Documentation](https://sachin-sankar.github.io/swiftshadow/) to get started.
```

### Comparing `swiftshadow-0.2.3/setup.py` & `swiftshadow-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     name="swiftshadow",
     author="Sachin Sankar",
     author_email="mail.sachinsankar@gmail.com",
     url="https://github.com/sachin-sankar/swiftshadow",
     description="Free IP Proxy rotator for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version=VERSION.get("__version__", "0.2.3"),
+    version=VERSION.get("__version__", "1.0.0"),
     packages=find_packages(where=".", exclude=["tests"]),
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
     ],
 )
```

### Comparing `swiftshadow-0.2.3/swiftshadow/constants.py` & `swiftshadow-1.0.0/swiftshadow/constants.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.3/swiftshadow/helpers.py` & `swiftshadow-1.0.0/swiftshadow/helpers.py`

 * *Files identical despite different names*

### Comparing `swiftshadow-0.2.3/swiftshadow/providers.py` & `swiftshadow-1.0.0/swiftshadow/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from swiftshadow.helpers import getCountryCode, checkProxy, log
 
 
 def Scrapingant(max, countries=[], protocol="http"):
     result = []
     count = 0
     raw = get("https://scrapingant.com/proxies").text
-    log("info", "Updating proxies from ScrapingAnt")
     rows = [i.split("<td>") for i in raw.split("<tr>")]
 
     def clean(text):
         return text[: text.find("<")].strip()
 
     for row in rows[2:]:
         if count == max:
@@ -29,15 +28,14 @@
     return result
 
 
 def Proxyscrape(max, countries=[], protocol="http"):
     result = []
     count = 0
     query = "https://api.proxyscrape.com/v2/?timeout=5000&request=displayproxies&protocol=http"
-    log("info", "Updating proxies from Proxyscrape")
     if countries == []:
         query += "&country=all"
     else:
         query += "&country=" + ",".join(countries)
     if protocol == "https":
         query += "&ssl=yes"
     ips = get(query).text
```

### Comparing `swiftshadow-0.2.3/swiftshadow/swiftshadow.py` & `swiftshadow-1.0.0/swiftshadow/classes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from requests import get
 from random import choice
 from datetime import datetime, timezone, timedelta
 from json import dump, load
 from swiftshadow.helpers import log
-from swiftshadow.providers import Proxyscrape, Scrapingant
+from swiftshadow.providers import Proxyscrape, Scrapingant, Providers
 import swiftshadow.cache as cache
+import os
 
 
 class Proxy:
     def __init__(
         self,
         countries: list = [],
         protocol: str = "http",
         maxProxies: int = 10,
         autoRotate: bool = False,
         cachePeriod: int = 10,
+        cacheFolder: str = "",
     ):
         """
         The one class for everything.
 
         Proxy class contains all necessary methods required to use swiftshadow.
 
         Args:
                 countries: ISO 3166-2 Two letter country codes to filter proxies.
                 protocol: HTTP/HTTPS protocol to filter proxies.
                 maxProxies: Maximum number of proxies to store and rotate from.
                 autoRotate: Rotates proxy when `Proxy.proxy()` function is called.
                 cachePeriod: Time to cache proxies in minutes.
+                cacheFolder: Folder to store cache file.
 
         Returns:
                 proxyClass (swiftshadow.Proxy): `swiftshadow.Proxy` class instance
 
         Examples:
                 Simplest way to get a proxy
                 >>> from swiftshadow.swiftshadow import Proxy
@@ -41,14 +44,18 @@
                 Proxies are sourced from **Proxyscrape** and **Scrapingant** websites which are freely available and validated locally.
         """
         self.countries = [i.upper() for i in countries]
         self.protocol = protocol
         self.maxProxies = maxProxies
         self.autoRotate = autoRotate
         self.cachePeriod = cachePeriod
+        if cacheFolder != "":
+            self.cacheFilePath = ".swiftshadow.json"
+        else:
+            self.cacheFilePath = f"{cacheFolder}/.swiftshadow.json"
 
         self.update()
 
     def checkIp(self, ip, cc, protocol):
         if (ip[1] == cc or cc == None) and ip[2] == protocol:
             proxy = {ip[2]: ip[0]}
             try:
@@ -60,15 +67,15 @@
             else:
                 return False
         else:
             return False
 
     def update(self):
         try:
-            with open(".swiftshadow.json", "r") as file:
+            with open(self.cacheFilePath, "r") as file:
                 data = load(file)
                 self.expiry = data[0]
                 expired = cache.checkExpiry(self.expiry)
             if not expired:
                 log(
                     "info",
                     f"Loaded proxies from cache",
@@ -93,15 +100,15 @@
             )
         if len(self.proxies) == 0:
             log(
                 "warning",
                 "No proxies found for current settings. To prevent runtime error updating the proxy list again.",
             )
             self.update()
-        with open(".swiftshadow.json", "w") as file:
+        with open(self.cacheFilePath, "w") as file:
             self.expiry = cache.getExpiry(self.cachePeriod).isoformat()
             dump([self.expiry, self.proxies], file)
         self.current = self.proxies[0]
 
     def rotate(self):
         """
         Rotate the current proxy.
@@ -124,7 +131,36 @@
         """
         if cache.checkExpiry(self.expiry):
             self.update()
         if self.autoRotate == True:
             return choice(self.proxies)
         else:
             return self.current
+
+
+class ProxyChains:
+    def __init__(
+        self, countries: list = [], protocol: str = "http", maxProxies: int = 10
+    ):
+        self.countries = [i.upper() for i in countries]
+        self.protocol = protocol
+        self.maxProxies = maxProxies
+        self.update()
+
+    def update(self):
+        proxies = []
+        for provider in Providers:
+            print(len(proxies))
+            if len(proxies) == self.maxProxies:
+                break
+            log("INFO", f"{provider}")
+            for proxyDict in provider(self.maxProxies, self.countries, self.protocol):
+                proxyRaw = list(proxyDict.items())[0]
+                proxy = f'{proxyRaw[0]} {proxyRaw[1].replace(":"," ")}'
+                proxies.append(proxy)
+        proxies = "\n".join(proxies)
+        configFileName = "swiftshadow-proxychains.conf"
+        config = f"random_chain\nchain_len=1\nproxy_dns\n[ProxyList]\n{proxies}"
+        with open(configFileName, "w") as file:
+            file.write(config)
+        cmd = f"proxychains -f {os.path.abspath(configFileName)}"
+        os.system(cmd)
```

### Comparing `swiftshadow-0.2.3/swiftshadow.egg-info/PKG-INFO` & `swiftshadow-1.0.0/swiftshadow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: swiftshadow
-Version: 0.2.3
+Version: 1.0.0
 Summary: Free IP Proxy rotator for python
 Home-page: https://github.com/sachin-sankar/swiftshadow
 Author: Sachin Sankar
 Author-email: mail.sachinsankar@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Swiftshadow
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/swiftshadow) ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/sachin-sankar/swiftshadow?include_prereleases&style=flat)
 ## About
@@ -26,17 +28,17 @@
 ``` py
 pip install swiftshadow
 ```
 
 ## One class rules all
 Everything in swiftshadow is under one class for ease of use and minimal code.
 
-Get a proxy using just 3 lines of code!
+Get a proxy using just 2 lines of code!
 ``` py
-from swiftshadow.swiftshadow import Proxy
+from swiftshadow.swiftshadow import QuickProxy
 
-swift = Proxy()
-print(swift.proxy())
+print(QuickProxy())
 ```
 That was easy. 
 
 Head to [Documentation](https://sachin-sankar.github.io/swiftshadow/) to get started.
+
```

