# Comparing `tmp/aws_adfs-2.6.3.tar.gz` & `tmp/aws_adfs-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_adfs-2.6.3.tar", max compression
+gzip compressed data, was "aws_adfs-2.7.0.tar", max compression
```

## Comparing `aws_adfs-2.6.3.tar` & `aws_adfs-2.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/LICENSE
--rw-r--r--   0        0        0    14536 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/README.md
--rw-r--r--   0        0        0      159 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/__init__.py
--rw-r--r--   0        0        0     2750 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/_azure_cloud_mfa_authenticator.py
--rw-r--r--   0        0        0     1848 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/_azure_mfa_authenticator.py
--rw-r--r--   0        0        0    20501 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/_duo_authenticator.py
--rw-r--r--   0        0        0    21283 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/_duo_universal_prompt_authenticator.py
--rw-r--r--   0        0        0     2124 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/_rsa_authenticator.py
--rw-r--r--   0        0        0     2450 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/_symantec_vip_access.py
--rw-r--r--   0        0        0     1518 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/account_aliases_fetcher.py
--rw-r--r--   0        0        0     7315 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/authenticator.py
--rw-r--r--   0        0        0     1327 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/commands.py
--rw-r--r--   0        0        0      217 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/consts.py
--rw-r--r--   0        0        0      856 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/helpers.py
--rw-r--r--   0        0        0     4161 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/html_roles_fetcher.py
--rw-r--r--   0        0        0      778 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/list_profiles.py
--rw-r--r--   0        0        0    24632 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/login.py
--rw-r--r--   0        0        0    10715 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/prepare.py
--rw-r--r--   0        0        0     1243 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/reset.py
--rw-r--r--   0        0        0     2457 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/role_chooser.py
--rw-r--r--   0        0        0     3729 2022-10-29 10:41:09.412789 aws_adfs-2.6.3/aws_adfs/roles_assertion_extractor.py
--rw-r--r--   0        0        0     1496 2022-10-29 10:41:09.416790 aws_adfs-2.6.3/pyproject.toml
--rw-r--r--   0        0        0    16088 1970-01-01 00:00:00.000000 aws_adfs-2.6.3/setup.py
--rw-r--r--   0        0        0    16078 1970-01-01 00:00:00.000000 aws_adfs-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/LICENSE
+-rw-r--r--   0        0        0    14886 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/README.md
+-rw-r--r--   0        0        0      159 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/__init__.py
+-rw-r--r--   0        0        0     3541 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_azure_cloud_mfa_authenticator.py
+-rw-r--r--   0        0        0     1848 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_azure_mfa_authenticator.py
+-rw-r--r--   0        0        0    20501 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_duo_authenticator.py
+-rw-r--r--   0        0        0    21283 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_duo_universal_prompt_authenticator.py
+-rw-r--r--   0        0        0     2124 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_rsa_authenticator.py
+-rw-r--r--   0        0        0     2450 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/_symantec_vip_access.py
+-rw-r--r--   0        0        0     1518 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/account_aliases_fetcher.py
+-rw-r--r--   0        0        0     7373 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/authenticator.py
+-rw-r--r--   0        0        0     1327 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/commands.py
+-rw-r--r--   0        0        0      217 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/consts.py
+-rw-r--r--   0        0        0      856 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/helpers.py
+-rw-r--r--   0        0        0     4161 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/html_roles_fetcher.py
+-rw-r--r--   0        0        0      778 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/list_profiles.py
+-rw-r--r--   0        0        0    24810 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/login.py
+-rw-r--r--   0        0        0    10918 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/prepare.py
+-rw-r--r--   0        0        0     1243 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/reset.py
+-rw-r--r--   0        0        0     2457 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/role_chooser.py
+-rw-r--r--   0        0        0     3729 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/aws_adfs/roles_assertion_extractor.py
+-rw-r--r--   0        0        0     1509 2023-05-09 14:45:03.026833 aws_adfs-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    16445 1970-01-01 00:00:00.000000 aws_adfs-2.7.0/setup.py
+-rw-r--r--   0        0        0    16428 1970-01-01 00:00:00.000000 aws_adfs-2.7.0/PKG-INFO
```

### Comparing `aws_adfs-2.6.3/LICENSE` & `aws_adfs-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/README.md` & `aws_adfs-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 * [duo security](https://duo.com) MFA provider with support for:
   * Duo mobile application push (verified by code or not) using the `Duo Push` authentication method.
   * Phone call using the `Phone Call` authentication method.
   * OTP 6 digit codes generated by Duo Mobile application, and hardware tokens (e.g. RSA or Yubikey) using the `Passcode` authentication method.
   * FIDO U2F (CTAP1) / FIDO2 (CTAP2) hardware authenticators using the `WebAuthn Security Key` authentication method.
 * [Symantec VIP](https://vip.symantec.com/) MFA provider
 * [RSA SecurID](https://www.rsa.com/) MFA provider
+* [Azure AD MFA](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) with support for:
+  * Microsoft Authenticator app
+  * OTP 6 digit codes
+  * SMS codes
+  * Phone call
 
 ## Setup Dependencies
 
 - `build-essential` (provides C/C++ compilers)
 - `python3` `>= 3.7 <4.0`
 - `python3-dev`
 - `libkrb5-dev`
@@ -288,14 +293,16 @@
                                       default one configured server side. Depends
                                       heavily on the Duo factor used. Known Duo
                                       devices that can be used with aws-adfs are
                                       "phone1" for "Duo Push" and "Phone Call"
                                       factors. For "Passcode" and "WebAuthn
                                       Security Key" factors, it is always "None".
       --enforce-role-arn              Only allow the role passed in by --role-arn.
+      --aad-verification-code TEXT    Verification code for Azure AD multi-factor
+                                      authentication.
       --help                          Show this message and exit.
     ```
     <!-- AWS_LOGIN_HELP_END -->
 
     <!-- AWS_RESET_HELP_START -->
     ```
     $ aws-adfs reset --help
```

### Comparing `aws_adfs-2.6.3/aws_adfs/_azure_cloud_mfa_authenticator.py` & `aws_adfs-2.7.0/aws_adfs/_azure_cloud_mfa_authenticator.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,50 +9,53 @@
 import logging
 import time
 
 from . import roles_assertion_extractor
 from .helpers import trace_http_request
 
 
-def extract(html_response, ssl_verification_enabled, session):
+def extract(html_response, ssl_verification_enabled, aad_verification_code, session):
     """
     :param html_response: html result of parsing http response
     :param ssl_verification_enabled: bool to enable SSL verification
     :param session: current requests Session object
     :return:
     """
 
-    roles_page_url = _action_url_on_validation_success(html_response)
+    click.echo(_mfa_instructions(html_response), err=True)
 
-    click.echo('Additional verification is required. Please check your mobile device', err=True)
-
-    # This function polls until we get a SAMLResponse
     return _retrieve_roles_page(
-        roles_page_url,
-        _context(html_response),
+        html_response,
         session,
-        ssl_verification_enabled
+        ssl_verification_enabled,
+        aad_verification_code
     )
 
-
-def _retrieve_roles_page(roles_page_url, context, session, ssl_verification_enabled):
+def _retrieve_roles_page(html_response, session, ssl_verification_enabled, aad_verification_code):
     seconds_to_wait = 5
     max_attempts = 12
     counter = 1
 
     while True:
         time.sleep(seconds_to_wait)
 
+        aad_verification_code_text = _aad_verification_code_text(html_response)
+        if aad_verification_code_text is not None:
+            seconds_to_wait = 0
+            if aad_verification_code is None:
+                aad_verification_code = click.prompt(aad_verification_code_text)
+
         response = session.post(
-            roles_page_url,
+            _action_url_on_validation_success(html_response),
             verify=ssl_verification_enabled,
             allow_redirects=True,
             data={
                 'AuthMethod': 'AzureMfaAuthentication',
-                'Context': context,
+                'Context': _context(html_response),
+                'VerificationCode': aad_verification_code,
             }
         )
         trace_http_request(response)
 
         if response.status_code != 200:
             raise click.ClickException(
                 u'Issues during redirection to aws roles page. The error response {}'.format(
@@ -63,15 +66,15 @@
         html_response = ET.fromstring(response.text, ET.HTMLParser())
         element = html_response.find('.//input[@name="SAMLResponse"]')
 
         if element is not None:
             break
 
         if counter == max_attempts:
-            raise click.ClickException(u'Timeout waiting for MFA approval')
+            raise click.ClickException(u'Unsuccessful MFA verification' if aad_verification_code else u'Timeout waiting for MFA approval')
 
         counter += 1
 
     # Save session cookies to avoid having to repeat MFA on each login
     session.cookies.save(ignore_discard=True)
 
     html_response = ET.fromstring(response.text, ET.HTMLParser())
@@ -86,7 +89,17 @@
 
 
 def _action_url_on_validation_success(html_response):
     post_url_query = './/form[@id="options"]'
     element = html_response.find(post_url_query)
 
     return element.get('action')
+
+def _mfa_instructions(html_response):
+    mfa_instructions_query = './/p[@id="instructions"]'
+    element = html_response.find(mfa_instructions_query)
+    return element.text if element is not None else ''
+
+def _aad_verification_code_text(html_response):
+    aad_verification_code_query = './/input[@id="verificationCodeInput"]'
+    element = html_response.find(aad_verification_code_query)
+    return None if element is None else element.get('placeholder')
```

### Comparing `aws_adfs-2.6.3/aws_adfs/_azure_mfa_authenticator.py` & `aws_adfs-2.7.0/aws_adfs/_azure_mfa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/_duo_authenticator.py` & `aws_adfs-2.7.0/aws_adfs/_duo_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/_duo_universal_prompt_authenticator.py` & `aws_adfs-2.7.0/aws_adfs/_duo_universal_prompt_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/_rsa_authenticator.py` & `aws_adfs-2.7.0/aws_adfs/_rsa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/_symantec_vip_access.py` & `aws_adfs-2.7.0/aws_adfs/_symantec_vip_access.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/account_aliases_fetcher.py` & `aws_adfs-2.7.0/aws_adfs/account_aliases_fetcher.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/authenticator.py` & `aws_adfs-2.7.0/aws_adfs/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from . import _azure_mfa_authenticator as azure_mfa_auth
 from . import _azure_cloud_mfa_authenticator as azure_cloud_mfa_auth
 from . import html_roles_fetcher
 from . import roles_assertion_extractor
 from .helpers import trace_http_request
 
 
-def authenticate(config, username=None, password=None, assertfile=None):
+def authenticate(config, username=None, password=None, assertfile=None, aad_verification_code=None):
     response, session = html_roles_fetcher.fetch_html_encoded_roles(
         adfs_host=config.adfs_host,
         adfs_cookie_location=config.adfs_cookie_location,
         ssl_verification_enabled=config.ssl_verification,
         adfs_ca_bundle=config.adfs_ca_bundle,
         provider_id=config.provider_id,
         username=username,
@@ -116,15 +116,15 @@
     def _azure_mfa_extractor():
         def extract():
             return azure_mfa_auth.extract(html_response, config.ssl_verification, session)
         return extract
 
     def _azure_cloud_mfa_extractor():
         def extract():
-            return azure_cloud_mfa_auth.extract(html_response, config.ssl_verification, session)
+            return azure_cloud_mfa_auth.extract(html_response, config.ssl_verification, config.aad_verification_code, session)
         return extract
 
     if assertfile is None:
         chosen_strategy = _plain_extractor
     else:
         chosen_strategy = _file_extractor
```

### Comparing `aws_adfs-2.6.3/aws_adfs/commands.py` & `aws_adfs-2.7.0/aws_adfs/commands.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/helpers.py` & `aws_adfs-2.7.0/aws_adfs/helpers.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/html_roles_fetcher.py` & `aws_adfs-2.7.0/aws_adfs/html_roles_fetcher.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/list_profiles.py` & `aws_adfs-2.7.0/aws_adfs/list_profiles.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/login.py` & `aws_adfs-2.7.0/aws_adfs/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,18 @@
 @click.option(
     "--enforce-role-arn",
     help=f'Only allow the role passed in by --role-arn.',
     type=bool,
     is_flag=True,
     default=False,
 )
+@click.option(
+    "--aad-verification-code",
+    help="Verification code for Azure AD multi-factor authentication.",
+)
 def login(
     profile,
     region,
     ssl_verification,
     adfs_ca_bundle,
     adfs_host,
     output_format,
@@ -168,14 +172,15 @@
     role_arn,
     session_duration,
     no_session_cache,
     assertfile,
     sspi,
     duo_factor,
     duo_device,
+    aad_verification_code,
     enforce_role_arn,
 ):
     """
     Authenticates an user with active directory credentials
     """
     config = prepare.get_prepared_config(
         profile,
@@ -187,14 +192,15 @@
         provider_id,
         s3_signature_version,
         session_duration,
         sspi,
         username_password_command,
         duo_factor,
         duo_device,
+        aad_verification_code,
         enforce_role_arn,
     )
 
     _verification_checks(config)
 
     # Get session credentials from cache if not expired to avoid invoking the ADFS host uselessly
     session_cache_dir = (
```

### Comparing `aws_adfs-2.6.3/aws_adfs/prepare.py` & `aws_adfs-2.7.0/aws_adfs/prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     provider_id,
     s3_signature_version,
     session_duration,
     sspi,
     username_password_command,
     duo_factor,
     duo_device,
+    aad_verification_code=None,
     enforce_role_arn=False
 ):
     """
     Prepares ADFS configuration for login task.
     The task comprises steps as follows:
         - default configuration preparation,
         - creating aws cli configuration files, if needed
@@ -44,14 +45,15 @@
     :param provider_id: Provider ID, e.g urn:amazon:webservices (optional)
     :param s3_signature_version: s3 signature version
     :param session_duration: AWS STS session duration (default 1 hour)
     :param sspi: Whether SSPI is enabled
     :param username_password_command: The command used to retrieve username and password information
     :param duo_factor: The specific Duo factor to use
     :param duo_device: The specific Duo device to use
+    :param aad_verification_code: If verification code is in config use that for multi-factor authentication
     :param enforce_role_arn: If role_arn is in config then only allow the provided value
     """
     def default_if_none(value, default):
         return value if value is not None else default
 
     # Normalise duo_factor if specified and we can find a single match
     if duo_factor:
@@ -82,14 +84,15 @@
         adfs_config.s3_signature_version
     )
     adfs_config.session_duration = default_if_none(session_duration, adfs_config.session_duration)
     adfs_config.sspi = default_if_none(sspi, adfs_config.sspi)
     adfs_config.username_password_command = default_if_none(username_password_command, adfs_config.username_password_command)
     adfs_config.duo_factor = default_if_none(duo_factor, adfs_config.duo_factor)
     adfs_config.duo_device = default_if_none(duo_device, adfs_config.duo_device)
+    adfs_config.aad_verification_code = aad_verification_code
     adfs_config.enforce_role_arn = enforce_role_arn
 
     return adfs_config
 
 
 def create_adfs_default_config(profile):
     config = type('', (), {})()
```

### Comparing `aws_adfs-2.6.3/aws_adfs/reset.py` & `aws_adfs-2.7.0/aws_adfs/reset.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/role_chooser.py` & `aws_adfs-2.7.0/aws_adfs/role_chooser.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/aws_adfs/roles_assertion_extractor.py` & `aws_adfs-2.7.0/aws_adfs/roles_assertion_extractor.py`

 * *Files identical despite different names*

### Comparing `aws_adfs-2.6.3/pyproject.toml` & `aws_adfs-2.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "aws-adfs"
-version = "2.6.3"
+version = "2.7.0"
 description = "AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role"
 keywords = ["aws", "adfs", "console", "tool"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
@@ -39,16 +39,16 @@
     { version = "^0.14", markers = "platform_system != 'Windows'" },
 ]
 requests-negotiate-sspi = [
     { version = "^0.5", markers = "platform_system == 'Windows'" },
 ]
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10"
-coverage = "^6.5"
+black = ">=22.12,<24.0"
+coverage = ">=6.5,<8.0"
 pre-commit = "^2.20.0"
 pytest = "^7.2"
 toml = "^0.10"
 
 [tool.black]
 line-length = 130          # black's default is 88
 target-version = ['py310']
```

### Comparing `aws_adfs-2.6.3/setup.py` & `aws_adfs-2.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  ':platform_system == "Windows"': ['requests-negotiate-sspi>=0.5,<0.6']}
 
 entry_points = \
 {'console_scripts': ['aws-adfs = aws_adfs.commands:cli']}
 
 setup_kwargs = {
     'name': 'aws-adfs',
-    'version': '2.6.3',
+    'version': '2.7.0',
     'description': 'AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role',
-    'long_description': '# aws-adfs\n[![PyPI version](https://badge.fury.io/py/aws-adfs.svg)](https://badge.fury.io/py/aws-adfs)\n[![Travis build](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)\n![Build Status](https://github.com/venth/aws-adfs/workflows/Build/badge.svg?branch=master)\n\nThe project provides command line tool - `aws-adfs` to ease AWS cli authentication against ADFS (multi factor authentication with active directory).\n\n## `aws-adfs` command line tool\n\n* allows you to re-login to STS without entering credentials for an extended period of time, without having to store the user\'s actual credentials. It also lets an organization control the period in which a user can re-login to STS without entering credentials, by altering the ADFS session lifetime.\n\n* supports automation tools like ansible by providing security token in `AWS_SESSION_TOKEN`/`AWS_SECURITY_TOKEN` environment variables.\n\n* supports using Security Support Provider Interface (SSPI) on Windows OS.\n\n### MFA integration\n\naws-adfs integrates with:\n* [duo security](https://duo.com) MFA provider with support for:\n  * Duo mobile application push (verified by code or not) using the `Duo Push` authentication method.\n  * Phone call using the `Phone Call` authentication method.\n  * OTP 6 digit codes generated by Duo Mobile application, and hardware tokens (e.g. RSA or Yubikey) using the `Passcode` authentication method.\n  * FIDO U2F (CTAP1) / FIDO2 (CTAP2) hardware authenticators using the `WebAuthn Security Key` authentication method.\n* [Symantec VIP](https://vip.symantec.com/) MFA provider\n* [RSA SecurID](https://www.rsa.com/) MFA provider\n\n## Setup Dependencies\n\n- `build-essential` (provides C/C++ compilers)\n- `python3` `>= 3.7 <4.0`\n- `python3-dev`\n- `libkrb5-dev`\n- `libxml2-dev`\n\n## Installation\n\n* user local installation with [pipx](https://github.com/pypa/pipx)\n\n    ```\n    pipx install aws-adfs\n    ```\n\n* user local installation with pip\n\n    ```\n    pip3 install --user aws-adfs\n    ```\n\n    Please note, that you need to add $HOME/.local/bin to your PATH\n\n* system wide installation\n\n    ```\n    sudo pip3 install aws-adfs\n    ```\n\n* virtualenvs\n\n    ```\n    virtualenv aws-adfs\n    source aws-adfs/bin/activate\n    pip install aws-adfs\n    ...\n    ...\n    deactivate\n    ```\n\n* Windows 10\n\n   - Install latest supported Visual C++ downloads from Microsoft for Visual Studio 2015, 2017 and 2019:\n      - https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads\n      - https://aka.ms/vs/16/release/vc_redist.x64.exe\n    - Install Python 3.7 from Microsoft Store:\n      - https://www.microsoft.com/en-us/p/python-37/9nj46sx7x90p\n    - Start PowerShell as Administrator\n    - Go to `C:\\Program Files`:\n        ```\n        C:\n        cd \'C:\\Program Files\\\'\n        ```\n    - Create virtual env:\n      ```\n      python3 -m venv aws-adfs\n      ```\n    - Install `aws-adfs`:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\pip\' install aws-adfs\n      ```\n    - Run it:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\aws-adfs\' login --adfs-host=your-adfs-hostname\n      ```\n\n## Examples of usage\n\n### `aws-adfs`\n* login to your adfs host with disabled ssl verification on aws cli profile: adfs\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=adfs s3 ls\n    ```\n\n* login to your adfs host with disabled ssl verification on specified aws cli profile: specified-profile\n\n    ```\n    aws-adfs login --profile=specified-profile --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=specified-profile s3 ls\n    ```\n\n* login to your adfs host and fetch roles for AWS GovCloud (US)\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --provider-id urn:amazon:webservices:govcloud --region us-gov-west-1\n    ```\n\n    and verification\n\n    ```\n    aws s3 ls\n    ```\n\n* login to your adfs host within ansible playbook\n\n    ```\n    ---\n    - name: "Auth sts aws"\n      command: "aws-adfs login --adfs-host sts.example.com --env --stdout --role-arn arn:aws:iam::000123456789:role/ADMIN"\n      register: sts_result\n      environment:\n        - username: "{{ ansible_user }}@example.com"\n        - password: "{{ ansible_ssh_pass }}"\n\n    - name: "Set sts facts"\n      set_fact:\n        sts: "{{ sts_result.stdout | from_json }}"\n\n    - name: "List s3 Buckets"\n      aws_s3_bucket_facts:\n        aws_access_key: "{{\xa0sts.AccessKeyId }}"\n        aws_secret_key: "{{\xa0sts.SecretAccessKey }}"\n        security_token: "{{\xa0sts.SessionToken }}"\n        region: "us-east-1"\n      register: buckets\n\n    - name: "Print Buckets"\n      debug:\n        var: buckets\n    ```\n\n* login to your adfs host by passing username and password credentials via a file\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --authfile=/path/and/file/name\n    ```\n\n    Auth file should be in format of\n\n    ```\n    [profile_name]\n    username = your_username\n    password = your_password\n    ```\n\n* .aws/config profile for automatically refreshing credentials\n    ```\n    [profile example-role-ue1]\n    credential_process=aws-adfs login --region=us-east-1 --role-arn=arn:aws:iam::1234567891234:role/example-role --adfs-host=adfs.example.com --stdout\n    ```\n    Warning: see [AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html) about security considerations to take when sourcing credentials with an external process.\n\n* help, help, help?\n    <!-- AWS_HELP_START -->\n    ```\n    $ aws-adfs --help\n    Usage: aws-adfs [OPTIONS] COMMAND [ARGS]...\n\n    Options:\n      --version      Show current tool version\n      -v, --verbose  Enables debug information on stdout. By default log level is\n                     set on ERROR\n      --help         Show this message and exit.\n\n    Commands:\n      list   lists available profiles\n      login  Authenticates an user with active directory credentials\n      reset  removes stored profile\n    ```\n    <!-- AWS_HELP_END -->\n\n    <!-- AWS_LIST_HELP_START -->\n    ```\n    $ aws-adfs list --help\n    Usage: aws-adfs list [OPTIONS]\n\n      lists available profiles\n\n    Options:\n      --help  Show this message and exit.\n    ```\n    <!-- AWS_LIST_HELP_END -->\n\n    <!-- AWS_LOGIN_HELP_START -->\n    ```\n    $ aws-adfs login --help\n    Usage: aws-adfs login [OPTIONS]\n\n      Authenticates an user with active directory credentials\n\n    Options:\n      --profile TEXT                  AWS cli profile that will be authenticated.\n                                      After successful authentication just use:\n                                      aws --profile <authenticated profile>\n                                      <service> ...\n      --region TEXT                   The default AWS region that this script will\n                                      connect to for all API calls\n      --ssl-verification / --no-ssl-verification\n                                      SSL certificate verification: Whether or not\n                                      strict certificate verification is done,\n                                      False should only be used for dev/test\n      --adfs-ca-bundle TEXT           Override CA bundle for SSL certificate\n                                      verification for ADFS server only.\n      --adfs-host TEXT                For the first time for a profile it has to\n                                      be provided, next time for the same profile\n                                      it will be loaded from the stored\n                                      configuration\n      --output-format [json|text|table]\n                                      Output format used by aws cli\n      --provider-id TEXT              Provider ID, e.g urn:amazon:webservices\n                                      (optional)\n      --s3-signature-version [s3v4]   s3 signature version: Identifies the version\n                                      of AWS Signature to support for\n                                      authenticated requests. Valid values: s3v4\n      --username-password-command TEXT\n                                      Read username and password from the output\n                                      of a shell command (expected JSON format:\n                                      `{"username": "myusername", "password":\n                                      "mypassword"}`)\n      --env                           Read username, password from environment\n                                      variables (username and password).\n      --stdin                         Read username, password from standard input\n                                      separated by a newline.\n      --authfile TEXT                 Read username, password from a local file\n                                      (optional)\n      --stdout                        Print aws_session_token in json on stdout.\n      --printenv                      Output commands to set AWS_ACCESS_KEY_ID,\n                                      AWS_SECRET_ACCESS_KEY, AWS_SESSION_TOKEN,\n                                      AWS_DEFAULT_REGION environmental variables\n                                      instead of saving them to the aws\n                                      configuration file.\n      --print-console-signin-url      Output a URL that lets users who sign in to\n                                      your organization\'s network securely access\n                                      the AWS Management Console.\n      --console-role-arn TEXT         Role to assume for use in conjunction with\n                                      --print-console-signin-url\n      --console-external-id TEXT      External ID to pass in assume role for use\n                                      in conjunction with --print-console-signin-\n                                      url\n      --role-arn TEXT                 Predefined role arn to selects, e.g. aws-\n                                      adfs login --role-arn arn:aws:iam::123456789\n                                      012:role/YourSpecialRole\n      --session-duration INTEGER      Define the amount of seconds you want to\n                                      establish your STS session, e.g. aws-adfs\n                                      login --session-duration 3600\n      --no-session-cache              Do not use AWS session cache in\n                                      ~/.aws/adfs_cache/ directory.\n      --assertfile TEXT               Use SAML assertion response from a local\n                                      file\n      --sspi / --no-sspi              Whether or not to use Kerberos SSO\n                                      authentication via SSPI (Windows only,\n                                      defaults to True).\n      --duo-factor TEXT               Use a specific Duo factor, overriding the\n                                      default one configured server side. Known\n                                      Duo factors that can be used with aws-adfs\n                                      are "Duo Push", "Passcode", "Phone Call" and\n                                      "WebAuthn Security Key".\n      --duo-device TEXT               Use a specific Duo device, overriding the\n                                      default one configured server side. Depends\n                                      heavily on the Duo factor used. Known Duo\n                                      devices that can be used with aws-adfs are\n                                      "phone1" for "Duo Push" and "Phone Call"\n                                      factors. For "Passcode" and "WebAuthn\n                                      Security Key" factors, it is always "None".\n      --enforce-role-arn              Only allow the role passed in by --role-arn.\n      --help                          Show this message and exit.\n    ```\n    <!-- AWS_LOGIN_HELP_END -->\n\n    <!-- AWS_RESET_HELP_START -->\n    ```\n    $ aws-adfs reset --help\n    Usage: aws-adfs reset [OPTIONS]\n\n      removes stored profile\n\n    Options:\n      --profile TEXT  AWS cli profile that will be removed\n      --help          Show this message and exit.\n    ```\n    <!-- AWS_RESET_HELP_END -->\n\n## Known issues\n\n* duo-security\n\n    `Error: Cannot begin authentication process. The error response: {"message": "Unknown authentication method.", "stat": "FAIL"}`\n\n    Please setup preferred auth method in duo-security settings (settings\' -> \'My Settings & Devices\').\n\n* USB FIDO2 does not work in Windows Subsystem for Linux (WSL)\n\n    `OSError: [Errno 2] No such file or directory: \'/sys/class/hidraw\'`\n\n    USB devices are not accessible in WSL, please install and run `aws-adfs` on the Windows 10 host and then access the credentials in WSL from the filesystem. Example:\n\n    ```\n    export AWS_CONFIG_FILE=/mnt/c/Users/username/.aws/config\n    export AWS_SHARED_CREDENTIALS_FILE=/mnt/c/Users/username/.aws/credentials\n    ```\n\n*  FIDO2 devices are not detected on Windows 10 build 1903 or newer\n\n    Running `aws-adfs` as Administrator is required since Windows 10 build 1903 to access FIDO2 devices, cf. https://github.com/Yubico/python-fido2/issues/55)\n\n* in cases of trouble with lxml please install\n\n  ```\n  sudo apt-get install python3-dev libxml2-dev libxslt1-dev zlib1g-dev\n  ```\n\n* in cases of trouble with pykerberos please install\n\n  ```\n  sudo apt-get install python3-dev libkrb5-dev\n  ```\n\n* in cases of trouble with OSX Sierra (obsolete OpenSSL), upgrade OpenSSL. Example:\n  ```\n  brew upgrade openssl\n  ```\n  AND add explicit directive to .bash_profile:\n  ```\n  export PATH=$(brew --prefix openssl)/bin:$PATH\n  ```\n\n* only python >= 3.7 to <4.0 are supported:\n  - python 2.6 is not supported\n  - python 2.7 is not supported\n  - python 3.2 is not supported\n  - python 3.3 is not supported\n  - python 3.4 is not supported\n  - python 3.5 is not supported\n  - python 3.6 is not supported\n\n## Development\n\n* update dependencies:\n```\npoetry update\n```\n\n* run unit tests:\n```\npoetry run pytest\n```\n\n* release:\n\n```\nexport CHANGELOG_GITHUB_TOKEN=$(gopass show -o pins/Github/github-changelog-generator)\n./script/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string\n```\n\n## Changelog\n\nSee the [CHANGELOG.md](CHANGELOG.md) file, which is generated using [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator).\n',
+    'long_description': '# aws-adfs\n[![PyPI version](https://badge.fury.io/py/aws-adfs.svg)](https://badge.fury.io/py/aws-adfs)\n[![Travis build](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)](https://api.travis-ci.org/venth/aws-adfs.svg?branch=master)\n![Build Status](https://github.com/venth/aws-adfs/workflows/Build/badge.svg?branch=master)\n\nThe project provides command line tool - `aws-adfs` to ease AWS cli authentication against ADFS (multi factor authentication with active directory).\n\n## `aws-adfs` command line tool\n\n* allows you to re-login to STS without entering credentials for an extended period of time, without having to store the user\'s actual credentials. It also lets an organization control the period in which a user can re-login to STS without entering credentials, by altering the ADFS session lifetime.\n\n* supports automation tools like ansible by providing security token in `AWS_SESSION_TOKEN`/`AWS_SECURITY_TOKEN` environment variables.\n\n* supports using Security Support Provider Interface (SSPI) on Windows OS.\n\n### MFA integration\n\naws-adfs integrates with:\n* [duo security](https://duo.com) MFA provider with support for:\n  * Duo mobile application push (verified by code or not) using the `Duo Push` authentication method.\n  * Phone call using the `Phone Call` authentication method.\n  * OTP 6 digit codes generated by Duo Mobile application, and hardware tokens (e.g. RSA or Yubikey) using the `Passcode` authentication method.\n  * FIDO U2F (CTAP1) / FIDO2 (CTAP2) hardware authenticators using the `WebAuthn Security Key` authentication method.\n* [Symantec VIP](https://vip.symantec.com/) MFA provider\n* [RSA SecurID](https://www.rsa.com/) MFA provider\n* [Azure AD MFA](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) with support for:\n  * Microsoft Authenticator app\n  * OTP 6 digit codes\n  * SMS codes\n  * Phone call\n\n## Setup Dependencies\n\n- `build-essential` (provides C/C++ compilers)\n- `python3` `>= 3.7 <4.0`\n- `python3-dev`\n- `libkrb5-dev`\n- `libxml2-dev`\n\n## Installation\n\n* user local installation with [pipx](https://github.com/pypa/pipx)\n\n    ```\n    pipx install aws-adfs\n    ```\n\n* user local installation with pip\n\n    ```\n    pip3 install --user aws-adfs\n    ```\n\n    Please note, that you need to add $HOME/.local/bin to your PATH\n\n* system wide installation\n\n    ```\n    sudo pip3 install aws-adfs\n    ```\n\n* virtualenvs\n\n    ```\n    virtualenv aws-adfs\n    source aws-adfs/bin/activate\n    pip install aws-adfs\n    ...\n    ...\n    deactivate\n    ```\n\n* Windows 10\n\n   - Install latest supported Visual C++ downloads from Microsoft for Visual Studio 2015, 2017 and 2019:\n      - https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads\n      - https://aka.ms/vs/16/release/vc_redist.x64.exe\n    - Install Python 3.7 from Microsoft Store:\n      - https://www.microsoft.com/en-us/p/python-37/9nj46sx7x90p\n    - Start PowerShell as Administrator\n    - Go to `C:\\Program Files`:\n        ```\n        C:\n        cd \'C:\\Program Files\\\'\n        ```\n    - Create virtual env:\n      ```\n      python3 -m venv aws-adfs\n      ```\n    - Install `aws-adfs`:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\pip\' install aws-adfs\n      ```\n    - Run it:\n      ```\n      & \'C:\\Program Files\\aws-adfs\\Scripts\\aws-adfs\' login --adfs-host=your-adfs-hostname\n      ```\n\n## Examples of usage\n\n### `aws-adfs`\n* login to your adfs host with disabled ssl verification on aws cli profile: adfs\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=adfs s3 ls\n    ```\n\n* login to your adfs host with disabled ssl verification on specified aws cli profile: specified-profile\n\n    ```\n    aws-adfs login --profile=specified-profile --adfs-host=your-adfs-hostname --no-ssl-verification\n    ```\n\n    and verification\n\n    ```\n    aws --profile=specified-profile s3 ls\n    ```\n\n* login to your adfs host and fetch roles for AWS GovCloud (US)\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --provider-id urn:amazon:webservices:govcloud --region us-gov-west-1\n    ```\n\n    and verification\n\n    ```\n    aws s3 ls\n    ```\n\n* login to your adfs host within ansible playbook\n\n    ```\n    ---\n    - name: "Auth sts aws"\n      command: "aws-adfs login --adfs-host sts.example.com --env --stdout --role-arn arn:aws:iam::000123456789:role/ADMIN"\n      register: sts_result\n      environment:\n        - username: "{{ ansible_user }}@example.com"\n        - password: "{{ ansible_ssh_pass }}"\n\n    - name: "Set sts facts"\n      set_fact:\n        sts: "{{ sts_result.stdout | from_json }}"\n\n    - name: "List s3 Buckets"\n      aws_s3_bucket_facts:\n        aws_access_key: "{{\xa0sts.AccessKeyId }}"\n        aws_secret_key: "{{\xa0sts.SecretAccessKey }}"\n        security_token: "{{\xa0sts.SessionToken }}"\n        region: "us-east-1"\n      register: buckets\n\n    - name: "Print Buckets"\n      debug:\n        var: buckets\n    ```\n\n* login to your adfs host by passing username and password credentials via a file\n\n    ```\n    aws-adfs login --adfs-host=your-adfs-hostname --authfile=/path/and/file/name\n    ```\n\n    Auth file should be in format of\n\n    ```\n    [profile_name]\n    username = your_username\n    password = your_password\n    ```\n\n* .aws/config profile for automatically refreshing credentials\n    ```\n    [profile example-role-ue1]\n    credential_process=aws-adfs login --region=us-east-1 --role-arn=arn:aws:iam::1234567891234:role/example-role --adfs-host=adfs.example.com --stdout\n    ```\n    Warning: see [AWS documentation](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-sourcing-external.html) about security considerations to take when sourcing credentials with an external process.\n\n* help, help, help?\n    <!-- AWS_HELP_START -->\n    ```\n    $ aws-adfs --help\n    Usage: aws-adfs [OPTIONS] COMMAND [ARGS]...\n\n    Options:\n      --version      Show current tool version\n      -v, --verbose  Enables debug information on stdout. By default log level is\n                     set on ERROR\n      --help         Show this message and exit.\n\n    Commands:\n      list   lists available profiles\n      login  Authenticates an user with active directory credentials\n      reset  removes stored profile\n    ```\n    <!-- AWS_HELP_END -->\n\n    <!-- AWS_LIST_HELP_START -->\n    ```\n    $ aws-adfs list --help\n    Usage: aws-adfs list [OPTIONS]\n\n      lists available profiles\n\n    Options:\n      --help  Show this message and exit.\n    ```\n    <!-- AWS_LIST_HELP_END -->\n\n    <!-- AWS_LOGIN_HELP_START -->\n    ```\n    $ aws-adfs login --help\n    Usage: aws-adfs login [OPTIONS]\n\n      Authenticates an user with active directory credentials\n\n    Options:\n      --profile TEXT                  AWS cli profile that will be authenticated.\n                                      After successful authentication just use:\n                                      aws --profile <authenticated profile>\n                                      <service> ...\n      --region TEXT                   The default AWS region that this script will\n                                      connect to for all API calls\n      --ssl-verification / --no-ssl-verification\n                                      SSL certificate verification: Whether or not\n                                      strict certificate verification is done,\n                                      False should only be used for dev/test\n      --adfs-ca-bundle TEXT           Override CA bundle for SSL certificate\n                                      verification for ADFS server only.\n      --adfs-host TEXT                For the first time for a profile it has to\n                                      be provided, next time for the same profile\n                                      it will be loaded from the stored\n                                      configuration\n      --output-format [json|text|table]\n                                      Output format used by aws cli\n      --provider-id TEXT              Provider ID, e.g urn:amazon:webservices\n                                      (optional)\n      --s3-signature-version [s3v4]   s3 signature version: Identifies the version\n                                      of AWS Signature to support for\n                                      authenticated requests. Valid values: s3v4\n      --username-password-command TEXT\n                                      Read username and password from the output\n                                      of a shell command (expected JSON format:\n                                      `{"username": "myusername", "password":\n                                      "mypassword"}`)\n      --env                           Read username, password from environment\n                                      variables (username and password).\n      --stdin                         Read username, password from standard input\n                                      separated by a newline.\n      --authfile TEXT                 Read username, password from a local file\n                                      (optional)\n      --stdout                        Print aws_session_token in json on stdout.\n      --printenv                      Output commands to set AWS_ACCESS_KEY_ID,\n                                      AWS_SECRET_ACCESS_KEY, AWS_SESSION_TOKEN,\n                                      AWS_DEFAULT_REGION environmental variables\n                                      instead of saving them to the aws\n                                      configuration file.\n      --print-console-signin-url      Output a URL that lets users who sign in to\n                                      your organization\'s network securely access\n                                      the AWS Management Console.\n      --console-role-arn TEXT         Role to assume for use in conjunction with\n                                      --print-console-signin-url\n      --console-external-id TEXT      External ID to pass in assume role for use\n                                      in conjunction with --print-console-signin-\n                                      url\n      --role-arn TEXT                 Predefined role arn to selects, e.g. aws-\n                                      adfs login --role-arn arn:aws:iam::123456789\n                                      012:role/YourSpecialRole\n      --session-duration INTEGER      Define the amount of seconds you want to\n                                      establish your STS session, e.g. aws-adfs\n                                      login --session-duration 3600\n      --no-session-cache              Do not use AWS session cache in\n                                      ~/.aws/adfs_cache/ directory.\n      --assertfile TEXT               Use SAML assertion response from a local\n                                      file\n      --sspi / --no-sspi              Whether or not to use Kerberos SSO\n                                      authentication via SSPI (Windows only,\n                                      defaults to True).\n      --duo-factor TEXT               Use a specific Duo factor, overriding the\n                                      default one configured server side. Known\n                                      Duo factors that can be used with aws-adfs\n                                      are "Duo Push", "Passcode", "Phone Call" and\n                                      "WebAuthn Security Key".\n      --duo-device TEXT               Use a specific Duo device, overriding the\n                                      default one configured server side. Depends\n                                      heavily on the Duo factor used. Known Duo\n                                      devices that can be used with aws-adfs are\n                                      "phone1" for "Duo Push" and "Phone Call"\n                                      factors. For "Passcode" and "WebAuthn\n                                      Security Key" factors, it is always "None".\n      --enforce-role-arn              Only allow the role passed in by --role-arn.\n      --aad-verification-code TEXT    Verification code for Azure AD multi-factor\n                                      authentication.\n      --help                          Show this message and exit.\n    ```\n    <!-- AWS_LOGIN_HELP_END -->\n\n    <!-- AWS_RESET_HELP_START -->\n    ```\n    $ aws-adfs reset --help\n    Usage: aws-adfs reset [OPTIONS]\n\n      removes stored profile\n\n    Options:\n      --profile TEXT  AWS cli profile that will be removed\n      --help          Show this message and exit.\n    ```\n    <!-- AWS_RESET_HELP_END -->\n\n## Known issues\n\n* duo-security\n\n    `Error: Cannot begin authentication process. The error response: {"message": "Unknown authentication method.", "stat": "FAIL"}`\n\n    Please setup preferred auth method in duo-security settings (settings\' -> \'My Settings & Devices\').\n\n* USB FIDO2 does not work in Windows Subsystem for Linux (WSL)\n\n    `OSError: [Errno 2] No such file or directory: \'/sys/class/hidraw\'`\n\n    USB devices are not accessible in WSL, please install and run `aws-adfs` on the Windows 10 host and then access the credentials in WSL from the filesystem. Example:\n\n    ```\n    export AWS_CONFIG_FILE=/mnt/c/Users/username/.aws/config\n    export AWS_SHARED_CREDENTIALS_FILE=/mnt/c/Users/username/.aws/credentials\n    ```\n\n*  FIDO2 devices are not detected on Windows 10 build 1903 or newer\n\n    Running `aws-adfs` as Administrator is required since Windows 10 build 1903 to access FIDO2 devices, cf. https://github.com/Yubico/python-fido2/issues/55)\n\n* in cases of trouble with lxml please install\n\n  ```\n  sudo apt-get install python3-dev libxml2-dev libxslt1-dev zlib1g-dev\n  ```\n\n* in cases of trouble with pykerberos please install\n\n  ```\n  sudo apt-get install python3-dev libkrb5-dev\n  ```\n\n* in cases of trouble with OSX Sierra (obsolete OpenSSL), upgrade OpenSSL. Example:\n  ```\n  brew upgrade openssl\n  ```\n  AND add explicit directive to .bash_profile:\n  ```\n  export PATH=$(brew --prefix openssl)/bin:$PATH\n  ```\n\n* only python >= 3.7 to <4.0 are supported:\n  - python 2.6 is not supported\n  - python 2.7 is not supported\n  - python 3.2 is not supported\n  - python 3.3 is not supported\n  - python 3.4 is not supported\n  - python 3.5 is not supported\n  - python 3.6 is not supported\n\n## Development\n\n* update dependencies:\n```\npoetry update\n```\n\n* run unit tests:\n```\npoetry run pytest\n```\n\n* release:\n\n```\nexport CHANGELOG_GITHUB_TOKEN=$(gopass show -o pins/Github/github-changelog-generator)\n./script/release.sh patch # or minor, major, prepatch, preminor, premajor, prerelease, or a valid semver string\n```\n\n## Changelog\n\nSee the [CHANGELOG.md](CHANGELOG.md) file, which is generated using [github-changelog-generator](https://github.com/github-changelog-generator/github-changelog-generator).\n',
     'author': 'Venth',
     'author_email': 'artur.krysiak.warszawa@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aws_adfs-2.6.3/PKG-INFO` & `aws_adfs-2.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-adfs
-Version: 2.6.3
+Version: 2.7.0
 Summary: AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role
 Keywords: aws,adfs,console,tool
 Author: Venth
 Author-email: artur.krysiak.warszawa@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -54,14 +54,19 @@
 * [duo security](https://duo.com) MFA provider with support for:
   * Duo mobile application push (verified by code or not) using the `Duo Push` authentication method.
   * Phone call using the `Phone Call` authentication method.
   * OTP 6 digit codes generated by Duo Mobile application, and hardware tokens (e.g. RSA or Yubikey) using the `Passcode` authentication method.
   * FIDO U2F (CTAP1) / FIDO2 (CTAP2) hardware authenticators using the `WebAuthn Security Key` authentication method.
 * [Symantec VIP](https://vip.symantec.com/) MFA provider
 * [RSA SecurID](https://www.rsa.com/) MFA provider
+* [Azure AD MFA](https://learn.microsoft.com/en-us/azure/active-directory/authentication/concept-mfa-howitworks) with support for:
+  * Microsoft Authenticator app
+  * OTP 6 digit codes
+  * SMS codes
+  * Phone call
 
 ## Setup Dependencies
 
 - `build-essential` (provides C/C++ compilers)
 - `python3` `>= 3.7 <4.0`
 - `python3-dev`
 - `libkrb5-dev`
@@ -323,14 +328,16 @@
                                       default one configured server side. Depends
                                       heavily on the Duo factor used. Known Duo
                                       devices that can be used with aws-adfs are
                                       "phone1" for "Duo Push" and "Phone Call"
                                       factors. For "Passcode" and "WebAuthn
                                       Security Key" factors, it is always "None".
       --enforce-role-arn              Only allow the role passed in by --role-arn.
+      --aad-verification-code TEXT    Verification code for Azure AD multi-factor
+                                      authentication.
       --help                          Show this message and exit.
     ```
     <!-- AWS_LOGIN_HELP_END -->
 
     <!-- AWS_RESET_HELP_START -->
     ```
     $ aws-adfs reset --help
```

