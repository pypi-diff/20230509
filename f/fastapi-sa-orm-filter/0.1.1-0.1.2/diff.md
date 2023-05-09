# Comparing `tmp/fastapi-sa-orm-filter-0.1.1.tar.gz` & `tmp/fastapi-sa-orm-filter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sa-orm-filter-0.1.1.tar", last modified: Sun May  7 20:03:52 2023, max compression
+gzip compressed data, was "fastapi-sa-orm-filter-0.1.2.tar", last modified: Tue May  9 21:00:40 2023, max compression
```

## Comparing `fastapi-sa-orm-filter-0.1.1.tar` & `fastapi-sa-orm-filter-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.1/.github/workflows/ci_filter.yml
--rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.1/LICENSE
--rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.1/Pipfile
--rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.1/Pipfile.lock
--rw-r--r--   0        0        0     2254 2023-05-07 18:27:00.869658 fastapi-sa-orm-filter-0.1.1/README.md
--rw-r--r--   0        0        0      111 2023-05-07 20:03:40.110270 fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/__init__.py
--rw-r--r--   0        0        0      436 2023-05-07 19:08:56.172612 fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/filters.py
--rw-r--r--   0        0        0     9002 2023-05-07 19:44:59.724445 fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/main.py
--rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.1/pytest.ini
--rw-r--r--   0        0        0     3313 2023-05-07 19:52:51.662374 fastapi-sa-orm-filter-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0    14318 2023-05-07 19:52:51.678374 fastapi-sa-orm-filter-0.1.1/tests/test_filter.py
--rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.1/tests/utils.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-05-07 17:56:59.474207 fastapi-sa-orm-filter-0.1.2/.github/workflows/ci_filter.yml
+-rw-r--r--   0        0        0     1073 2023-05-07 07:37:25.294746 fastapi-sa-orm-filter-0.1.2/LICENSE
+-rw-r--r--   0        0        0      271 2023-05-07 14:19:55.337103 fastapi-sa-orm-filter-0.1.2/Pipfile
+-rw-r--r--   0        0        0    23646 2023-05-07 14:21:44.504856 fastapi-sa-orm-filter-0.1.2/Pipfile.lock
+-rw-r--r--   0        0        0     2262 2023-05-09 20:58:55.302181 fastapi-sa-orm-filter-0.1.2/README.md
+-rw-r--r--   0        0        0      111 2023-05-09 21:00:38.156799 fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/__init__.py
+-rw-r--r--   0        0        0     8558 2023-05-09 20:19:47.476212 fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/main.py
+-rw-r--r--   0        0        0      434 2023-05-09 20:13:04.305063 fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/operators.py
+-rw-r--r--   0        0        0      844 2023-05-07 18:13:40.160724 fastapi-sa-orm-filter-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-04 19:03:00.838038 fastapi-sa-orm-filter-0.1.2/pytest.ini
+-rw-r--r--   0        0        0     3364 2023-05-09 20:41:44.249744 fastapi-sa-orm-filter-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0    15503 2023-05-09 20:55:09.225275 fastapi-sa-orm-filter-0.1.2/tests/test_filter.py
+-rw-r--r--   0        0        0      323 2023-05-05 21:57:39.693231 fastapi-sa-orm-filter-0.1.2/tests/utils.py
+-rw-r--r--   0        0        0     3021 1970-01-01 00:00:00.000000 fastapi-sa-orm-filter-0.1.2/PKG-INFO
```

### Comparing `fastapi-sa-orm-filter-0.1.1/.github/workflows/ci_filter.yml` & `fastapi-sa-orm-filter-0.1.2/.github/workflows/ci_filter.yml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.1/LICENSE` & `fastapi-sa-orm-filter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.1/Pipfile.lock` & `fastapi-sa-orm-filter-0.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.1/README.md` & `fastapi-sa-orm-filter-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ### Quickstart
 
 ```shell
 from fastapi import FastAPI
 from fastapi.params import Query
 from fastapi_sa_orm_filter.main import FilterCore
-from fastapi_sa_orm_filter.filters import FiltersList as fls
+from fastapi_sa_orm_filter.operators import Operators as ops
 
 from db.base import get_session
 from db.models import MyModel
 
 
 app = FastAPI()
 
@@ -29,32 +29,32 @@
     'my_model_field_name': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_],
     'my_model_field_name': [fls.like, fls.startswith, fls.contains, fls.in_],
     'my_model_field_name': [fls.between, fls.not_eq, fls.gte, fls.lte]
 }
 
 @app.get("/")
 async def get_filtered_items(
-    filter: str = Query(default=''),
+    filter_query: str = Query(default=''),
     db: AsyncSession = Depends(get_session)
  ) -> List[MyModel]:
     my_filter = FilterCore(MyModel, my_item_filter)
-    query = my_filter.get_query(filter)
+    query = my_filter.get_query(filter_query)
     res = await db.execute(query)
     return res.scalars().all()
 ```
 
 ### Example of work
 
 ```shell
 
 # Input query string
 '''
-    salary_from__in_=60,70,80&
-    created_at__between=2023-05-01,2023-05-05|
-    category__eq=Medicine"
+salary_from__in_=60,70,80&
+created_at__between=2023-05-01,2023-05-05|
+category__eq=Medicine"
 '''
 
    
 # Returned SQLAlchemy orm query exact as:
            
 select(model)
     .where(
@@ -73,14 +73,15 @@
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
 
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
 * INTEGER
+* FLOAT
 * TEXT
 * VARCHAR
 * Enum(VARCHAR())
 * BOOLEAN
 
 ### Available filter operators:
 * __eq__
```

### Comparing `fastapi-sa-orm-filter-0.1.1/fastapi_sa_orm_filter/main.py` & `fastapi-sa-orm-filter-0.1.2/fastapi_sa_orm_filter/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import json
-from datetime import datetime
 from typing import Any, Dict, List, Tuple, Optional, Union, Type
 
 import pydantic
-from fastapi import HTTPException
+from fastapi import HTTPException, Query
 from pydantic import create_model
 from pydantic.main import ModelMetaclass
 from pydantic_sqlalchemy import sqlalchemy_to_pydantic
 from sqlalchemy import select
 from sqlalchemy.orm import InstrumentedAttribute, DeclarativeMeta
 from sqlalchemy.sql.elements import BinaryExpression
 from sqlalchemy.sql.expression import and_, or_
 from starlette import status
-from sqlalchemy.types import Date, DateTime
 from sqlalchemy.sql import Select
 
-from fastapi_sa_orm_filter.filters import FiltersList as fls
+from fastapi_sa_orm_filter.operators import Operators as ops
 
 
 class FilterCore:
     """
     Class serves of SQLAlchemy orm query creation.
     Convert parsed query data to python data types and form SQLAlchemy query.
     """
 
     def __init__(
-        self, model: Type[DeclarativeMeta], allowed_filters: Dict[str, List[fls]]
+        self, model: Type[DeclarativeMeta], allowed_filters: Dict[str, List[ops]]
     ) -> None:
         """
         Produce a class:`FilterCore` object against a function
 
         :param model: declared SQLAlchemy db model
         :param allowed_filters: dict with allowed model fields and operators
             for filter, like:
@@ -43,17 +41,18 @@
         self._model_serializer = self._create_pydantic_serializer()
 
     def get_query(self, custom_filter: str) -> Select:
         """
         Construct the SQLAlchemy orm query from request query string
 
         :param custom_filter: request query string with fields and filter conditions
-            'salary_from__in_=60,70,80&
-             created_at__between=2023-05-01,2023-05-05|
-             category__eq=Medicine'
+            salary_from__in_=60,70,80&
+            created_at__between=2023-05-01,2023-05-05|
+            category__eq=Medicine
+
         :return:
             select(model)
                 .where(
                     or_(
                         and_(
                             model.salary_from.in_(60,70,80),
                             model.created_at.between(2023-05-01, 2023-05-05)
@@ -107,42 +106,32 @@
     @staticmethod
     def _get_orm_for_field(
         column: InstrumentedAttribute, operator: str, value: Any
     ) -> BinaryExpression:
         """
         Create SQLAlchemy orm expression for the field
         """
-        if operator in [fls.between]:
-            param = getattr(column, fls[operator].value)(*value)
+        if operator in [ops.between]:
+            param = getattr(column, ops[operator].value)(*value)
         else:
-            param = getattr(column, fls[operator].value)(value)
-
+            param = getattr(column, ops[operator].value)(value)
         return param
 
     def _format_expression(
         self, column: InstrumentedAttribute, operator: str, value: str
     ) -> dict[str, Any]:
         """
         Serialize expression value from string to python type value,
         according to db model types
 
         :return: {'field_name': [value, value]}
         """
         value = value.split(",")
         try:
-            if isinstance(column.type, DateTime):
-                value = [
-                    datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")
-                    for date_str in value
-                ]
-            if isinstance(column.type, Date):
-                value = [
-                    datetime.strptime(date_str, "%Y-%m-%d").date() for date_str in value
-                ]
-            if operator not in [fls.between, fls.in_]:
+            if operator not in [ops.between, ops.in_]:
                 value = value[0]
                 serialized_dict = self._model_serializer["optional_model"](
                     **{column.name: value}
                 ).dict(exclude_none=True)
                 return serialized_dict
             serialized_dict = self._model_serializer["list_model"](
                 **{column.name: value}
@@ -237,7 +226,9 @@
         for allow_filter in self.allowed_filters[field_name]:
             if operator == allow_filter.name:
                 return
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=f"Forbidden filter '{operator}' for '{field_name}'",
         )
+
+    Query
```

### Comparing `fastapi-sa-orm-filter-0.1.1/pyproject.toml` & `fastapi-sa-orm-filter-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-sa-orm-filter-0.1.1/tests/conftest.py` & `fastapi-sa-orm-filter-0.1.2/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import asyncio
 from datetime import date, datetime
 
 import pytest
 import pytest_asyncio
-from sqlalchemy import Column, Integer, Date, Text, String, Boolean, DateTime, Enum
+from sqlalchemy import Column, Integer, Date, Text, String, Boolean, DateTime, Enum, Float
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.orm import sessionmaker, declarative_base
 
 from fastapi_sa_orm_filter.main import FilterCore
-from fastapi_sa_orm_filter.filters import FiltersList as fls
+from fastapi_sa_orm_filter.operators import Operators as ops
 from tests.utils import JobCategory
 
 Base = declarative_base()
 
 
 class Vacancy(Base):
     __tablename__ = "vacancies"
     id = Column(Integer, primary_key=True)
     title = Column(String)
     description = Column(Text)
     is_active = Column(Boolean, default=True)
     created_at = Column(Date)
     updated_at = Column(DateTime)
     salary_from = Column(Integer)
-    salary_up_to = Column(Integer)
+    salary_up_to = Column(Float)
     category = Column(Enum(JobCategory), nullable=False)
 
 
 @pytest.fixture(scope="session")
 def sqlite_file_path(tmp_path_factory):
     file_path = tmp_path_factory.mktemp("data")
     yield file_path
@@ -76,33 +76,34 @@
     vacancy_instances = []
     enum_category = [member.name for member in JobCategory]
     for i in range(1, 11):
         vacancy = Vacancy(
             title=f"title{i}",
             description=f"description{i}",
             salary_from=50 + i * 10,
-            salary_up_to=100 + i * 10,
+            salary_up_to=100.725 + i * 10,
             created_at=date(2023, 5, i),
             updated_at=datetime(2023, i, 5, 15, 15, 15),
             category=JobCategory[enum_category[i - 1]]
         )
         vacancy_instances.append(vacancy)
     session.add_all(vacancy_instances)
     await session.commit()
 
 
 @pytest.fixture
 def get_custom_restriction():
     return {
-        'title': [fls.startswith, fls.eq, fls.endswith],
-        'category': [fls.startswith, fls.eq, fls.in_],
-        'salary_from': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_, fls.gte],
-        'description': [fls.like, fls.not_like, fls.contains, fls.eq, fls.in_],
-        'created_at': [fls.between, fls.in_, fls.eq, fls.gt, fls.lt, fls.not_eq],
-        'updated_at': [fls.between, fls.in_, fls.eq, fls.gt, fls.lt],
-        'is_active': [fls.eq]
+        'title': [ops.startswith, ops.eq, ops.endswith],
+        'category': [ops.startswith, ops.eq, ops.in_],
+        'salary_from': [ops.between, ops.eq, ops.gt, ops.lt, ops.in_, ops.gte],
+        'salary_up_to': [ops.eq, ops.gt],
+        'description': [ops.like, ops.not_like, ops.contains, ops.eq, ops.in_],
+        'created_at': [ops.between, ops.in_, ops.eq, ops.gt, ops.lt, ops.not_eq],
+        'updated_at': [ops.between, ops.in_, ops.eq, ops.gt, ops.lt],
+        'is_active': [ops.eq]
     }
 
 
 @pytest.fixture
 def get_filter(get_custom_restriction):
     return FilterCore(Vacancy, get_custom_restriction)
```

### Comparing `fastapi-sa-orm-filter-0.1.1/tests/test_filter.py` & `fastapi-sa-orm-filter-0.1.2/tests/test_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,53 @@
 class ListPydanticVacancy(BaseModel):
     vacancies: List[PydanticVacancy] = []
 
 
 async def test_eq_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__eq=60")
     res = await session.execute(query)
-    data = PydanticVacancy.from_orm(res.scalar()).dict()
-    assert isinstance(data["created_at"], date)
-    assert isinstance(data["updated_at"], datetime)
-    check_data = data.copy()
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 1
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
     del check_data["created_at"]
     del check_data["updated_at"]
     assert check_data == {
         'id': 1,
         'title': 'title1',
         'description': 'description1',
         'is_active': True,
         'salary_from': 60,
-        'salary_up_to': 110,
+        'salary_up_to': 110.725,
         'category': JobCategory.finance
     }
 
 
+async def test_eq_with_float(session, get_filter, create_vacancies):
+    query = get_filter.get_query("salary_up_to__eq=120.725")
+    res = await session.execute(query)
+    data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
+    assert len(data['vacancies']) == 1
+    assert isinstance(data['vacancies'][0]["created_at"], date)
+    assert isinstance(data['vacancies'][0]["updated_at"], datetime)
+    check_data = data['vacancies'][0].copy()
+    del check_data["created_at"]
+    del check_data["updated_at"]
+    assert check_data == {
+        'id': 2,
+        'title': 'title2',
+        'description': 'description2',
+        'is_active': True,
+        'salary_from': 70,
+        'salary_up_to': 120.725,
+        'category': JobCategory.marketing
+    }
+
+
 async def test_in_with_str(session, get_filter, create_vacancies):
     query = get_filter.get_query("description__in_=description1,description2")
     res = await session.execute(query)
     data = ListPydanticVacancy(vacancies=res.scalars().all()).dict()
     assert len(data['vacancies']) == 2
     assert isinstance(data['vacancies'][0]["created_at"], date)
     assert isinstance(data['vacancies'][0]["updated_at"], datetime)
@@ -49,15 +71,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 1,
         'title': 'title1',
         'description': 'description1',
         'is_active': True,
         'salary_from': 60,
-        'salary_up_to': 110,
+        'salary_up_to': 110.725,
         'category': JobCategory.finance
     }
 
 
 async def test_contains_with_str(session, get_filter, create_vacancies):
     query = get_filter.get_query("description__contains=tion1")
     res = await session.execute(query)
@@ -70,15 +92,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 10,
         'title': 'title10',
         'description': 'description10',
         'is_active': True,
         'salary_from': 150,
-        'salary_up_to': 200,
+        'salary_up_to': 200.725,
         'category': JobCategory.miscellaneous
     }
 
 
 async def test_endswith_with_str(session, get_filter, create_vacancies):
     query = get_filter.get_query("title__endswith=le1")
     res = await session.execute(query)
@@ -91,15 +113,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 1,
         'title': 'title1',
         'description': 'description1',
         'is_active': True,
         'salary_from': 60,
-        'salary_up_to': 110,
+        'salary_up_to': 110.725,
         'category': JobCategory.finance
     }
 
 
 async def test_in_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__in_=60,70,80")
     res = await session.execute(query)
@@ -112,15 +134,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 1,
         'title': 'title1',
         'description': 'description1',
         'is_active': True,
         'salary_from': 60,
-        'salary_up_to': 110,
+        'salary_up_to': 110.725,
         'category': JobCategory.finance
     }
 
 
 async def test_gte_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__gte=120")
     res = await session.execute(query)
@@ -133,15 +155,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 7,
         'title': 'title7',
         'description': 'description7',
         'is_active': True,
         'salary_from': 120,
-        'salary_up_to': 170,
+        'salary_up_to': 170.725,
         'category': JobCategory.construction
     }
 
 
 async def test_not_eq_with_date(session, get_filter, create_vacancies):
     query = get_filter.get_query("created_at__not_eq=2023-05-01")
     res = await session.execute(query)
@@ -154,15 +176,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 2,
         'title': 'title2',
         'description': 'description2',
         'is_active': True,
         'salary_from': 70,
-        'salary_up_to': 120,
+        'salary_up_to': 120.725,
         'category': JobCategory.marketing
     }
 
 
 async def test_eq_with_bool(session, get_filter, create_vacancies):
     query = get_filter.get_query("is_active__eq=true")
     res = await session.execute(query)
@@ -175,15 +197,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 1,
         'title': 'title1',
         'description': 'description1',
         'is_active': True,
         'salary_from': 60,
-        'salary_up_to': 110,
+        'salary_up_to': 110.725,
         'category': JobCategory.finance
     }
 
 
 async def test_between_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__between=50,90")
     res = await session.execute(query)
@@ -196,15 +218,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 1,
         'title': 'title1',
         'description': 'description1',
         'is_active': True,
         'salary_from': 60,
-        'salary_up_to': 110,
+        'salary_up_to': 110.725,
         'category': JobCategory.finance
     }
 
 
 async def test_between_with_datetime(session, get_filter, create_vacancies):
     query = get_filter.get_query("updated_at__between=2023-01-01 0:0:0,2023-05-01 0:0:0")
     res = await session.execute(query)
@@ -217,15 +239,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 4,
         'title': 'title4',
         'description': 'description4',
         'is_active': True,
         'salary_from': 90,
-        'salary_up_to': 140,
+        'salary_up_to': 140.725,
         'category': JobCategory.it
     }
 
 
 async def test_between_with_date(session, get_filter, create_vacancies):
     query = get_filter.get_query("created_at__between=2023-05-01,2023-05-05")
     res = await session.execute(query)
@@ -238,15 +260,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 5,
         'title': 'title5',
         'description': 'description5',
         'is_active': True,
         'salary_from': 100,
-        'salary_up_to': 150,
+        'salary_up_to': 150.725,
         'category': JobCategory.metallurgy
     }
 
 
 async def test_gt_with_int(session, get_filter, create_vacancies):
     query = get_filter.get_query("salary_from__gt=100")
     res = await session.execute(query)
@@ -259,15 +281,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 6,
         'title': 'title6',
         'description': 'description6',
         'is_active': True,
         'salary_from': 110,
-        'salary_up_to': 160,
+        'salary_up_to': 160.725,
         'category': JobCategory.medicine
     }
 
 
 async def test_enum_with_str(session, get_filter, create_vacancies):
     query = get_filter.get_query("category__eq=Medicine")
     res = await session.execute(query)
@@ -280,15 +302,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 6,
         'title': 'title6',
         'description': 'description6',
         'is_active': True,
         'salary_from': 110,
-        'salary_up_to': 160,
+        'salary_up_to': 160.725,
         'category': JobCategory.medicine
     }
 
 
 async def test_complex_query(session, get_filter, create_vacancies):
     query = get_filter.get_query(
         "created_at__between=2023-05-01,2023-05-05&"
@@ -305,15 +327,15 @@
     del check_data['updated_at']
     assert check_data == {
         'id': 5,
         'title': 'title5',
         'description': 'description5',
         'is_active': True,
         'salary_from': 100,
-        'salary_up_to': 150,
+        'salary_up_to': 150.725,
         'category': JobCategory.metallurgy
     }
 
 
 @pytest.mark.parametrize(
     "bad_filter, expected_status_code, expected_detail",
     (
@@ -389,14 +411,23 @@
             HTTP_400_BAD_REQUEST,
             [
                 {'loc': ['is_active'],
                  'msg': 'value could not be parsed to a boolean',
                  'type': 'type_error.bool'}
             ]
         ),
+        (
+            "salary_up_to__eq=100/12",
+            HTTP_400_BAD_REQUEST,
+            [
+                {'loc': ['salary_up_to'],
+                 'msg': 'value is not a valid float',
+                 'type': 'type_error.float'}
+            ]
+        ),
     )
 )
 def test_fail_filter(get_filter, bad_filter, expected_status_code, expected_detail):
     with pytest.raises(Exception) as e:
         get_filter.get_query(bad_filter)
     assert e.type == HTTPException
     assert e.value.status_code == expected_status_code
```

### Comparing `fastapi-sa-orm-filter-0.1.1/PKG-INFO` & `fastapi-sa-orm-filter-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sa-orm-filter
-Version: 0.1.1
+Version: 0.1.2
 Summary: FastAPI-SQLAlchemy filter, transform request query string to SQLAlchemy orm query
 Author-email: Oleksandr Zhydyk <zhydykalex@ukr.net>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: fastapi
 Requires-Dist: sqlalchemy
@@ -31,15 +31,15 @@
 
 ### Quickstart
 
 ```shell
 from fastapi import FastAPI
 from fastapi.params import Query
 from fastapi_sa_orm_filter.main import FilterCore
-from fastapi_sa_orm_filter.filters import FiltersList as fls
+from fastapi_sa_orm_filter.operators import Operators as ops
 
 from db.base import get_session
 from db.models import MyModel
 
 
 app = FastAPI()
 
@@ -49,32 +49,32 @@
     'my_model_field_name': [fls.between, fls.eq, fls.gt, fls.lt, fls.in_],
     'my_model_field_name': [fls.like, fls.startswith, fls.contains, fls.in_],
     'my_model_field_name': [fls.between, fls.not_eq, fls.gte, fls.lte]
 }
 
 @app.get("/")
 async def get_filtered_items(
-    filter: str = Query(default=''),
+    filter_query: str = Query(default=''),
     db: AsyncSession = Depends(get_session)
  ) -> List[MyModel]:
     my_filter = FilterCore(MyModel, my_item_filter)
-    query = my_filter.get_query(filter)
+    query = my_filter.get_query(filter_query)
     res = await db.execute(query)
     return res.scalars().all()
 ```
 
 ### Example of work
 
 ```shell
 
 # Input query string
 '''
-    salary_from__in_=60,70,80&
-    created_at__between=2023-05-01,2023-05-05|
-    category__eq=Medicine"
+salary_from__in_=60,70,80&
+created_at__between=2023-05-01,2023-05-05|
+category__eq=Medicine"
 '''
 
    
 # Returned SQLAlchemy orm query exact as:
            
 select(model)
     .where(
@@ -93,14 +93,15 @@
 * field_name__in_=value1,value2
 * field_name__eq=value&field_name__in_=value1,value2
 
 ### Supported SQLAlchemy datatypes:
 * DATETIME
 * DATE
 * INTEGER
+* FLOAT
 * TEXT
 * VARCHAR
 * Enum(VARCHAR())
 * BOOLEAN
 
 ### Available filter operators:
 * __eq__
```

