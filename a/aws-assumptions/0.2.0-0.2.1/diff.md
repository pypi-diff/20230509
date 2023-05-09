# Comparing `tmp/aws_assumptions-0.2.0.tar.gz` & `tmp/aws_assumptions-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_assumptions-0.2.0.tar", max compression
+gzip compressed data, was "aws_assumptions-0.2.1.tar", max compression
```

## Comparing `aws_assumptions-0.2.0.tar` & `aws_assumptions-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6191 2023-05-04 15:45:21.952366 aws_assumptions-0.2.0/README.md
--rw-r--r--   0        0        0        1 2023-05-03 20:32:09.274067 aws_assumptions-0.2.0/aws_assumptions/__init__.py
--rwxr-xr-x   0        0        0     6306 2023-05-03 20:08:54.547756 aws_assumptions-0.2.0/aws_assumptions/identity.py
--rwxr-xr-x   0        0        0     5345 2023-05-04 15:42:05.111942 aws_assumptions-0.2.0/aws_assumptions/scripts.py
--rw-r--r--   0        0        0      661 2023-05-04 15:47:21.765634 aws_assumptions-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7230 1970-01-01 00:00:00.000000 aws_assumptions-0.2.0/setup.py
--rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 aws_assumptions-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6191 2023-05-04 15:45:21.952366 aws_assumptions-0.2.1/README.md
+-rw-r--r--   0        0        0        1 2023-05-03 20:32:09.274067 aws_assumptions-0.2.1/aws_assumptions/__init__.py
+-rwxr-xr-x   0        0        0     6451 2023-05-09 19:06:36.344510 aws_assumptions-0.2.1/aws_assumptions/identity.py
+-rwxr-xr-x   0        0        0     5345 2023-05-04 15:42:05.111942 aws_assumptions-0.2.1/aws_assumptions/scripts.py
+-rw-r--r--   0        0        0      661 2023-05-09 19:08:25.283297 aws_assumptions-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7230 1970-01-01 00:00:00.000000 aws_assumptions-0.2.1/setup.py
+-rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 aws_assumptions-0.2.1/PKG-INFO
```

### Comparing `aws_assumptions-0.2.0/README.md` & `aws_assumptions-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aws_assumptions-0.2.0/aws_assumptions/identity.py` & `aws_assumptions-0.2.1/aws_assumptions/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,21 @@
     __slots__ = [
         "AccessKeyId",
         "SecretAccessKey",
         "SessionToken",
         "Expiration",
     ]
 
+    def __init__(self, **kwargs):
+        args = {
+            k: str(v) for k, v in kwargs.items()
+        }
+        super().__init__(**args)
+
+
     def __getattribute__(self, __name: str) -> Any:
         # So I like dots..... Get over it.....
         if __name in super().__getattribute__("__slots__"):
             return super().__getitem__(__name)
         else:
             return super().__getattribute__(__name)
```

### Comparing `aws_assumptions-0.2.0/aws_assumptions/scripts.py` & `aws_assumptions-0.2.1/aws_assumptions/scripts.py`

 * *Files identical despite different names*

### Comparing `aws_assumptions-0.2.0/pyproject.toml` & `aws_assumptions-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-assumptions"
-version = "0.2.0"
+version = "0.2.1"
 description = "Assume role(s) from a terminal and easily manage boto3 clients for multiple identities at once."
 authors = ["Mathew Moon <me@mathewmoon.net>"]
 packages = [
     { include = "aws_assumptions"}
 ]
 homepage = "https://github.com/mathewmoon/aws-assumptions"
 documentation = "https://github.com/mathewmoon/aws-assumptions"
```

### Comparing `aws_assumptions-0.2.0/setup.py` & `aws_assumptions-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['boto3>=1.26', 'python-dotenv>=1.0.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['assumptions = aws_assumptions.scripts:main']}
 
 setup_kwargs = {
     'name': 'aws-assumptions',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Assume role(s) from a terminal and easily manage boto3 clients for multiple identities at once.',
     'long_description': '# aws-assumptions\n\n* Easily switch between roles, or a chain of roles and create boto3 clients and resources off of those assumed identities.\n* Can be used as a library to assume roles. The created object also provides a factory for creating boto3 clients/resources off of the object\n* CLI script that allows printing credentials to stdout as either the standard response from boto3.sts.assume_role or formatted to use as env vars in a *nix terminal.\n* CLI provides `exec` command to execute terminal commands in a subshell with the newly minted credentials injected into the environment\n\n\n### Available CLI commands\n```\n~  > assumptions -h\nusage: assumptions [-h] {whoami,assume} ...\n\npositional arguments:\n  {whoami,assume,exec}\n\noptional arguments:\n  -h, --help       show this help message and exit\n\nSwitch roles, or through a chain or roles, or print identity information from AWS STS\n```\n\n### Getting current identity\n```\n> assumptions whoami -h\nusage: assumptions whoami [-h]\n\noptional arguments:\n  -h, --help  show this help message and exit\n\nPrints get-caller-identity info in JSON format\n```\n\n### Assuming a role\n```\n~  > assumptions assume -h\nusage: assumptions assume [-h] -r ROLE_ARN [-n ROLE_SESSION_NAME] [-p POLICY_ARN] [-t TAG] [-T TRANSITIVE_TAG_KEY] [-E EXTERNAL_ID] [-d DURATION_SECONDS] [-e]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -r ROLE_ARN, --role-arn ROLE_ARN\n                        Role to assume. If declared multiple times each role will assume the next in the order given. All other options will be applied to all roles in the chain.\n  -n ROLE_SESSION_NAME, --role-session-name ROLE_SESSION_NAME\n                        The session name to use with the role.\n  -p POLICY_ARN, --policy-arn POLICY_ARN\n                        Optional policy to attach to a session. Can be declared multiple times.\n  -t TAG, --tag TAG     Optional tag to add to the session in the format of `mytagkey=myvalue`. Can be declared multiple times for multiple tags.\n  -T TRANSITIVE_TAG_KEY, --transitive-tag-key TRANSITIVE_TAG_KEY\n                        Transitive tag key. Can be declared multiple times.\n  -E EXTERNAL_ID, --external-id EXTERNAL_ID\n                        Optional External ID for the session. Required by some AssumeRole policies\n  -d DURATION_SECONDS, --duration-seconds DURATION_SECONDS\n                        Optional duration for the session.\n  -e, --env-vars        Output env vars usable from a terminal. If not set the output will match the output of aws-cli\'s `aws sts assume-role` JSON\n\nAssume a role or a chain of roles with optional attributes, outputting the newly acquired credentials. Maintains parity with boto3\'s sts.assume_role except for MFA\n```\n\nExample of assuming a role with env vars\n```\n> assumptions assume -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com -e > creds.env\n> . creds.env\n```\n\nor\n\n```\n$(assumptions assume -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com)\n```\n\n### Using `exec`\n\n```\nusage: scripts.py exec [-h] -r ROLE_ARN [-n ROLE_SESSION_NAME] [-p POLICY_ARN] [-t TAG] [-T TRANSITIVE_TAG_KEY] [-E EXTERNAL_ID] [-d DURATION_SECONDS] [-N] [-e ENV_VAR] [--env-file ENV_FILE] ...\n\npositional arguments:\n  exec_command\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -r ROLE_ARN, --role-arn ROLE_ARN\n                        Role to assume. If declared multiple times each role will assume the next in the order given. All other options will be applied to all roles in the chain.\n  -n ROLE_SESSION_NAME, --role-session-name ROLE_SESSION_NAME\n                        The session name to use with the role.\n  -p POLICY_ARN, --policy-arn POLICY_ARN\n                        Optional policy to attach to a session. Can be declared multiple times.\n  -t TAG, --tag TAG     Optional tag to add to the session in the format of `mytagkey=myvalue`. Can be declared multiple times for multiple tags.\n  -T TRANSITIVE_TAG_KEY, --transitive-tag-key TRANSITIVE_TAG_KEY\n                        Transitive tag key. Can be declared multiple times.\n  -E EXTERNAL_ID, --external-id EXTERNAL_ID\n                        Optional External ID for the session. Required by some AssumeRole policies\n  -d DURATION_SECONDS, --duration-seconds DURATION_SECONDS\n                        Optional duration for the session.\n  -N, --no-inherit-env  Don\'t allow the executed command to inherit the parent\'s env.\n  -e ENV_VAR, --env-var ENV_VAR\n                        Env var in the format `MYVAR=foo` to pass to the executed command\'s environment. Can be declared multiple times.\n  --env-file ENV_FILE   Load env vars from a .env file.\n\nExecute a command in a shell with newly created credentials.\n```\n\nExample\n```\n> assumptions exec -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com aws sts get-caller-identity\n{\n    "UserId": "AROA4HO3IAI67GZHCWWWQ:bob@nowhere.com",\n    "Account": "840662778429",\n    "Arn": "arn:aws:sts::123456789876:assumed-role/my-role/bob@nowhere.com"\n}\n```\n\nExample passing env vars to an interactive shell\n```\n> assumptions exec -r "arn:aws:iam::123456789876:role/my-role" -n bob@nowhere.com -e FOO=bar bash\n$ echo $FOO\nbar\n```\n\n## Switching through multiple roles\nIf you need to chain roles (EG: Assume a role that assumes a role that assumes a role) you can pass the `-r` flag multiple times.\nNote however that all other options, such as `--external-id` or `--tag` will be applied to every session in the chain.\n\n## As a library\n\nAssuming a role and creating clients\n```python\nfrom aws_assumptions.identity import Identity\n\nsession = Identity(\n  RoleArn="arn:aws:iam::123456789876:role/my-role",\n  RoleSessionName="bob"\n)\n\nres = session.client("eks").list_clusters()\ncurrent_role = session.whoami()\nsession_that_made_current_rule = session.whomademe()\n```\n\nChaining roles\n\n```python\nfrom aws_assumptions.identity import Identity\n\nsession = Identity(\n  RoleArn=[\n    "arn:aws:iam::123456789876:role/my-role",\n    "arn:aws:iam::123456789876:role/my-second-role"\n  ],\n  RoleSessionName="bob"\n)\n\nres = session.client("eks").list_clusters()\ncurrent_role = session.whoami()\nsession_that_made_current_rule = session.whomademe()\n```\n\n',
     'author': 'Mathew Moon',
     'author_email': 'me@mathewmoon.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mathewmoon/aws-assumptions',
```

### Comparing `aws_assumptions-0.2.0/PKG-INFO` & `aws_assumptions-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-assumptions
-Version: 0.2.0
+Version: 0.2.1
 Summary: Assume role(s) from a terminal and easily manage boto3 clients for multiple identities at once.
 Home-page: https://github.com/mathewmoon/aws-assumptions
 Author: Mathew Moon
 Author-email: me@mathewmoon.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

