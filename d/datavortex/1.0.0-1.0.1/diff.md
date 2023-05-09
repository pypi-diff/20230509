# Comparing `tmp/datavortex-1.0.0.tar.gz` & `tmp/datavortex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datavortex-1.0.0.tar", last modified: Mon May  8 16:44:34 2023, max compression
+gzip compressed data, was "datavortex-1.0.1.tar", last modified: Tue May  9 17:45:54 2023, max compression
```

## Comparing `datavortex-1.0.0.tar` & `datavortex-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 16:44:34.433450 datavortex-1.0.0/
--rw-rw-r--   0 oem      (29999) oem      (29999)     1079 2023-05-08 13:41:26.000000 datavortex-1.0.0/LICENCE
--rw-rw-r--   0 oem      (29999) oem      (29999)      445 2023-05-08 16:44:34.433450 datavortex-1.0.0/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)       75 2023-05-08 13:48:09.000000 datavortex-1.0.0/README.md
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 16:44:34.433450 datavortex-1.0.0/datavortex/
--rw-rw-r--   0 oem      (29999) oem      (29999)       20 2023-05-08 13:36:09.000000 datavortex-1.0.0/datavortex/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)    23977 2023-05-08 13:44:47.000000 datavortex-1.0.0/datavortex/dados.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-08 16:44:34.433450 datavortex-1.0.0/datavortex.egg-info/
--rw-rw-r--   0 oem      (29999) oem      (29999)      445 2023-05-08 16:44:34.000000 datavortex-1.0.0/datavortex.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      238 2023-05-08 16:44:34.000000 datavortex-1.0.0/datavortex.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-05-08 16:44:34.000000 datavortex-1.0.0/datavortex.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       55 2023-05-08 16:44:34.000000 datavortex-1.0.0/datavortex.egg-info/requires.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       11 2023-05-08 16:44:34.000000 datavortex-1.0.0/datavortex.egg-info/top_level.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-05-08 16:44:34.433450 datavortex-1.0.0/setup.cfg
--rw-rw-r--   0 oem      (29999) oem      (29999)      597 2023-05-08 16:44:18.000000 datavortex-1.0.0/setup.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-09 17:45:54.964774 datavortex-1.0.1/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     1079 2023-05-08 13:41:26.000000 datavortex-1.0.1/LICENCE
+-rw-rw-r--   0 oem      (29999) oem      (29999)      687 2023-05-09 17:45:54.964774 datavortex-1.0.1/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      317 2023-05-09 17:43:55.000000 datavortex-1.0.1/README.md
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-09 17:45:54.960775 datavortex-1.0.1/datavortex/
+-rw-rw-r--   0 oem      (29999) oem      (29999)       20 2023-05-08 13:36:09.000000 datavortex-1.0.1/datavortex/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)    24465 2023-05-09 17:43:14.000000 datavortex-1.0.1/datavortex/dados.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-05-09 17:45:54.964774 datavortex-1.0.1/datavortex.egg-info/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      687 2023-05-09 17:45:54.000000 datavortex-1.0.1/datavortex.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      238 2023-05-09 17:45:54.000000 datavortex-1.0.1/datavortex.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-05-09 17:45:54.000000 datavortex-1.0.1/datavortex.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       55 2023-05-09 17:45:54.000000 datavortex-1.0.1/datavortex.egg-info/requires.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       11 2023-05-09 17:45:54.000000 datavortex-1.0.1/datavortex.egg-info/top_level.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-05-09 17:45:54.964774 datavortex-1.0.1/setup.cfg
+-rw-rw-r--   0 oem      (29999) oem      (29999)      597 2023-05-09 17:42:22.000000 datavortex-1.0.1/setup.py
```

### Comparing `datavortex-1.0.0/LICENCE` & `datavortex-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `datavortex-1.0.0/datavortex/dados.py` & `datavortex-1.0.1/datavortex/dados.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,38 +484,52 @@
         logger.info('Gerando informações de correlação...')
         correlacao = data[colunas].corr()
 
         return correlacao
     
 
 class DataProcess:
-    name_sheets = []
-    sheet_selected = pd.DataFrame
     def __init__(self, data: str) -> None:
-        self.data = pd.ExcelFile(data)
+        self.data = data
+        self.__name_sheets = []
+        self.sheet_selected = None
+        self.__file_extension = self.data.split('.')[-1]
+        if self.__file_extension == 'xls' or self.__file_extension == 'xlsx':
+            self.__load_excel()
+        elif self.__file_extension == 'csv':
+            self.__load_csv()
+        else:
+            raise ValueError("Unsupported file format")
+            
+    def __load_excel(self):
+        self.data = pd.ExcelFile(self.data)
         self.__name_sheets = self.data.sheet_names
-    """
-    Class DataProcess
-    Classe responsável por pegar uma planilha do excel e processar ela.
-    :param data: str.
-    """
+        
+    def __load_csv(self):
+        self.__name_sheets = ['Sheet1']
+        
     def sheets(self) -> list:
         """
         Retorna uma lista com os nomes de todas as abas da planilha.
         """
-        logger.info('Gerando lista com nomes das abas do excel...')
         return self.__name_sheets
     
-    def sheet_select(self, sheet: str) -> DataFrame:
+    def sheet_select(self, sheet: str) -> pd.DataFrame:
         """
         Retorna a aba selecionada da planilha em formato de DataFrame.
         :param sheet: str
         """
-        logger.info('Selecionando aba do excel escolhida...')
-        self.sheet_selected = pd.read_excel(self.data, sheet_name=sheet)
+        if self.__file_extension == 'xls' or self.__file_extension == 'xlsx':
+            self.sheet_selected = pd.read_excel(self.data, sheet_name=sheet)
+        elif self.__file_extension == 'csv':
+            df = pd.read_csv(self.data, sep=";")
+
+            return df
+        else:
+            raise ValueError("Unsupported file format")
 
         return self.sheet_selected
     
 
 class Treatment:
     def __init__(self) -> None:
        self.colunas_vazias = []
```

### Comparing `datavortex-1.0.0/setup.py` & `datavortex-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='datavortex',
-    version='1.0.0',
+    version='1.0.1',
     license='MIT License',
     author='Brayan Robert',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='robertbrayan60@gmail.com',
     keywords='dados, analise de dados, processamento de dados, datahub',
     description=u'Classes para processamento, tratamento e análise de dados',
```

