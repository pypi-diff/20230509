# Comparing `tmp/TCLR-1.7.3.tar.gz` & `tmp/TCLR-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCLR-1.7.3.tar", last modified: Tue May  9 02:11:39 2023, max compression
+gzip compressed data, was "TCLR-1.7.4.tar", last modified: Tue May  9 02:22:25 2023, max compression
```

## Comparing `TCLR-1.7.3.tar` & `TCLR-1.7.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 02:11:39.946218 TCLR-1.7.3/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 02:11:39.946096 TCLR-1.7.3/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.7.3/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 02:11:39.945242 TCLR-1.7.3/TCLR/
--rw-r-----   0 jacob      (501) staff       (20)    36528 2023-05-09 02:11:21.000000 TCLR-1.7.3/TCLR/TCLRalgorithm.py
--rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.7.3/TCLR/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 02:11:39.945929 TCLR-1.7.3/TCLR.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 02:11:39.000000 TCLR-1.7.3/TCLR.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-09 02:11:39.000000 TCLR-1.7.3/TCLR.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-09 02:11:39.000000 TCLR-1.7.3/TCLR.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-09 02:11:39.000000 TCLR-1.7.3/TCLR.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-09 02:11:39.000000 TCLR-1.7.3/TCLR.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-09 02:11:39.946255 TCLR-1.7.3/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-09 02:11:36.000000 TCLR-1.7.3/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 02:22:25.201777 TCLR-1.7.4/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 02:22:25.201648 TCLR-1.7.4/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     2570 2022-08-21 10:21:47.000000 TCLR-1.7.4/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 02:22:25.200888 TCLR-1.7.4/TCLR/
+-rw-r-----   0 jacob      (501) staff       (20)    36640 2023-05-09 02:21:47.000000 TCLR-1.7.4/TCLR/TCLRalgorithm.py
+-rw-r--r--   0 jacob      (501) staff       (20)      981 2023-05-08 04:07:49.000000 TCLR-1.7.4/TCLR/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2023-05-09 02:22:25.201480 TCLR-1.7.4/TCLR.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     3228 2023-05-09 02:22:25.000000 TCLR-1.7.4/TCLR.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      196 2023-05-09 02:22:25.000000 TCLR-1.7.4/TCLR.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2023-05-09 02:22:25.000000 TCLR-1.7.4/TCLR.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       30 2023-05-09 02:22:25.000000 TCLR-1.7.4/TCLR.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        5 2023-05-09 02:22:25.000000 TCLR-1.7.4/TCLR.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2023-05-09 02:22:25.201816 TCLR-1.7.4/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1440 2023-05-09 02:22:11.000000 TCLR-1.7.4/setup.py
```

### Comparing `TCLR-1.7.3/PKG-INFO` & `TCLR-1.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.7.3
+Version: 1.7.4
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.7.3/README.md` & `TCLR-1.7.4/README.md`

 * *Files identical despite different names*

### Comparing `TCLR-1.7.3/TCLR/TCLRalgorithm.py` & `TCLR-1.7.4/TCLR/TCLRalgorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,29 +178,32 @@
     os.makedirs('Segmented', exist_ok=True)
     # global var. for statisticaling  results
     global record
     record = 0
     timename = time.localtime(time.time())
     namey, nameM, named, nameh, namem = timename.tm_year, timename.tm_mon, timename.tm_mday, timename.tm_hour, timename.tm_min
 
-    input_csvData = pd.read_csv(filePath)
-    
+    read_csvData = pd.read_csv(filePath)
+
+    input_csvData = read_csvData.iloc[:,:-1]
     if Generate_Features == True:
         # cal an appropriate value of batch
         if len(input_csvData) - 1 <= 3:
             batch = 1
         else:
             batch = 3
         # generate new dataset
         for epoch in range(epochs):
             input_csvData = generate_random_features(input_csvData,[column for column in input_csvData],batch)
+        csvData = input_csvData.assign(response=read_csvData.iloc[:,-1])
+
     else:
-        pass
+        csvData = read_csvData
+    
     
-    csvData = input_csvData
     copy_csvData = copy.deepcopy(csvData)
     copy_csvData['slope'] = None
     copy_csvData['intercept'] = None
     copy_csvData[correlation] = None
     copy_csvData.to_csv('Segmented/all_dataset.csv', index=False)
 
     feats = [column for column in csvData]
```

### Comparing `TCLR-1.7.3/TCLR/__init__.py` & `TCLR-1.7.4/TCLR/__init__.py`

 * *Files identical despite different names*

### Comparing `TCLR-1.7.3/TCLR.egg-info/PKG-INFO` & `TCLR-1.7.4/TCLR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCLR
-Version: 1.7.3
+Version: 1.7.4
 Summary: Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.
 Home-page: https://github.com/Bin-Cao/TCLRmodel
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `TCLR-1.7.3/setup.py` & `TCLR-1.7.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='TCLR',  # 包名
-    version='1.7.3',  # 版本
+    version='1.7.4',  # 版本
     description="Tree-Classifier for Linear Regression (TCLR) is a novel tree model to capture the functional relationships between features and a target based on correlation.",  # 包简介
     long_description=open('README.md',encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='CaoBin',  # 作者
     author_email='bcao@shu.edu.com',  # 作者邮件
     maintainer='CaoBin',  # 维护者
     maintainer_email='binjacobcao@gmail.com',  # 维护者邮件
```

