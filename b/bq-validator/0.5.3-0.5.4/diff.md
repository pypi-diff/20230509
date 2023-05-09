# Comparing `tmp/bq-validator-0.5.3.tar.gz` & `tmp/bq-validator-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bq-validator-0.5.3.tar", last modified: Tue Feb 21 05:13:52 2023, max compression
+gzip compressed data, was "bq-validator-0.5.4.tar", last modified: Tue May  9 09:13:04 2023, max compression
```

## Comparing `bq-validator-0.5.3.tar` & `bq-validator-0.5.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      804 2023-02-21 05:13:31.538970 bq-validator-0.5.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      961 2023-02-21 05:13:31.538970 bq-validator-0.5.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      966 2023-02-21 05:13:31.538970 bq-validator-0.5.3/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0      967 2023-02-21 05:13:31.538970 bq-validator-0.5.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2023-02-21 05:13:31.542971 bq-validator-0.5.3/.gitignore
--rw-r--r--   0        0        0      150 2023-02-21 05:13:31.542971 bq-validator-0.5.3/.pypirc
--rw-r--r--   0        0        0       32 2023-02-21 05:13:31.542971 bq-validator-0.5.3/.style.yapf
--rw-r--r--   0        0        0    11357 2023-02-21 05:13:31.542971 bq-validator-0.5.3/LICENSE
--rw-r--r--   0        0        0      100 2023-02-21 05:13:31.542971 bq-validator-0.5.3/MANIFEST.in
--rw-r--r--   0        0        0      749 2023-02-21 05:13:31.542971 bq-validator-0.5.3/Makefile
--rw-r--r--   0        0        0     1788 2023-02-21 05:13:31.542971 bq-validator-0.5.3/README.md
--rw-r--r--   0        0        0      890 2023-02-21 05:13:31.542971 bq-validator-0.5.3/bq_validator/__init__.py
--rw-r--r--   0        0        0     4443 2023-02-21 05:13:31.542971 bq-validator-0.5.3/bq_validator/bigquery.py
--rw-r--r--   0        0        0     2876 2023-02-21 05:13:31.542971 bq-validator-0.5.3/bq_validator/cli.py
--rw-r--r--   0        0        0     1445 2023-02-21 05:13:31.542971 bq-validator-0.5.3/bq_validator/utils.py
--rwxr-xr-x   0        0        0     1121 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/clean.sh
--rwxr-xr-x   0        0        0     1013 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/format_python.sh
--rw-r--r--   0        0        0      970 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1366 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/publish.sh
--rwxr-xr-x   0        0        0     1023 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/setup.sh
--rw-r--r--   0        0        0      921 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/test_entry_point.sh
--rwxr-xr-x   0        0        0      958 2023-02-21 05:13:31.542971 bq-validator-0.5.3/dev/test_python.sh
--rw-r--r--   0        0        0    14273 2023-02-21 05:13:31.542971 bq-validator-0.5.3/pylintrc
--rw-r--r--   0        0        0     1982 2023-02-21 05:13:31.542971 bq-validator-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      830 2023-02-21 05:13:31.542971 bq-validator-0.5.3/setup.py
--rw-r--r--   0        0        0      792 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/orders.sql
--rw-r--r--   0        0        0      218 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/staging/stg_customers.sql
--rw-r--r--   0        0        0      241 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/staging/stg_orders.sql
--rw-r--r--   0        0        0      330 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/staging/stg_payments.sql
--rw-r--r--   0        0        0      166 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/test_insert_overwrite.sql
--rw-r--r--   0        0        0      166 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/test_merge.sql
--rw-r--r--   0        0        0     1442 2023-02-21 05:13:31.542971 bq-validator-0.5.3/tests/test_utils.py
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 bq-validator-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      961 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      966 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0      967 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.gitignore
+-rw-r--r--   0        0        0      150 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.pypirc
+-rw-r--r--   0        0        0       32 2023-05-09 09:12:38.440499 bq-validator-0.5.4/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-05-09 09:12:38.440499 bq-validator-0.5.4/LICENSE
+-rw-r--r--   0        0        0      100 2023-05-09 09:12:38.440499 bq-validator-0.5.4/MANIFEST.in
+-rw-r--r--   0        0        0      749 2023-05-09 09:12:38.440499 bq-validator-0.5.4/Makefile
+-rw-r--r--   0        0        0     1788 2023-05-09 09:12:38.440499 bq-validator-0.5.4/README.md
+-rw-r--r--   0        0        0      890 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/__init__.py
+-rw-r--r--   0        0        0     4443 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/bigquery.py
+-rw-r--r--   0        0        0     2876 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/cli.py
+-rw-r--r--   0        0        0     1445 2023-05-09 09:12:38.440499 bq-validator-0.5.4/bq_validator/utils.py
+-rwxr-xr-x   0        0        0     1121 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/clean.sh
+-rwxr-xr-x   0        0        0     1013 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/format_python.sh
+-rw-r--r--   0        0        0      970 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1366 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/publish.sh
+-rwxr-xr-x   0        0        0     1023 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/setup.sh
+-rw-r--r--   0        0        0      921 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/test_entry_point.sh
+-rwxr-xr-x   0        0        0      958 2023-05-09 09:12:38.440499 bq-validator-0.5.4/dev/test_python.sh
+-rw-r--r--   0        0        0    14273 2023-05-09 09:12:38.440499 bq-validator-0.5.4/pylintrc
+-rw-r--r--   0        0        0     1989 2023-05-09 09:12:38.440499 bq-validator-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-05-09 09:12:38.440499 bq-validator-0.5.4/setup.py
+-rw-r--r--   0        0        0      792 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/__init__.py
+-rw-r--r--   0        0        0     1160 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/orders.sql
+-rw-r--r--   0        0        0      218 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/staging/stg_customers.sql
+-rw-r--r--   0        0        0      241 2023-05-09 09:12:38.440499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/staging/stg_orders.sql
+-rw-r--r--   0        0        0      330 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/staging/stg_payments.sql
+-rw-r--r--   0        0        0      166 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/test_insert_overwrite.sql
+-rw-r--r--   0        0        0      166 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/test_merge.sql
+-rw-r--r--   0        0        0     1442 2023-05-09 09:12:38.444499 bq-validator-0.5.4/tests/test_utils.py
+-rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 bq-validator-0.5.4/PKG-INFO
```

### Comparing `bq-validator-0.5.3/.github/CODEOWNERS` & `bq-validator-0.5.4/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/.github/workflows/publish.yml` & `bq-validator-0.5.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/.github/workflows/test-publish.yml` & `bq-validator-0.5.4/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/.github/workflows/test.yml` & `bq-validator-0.5.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/.gitignore` & `bq-validator-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/LICENSE` & `bq-validator-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/Makefile` & `bq-validator-0.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/README.md` & `bq-validator-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/bq_validator/__init__.py` & `bq-validator-0.5.4/bq_validator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
 The `bq-validator` command enables us to validate BigQuery queries.
 """
-__version__ = "0.5.3"
+__version__ = "0.5.4"
```

### Comparing `bq-validator-0.5.3/bq_validator/bigquery.py` & `bq-validator-0.5.4/bq_validator/bigquery.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/bq_validator/cli.py` & `bq-validator-0.5.4/bq_validator/cli.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/bq_validator/utils.py` & `bq-validator-0.5.4/bq_validator/utils.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/clean.sh` & `bq-validator-0.5.4/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/format_python.sh` & `bq-validator-0.5.4/dev/format_python.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/lint_python.sh` & `bq-validator-0.5.4/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/publish.sh` & `bq-validator-0.5.4/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/setup.sh` & `bq-validator-0.5.4/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/test_entry_point.sh` & `bq-validator-0.5.4/dev/test_entry_point.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/dev/test_python.sh` & `bq-validator-0.5.4/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/pylintrc` & `bq-validator-0.5.4/pylintrc`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/pyproject.toml` & `bq-validator-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 [project]
 name = "bq-validator"
 authors = [
     {name = "yu-iskw"},
 ]
 dynamic = ["version", "description"]
 dependencies = [
-    "click ==8.0.3",
-    "click-completion ==0.5.2",
+    "click >=8.0.0,<9.0.0",
+    "click-completion >=0.5.2",
     "google-cloud-bigquery >=1.25.0,<4.0.0",
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6.1"
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `bq-validator-0.5.3/setup.py` & `bq-validator-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/tests/__init__.py` & `bq-validator-0.5.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/tests/resources/target/compiled/jaffle_shop/models/orders.sql` & `bq-validator-0.5.4/tests/resources/target/compiled/jaffle_shop/models/orders.sql`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/tests/test_utils.py` & `bq-validator-0.5.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bq-validator-0.5.3/PKG-INFO` & `bq-validator-0.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-validator
-Version: 0.5.3
+Version: 0.5.4
 Summary: The `bq-validator` command enables us to validate BigQuery queries.
 Author: yu-iskw
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -17,16 +17,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: click ==8.0.3
-Requires-Dist: click-completion ==0.5.2
+Requires-Dist: click >=8.0.0,<9.0.0
+Requires-Dist: click-completion >=0.5.2
 Requires-Dist: google-cloud-bigquery >=1.25.0,<4.0.0
 Requires-Dist: flit ==3.7.1 ; extra == "dev"
 Requires-Dist: build ==0.7.0 ; extra == "dev"
 Requires-Dist: yapf >=0.29.0 ; extra == "dev"
 Requires-Dist: pyyaml >=5.3 ; extra == "dev"
 Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev"
 Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra == "test"
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1 Name: bq-validator Version: 0.5.3 Summary: The `bq-
+Metadata-Version: 2.1 Name: bq-validator Version: 0.5.4 Summary: The `bq-
 validator` command enables us to validate BigQuery queries. Author: yu-iskw
 Requires-Python: >=3.6.1 Description-Content-Type: text/markdown Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
-click ==8.0.3 Requires-Dist: click-completion ==0.5.2 Requires-Dist: google-
-cloud-bigquery >=1.25.0,<4.0.0 Requires-Dist: flit ==3.7.1 ; extra == "dev"
-Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist: yapf >=0.29.0 ;
-extra == "dev" Requires-Dist: pyyaml >=5.3 ; extra == "dev" Requires-Dist:
-pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pytest >=6.2.4,<7.0.0 ; extra ==
-"test" Requires-Dist: pylint >=2.12.0 ; extra == "test" Requires-Dist: mypy
-==0.910 ; extra == "test" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra ==
-"test" Requires-Dist: black ==21.9b0 ; extra == "test" Requires-Dist: isort
->=5.0.6,<6.0.0 ; extra == "test" Requires-Dist: yapf >=0.29.0 ; extra == "test"
-Provides-Extra: dev Provides-Extra: test [![Test python](https://github.com/yu-
-iskw/bq-validator/actions/workflows/test.yml/badge.svg)](https://github.com/yu-
-iskw/bq-validator/actions/workflows/test.yml) [Package_version] [Supported
-Python_versions] # bq-validator This is a yet another python-based BigQuery
-query validator. The `bq query --dry_run` command enables us to validate
-queries. However, the `bq` command doesn't support service account
-impersonation, even though it supports workload identity federation credentials
-at Google Cloud SDK 390.0.0. The `bq-validator` command would be useful, when
-we take advantage of service account impersonation to validate BigQuery
-queries. ## Install The package is available on [pypi](https://pypi.org/
-project/bq-validator/) ```bash pip install -U bq-validator ``` ## How to use
-```bash $ bq-validator --help Usage: bq-validator [OPTIONS] PATH Validate
-BigQuery queries PATH is either of a SQL file path or a directory. When it is a
-directory, the command recursively validates all SQL files in the directory.
-Options: --quota_project TEXT BigQuery client project ID --client_project TEXT
-BigQuery client project ID --client_location TEXT BigQuery client location --
-impersonate_service_account TEXT Impersonate service account email --version
-Show the version and exit. --help Show this message and exit. ```
+click >=8.0.0,<9.0.0 Requires-Dist: click-completion >=0.5.2 Requires-Dist:
+google-cloud-bigquery >=1.25.0,<4.0.0 Requires-Dist: flit ==3.7.1 ; extra ==
+"dev" Requires-Dist: build ==0.7.0 ; extra == "dev" Requires-Dist: yapf
+>=0.29.0 ; extra == "dev" Requires-Dist: pyyaml >=5.3 ; extra == "dev"
+Requires-Dist: pdoc3 >=0.9.2 ; extra == "dev" Requires-Dist: pytest
+>=6.2.4,<7.0.0 ; extra == "test" Requires-Dist: pylint >=2.12.0 ; extra ==
+"test" Requires-Dist: mypy ==0.910 ; extra == "test" Requires-Dist: flake8
+>=3.8.3,<4.0.0 ; extra == "test" Requires-Dist: black ==21.9b0 ; extra ==
+"test" Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test" Requires-Dist:
+yapf >=0.29.0 ; extra == "test" Provides-Extra: dev Provides-Extra: test [!
+[Test python](https://github.com/yu-iskw/bq-validator/actions/workflows/
+test.yml/badge.svg)](https://github.com/yu-iskw/bq-validator/actions/workflows/
+test.yml) [Package_version] [Supported_Python_versions] # bq-validator This is
+a yet another python-based BigQuery query validator. The `bq query --dry_run`
+command enables us to validate queries. However, the `bq` command doesn't
+support service account impersonation, even though it supports workload
+identity federation credentials at Google Cloud SDK 390.0.0. The `bq-validator`
+command would be useful, when we take advantage of service account
+impersonation to validate BigQuery queries. ## Install The package is available
+on [pypi](https://pypi.org/project/bq-validator/) ```bash pip install -U bq-
+validator ``` ## How to use ```bash $ bq-validator --help Usage: bq-validator
+[OPTIONS] PATH Validate BigQuery queries PATH is either of a SQL file path or a
+directory. When it is a directory, the command recursively validates all SQL
+files in the directory. Options: --quota_project TEXT BigQuery client project
+ID --client_project TEXT BigQuery client project ID --client_location TEXT
+BigQuery client location --impersonate_service_account TEXT Impersonate service
+account email --version Show the version and exit. --help Show this message and
+exit. ```
```

