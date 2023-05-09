# Comparing `tmp/tap-github-2.0.0.tar.gz` & `tmp/tap-github-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-github-2.0.0.tar", last modified: Thu Sep 29 09:45:42 2022, max compression
+gzip compressed data, was "tap-github-2.0.1.tar", last modified: Tue May  9 13:40:33 2023, max compression
```

## Comparing `tap-github-2.0.0.tar` & `tap-github-2.0.1.tar`

### file list

```diff
@@ -1,50 +1,62 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-09-29 09:45:42.367094 tap-github-2.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-09-29 09:42:13.000000 tap-github-2.0.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2022-09-29 09:42:13.000000 tap-github-2.0.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-09-29 09:45:42.367094 tap-github-2.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4468 2022-09-29 09:42:13.000000 tap-github-2.0.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-09-29 09:45:42.367094 tap-github-2.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-09-29 09:42:13.000000 tap-github-2.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-09-29 09:45:42.363094 tap-github-2.0.0/tap_github/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      956 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13523 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2737 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-09-29 09:45:42.367094 tap-github-2.0.0/tap_github/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1394 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/assignees.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1468 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/collaborators.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2744 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2674 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/commit_comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6843 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/commits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33251 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26740 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/issue_events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      564 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/issue_labels.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2819 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/issue_milestones.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6192 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/issues.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/pr_commits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2811 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/project_cards.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/project_columns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/projects.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46825 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/pull_requests.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4696 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/releases.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3630 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/review_comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1393 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/reviews.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-09-29 09:45:42.367094 tap-github-2.0.0/tap_github/schemas/shared/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      381 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/shared/issue_permissions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/shared/performed_via_github_app.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/shared/pull_permissions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/shared/reactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/shared/user.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      348 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/stargazers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1571 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/team_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      336 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/team_memberships.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      894 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/schemas/teams.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30669 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10030 2022-09-29 09:42:13.000000 tap-github-2.0.0/tap_github/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-09-29 09:45:42.363094 tap-github-2.0.0/tap_github.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-09-29 09:45:42.000000 tap-github-2.0.0/tap_github.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1389 2022-09-29 09:45:42.000000 tap-github-2.0.0/tap_github.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-09-29 09:45:42.000000 tap-github-2.0.0/tap_github.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2022-09-29 09:45:42.000000 tap-github-2.0.0/tap_github.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2022-09-29 09:45:42.000000 tap-github-2.0.0/tap_github.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2022-09-29 09:45:42.000000 tap-github-2.0.0/tap_github.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 13:40:32.995657 tap-github-2.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-10-26 18:47:27.000000 tap-github-2.0.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       91 2022-10-26 18:47:27.000000 tap-github-2.0.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-05-09 13:40:32.991657 tap-github-2.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4468 2022-10-26 18:47:27.000000 tap-github-2.0.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-09 13:40:32.995657 tap-github-2.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      895 2023-05-09 13:40:12.000000 tap-github-2.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 13:40:32.967656 tap-github-2.0.1/tap_github/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      956 2023-04-25 18:36:52.000000 tap-github-2.0.1/tap_github/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13921 2023-05-09 13:40:12.000000 tap-github-2.0.1/tap_github/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-04-25 14:24:22.000000 tap-github-2.0.1/tap_github/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2737 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 13:40:32.983657 tap-github-2.0.1/tap_github/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1394 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/assignees.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1468 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/collaborators.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2744 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2674 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/commit_comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6843 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/commits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    33251 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26740 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/issue_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      564 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/issue_labels.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2819 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/issue_milestones.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6192 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/issues.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/pr_commits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2811 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/project_cards.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/project_columns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2639 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/projects.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46825 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/pull_requests.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4696 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/releases.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3630 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/review_comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1393 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/reviews.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 13:40:32.987656 tap-github-2.0.1/tap_github/schemas/shared/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      381 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/shared/issue_permissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1199 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/shared/performed_via_github_app.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      352 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/shared/pull_permissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/shared/reactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/shared/user.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      348 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/stargazers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1571 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/team_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      336 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/team_memberships.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      894 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/schemas/teams.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30669 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10030 2022-10-26 18:47:27.000000 tap-github-2.0.1/tap_github/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 13:40:32.967656 tap-github-2.0.1/tap_github.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      258 2023-05-09 13:40:32.000000 tap-github-2.0.1/tap_github.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1797 2023-05-09 13:40:32.000000 tap-github-2.0.1/tap_github.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-09 13:40:32.000000 tap-github-2.0.1/tap_github.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-05-09 13:40:32.000000 tap-github-2.0.1/tap_github.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-05-09 13:40:32.000000 tap-github-2.0.1/tap_github.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-09 13:40:32.000000 tap-github-2.0.1/tap_github.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-09 13:40:32.991657 tap-github-2.0.1/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5265 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2975 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10401 2023-05-09 13:40:12.000000 tap-github-2.0.1/tests/test_github_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5300 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9228 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_interrupted_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9163 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_interrupted_sync_add_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10788 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_interrupted_sync_remove_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2023-05-09 13:40:12.000000 tap-github-2.0.1/tests/test_github_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2000 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_parent_child_independednt.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10993 2023-05-09 13:40:12.000000 tap-github-2.0.1/tests/test_github_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1016 2022-10-26 18:47:27.000000 tap-github-2.0.1/tests/test_github_sync.py
```

### Comparing `tap-github-2.0.0/LICENSE` & `tap-github-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/README.md` & `tap-github-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/setup.py` & `tap-github-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-github',
-      version='2.0.0',
+      version='2.0.1',
       description='Singer.io tap for extracting data from the GitHub API',
       author='Stitch',
       url='http://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_github'],
       install_requires=[
           'singer-python==5.12.1',
```

### Comparing `tap-github-2.0.0/tap_github/__init__.py` & `tap-github-2.0.1/tap_github/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/client.py` & `tap-github-2.0.1/tap_github/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,18 @@
     """
     error_code = resp.status_code
     try:
         response_json = resp.json()
     except JSONDecodeError:
         response_json = {}
 
+    if stream == "commits" and response_json.get("message") == "Git Repository is empty.":
+        LOGGER.info("Encountered an empty git repository")
+        return None
+
     if error_code == 404 and should_skip_404:
         # Add not accessible stream into list.
         client.not_accessible_repos.add(stream)
         details = ERROR_CODE_EXCEPTION_MAPPING.get(error_code).get("message")
         if source == "teams":
             details += ' or it is a personal account repository'
         message = "HTTP-error-code: 404, Error: {}. Please refer \'{}\' for more details.".format(details, response_json.get("documentation_url"))
@@ -195,16 +199,20 @@
         with metrics.http_request_timer(source) as timer:
             self.session.headers.update(headers)
             resp = self.session.request(method='get', url=url, timeout=self.get_request_timeout())
             if resp.status_code != 200:
                 raise_for_error(resp, source, stream, self, should_skip_404)
             timer.tags[metrics.Tag.http_status_code] = resp.status_code
             rate_throttling(resp, self.max_sleep_seconds)
-            if resp.status_code == 404:
+            if resp.status_code in {404, 409}:
                 # Return an empty response body since we're not raising a NotFoundException
+
+                # In the 409 case, this is only for `commits` returning an
+                # error for an empty repository, so we'll treat this as an
+                # empty list of records to process
                 resp._content = b'{}' # pylint: disable=protected-access
             return resp
 
     def authed_get_all_pages(self, source, url, headers={}, stream="", should_skip_404 = True):
         """
         Fetch all pages of records and return them.
         """
@@ -220,15 +228,15 @@
                 break
 
     def verify_repo_access(self, url_for_repo, repo):
         """
         Call rest API to verify that the user has sufficient permissions to access this repository.
         """
         try:
-            self.authed_get("verifying repository access", url_for_repo)
+            self.authed_get("verifying repository access", url_for_repo, stream="commits")
         except NotFoundException:
             # Throwing user-friendly error message as it checks token access
             message = "HTTP-error-code: 404, Error: Please check the repository name \'{}\' or you do not have sufficient permissions to access this repository.".format(repo)
             raise NotFoundException(message) from None
 
     def verify_access_for_repo(self):
         """
```

### Comparing `tap-github-2.0.0/tap_github/discover.py` & `tap-github-2.0.1/tap_github/discover.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schema.py` & `tap-github-2.0.1/tap_github/schema.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/assignees.json` & `tap-github-2.0.1/tap_github/schemas/assignees.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/collaborators.json` & `tap-github-2.0.1/tap_github/schemas/collaborators.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/comments.json` & `tap-github-2.0.1/tap_github/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/commit_comments.json` & `tap-github-2.0.1/tap_github/schemas/commit_comments.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/commits.json` & `tap-github-2.0.1/tap_github/schemas/commits.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/events.json` & `tap-github-2.0.1/tap_github/schemas/events.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/issue_events.json` & `tap-github-2.0.1/tap_github/schemas/issue_events.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/issue_labels.json` & `tap-github-2.0.1/tap_github/schemas/issue_labels.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/issue_milestones.json` & `tap-github-2.0.1/tap_github/schemas/issue_milestones.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/issues.json` & `tap-github-2.0.1/tap_github/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/pr_commits.json` & `tap-github-2.0.1/tap_github/schemas/pr_commits.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/project_cards.json` & `tap-github-2.0.1/tap_github/schemas/project_cards.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/project_columns.json` & `tap-github-2.0.1/tap_github/schemas/project_columns.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/projects.json` & `tap-github-2.0.1/tap_github/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/pull_requests.json` & `tap-github-2.0.1/tap_github/schemas/pull_requests.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/releases.json` & `tap-github-2.0.1/tap_github/schemas/releases.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/review_comments.json` & `tap-github-2.0.1/tap_github/schemas/review_comments.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/reviews.json` & `tap-github-2.0.1/tap_github/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/shared/performed_via_github_app.json` & `tap-github-2.0.1/tap_github/schemas/shared/performed_via_github_app.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/shared/reactions.json` & `tap-github-2.0.1/tap_github/schemas/shared/reactions.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/shared/user.json` & `tap-github-2.0.1/tap_github/schemas/shared/user.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/team_members.json` & `tap-github-2.0.1/tap_github/schemas/team_members.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/schemas/teams.json` & `tap-github-2.0.1/tap_github/schemas/teams.json`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/streams.py` & `tap-github-2.0.1/tap_github/streams.py`

 * *Files identical despite different names*

### Comparing `tap-github-2.0.0/tap_github/sync.py` & `tap-github-2.0.1/tap_github/sync.py`

 * *Files identical despite different names*

