# Comparing `tmp/duckdb_engine-0.7.0rc1.tar.gz` & `tmp/duckdb_engine-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.7.0rc1.tar", max compression
+gzip compressed data, was "duckdb_engine-0.7.1.tar", max compression
```

## Comparing `duckdb_engine-0.7.0rc1.tar` & `duckdb_engine-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/LICENSE.txt
--rw-r--r--   0        0        0     5953 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/README.md
--rw-r--r--   0        0        0    11516 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/__init__.py
--rw-r--r--   0        0        0      985 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     1707 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1042 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    10441 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     1985 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      948 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0      455 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1374 2023-03-07 06:59:08.995926 duckdb_engine-0.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6870 1970-01-01 00:00:00.000000 duckdb_engine-0.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-09 16:12:04.584668 duckdb_engine-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     5953 2023-05-09 16:12:04.584668 duckdb_engine-0.7.1/README.md
+-rw-r--r--   0        0        0        4 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    11514 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     1707 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    10426 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     2351 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      948 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0      455 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1370 2023-05-09 16:12:04.588668 duckdb_engine-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.7.1/PKG-INFO
```

### Comparing `duckdb_engine-0.7.0rc1/LICENSE.txt` & `duckdb_engine-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/README.md` & `duckdb_engine-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/__init__.py` & `duckdb_engine-0.7.1/duckdb_engine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 )
 
 import duckdb
 from sqlalchemy import pool, text
 from sqlalchemy import types as sqltypes
 from sqlalchemy import util
 from sqlalchemy.dialects.postgresql import UUID
-from sqlalchemy.dialects.postgresql.base import PGInspector
+from sqlalchemy.dialects.postgresql.base import PGDialect, PGInspector
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.url import URL
 
 from .config import apply_config, get_core_config
 from .datatypes import register_extension_types
 
-__version__ = "0.7.0-rc1"
+__version__ = "0.7.1"
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
 
 
 register_extension_types()
@@ -170,15 +170,15 @@
     supports_statement_cache = False
     supports_comments = False
     supports_sane_rowcount = False
     supports_server_side_cursors = False
     inspector = DuckDBInspector
     # colspecs TODO: remap types to duckdb types
     colspecs = util.update_copy(
-        PGDialect_psycopg2.colspecs,
+        PGDialect.colspecs,
         {
             # the psycopg2 driver registers a _PGNumeric with custom logic for
             # postgres type_codes (such as 701 for float) that duckdb doesn't have
             sqltypes.Numeric: sqltypes.Numeric,
             sqltypes.Interval: sqltypes.Interval,
             sqltypes.JSON: sqltypes.JSON,
             UUID: UUID,
```

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/config.py` & `duckdb_engine-0.7.1/duckdb_engine/config.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/datatypes.py` & `duckdb_engine-0.7.1/duckdb_engine/datatypes.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.7.1/duckdb_engine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.7.1/duckdb_engine/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from sqlalchemy.engine import Engine
 from sqlalchemy.engine.reflection import Inspector
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session, relationship, sessionmaker
 
 from .. import DBAPI, Dialect
-from .util import sqlalchemy_1_only
 
 try:
     # sqlalchemy 2
     from sqlalchemy.engine import ObjectKind  # type: ignore[attr-defined]
     from sqlalchemy.orm import Mapped
 except ImportError:
     # sqlalchemy 1
@@ -246,16 +245,16 @@
             schema=None,
             filter_names=set(),
             scope=None,
             kind=(ObjectKind.TABLE,),
         )
 
 
-@sqlalchemy_1_only
 def test_commit(session: Session, engine: Engine) -> None:
+    importorskip("sqlalchemy", "1.4.0")
     session.execute(text("commit;"))
 
     InteractiveShell = importorskip("IPython.core.interactiveshell").InteractiveShell
 
     shell = InteractiveShell()
     assert not shell.run_line_magic("load_ext", "sql")
     assert not shell.run_line_magic("sql", "duckdb:///:memory:")
```

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.7.1/duckdb_engine/tests/test_datatypes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Type
 from uuid import uuid4
 
 from pytest import importorskip, mark
-from sqlalchemy import Column, Integer, inspect
+from sqlalchemy import Column, Integer, MetaData, Table, inspect, text
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session
 from sqlalchemy.types import JSON
 
 from ..datatypes import types
@@ -76,7 +76,20 @@
 
     session.add(Entry(id=ident))  # type: ignore[call-arg]
     session.commit()
 
     result = session.query(Entry).one()
 
     assert result.id == ident
+
+
+def test_double_in_sqla_v2(engine: Engine) -> None:
+    with engine.begin() as con:
+        con.execute(text("CREATE TABLE t (x DOUBLE)"))
+        con.execute(text("INSERT INTO t VALUES (1.0), (2.0), (3.0)"))
+
+    md = MetaData()
+
+    t = Table("t", md, autoload_with=engine)
+
+    with engine.begin() as con:
+        con.execute(t.select())
```

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.7.1/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.7.1/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.0rc1/pyproject.toml` & `duckdb_engine-0.7.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.7.0-rc1"
+version = "0.7.1"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Mause/duckdb_engine/issues"
 "Changelog" = "https://github.com/Mause/duckdb_engine/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 duckdb = ">=0.4.0"
-sqlalchemy = ">=1.3.19"
+sqlalchemy = ">=1.3.22"
 numpy = "*"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pre-commit = "^2.21.0"
 pdbpp = "^0.10.3"
-mypy = "^1.0"
-hypothesis = "^6.68.2"
+mypy = "^1.1"
+hypothesis = "^6.75.2"
 pandas = "^1"
-jupysql = "^0.6.2"
+jupysql = "^0.7.4"
 sqlalchemy = {version="^1.3.19", extras=['mypy']}
 pytest-cov = {extras = ["coverage"], version = "^4.0.0"}
 snapshottest = "^0.6.0"
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
 duckdb = "duckdb_engine:Dialect"
```

### Comparing `duckdb_engine-0.7.0rc1/PKG-INFO` & `duckdb_engine-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb-engine
-Version: 0.7.0rc1
+Version: 0.7.1
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: duckdb (>=0.4.0)
 Requires-Dist: numpy
-Requires-Dist: sqlalchemy (>=1.3.19)
+Requires-Dist: sqlalchemy (>=1.3.22)
 Project-URL: Bug Tracker, https://github.com/Mause/duckdb_engine/issues
 Project-URL: Changelog, https://github.com/Mause/duckdb_engine/releases
 Project-URL: Repository, https://github.com/Mause/duckdb_engine
 Description-Content-Type: text/markdown
 
 # duckdb_engine
```

