# Comparing `tmp/microsoft-kiota-http-0.4.1.tar.gz` & `tmp/microsoft-kiota-http-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-http-0.4.1.tar", last modified: Thu Mar 30 13:04:52 2023, max compression
+gzip compressed data, was "microsoft-kiota-http-0.4.2.tar", last modified: Tue May  9 10:48:49 2023, max compression
```

## Comparing `microsoft-kiota-http-0.4.1.tar` & `microsoft-kiota-http-0.4.2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0       80 2023-03-30 13:04:48.807835 microsoft-kiota-http-0.4.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-03-30 13:04:48.807835 microsoft-kiota-http-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-03-30 13:04:48.807835 microsoft-kiota-http-0.4.1/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1800 2023-03-30 13:04:48.807835 microsoft-kiota-http-0.4.1/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/.gitignore
--rw-r--r--   0        0        0    15946 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/.pylintrc
--rw-r--r--   0        0        0      887 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/LICENSE
--rw-r--r--   0        0        0      447 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/Pipfile
--rw-r--r--   0        0        0    39513 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/Pipfile.lock
--rw-r--r--   0        0        0     2376 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/README.md
--rw-r--r--   0        0        0     2757 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/SUPPORT.md
--rw-r--r--   0        0        0      121 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/__init__.py
--rw-r--r--   0        0        0       23 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/_version.py
--rw-r--r--   0        0        0    14236 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/httpx_request_adapter.py
--rw-r--r--   0        0        0     4823 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/kiota_client_factory.py
--rw-r--r--   0        0        0      276 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/__init__.py
--rw-r--r--   0        0        0      652 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/async_kiota_transport.py
--rw-r--r--   0        0        0     2011 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/middleware.py
--rw-r--r--   0        0        0      321 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/options/__init__.py
--rw-r--r--   0        0        0     1621 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
--rw-r--r--   0        0        0     2127 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/options/redirect_handler_option.py
--rw-r--r--   0        0        0      858 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/options/response_handler_option.py
--rw-r--r--   0        0        0     3067 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/options/retry_handler_option.py
--rw-r--r--   0        0        0      714 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/options/telemetry_handler_option.py
--rw-r--r--   0        0        0     2303 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     8479 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/redirect_handler.py
--rw-r--r--   0        0        0     8057 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/kiota_http/middleware/retry_handler.py
--rw-r--r--   0        0        0     1286 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     4085 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      114 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0     4498 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/helpers/mock_response_object.py
--rw-r--r--   0        0        0      105 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/helpers/office_location.py
--rw-r--r--   0        0        0        0 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/middleware_tests/__init__.py
--rw-r--r--   0        0        0      989 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/middleware_tests/test_parameters_name_decoding_handler.py
--rw-r--r--   0        0        0     2207 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/middleware_tests/test_redirect_handler.py
--rw-r--r--   0        0        0     4324 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/middleware_tests/test_retry_handler.py
--rw-r--r--   0        0        0     9066 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/test_httpx_request_adapter.py
--rw-r--r--   0        0        0     3277 2023-03-30 13:04:48.811835 microsoft-kiota-http-0.4.1/tests/test_kiota_client_factory.py
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft-kiota-http-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      117 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1800 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.gitignore
+-rw-r--r--   0        0        0    15946 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/.pylintrc
+-rw-r--r--   0        0        0     1002 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/LICENSE
+-rw-r--r--   0        0        0      447 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/Pipfile
+-rw-r--r--   0        0        0    39819 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/Pipfile.lock
+-rw-r--r--   0        0        0     2376 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/README.md
+-rw-r--r--   0        0        0     2757 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/SUPPORT.md
+-rw-r--r--   0        0        0      121 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/kiota_http/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/kiota_http/_version.py
+-rw-r--r--   0        0        0    14620 2023-05-09 10:48:45.280268 microsoft-kiota-http-0.4.2/kiota_http/httpx_request_adapter.py
+-rw-r--r--   0        0        0     4823 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/kiota_client_factory.py
+-rw-r--r--   0        0        0      276 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/__init__.py
+-rw-r--r--   0        0        0      652 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/async_kiota_transport.py
+-rw-r--r--   0        0        0     2011 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/middleware.py
+-rw-r--r--   0        0        0      321 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/__init__.py
+-rw-r--r--   0        0        0     1621 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/parameters_name_decoding_handler_option.py
+-rw-r--r--   0        0        0     2127 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/redirect_handler_option.py
+-rw-r--r--   0        0        0      858 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/response_handler_option.py
+-rw-r--r--   0        0        0     3067 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/retry_handler_option.py
+-rw-r--r--   0        0        0      714 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/options/telemetry_handler_option.py
+-rw-r--r--   0        0        0     2303 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     8479 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/redirect_handler.py
+-rw-r--r--   0        0        0     8057 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/kiota_http/middleware/retry_handler.py
+-rw-r--r--   0        0        0     1286 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1810 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     4636 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      114 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     4498 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/helpers/mock_response_object.py
+-rw-r--r--   0        0        0      105 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/helpers/office_location.py
+-rw-r--r--   0        0        0        0 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/__init__.py
+-rw-r--r--   0        0        0      989 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/test_parameters_name_decoding_handler.py
+-rw-r--r--   0        0        0     2207 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/test_redirect_handler.py
+-rw-r--r--   0        0        0     4324 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/middleware_tests/test_retry_handler.py
+-rw-r--r--   0        0        0    10291 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/test_httpx_request_adapter.py
+-rw-r--r--   0        0        0     3277 2023-05-09 10:48:45.284268 microsoft-kiota-http-0.4.2/tests/test_kiota_client_factory.py
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 microsoft-kiota-http-0.4.2/PKG-INFO
```

### Comparing `microsoft-kiota-http-0.4.1/.github/workflows/auto-merge-dependabot.yml` & `microsoft-kiota-http-0.4.2/.github/workflows/auto-merge-dependabot.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.3.6
+        uses: dependabot/fetch-metadata@v1.4.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft-kiota-http-0.4.1/.github/workflows/build_publish.yml` & `microsoft-kiota-http-0.4.2/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/.github/workflows/codeql-analysis.yml` & `microsoft-kiota-http-0.4.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/.github/workflows/conflicting-pr-label.yml` & `microsoft-kiota-http-0.4.2/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/.gitignore` & `microsoft-kiota-http-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/.pylintrc` & `microsoft-kiota-http-0.4.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/CHANGELOG.md` & `microsoft-kiota-http-0.4.2/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.2] - 2023-05-02
+
+### Added
+
+### Changed
+
+- Includes Response headers in APIException for failed requests.
+
 ## [0.4.1] - 2023-03-29
 
 ### Added
 
 ### Changed
 
 - Fixed bug with mapping when deserializing primitive response types.
```

### Comparing `microsoft-kiota-http-0.4.1/LICENSE` & `microsoft-kiota-http-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/Pipfile.lock` & `microsoft-kiota-http-0.4.2/Pipfile.lock`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9429262258209626%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'9168d36e511d3e76f3df5bdd3f2f496a5d8ce2a88baa0ce9206514aacae0538d'}}",*

 * * "'default'": "{'httpcore': {'hashes': "*

 * *              "['sha256:0fdfea45e94f0c9fd96eab9286077f9ff788dd186635ae61b312693e4d943599', "*

 * *              "'sha256:cc045a3241afbf60ce056202301b4d8b6af08845e3294055eb26b09913ef903c'], "*

 * *              "'version': '==0.17.0'}, 'httpx': {'hashes': "*

 * *              "['sha256:447556b50c1921c351ea54b4fe79d91b724ed2b027462ab9a329465d147d5a4e', "*

 * *             […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "3cbdb1f90e92518f94aa1492c00013f27622351d385f060bd5890631e206faa7"
+            "sha256": "9168d36e511d3e76f3df5bdd3f2f496a5d8ce2a88baa0ce9206514aacae0538d"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
@@ -51,30 +51,30 @@
                 "sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095"
             ],
             "markers": "python_full_version >= '3.6.1'",
             "version": "==4.0.0"
         },
         "httpcore": {
             "hashes": [
-                "sha256:c5d6f04e2fc530f39e0c077e6a30caa53f1451096120f1f38b954afd0b17c0cb",
-                "sha256:da1fb708784a938aa084bde4feb8317056c55037247c787bd7e19eb2c2949dc0"
+                "sha256:0fdfea45e94f0c9fd96eab9286077f9ff788dd186635ae61b312693e4d943599",
+                "sha256:cc045a3241afbf60ce056202301b4d8b6af08845e3294055eb26b09913ef903c"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.16.3"
+            "version": "==0.17.0"
         },
         "httpx": {
             "extras": [
                 "http2"
             ],
             "hashes": [
-                "sha256:9818458eb565bb54898ccb9b8b251a28785dd4a55afbc23d0eb410754fe7d0f9",
-                "sha256:a211fcce9b1254ea24f0cd6af9869b3d29aba40154e947d2a07bb499b3e310d6"
+                "sha256:447556b50c1921c351ea54b4fe79d91b724ed2b027462ab9a329465d147d5a4e",
+                "sha256:507d676fc3e26110d41df7d35ebd8b3b8585052450f4097401c9be59d928c63e"
             ],
             "index": "pypi",
-            "version": "==0.23.3"
+            "version": "==0.24.0"
         },
         "hyperframe": {
             "hashes": [
                 "sha256:0ec6bafd80d8ad2195c4f03aacba3a8265e57bc4cff261e802bf39970ed02a15",
                 "sha256:ae510046231dc8e9ecb1a6586f63d2347bf4c8905914aa84ba585ae85f28a914"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -86,29 +86,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "microsoft-kiota-abstractions": {
             "hashes": [
-                "sha256:05235ea101725d5766408fec149c04dc2e0ca71b7b31a0e920987bb97a44cf81",
-                "sha256:6a5dfbeb2d6bc6d05e79ce3cbbd487da36fc0ddf0ecbab58ca96222ff2daa39e"
+                "sha256:1e9e3696b2414e6a6787e756eb69c658743f8db2b9eef8ecc415e03f6bc8b9c9",
+                "sha256:3ff7a0ba5d0476d7b6765d71fa3153b4198cb5507d367640d20d8e5107efd64c"
             ],
             "index": "pypi",
-            "version": "==0.5.0"
-        },
-        "rfc3986": {
-            "extras": [
-                "idna2008"
-            ],
-            "hashes": [
-                "sha256:270aaf10d87d0d4e095063c65bf3ddbc6ee3d0b226328ce21e036f946e421835",
-                "sha256:a86d6e1f5b1dc238b218b012df0aa79409667bb209e58da56d0b94704e712a97"
-            ],
-            "version": "==1.5.0"
+            "version": "==0.5.1"
         },
         "sniffio": {
             "hashes": [
                 "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
                 "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
             ],
             "markers": "python_version >= '3.7'",
@@ -122,36 +112,28 @@
             "markers": "python_version >= '3.6'",
             "version": "==4.1.1"
         }
     },
     "develop": {
         "astroid": {
             "hashes": [
-                "sha256:525f126d5dc1b8b0b6ee398b33159105615d92dc4a17f2cd064125d57f6186fa",
-                "sha256:e3e4d0ffc2d15d954065579689c36aac57a339a4679a679579af6401db4d3fdb"
+                "sha256:a1b8543ef9d36ea777194bc9b17f5f8678d2c56ee6a45b2c2f17eec96f242347",
+                "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
             ],
             "markers": "python_full_version >= '3.7.2'",
-            "version": "==2.15.0"
+            "version": "==2.15.4"
         },
         "asyncmock": {
             "hashes": [
                 "sha256:c251889d542e98fe5f7ece2b5b8643b7d62b50a5657d34a4cbce8a1d5170d750",
                 "sha256:fd8bc4e7813251a8959d1140924ccba3adbbc7af885dba7047c67f73c0b664b1"
             ],
             "index": "pypi",
             "version": "==0.4.2"
         },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
-        },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==2022.12.7"
@@ -230,93 +212,109 @@
                 "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
                 "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
                 "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
                 "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
                 "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
                 "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
             ],
-            "markers": "python_version >= '3.7'",
+            "markers": "python_full_version >= '3.7.0'",
             "version": "==3.1.0"
         },
+        "colorama": {
+            "hashes": [
+                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
+                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
+            ],
+            "markers": "sys_platform == 'win32'",
+            "version": "==0.4.6"
+        },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
-                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
-                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
-                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
-                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
-                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
-                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
-                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
-                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
-                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
-                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
-                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
-                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
-                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
-                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
-                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
-                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
-                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
-                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
-                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
-                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
-                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
-                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
-                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
-                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
-                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
-                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
-                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
-                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
-                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
-                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
-                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
-                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
-                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
-                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
-                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
-                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
-                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
-                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
-                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
-                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
-                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
-                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
-                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
-                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
-                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
-                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
-                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
-                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
-                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
-                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
+                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
+                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
+                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
+                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
+                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
+                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
+                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
+                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
+                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
+                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
+                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
+                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
+                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
+                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
+                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
+                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
+                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
+                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
+                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
+                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
+                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
+                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
+                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
+                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
+                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
+                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
+                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
+                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
+                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
+                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
+                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
+                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
+                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
+                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
+                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
+                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
+                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
+                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
+                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
+                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
+                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
+                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
+                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
+                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
+                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
+                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
+                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
+                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
+                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
+                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
+                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.2"
+            "version": "==7.2.5"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
                 "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
                 "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19"
         },
+        "exceptiongroup": {
+            "hashes": [
+                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
+                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==1.1.1"
+        },
         "flit": {
             "hashes": [
                 "sha256:5ee0f88fd1cfa4160d1a8fa01237e96d06d677ae0403a0bbabbb277cb37c5e9c",
                 "sha256:d0f2a8f4bd45dc794befbf5839ecc0fd3830d65a57bd52b5997542fac5d5e937"
             ],
             "index": "pypi",
             "version": "==3.8.0"
@@ -401,99 +399,99 @@
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mock": {
             "hashes": [
-                "sha256:c41cfb1e99ba5d341fbcc5308836e7d7c9786d302f995b2c271ce2144dece9eb",
-                "sha256:e3ea505c03babf7977fd21674a69ad328053d414f05e6433c30d8fa14a534a6b"
+                "sha256:06f18d7d65b44428202b145a9a36e99c2ee00d1eb992df0caf881d4664377891",
+                "sha256:0e0bc5ba78b8db3667ad636d964eb963dc97a59f04c6f6214c5f0e4a8f726c56"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==5.0.1"
+            "version": "==5.0.2"
         },
         "mypy": {
             "hashes": [
-                "sha256:0a28a76785bf57655a8ea5eb0540a15b0e781c807b5aa798bd463779988fa1d5",
-                "sha256:19ba15f9627a5723e522d007fe708007bae52b93faab00f95d72f03e1afa9598",
-                "sha256:21b437be1c02712a605591e1ed1d858aba681757a1e55fe678a15c2244cd68a5",
-                "sha256:26cdd6a22b9b40b2fd71881a8a4f34b4d7914c679f154f43385ca878a8297389",
-                "sha256:2888ce4fe5aae5a673386fa232473014056967f3904f5abfcf6367b5af1f612a",
-                "sha256:2b0c373d071593deefbcdd87ec8db91ea13bd8f1328d44947e88beae21e8d5e9",
-                "sha256:315ac73cc1cce4771c27d426b7ea558fb4e2836f89cb0296cbe056894e3a1f78",
-                "sha256:39c7119335be05630611ee798cc982623b9e8f0cff04a0b48dfc26100e0b97af",
-                "sha256:4b398d8b1f4fba0e3c6463e02f8ad3346f71956b92287af22c9b12c3ec965a9f",
-                "sha256:4e4e8b362cdf99ba00c2b218036002bdcdf1e0de085cdb296a49df03fb31dfc4",
-                "sha256:59bbd71e5c58eed2e992ce6523180e03c221dcd92b52f0e792f291d67b15a71c",
-                "sha256:5b5f81b40d94c785f288948c16e1f2da37203c6006546c5d947aab6f90aefef2",
-                "sha256:5cb14ff9919b7df3538590fc4d4c49a0f84392237cbf5f7a816b4161c061829e",
-                "sha256:61bf08362e93b6b12fad3eab68c4ea903a077b87c90ac06c11e3d7a09b56b9c1",
-                "sha256:64cc3afb3e9e71a79d06e3ed24bb508a6d66f782aff7e56f628bf35ba2e0ba51",
-                "sha256:69b35d1dcb5707382810765ed34da9db47e7f95b3528334a3c999b0c90fe523f",
-                "sha256:9401e33814cec6aec8c03a9548e9385e0e228fc1b8b0a37b9ea21038e64cdd8a",
-                "sha256:a380c041db500e1410bb5b16b3c1c35e61e773a5c3517926b81dfdab7582be54",
-                "sha256:ae9ceae0f5b9059f33dbc62dea087e942c0ccab4b7a003719cb70f9b8abfa32f",
-                "sha256:b7c7b708fe9a871a96626d61912e3f4ddd365bf7f39128362bc50cbd74a634d5",
-                "sha256:c1c10fa12df1232c936830839e2e935d090fc9ee315744ac33b8a32216b93707",
-                "sha256:ce61663faf7a8e5ec6f456857bfbcec2901fbdb3ad958b778403f63b9e606a1b",
-                "sha256:d64c28e03ce40d5303450f547e07418c64c241669ab20610f273c9e6290b4b0b",
-                "sha256:d809f88734f44a0d44959d795b1e6f64b2bbe0ea4d9cc4776aa588bb4229fc1c",
-                "sha256:dbb19c9f662e41e474e0cff502b7064a7edc6764f5262b6cd91d698163196799",
-                "sha256:ef6a01e563ec6a4940784c574d33f6ac1943864634517984471642908b30b6f7"
+                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
+                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
+                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
+                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
+                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
+                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
+                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
+                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
+                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
+                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
+                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
+                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
+                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
+                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
+                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
+                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
+                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
+                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
+                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
+                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
+                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
+                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
+                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
+                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
+                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
+                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
             ],
             "index": "pypi",
-            "version": "==1.1.1"
+            "version": "==1.2.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:024996549ee88ec1a9aa99ff7f8fc819bb59e2c3477b410d90a16d32d6e707aa",
-                "sha256:e5986afb596e4bb5bde29a79ac9061aa955b94fca2399b7aaac4090860920dd8"
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.1.1"
+            "version": "==3.5.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:8660a54e3f696243d644fca98f79013a959c03f979992c1ab59c24d3f4ec2700",
-                "sha256:d4d009b0116e16845533bc2163493d6681846ac725eab8ca8014afb520178ddd"
+                "sha256:761907349e699f8afdcd56c4fe02f3021ab5b3a0fc26d19a9bfdc66c7d0d5cd5",
+                "sha256:a6cbb4c6e96eab4a3c7de7c6383c512478f58f88d95764507d84c899d656a89a"
             ],
             "index": "pypi",
-            "version": "==2.17.1"
+            "version": "==2.17.3"
         },
         "pytest": {
             "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.3.1"
         },
         "pytest-asyncio": {
             "hashes": [
                 "sha256:2b38a496aef56f56b0e87557ec313e11e1ab9276fc3863f6a7be0f1d0e415e1b",
                 "sha256:f2b3366b7cd501a4056858bd39349d5af19742aed2d81660b7998b6341c7eb9c"
             ],
             "index": "pypi",
@@ -513,51 +511,59 @@
                 "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
             ],
             "index": "pypi",
             "version": "==3.10.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b",
+                "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.29.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
             "version": "==0.10.2"
         },
+        "tomli": {
+            "hashes": [
+                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
+                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
+            ],
+            "markers": "python_version < '3.11'",
+            "version": "==2.0.1"
+        },
         "tomli-w": {
             "hashes": [
                 "sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463",
                 "sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "tomlkit": {
             "hashes": [
-                "sha256:07de26b0d8cfc18f871aec595fda24d95b08fef89d147caa861939f37230bf4b",
-                "sha256:71b952e5721688937fb02cf9d354dbcf0785066149d2855e44531ebdd2b65d73"
+                "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171",
+                "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.11.6"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.11.8"
         },
         "types-python-dateutil": {
             "hashes": [
-                "sha256:c640f2eb71b4b94a9d3bfda4c04250d29a24e51b8bad6e12fddec0cf6e96f7a3",
-                "sha256:fbecd02c19cac383bf4a16248d45ffcff17c93a04c0794be5f95d42c6aa5de39"
+                "sha256:355b2cb82b31e556fd18e7b074de7c350c680ab80608f0cc55ba6770d986d67d",
+                "sha256:fe5b545e678ec13e3ddc83a0eee1545c1b5e2fba4cfc39b276ab6f4e7604a923"
             ],
             "index": "pypi",
-            "version": "==2.8.19.10"
+            "version": "==2.8.19.12"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
@@ -645,20 +651,20 @@
                 "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29",
                 "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6",
                 "sha256:f2e69b3ed24544b0d3dbe2c5c0ba5153ce50dcebb576fdc4696d52aa22db6034",
                 "sha256:f87ec75864c37c4c6cb908d282e1969e79763e0d9becdfe9fe5473b7bb1e5f09",
                 "sha256:fbec11614dba0424ca72f4e8ba3c420dba07b4a7c206c8c8e4e73f2e98f4c559",
                 "sha256:fd69666217b62fa5d7c6aa88e507493a34dec4fa20c5bd925e4bc12fce586639"
             ],
-            "markers": "python_version >= '3.11'",
+            "markers": "python_version < '3.11'",
             "version": "==1.15.0"
         },
         "yapf": {
             "hashes": [
-                "sha256:8fea849025584e486fd06d6ba2bed717f396080fd3cc236ba10cb97c4c51cf32",
-                "sha256:a3f5085d37ef7e3e004c4ba9f9b3e40c54ff1901cd111f05145ae313a7c67d1b"
+                "sha256:4c2b59bd5ffe46f3a7da48df87596877189148226ce267c16e8b44240e51578d",
+                "sha256:da62bdfea3df3673553351e6246abed26d9fe6780e548a5af9e70f6d2b4f5b9a"
             ],
             "index": "pypi",
-            "version": "==0.32.0"
+            "version": "==0.33.0"
         }
     }
 }
```

### Comparing `microsoft-kiota-http-0.4.1/README.md` & `microsoft-kiota-http-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/SECURITY.md` & `microsoft-kiota-http-0.4.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/SUPPORT.md` & `microsoft-kiota-http-0.4.2/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/httpx_request_adapter.py` & `microsoft-kiota-http-0.4.2/kiota_http/httpx_request_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -276,45 +276,50 @@
 
     async def throw_failed_responses(
         self, response: httpx.Response, error_map: Dict[str, ParsableFactory]
     ) -> None:
         if response.is_success:
             return
 
-        status_code = response.status_code
-        status_code_str = str(response.status_code)
+        response_status_code = response.status_code
+        response_status_code_str = str(response_status_code)
+        response_headers = response.headers
 
         if not error_map:
             raise APIError(
                 "The server returned an unexpected status code and no error class is registered"
-                f" for this code {status_code}", status_code
+                f" for this code {response_status_code}", response_headers, response_status_code
             )
-        if (status_code_str not in error_map) and (
-            (400 <= status_code < 500 and '4XX' not in error_map) or
-            (500 <= status_code < 600 and '5XX' not in error_map)
+        if (response_status_code_str not in error_map) and (
+            (400 <= response_status_code < 500 and '4XX' not in error_map) or
+            (500 <= response_status_code < 600 and '5XX' not in error_map)
         ):
             raise APIError(
                 "The server returned an unexpected status code and no error class is registered"
-                f" for this code {status_code}", status_code
+                f" for this code {response_status_code}", response_headers, response_status_code
             )
 
         error_class = None
-        if status_code_str in error_map:
-            error_class = error_map[status_code_str]
-        elif 400 <= status_code < 500:
+        if response_status_code_str in error_map:
+            error_class = error_map[response_status_code_str]
+        elif 400 <= response_status_code < 500:
             error_class = error_map['4XX']
-        elif 500 <= status_code < 600:
+        elif 500 <= response_status_code < 600:
             error_class = error_map['5XX']
 
         root_node = await self.get_root_parse_node(response)
         error = root_node.get_object_value(error_class)
 
-        if error:
+        if isinstance(error, APIError):
+            error.response_headers = response_headers
+            error.response_status_code = response_status_code
             raise error
-        raise APIError(f"Unexpected error type: {type(error)}", status_code)
+        raise APIError(
+            f"Unexpected error type: {type(error)}", response_headers, response_status_code
+        )
 
     async def get_http_response_message(self, request_info: RequestInformation) -> httpx.Response:
         self.set_base_url_for_request_information(request_info)
         await self._authentication_provider.authenticate_request(request_info)
 
         request = self.get_request_from_request_information(request_info)
         resp = await self._http_client.send(request)
```

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/kiota_client_factory.py` & `microsoft-kiota-http-0.4.2/kiota_http/kiota_client_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/async_kiota_transport.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/async_kiota_transport.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/middleware.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/options/parameters_name_decoding_handler_option.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/parameters_name_decoding_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/options/redirect_handler_option.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/redirect_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/options/response_handler_option.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/response_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/options/retry_handler_option.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/retry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/options/telemetry_handler_option.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/options/telemetry_handler_option.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/parameters_name_decoding_handler.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/redirect_handler.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/redirect_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/kiota_http/middleware/retry_handler.py` & `microsoft-kiota-http-0.4.2/kiota_http/middleware/retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/pyproject.toml` & `microsoft-kiota-http-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/tests/conftest.py` & `microsoft-kiota-http-0.4.2/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 
 import httpx
 import pytest
 from asyncmock import AsyncMock
+from kiota_abstractions.api_error import APIError
 from kiota_abstractions.authentication import AnonymousAuthenticationProvider
 from kiota_abstractions.request_information import RequestInformation
 
 from kiota_http.httpx_request_adapter import HttpxRequestAdapter
 
 from .helpers import MockErrorObject, MockResponseObject, OfficeLocation
 
@@ -41,30 +42,51 @@
 def mock_error_map():
     return {
         "500": Exception("Internal Server Error"),
     }
 
 
 @pytest.fixture
+def mock_apierror_map():
+    return {
+        "500":
+        APIError(
+            "Custom Internal Server Error", {
+                'cache-control': 'private',
+                'transfer-encoding': 'chunked',
+                'content-type': 'application/json'
+            }, 500
+        )
+    }
+
+
+@pytest.fixture
 def mock_request_adapter():
     resp = httpx.Response(
         json={'error': 'not found'}, status_code=404, headers={"Content-Type": "application/json"}
     )
     mock_request_adapter = AsyncMock
     mock_request_adapter.get_http_response_message = AsyncMock(return_value=resp)
 
 
 @pytest.fixture
-def simple_response():
+def simple_error_response():
     return httpx.Response(
         json={'error': 'not found'}, status_code=404, headers={"Content-Type": "application/json"}
     )
 
 
 @pytest.fixture
+def simple_success_response():
+    return httpx.Response(
+        json={'message': 'Success!'}, status_code=200, headers={"Content-Type": "application/json"}
+    )
+
+
+@pytest.fixture
 def mock_user_response(mocker):
     return httpx.Response(
         200,
         headers={"Content-Type": "application/json"},
         json={
             "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
             "businessPhones": ["+1 205 555 0108"],
```

### Comparing `microsoft-kiota-http-0.4.1/tests/helpers/mock_response_object.py` & `microsoft-kiota-http-0.4.2/tests/helpers/mock_response_object.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/tests/middleware_tests/test_parameters_name_decoding_handler.py` & `microsoft-kiota-http-0.4.2/tests/middleware_tests/test_parameters_name_decoding_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/tests/middleware_tests/test_redirect_handler.py` & `microsoft-kiota-http-0.4.2/tests/middleware_tests/test_redirect_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/tests/middleware_tests/test_retry_handler.py` & `microsoft-kiota-http-0.4.2/tests/middleware_tests/test_retry_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/tests/test_httpx_request_adapter.py` & `microsoft-kiota-http-0.4.2/tests/test_httpx_request_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 def test_get_serialization_writer_factory(request_adapter):
     assert isinstance(
         request_adapter.get_serialization_writer_factory(), SerializationWriterFactoryRegistry
     )
 
 
-def test_get_response_content_type(request_adapter, simple_response):
-    content_type = request_adapter.get_response_content_type(simple_response)
+def test_get_response_content_type(request_adapter, simple_success_response):
+    content_type = request_adapter.get_response_content_type(simple_success_response)
     assert content_type == 'application/json'
 
 
 def test_set_base_url_for_request_information(request_adapter, request_info):
     request_adapter.base_url = BASE_URL
     request_adapter.set_base_url_for_request_information(request_info)
     assert request_info.path_parameters["baseurl"] == BASE_URL
@@ -79,67 +79,91 @@
 def test_enable_backing_store(request_adapter):
     request_adapter.enable_backing_store(None)
     assert request_adapter._parse_node_factory
     assert request_adapter._serialization_writer_factory
 
 
 @pytest.mark.asyncio
-async def test_get_root_parse_node(request_adapter, simple_response):
-    assert simple_response.text == '{"error": "not found"}'
-    assert simple_response.status_code == 404
-    content_type = request_adapter.get_response_content_type(simple_response)
+async def test_get_root_parse_node(request_adapter, simple_success_response):
+    assert simple_success_response.text == '{"message": "Success!"}'
+    assert simple_success_response.status_code == 200
+    content_type = request_adapter.get_response_content_type(simple_success_response)
     assert content_type == 'application/json'
 
     with pytest.raises(Exception) as e:
-        await request_adapter.get_root_parse_node(simple_response)
+        await request_adapter.get_root_parse_node(simple_success_response)
 
 
 @pytest.mark.asyncio
-async def test_throw_failed_responses_null_error_map(request_adapter, simple_response):
-    assert simple_response.text == '{"error": "not found"}'
-    assert simple_response.status_code == 404
-    content_type = request_adapter.get_response_content_type(simple_response)
+async def test_does_not_throw_failed_responses_on_success(request_adapter, simple_success_response):
+    try:
+        assert simple_success_response.text == '{"message": "Success!"}'
+        assert simple_success_response.status_code == 200
+        content_type = request_adapter.get_response_content_type(simple_success_response)
+        assert content_type == 'application/json'
+    except APIError as e:
+        assert False, f"'Function raised an exception {e}"
+
+
+@pytest.mark.asyncio
+async def test_throw_failed_responses_null_error_map(request_adapter, simple_error_response):
+    assert simple_error_response.text == '{"error": "not found"}'
+    assert simple_error_response.status_code == 404
+    content_type = request_adapter.get_response_content_type(simple_error_response)
     assert content_type == 'application/json'
 
     with pytest.raises(APIError) as e:
-        await request_adapter.throw_failed_responses(simple_response, None)
+        await request_adapter.throw_failed_responses(simple_error_response, None)
     assert str(e.value) == "The server returned an unexpected status code and"\
             " no error class is registered for this code 404"
     assert e.value.response_status_code == 404
 
 
 @pytest.mark.asyncio
 async def test_throw_failed_responses_no_error_class(
-    request_adapter, simple_response, mock_error_map
+    request_adapter, simple_error_response, mock_error_map
 ):
-    assert simple_response.text == '{"error": "not found"}'
-    assert simple_response.status_code == 404
-    content_type = request_adapter.get_response_content_type(simple_response)
+    assert simple_error_response.text == '{"error": "not found"}'
+    assert simple_error_response.status_code == 404
+    content_type = request_adapter.get_response_content_type(simple_error_response)
     assert content_type == 'application/json'
 
     with pytest.raises(APIError) as e:
-        await request_adapter.throw_failed_responses(simple_response, mock_error_map)
+        await request_adapter.throw_failed_responses(simple_error_response, mock_error_map)
     assert str(e.value) == "The server returned an unexpected status code and"\
             " no error class is registered for this code 404"
     assert e.value.response_status_code == 404
 
 
 @pytest.mark.asyncio
-async def test_throw_failed_responses_status_code_str_in_error_map(
+async def test_throw_failed_responses_not_apierror(
     request_adapter, mock_error_map, mock_error_object
 ):
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_error_object)
     resp = httpx.Response(status_code=500, headers={"Content-Type": "application/json"})
     assert resp.status_code == 500
     content_type = request_adapter.get_response_content_type(resp)
     assert content_type == 'application/json'
 
     with pytest.raises(Exception) as e:
         await request_adapter.throw_failed_responses(resp, mock_error_map)
-    assert str(e.value) == "Internal Server Error"
+    assert str(e.value) == "Unexpected error type: <class 'Exception'>"
+
+
+@pytest.mark.asyncio
+async def test_throw_failed_responses(request_adapter, mock_apierror_map, mock_error_object):
+    request_adapter.get_root_parse_node = AsyncMock(return_value=mock_error_object)
+    resp = httpx.Response(status_code=500, headers={"Content-Type": "application/json"})
+    assert resp.status_code == 500
+    content_type = request_adapter.get_response_content_type(resp)
+    assert content_type == 'application/json'
+
+    with pytest.raises(APIError) as e:
+        await request_adapter.throw_failed_responses(resp, mock_apierror_map)
+    assert str(e.value) == "Custom Internal Server Error"
 
 
 @pytest.mark.asyncio
 async def test_send_async(request_adapter, request_info, mock_user_response, mock_user):
     request_adapter.get_http_response_message = AsyncMock(return_value=mock_user_response)
     request_adapter.get_root_parse_node = AsyncMock(return_value=mock_user)
     resp = await request_adapter.get_http_response_message(request_info)
```

### Comparing `microsoft-kiota-http-0.4.1/tests/test_kiota_client_factory.py` & `microsoft-kiota-http-0.4.2/tests/test_kiota_client_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-http-0.4.1/PKG-INFO` & `microsoft-kiota-http-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-http
-Version: 0.4.1
+Version: 0.4.2
 Summary: Kiota http request adapter implementation for httpx library
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

