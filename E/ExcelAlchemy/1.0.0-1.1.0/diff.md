# Comparing `tmp/ExcelAlchemy-1.0.0.tar.gz` & `tmp/ExcelAlchemy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExcelAlchemy-1.0.0.tar", last modified: Sat May  6 02:07:47 2023, max compression
+gzip compressed data, was "ExcelAlchemy-1.1.0.tar", last modified: Tue May  9 10:04:43 2023, max compression
```

## Comparing `ExcelAlchemy-1.0.0.tar` & `ExcelAlchemy-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1073 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     6282 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/README.md
--rw-r--r--   0        0        0     3182 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/__init__.py
--rw-r--r--   0        0        0     3199 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/const.py
--rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/__init__.py
--rw-r--r--   0        0        0     1674 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/abstract.py
--rw-r--r--   0        0        0    37296 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/alchemy.py
--rw-r--r--   0        0        0    18140 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/core/writer.py
--rw-r--r--   0        0        0     2067 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/exc.py
--rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/helper/__init__.py
--rw-r--r--   0        0        0     7334 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/helper/pydantic.py
--rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/py.typed
--rw-r--r--   0        0        0        0 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/__init__.py
--rw-r--r--   0        0        0     3724 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/abstract.py
--rw-r--r--   0        0        0     4790 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/alchemy.py
--rw-r--r--   0        0        0    15756 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/field.py
--rw-r--r--   0        0        0      941 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/header.py
--rw-r--r--   0        0        0      546 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/identity.py
--rw-r--r--   0        0        0     2676 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/result.py
--rw-r--r--   0        0        0      377 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/__init__.py
--rw-r--r--   0        0        0     1703 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/boolean.py
--rw-r--r--   0        0        0     3997 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/date.py
--rw-r--r--   0        0        0     6463 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/date_range.py
--rw-r--r--   0        0        0      748 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/email.py
--rw-r--r--   0        0        0      341 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/money.py
--rw-r--r--   0        0        0     2724 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/multi_checkbox.py
--rw-r--r--   0        0        0     5335 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/number.py
--rw-r--r--   0        0        0     4203 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/number_range.py
--rw-r--r--   0        0        0     2440 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/organization.py
--rw-r--r--   0        0        0      498 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/phone_number.py
--rw-r--r--   0        0        0     2262 2023-05-06 02:07:34.650865 ExcelAlchemy-1.0.0/excelalchemy/types/value/radio.py
--rw-r--r--   0        0        0     2547 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/staff.py
--rw-r--r--   0        0        0     4898 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/string.py
--rw-r--r--   0        0        0     1914 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/tree.py
--rw-r--r--   0        0        0      659 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/types/value/url.py
--rw-r--r--   0        0        0        0 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/util/__init__.py
--rw-r--r--   0        0        0     1557 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/util/convertor.py
--rw-r--r--   0        0        0     2736 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/excelalchemy/util/file.py
--rw-r--r--   0        0        0     2487 2023-05-06 02:07:34.654865 ExcelAlchemy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 ExcelAlchemy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-09 10:04:32.759201 ExcelAlchemy-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0     6282 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/README.md
+-rw-r--r--   0        0        0     3182 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/__init__.py
+-rw-r--r--   0        0        0     3199 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/const.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/core/__init__.py
+-rw-r--r--   0        0        0     1674 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/core/abstract.py
+-rw-r--r--   0        0        0    37318 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/core/alchemy.py
+-rw-r--r--   0        0        0    18140 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/core/writer.py
+-rw-r--r--   0        0        0     2067 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/exc.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/helper/__init__.py
+-rw-r--r--   0        0        0     7334 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/helper/pydantic.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/py.typed
+-rw-r--r--   0        0        0        0 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/__init__.py
+-rw-r--r--   0        0        0     3724 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/abstract.py
+-rw-r--r--   0        0        0     4790 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/alchemy.py
+-rw-r--r--   0        0        0    15756 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/field.py
+-rw-r--r--   0        0        0      941 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/header.py
+-rw-r--r--   0        0        0      546 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/identity.py
+-rw-r--r--   0        0        0     2676 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/result.py
+-rw-r--r--   0        0        0      377 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/__init__.py
+-rw-r--r--   0        0        0     1703 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/boolean.py
+-rw-r--r--   0        0        0     3997 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/date.py
+-rw-r--r--   0        0        0     6463 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/date_range.py
+-rw-r--r--   0        0        0      748 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/email.py
+-rw-r--r--   0        0        0      341 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/money.py
+-rw-r--r--   0        0        0     2724 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/multi_checkbox.py
+-rw-r--r--   0        0        0     5335 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/number.py
+-rw-r--r--   0        0        0     4203 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/number_range.py
+-rw-r--r--   0        0        0     2440 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/organization.py
+-rw-r--r--   0        0        0      498 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/phone_number.py
+-rw-r--r--   0        0        0     2262 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/radio.py
+-rw-r--r--   0        0        0     2547 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/staff.py
+-rw-r--r--   0        0        0     4898 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/string.py
+-rw-r--r--   0        0        0     1914 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/tree.py
+-rw-r--r--   0        0        0      659 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/types/value/url.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/util/__init__.py
+-rw-r--r--   0        0        0     1557 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/util/convertor.py
+-rw-r--r--   0        0        0     2736 2023-05-09 10:04:32.763201 ExcelAlchemy-1.1.0/excelalchemy/util/file.py
+-rw-r--r--   0        0        0     2499 2023-05-09 10:04:32.767201 ExcelAlchemy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7326 1970-01-01 00:00:00.000000 ExcelAlchemy-1.1.0/PKG-INFO
```

### Comparing `ExcelAlchemy-1.0.0/LICENSE` & `ExcelAlchemy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/README.md` & `ExcelAlchemy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/__init__.py` & `ExcelAlchemy-1.1.0/excelalchemy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A Python Library for Reading and Writing Excel Files"""
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 from excelalchemy.const import CharacterSet
 from excelalchemy.const import DataRangeOption
 from excelalchemy.const import DateFormat
 from excelalchemy.const import Option
 from excelalchemy.core.alchemy import ExcelAlchemy
 from excelalchemy.exc import ConfigError
 from excelalchemy.exc import ExcelCellError
```

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/const.py` & `ExcelAlchemy-1.1.0/excelalchemy/const.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/core/abstract.py` & `ExcelAlchemy-1.1.0/excelalchemy/core/abstract.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/core/alchemy.py` & `ExcelAlchemy-1.1.0/excelalchemy/core/alchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,48 +132,47 @@
         self.__init_field_meta__(importer_model)
 
     def __init_field_meta__(self, importer_model: type[BaseModel]) -> None:
         """从配置类初始化"""
         self.field_metas = extract_pydantic_model(importer_model)
         self._check_field_meta_order(self.field_metas)
         if len(self.field_metas) == 0:
-            raise ConfigError(f'没有从模型 {importer_model} 中提取到字段元数据，请检查模型是否定义了字段')
+            raise ConfigError(f'没有从模型 {importer_model.__name__} 中提取到字段元数据，请检查模型是否定义了字段')
         self.ordered_field_meta: list[FieldMetaInfo] = self._sort_field_meta(self.field_metas)  # type: ignore[no-redef]
 
         for field_meta in self.ordered_field_meta:
             if field_meta.parent_label is None:
                 raise ConfigError('父标签不能为空')
             if field_meta.parent_key is None:
                 raise ConfigError('父键不能为空')
 
             self.parent_label_to_field_metas.setdefault(field_meta.parent_label, []).append(field_meta)
             self.parent_key_to_field_metas.setdefault(field_meta.parent_key, []).append(field_meta)
             self.unique_key_to_field_meta[field_meta.unique_key] = field_meta
             self.unique_label_to_field_meta[field_meta.unique_label] = field_meta
 
     def __get_importer_model__(self) -> type[ImporterCreateModelT] | type[ImporterUpdateModelT] | type[ExporterModelT]:
+        importer_model = None
         if self.excel_mode == ExcelMode.IMPORT:
             if not isinstance(self.config, ImporterConfig):
-                raise TypeError(f'导入模式的配置类必须是 {ImporterConfig.__name__}')
+                raise ConfigError(f'导入模式的配置类必须是 {ImporterConfig.__name__}')
             if self.config.import_mode in (ImportMode.CREATE, ImportMode.CREATE_OR_UPDATE):
                 importer_model = self.config.create_importer_model  # type: ignore[assignment]
             elif self.config.import_mode == ImportMode.UPDATE:
                 importer_model = self.config.update_importer_model  # type: ignore[assignment]
-            else:
-                raise ConfigError('不支持的导入模式')
 
         elif self.excel_mode == ExcelMode.EXPORT:
             if not isinstance(self.config, ExporterConfig):
-                raise TypeError(f'导出模式的配置类必须是 {ExporterConfig.__name__}')
+                raise ConfigError(f'导出模式的配置类必须是 {ExporterConfig.__name__}')
             importer_model = self.config.exporter_model  # type: ignore[assignment]
 
-        else:
-            raise ConfigError('不支持的模式')
+        if importer_model is None:
+            raise ConfigError('请检查配置类是否定义了导入模型或导出模型')
 
-        return importer_model  # type: ignore
+        return importer_model
 
     @staticmethod
     def _check_field_meta_order(field_metas: list[FieldMetaInfo]) -> None:
         """检查字段顺序是否有重复"""
         order_to_field_meta: dict[int, set[Label]] = defaultdict(set)
         for field_meta in field_metas:
             assert field_meta.parent_label is not None  # only for mypy, remove this line at runtime if you want
@@ -350,15 +349,15 @@
         input_labels = [x.label for x in self.input_excel_headers]
 
         visited = set()
         duplicated = [x for x in input_labels if x in visited or visited.add(x)]  # type: ignore[func-returns-value]
         unrecognized = list(set(input_labels) - set(x.label for x in self.ordered_field_meta))
 
         missing_primary, missing_required = [], []
-        if self.config == ImportMode.UPDATE:
+        if self.config.import_mode == ImportMode.UPDATE:
             missing_primary = list(set(primary_labels) - set(input_labels))
 
         missing_required = list(set(required_labels) - set(input_labels) - set(missing_primary))
 
         return ValidateHeaderResult(
             unrecognized=unrecognized,
             duplicated=duplicated,
```

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/core/writer.py` & `ExcelAlchemy-1.1.0/excelalchemy/core/writer.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/exc.py` & `ExcelAlchemy-1.1.0/excelalchemy/exc.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/helper/pydantic.py` & `ExcelAlchemy-1.1.0/excelalchemy/helper/pydantic.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/abstract.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/abstract.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/alchemy.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/alchemy.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/field.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/field.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/header.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/header.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/identity.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/identity.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/result.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/result.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/boolean.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/boolean.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/date.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/date.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/date_range.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/date_range.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/email.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/email.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/multi_checkbox.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/multi_checkbox.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/number.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/number.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/number_range.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/number_range.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/organization.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/organization.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/radio.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/radio.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/staff.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/staff.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/string.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/string.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/tree.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/tree.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/types/value/url.py` & `ExcelAlchemy-1.1.0/excelalchemy/types/value/url.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/util/convertor.py` & `ExcelAlchemy-1.1.0/excelalchemy/util/convertor.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/excelalchemy/util/file.py` & `ExcelAlchemy-1.1.0/excelalchemy/util/file.py`

 * *Files identical despite different names*

### Comparing `ExcelAlchemy-1.0.0/pyproject.toml` & `ExcelAlchemy-1.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
+requires = ['flit_core >=3.2,<4']
+build-backend = 'flit_core.buildapi'
 
 [project]
-name = "ExcelAlchemy"
-authors = [{ name = "何睿", email = "hrui835@gmail.com" }]
-readme = "README.md"
-license = { file = "LICENSE" }
-classifiers = ["License :: OSI Approved :: MIT License"]
-dynamic = ["version", "description"]
-requires-python = ">=3.10"
+name = 'ExcelAlchemy'
+authors = [{ name = '何睿', email = 'hrui835@gmail.com' }]
+readme = 'README.md'
+license = { file = 'LICENSE' }
+classifiers = ['License :: OSI Approved :: MIT License']
+dynamic = ['version', 'description']
+requires-python = '>=3.10'
 dependencies = [
-    "pandas >=1.5.1, <1.6",
-    "minio >=7.0.0, <8",
-    "pydantic[email] >=1.9, <2",
-    "openpyxl >=3.0.10, <4",
+    'pandas >=2.0.0, <2.1.0',
+    'minio >=7.0.0, <8',
+    'pydantic[email] >=1.9, <2',
+    'openpyxl >=3.0.10, <4',
     'pendulum >=2.1.2, <3',
 ]
 
 [tool.flit.module]
-name = "excelalchemy"
+name = 'excelalchemy'
 
 [project.urls]
-Home = "https://github.com/SundayWindy/excelalchemy"
+Home = 'https://github.com/SundayWindy/excelalchemy'
 
 [project.optional-dependencies]
 development = [
-    "pandas-stubs",
-    "black",
-    "isort",
-    "mypy",
-    "pylint",
-    "pre-commit",
-    "pyright",
-    "pytest",
-    "coverage",
-    "pytest-cov",
+    'pandas-stubs',
+    'black',
+    'isort',
+    'mypy',
+    'pylint',
+    'pre-commit',
+    'pyright==1.1.299',
+    'pytest',
+    'coverage',
+    'pytest-cov',
 ]
 
 [tool.pyright]
 exclude = [
-    ".venv",
-    "venv",
-    ".git",
-    "**/.mypy_cache",
-    "**/__pycache__",
-    "**/.pytest_cache",
+    '.venv',
+    'venv',
+    '.git',
+    '**/.mypy_cache',
+    '**/__pycache__',
+    '**/.pytest_cache',
 ]
-ignore = ["pands"]
+ignore = ['pandas']
 enableTypeIgnoreComments = false
 reportUnusedFunction = false
-typeCheckingMode = "strict"
+typeCheckingMode = 'strict'
 reportUnusedImport = false
 reportMissingTypeStubs = false
 reportUnknownVariableType = false
 
 
-extension-pkg-whitelist = ["pydantic", 'pendulum']
+extension-pkg-whitelist = ['pydantic', 'pendulum']
 
 [tool.pylint.basic]
-attr-rgx = "^[_a-z][a-z0-9_]*$"        # snake_case
-variable-rgx = "^[_a-z][a-z0-9_]*$"    # snake_case
-argument-rgx = "^[_a-z][a-z0-9_]*$"    # snake_case
-class-rgx = "^(_?[A-Z][a-zA-Z0-9]*)*$"
-method-rgx = "^[_a-z][a-z0-9_]*$"      # snake_case
+attr-rgx = '^[_a-z][a-z0-9_]*$'        # snake_case
+variable-rgx = '^[_a-z][a-z0-9_]*$'    # snake_case
+argument-rgx = '^[_a-z][a-z0-9_]*$'    # snake_case
+class-rgx = '^(_?[A-Z][a-zA-Z0-9]*)*$'
+method-rgx = '^[_a-z][a-z0-9_]*$'      # snake_case
 
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = [
-    "missing-module-docstring",
-    "missing-function-docstring",
-    "missing-class-docstring",
-    "too-many-instance-attributes",
-    "too-many-arguments",
-    "too-few-public-methods",
-    "too-many-public-methods",
-    "no-else-return",
-    "no-else-raise",
-    "fixme",
-    "duplicate-code",
-    "redefined-builtin",
-    "broad-except",
-    "abstract-class-instantiated"
+    'missing-module-docstring',
+    'missing-function-docstring',
+    'missing-class-docstring',
+    'too-many-instance-attributes',
+    'too-many-arguments',
+    'too-few-public-methods',
+    'too-many-public-methods',
+    'no-else-return',
+    'no-else-raise',
+    'fixme',
+    'duplicate-code',
+    'redefined-builtin',
+    'broad-except',
+    'abstract-class-instantiated'
 ]
 
 
 [tool.pylint.'MASTER']
 jobs = 4
 score = false
 ignore-paths = [
-    ".git/",
-    "venv/",
-    ".venv/",
-    ".mypy_cache/",
-    "__pycache__/",
-    ".pytest_cache/",
-    "tests/",
-    "dist/",
+    '.git/',
+    'venv/',
+    '.venv/',
+    '.mypy_cache/',
+    '__pycache__/',
+    '.pytest_cache/',
+    'tests/',
+    'dist/',
 ]
 extension-pkg-whitelist = [
-    "pydantic",
-    "pandas",
-    "pendulum",
+    'pydantic',
+    'pandas',
+    'pendulum',
 
 ]
 
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 
 
 [tool.pylint.'FORMAT']
 max-line-length = 120
 
 [tool.isort]
 skip_gitignore = true
-profile = "black"
+profile = 'black'
 line_length = 120
 indent = '    '
 no_lines_before = 'LOCALFOLDER'
 force_single_line = true
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `ExcelAlchemy-1.0.0/PKG-INFO` & `ExcelAlchemy-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: ExcelAlchemy
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python Library for Reading and Writing Excel Files
 Author-email: 何睿 <hrui835@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: pandas >=1.5.1, <1.6
+Requires-Dist: pandas >=2.0.0, <2.1.0
 Requires-Dist: minio >=7.0.0, <8
 Requires-Dist: pydantic[email] >=1.9, <2
 Requires-Dist: openpyxl >=3.0.10, <4
 Requires-Dist: pendulum >=2.1.2, <3
 Requires-Dist: pandas-stubs ; extra == "development"
 Requires-Dist: black ; extra == "development"
 Requires-Dist: isort ; extra == "development"
 Requires-Dist: mypy ; extra == "development"
 Requires-Dist: pylint ; extra == "development"
 Requires-Dist: pre-commit ; extra == "development"
-Requires-Dist: pyright ; extra == "development"
+Requires-Dist: pyright==1.1.299 ; extra == "development"
 Requires-Dist: pytest ; extra == "development"
 Requires-Dist: coverage ; extra == "development"
 Requires-Dist: pytest-cov ; extra == "development"
 Project-URL: Home, https://github.com/SundayWindy/excelalchemy
 Provides-Extra: development
 
 > [中文](https://github.com/SundayWindy/ExcelAlchemy/blob/main/README_cn.md) | English
```

