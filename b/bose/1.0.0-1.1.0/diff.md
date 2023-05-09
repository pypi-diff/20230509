# Comparing `tmp/bose-1.0.0.tar.gz` & `tmp/bose-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.0.0.tar", last modified: Tue May  9 11:46:21 2023, max compression
+gzip compressed data, was "bose-1.1.0.tar", last modified: Tue May  9 15:57:22 2023, max compression
```

## Comparing `bose-1.0.0.tar` & `bose-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 11:46:21.286920 bose-1.0.0/
--rw-rw-rw-   0        0        0     8678 2023-05-09 11:46:21.287922 bose-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-09 11:46:21.285921 bose-1.0.0/bose/
--rw-rw-rw-   0        0        0      261 2023-05-09 11:34:21.555551 bose-1.0.0/bose/__init__.py
--rw-rw-rw-   0        0        0     2861 2023-05-09 09:08:49.452740 bose-1.0.0/bose/base_data.py
--rw-rw-rw-   0        0        0     3227 2023-05-09 08:59:20.033214 bose-1.0.0/bose/base_task.py
--rw-rw-rw-   0        0        0     7193 2023-05-09 11:34:44.632406 bose-1.0.0/bose/create_driver.py
--rw-rw-rw-   0        0        0     1559 2023-05-09 09:26:46.769040 bose-1.0.0/bose/download_driver.py
--rw-rw-rw-   0        0        0     2493 2023-05-09 07:32:15.014678 bose-1.0.0/bose/local_storage.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.0.0/bose/opponent.py
--rw-rw-rw-   0        0        0     3004 2023-05-09 11:34:21.555551 bose-1.0.0/bose/output.py
--rw-rw-rw-   0        0        0     1659 2023-05-09 08:45:01.078947 bose-1.0.0/bose/task_info.py
--rw-rw-rw-   0        0        0     7304 2023-05-09 09:07:17.734961 bose-1.0.0/bose/user_agent.py
--rw-rw-rw-   0        0        0     5882 2023-05-09 11:32:50.275917 bose-1.0.0/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.0.0/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.0.0/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2189 2023-05-09 11:46:16.633043 bose-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 15:57:22.667518 bose-1.1.0/
+-rw-rw-rw-   0        0        0     8678 2023-05-09 15:57:22.669516 bose-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 15:57:22.667518 bose-1.1.0/bose/
+-rw-rw-rw-   0        0        0      303 2023-05-09 12:16:48.786461 bose-1.1.0/bose/__init__.py
+-rw-rw-rw-   0        0        0     2861 2023-05-09 09:08:49.452740 bose-1.1.0/bose/base_data.py
+-rw-rw-rw-   0        0        0     3646 2023-05-09 15:26:36.574181 bose-1.1.0/bose/base_task.py
+-rw-rw-rw-   0        0        0     7265 2023-05-09 15:15:30.436760 bose-1.1.0/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1559 2023-05-09 09:26:46.769040 bose-1.1.0/bose/download_driver.py
+-rw-rw-rw-   0        0        0     2493 2023-05-09 07:32:15.014678 bose-1.1.0/bose/local_storage.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.1.0/bose/opponent.py
+-rw-rw-rw-   0        0        0     3173 2023-05-09 15:50:46.922925 bose-1.1.0/bose/output.py
+-rw-rw-rw-   0        0        0     1654 2023-05-09 12:06:31.715212 bose-1.1.0/bose/task_info.py
+-rw-rw-rw-   0        0        0     7337 2023-05-09 11:56:53.677609 bose-1.1.0/bose/user_agent.py
+-rw-rw-rw-   0        0        0     5882 2023-05-09 11:32:50.275917 bose-1.1.0/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.1.0/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.1.0/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2189 2023-05-09 15:57:09.812603 bose-1.1.0/setup.py
```

### Comparing `bose-1.0.0/PKG-INFO` & `bose-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 1.0.0
+Version: 1.1.0
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: # Bose - The Ultimate Web Scraping Framework!
```

### Comparing `bose-1.0.0/bose/base_data.py` & `bose-1.1.0/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.0.0/bose/base_task.py` & `bose-1.1.0/bose/base_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import os
 import traceback
 from bose.create_driver import BrowserConfig, create_driver
 from bose.drivers.boss_driver import BossDriver
-from bose.utils import merge_dicts_in_one_dict, write_file, write_html, write_json
-from local_storage import LocalStorage
-from task_info import TaskInfo
+from bose.utils import relative_path, merge_dicts_in_one_dict, write_file, write_html, write_json
+from .local_storage import LocalStorage
+from .task_info import TaskInfo
 
 
 class RetryException(Exception):
     pass
 
 def get_driver_url_safe(driver):
     try:
@@ -26,23 +27,30 @@
         pass
 
     browser_config = BrowserConfig()
 
     def get_browser_config(self):
         return self.browser_config
 
-    def create_driver(config: BrowserConfig):
-        create_driver(config)
+    def create_driver(self, config: BrowserConfig):
+        return create_driver(config)
     
     def begin_task(self):
+        def create_task_directory(task_path):
+            path =  relative_path(task_path, 0)
+            if not os.path.exists(path):
+                os.makedirs(path)
+            else:
+                pass
+
         def run_task(is_retry, retry_attempt):
             task = TaskInfo()
             print('Task Started')
             task.start()
-
+            
             def end_task(driver:BossDriver):
                 task.end()
                 task.set_ip()
                 data = task.data
                 driver.save_screenshot()
                 
                 html_path  = f'{self.task_path}/page.html'
@@ -50,16 +58,18 @@
                 write_html(source, html_path)
 
                 data["driver_url"] = get_driver_url_safe(driver)
                 
                 if is_retry: 
                     data["is_retry"] = is_retry
                     data["retry_attempt"] = retry_attempt
-                
+
+                print("Closing Browser")                
                 driver.close()
+                print("Closed Browser")                
 
                 task_info_path  = f'{self.task_path}/task_info.json'
                 
                 if driver._init_data is not None:
                     data = merge_dicts_in_one_dict(data , driver._init_data)
                 
                 write_json(data , task_info_path)
@@ -68,14 +78,15 @@
             LocalStorage.set_item('count', count)
 
             driver = self.create_driver(self.get_browser_config())
 
             self.task_path = f'tasks/{count}' 
             self.task_id = count
 
+            create_task_directory(self.task_path)
             driver.task_id = self.task_id
             driver.task_path = self.task_path
 
 
             try:
                 self.run(driver)
                 end_task(driver)
```

### Comparing `bose-1.0.0/bose/create_driver.py` & `bose-1.1.0/bose/create_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from selenium.common.exceptions import WebDriverException
 from bose.user_agent import UserAgentInstance, UserAgent
 from bose.window_size import WindowSize, WindowSizeInstance
-from bose.utils import relative_path, silentremove
+from bose.utils import NETWORK_ERRORS, is_windows, relative_path, retry_if_is_error, silentremove
 from selenium.webdriver.chrome.options import Options as GoogleChromeOptions
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
-from undetected_chromedriver.v2 import ChromeOptions
+from undetected_chromedriver import ChromeOptions
 from bose.drivers.boss_driver import BossDriver
 
 from bose.drivers.boss_undetected_driver import BossUndetectedDriver
 import shutil
+import os
 
 class RetryException(Exception):
     pass
 
 
 class BrowserConfig:
     def __init__(self, user_agent=None, window_size=WindowSize.window_size_1920_1080, profile=None, is_eager=False, use_undetected_driver=False):
@@ -65,36 +66,37 @@
     if window_size == None:
         if profile == None:
             window_size = WindowSizeInstance.get_random()
         else:
             window_size = WindowSizeInstance.get_hashed(profile)
     else: 
         if window_size == WindowSize.RANDOM:
-            window_size = WindowSizeInstance.get_random(profile)
+            window_size = WindowSizeInstance.get_random()
         elif window_size == WindowSize.HASHED:
             window_size = WindowSizeInstance.get_hashed(profile)
         else: 
             window_size = window_size
     
     window_size = WindowSize.window_size_to_string(window_size)
     options.add_argument(f"--window-size={window_size}")
 
+    if profile is not None:
+        profile = str(profile)
     if user_agent == None:
         if profile == None:
             user_agent = UserAgentInstance.get_random()
         else:
             user_agent = UserAgentInstance.get_hashed(profile)
     else: 
         if user_agent == UserAgent.RANDOM:
-            user_agent = UserAgentInstance.get_random(profile)
+            user_agent = UserAgentInstance.get_random()
         elif user_agent == UserAgent.HASHED:
             user_agent = UserAgentInstance.get_hashed(profile)
         else: 
             user_agent = user_agent
-
     
     add_useragent(options, user_agent)
 
     has_user = profile is not None
     if has_user:
         path = create_profile_path(profile)
         user_data_path = f"--user-data-dir={path}"
@@ -161,29 +163,28 @@
             desired_capabilities = get_eager_startegy()
         else:
             desired_capabilities = None
         
         print(driver_string)
 
         if is_undetected:
-            driver = BossUndetectedDriver(desired_capabilities=desired_capabilities,
+            driver = BossUndetectedDriver(
+                desired_capabilities=desired_capabilities,
                               options=options
                             )
         else:
             # options.add_experimental_option("prefs",  {"profile.managed_default_content_settings.images": 2})
             hide_automation_flags(options)
             
             # CAPTCHA
             options.arguments.extend(
                 ["--disable-web-security", "--disable-site-isolation-trials", "--disable-application-cache"])
 
             path = relative_path(get_driver_path(), 0)
 
-            print(f'driver path: {path}' )
-
             driver = BossDriver(
                 desired_capabilities=desired_capabilities,
                 chrome_options=options,
                 executable_path=path,
             )
 
         if driver_attributes["profile"] is None:
```

### Comparing `bose-1.0.0/bose/download_driver.py` & `bose-1.1.0/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.0.0/bose/local_storage.py` & `bose-1.1.0/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-1.0.0/bose/output.py` & `bose-1.1.0/bose/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
         if not filename.endswith(".json"):
             filename = filename + ".json"
 
         write_json(data, filename)
-        
+        print(f"View written JSON file at {filename}")        
 
     def write_csv(data, filename):
         """
         Save a list of dictionaries as a CSV file.
 
         Args:
             data: a list of dictionaries
@@ -42,20 +42,20 @@
 
         if not filename.startswith("output/"):
             filename = "output/" +  filename
 
         if not filename.endswith(".csv"):
             filename = filename + ".csv"
 
-        with open('output/'+ filename, 'w', newline='') as csvfile:
+        with open(filename, 'w', newline='') as csvfile:
             fieldnames = data[0].keys()  # get the fieldnames from the first dictionary
             writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
             writer.writeheader()  # write the header row
             writer.writerows(data)  # write each row of data
-
+        print(f"View written CSV file at {filename}")        
     def write_xlsx(data, filename):
         """
         Saves a list of dictionaries as an Excel file with the given filename.
         Each dictionary in the list corresponds to a row in the Excel file.
         The keys of each dictionary correspond to column names in the Excel file.
         """
         if len(data) == 0:
@@ -80,14 +80,15 @@
         if data:
             for row_num, data in enumerate(data, start=2):
                 for col_num, key in enumerate(headers, start=1):
                     ws.cell(row=row_num, column=col_num).value = data.get(key)
 
         # save file
         wb.save(filename)
+        print(f"View written Excel file at {filename}")        
 
     def read_pending():
         return Output.read_json("pending.json")
 
     def write_pending(data):
         return Output.write_json(data, "pending.json")
```

### Comparing `bose-1.0.0/bose/task_info.py` & `bose-1.1.0/bose/task_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,19 +44,18 @@
   
   def start(self):
     self.data["start_time"] = datetime.now()
     pass
   
   def end(self):
     self.data["end_time"] = datetime.now()
-    
     self.data["duration"] = format_time_diff(self.data["start_time"],self.data["end_time"])
     
 
-    self.data["start_time"] =pretty_format_time(self.data["start_time"])
+    self.data["start_time"] = pretty_format_time(self.data["start_time"])
     self.data["end_time"] = pretty_format_time(self.data["end_time"])
 
 
   def set_ip(self):
     self.data["ip_details"] = find_safe_ip()
```

### Comparing `bose-1.0.0/bose/user_agent.py` & `bose-1.1.0/bose/user_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,12 +109,13 @@
 
         result = _106 + _105 + _104 + _103 + \
             _101 + _99 + _100 + _98 + _97 + _96 + _95 + _94
 
         return result
 
 
+UserAgentInstance = UserAgent()
 if __name__ == '__main__':
     UserAgentInstance = UserAgent()
     print(UserAgentInstance.get_hashed('a'))
     print(UserAgentInstance.get_hashed('a'))
     print(UserAgentInstance.get_hashed('b'))
```

### Comparing `bose-1.0.0/bose/utils.py` & `bose-1.1.0/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-1.0.0/bose/window_size.py` & `bose-1.1.0/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.0.0/setup.py` & `bose-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 cpython_dependencies = [
     "PyDispatcher>=2.0.5",
 ]
 
 setup(
     name='bose',
     packages=['bose'],
-    version='1.0.0',
+    version='1.1.0',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/docs/",
         "Source": "https://github.com/omkarcloud/boss",
         "Tracker": "https://github.com/omkarcloud/boss/issues",
     },
```

