# Comparing `tmp/gpt-review-0.8.0rc549.post1.tar.gz` & `tmp/gpt-review-0.8.0rc552.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.0rc549.post1.tar", last modified: Tue May  9 15:56:52 2023, max compression
+gzip compressed data, was "gpt-review-0.8.0rc552.post1.tar", last modified: Tue May  9 16:49:38 2023, max compression
```

## Comparing `gpt-review-0.8.0rc549.post1.tar` & `gpt-review-0.8.0rc552.post1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
--rw-r--r--   0        0        0      336 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     2153 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4246 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8346 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-09 15:56:52.414263 gpt-review-0.8.0rc549.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-09 15:56:52.414263 gpt-review-0.8.0rc549.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0    10080 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     2772 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     3266 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0      788 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     9707 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      523 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      218 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     3124 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/test_github.py
--rw-r--r--   0        0        0     6815 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      590 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1015 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/test_report.py
--rw-r--r--   0        0        0      420 2023-05-09 15:56:45.810219 gpt-review-0.8.0rc549.post1/tests/test_review.py
--rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc549.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2153 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4246 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1851 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8346 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-09 16:49:37.499710 gpt-review-0.8.0rc552.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-09 16:49:37.503710 gpt-review-0.8.0rc552.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     8702 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     2772 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5769 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     3481 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     9707 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      523 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      218 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     4002 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_github.py
+-rw-r--r--   0        0        0     6830 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1222 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_report.py
+-rw-r--r--   0        0        0      420 2023-05-09 16:49:25.859544 gpt-review-0.8.0rc552.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc552.post1/PKG-INFO
```

### Comparing `gpt-review-0.8.0rc549.post1/.devcontainer/devcontainer.json` & `gpt-review-0.8.0rc552.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.8.0rc552.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/dependabot.yml` & `gpt-review-0.8.0rc552.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/pull_request_template.md` & `gpt-review-0.8.0rc552.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/workflows/codeql.yml` & `gpt-review-0.8.0rc552.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.8.0rc552.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.8.0rc552.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/workflows/python.yml` & `gpt-review-0.8.0rc552.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.github/workflows/test-action.yml` & `gpt-review-0.8.0rc552.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/.gitignore` & `gpt-review-0.8.0rc552.post1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -124,8 +124,9 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-index.*
+# Default Directory for llama index files
+storage/
```

### Comparing `gpt-review-0.8.0rc549.post1/.vscode/settings.json` & `gpt-review-0.8.0rc552.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/LICENSE` & `gpt-review-0.8.0rc552.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/README.md` & `gpt-review-0.8.0rc552.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/action.yml` & `gpt-review-0.8.0rc552.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/pyproject.toml` & `gpt-review-0.8.0rc552.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/_git.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/_github.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/_repository.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/_review.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/constants.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/src/gpt_review/main.py` & `gpt-review-0.8.0rc552.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/tests/conftest.py` & `gpt-review-0.8.0rc552.post1/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pytest
 import yaml
 from collections import namedtuple
 
+from llama_index import SimpleDirectoryReader
+
 
 @pytest.fixture
 def mock_openai(monkeypatch) -> None:
     """
     Mock OpenAI Functions with monkeypatch
     - aopenai.ChatCompletion.create
     """
@@ -17,15 +19,22 @@
         def __init__(self) -> None:
             self.choices = [namedtuple("mockMessage", "message")(*[namedtuple("mockContent", "content")(*[["test"]])])]
 
     class MockQueryResponse:
         def __init__(self) -> None:
             self.response = "test"
 
+    class MockStorageContext:
+        def persist(self, persist_dir) -> None:
+            pass
+
     class MockIndex:
+        def __init__(self) -> None:
+            self.storage_context = MockStorageContext()
+
         def query(self, question: str) -> MockQueryResponse:
             assert isinstance(question, str)
             return MockQueryResponse()
 
         def as_query_engine(self):
             return self
 
@@ -39,16 +48,30 @@
         presence_penalty,
     ) -> MockResponse:
         return MockResponse()
 
     def from_documents(documents, service_context=None) -> MockIndex:
         return MockIndex()
 
+    class MockRepoReader:
+        def __init__(self, owner, repo, use_parser) -> None:
+            self.owner = owner
+            self.repo = repo
+            self.use_parser = use_parser
+
+    def init_mock_reader(self, owner, repo, use_parser) -> None:
+        MockRepoReader(owner=owner, repo=repo, use_parser=use_parser)
+
+    def mock_load_data_from_branch(self, branch):
+        return SimpleDirectoryReader(input_dir=".").load_data()
+
     monkeypatch.setattr("openai.ChatCompletion.create", mock_create)
     monkeypatch.setattr("llama_index.GPTVectorStoreIndex.from_documents", from_documents)
+    monkeypatch.setattr("llama_index.GithubRepositoryReader.__init__", init_mock_reader)
+    monkeypatch.setattr("llama_index.GithubRepositoryReader._load_data_from_branch", mock_load_data_from_branch)
 
 
 @pytest.fixture
 def mock_github(monkeypatch) -> None:
     """
     Mock GitHub Functions with monkeypatch
     - requests.get
```

### Comparing `gpt-review-0.8.0rc549.post1/tests/mock.diff` & `gpt-review-0.8.0rc552.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/tests/test_github.py` & `gpt-review-0.8.0rc552.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/tests/test_gpt_cli.py` & `gpt-review-0.8.0rc552.post1/tests/test_gpt_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 
 ROOT_COMMANDS = [
     CLICase("--version"),
     CLICase("--help"),
 ]
 
+WHAT_LANGUAGE = "what programming language is this code written in?"
+
 ASK_COMMANDS = [
     CLICase("ask --help"),
     CLICase("ask how are you"),
     CLICase("ask --fast how are you"),
     CLICase(f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT}"),
     CLICase(
         "ask how are you --fast --max-tokens",
@@ -98,23 +100,20 @@
     ),
     CLICase(
         f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"
     ),
     CLICase(
         f"""ask how are you --fast --max-tokens {C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"""
     ),
-    CLICase(
-        "ask --files src/gpt_review/main.py --files src/gpt_review/main.py what programming language is this code written in?"
-    ),
     CLICase("github review --help"),
     CLICase("github review"),
-    CLICase(
-        "ask --files src/gpt_review/__init__.py --files src/gpt_review/__init__.py what programming language is this code written in?"
-    ),
-    CLICase("ask --fast -f src/gpt_review/__init__.py what programming language is this code written in?"),
+    CLICase(f"ask --files src/gpt_review/__init__.py --files src/gpt_review/__init__.py {WHAT_LANGUAGE}"),
+    CLICase(f"ask --fast -f src/gpt_review/__init__.py {WHAT_LANGUAGE}"),
+    CLICase(f"ask --fast -d src/gpt_review --recursive --hidden --required-exts .py {WHAT_LANGUAGE}"),
+    CLICase(f"ask --fast -repo microsoft/gpt-review {WHAT_LANGUAGE}"),
 ]
 
 GIT_COMMANDS = [
     CLICase("git commit --help"),
     # CLICase("git commit"),
     # CLICase("git commit --large"),
     # CLICase("git commit --gpt4"),
```

### Comparing `gpt-review-0.8.0rc549.post1/tests/test_llama_index.py` & `gpt-review-0.8.0rc552.post1/tests/test_llama_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Tests for the Llame Index Package."""
 import pytest
 
 from gpt_review._ask import _load_azure_openai_context
-from gpt_review._llama_index import _ask_doc
+from gpt_review._llama_index import _query_index
 
 
 def ask_doc_test() -> None:
     _load_azure_openai_context()
     question = "What is the name of the package?"
     files = ["src/gpt_review/__init__.py"]
-    _ask_doc(question, files, fast=True)
+    _query_index(question, files, fast=True)
+
+    # Try again to use the cached index
+    _query_index(question, files, fast=True)
 
 
 def test_ask_doc(mock_openai) -> None:
     """Unit Test for the ask_doc function."""
     ask_doc_test()
```

### Comparing `gpt-review-0.8.0rc549.post1/tests/test_report.py` & `gpt-review-0.8.0rc552.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc549.post1/PKG-INFO` & `gpt-review-0.8.0rc552.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.8.0rc549.post1
+Version: 0.8.0rc552.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc549.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc552.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

