# Comparing `tmp/decentro-in-kyc-python-sdk-4.3.0.tar.gz` & `tmp/decentro_in_kyc_python_sdk-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dylanhuang/Git/konfig-monorepo/customers/decentro/decentro-in-kyc-sdk/python/dist/.tmp-s414k7q0/decentro-in-kyc-python-s", last modified: Thu Apr 20 19:33:43 2023, max compression
+gzip compressed data, was "decentro_in_kyc_python_sdk-4.4.0.tar", max compression
```

## Comparing `decentro-in-kyc-python-sdk-4.3.0.tar` & `decentro_in_kyc_python_sdk-4.4.0.tar`

### file list

```diff
@@ -1,150 +1,133 @@
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1081 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/LICENSE
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6426 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6122 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/README.md
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      824 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    63552 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/api_client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      266 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/api_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      214 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2245 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/path_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      249 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      149 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/kyc_public_registry_validate.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      133 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/kyc_scan_extract_ocr.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      153 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_document_classification.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      146 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_face_match.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      152 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_image_quality.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      156 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_photocopy_check.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      154 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_video_liveness.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      159 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/paths/v2_kyc_identities_mask_aadhaar_uid.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      312 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tag_to_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      311 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1147 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/kyc_api.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      714 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/client.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    18943 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/configuration.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5669 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2274 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions_base.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      356 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3998 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5719 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    39305 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3992 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5065 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7404 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     4000 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5268 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7412 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3996 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5964 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7772 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8727 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8049 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    14321 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     5059 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3992 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8531 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3982 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6934 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     7329 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     8177 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6692 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)   270536 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     2538 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/models/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      850 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      359 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    20468 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      343 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17351 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      363 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17460 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      357 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17299 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      363 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    21753 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      367 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    17414 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      365 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13262 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/
--rw-r--r--   0 dylanhuang   (501) staff       (20)      371 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    13165 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      673 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_after_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      674 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_before_hook.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    10705 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/rest.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)    95007 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/schemas.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)     3178 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/validation_metadata.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6426 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dylanhuang   (501) staff       (20)     6442 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)        1 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)      139 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/requires.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       28 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 dylanhuang   (501) staff       (20)       69 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/setup.cfg
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1286 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/setup.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/
--rw-r--r--   0 dylanhuang   (501) staff       (20)    19452 2023-04-20 19:07:01.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_kyc_api.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      559 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      543 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_image_quality_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      546 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      530 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      534 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      563 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      551 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_video_liveness_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      554 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      538 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      542 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      534 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      518 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      522 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_extract_text_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      518 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      547 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_uid400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      535 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_mask_aadhaar_uid_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      526 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      510 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      514 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_match_face_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      521 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate400_response.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      505 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate_request.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      509 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_validate_response.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/
--rw-r--r--   0 dylanhuang   (501) staff       (20)     1984 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/__init__.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      760 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_public_registry_validate/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      740 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_kyc_scan_extract_ocr/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      773 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_document_classification/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      755 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_face_match/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      773 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_image_quality/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      775 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_photocopy_check/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      771 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_forensics_video_liveness/test_post.py
-drwxr-xr-x   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:33:43.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/
--rw-r--r--   0 dylanhuang   (501) staff       (20)        0 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/__init__.py
--rw-r--r--   0 dylanhuang   (501) staff       (20)      779 2023-04-20 19:08:21.000000 decentro-in-kyc-python-sdk-4.3.0/test/test_paths/test_v2_kyc_identities_mask_aadhaar_uid/test_post.py
+-rw-r--r--   0        0        0     1081 2023-05-09 01:36:39.857809 decentro_in_kyc_python_sdk-4.4.0/LICENSE
+-rw-r--r--   0        0        0     5325 2023-05-09 01:36:39.903619 decentro_in_kyc_python_sdk-4.4.0/README.md
+-rw-r--r--   0        0        0      824 2023-05-09 01:36:39.820214 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/__init__.py
+-rw-r--r--   0        0        0    72692 2023-05-09 01:36:39.820553 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/api_client.py
+-rw-r--r--   0        0        0      663 2023-05-09 01:36:39.820788 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/api_response.py
+-rw-r--r--   0        0        0      214 2023-05-09 01:36:39.820934 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/__init__.py
+-rw-r--r--   0        0        0     2245 2023-05-09 01:36:39.821050 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/path_to_api.py
+-rw-r--r--   0        0        0      249 2023-05-09 01:36:39.821200 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-09 01:36:39.821683 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/kyc_public_registry_validate.py
+-rw-r--r--   0        0        0      133 2023-05-09 01:36:39.821842 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/kyc_scan_extract_ocr.py
+-rw-r--r--   0        0        0      153 2023-05-09 01:36:39.821985 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/v2_kyc_document_classification.py
+-rw-r--r--   0        0        0      146 2023-05-09 01:36:39.822121 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_face_match.py
+-rw-r--r--   0        0        0      152 2023-05-09 01:36:39.822245 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_image_quality.py
+-rw-r--r--   0        0        0      156 2023-05-09 01:36:39.822384 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_photocopy_check.py
+-rw-r--r--   0        0        0      154 2023-05-09 01:36:39.822529 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/v2_kyc_forensics_video_liveness.py
+-rw-r--r--   0        0        0      159 2023-05-09 01:36:39.822671 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/paths/v2_kyc_identities_mask_aadhaar_uid.py
+-rw-r--r--   0        0        0      312 2023-05-09 01:36:39.822806 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/tag_to_api.py
+-rw-r--r--   0        0        0      311 2023-05-09 01:36:39.822899 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/tags/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-09 01:36:39.822981 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/tags/kyc_api.py
+-rw-r--r--   0        0        0      986 2023-05-09 01:36:39.823222 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/client.py
+-rw-r--r--   0        0        0      986 2023-05-09 01:36:39.823312 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/client.pyi
+-rw-r--r--   0        0        0      711 2023-05-09 01:36:39.823448 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/client_custom.py
+-rw-r--r--   0        0        0    18935 2023-05-09 01:36:39.823651 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/configuration.py
+-rw-r--r--   0        0        0     7129 2023-05-09 01:36:39.823849 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/exceptions.py
+-rw-r--r--   0        0        0     2274 2023-05-09 01:36:39.824015 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/exceptions_base.py
+-rw-r--r--   0        0        0      356 2023-05-09 01:36:39.824233 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/__init__.py
+-rw-r--r--   0        0        0     3998 2023-05-09 01:36:39.824405 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality400_response.py
+-rw-r--r--   0        0        0     3998 2023-05-09 01:36:39.824590 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality400_response.pyi
+-rw-r--r--   0        0        0     5719 2023-05-09 01:36:39.824763 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality_request.py
+-rw-r--r--   0        0        0     5491 2023-05-09 01:36:39.824939 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality_request.pyi
+-rw-r--r--   0        0        0    39305 2023-05-09 01:36:39.825209 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality_response.py
+-rw-r--r--   0        0        0    39305 2023-05-09 01:36:39.825541 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality_response.pyi
+-rw-r--r--   0        0        0     3992 2023-05-09 01:36:39.825761 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy400_response.py
+-rw-r--r--   0        0        0     3992 2023-05-09 01:36:39.825940 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy400_response.pyi
+-rw-r--r--   0        0        0     5065 2023-05-09 01:36:39.826103 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy_request.py
+-rw-r--r--   0        0        0     4837 2023-05-09 01:36:39.826261 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy_request.pyi
+-rw-r--r--   0        0        0     7404 2023-05-09 01:36:39.826430 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy_response.py
+-rw-r--r--   0        0        0     7404 2023-05-09 01:36:39.826604 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy_response.pyi
+-rw-r--r--   0        0        0     4000 2023-05-09 01:36:39.826765 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness400_response.py
+-rw-r--r--   0        0        0     4000 2023-05-09 01:36:39.826948 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness400_response.pyi
+-rw-r--r--   0        0        0     5268 2023-05-09 01:36:39.827114 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness_request.py
+-rw-r--r--   0        0        0     4926 2023-05-09 01:36:39.827348 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness_request.pyi
+-rw-r--r--   0        0        0     7412 2023-05-09 01:36:39.827508 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness_response.py
+-rw-r--r--   0        0        0     7412 2023-05-09 01:36:39.827633 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness_response.pyi
+-rw-r--r--   0        0        0     3996 2023-05-09 01:36:39.827749 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document400_response.py
+-rw-r--r--   0        0        0     3996 2023-05-09 01:36:39.827884 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document400_response.pyi
+-rw-r--r--   0        0        0     5964 2023-05-09 01:36:39.828084 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document_request.py
+-rw-r--r--   0        0        0     5622 2023-05-09 01:36:39.828232 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document_request.pyi
+-rw-r--r--   0        0        0     7772 2023-05-09 01:36:39.828355 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document_response.py
+-rw-r--r--   0        0        0     7772 2023-05-09 01:36:39.828527 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document_response.pyi
+-rw-r--r--   0        0        0     8727 2023-05-09 01:36:39.828753 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text400_response.py
+-rw-r--r--   0        0        0     8727 2023-05-09 01:36:39.829033 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text400_response.pyi
+-rw-r--r--   0        0        0     8049 2023-05-09 01:36:39.829231 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text_request.py
+-rw-r--r--   0        0        0     7593 2023-05-09 01:36:39.829486 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text_request.pyi
+-rw-r--r--   0        0        0    14321 2023-05-09 01:36:39.829650 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text_response.py
+-rw-r--r--   0        0        0    14321 2023-05-09 01:36:39.830140 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text_response.pyi
+-rw-r--r--   0        0        0     5059 2023-05-09 01:36:39.830443 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_request.py
+-rw-r--r--   0        0        0     4831 2023-05-09 01:36:39.830630 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_request.pyi
+-rw-r--r--   0        0        0     3992 2023-05-09 01:36:39.830795 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py
+-rw-r--r--   0        0        0     3992 2023-05-09 01:36:39.830958 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.pyi
+-rw-r--r--   0        0        0     8531 2023-05-09 01:36:39.831158 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py
+-rw-r--r--   0        0        0     8531 2023-05-09 01:36:39.831383 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.pyi
+-rw-r--r--   0        0        0     3982 2023-05-09 01:36:39.831607 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face400_response.py
+-rw-r--r--   0        0        0     3982 2023-05-09 01:36:39.831766 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face400_response.pyi
+-rw-r--r--   0        0        0     6934 2023-05-09 01:36:39.831922 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face_request.py
+-rw-r--r--   0        0        0     6592 2023-05-09 01:36:39.832094 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face_request.pyi
+-rw-r--r--   0        0        0     7329 2023-05-09 01:36:39.832256 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face_response.py
+-rw-r--r--   0        0        0     7329 2023-05-09 01:36:39.832431 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face_response.pyi
+-rw-r--r--   0        0        0     8177 2023-05-09 01:36:39.832598 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate400_response.py
+-rw-r--r--   0        0        0     8177 2023-05-09 01:36:39.832754 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate400_response.pyi
+-rw-r--r--   0        0        0     6692 2023-05-09 01:36:39.832908 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate_request.py
+-rw-r--r--   0        0        0     6122 2023-05-09 01:36:39.833065 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate_request.pyi
+-rw-r--r--   0        0        0   270536 2023-05-09 01:36:39.833898 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate_response.py
+-rw-r--r--   0        0        0   270536 2023-05-09 01:36:39.834735 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate_response.pyi
+-rw-r--r--   0        0        0     2538 2023-05-09 01:36:39.834919 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/models/__init__.py
+-rw-r--r--   0        0        0      850 2023-05-09 01:36:39.835134 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/__init__.py
+-rw-r--r--   0        0        0      359 2023-05-09 01:36:39.835370 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/__init__.py
+-rw-r--r--   0        0        0    23279 2023-05-09 01:36:39.835584 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py
+-rw-r--r--   0        0        0    18806 2023-05-09 01:36:39.835842 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.pyi
+-rw-r--r--   0        0        0      343 2023-05-09 01:36:39.836118 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/__init__.py
+-rw-r--r--   0        0        0    21323 2023-05-09 01:36:39.836432 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py
+-rw-r--r--   0        0        0    18811 2023-05-09 01:36:39.836865 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-09 01:36:39.837066 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/__init__.py
+-rw-r--r--   0        0        0    19929 2023-05-09 01:36:39.837285 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py
+-rw-r--r--   0        0        0    17417 2023-05-09 01:36:39.837624 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.pyi
+-rw-r--r--   0        0        0      357 2023-05-09 01:36:39.837853 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/__init__.py
+-rw-r--r--   0        0        0    20370 2023-05-09 01:36:39.838099 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py
+-rw-r--r--   0        0        0    17858 2023-05-09 01:36:39.838365 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.pyi
+-rw-r--r--   0        0        0      363 2023-05-09 01:36:39.838690 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/__init__.py
+-rw-r--r--   0        0        0    24221 2023-05-09 01:36:39.838863 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py
+-rw-r--r--   0        0        0    19379 2023-05-09 01:36:39.839136 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.pyi
+-rw-r--r--   0        0        0      367 2023-05-09 01:36:39.839371 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/__init__.py
+-rw-r--r--   0        0        0    19228 2023-05-09 01:36:39.839606 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py
+-rw-r--r--   0        0        0    16716 2023-05-09 01:36:39.839855 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.pyi
+-rw-r--r--   0        0        0      365 2023-05-09 01:36:39.840070 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/__init__.py
+-rw-r--r--   0        0        0    15165 2023-05-09 01:36:39.840257 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py
+-rw-r--r--   0        0        0    14983 2023-05-09 01:36:39.840480 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.pyi
+-rw-r--r--   0        0        0      371 2023-05-09 01:36:39.840685 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/__init__.py
+-rw-r--r--   0        0        0    14949 2023-05-09 01:36:39.840873 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py
+-rw-r--r--   0        0        0    14767 2023-05-09 01:36:39.841135 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.pyi
+-rw-r--r--   0        0        0      673 2023-05-09 01:36:39.841364 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/request_after_hook.py
+-rw-r--r--   0        0        0      674 2023-05-09 01:36:39.841511 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/request_before_hook.py
+-rw-r--r--   0        0        0    10991 2023-05-09 01:36:39.841672 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/rest.py
+-rw-r--r--   0        0        0    95653 2023-05-09 01:36:39.842221 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-09 01:36:39.842365 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/__init__.py
+-rw-r--r--   0        0        0      735 2023-05-09 01:36:39.842500 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_image_quality400_response.py
+-rw-r--r--   0        0        0      768 2023-05-09 01:36:39.842640 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_image_quality_request.py
+-rw-r--r--   0        0        0      816 2023-05-09 01:36:39.842800 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_image_quality_response.py
+-rw-r--r--   0        0        0      714 2023-05-09 01:36:39.842943 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_photocopy400_response.py
+-rw-r--r--   0        0        0      716 2023-05-09 01:36:39.843088 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_photocopy_request.py
+-rw-r--r--   0        0        0      795 2023-05-09 01:36:39.843246 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_photocopy_response.py
+-rw-r--r--   0        0        0      742 2023-05-09 01:36:39.843377 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_video_liveness400_response.py
+-rw-r--r--   0        0        0      743 2023-05-09 01:36:39.843512 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_video_liveness_request.py
+-rw-r--r--   0        0        0      823 2023-05-09 01:36:39.843640 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_video_liveness_response.py
+-rw-r--r--   0        0        0      728 2023-05-09 01:36:39.843779 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/classify_document400_response.py
+-rw-r--r--   0        0        0      763 2023-05-09 01:36:39.843924 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/classify_document_request.py
+-rw-r--r--   0        0        0      809 2023-05-09 01:36:39.844065 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/classify_document_response.py
+-rw-r--r--   0        0        0      856 2023-05-09 01:36:39.844209 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/extract_text400_response.py
+-rw-r--r--   0        0        0      817 2023-05-09 01:36:39.844346 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/extract_text_request.py
+-rw-r--r--   0        0        0      863 2023-05-09 01:36:39.844476 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/extract_text_response.py
+-rw-r--r--   0        0        0      695 2023-05-09 01:36:39.844603 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/mask_aadhaar_request.py
+-rw-r--r--   0        0        0      714 2023-05-09 01:36:39.844712 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/mask_aadhaar_uid400_response.py
+-rw-r--r--   0        0        0      795 2023-05-09 01:36:39.844859 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/mask_aadhaar_uid_response.py
+-rw-r--r--   0        0        0      679 2023-05-09 01:36:39.844981 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/match_face400_response.py
+-rw-r--r--   0        0        0      755 2023-05-09 01:36:39.845080 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/match_face_request.py
+-rw-r--r--   0        0        0      760 2023-05-09 01:36:39.845163 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/match_face_response.py
+-rw-r--r--   0        0        0      812 2023-05-09 01:36:39.845299 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/validate400_response.py
+-rw-r--r--   0        0        0      710 2023-05-09 01:36:39.845440 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/validate_request.py
+-rw-r--r--   0        0        0      945 2023-05-09 01:36:39.845570 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/validate_response.py
+-rw-r--r--   0        0        0      517 2023-05-09 01:36:39.845713 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type_util.py
+-rw-r--r--   0        0        0     3178 2023-05-09 01:36:39.845852 decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/validation_metadata.py
+-rw-r--r--   0        0        0      728 2023-05-09 01:36:39.850585 decentro_in_kyc_python_sdk-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6178 1970-01-01 00:00:00.000000 decentro_in_kyc_python_sdk-4.4.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/LICENSE` & `decentro_in_kyc_python_sdk-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/PKG-INFO` & `decentro_in_kyc_python_sdk-4.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,54 @@
-Metadata-Version: 2.1
-Name: decentro-in-kyc-python-sdk
-Version: 4.3.0
-Summary: decentro-in-kyc
-Home-page: https://decentro.tech
-Author: Decentro
-Author-email: admin@decentro.tech
-License: MIT
-Keywords: decentro-in-kyc
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# decentro-in-kyc-python-sdk
+# decentro-in-kyc-python-sdk@4.4.0
 KYC & Onboarding
 
-- API version: 1.0.0
-- Package version: 4.3.0
-For more information, please visit [https://decentro.tech](https://decentro.tech)
 
-## Requirements.
+## Requirements
 
 Python >=3.7
 
-## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
+## Installing
 
 ```sh
-pip install decentro-in-kyc-python-sdk==4.3.0
+pip install decentro-in-kyc-python-sdk==4.4.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.3.0`)
 
-Then import the package:
-```python
-import decentro_in_kyc_client
-```
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
-
 ```python
 from pprint import pprint
-from decentro_in_kyc_client import Decentro
+from decentro_in_kyc_client import Decentro, ApiException
 
 decentro = Decentro(
     # Defining the host is optional and defaults to https://in.staging.decentro.tech
     # See configuration.py for a list of all supported configuration parameters.
-    host = "https://in.staging.decentro.tech",
-
+    host="https://in.staging.decentro.tech",
     # Configure API key authorization: client_id
-    client_id = 'YOUR_API_KEY',
+    client_id="YOUR_API_KEY",
     # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
     # api_key_prefix = {'client_id': 'Bearer'},
-
     # Configure API key authorization: client_secret
-    client_secret = 'YOUR_API_KEY',
+    client_secret="YOUR_API_KEY",
     # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
     # api_key_prefix = {'client_secret': 'Bearer'},
-
     # Configure API key authorization: module_secret
-    module_secret = 'YOUR_API_KEY',
+    module_secret="YOUR_API_KEY",
     # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
     # api_key_prefix = {'module_secret': 'Bearer'},
 )
 
-body = {
-        "reference_id": "ABCDEF12345",
-        "consent": False,
-        "consent_purpose": "For Testing Purpose Only",
-        "quality_parameter": "all",
-    }
 try:
     # Image Quality Check
     check_image_quality_response = decentro.kyc.check_image_quality(
-        body=body
+        reference_id="ABCDEF12345",  # required
+        consent=False,  # required
+        consent_purpose="For Testing Purpose Only",  # required
+        image=open("/path/to/file", "rb"),  # optional
+        quality_parameter="all",  # optional
+        image_url="string_example",  # optional
     )
     pprint(check_image_quality_response.body)
     pprint(check_image_quality_response.body["decentroTxnId"])
     pprint(check_image_quality_response.body["status"])
     pprint(check_image_quality_response.body["responseCode"])
     pprint(check_image_quality_response.body["message"])
     pprint(check_image_quality_response.body["data"])
@@ -137,32 +107,8 @@
  - [MatchFace400Response](docs/models/MatchFace400Response.md)
  - [MatchFaceRequest](docs/models/MatchFaceRequest.md)
  - [MatchFaceResponse](docs/models/MatchFaceResponse.md)
  - [Validate400Response](docs/models/Validate400Response.md)
  - [ValidateRequest](docs/models/ValidateRequest.md)
  - [ValidateResponse](docs/models/ValidateResponse.md)
 
-## Documentation For Authorization
-
- Authentication schemes defined for the API:
-## client_id
-
-- **Type**: API key
-- **API key parameter name**: client_id
-- **Location**: HTTP header
-
-
-## client_secret
-
-- **Type**: API key
-- **API key parameter name**: client_secret
-- **Location**: HTTP header
-
-
-## module_secret
-
-- **Type**: API key
-- **API key parameter name**: module_secret
-- **Location**: HTTP header
-
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/README.md` & `decentro_in_kyc_python_sdk-4.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,78 @@
-# decentro-in-kyc-python-sdk
+Metadata-Version: 2.1
+Name: decentro-in-kyc-python-sdk
+Version: 4.4.0
+Summary: KYC &amp; Onboarding
+License: MIT
+Author: Decentro
+Author-email: admin@decentro.tech
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: certifi (==2022.12.7)
+Requires-Dist: frozendict (==2.3.4)
+Requires-Dist: python-dateutil (==2.8.2)
+Requires-Dist: typing_extensions (==4.3.0)
+Requires-Dist: urllib3 (==1.26.7)
+Requires-Dist: validators (==0.20.0)
+Description-Content-Type: text/markdown
+
+# decentro-in-kyc-python-sdk@4.4.0
 KYC & Onboarding
 
-- API version: 1.0.0
-- Package version: 4.3.0
-For more information, please visit [https://decentro.tech](https://decentro.tech)
 
-## Requirements.
+## Requirements
 
 Python >=3.7
 
-## Installation & Usage
-### pip install
-
-If the python package is hosted on a repository, you can install directly using:
+## Installing
 
 ```sh
-pip install decentro-in-kyc-python-sdk==4.3.0
+pip install decentro-in-kyc-python-sdk==4.4.0
 ```
-(you may need to run `pip` with root permission: `sudo pip install decentro-in-kyc-python-sdk==4.3.0`)
 
-Then import the package:
-```python
-import decentro_in_kyc_client
-```
 ## Getting Started
 
-Please follow the [installation procedure](#installation--usage) and then run the following:
-
 ```python
 from pprint import pprint
-from decentro_in_kyc_client import Decentro
+from decentro_in_kyc_client import Decentro, ApiException
 
 decentro = Decentro(
     # Defining the host is optional and defaults to https://in.staging.decentro.tech
     # See configuration.py for a list of all supported configuration parameters.
-    host = "https://in.staging.decentro.tech",
-
+    host="https://in.staging.decentro.tech",
     # Configure API key authorization: client_id
-    client_id = 'YOUR_API_KEY',
+    client_id="YOUR_API_KEY",
     # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
     # api_key_prefix = {'client_id': 'Bearer'},
-
     # Configure API key authorization: client_secret
-    client_secret = 'YOUR_API_KEY',
+    client_secret="YOUR_API_KEY",
     # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
     # api_key_prefix = {'client_secret': 'Bearer'},
-
     # Configure API key authorization: module_secret
-    module_secret = 'YOUR_API_KEY',
+    module_secret="YOUR_API_KEY",
     # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
     # api_key_prefix = {'module_secret': 'Bearer'},
 )
 
-body = {
-        "reference_id": "ABCDEF12345",
-        "consent": False,
-        "consent_purpose": "For Testing Purpose Only",
-        "quality_parameter": "all",
-    }
 try:
     # Image Quality Check
     check_image_quality_response = decentro.kyc.check_image_quality(
-        body=body
+        reference_id="ABCDEF12345",  # required
+        consent=False,  # required
+        consent_purpose="For Testing Purpose Only",  # required
+        image=open("/path/to/file", "rb"),  # optional
+        quality_parameter="all",  # optional
+        image_url="string_example",  # optional
     )
     pprint(check_image_quality_response.body)
     pprint(check_image_quality_response.body["decentroTxnId"])
     pprint(check_image_quality_response.body["status"])
     pprint(check_image_quality_response.body["responseCode"])
     pprint(check_image_quality_response.body["message"])
     pprint(check_image_quality_response.body["data"])
@@ -124,32 +131,9 @@
  - [MatchFace400Response](docs/models/MatchFace400Response.md)
  - [MatchFaceRequest](docs/models/MatchFaceRequest.md)
  - [MatchFaceResponse](docs/models/MatchFaceResponse.md)
  - [Validate400Response](docs/models/Validate400Response.md)
  - [ValidateRequest](docs/models/ValidateRequest.md)
  - [ValidateResponse](docs/models/ValidateResponse.md)
 
-## Documentation For Authorization
-
- Authentication schemes defined for the API:
-## client_id
-
-- **Type**: API key
-- **API key parameter name**: client_id
-- **Location**: HTTP header
-
-
-## client_secret
-
-- **Type**: API key
-- **API key parameter name**: client_secret
-- **Location**: HTTP header
-
-
-## module_secret
-
-- **Type**: API key
-- **API key parameter name**: module_secret
-- **Location**: HTTP header
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/__init__.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     KYC & Onboarding
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
-__version__ = "4.3.0"
+__version__ = "4.4.0"
 
 # import ApiClient
 from decentro_in_kyc_client.api_client import ApiClient
 
 # import Configuration
 from decentro_in_kyc_client.configuration import Configuration
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/api_client.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/api_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,3955 +18,4527 @@
 00000110: 0a69 6d70 6f72 7420 6a73 6f6e 0a69 6d70  .import json.imp
 00000120: 6f72 7420 6f73 0a69 6d70 6f72 7420 696f  ort os.import io
 00000130: 0a69 6d70 6f72 7420 6174 6578 6974 0a66  .import atexit.f
 00000140: 726f 6d20 6d75 6c74 6970 726f 6365 7373  rom multiprocess
 00000150: 696e 672e 706f 6f6c 2069 6d70 6f72 7420  ing.pool import 
 00000160: 5468 7265 6164 506f 6f6c 0a69 6d70 6f72  ThreadPool.impor
 00000170: 7420 7265 0a69 6d70 6f72 7420 7465 6d70  t re.import temp
-00000180: 6669 6c65 0a69 6d70 6f72 7420 7479 7069  file.import typi
-00000190: 6e67 0a69 6d70 6f72 7420 7479 7069 6e67  ng.import typing
-000001a0: 5f65 7874 656e 7369 6f6e 730a 696d 706f  _extensions.impo
-000001b0: 7274 2075 726c 6c69 6233 0a66 726f 6d20  rt urllib3.from 
-000001c0: 7572 6c6c 6962 332e 5f63 6f6c 6c65 6374  urllib3._collect
-000001d0: 696f 6e73 2069 6d70 6f72 7420 4854 5450  ions import HTTP
-000001e0: 4865 6164 6572 4469 6374 0a66 726f 6d20  HeaderDict.from 
-000001f0: 7572 6c6c 6962 2e70 6172 7365 2069 6d70  urllib.parse imp
-00000200: 6f72 7420 7572 6c70 6172 7365 2c20 7175  ort urlparse, qu
-00000210: 6f74 650a 6672 6f6d 2075 726c 6c69 6233  ote.from urllib3
-00000220: 2e66 6965 6c64 7320 696d 706f 7274 2052  .fields import R
-00000230: 6571 7565 7374 4669 656c 6420 6173 2052  equestField as R
-00000240: 6571 7565 7374 4669 656c 6442 6173 650a  equestFieldBase.
-00000250: 6672 6f6d 2075 726c 6c69 6233 2e66 6965  from urllib3.fie
-00000260: 6c64 7320 696d 706f 7274 2067 7565 7373  lds import guess
-00000270: 5f63 6f6e 7465 6e74 5f74 7970 650a 0a69  _content_type..i
-00000280: 6d70 6f72 7420 6672 6f7a 656e 6469 6374  mport frozendict
-00000290: 0a0a 6672 6f6d 2064 6563 656e 7472 6f5f  ..from decentro_
-000002a0: 696e 5f6b 7963 5f63 6c69 656e 7420 696d  in_kyc_client im
-000002b0: 706f 7274 2072 6573 740a 6672 6f6d 2064  port rest.from d
-000002c0: 6563 656e 7472 6f5f 696e 5f6b 7963 5f63  ecentro_in_kyc_c
-000002d0: 6c69 656e 742e 6170 695f 7265 7370 6f6e  lient.api_respon
-000002e0: 7365 2069 6d70 6f72 7420 4170 6952 6573  se import ApiRes
-000002f0: 706f 6e73 650a 6672 6f6d 2064 6563 656e  ponse.from decen
-00000300: 7472 6f5f 696e 5f6b 7963 5f63 6c69 656e  tro_in_kyc_clien
-00000310: 742e 7265 7374 2069 6d70 6f72 7420 5265  t.rest import Re
-00000320: 7370 6f6e 7365 5772 6170 7065 720a 6672  sponseWrapper.fr
-00000330: 6f6d 2064 6563 656e 7472 6f5f 696e 5f6b  om decentro_in_k
-00000340: 7963 5f63 6c69 656e 742e 636f 6e66 6967  yc_client.config
-00000350: 7572 6174 696f 6e20 696d 706f 7274 2043  uration import C
-00000360: 6f6e 6669 6775 7261 7469 6f6e 0a66 726f  onfiguration.fro
-00000370: 6d20 6465 6365 6e74 726f 5f69 6e5f 6b79  m decentro_in_ky
-00000380: 635f 636c 6965 6e74 2e65 7863 6570 7469  c_client.excepti
-00000390: 6f6e 7320 696d 706f 7274 2041 7069 5479  ons import ApiTy
-000003a0: 7065 4572 726f 722c 2041 7069 5661 6c75  peError, ApiValu
-000003b0: 6545 7272 6f72 2c20 4d69 7373 696e 6752  eError, MissingR
-000003c0: 6571 7569 7265 6450 6172 616d 6574 6572  equiredParameter
-000003d0: 7345 7272 6f72 0a66 726f 6d20 6465 6365  sError.from dece
-000003e0: 6e74 726f 5f69 6e5f 6b79 635f 636c 6965  ntro_in_kyc_clie
-000003f0: 6e74 2e72 6571 7565 7374 5f61 6674 6572  nt.request_after
-00000400: 5f68 6f6f 6b20 696d 706f 7274 2072 6571  _hook import req
-00000410: 7565 7374 5f61 6674 6572 5f68 6f6f 6b0a  uest_after_hook.
-00000420: 6672 6f6d 2064 6563 656e 7472 6f5f 696e  from decentro_in
-00000430: 5f6b 7963 5f63 6c69 656e 742e 7265 7175  _kyc_client.requ
-00000440: 6573 745f 6265 666f 7265 5f68 6f6f 6b20  est_before_hook 
-00000450: 696d 706f 7274 2072 6571 7565 7374 5f62  import request_b
-00000460: 6566 6f72 655f 686f 6f6b 0a66 726f 6d20  efore_hook.from 
-00000470: 6465 6365 6e74 726f 5f69 6e5f 6b79 635f  decentro_in_kyc_
-00000480: 636c 6965 6e74 2e73 6368 656d 6173 2069  client.schemas i
-00000490: 6d70 6f72 7420 280a 2020 2020 4e6f 6e65  mport (.    None
-000004a0: 436c 6173 732c 0a20 2020 2042 6f6f 6c43  Class,.    BoolC
-000004b0: 6c61 7373 2c0a 2020 2020 5363 6865 6d61  lass,.    Schema
-000004c0: 2c0a 2020 2020 4669 6c65 494f 2c0a 2020  ,.    FileIO,.  
-000004d0: 2020 4269 6e61 7279 5363 6865 6d61 2c0a    BinarySchema,.
-000004e0: 2020 2020 6461 7465 2c0a 2020 2020 6461      date,.    da
-000004f0: 7465 7469 6d65 2c0a 2020 2020 6e6f 6e65  tetime,.    none
-00000500: 5f74 7970 652c 0a20 2020 2055 6e73 6574  _type,.    Unset
-00000510: 2c0a 2020 2020 756e 7365 742c 0a29 0a0a  ,.    unset,.)..
-00000520: 0a63 6c61 7373 2052 6571 7565 7374 4669  .class RequestFi
-00000530: 656c 6428 5265 7175 6573 7446 6965 6c64  eld(RequestField
-00000540: 4261 7365 293a 0a20 2020 2064 6566 205f  Base):.    def _
-00000550: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
-00000560: 7229 3a0a 2020 2020 2020 2020 6966 206e  r):.        if n
-00000570: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
-00000580: 6865 722c 2052 6571 7565 7374 4669 656c  her, RequestFiel
-00000590: 6429 3a0a 2020 2020 2020 2020 2020 2020  d):.            
-000005a0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
-000005b0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000005c0: 2e5f 5f64 6963 745f 5f20 3d3d 206f 7468  .__dict__ == oth
-000005d0: 6572 2e5f 5f64 6963 745f 5f0a 0a0a 636c  er.__dict__...cl
-000005e0: 6173 7320 4a53 4f4e 456e 636f 6465 7228  ass JSONEncoder(
-000005f0: 6a73 6f6e 2e4a 534f 4e45 6e63 6f64 6572  json.JSONEncoder
-00000600: 293a 0a20 2020 2063 6f6d 7061 6374 5f73  ):.    compact_s
-00000610: 6570 6172 6174 6f72 7320 3d20 2827 2c27  eparators = (','
-00000620: 2c20 273a 2729 0a0a 2020 2020 6465 6620  , ':')..    def 
-00000630: 6465 6661 756c 7428 7365 6c66 2c20 6f62  default(self, ob
-00000640: 6a29 3a0a 2020 2020 2020 2020 6966 2069  j):.        if i
-00000650: 7369 6e73 7461 6e63 6528 6f62 6a2c 2073  sinstance(obj, s
-00000660: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
-00000670: 2072 6574 7572 6e20 7374 7228 6f62 6a29   return str(obj)
-00000680: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00000690: 696e 7374 616e 6365 286f 626a 2c20 666c  instance(obj, fl
-000006a0: 6f61 7429 3a0a 2020 2020 2020 2020 2020  oat):.          
-000006b0: 2020 7265 7475 726e 2066 6c6f 6174 286f    return float(o
-000006c0: 626a 290a 2020 2020 2020 2020 656c 6966  bj).        elif
-000006d0: 2069 7369 6e73 7461 6e63 6528 6f62 6a2c   isinstance(obj,
-000006e0: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
-000006f0: 2020 2072 6574 7572 6e20 696e 7428 6f62     return int(ob
-00000700: 6a29 0a20 2020 2020 2020 2065 6c69 6620  j).        elif 
-00000710: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
-00000720: 4465 6369 6d61 6c29 3a0a 2020 2020 2020  Decimal):.      
-00000730: 2020 2020 2020 6966 206f 626a 2e61 735f        if obj.as_
-00000740: 7475 706c 6528 292e 6578 706f 6e65 6e74  tuple().exponent
-00000750: 203e 3d20 303a 0a20 2020 2020 2020 2020   >= 0:.         
-00000760: 2020 2020 2020 2072 6574 7572 6e20 696e         return in
-00000770: 7428 6f62 6a29 0a20 2020 2020 2020 2020  t(obj).         
-00000780: 2020 2072 6574 7572 6e20 666c 6f61 7428     return float(
-00000790: 6f62 6a29 0a20 2020 2020 2020 2065 6c69  obj).        eli
-000007a0: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-000007b0: 2c20 4e6f 6e65 436c 6173 7329 3a0a 2020  , NoneClass):.  
-000007c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000007d0: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
-000007e0: 6966 2069 7369 6e73 7461 6e63 6528 6f62  if isinstance(ob
-000007f0: 6a2c 2042 6f6f 6c43 6c61 7373 293a 0a20  j, BoolClass):. 
-00000800: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000810: 6e20 626f 6f6c 286f 626a 290a 2020 2020  n bool(obj).    
-00000820: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-00000830: 6e63 6528 6f62 6a2c 2028 6469 6374 2c20  nce(obj, (dict, 
-00000840: 6672 6f7a 656e 6469 6374 2e66 726f 7a65  frozendict.froze
-00000850: 6e64 6963 7429 293a 0a20 2020 2020 2020  ndict)):.       
-00000860: 2020 2020 2072 6574 7572 6e20 7b6b 6579       return {key
-00000870: 3a20 7365 6c66 2e64 6566 6175 6c74 2876  : self.default(v
-00000880: 616c 2920 666f 7220 6b65 792c 2076 616c  al) for key, val
-00000890: 2069 6e20 6f62 6a2e 6974 656d 7328 297d   in obj.items()}
-000008a0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-000008b0: 696e 7374 616e 6365 286f 626a 2c20 286c  instance(obj, (l
-000008c0: 6973 742c 2074 7570 6c65 2929 3a0a 2020  ist, tuple)):.  
-000008d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000008e0: 205b 7365 6c66 2e64 6566 6175 6c74 2869   [self.default(i
-000008f0: 7465 6d29 2066 6f72 2069 7465 6d20 696e  tem) for item in
-00000900: 206f 626a 5d0a 2020 2020 2020 2020 7261   obj].        ra
-00000910: 6973 6520 4170 6956 616c 7565 4572 726f  ise ApiValueErro
-00000920: 7228 2755 6e61 626c 6520 746f 2070 7265  r('Unable to pre
-00000930: 7061 7265 2074 7970 6520 7b7d 2066 6f72  pare type {} for
-00000940: 2073 6572 6961 6c69 7a61 7469 6f6e 272e   serialization'.
-00000950: 666f 726d 6174 286f 626a 2e5f 5f63 6c61  format(obj.__cla
-00000960: 7373 5f5f 2e5f 5f6e 616d 655f 5f29 290a  ss__.__name__)).
-00000970: 0a0a 636c 6173 7320 5061 7261 6d65 7465  ..class Paramete
-00000980: 7249 6e54 7970 6528 656e 756d 2e45 6e75  rInType(enum.Enu
-00000990: 6d29 3a0a 2020 2020 5155 4552 5920 3d20  m):.    QUERY = 
-000009a0: 2771 7565 7279 270a 2020 2020 4845 4144  'query'.    HEAD
-000009b0: 4552 203d 2027 6865 6164 6572 270a 2020  ER = 'header'.  
-000009c0: 2020 5041 5448 203d 2027 7061 7468 270a    PATH = 'path'.
-000009d0: 2020 2020 434f 4f4b 4945 203d 2027 636f      COOKIE = 'co
-000009e0: 6f6b 6965 270a 0a0a 636c 6173 7320 5061  okie'...class Pa
-000009f0: 7261 6d65 7465 7253 7479 6c65 2865 6e75  rameterStyle(enu
-00000a00: 6d2e 456e 756d 293a 0a20 2020 204d 4154  m.Enum):.    MAT
-00000a10: 5249 5820 3d20 276d 6174 7269 7827 0a20  RIX = 'matrix'. 
-00000a20: 2020 204c 4142 454c 203d 2027 6c61 6265     LABEL = 'labe
-00000a30: 6c27 0a20 2020 2046 4f52 4d20 3d20 2766  l'.    FORM = 'f
-00000a40: 6f72 6d27 0a20 2020 2053 494d 504c 4520  orm'.    SIMPLE 
-00000a50: 3d20 2773 696d 706c 6527 0a20 2020 2053  = 'simple'.    S
-00000a60: 5041 4345 5f44 454c 494d 4954 4544 203d  PACE_DELIMITED =
-00000a70: 2027 7370 6163 6544 656c 696d 6974 6564   'spaceDelimited
-00000a80: 270a 2020 2020 5049 5045 5f44 454c 494d  '.    PIPE_DELIM
-00000a90: 4954 4544 203d 2027 7069 7065 4465 6c69  ITED = 'pipeDeli
-00000aa0: 6d69 7465 6427 0a20 2020 2044 4545 505f  mited'.    DEEP_
-00000ab0: 4f42 4a45 4354 203d 2027 6465 6570 4f62  OBJECT = 'deepOb
-00000ac0: 6a65 6374 270a 0a0a 636c 6173 7320 5072  ject'...class Pr
-00000ad0: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
-00000ae0: 7261 746f 723a 0a20 2020 2023 2041 2063  rator:.    # A c
-00000af0: 6c61 7373 2074 6f20 7374 6f72 6520 7072  lass to store pr
-00000b00: 6566 6978 6573 2061 6e64 2073 6570 6172  efixes and separ
-00000b10: 6174 6f72 7320 666f 7220 7266 6336 3537  ators for rfc657
-00000b20: 3020 6578 7061 6e73 696f 6e73 0a0a 2020  0 expansions..  
-00000b30: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000b40: 656c 662c 2070 7265 6669 783a 2073 7472  elf, prefix: str
-00000b50: 2c20 7365 7061 7261 746f 723a 2073 7472  , separator: str
-00000b60: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00000b70: 7072 6566 6978 203d 2070 7265 6669 780a  prefix = prefix.
-00000b80: 2020 2020 2020 2020 7365 6c66 2e73 6570          self.sep
-00000b90: 6172 6174 6f72 203d 2073 6570 6172 6174  arator = separat
-00000ba0: 6f72 0a20 2020 2020 2020 2073 656c 662e  or.        self.
-00000bb0: 6669 7273 7420 3d20 5472 7565 0a20 2020  first = True.   
-00000bc0: 2020 2020 2069 6620 7365 7061 7261 746f       if separato
-00000bd0: 7220 696e 207b 272e 272c 2027 7c27 2c20  r in {'.', '|', 
-00000be0: 2725 3230 277d 3a0a 2020 2020 2020 2020  '%20'}:.        
-00000bf0: 2020 2020 6974 656d 5f73 6570 6172 6174      item_separat
-00000c00: 6f72 203d 2073 6570 6172 6174 6f72 0a20  or = separator. 
-00000c10: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000c20: 2020 2020 2020 2020 2069 7465 6d5f 7365           item_se
-00000c30: 7061 7261 746f 7220 3d20 272c 270a 2020  parator = ','.  
-00000c40: 2020 2020 2020 7365 6c66 2e69 7465 6d5f        self.item_
-00000c50: 7365 7061 7261 746f 7220 3d20 6974 656d  separator = item
-00000c60: 5f73 6570 6172 6174 6f72 0a0a 2020 2020  _separator..    
-00000c70: 6465 6620 5f5f 6974 6572 5f5f 2873 656c  def __iter__(sel
-00000c80: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00000c90: 726e 2073 656c 660a 0a20 2020 2064 6566  rn self..    def
-00000ca0: 205f 5f6e 6578 745f 5f28 7365 6c66 293a   __next__(self):
-00000cb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00000cc0: 2e66 6972 7374 3a0a 2020 2020 2020 2020  .first:.        
-00000cd0: 2020 2020 7365 6c66 2e66 6972 7374 203d      self.first =
-00000ce0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00000cf0: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
-00000d00: 7265 6669 780a 2020 2020 2020 2020 7265  refix.        re
-00000d10: 7475 726e 2073 656c 662e 7365 7061 7261  turn self.separa
-00000d20: 746f 720a 0a0a 636c 6173 7320 5061 7261  tor...class Para
-00000d30: 6d65 7465 7253 6572 6961 6c69 7a65 7242  meterSerializerB
-00000d40: 6173 653a 0a20 2020 2040 636c 6173 736d  ase:.    @classm
-00000d50: 6574 686f 640a 2020 2020 6465 6620 5f67  ethod.    def _g
-00000d60: 6574 5f64 6566 6175 6c74 5f65 7870 6c6f  et_default_explo
-00000d70: 6465 2863 6c73 2c20 7374 796c 653a 2050  de(cls, style: P
-00000d80: 6172 616d 6574 6572 5374 796c 6529 202d  arameterStyle) -
-00000d90: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
-00000da0: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
-00000db0: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-00000dc0: 2020 2020 6465 6620 5f5f 7265 6636 3537      def __ref657
-00000dd0: 305f 6974 656d 5f76 616c 7565 2869 6e5f  0_item_value(in_
-00000de0: 6461 7461 3a20 7479 7069 6e67 2e41 6e79  data: typing.Any
-00000df0: 2c20 7065 7263 656e 745f 656e 636f 6465  , percent_encode
-00000e00: 3a20 626f 6f6c 293a 0a20 2020 2020 2020  : bool):.       
-00000e10: 2022 2222 0a20 2020 2020 2020 2047 6574   """.        Get
-00000e20: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-00000e30: 6966 2073 7472 2f66 6c6f 6174 2f69 6e74  if str/float/int
-00000e40: 2f4e 6f6e 652f 6974 656d 7320 696e 206c  /None/items in l
-00000e50: 6973 742f 2076 616c 7565 7320 696e 2064  ist/ values in d
-00000e60: 6963 740a 2020 2020 2020 2020 4e6f 6e65  ict.        None
-00000e70: 2069 7320 7265 7475 726e 6564 2069 6620   is returned if 
-00000e80: 616e 2069 7465 6d20 6973 2075 6e64 6566  an item is undef
-00000e90: 696e 6564 2c20 7573 6520 6361 7365 7320  ined, use cases 
-00000ea0: 6172 6520 7661 6c75 653d 0a20 2020 2020  are value=.     
-00000eb0: 2020 202d 204e 6f6e 650a 2020 2020 2020     - None.      
-00000ec0: 2020 2d20 5b5d 0a20 2020 2020 2020 202d    - [].        -
-00000ed0: 207b 7d0a 2020 2020 2020 2020 2d20 5b4e   {}.        - [N
-00000ee0: 6f6e 652c 204e 6f6e 6520 4e6f 6e65 5d0a  one, None None].
-00000ef0: 2020 2020 2020 2020 2d20 7b27 6127 3a20          - {'a': 
-00000f00: 4e6f 6e65 2c20 2762 273a 204e 6f6e 657d  None, 'b': None}
-00000f10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00000f20: 2020 2020 2069 6620 7479 7065 2869 6e5f       if type(in_
-00000f30: 6461 7461 2920 696e 207b 7374 722c 2066  data) in {str, f
-00000f40: 6c6f 6174 2c20 696e 747d 3a0a 2020 2020  loat, int}:.    
-00000f50: 2020 2020 2020 2020 6966 2070 6572 6365          if perce
-00000f60: 6e74 5f65 6e63 6f64 653a 0a20 2020 2020  nt_encode:.     
-00000f70: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000f80: 6e20 7175 6f74 6528 7374 7228 696e 5f64  n quote(str(in_d
-00000f90: 6174 6129 290a 2020 2020 2020 2020 2020  ata)).          
-00000fa0: 2020 7265 7475 726e 2073 7472 2869 6e5f    return str(in_
-00000fb0: 6461 7461 290a 2020 2020 2020 2020 656c  data).        el
-00000fc0: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
-00000fd0: 5f64 6174 612c 206e 6f6e 655f 7479 7065  _data, none_type
-00000fe0: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00000ff0: 2069 676e 6f72 6564 2062 7920 7468 6520   ignored by the 
-00001000: 6578 7061 6e73 696f 6e20 7072 6f63 6573  expansion proces
-00001010: 7320 6874 7470 733a 2f2f 6461 7461 7472  s https://datatr
-00001020: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
-00001030: 6f63 2f68 746d 6c2f 7266 6336 3537 3023  oc/html/rfc6570#
-00001040: 7365 6374 696f 6e2d 332e 322e 310a 2020  section-3.2.1.  
-00001050: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001060: 204e 6f6e 650a 2020 2020 2020 2020 656c   None.        el
-00001070: 6966 2069 7369 6e73 7461 6e63 6528 696e  if isinstance(in
-00001080: 5f64 6174 612c 206c 6973 7429 2061 6e64  _data, list) and
-00001090: 206e 6f74 2069 6e5f 6461 7461 3a0a 2020   not in_data:.  
-000010a0: 2020 2020 2020 2020 2020 2320 6967 6e6f            # igno
-000010b0: 7265 6420 6279 2074 6865 2065 7870 616e  red by the expan
-000010c0: 7369 6f6e 2070 726f 6365 7373 2068 7474  sion process htt
-000010d0: 7073 3a2f 2f64 6174 6174 7261 636b 6572  ps://datatracker
-000010e0: 2e69 6574 662e 6f72 672f 646f 632f 6874  .ietf.org/doc/ht
-000010f0: 6d6c 2f72 6663 3635 3730 2373 6563 7469  ml/rfc6570#secti
-00001100: 6f6e 2d33 2e32 2e31 0a20 2020 2020 2020  on-3.2.1.       
-00001110: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00001120: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-00001130: 696e 7374 616e 6365 2869 6e5f 6461 7461  instance(in_data
-00001140: 2c20 6469 6374 2920 616e 6420 6e6f 7420  , dict) and not 
-00001150: 696e 5f64 6174 613a 0a20 2020 2020 2020  in_data:.       
-00001160: 2020 2020 2023 2069 676e 6f72 6564 2062       # ignored b
-00001170: 7920 7468 6520 6578 7061 6e73 696f 6e20  y the expansion 
-00001180: 7072 6f63 6573 7320 6874 7470 733a 2f2f  process https://
-00001190: 6461 7461 7472 6163 6b65 722e 6965 7466  datatracker.ietf
-000011a0: 2e6f 7267 2f64 6f63 2f68 746d 6c2f 7266  .org/doc/html/rf
-000011b0: 6336 3537 3023 7365 6374 696f 6e2d 332e  c6570#section-3.
-000011c0: 322e 310a 2020 2020 2020 2020 2020 2020  2.1.            
-000011d0: 7265 7475 726e 204e 6f6e 650a 2020 2020  return None.    
-000011e0: 2020 2020 7261 6973 6520 4170 6956 616c      raise ApiVal
-000011f0: 7565 4572 726f 7228 2755 6e61 626c 6520  ueError('Unable 
-00001200: 746f 2067 656e 6572 6174 6520 6120 7265  to generate a re
-00001210: 6636 3537 3020 6974 656d 2072 6570 7265  f6570 item repre
-00001220: 7365 6e74 6174 696f 6e20 6f66 207b 7d27  sentation of {}'
-00001230: 2e66 6f72 6d61 7428 696e 5f64 6174 6129  .format(in_data)
-00001240: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
-00001250: 7468 6f64 0a20 2020 2064 6566 205f 746f  thod.    def _to
-00001260: 5f64 6963 7428 6e61 6d65 3a20 7374 722c  _dict(name: str,
-00001270: 2076 616c 7565 3a20 7374 7229 3a0a 2020   value: str):.  
-00001280: 2020 2020 2020 7265 7475 726e 207b 6e61        return {na
-00001290: 6d65 3a20 7661 6c75 657d 0a0a 2020 2020  me: value}..    
-000012a0: 2222 220a 2020 2020 7266 6336 3537 3020  """.    rfc6570 
-000012b0: 646f 6573 206e 6f74 2073 7065 6369 6679  does not specify
-000012c0: 2068 6f77 2062 6f6f 6c65 616e 2076 616c   how boolean val
-000012d0: 7565 7320 6172 6520 7365 7269 616c 697a  ues are serializ
-000012e0: 6564 2073 6f20 7765 2075 7365 206c 6f77  ed so we use low
-000012f0: 6572 6361 7365 2022 7472 7565 2220 616e  ercase "true" an
-00001300: 6420 2266 616c 7365 0a20 2020 2022 2222  d "false.    """
-00001310: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00001320: 640a 2020 2020 6465 6620 5f5f 6b6f 6e66  d.    def __konf
-00001330: 6967 5f62 6f6f 6c5f 6578 7061 6e73 696f  ig_bool_expansio
-00001340: 6e28 0a20 2020 2020 2020 2063 6c73 2c0a  n(.        cls,.
-00001350: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
-00001360: 2074 7970 696e 672e 416e 792c 0a20 2020   typing.Any,.   
-00001370: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-00001380: 7261 746f 725f 6974 6572 6174 6f72 3a20  rator_iterator: 
-00001390: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
-000013a0: 7465 7261 746f 722c 0a20 2020 2020 2020  terator,.       
-000013b0: 2076 6172 5f6e 616d 655f 7069 6563 653a   var_name_piece:
-000013c0: 2073 7472 2c0a 2020 2020 2020 2020 6e61   str,.        na
-000013d0: 6d65 645f 7061 7261 6d65 7465 725f 6578  med_parameter_ex
-000013e0: 7061 6e73 696f 6e3a 2062 6f6f 6c0a 2020  pansion: bool.  
-000013f0: 2020 2920 2d3e 2073 7472 3a0a 2020 2020    ) -> str:.    
-00001400: 2020 2020 6974 656d 5f76 616c 7565 203d      item_value =
-00001410: 2022 7472 7565 2220 6966 2069 6e5f 6461   "true" if in_da
-00001420: 7461 2069 7320 5472 7565 2065 6c73 6520  ta is True else 
-00001430: 2266 616c 7365 220a 2020 2020 2020 2020  "false".        
-00001440: 6966 2069 7465 6d5f 7661 6c75 6520 6973  if item_value is
-00001450: 204e 6f6e 6520 6f72 2028 6974 656d 5f76   None or (item_v
-00001460: 616c 7565 203d 3d20 2727 2061 6e64 2070  alue == '' and p
-00001470: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00001480: 6974 6572 6174 6f72 2e73 6570 6172 6174  iterator.separat
-00001490: 6f72 203d 3d20 273b 2729 3a0a 2020 2020  or == ';'):.    
-000014a0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-000014b0: 6578 7428 7072 6566 6978 5f73 6570 6172  ext(prefix_separ
-000014c0: 6174 6f72 5f69 7465 7261 746f 7229 202b  ator_iterator) +
-000014d0: 2076 6172 5f6e 616d 655f 7069 6563 650a   var_name_piece.
-000014e0: 2020 2020 2020 2020 7661 6c75 655f 7061          value_pa
-000014f0: 6972 5f65 7175 616c 7320 3d20 273d 2720  ir_equals = '=' 
-00001500: 6966 206e 616d 6564 5f70 6172 616d 6574  if named_paramet
-00001510: 6572 5f65 7870 616e 7369 6f6e 2065 6c73  er_expansion els
-00001520: 6520 2727 0a20 2020 2020 2020 2072 6574  e ''.        ret
-00001530: 7572 6e20 6e65 7874 2870 7265 6669 785f  urn next(prefix_
-00001540: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-00001550: 6f72 2920 2b20 7661 725f 6e61 6d65 5f70  or) + var_name_p
-00001560: 6965 6365 202b 2076 616c 7565 5f70 6169  iece + value_pai
-00001570: 725f 6571 7561 6c73 202b 2069 7465 6d5f  r_equals + item_
-00001580: 7661 6c75 650a 0a20 2020 2040 636c 6173  value..    @clas
-00001590: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-000015a0: 5f5f 7265 6636 3537 305f 7374 725f 666c  __ref6570_str_fl
-000015b0: 6f61 745f 696e 745f 6578 7061 6e73 696f  oat_int_expansio
-000015c0: 6e28 0a20 2020 2020 2020 2063 6c73 2c0a  n(.        cls,.
-000015d0: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
-000015e0: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
-000015f0: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
-00001600: 696e 672e 416e 792c 0a20 2020 2020 2020  ing.Any,.       
-00001610: 2065 7870 6c6f 6465 3a20 626f 6f6c 2c0a   explode: bool,.
-00001620: 2020 2020 2020 2020 7065 7263 656e 745f          percent_
-00001630: 656e 636f 6465 3a20 626f 6f6c 2c0a 2020  encode: bool,.  
-00001640: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-00001650: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
-00001660: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
-00001670: 4974 6572 6174 6f72 2c0a 2020 2020 2020  Iterator,.      
-00001680: 2020 7661 725f 6e61 6d65 5f70 6965 6365    var_name_piece
-00001690: 3a20 7374 722c 0a20 2020 2020 2020 206e  : str,.        n
-000016a0: 616d 6564 5f70 6172 616d 6574 6572 5f65  amed_parameter_e
-000016b0: 7870 616e 7369 6f6e 3a20 626f 6f6c 0a20  xpansion: bool. 
-000016c0: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
-000016d0: 2020 2020 2069 7465 6d5f 7661 6c75 6520       item_value 
-000016e0: 3d20 636c 732e 5f5f 7265 6636 3537 305f  = cls.__ref6570_
-000016f0: 6974 656d 5f76 616c 7565 2869 6e5f 6461  item_value(in_da
-00001700: 7461 2c20 7065 7263 656e 745f 656e 636f  ta, percent_enco
-00001710: 6465 290a 2020 2020 2020 2020 6966 2069  de).        if i
-00001720: 7465 6d5f 7661 6c75 6520 6973 204e 6f6e  tem_value is Non
-00001730: 6520 6f72 2028 6974 656d 5f76 616c 7565  e or (item_value
-00001740: 203d 3d20 2727 2061 6e64 2070 7265 6669   == '' and prefi
-00001750: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00001760: 6174 6f72 2e73 6570 6172 6174 6f72 203d  ator.separator =
-00001770: 3d20 273b 2729 3a0a 2020 2020 2020 2020  = ';'):.        
-00001780: 2020 2020 7265 7475 726e 206e 6578 7428      return next(
-00001790: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-000017a0: 5f69 7465 7261 746f 7229 202b 2076 6172  _iterator) + var
-000017b0: 5f6e 616d 655f 7069 6563 650a 2020 2020  _name_piece.    
-000017c0: 2020 2020 7661 6c75 655f 7061 6972 5f65      value_pair_e
-000017d0: 7175 616c 7320 3d20 273d 2720 6966 206e  quals = '=' if n
-000017e0: 616d 6564 5f70 6172 616d 6574 6572 5f65  amed_parameter_e
-000017f0: 7870 616e 7369 6f6e 2065 6c73 6520 2727  xpansion else ''
-00001800: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001810: 6e65 7874 2870 7265 6669 785f 7365 7061  next(prefix_sepa
-00001820: 7261 746f 725f 6974 6572 6174 6f72 2920  rator_iterator) 
-00001830: 2b20 7661 725f 6e61 6d65 5f70 6965 6365  + var_name_piece
-00001840: 202b 2076 616c 7565 5f70 6169 725f 6571   + value_pair_eq
-00001850: 7561 6c73 202b 2069 7465 6d5f 7661 6c75  uals + item_valu
-00001860: 650a 0a20 2020 2040 636c 6173 736d 6574  e..    @classmet
-00001870: 686f 640a 2020 2020 6465 6620 5f5f 7265  hod.    def __re
-00001880: 6636 3537 305f 6c69 7374 5f65 7870 616e  f6570_list_expan
-00001890: 7369 6f6e 280a 2020 2020 2020 2020 636c  sion(.        cl
-000018a0: 732c 0a20 2020 2020 2020 2076 6172 6961  s,.        varia
-000018b0: 626c 655f 6e61 6d65 3a20 7374 722c 0a20  ble_name: str,. 
-000018c0: 2020 2020 2020 2069 6e5f 6461 7461 3a20         in_data: 
-000018d0: 7479 7069 6e67 2e41 6e79 2c0a 2020 2020  typing.Any,.    
-000018e0: 2020 2020 6578 706c 6f64 653a 2062 6f6f      explode: boo
-000018f0: 6c2c 0a20 2020 2020 2020 2070 6572 6365  l,.        perce
-00001900: 6e74 5f65 6e63 6f64 653a 2062 6f6f 6c2c  nt_encode: bool,
-00001910: 0a20 2020 2020 2020 2070 7265 6669 785f  .        prefix_
-00001920: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-00001930: 6f72 3a20 5072 6566 6978 5365 7061 7261  or: PrefixSepara
-00001940: 746f 7249 7465 7261 746f 722c 0a20 2020  torIterator,.   
-00001950: 2020 2020 2076 6172 5f6e 616d 655f 7069       var_name_pi
-00001960: 6563 653a 2073 7472 2c0a 2020 2020 2020  ece: str,.      
-00001970: 2020 6e61 6d65 645f 7061 7261 6d65 7465    named_paramete
-00001980: 725f 6578 7061 6e73 696f 6e3a 2062 6f6f  r_expansion: boo
-00001990: 6c0a 2020 2020 2920 2d3e 2073 7472 3a0a  l.    ) -> str:.
-000019a0: 2020 2020 2020 2020 6974 656d 5f76 616c          item_val
-000019b0: 7565 7320 3d20 5b63 6c73 2e5f 5f72 6566  ues = [cls.__ref
-000019c0: 3635 3730 5f69 7465 6d5f 7661 6c75 6528  6570_item_value(
-000019d0: 762c 2070 6572 6365 6e74 5f65 6e63 6f64  v, percent_encod
-000019e0: 6529 2066 6f72 2076 2069 6e20 696e 5f64  e) for v in in_d
-000019f0: 6174 615d 0a20 2020 2020 2020 2069 7465  ata].        ite
-00001a00: 6d5f 7661 6c75 6573 203d 205b 7620 666f  m_values = [v fo
-00001a10: 7220 7620 696e 2069 7465 6d5f 7661 6c75  r v in item_valu
-00001a20: 6573 2069 6620 7620 6973 206e 6f74 204e  es if v is not N
-00001a30: 6f6e 655d 0a20 2020 2020 2020 2069 6620  one].        if 
-00001a40: 6e6f 7420 6974 656d 5f76 616c 7565 733a  not item_values:
-00001a50: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-00001a60: 676e 6f72 6564 2062 7920 7468 6520 6578  gnored by the ex
-00001a70: 7061 6e73 696f 6e20 7072 6f63 6573 7320  pansion process 
-00001a80: 6874 7470 733a 2f2f 6461 7461 7472 6163  https://datatrac
-00001a90: 6b65 722e 6965 7466 2e6f 7267 2f64 6f63  ker.ietf.org/doc
-00001aa0: 2f68 746d 6c2f 7266 6336 3537 3023 7365  /html/rfc6570#se
-00001ab0: 6374 696f 6e2d 332e 322e 310a 2020 2020  ction-3.2.1.    
-00001ac0: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00001ad0: 220a 2020 2020 2020 2020 7661 6c75 655f  ".        value_
-00001ae0: 7061 6972 5f65 7175 616c 7320 3d20 273d  pair_equals = '=
-00001af0: 2720 6966 206e 616d 6564 5f70 6172 616d  ' if named_param
-00001b00: 6574 6572 5f65 7870 616e 7369 6f6e 2065  eter_expansion e
-00001b10: 6c73 6520 2727 0a20 2020 2020 2020 2069  lse ''.        i
-00001b20: 6620 6e6f 7420 6578 706c 6f64 653a 0a20  f not explode:. 
-00001b30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001b40: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-00001b50: 2020 2020 6e65 7874 2870 7265 6669 785f      next(prefix_
-00001b60: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
-00001b70: 6f72 2920 2b0a 2020 2020 2020 2020 2020  or) +.          
-00001b80: 2020 2020 2020 7661 725f 6e61 6d65 5f70        var_name_p
-00001b90: 6965 6365 202b 0a20 2020 2020 2020 2020  iece +.         
-00001ba0: 2020 2020 2020 2076 616c 7565 5f70 6169         value_pai
-00001bb0: 725f 6571 7561 6c73 202b 0a20 2020 2020  r_equals +.     
-00001bc0: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-00001bd0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00001be0: 6174 6f72 2e69 7465 6d5f 7365 7061 7261  ator.item_separa
-00001bf0: 746f 722e 6a6f 696e 2869 7465 6d5f 7661  tor.join(item_va
-00001c00: 6c75 6573 290a 2020 2020 2020 2020 2020  lues).          
-00001c10: 2020 290a 2020 2020 2020 2020 2320 6578    ).        # ex
-00001c20: 706c 6f64 6564 0a20 2020 2020 2020 2072  ploded.        r
-00001c30: 6574 7572 6e20 6e65 7874 2870 7265 6669  eturn next(prefi
-00001c40: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00001c50: 6174 6f72 2920 2b20 6e65 7874 2870 7265  ator) + next(pre
-00001c60: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-00001c70: 6572 6174 6f72 292e 6a6f 696e 280a 2020  erator).join(.  
-00001c80: 2020 2020 2020 2020 2020 5b76 6172 5f6e            [var_n
-00001c90: 616d 655f 7069 6563 6520 2b20 7661 6c75  ame_piece + valu
-00001ca0: 655f 7061 6972 5f65 7175 616c 7320 2b20  e_pair_equals + 
-00001cb0: 7661 6c20 666f 7220 7661 6c20 696e 2069  val for val in i
-00001cc0: 7465 6d5f 7661 6c75 6573 5d0a 2020 2020  tem_values].    
-00001cd0: 2020 2020 290a 0a20 2020 2040 636c 6173      )..    @clas
-00001ce0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00001cf0: 5f5f 7265 6636 3537 305f 6469 6374 5f65  __ref6570_dict_e
-00001d00: 7870 616e 7369 6f6e 280a 2020 2020 2020  xpansion(.      
-00001d10: 2020 636c 732c 0a20 2020 2020 2020 2076    cls,.        v
-00001d20: 6172 6961 626c 655f 6e61 6d65 3a20 7374  ariable_name: st
-00001d30: 722c 0a20 2020 2020 2020 2069 6e5f 6461  r,.        in_da
-00001d40: 7461 3a20 7479 7069 6e67 2e41 6e79 2c0a  ta: typing.Any,.
-00001d50: 2020 2020 2020 2020 6578 706c 6f64 653a          explode:
-00001d60: 2062 6f6f 6c2c 0a20 2020 2020 2020 2070   bool,.        p
-00001d70: 6572 6365 6e74 5f65 6e63 6f64 653a 2062  ercent_encode: b
-00001d80: 6f6f 6c2c 0a20 2020 2020 2020 2070 7265  ool,.        pre
-00001d90: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-00001da0: 6572 6174 6f72 3a20 5072 6566 6978 5365  erator: PrefixSe
-00001db0: 7061 7261 746f 7249 7465 7261 746f 722c  paratorIterator,
-00001dc0: 0a20 2020 2020 2020 2076 6172 5f6e 616d  .        var_nam
-00001dd0: 655f 7069 6563 653a 2073 7472 2c0a 2020  e_piece: str,.  
-00001de0: 2020 2020 2020 6e61 6d65 645f 7061 7261        named_para
-00001df0: 6d65 7465 725f 6578 7061 6e73 696f 6e3a  meter_expansion:
-00001e00: 2062 6f6f 6c0a 2020 2020 2920 2d3e 2073   bool.    ) -> s
-00001e10: 7472 3a0a 2020 2020 2020 2020 696e 5f64  tr:.        in_d
-00001e20: 6174 615f 7472 616e 7366 6f72 6d65 6420  ata_transformed 
-00001e30: 3d20 7b6b 6579 3a20 636c 732e 5f5f 7265  = {key: cls.__re
-00001e40: 6636 3537 305f 6974 656d 5f76 616c 7565  f6570_item_value
-00001e50: 2876 616c 2c20 7065 7263 656e 745f 656e  (val, percent_en
-00001e60: 636f 6465 2920 666f 7220 6b65 792c 2076  code) for key, v
-00001e70: 616c 2069 6e20 696e 5f64 6174 612e 6974  al in in_data.it
-00001e80: 656d 7328 297d 0a20 2020 2020 2020 2069  ems()}.        i
-00001e90: 6e5f 6461 7461 5f74 7261 6e73 666f 726d  n_data_transform
-00001ea0: 6564 203d 207b 6b65 793a 2076 616c 2066  ed = {key: val f
-00001eb0: 6f72 206b 6579 2c20 7661 6c20 696e 2069  or key, val in i
-00001ec0: 6e5f 6461 7461 5f74 7261 6e73 666f 726d  n_data_transform
-00001ed0: 6564 2e69 7465 6d73 2829 2069 6620 7661  ed.items() if va
-00001ee0: 6c20 6973 206e 6f74 204e 6f6e 657d 0a20  l is not None}. 
-00001ef0: 2020 2020 2020 2069 6620 6e6f 7420 696e         if not in
-00001f00: 5f64 6174 615f 7472 616e 7366 6f72 6d65  _data_transforme
-00001f10: 643a 0a20 2020 2020 2020 2020 2020 2023  d:.            #
-00001f20: 2069 676e 6f72 6564 2062 7920 7468 6520   ignored by the 
-00001f30: 6578 7061 6e73 696f 6e20 7072 6f63 6573  expansion proces
-00001f40: 7320 6874 7470 733a 2f2f 6461 7461 7472  s https://datatr
-00001f50: 6163 6b65 722e 6965 7466 2e6f 7267 2f64  acker.ietf.org/d
-00001f60: 6f63 2f68 746d 6c2f 7266 6336 3537 3023  oc/html/rfc6570#
-00001f70: 7365 6374 696f 6e2d 332e 322e 310a 2020  section-3.2.1.  
-00001f80: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001f90: 2022 220a 2020 2020 2020 2020 7661 6c75   "".        valu
-00001fa0: 655f 7061 6972 5f65 7175 616c 7320 3d20  e_pair_equals = 
-00001fb0: 273d 2720 6966 206e 616d 6564 5f70 6172  '=' if named_par
-00001fc0: 616d 6574 6572 5f65 7870 616e 7369 6f6e  ameter_expansion
-00001fd0: 2065 6c73 6520 2727 0a20 2020 2020 2020   else ''.       
-00001fe0: 2069 6620 6e6f 7420 6578 706c 6f64 653a   if not explode:
-00001ff0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00002000: 7572 6e20 280a 2020 2020 2020 2020 2020  urn (.          
-00002010: 2020 2020 2020 6e65 7874 2870 7265 6669        next(prefi
-00002020: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00002030: 6174 6f72 2920 2b0a 2020 2020 2020 2020  ator) +.        
-00002040: 2020 2020 2020 2020 7661 725f 6e61 6d65          var_name
-00002050: 5f70 6965 6365 202b 2076 616c 7565 5f70  _piece + value_p
-00002060: 6169 725f 6571 7561 6c73 202b 0a20 2020  air_equals +.   
-00002070: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-00002080: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-00002090: 6572 6174 6f72 2e69 7465 6d5f 7365 7061  erator.item_sepa
-000020a0: 7261 746f 722e 6a6f 696e 280a 2020 2020  rator.join(.    
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-000020d0: 5f69 7465 7261 746f 722e 6974 656d 5f73  _iterator.item_s
-000020e0: 6570 6172 6174 6f72 2e6a 6f69 6e28 0a20  eparator.join(. 
-000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002100: 2020 2020 2020 2069 7465 6d5f 7061 6972         item_pair
-00002110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002120: 2020 2020 2029 2066 6f72 2069 7465 6d5f       ) for item_
-00002130: 7061 6972 2069 6e20 696e 5f64 6174 615f  pair in in_data_
-00002140: 7472 616e 7366 6f72 6d65 642e 6974 656d  transformed.item
-00002150: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00002160: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00002170: 2020 290a 2020 2020 2020 2020 2320 6578    ).        # ex
-00002180: 706c 6f64 6564 0a20 2020 2020 2020 2072  ploded.        r
-00002190: 6574 7572 6e20 6e65 7874 2870 7265 6669  eturn next(prefi
-000021a0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-000021b0: 6174 6f72 2920 2b20 6e65 7874 2870 7265  ator) + next(pre
-000021c0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-000021d0: 6572 6174 6f72 292e 6a6f 696e 280a 2020  erator).join(.  
-000021e0: 2020 2020 2020 2020 2020 5b6b 6579 202b            [key +
-000021f0: 2027 3d27 202b 2076 616c 2066 6f72 206b   '=' + val for k
-00002200: 6579 2c20 7661 6c20 696e 2069 6e5f 6461  ey, val in in_da
-00002210: 7461 5f74 7261 6e73 666f 726d 6564 2e69  ta_transformed.i
-00002220: 7465 6d73 2829 5d0a 2020 2020 2020 2020  tems()].        
-00002230: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-00002240: 686f 640a 2020 2020 6465 6620 5f72 6566  hod.    def _ref
-00002250: 3635 3730 5f65 7870 616e 7369 6f6e 280a  6570_expansion(.
-00002260: 2020 2020 2020 2020 636c 732c 0a20 2020          cls,.   
-00002270: 2020 2020 2076 6172 6961 626c 655f 6e61       variable_na
-00002280: 6d65 3a20 7374 722c 0a20 2020 2020 2020  me: str,.       
-00002290: 2069 6e5f 6461 7461 3a20 7479 7069 6e67   in_data: typing
-000022a0: 2e41 6e79 2c0a 2020 2020 2020 2020 6578  .Any,.        ex
-000022b0: 706c 6f64 653a 2062 6f6f 6c2c 0a20 2020  plode: bool,.   
-000022c0: 2020 2020 2070 6572 6365 6e74 5f65 6e63       percent_enc
-000022d0: 6f64 653a 2062 6f6f 6c2c 0a20 2020 2020  ode: bool,.     
-000022e0: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-000022f0: 746f 725f 6974 6572 6174 6f72 3a20 5072  tor_iterator: Pr
-00002300: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
-00002310: 7261 746f 720a 2020 2020 2920 2d3e 2073  rator.    ) -> s
-00002320: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
-00002330: 2020 2020 2020 2020 5365 7061 7261 746f          Separato
-00002340: 7220 6973 2066 6f72 2073 6570 6172 6174  r is for separat
-00002350: 6520 7661 7269 6162 6c65 7320 6c69 6b65  e variables like
-00002360: 2064 6963 7420 7769 7468 2065 7870 6c6f   dict with explo
-00002370: 6465 2074 7275 652c 206e 6f74 2066 6f72  de true, not for
-00002380: 2061 7272 6179 2069 7465 6d20 7365 7061   array item sepa
-00002390: 7261 7469 6f6e 0a20 2020 2020 2020 2022  ration.        "
-000023a0: 2222 0a20 2020 2020 2020 206e 616d 6564  "".        named
-000023b0: 5f70 6172 616d 6574 6572 5f65 7870 616e  _parameter_expan
-000023c0: 7369 6f6e 203d 2070 7265 6669 785f 7365  sion = prefix_se
-000023d0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-000023e0: 2e73 6570 6172 6174 6f72 2069 6e20 7b27  .separator in {'
-000023f0: 2627 2c20 273b 277d 0a20 2020 2020 2020  &', ';'}.       
-00002400: 2076 6172 5f6e 616d 655f 7069 6563 6520   var_name_piece 
-00002410: 3d20 7661 7269 6162 6c65 5f6e 616d 6520  = variable_name 
-00002420: 6966 206e 616d 6564 5f70 6172 616d 6574  if named_paramet
-00002430: 6572 5f65 7870 616e 7369 6f6e 2065 6c73  er_expansion els
-00002440: 6520 2727 0a20 2020 2020 2020 2069 6620  e ''.        if 
-00002450: 7479 7065 2869 6e5f 6461 7461 2920 696e  type(in_data) in
-00002460: 207b 7374 722c 2066 6c6f 6174 2c20 696e   {str, float, in
-00002470: 747d 3a0a 2020 2020 2020 2020 2020 2020  t}:.            
-00002480: 7265 7475 726e 2063 6c73 2e5f 5f72 6566  return cls.__ref
-00002490: 3635 3730 5f73 7472 5f66 6c6f 6174 5f69  6570_str_float_i
-000024a0: 6e74 5f65 7870 616e 7369 6f6e 280a 2020  nt_expansion(.  
-000024b0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-000024c0: 7269 6162 6c65 5f6e 616d 652c 0a20 2020  riable_name,.   
-000024d0: 2020 2020 2020 2020 2020 2020 2069 6e5f               in_
-000024e0: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-000024f0: 2020 2020 2020 6578 706c 6f64 652c 0a20        explode,. 
-00002500: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002510: 6572 6365 6e74 5f65 6e63 6f64 652c 0a20  ercent_encode,. 
-00002520: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002530: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00002540: 6974 6572 6174 6f72 2c0a 2020 2020 2020  iterator,.      
-00002550: 2020 2020 2020 2020 2020 7661 725f 6e61            var_na
-00002560: 6d65 5f70 6965 6365 2c0a 2020 2020 2020  me_piece,.      
-00002570: 2020 2020 2020 2020 2020 6e61 6d65 645f            named_
-00002580: 7061 7261 6d65 7465 725f 6578 7061 6e73  parameter_expans
-00002590: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000025a0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
-000025b0: 7369 6e73 7461 6e63 6528 696e 5f64 6174  sinstance(in_dat
-000025c0: 612c 206e 6f6e 655f 7479 7065 293a 0a20  a, none_type):. 
-000025d0: 2020 2020 2020 2020 2020 2023 2069 676e             # ign
-000025e0: 6f72 6564 2062 7920 7468 6520 6578 7061  ored by the expa
-000025f0: 6e73 696f 6e20 7072 6f63 6573 7320 6874  nsion process ht
-00002600: 7470 733a 2f2f 6461 7461 7472 6163 6b65  tps://datatracke
-00002610: 722e 6965 7466 2e6f 7267 2f64 6f63 2f68  r.ietf.org/doc/h
-00002620: 746d 6c2f 7266 6336 3537 3023 7365 6374  tml/rfc6570#sect
-00002630: 696f 6e2d 332e 322e 310a 2020 2020 2020  ion-3.2.1.      
-00002640: 2020 2020 2020 7265 7475 726e 2022 220a        return "".
-00002650: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
-00002660: 6e73 7461 6e63 6528 696e 5f64 6174 612c  nstance(in_data,
-00002670: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
-00002680: 2020 2020 7265 7475 726e 2063 6c73 2e5f      return cls._
-00002690: 5f72 6566 3635 3730 5f6c 6973 745f 6578  _ref6570_list_ex
-000026a0: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
-000026b0: 2020 2020 2020 2020 2076 6172 6961 626c           variabl
-000026c0: 655f 6e61 6d65 2c0a 2020 2020 2020 2020  e_name,.        
-000026d0: 2020 2020 2020 2020 696e 5f64 6174 612c          in_data,
-000026e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000026f0: 2065 7870 6c6f 6465 2c0a 2020 2020 2020   explode,.      
-00002700: 2020 2020 2020 2020 2020 7065 7263 656e            percen
-00002710: 745f 656e 636f 6465 2c0a 2020 2020 2020  t_encode,.      
-00002720: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00002730: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00002740: 746f 722c 0a20 2020 2020 2020 2020 2020  tor,.           
-00002750: 2020 2020 2076 6172 5f6e 616d 655f 7069       var_name_pi
-00002760: 6563 652c 0a20 2020 2020 2020 2020 2020  ece,.           
-00002770: 2020 2020 206e 616d 6564 5f70 6172 616d       named_param
-00002780: 6574 6572 5f65 7870 616e 7369 6f6e 0a20  eter_expansion. 
-00002790: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000027a0: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
-000027b0: 616e 6365 2869 6e5f 6461 7461 2c20 6469  ance(in_data, di
-000027c0: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
-000027d0: 2072 6574 7572 6e20 636c 732e 5f5f 7265   return cls.__re
-000027e0: 6636 3537 305f 6469 6374 5f65 7870 616e  f6570_dict_expan
-000027f0: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
-00002800: 2020 2020 2020 7661 7269 6162 6c65 5f6e        variable_n
-00002810: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00002820: 2020 2020 2069 6e5f 6461 7461 2c0a 2020       in_data,.  
-00002830: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00002840: 706c 6f64 652c 0a20 2020 2020 2020 2020  plode,.         
-00002850: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
-00002860: 6e63 6f64 652c 0a20 2020 2020 2020 2020  ncode,.         
-00002870: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
-00002880: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-00002890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000028a0: 2020 7661 725f 6e61 6d65 5f70 6965 6365    var_name_piece
-000028b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000028c0: 2020 6e61 6d65 645f 7061 7261 6d65 7465    named_paramete
-000028d0: 725f 6578 7061 6e73 696f 6e0a 2020 2020  r_expansion.    
-000028e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000028f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-00002900: 6528 696e 5f64 6174 612c 2062 6f6f 6c29  e(in_data, bool)
-00002910: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00002920: 7475 726e 2063 6c73 2e5f 5f6b 6f6e 6669  turn cls.__konfi
-00002930: 675f 626f 6f6c 5f65 7870 616e 7369 6f6e  g_bool_expansion
-00002940: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00002950: 2020 696e 5f64 6174 612c 0a20 2020 2020    in_data,.     
-00002960: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-00002970: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00002980: 6174 6f72 2c0a 2020 2020 2020 2020 2020  ator,.          
-00002990: 2020 2020 2020 7661 725f 6e61 6d65 5f70        var_name_p
-000029a0: 6965 6365 2c0a 2020 2020 2020 2020 2020  iece,.          
-000029b0: 2020 2020 2020 6e61 6d65 645f 7061 7261        named_para
-000029c0: 6d65 7465 725f 6578 7061 6e73 696f 6e0a  meter_expansion.
-000029d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000029e0: 2020 2020 2020 2320 6279 7465 732c 2065        # bytes, e
-000029f0: 7463 0a20 2020 2020 2020 2072 6169 7365  tc.        raise
-00002a00: 2041 7069 5661 6c75 6545 7272 6f72 2827   ApiValueError('
-00002a10: 556e 6162 6c65 2074 6f20 6765 6e65 7261  Unable to genera
-00002a20: 7465 2061 2072 6566 3635 3730 2072 6570  te a ref6570 rep
-00002a30: 7265 7365 6e74 6174 696f 6e20 6f66 207b  resentation of {
-00002a40: 7d27 2e66 6f72 6d61 7428 696e 5f64 6174  }'.format(in_dat
-00002a50: 6129 290a 0a0a 636c 6173 7320 5374 796c  a))...class Styl
-00002a60: 6546 6f72 6d53 6572 6961 6c69 7a65 7228  eFormSerializer(
-00002a70: 5061 7261 6d65 7465 7253 6572 6961 6c69  ParameterSeriali
-00002a80: 7a65 7242 6173 6529 3a0a 2020 2020 4063  zerBase):.    @c
-00002a90: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00002aa0: 6566 205f 6765 745f 6465 6661 756c 745f  ef _get_default_
-00002ab0: 6578 706c 6f64 6528 636c 732c 2073 7479  explode(cls, sty
-00002ac0: 6c65 3a20 5061 7261 6d65 7465 7253 7479  le: ParameterSty
-00002ad0: 6c65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  le) -> bool:.   
-00002ae0: 2020 2020 2069 6620 7374 796c 6520 6973       if style is
-00002af0: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
-00002b00: 464f 524d 3a0a 2020 2020 2020 2020 2020  FORM:.          
-00002b10: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-00002b20: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-00002b30: 6572 2829 2e5f 6765 745f 6465 6661 756c  er()._get_defaul
-00002b40: 745f 6578 706c 6f64 6528 7374 796c 6529  t_explode(style)
-00002b50: 0a0a 2020 2020 6465 6620 5f73 6572 6961  ..    def _seria
-00002b60: 6c69 7a65 5f66 6f72 6d28 0a20 2020 2020  lize_form(.     
-00002b70: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00002b80: 2069 6e5f 6461 7461 3a20 7479 7069 6e67   in_data: typing
-00002b90: 2e55 6e69 6f6e 5b4e 6f6e 652c 2069 6e74  .Union[None, int
-00002ba0: 2c20 666c 6f61 742c 2073 7472 2c20 626f  , float, str, bo
-00002bb0: 6f6c 2c20 6469 6374 2c20 6c69 7374 5d2c  ol, dict, list],
-00002bc0: 0a20 2020 2020 2020 206e 616d 653a 2073  .        name: s
-00002bd0: 7472 2c0a 2020 2020 2020 2020 6578 706c  tr,.        expl
-00002be0: 6f64 653a 2062 6f6f 6c2c 0a20 2020 2020  ode: bool,.     
-00002bf0: 2020 2070 6572 6365 6e74 5f65 6e63 6f64     percent_encod
-00002c00: 653a 2062 6f6f 6c2c 0a20 2020 2020 2020  e: bool,.       
-00002c10: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00002c20: 725f 6974 6572 6174 6f72 3a20 7479 7069  r_iterator: typi
-00002c30: 6e67 2e4f 7074 696f 6e61 6c5b 5072 6566  ng.Optional[Pref
-00002c40: 6978 5365 7061 7261 746f 7249 7465 7261  ixSeparatorItera
-00002c50: 746f 725d 203d 204e 6f6e 650a 2020 2020  tor] = None.    
-00002c60: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00002c70: 2020 6966 2070 7265 6669 785f 7365 7061    if prefix_sepa
-00002c80: 7261 746f 725f 6974 6572 6174 6f72 2069  rator_iterator i
-00002c90: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00002ca0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
-00002cb0: 6174 6f72 5f69 7465 7261 746f 7220 3d20  ator_iterator = 
-00002cc0: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
-00002cd0: 7465 7261 746f 7228 2727 2c20 2726 2729  terator('', '&')
-00002ce0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002cf0: 7365 6c66 2e5f 7265 6636 3537 305f 6578  self._ref6570_ex
-00002d00: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
-00002d10: 2020 2020 2076 6172 6961 626c 655f 6e61       variable_na
-00002d20: 6d65 3d6e 616d 652c 0a20 2020 2020 2020  me=name,.       
-00002d30: 2020 2020 2069 6e5f 6461 7461 3d69 6e5f       in_data=in_
-00002d40: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
-00002d50: 2020 6578 706c 6f64 653d 6578 706c 6f64    explode=explod
-00002d60: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
-00002d70: 6572 6365 6e74 5f65 6e63 6f64 653d 7065  ercent_encode=pe
-00002d80: 7263 656e 745f 656e 636f 6465 2c0a 2020  rcent_encode,.  
-00002d90: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00002da0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00002db0: 746f 723d 7072 6566 6978 5f73 6570 6172  tor=prefix_separ
-00002dc0: 6174 6f72 5f69 7465 7261 746f 720a 2020  ator_iterator.  
-00002dd0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-00002de0: 5374 796c 6553 696d 706c 6553 6572 6961  StyleSimpleSeria
-00002df0: 6c69 7a65 7228 5061 7261 6d65 7465 7253  lizer(ParameterS
-00002e00: 6572 6961 6c69 7a65 7242 6173 6529 3a0a  erializerBase):.
-00002e10: 0a20 2020 2064 6566 205f 7365 7269 616c  .    def _serial
-00002e20: 697a 655f 7369 6d70 6c65 280a 2020 2020  ize_simple(.    
-00002e30: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00002e40: 2020 696e 5f64 6174 613a 2074 7970 696e    in_data: typin
-00002e50: 672e 556e 696f 6e5b 4e6f 6e65 2c20 696e  g.Union[None, in
-00002e60: 742c 2066 6c6f 6174 2c20 7374 722c 2062  t, float, str, b
-00002e70: 6f6f 6c2c 2064 6963 742c 206c 6973 745d  ool, dict, list]
-00002e80: 2c0a 2020 2020 2020 2020 6e61 6d65 3a20  ,.        name: 
-00002e90: 7374 722c 0a20 2020 2020 2020 2065 7870  str,.        exp
-00002ea0: 6c6f 6465 3a20 626f 6f6c 2c0a 2020 2020  lode: bool,.    
-00002eb0: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
-00002ec0: 6465 3a20 626f 6f6c 0a20 2020 2029 202d  de: bool.    ) -
-00002ed0: 3e20 7374 723a 0a20 2020 2020 2020 2070  > str:.        p
-00002ee0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00002ef0: 6974 6572 6174 6f72 203d 2050 7265 6669  iterator = Prefi
-00002f00: 7853 6570 6172 6174 6f72 4974 6572 6174  xSeparatorIterat
-00002f10: 6f72 2827 272c 2027 2c27 290a 2020 2020  or('', ',').    
-00002f20: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002f30: 5f72 6566 3635 3730 5f65 7870 616e 7369  _ref6570_expansi
-00002f40: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
-00002f50: 7661 7269 6162 6c65 5f6e 616d 653d 6e61  variable_name=na
-00002f60: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00002f70: 696e 5f64 6174 613d 696e 5f64 6174 612c  in_data=in_data,
-00002f80: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
-00002f90: 6c6f 6465 3d65 7870 6c6f 6465 2c0a 2020  lode=explode,.  
-00002fa0: 2020 2020 2020 2020 2020 7065 7263 656e            percen
-00002fb0: 745f 656e 636f 6465 3d70 6572 6365 6e74  t_encode=percent
-00002fc0: 5f65 6e63 6f64 652c 0a20 2020 2020 2020  _encode,.       
-00002fd0: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-00002fe0: 7261 746f 725f 6974 6572 6174 6f72 3d70  rator_iterator=p
-00002ff0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00003000: 6974 6572 6174 6f72 0a20 2020 2020 2020  iterator.       
-00003010: 2029 0a0a 0a63 6c61 7373 204a 534f 4e44   )...class JSOND
-00003020: 6574 6563 746f 723a 0a20 2020 2022 2222  etector:.    """
-00003030: 0a20 2020 2057 6f72 6b73 2066 6f72 3a0a  .    Works for:.
-00003040: 2020 2020 6170 706c 6963 6174 696f 6e2f      application/
-00003050: 6a73 6f6e 0a20 2020 2061 7070 6c69 6361  json.    applica
-00003060: 7469 6f6e 2f6a 736f 6e3b 2063 6861 7273  tion/json; chars
-00003070: 6574 3d55 5446 2d38 0a20 2020 2061 7070  et=UTF-8.    app
-00003080: 6c69 6361 7469 6f6e 2f6a 736f 6e2d 7061  lication/json-pa
-00003090: 7463 682b 6a73 6f6e 0a20 2020 2061 7070  tch+json.    app
-000030a0: 6c69 6361 7469 6f6e 2f67 656f 2b6a 736f  lication/geo+jso
-000030b0: 6e0a 2020 2020 2222 220a 2020 2020 5f5f  n.    """.    __
-000030c0: 6a73 6f6e 5f63 6f6e 7465 6e74 5f74 7970  json_content_typ
-000030d0: 655f 7061 7474 6572 6e20 3d20 7265 2e63  e_pattern = re.c
-000030e0: 6f6d 7069 6c65 2822 6170 706c 6963 6174  ompile("applicat
-000030f0: 696f 6e2f 5b5e 2b5d 2a5b 2b5d 3f28 6a73  ion/[^+]*[+]?(js
-00003100: 6f6e 293b 3f2e 2a22 290a 0a20 2020 2040  on);?.*")..    @
-00003110: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00003120: 6465 6620 5f63 6f6e 7465 6e74 5f74 7970  def _content_typ
-00003130: 655f 6973 5f6a 736f 6e28 636c 732c 2063  e_is_json(cls, c
-00003140: 6f6e 7465 6e74 5f74 7970 653a 2073 7472  ontent_type: str
-00003150: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00003160: 2020 2069 6620 636c 732e 5f5f 6a73 6f6e     if cls.__json
-00003170: 5f63 6f6e 7465 6e74 5f74 7970 655f 7061  _content_type_pa
-00003180: 7474 6572 6e2e 6d61 7463 6828 636f 6e74  ttern.match(cont
-00003190: 656e 745f 7479 7065 293a 0a20 2020 2020  ent_type):.     
-000031a0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000031b0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-000031c0: 6e20 4661 6c73 650a 0a0a 4064 6174 6163  n False...@datac
-000031d0: 6c61 7373 0a63 6c61 7373 2050 6172 616d  lass.class Param
-000031e0: 6574 6572 4261 7365 284a 534f 4e44 6574  eterBase(JSONDet
-000031f0: 6563 746f 7229 3a0a 2020 2020 6e61 6d65  ector):.    name
-00003200: 3a20 7374 720a 2020 2020 696e 5f74 7970  : str.    in_typ
-00003210: 653a 2050 6172 616d 6574 6572 496e 5479  e: ParameterInTy
-00003220: 7065 0a20 2020 2072 6571 7569 7265 643a  pe.    required:
-00003230: 2062 6f6f 6c0a 2020 2020 7374 796c 653a   bool.    style:
-00003240: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00003250: 5b50 6172 616d 6574 6572 5374 796c 655d  [ParameterStyle]
-00003260: 0a20 2020 2065 7870 6c6f 6465 3a20 7479  .    explode: ty
-00003270: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
-00003280: 6f6c 5d0a 2020 2020 616c 6c6f 775f 7265  ol].    allow_re
-00003290: 7365 7276 6564 3a20 7479 7069 6e67 2e4f  served: typing.O
-000032a0: 7074 696f 6e61 6c5b 626f 6f6c 5d0a 2020  ptional[bool].  
-000032b0: 2020 7363 6865 6d61 3a20 7479 7069 6e67    schema: typing
-000032c0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-000032d0: 2e54 7970 655b 5363 6865 6d61 5d5d 0a20  .Type[Schema]]. 
-000032e0: 2020 2063 6f6e 7465 6e74 3a20 7479 7069     content: typi
-000032f0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00003300: 6e67 2e44 6963 745b 7374 722c 2074 7970  ng.Dict[str, typ
-00003310: 696e 672e 5479 7065 5b53 6368 656d 615d  ing.Type[Schema]
-00003320: 5d5d 0a0a 2020 2020 5f5f 7374 796c 655f  ]]..    __style_
-00003330: 746f 5f69 6e5f 7479 7065 203d 207b 0a20  to_in_type = {. 
-00003340: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00003350: 5374 796c 652e 4d41 5452 4958 3a20 7b50  Style.MATRIX: {P
-00003360: 6172 616d 6574 6572 496e 5479 7065 2e50  arameterInType.P
-00003370: 4154 487d 2c0a 2020 2020 2020 2020 5061  ATH},.        Pa
-00003380: 7261 6d65 7465 7253 7479 6c65 2e4c 4142  rameterStyle.LAB
-00003390: 454c 3a20 7b50 6172 616d 6574 6572 496e  EL: {ParameterIn
-000033a0: 5479 7065 2e50 4154 487d 2c0a 2020 2020  Type.PATH},.    
-000033b0: 2020 2020 5061 7261 6d65 7465 7253 7479      ParameterSty
-000033c0: 6c65 2e46 4f52 4d3a 207b 5061 7261 6d65  le.FORM: {Parame
-000033d0: 7465 7249 6e54 7970 652e 5155 4552 592c  terInType.QUERY,
-000033e0: 2050 6172 616d 6574 6572 496e 5479 7065   ParameterInType
-000033f0: 2e43 4f4f 4b49 457d 2c0a 2020 2020 2020  .COOKIE},.      
-00003400: 2020 5061 7261 6d65 7465 7253 7479 6c65    ParameterStyle
-00003410: 2e53 494d 504c 453a 207b 5061 7261 6d65  .SIMPLE: {Parame
-00003420: 7465 7249 6e54 7970 652e 5041 5448 2c20  terInType.PATH, 
-00003430: 5061 7261 6d65 7465 7249 6e54 7970 652e  ParameterInType.
-00003440: 4845 4144 4552 7d2c 0a20 2020 2020 2020  HEADER},.       
-00003450: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
-00003460: 5350 4143 455f 4445 4c49 4d49 5445 443a  SPACE_DELIMITED:
-00003470: 207b 5061 7261 6d65 7465 7249 6e54 7970   {ParameterInTyp
-00003480: 652e 5155 4552 597d 2c0a 2020 2020 2020  e.QUERY},.      
-00003490: 2020 5061 7261 6d65 7465 7253 7479 6c65    ParameterStyle
-000034a0: 2e50 4950 455f 4445 4c49 4d49 5445 443a  .PIPE_DELIMITED:
+00000180: 6669 6c65 0a69 6d70 6f72 7420 7469 6d65  file.import time
+00000190: 0a69 6d70 6f72 7420 7479 7069 6e67 0a69  .import typing.i
+000001a0: 6d70 6f72 7420 7479 7069 6e67 5f65 7874  mport typing_ext
+000001b0: 656e 7369 6f6e 730a 696d 706f 7274 2061  ensions.import a
+000001c0: 696f 6874 7470 0a69 6d70 6f72 7420 7572  iohttp.import ur
+000001d0: 6c6c 6962 330a 6672 6f6d 2075 726c 6c69  llib3.from urlli
+000001e0: 6233 2e5f 636f 6c6c 6563 7469 6f6e 7320  b3._collections 
+000001f0: 696d 706f 7274 2048 5454 5048 6561 6465  import HTTPHeade
+00000200: 7244 6963 740a 6672 6f6d 2075 726c 6c69  rDict.from urlli
+00000210: 622e 7061 7273 6520 696d 706f 7274 2075  b.parse import u
+00000220: 726c 7061 7273 652c 2071 756f 7465 0a66  rlparse, quote.f
+00000230: 726f 6d20 7572 6c6c 6962 332e 6669 656c  rom urllib3.fiel
+00000240: 6473 2069 6d70 6f72 7420 5265 7175 6573  ds import Reques
+00000250: 7446 6965 6c64 2061 7320 5265 7175 6573  tField as Reques
+00000260: 7446 6965 6c64 4261 7365 0a66 726f 6d20  tFieldBase.from 
+00000270: 7572 6c6c 6962 332e 6669 656c 6473 2069  urllib3.fields i
+00000280: 6d70 6f72 7420 6775 6573 735f 636f 6e74  mport guess_cont
+00000290: 656e 745f 7479 7065 0a0a 696d 706f 7274  ent_type..import
+000002a0: 2066 726f 7a65 6e64 6963 740a 0a66 726f   frozendict..fro
+000002b0: 6d20 6465 6365 6e74 726f 5f69 6e5f 6b79  m decentro_in_ky
+000002c0: 635f 636c 6965 6e74 2069 6d70 6f72 7420  c_client import 
+000002d0: 7265 7374 0a66 726f 6d20 6465 6365 6e74  rest.from decent
+000002e0: 726f 5f69 6e5f 6b79 635f 636c 6965 6e74  ro_in_kyc_client
+000002f0: 2e61 7069 5f72 6573 706f 6e73 6520 696d  .api_response im
+00000300: 706f 7274 2041 7069 5265 7370 6f6e 7365  port ApiResponse
+00000310: 2c20 4173 796e 6341 7069 5265 7370 6f6e  , AsyncApiRespon
+00000320: 7365 0a66 726f 6d20 6465 6365 6e74 726f  se.from decentro
+00000330: 5f69 6e5f 6b79 635f 636c 6965 6e74 2e72  _in_kyc_client.r
+00000340: 6573 7420 696d 706f 7274 2041 7379 6e63  est import Async
+00000350: 5265 7370 6f6e 7365 5772 6170 7065 722c  ResponseWrapper,
+00000360: 2052 6573 706f 6e73 6557 7261 7070 6572   ResponseWrapper
+00000370: 0a66 726f 6d20 6465 6365 6e74 726f 5f69  .from decentro_i
+00000380: 6e5f 6b79 635f 636c 6965 6e74 2e63 6f6e  n_kyc_client.con
+00000390: 6669 6775 7261 7469 6f6e 2069 6d70 6f72  figuration impor
+000003a0: 7420 436f 6e66 6967 7572 6174 696f 6e0a  t Configuration.
+000003b0: 6672 6f6d 2064 6563 656e 7472 6f5f 696e  from decentro_in
+000003c0: 5f6b 7963 5f63 6c69 656e 742e 6578 6365  _kyc_client.exce
+000003d0: 7074 696f 6e73 2069 6d70 6f72 7420 4170  ptions import Ap
+000003e0: 6954 7970 6545 7272 6f72 2c20 4170 6956  iTypeError, ApiV
+000003f0: 616c 7565 4572 726f 722c 204d 6973 7369  alueError, Missi
+00000400: 6e67 5265 7175 6972 6564 5061 7261 6d65  ngRequiredParame
+00000410: 7465 7273 4572 726f 720a 6672 6f6d 2064  tersError.from d
+00000420: 6563 656e 7472 6f5f 696e 5f6b 7963 5f63  ecentro_in_kyc_c
+00000430: 6c69 656e 742e 7265 7175 6573 745f 6166  lient.request_af
+00000440: 7465 725f 686f 6f6b 2069 6d70 6f72 7420  ter_hook import 
+00000450: 7265 7175 6573 745f 6166 7465 725f 686f  request_after_ho
+00000460: 6f6b 0a66 726f 6d20 6465 6365 6e74 726f  ok.from decentro
+00000470: 5f69 6e5f 6b79 635f 636c 6965 6e74 2e72  _in_kyc_client.r
+00000480: 6571 7565 7374 5f62 6566 6f72 655f 686f  equest_before_ho
+00000490: 6f6b 2069 6d70 6f72 7420 7265 7175 6573  ok import reques
+000004a0: 745f 6265 666f 7265 5f68 6f6f 6b0a 6672  t_before_hook.fr
+000004b0: 6f6d 2064 6563 656e 7472 6f5f 696e 5f6b  om decentro_in_k
+000004c0: 7963 5f63 6c69 656e 742e 7363 6865 6d61  yc_client.schema
+000004d0: 7320 696d 706f 7274 2028 0a20 2020 204e  s import (.    N
+000004e0: 6f6e 6543 6c61 7373 2c0a 2020 2020 426f  oneClass,.    Bo
+000004f0: 6f6c 436c 6173 732c 0a20 2020 2053 6368  olClass,.    Sch
+00000500: 656d 612c 0a20 2020 2046 696c 6549 4f2c  ema,.    FileIO,
+00000510: 0a20 2020 2042 696e 6172 7953 6368 656d  .    BinarySchem
+00000520: 612c 0a20 2020 2064 6174 652c 0a20 2020  a,.    date,.   
+00000530: 2064 6174 6574 696d 652c 0a20 2020 206e   datetime,.    n
+00000540: 6f6e 655f 7479 7065 2c0a 2020 2020 556e  one_type,.    Un
+00000550: 7365 742c 0a20 2020 2075 6e73 6574 2c0a  set,.    unset,.
+00000560: 290a 0a40 6461 7461 636c 6173 730a 636c  )..@dataclass.cl
+00000570: 6173 7320 4d61 7070 6564 4172 6773 3a0a  ass MappedArgs:.
+00000580: 2020 2020 626f 6479 3a20 7479 7069 6e67      body: typing
+00000590: 2e41 6e79 203d 204e 6f6e 650a 2020 2020  .Any = None.    
+000005a0: 7175 6572 793a 2074 7970 696e 672e 4f70  query: typing.Op
+000005b0: 7469 6f6e 616c 5b64 6963 745d 203d 204e  tional[dict] = N
+000005c0: 6f6e 650a 2020 2020 7061 7468 3a20 7479  one.    path: ty
+000005d0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 6469  ping.Optional[di
+000005e0: 6374 5d20 3d20 4e6f 6e65 0a20 2020 2068  ct] = None.    h
+000005f0: 6561 6465 723a 2074 7970 696e 672e 4f70  eader: typing.Op
+00000600: 7469 6f6e 616c 5b64 6963 745d 203d 204e  tional[dict] = N
+00000610: 6f6e 650a 2020 2020 636f 6f6b 6965 3a20  one.    cookie: 
+00000620: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00000630: 6469 6374 5d20 3d20 4e6f 6e65 0a0a 636c  dict] = None..cl
+00000640: 6173 7320 5265 7175 6573 7446 6965 6c64  ass RequestField
+00000650: 2852 6571 7565 7374 4669 656c 6442 6173  (RequestFieldBas
+00000660: 6529 3a0a 2020 2020 6465 6620 5f5f 6571  e):.    def __eq
+00000670: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+00000680: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00000690: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+000006a0: 2c20 5265 7175 6573 7446 6965 6c64 293a  , RequestField):
+000006b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000006c0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+000006d0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+000006e0: 6469 6374 5f5f 203d 3d20 6f74 6865 722e  dict__ == other.
+000006f0: 5f5f 6469 6374 5f5f 0a0a 0a63 6c61 7373  __dict__...class
+00000700: 204a 534f 4e45 6e63 6f64 6572 286a 736f   JSONEncoder(jso
+00000710: 6e2e 4a53 4f4e 456e 636f 6465 7229 3a0a  n.JSONEncoder):.
+00000720: 2020 2020 636f 6d70 6163 745f 7365 7061      compact_sepa
+00000730: 7261 746f 7273 203d 2028 272c 272c 2027  rators = (',', '
+00000740: 3a27 290a 0a20 2020 2064 6566 2064 6566  :')..    def def
+00000750: 6175 6c74 2873 656c 662c 206f 626a 293a  ault(self, obj):
+00000760: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00000770: 7374 616e 6365 286f 626a 2c20 7374 7229  stance(obj, str)
+00000780: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00000790: 7475 726e 2073 7472 286f 626a 290a 2020  turn str(obj).  
+000007a0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+000007b0: 7461 6e63 6528 6f62 6a2c 2066 6c6f 6174  tance(obj, float
+000007c0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
+000007d0: 6574 7572 6e20 666c 6f61 7428 6f62 6a29  eturn float(obj)
+000007e0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
+000007f0: 696e 7374 616e 6365 286f 626a 2c20 696e  instance(obj, in
+00000800: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00000810: 7265 7475 726e 2069 6e74 286f 626a 290a  return int(obj).
+00000820: 2020 2020 2020 2020 656c 6966 2069 7369          elif isi
+00000830: 6e73 7461 6e63 6528 6f62 6a2c 2044 6563  nstance(obj, Dec
+00000840: 696d 616c 293a 0a20 2020 2020 2020 2020  imal):.         
+00000850: 2020 2069 6620 6f62 6a2e 6173 5f74 7570     if obj.as_tup
+00000860: 6c65 2829 2e65 7870 6f6e 656e 7420 3e3d  le().exponent >=
+00000870: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00000880: 2020 2020 7265 7475 726e 2069 6e74 286f      return int(o
+00000890: 626a 290a 2020 2020 2020 2020 2020 2020  bj).            
+000008a0: 7265 7475 726e 2066 6c6f 6174 286f 626a  return float(obj
+000008b0: 290a 2020 2020 2020 2020 656c 6966 2069  ).        elif i
+000008c0: 7369 6e73 7461 6e63 6528 6f62 6a2c 204e  sinstance(obj, N
+000008d0: 6f6e 6543 6c61 7373 293a 0a20 2020 2020  oneClass):.     
+000008e0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000008f0: 6e65 0a20 2020 2020 2020 2065 6c69 6620  ne.        elif 
+00000900: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
+00000910: 426f 6f6c 436c 6173 7329 3a0a 2020 2020  BoolClass):.    
+00000920: 2020 2020 2020 2020 7265 7475 726e 2062          return b
+00000930: 6f6f 6c28 6f62 6a29 0a20 2020 2020 2020  ool(obj).       
+00000940: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00000950: 286f 626a 2c20 2864 6963 742c 2066 726f  (obj, (dict, fro
+00000960: 7a65 6e64 6963 742e 6672 6f7a 656e 6469  zendict.frozendi
+00000970: 6374 2929 3a0a 2020 2020 2020 2020 2020  ct)):.          
+00000980: 2020 7265 7475 726e 207b 6b65 793a 2073    return {key: s
+00000990: 656c 662e 6465 6661 756c 7428 7661 6c29  elf.default(val)
+000009a0: 2066 6f72 206b 6579 2c20 7661 6c20 696e   for key, val in
+000009b0: 206f 626a 2e69 7465 6d73 2829 7d0a 2020   obj.items()}.  
+000009c0: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+000009d0: 7461 6e63 6528 6f62 6a2c 2028 6c69 7374  tance(obj, (list
+000009e0: 2c20 7475 706c 6529 293a 0a20 2020 2020  , tuple)):.     
+000009f0: 2020 2020 2020 2072 6574 7572 6e20 5b73         return [s
+00000a00: 656c 662e 6465 6661 756c 7428 6974 656d  elf.default(item
+00000a10: 2920 666f 7220 6974 656d 2069 6e20 6f62  ) for item in ob
+00000a20: 6a5d 0a20 2020 2020 2020 2072 6169 7365  j].        raise
+00000a30: 2041 7069 5661 6c75 6545 7272 6f72 2827   ApiValueError('
+00000a40: 556e 6162 6c65 2074 6f20 7072 6570 6172  Unable to prepar
+00000a50: 6520 7479 7065 207b 7d20 666f 7220 7365  e type {} for se
+00000a60: 7269 616c 697a 6174 696f 6e27 2e66 6f72  rialization'.for
+00000a70: 6d61 7428 6f62 6a2e 5f5f 636c 6173 735f  mat(obj.__class_
+00000a80: 5f2e 5f5f 6e61 6d65 5f5f 2929 0a0a 0a63  _.__name__))...c
+00000a90: 6c61 7373 2050 6172 616d 6574 6572 496e  lass ParameterIn
+00000aa0: 5479 7065 2865 6e75 6d2e 456e 756d 293a  Type(enum.Enum):
+00000ab0: 0a20 2020 2051 5545 5259 203d 2027 7175  .    QUERY = 'qu
+00000ac0: 6572 7927 0a20 2020 2048 4541 4445 5220  ery'.    HEADER 
+00000ad0: 3d20 2768 6561 6465 7227 0a20 2020 2050  = 'header'.    P
+00000ae0: 4154 4820 3d20 2770 6174 6827 0a20 2020  ATH = 'path'.   
+00000af0: 2043 4f4f 4b49 4520 3d20 2763 6f6f 6b69   COOKIE = 'cooki
+00000b00: 6527 0a0a 0a63 6c61 7373 2050 6172 616d  e'...class Param
+00000b10: 6574 6572 5374 796c 6528 656e 756d 2e45  eterStyle(enum.E
+00000b20: 6e75 6d29 3a0a 2020 2020 4d41 5452 4958  num):.    MATRIX
+00000b30: 203d 2027 6d61 7472 6978 270a 2020 2020   = 'matrix'.    
+00000b40: 4c41 4245 4c20 3d20 276c 6162 656c 270a  LABEL = 'label'.
+00000b50: 2020 2020 464f 524d 203d 2027 666f 726d      FORM = 'form
+00000b60: 270a 2020 2020 5349 4d50 4c45 203d 2027  '.    SIMPLE = '
+00000b70: 7369 6d70 6c65 270a 2020 2020 5350 4143  simple'.    SPAC
+00000b80: 455f 4445 4c49 4d49 5445 4420 3d20 2773  E_DELIMITED = 's
+00000b90: 7061 6365 4465 6c69 6d69 7465 6427 0a20  paceDelimited'. 
+00000ba0: 2020 2050 4950 455f 4445 4c49 4d49 5445     PIPE_DELIMITE
+00000bb0: 4420 3d20 2770 6970 6544 656c 696d 6974  D = 'pipeDelimit
+00000bc0: 6564 270a 2020 2020 4445 4550 5f4f 424a  ed'.    DEEP_OBJ
+00000bd0: 4543 5420 3d20 2764 6565 704f 626a 6563  ECT = 'deepObjec
+00000be0: 7427 0a0a 0a63 6c61 7373 2050 7265 6669  t'...class Prefi
+00000bf0: 7853 6570 6172 6174 6f72 4974 6572 6174  xSeparatorIterat
+00000c00: 6f72 3a0a 2020 2020 2320 4120 636c 6173  or:.    # A clas
+00000c10: 7320 746f 2073 746f 7265 2070 7265 6669  s to store prefi
+00000c20: 7865 7320 616e 6420 7365 7061 7261 746f  xes and separato
+00000c30: 7273 2066 6f72 2072 6663 3635 3730 2065  rs for rfc6570 e
+00000c40: 7870 616e 7369 6f6e 730a 0a20 2020 2064  xpansions..    d
+00000c50: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00000c60: 2c20 7072 6566 6978 3a20 7374 722c 2073  , prefix: str, s
+00000c70: 6570 6172 6174 6f72 3a20 7374 7229 3a0a  eparator: str):.
+00000c80: 2020 2020 2020 2020 7365 6c66 2e70 7265          self.pre
+00000c90: 6669 7820 3d20 7072 6566 6978 0a20 2020  fix = prefix.   
+00000ca0: 2020 2020 2073 656c 662e 7365 7061 7261       self.separa
+00000cb0: 746f 7220 3d20 7365 7061 7261 746f 720a  tor = separator.
+00000cc0: 2020 2020 2020 2020 7365 6c66 2e66 6972          self.fir
+00000cd0: 7374 203d 2054 7275 650a 2020 2020 2020  st = True.      
+00000ce0: 2020 6966 2073 6570 6172 6174 6f72 2069    if separator i
+00000cf0: 6e20 7b27 2e27 2c20 277c 272c 2027 2532  n {'.', '|', '%2
+00000d00: 3027 7d3a 0a20 2020 2020 2020 2020 2020  0'}:.           
+00000d10: 2069 7465 6d5f 7365 7061 7261 746f 7220   item_separator 
+00000d20: 3d20 7365 7061 7261 746f 720a 2020 2020  = separator.    
+00000d30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000d40: 2020 2020 2020 6974 656d 5f73 6570 6172        item_separ
+00000d50: 6174 6f72 203d 2027 2c27 0a20 2020 2020  ator = ','.     
+00000d60: 2020 2073 656c 662e 6974 656d 5f73 6570     self.item_sep
+00000d70: 6172 6174 6f72 203d 2069 7465 6d5f 7365  arator = item_se
+00000d80: 7061 7261 746f 720a 0a20 2020 2064 6566  parator..    def
+00000d90: 205f 5f69 7465 725f 5f28 7365 6c66 293a   __iter__(self):
+00000da0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000db0: 7365 6c66 0a0a 2020 2020 6465 6620 5f5f  self..    def __
+00000dc0: 6e65 7874 5f5f 2873 656c 6629 3a0a 2020  next__(self):.  
+00000dd0: 2020 2020 2020 6966 2073 656c 662e 6669        if self.fi
+00000de0: 7273 743a 0a20 2020 2020 2020 2020 2020  rst:.           
+00000df0: 2073 656c 662e 6669 7273 7420 3d20 4661   self.first = Fa
+00000e00: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00000e10: 7265 7475 726e 2073 656c 662e 7072 6566  return self.pref
+00000e20: 6978 0a20 2020 2020 2020 2072 6574 7572  ix.        retur
+00000e30: 6e20 7365 6c66 2e73 6570 6172 6174 6f72  n self.separator
+00000e40: 0a0a 0a63 6c61 7373 2050 6172 616d 6574  ...class Paramet
+00000e50: 6572 5365 7269 616c 697a 6572 4261 7365  erSerializerBase
+00000e60: 3a0a 2020 2020 4063 6c61 7373 6d65 7468  :.    @classmeth
+00000e70: 6f64 0a20 2020 2064 6566 205f 6765 745f  od.    def _get_
+00000e80: 6465 6661 756c 745f 6578 706c 6f64 6528  default_explode(
+00000e90: 636c 732c 2073 7479 6c65 3a20 5061 7261  cls, style: Para
+00000ea0: 6d65 7465 7253 7479 6c65 2920 2d3e 2062  meterStyle) -> b
+00000eb0: 6f6f 6c3a 0a20 2020 2020 2020 2072 6574  ool:.        ret
+00000ec0: 7572 6e20 4661 6c73 650a 0a20 2020 2040  urn False..    @
+00000ed0: 7374 6174 6963 6d65 7468 6f64 0a20 2020  staticmethod.   
+00000ee0: 2064 6566 205f 5f72 6566 3635 3730 5f69   def __ref6570_i
+00000ef0: 7465 6d5f 7661 6c75 6528 696e 5f64 6174  tem_value(in_dat
+00000f00: 613a 2074 7970 696e 672e 416e 792c 2070  a: typing.Any, p
+00000f10: 6572 6365 6e74 5f65 6e63 6f64 653a 2062  ercent_encode: b
+00000f20: 6f6f 6c29 3a0a 2020 2020 2020 2020 2222  ool):.        ""
+00000f30: 220a 2020 2020 2020 2020 4765 7420 7265  ".        Get re
+00000f40: 7072 6573 656e 7461 7469 6f6e 2069 6620  presentation if 
+00000f50: 7374 722f 666c 6f61 742f 696e 742f 4e6f  str/float/int/No
+00000f60: 6e65 2f69 7465 6d73 2069 6e20 6c69 7374  ne/items in list
+00000f70: 2f20 7661 6c75 6573 2069 6e20 6469 6374  / values in dict
+00000f80: 0a20 2020 2020 2020 204e 6f6e 6520 6973  .        None is
+00000f90: 2072 6574 7572 6e65 6420 6966 2061 6e20   returned if an 
+00000fa0: 6974 656d 2069 7320 756e 6465 6669 6e65  item is undefine
+00000fb0: 642c 2075 7365 2063 6173 6573 2061 7265  d, use cases are
+00000fc0: 2076 616c 7565 3d0a 2020 2020 2020 2020   value=.        
+00000fd0: 2d20 4e6f 6e65 0a20 2020 2020 2020 202d  - None.        -
+00000fe0: 205b 5d0a 2020 2020 2020 2020 2d20 7b7d   [].        - {}
+00000ff0: 0a20 2020 2020 2020 202d 205b 4e6f 6e65  .        - [None
+00001000: 2c20 4e6f 6e65 204e 6f6e 655d 0a20 2020  , None None].   
+00001010: 2020 2020 202d 207b 2761 273a 204e 6f6e       - {'a': Non
+00001020: 652c 2027 6227 3a20 4e6f 6e65 7d0a 2020  e, 'b': None}.  
+00001030: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00001040: 2020 6966 2074 7970 6528 696e 5f64 6174    if type(in_dat
+00001050: 6129 2069 6e20 7b73 7472 2c20 666c 6f61  a) in {str, floa
+00001060: 742c 2069 6e74 7d3a 0a20 2020 2020 2020  t, int}:.       
+00001070: 2020 2020 2069 6620 7065 7263 656e 745f       if percent_
+00001080: 656e 636f 6465 3a0a 2020 2020 2020 2020  encode:.        
+00001090: 2020 2020 2020 2020 7265 7475 726e 2071          return q
+000010a0: 756f 7465 2873 7472 2869 6e5f 6461 7461  uote(str(in_data
+000010b0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+000010c0: 6574 7572 6e20 7374 7228 696e 5f64 6174  eturn str(in_dat
+000010d0: 6129 0a20 2020 2020 2020 2065 6c69 6620  a).        elif 
+000010e0: 6973 696e 7374 616e 6365 2869 6e5f 6461  isinstance(in_da
+000010f0: 7461 2c20 6e6f 6e65 5f74 7970 6529 3a0a  ta, none_type):.
+00001100: 2020 2020 2020 2020 2020 2020 2320 6967              # ig
+00001110: 6e6f 7265 6420 6279 2074 6865 2065 7870  nored by the exp
+00001120: 616e 7369 6f6e 2070 726f 6365 7373 2068  ansion process h
+00001130: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00001140: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00001150: 6874 6d6c 2f72 6663 3635 3730 2373 6563  html/rfc6570#sec
+00001160: 7469 6f6e 2d33 2e32 2e31 0a20 2020 2020  tion-3.2.1.     
+00001170: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00001180: 6e65 0a20 2020 2020 2020 2065 6c69 6620  ne.        elif 
+00001190: 6973 696e 7374 616e 6365 2869 6e5f 6461  isinstance(in_da
+000011a0: 7461 2c20 6c69 7374 2920 616e 6420 6e6f  ta, list) and no
+000011b0: 7420 696e 5f64 6174 613a 0a20 2020 2020  t in_data:.     
+000011c0: 2020 2020 2020 2023 2069 676e 6f72 6564         # ignored
+000011d0: 2062 7920 7468 6520 6578 7061 6e73 696f   by the expansio
+000011e0: 6e20 7072 6f63 6573 7320 6874 7470 733a  n process https:
+000011f0: 2f2f 6461 7461 7472 6163 6b65 722e 6965  //datatracker.ie
+00001200: 7466 2e6f 7267 2f64 6f63 2f68 746d 6c2f  tf.org/doc/html/
+00001210: 7266 6336 3537 3023 7365 6374 696f 6e2d  rfc6570#section-
+00001220: 332e 322e 310a 2020 2020 2020 2020 2020  3.2.1.          
+00001230: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
+00001240: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00001250: 7461 6e63 6528 696e 5f64 6174 612c 2064  tance(in_data, d
+00001260: 6963 7429 2061 6e64 206e 6f74 2069 6e5f  ict) and not in_
+00001270: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+00001280: 2020 2320 6967 6e6f 7265 6420 6279 2074    # ignored by t
+00001290: 6865 2065 7870 616e 7369 6f6e 2070 726f  he expansion pro
+000012a0: 6365 7373 2068 7474 7073 3a2f 2f64 6174  cess https://dat
+000012b0: 6174 7261 636b 6572 2e69 6574 662e 6f72  atracker.ietf.or
+000012c0: 672f 646f 632f 6874 6d6c 2f72 6663 3635  g/doc/html/rfc65
+000012d0: 3730 2373 6563 7469 6f6e 2d33 2e32 2e31  70#section-3.2.1
+000012e0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000012f0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+00001300: 2072 6169 7365 2041 7069 5661 6c75 6545   raise ApiValueE
+00001310: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
+00001320: 6765 6e65 7261 7465 2061 2072 6566 3635  generate a ref65
+00001330: 3730 2069 7465 6d20 7265 7072 6573 656e  70 item represen
+00001340: 7461 7469 6f6e 206f 6620 7b7d 272e 666f  tation of {}'.fo
+00001350: 726d 6174 2869 6e5f 6461 7461 2929 0a0a  rmat(in_data))..
+00001360: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
+00001370: 640a 2020 2020 6465 6620 5f74 6f5f 6469  d.    def _to_di
+00001380: 6374 286e 616d 653a 2073 7472 2c20 7661  ct(name: str, va
+00001390: 6c75 653a 2073 7472 293a 0a20 2020 2020  lue: str):.     
+000013a0: 2020 2072 6574 7572 6e20 7b6e 616d 653a     return {name:
+000013b0: 2076 616c 7565 7d0a 0a20 2020 2022 2222   value}..    """
+000013c0: 0a20 2020 2072 6663 3635 3730 2064 6f65  .    rfc6570 doe
+000013d0: 7320 6e6f 7420 7370 6563 6966 7920 686f  s not specify ho
+000013e0: 7720 626f 6f6c 6561 6e20 7661 6c75 6573  w boolean values
+000013f0: 2061 7265 2073 6572 6961 6c69 7a65 6420   are serialized 
+00001400: 736f 2077 6520 7573 6520 6c6f 7765 7263  so we use lowerc
+00001410: 6173 6520 2274 7275 6522 2061 6e64 2022  ase "true" and "
+00001420: 6661 6c73 650a 2020 2020 2222 220a 2020  false.    """.  
+00001430: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00001440: 2020 2064 6566 205f 5f6b 6f6e 6669 675f     def __konfig_
+00001450: 626f 6f6c 5f65 7870 616e 7369 6f6e 280a  bool_expansion(.
+00001460: 2020 2020 2020 2020 636c 732c 0a20 2020          cls,.   
+00001470: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
+00001480: 7069 6e67 2e41 6e79 2c0a 2020 2020 2020  ping.Any,.      
+00001490: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+000014a0: 6f72 5f69 7465 7261 746f 723a 2050 7265  or_iterator: Pre
+000014b0: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
+000014c0: 6174 6f72 2c0a 2020 2020 2020 2020 7661  ator,.        va
+000014d0: 725f 6e61 6d65 5f70 6965 6365 3a20 7374  r_name_piece: st
+000014e0: 722c 0a20 2020 2020 2020 206e 616d 6564  r,.        named
+000014f0: 5f70 6172 616d 6574 6572 5f65 7870 616e  _parameter_expan
+00001500: 7369 6f6e 3a20 626f 6f6c 0a20 2020 2029  sion: bool.    )
+00001510: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00001520: 2069 7465 6d5f 7661 6c75 6520 3d20 2274   item_value = "t
+00001530: 7275 6522 2069 6620 696e 5f64 6174 6120  rue" if in_data 
+00001540: 6973 2054 7275 6520 656c 7365 2022 6661  is True else "fa
+00001550: 6c73 6522 0a20 2020 2020 2020 2069 6620  lse".        if 
+00001560: 6974 656d 5f76 616c 7565 2069 7320 4e6f  item_value is No
+00001570: 6e65 206f 7220 2869 7465 6d5f 7661 6c75  ne or (item_valu
+00001580: 6520 3d3d 2027 2720 616e 6420 7072 6566  e == '' and pref
+00001590: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+000015a0: 7261 746f 722e 7365 7061 7261 746f 7220  rator.separator 
+000015b0: 3d3d 2027 3b27 293a 0a20 2020 2020 2020  == ';'):.       
+000015c0: 2020 2020 2072 6574 7572 6e20 6e65 7874       return next
+000015d0: 2870 7265 6669 785f 7365 7061 7261 746f  (prefix_separato
+000015e0: 725f 6974 6572 6174 6f72 2920 2b20 7661  r_iterator) + va
+000015f0: 725f 6e61 6d65 5f70 6965 6365 0a20 2020  r_name_piece.   
+00001600: 2020 2020 2076 616c 7565 5f70 6169 725f       value_pair_
+00001610: 6571 7561 6c73 203d 2027 3d27 2069 6620  equals = '=' if 
+00001620: 6e61 6d65 645f 7061 7261 6d65 7465 725f  named_parameter_
+00001630: 6578 7061 6e73 696f 6e20 656c 7365 2027  expansion else '
+00001640: 270a 2020 2020 2020 2020 7265 7475 726e  '.        return
+00001650: 206e 6578 7428 7072 6566 6978 5f73 6570   next(prefix_sep
+00001660: 6172 6174 6f72 5f69 7465 7261 746f 7229  arator_iterator)
+00001670: 202b 2076 6172 5f6e 616d 655f 7069 6563   + var_name_piec
+00001680: 6520 2b20 7661 6c75 655f 7061 6972 5f65  e + value_pair_e
+00001690: 7175 616c 7320 2b20 6974 656d 5f76 616c  quals + item_val
+000016a0: 7565 0a0a 2020 2020 4063 6c61 7373 6d65  ue..    @classme
+000016b0: 7468 6f64 0a20 2020 2064 6566 205f 5f72  thod.    def __r
+000016c0: 6566 3635 3730 5f73 7472 5f66 6c6f 6174  ef6570_str_float
+000016d0: 5f69 6e74 5f65 7870 616e 7369 6f6e 280a  _int_expansion(.
+000016e0: 2020 2020 2020 2020 636c 732c 0a20 2020          cls,.   
+000016f0: 2020 2020 2076 6172 6961 626c 655f 6e61       variable_na
+00001700: 6d65 3a20 7374 722c 0a20 2020 2020 2020  me: str,.       
+00001710: 2069 6e5f 6461 7461 3a20 7479 7069 6e67   in_data: typing
+00001720: 2e41 6e79 2c0a 2020 2020 2020 2020 6578  .Any,.        ex
+00001730: 706c 6f64 653a 2062 6f6f 6c2c 0a20 2020  plode: bool,.   
+00001740: 2020 2020 2070 6572 6365 6e74 5f65 6e63       percent_enc
+00001750: 6f64 653a 2062 6f6f 6c2c 0a20 2020 2020  ode: bool,.     
+00001760: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
+00001770: 746f 725f 6974 6572 6174 6f72 3a20 5072  tor_iterator: Pr
+00001780: 6566 6978 5365 7061 7261 746f 7249 7465  efixSeparatorIte
+00001790: 7261 746f 722c 0a20 2020 2020 2020 2076  rator,.        v
+000017a0: 6172 5f6e 616d 655f 7069 6563 653a 2073  ar_name_piece: s
+000017b0: 7472 2c0a 2020 2020 2020 2020 6e61 6d65  tr,.        name
+000017c0: 645f 7061 7261 6d65 7465 725f 6578 7061  d_parameter_expa
+000017d0: 6e73 696f 6e3a 2062 6f6f 6c0a 2020 2020  nsion: bool.    
+000017e0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+000017f0: 2020 6974 656d 5f76 616c 7565 203d 2063    item_value = c
+00001800: 6c73 2e5f 5f72 6566 3635 3730 5f69 7465  ls.__ref6570_ite
+00001810: 6d5f 7661 6c75 6528 696e 5f64 6174 612c  m_value(in_data,
+00001820: 2070 6572 6365 6e74 5f65 6e63 6f64 6529   percent_encode)
+00001830: 0a20 2020 2020 2020 2069 6620 6974 656d  .        if item
+00001840: 5f76 616c 7565 2069 7320 4e6f 6e65 206f  _value is None o
+00001850: 7220 2869 7465 6d5f 7661 6c75 6520 3d3d  r (item_value ==
+00001860: 2027 2720 616e 6420 7072 6566 6978 5f73   '' and prefix_s
+00001870: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00001880: 722e 7365 7061 7261 746f 7220 3d3d 2027  r.separator == '
+00001890: 3b27 293a 0a20 2020 2020 2020 2020 2020  ;'):.           
+000018a0: 2072 6574 7572 6e20 6e65 7874 2870 7265   return next(pre
+000018b0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+000018c0: 6572 6174 6f72 2920 2b20 7661 725f 6e61  erator) + var_na
+000018d0: 6d65 5f70 6965 6365 0a20 2020 2020 2020  me_piece.       
+000018e0: 2076 616c 7565 5f70 6169 725f 6571 7561   value_pair_equa
+000018f0: 6c73 203d 2027 3d27 2069 6620 6e61 6d65  ls = '=' if name
+00001900: 645f 7061 7261 6d65 7465 725f 6578 7061  d_parameter_expa
+00001910: 6e73 696f 6e20 656c 7365 2027 270a 2020  nsion else ''.  
+00001920: 2020 2020 2020 7265 7475 726e 206e 6578        return nex
+00001930: 7428 7072 6566 6978 5f73 6570 6172 6174  t(prefix_separat
+00001940: 6f72 5f69 7465 7261 746f 7229 202b 2076  or_iterator) + v
+00001950: 6172 5f6e 616d 655f 7069 6563 6520 2b20  ar_name_piece + 
+00001960: 7661 6c75 655f 7061 6972 5f65 7175 616c  value_pair_equal
+00001970: 7320 2b20 6974 656d 5f76 616c 7565 0a0a  s + item_value..
+00001980: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00001990: 0a20 2020 2064 6566 205f 5f72 6566 3635  .    def __ref65
+000019a0: 3730 5f6c 6973 745f 6578 7061 6e73 696f  70_list_expansio
+000019b0: 6e28 0a20 2020 2020 2020 2063 6c73 2c0a  n(.        cls,.
+000019c0: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+000019d0: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
+000019e0: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
+000019f0: 696e 672e 416e 792c 0a20 2020 2020 2020  ing.Any,.       
+00001a00: 2065 7870 6c6f 6465 3a20 626f 6f6c 2c0a   explode: bool,.
+00001a10: 2020 2020 2020 2020 7065 7263 656e 745f          percent_
+00001a20: 656e 636f 6465 3a20 626f 6f6c 2c0a 2020  encode: bool,.  
+00001a30: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
+00001a40: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
+00001a50: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
+00001a60: 4974 6572 6174 6f72 2c0a 2020 2020 2020  Iterator,.      
+00001a70: 2020 7661 725f 6e61 6d65 5f70 6965 6365    var_name_piece
+00001a80: 3a20 7374 722c 0a20 2020 2020 2020 206e  : str,.        n
+00001a90: 616d 6564 5f70 6172 616d 6574 6572 5f65  amed_parameter_e
+00001aa0: 7870 616e 7369 6f6e 3a20 626f 6f6c 0a20  xpansion: bool. 
+00001ab0: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
+00001ac0: 2020 2020 2069 7465 6d5f 7661 6c75 6573       item_values
+00001ad0: 203d 205b 636c 732e 5f5f 7265 6636 3537   = [cls.__ref657
+00001ae0: 305f 6974 656d 5f76 616c 7565 2876 2c20  0_item_value(v, 
+00001af0: 7065 7263 656e 745f 656e 636f 6465 2920  percent_encode) 
+00001b00: 666f 7220 7620 696e 2069 6e5f 6461 7461  for v in in_data
+00001b10: 5d0a 2020 2020 2020 2020 6974 656d 5f76  ].        item_v
+00001b20: 616c 7565 7320 3d20 5b76 2066 6f72 2076  alues = [v for v
+00001b30: 2069 6e20 6974 656d 5f76 616c 7565 7320   in item_values 
+00001b40: 6966 2076 2069 7320 6e6f 7420 4e6f 6e65  if v is not None
+00001b50: 5d0a 2020 2020 2020 2020 6966 206e 6f74  ].        if not
+00001b60: 2069 7465 6d5f 7661 6c75 6573 3a0a 2020   item_values:.  
+00001b70: 2020 2020 2020 2020 2020 2320 6967 6e6f            # igno
+00001b80: 7265 6420 6279 2074 6865 2065 7870 616e  red by the expan
+00001b90: 7369 6f6e 2070 726f 6365 7373 2068 7474  sion process htt
+00001ba0: 7073 3a2f 2f64 6174 6174 7261 636b 6572  ps://datatracker
+00001bb0: 2e69 6574 662e 6f72 672f 646f 632f 6874  .ietf.org/doc/ht
+00001bc0: 6d6c 2f72 6663 3635 3730 2373 6563 7469  ml/rfc6570#secti
+00001bd0: 6f6e 2d33 2e32 2e31 0a20 2020 2020 2020  on-3.2.1.       
+00001be0: 2020 2020 2072 6574 7572 6e20 2222 0a20       return "". 
+00001bf0: 2020 2020 2020 2076 616c 7565 5f70 6169         value_pai
+00001c00: 725f 6571 7561 6c73 203d 2027 3d27 2069  r_equals = '=' i
+00001c10: 6620 6e61 6d65 645f 7061 7261 6d65 7465  f named_paramete
+00001c20: 725f 6578 7061 6e73 696f 6e20 656c 7365  r_expansion else
+00001c30: 2027 270a 2020 2020 2020 2020 6966 206e   ''.        if n
+00001c40: 6f74 2065 7870 6c6f 6465 3a0a 2020 2020  ot explode:.    
+00001c50: 2020 2020 2020 2020 7265 7475 726e 2028          return (
+00001c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c70: 206e 6578 7428 7072 6566 6978 5f73 6570   next(prefix_sep
+00001c80: 6172 6174 6f72 5f69 7465 7261 746f 7229  arator_iterator)
+00001c90: 202b 0a20 2020 2020 2020 2020 2020 2020   +.             
+00001ca0: 2020 2076 6172 5f6e 616d 655f 7069 6563     var_name_piec
+00001cb0: 6520 2b0a 2020 2020 2020 2020 2020 2020  e +.            
+00001cc0: 2020 2020 7661 6c75 655f 7061 6972 5f65      value_pair_e
+00001cd0: 7175 616c 7320 2b0a 2020 2020 2020 2020  quals +.        
+00001ce0: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+00001cf0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00001d00: 722e 6974 656d 5f73 6570 6172 6174 6f72  r.item_separator
+00001d10: 2e6a 6f69 6e28 6974 656d 5f76 616c 7565  .join(item_value
+00001d20: 7329 0a20 2020 2020 2020 2020 2020 2029  s).            )
+00001d30: 0a20 2020 2020 2020 2023 2065 7870 6c6f  .        # explo
+00001d40: 6465 640a 2020 2020 2020 2020 7265 7475  ded.        retu
+00001d50: 726e 206e 6578 7428 7072 6566 6978 5f73  rn next(prefix_s
+00001d60: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00001d70: 7229 202b 206e 6578 7428 7072 6566 6978  r) + next(prefix
+00001d80: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+00001d90: 746f 7229 2e6a 6f69 6e28 0a20 2020 2020  tor).join(.     
+00001da0: 2020 2020 2020 205b 7661 725f 6e61 6d65         [var_name
+00001db0: 5f70 6965 6365 202b 2076 616c 7565 5f70  _piece + value_p
+00001dc0: 6169 725f 6571 7561 6c73 202b 2076 616c  air_equals + val
+00001dd0: 2066 6f72 2076 616c 2069 6e20 6974 656d   for val in item
+00001de0: 5f76 616c 7565 735d 0a20 2020 2020 2020  _values].       
+00001df0: 2029 0a0a 2020 2020 4063 6c61 7373 6d65   )..    @classme
+00001e00: 7468 6f64 0a20 2020 2064 6566 205f 5f72  thod.    def __r
+00001e10: 6566 3635 3730 5f64 6963 745f 6578 7061  ef6570_dict_expa
+00001e20: 6e73 696f 6e28 0a20 2020 2020 2020 2063  nsion(.        c
+00001e30: 6c73 2c0a 2020 2020 2020 2020 7661 7269  ls,.        vari
+00001e40: 6162 6c65 5f6e 616d 653a 2073 7472 2c0a  able_name: str,.
+00001e50: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
+00001e60: 2074 7970 696e 672e 416e 792c 0a20 2020   typing.Any,.   
+00001e70: 2020 2020 2065 7870 6c6f 6465 3a20 626f       explode: bo
+00001e80: 6f6c 2c0a 2020 2020 2020 2020 7065 7263  ol,.        perc
+00001e90: 656e 745f 656e 636f 6465 3a20 626f 6f6c  ent_encode: bool
+00001ea0: 2c0a 2020 2020 2020 2020 7072 6566 6978  ,.        prefix
+00001eb0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+00001ec0: 746f 723a 2050 7265 6669 7853 6570 6172  tor: PrefixSepar
+00001ed0: 6174 6f72 4974 6572 6174 6f72 2c0a 2020  atorIterator,.  
+00001ee0: 2020 2020 2020 7661 725f 6e61 6d65 5f70        var_name_p
+00001ef0: 6965 6365 3a20 7374 722c 0a20 2020 2020  iece: str,.     
+00001f00: 2020 206e 616d 6564 5f70 6172 616d 6574     named_paramet
+00001f10: 6572 5f65 7870 616e 7369 6f6e 3a20 626f  er_expansion: bo
+00001f20: 6f6c 0a20 2020 2029 202d 3e20 7374 723a  ol.    ) -> str:
+00001f30: 0a20 2020 2020 2020 2069 6e5f 6461 7461  .        in_data
+00001f40: 5f74 7261 6e73 666f 726d 6564 203d 207b  _transformed = {
+00001f50: 6b65 793a 2063 6c73 2e5f 5f72 6566 3635  key: cls.__ref65
+00001f60: 3730 5f69 7465 6d5f 7661 6c75 6528 7661  70_item_value(va
+00001f70: 6c2c 2070 6572 6365 6e74 5f65 6e63 6f64  l, percent_encod
+00001f80: 6529 2066 6f72 206b 6579 2c20 7661 6c20  e) for key, val 
+00001f90: 696e 2069 6e5f 6461 7461 2e69 7465 6d73  in in_data.items
+00001fa0: 2829 7d0a 2020 2020 2020 2020 696e 5f64  ()}.        in_d
+00001fb0: 6174 615f 7472 616e 7366 6f72 6d65 6420  ata_transformed 
+00001fc0: 3d20 7b6b 6579 3a20 7661 6c20 666f 7220  = {key: val for 
+00001fd0: 6b65 792c 2076 616c 2069 6e20 696e 5f64  key, val in in_d
+00001fe0: 6174 615f 7472 616e 7366 6f72 6d65 642e  ata_transformed.
+00001ff0: 6974 656d 7328 2920 6966 2076 616c 2069  items() if val i
+00002000: 7320 6e6f 7420 4e6f 6e65 7d0a 2020 2020  s not None}.    
+00002010: 2020 2020 6966 206e 6f74 2069 6e5f 6461      if not in_da
+00002020: 7461 5f74 7261 6e73 666f 726d 6564 3a0a  ta_transformed:.
+00002030: 2020 2020 2020 2020 2020 2020 2320 6967              # ig
+00002040: 6e6f 7265 6420 6279 2074 6865 2065 7870  nored by the exp
+00002050: 616e 7369 6f6e 2070 726f 6365 7373 2068  ansion process h
+00002060: 7474 7073 3a2f 2f64 6174 6174 7261 636b  ttps://datatrack
+00002070: 6572 2e69 6574 662e 6f72 672f 646f 632f  er.ietf.org/doc/
+00002080: 6874 6d6c 2f72 6663 3635 3730 2373 6563  html/rfc6570#sec
+00002090: 7469 6f6e 2d33 2e32 2e31 0a20 2020 2020  tion-3.2.1.     
+000020a0: 2020 2020 2020 2072 6574 7572 6e20 2222         return ""
+000020b0: 0a20 2020 2020 2020 2076 616c 7565 5f70  .        value_p
+000020c0: 6169 725f 6571 7561 6c73 203d 2027 3d27  air_equals = '='
+000020d0: 2069 6620 6e61 6d65 645f 7061 7261 6d65   if named_parame
+000020e0: 7465 725f 6578 7061 6e73 696f 6e20 656c  ter_expansion el
+000020f0: 7365 2027 270a 2020 2020 2020 2020 6966  se ''.        if
+00002100: 206e 6f74 2065 7870 6c6f 6465 3a0a 2020   not explode:.  
+00002110: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002120: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00002130: 2020 206e 6578 7428 7072 6566 6978 5f73     next(prefix_s
+00002140: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00002150: 7229 202b 0a20 2020 2020 2020 2020 2020  r) +.           
+00002160: 2020 2020 2076 6172 5f6e 616d 655f 7069       var_name_pi
+00002170: 6563 6520 2b20 7661 6c75 655f 7061 6972  ece + value_pair
+00002180: 5f65 7175 616c 7320 2b0a 2020 2020 2020  _equals +.      
+00002190: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
+000021a0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+000021b0: 746f 722e 6974 656d 5f73 6570 6172 6174  tor.item_separat
+000021c0: 6f72 2e6a 6f69 6e28 0a20 2020 2020 2020  or.join(.       
+000021d0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+000021e0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+000021f0: 6572 6174 6f72 2e69 7465 6d5f 7365 7061  erator.item_sepa
+00002200: 7261 746f 722e 6a6f 696e 280a 2020 2020  rator.join(.    
+00002210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002220: 2020 2020 6974 656d 5f70 6169 720a 2020      item_pair.  
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2020 2920 666f 7220 6974 656d 5f70 6169    ) for item_pai
+00002250: 7220 696e 2069 6e5f 6461 7461 5f74 7261  r in in_data_tra
+00002260: 6e73 666f 726d 6564 2e69 7465 6d73 2829  nsformed.items()
+00002270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002280: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+00002290: 0a20 2020 2020 2020 2023 2065 7870 6c6f  .        # explo
+000022a0: 6465 640a 2020 2020 2020 2020 7265 7475  ded.        retu
+000022b0: 726e 206e 6578 7428 7072 6566 6978 5f73  rn next(prefix_s
+000022c0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+000022d0: 7229 202b 206e 6578 7428 7072 6566 6978  r) + next(prefix
+000022e0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+000022f0: 746f 7229 2e6a 6f69 6e28 0a20 2020 2020  tor).join(.     
+00002300: 2020 2020 2020 205b 6b65 7920 2b20 273d         [key + '=
+00002310: 2720 2b20 7661 6c20 666f 7220 6b65 792c  ' + val for key,
+00002320: 2076 616c 2069 6e20 696e 5f64 6174 615f   val in in_data_
+00002330: 7472 616e 7366 6f72 6d65 642e 6974 656d  transformed.item
+00002340: 7328 295d 0a20 2020 2020 2020 2029 0a0a  s()].        )..
+00002350: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00002360: 0a20 2020 2064 6566 205f 7265 6636 3537  .    def _ref657
+00002370: 305f 6578 7061 6e73 696f 6e28 0a20 2020  0_expansion(.   
+00002380: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+00002390: 2020 7661 7269 6162 6c65 5f6e 616d 653a    variable_name:
+000023a0: 2073 7472 2c0a 2020 2020 2020 2020 696e   str,.        in
+000023b0: 5f64 6174 613a 2074 7970 696e 672e 416e  _data: typing.An
+000023c0: 792c 0a20 2020 2020 2020 2065 7870 6c6f  y,.        explo
+000023d0: 6465 3a20 626f 6f6c 2c0a 2020 2020 2020  de: bool,.      
+000023e0: 2020 7065 7263 656e 745f 656e 636f 6465    percent_encode
+000023f0: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
+00002400: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00002410: 5f69 7465 7261 746f 723a 2050 7265 6669  _iterator: Prefi
+00002420: 7853 6570 6172 6174 6f72 4974 6572 6174  xSeparatorIterat
+00002430: 6f72 0a20 2020 2029 202d 3e20 7374 723a  or.    ) -> str:
+00002440: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00002450: 2020 2020 2053 6570 6172 6174 6f72 2069       Separator i
+00002460: 7320 666f 7220 7365 7061 7261 7465 2076  s for separate v
+00002470: 6172 6961 626c 6573 206c 696b 6520 6469  ariables like di
+00002480: 6374 2077 6974 6820 6578 706c 6f64 6520  ct with explode 
+00002490: 7472 7565 2c20 6e6f 7420 666f 7220 6172  true, not for ar
+000024a0: 7261 7920 6974 656d 2073 6570 6172 6174  ray item separat
+000024b0: 696f 6e0a 2020 2020 2020 2020 2222 220a  ion.        """.
+000024c0: 2020 2020 2020 2020 6e61 6d65 645f 7061          named_pa
+000024d0: 7261 6d65 7465 725f 6578 7061 6e73 696f  rameter_expansio
+000024e0: 6e20 3d20 7072 6566 6978 5f73 6570 6172  n = prefix_separ
+000024f0: 6174 6f72 5f69 7465 7261 746f 722e 7365  ator_iterator.se
+00002500: 7061 7261 746f 7220 696e 207b 2726 272c  parator in {'&',
+00002510: 2027 3b27 7d0a 2020 2020 2020 2020 7661   ';'}.        va
+00002520: 725f 6e61 6d65 5f70 6965 6365 203d 2076  r_name_piece = v
+00002530: 6172 6961 626c 655f 6e61 6d65 2069 6620  ariable_name if 
+00002540: 6e61 6d65 645f 7061 7261 6d65 7465 725f  named_parameter_
+00002550: 6578 7061 6e73 696f 6e20 656c 7365 2027  expansion else '
+00002560: 270a 2020 2020 2020 2020 6966 2074 7970  '.        if typ
+00002570: 6528 696e 5f64 6174 6129 2069 6e20 7b73  e(in_data) in {s
+00002580: 7472 2c20 666c 6f61 742c 2069 6e74 7d3a  tr, float, int}:
+00002590: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000025a0: 7572 6e20 636c 732e 5f5f 7265 6636 3537  urn cls.__ref657
+000025b0: 305f 7374 725f 666c 6f61 745f 696e 745f  0_str_float_int_
+000025c0: 6578 7061 6e73 696f 6e28 0a20 2020 2020  expansion(.     
+000025d0: 2020 2020 2020 2020 2020 2076 6172 6961             varia
+000025e0: 626c 655f 6e61 6d65 2c0a 2020 2020 2020  ble_name,.      
+000025f0: 2020 2020 2020 2020 2020 696e 5f64 6174            in_dat
+00002600: 612c 0a20 2020 2020 2020 2020 2020 2020  a,.             
+00002610: 2020 2065 7870 6c6f 6465 2c0a 2020 2020     explode,.    
+00002620: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+00002630: 656e 745f 656e 636f 6465 2c0a 2020 2020  ent_encode,.    
+00002640: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+00002650: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00002660: 7261 746f 722c 0a20 2020 2020 2020 2020  rator,.         
+00002670: 2020 2020 2020 2076 6172 5f6e 616d 655f         var_name_
+00002680: 7069 6563 652c 0a20 2020 2020 2020 2020  piece,.         
+00002690: 2020 2020 2020 206e 616d 6564 5f70 6172         named_par
+000026a0: 616d 6574 6572 5f65 7870 616e 7369 6f6e  ameter_expansion
+000026b0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000026c0: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+000026d0: 7374 616e 6365 2869 6e5f 6461 7461 2c20  stance(in_data, 
+000026e0: 6e6f 6e65 5f74 7970 6529 3a0a 2020 2020  none_type):.    
+000026f0: 2020 2020 2020 2020 2320 6967 6e6f 7265          # ignore
+00002700: 6420 6279 2074 6865 2065 7870 616e 7369  d by the expansi
+00002710: 6f6e 2070 726f 6365 7373 2068 7474 7073  on process https
+00002720: 3a2f 2f64 6174 6174 7261 636b 6572 2e69  ://datatracker.i
+00002730: 6574 662e 6f72 672f 646f 632f 6874 6d6c  etf.org/doc/html
+00002740: 2f72 6663 3635 3730 2373 6563 7469 6f6e  /rfc6570#section
+00002750: 2d33 2e32 2e31 0a20 2020 2020 2020 2020  -3.2.1.         
+00002760: 2020 2072 6574 7572 6e20 2222 0a20 2020     return "".   
+00002770: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00002780: 616e 6365 2869 6e5f 6461 7461 2c20 6c69  ance(in_data, li
+00002790: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+000027a0: 2072 6574 7572 6e20 636c 732e 5f5f 7265   return cls.__re
+000027b0: 6636 3537 305f 6c69 7374 5f65 7870 616e  f6570_list_expan
+000027c0: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+000027d0: 2020 2020 2020 7661 7269 6162 6c65 5f6e        variable_n
+000027e0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+000027f0: 2020 2020 2069 6e5f 6461 7461 2c0a 2020       in_data,.  
+00002800: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00002810: 706c 6f64 652c 0a20 2020 2020 2020 2020  plode,.         
+00002820: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
+00002830: 6e63 6f64 652c 0a20 2020 2020 2020 2020  ncode,.         
+00002840: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+00002850: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00002860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002870: 2020 7661 725f 6e61 6d65 5f70 6965 6365    var_name_piece
+00002880: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002890: 2020 6e61 6d65 645f 7061 7261 6d65 7465    named_paramete
+000028a0: 725f 6578 7061 6e73 696f 6e0a 2020 2020  r_expansion.    
+000028b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000028c0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+000028d0: 6528 696e 5f64 6174 612c 2064 6963 7429  e(in_data, dict)
+000028e0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000028f0: 7475 726e 2063 6c73 2e5f 5f72 6566 3635  turn cls.__ref65
+00002900: 3730 5f64 6963 745f 6578 7061 6e73 696f  70_dict_expansio
+00002910: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00002920: 2020 2076 6172 6961 626c 655f 6e61 6d65     variable_name
+00002930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002940: 2020 696e 5f64 6174 612c 0a20 2020 2020    in_data,.     
+00002950: 2020 2020 2020 2020 2020 2065 7870 6c6f             explo
+00002960: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00002970: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
+00002980: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
+00002990: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
+000029a0: 6174 6f72 5f69 7465 7261 746f 722c 0a20  ator_iterator,. 
+000029b0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+000029c0: 6172 5f6e 616d 655f 7069 6563 652c 0a20  ar_name_piece,. 
+000029d0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000029e0: 616d 6564 5f70 6172 616d 6574 6572 5f65  amed_parameter_e
+000029f0: 7870 616e 7369 6f6e 0a20 2020 2020 2020  xpansion.       
+00002a00: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+00002a10: 6c69 6620 6973 696e 7374 616e 6365 2869  lif isinstance(i
+00002a20: 6e5f 6461 7461 2c20 626f 6f6c 293a 0a20  n_data, bool):. 
+00002a30: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00002a40: 6e20 636c 732e 5f5f 6b6f 6e66 6967 5f62  n cls.__konfig_b
+00002a50: 6f6f 6c5f 6578 7061 6e73 696f 6e28 0a20  ool_expansion(. 
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002a70: 6e5f 6461 7461 2c0a 2020 2020 2020 2020  n_data,.        
+00002a80: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+00002a90: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00002aa0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+00002ab0: 2020 2076 6172 5f6e 616d 655f 7069 6563     var_name_piec
+00002ac0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00002ad0: 2020 206e 616d 6564 5f70 6172 616d 6574     named_paramet
+00002ae0: 6572 5f65 7870 616e 7369 6f6e 0a20 2020  er_expansion.   
+00002af0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00002b00: 2020 2023 2062 7974 6573 2c20 6574 630a     # bytes, etc.
+00002b10: 2020 2020 2020 2020 7261 6973 6520 4170          raise Ap
+00002b20: 6956 616c 7565 4572 726f 7228 2755 6e61  iValueError('Una
+00002b30: 626c 6520 746f 2067 656e 6572 6174 6520  ble to generate 
+00002b40: 6120 7265 6636 3537 3020 7265 7072 6573  a ref6570 repres
+00002b50: 656e 7461 7469 6f6e 206f 6620 7b7d 272e  entation of {}'.
+00002b60: 666f 726d 6174 2869 6e5f 6461 7461 2929  format(in_data))
+00002b70: 0a0a 0a63 6c61 7373 2053 7479 6c65 466f  ...class StyleFo
+00002b80: 726d 5365 7269 616c 697a 6572 2850 6172  rmSerializer(Par
+00002b90: 616d 6574 6572 5365 7269 616c 697a 6572  ameterSerializer
+00002ba0: 4261 7365 293a 0a20 2020 2040 636c 6173  Base):.    @clas
+00002bb0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00002bc0: 5f67 6574 5f64 6566 6175 6c74 5f65 7870  _get_default_exp
+00002bd0: 6c6f 6465 2863 6c73 2c20 7374 796c 653a  lode(cls, style:
+00002be0: 2050 6172 616d 6574 6572 5374 796c 6529   ParameterStyle)
+00002bf0: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00002c00: 2020 6966 2073 7479 6c65 2069 7320 5061    if style is Pa
+00002c10: 7261 6d65 7465 7253 7479 6c65 2e46 4f52  rameterStyle.FOR
+00002c20: 4d3a 0a20 2020 2020 2020 2020 2020 2072  M:.            r
+00002c30: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00002c40: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00002c50: 292e 5f67 6574 5f64 6566 6175 6c74 5f65  )._get_default_e
+00002c60: 7870 6c6f 6465 2873 7479 6c65 290a 0a20  xplode(style).. 
+00002c70: 2020 2064 6566 205f 7365 7269 616c 697a     def _serializ
+00002c80: 655f 666f 726d 280a 2020 2020 2020 2020  e_form(.        
+00002c90: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
+00002ca0: 5f64 6174 613a 2074 7970 696e 672e 556e  _data: typing.Un
+00002cb0: 696f 6e5b 4e6f 6e65 2c20 696e 742c 2066  ion[None, int, f
+00002cc0: 6c6f 6174 2c20 7374 722c 2062 6f6f 6c2c  loat, str, bool,
+00002cd0: 2064 6963 742c 206c 6973 745d 2c0a 2020   dict, list],.  
+00002ce0: 2020 2020 2020 6e61 6d65 3a20 7374 722c        name: str,
+00002cf0: 0a20 2020 2020 2020 2065 7870 6c6f 6465  .        explode
+00002d00: 3a20 626f 6f6c 2c0a 2020 2020 2020 2020  : bool,.        
+00002d10: 7065 7263 656e 745f 656e 636f 6465 3a20  percent_encode: 
+00002d20: 626f 6f6c 2c0a 2020 2020 2020 2020 7072  bool,.        pr
+00002d30: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00002d40: 7465 7261 746f 723a 2074 7970 696e 672e  terator: typing.
+00002d50: 4f70 7469 6f6e 616c 5b50 7265 6669 7853  Optional[PrefixS
+00002d60: 6570 6172 6174 6f72 4974 6572 6174 6f72  eparatorIterator
+00002d70: 5d20 3d20 4e6f 6e65 0a20 2020 2029 202d  ] = None.    ) -
+00002d80: 3e20 7374 723a 0a20 2020 2020 2020 2069  > str:.        i
+00002d90: 6620 7072 6566 6978 5f73 6570 6172 6174  f prefix_separat
+00002da0: 6f72 5f69 7465 7261 746f 7220 6973 204e  or_iterator is N
+00002db0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00002dc0: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
+00002dd0: 725f 6974 6572 6174 6f72 203d 2050 7265  r_iterator = Pre
+00002de0: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
+00002df0: 6174 6f72 2827 272c 2027 2627 290a 2020  ator('', '&').  
+00002e00: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00002e10: 662e 5f72 6566 3635 3730 5f65 7870 616e  f._ref6570_expan
+00002e20: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+00002e30: 2020 7661 7269 6162 6c65 5f6e 616d 653d    variable_name=
+00002e40: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00002e50: 2020 696e 5f64 6174 613d 696e 5f64 6174    in_data=in_dat
+00002e60: 612c 0a20 2020 2020 2020 2020 2020 2065  a,.            e
+00002e70: 7870 6c6f 6465 3d65 7870 6c6f 6465 2c0a  xplode=explode,.
+00002e80: 2020 2020 2020 2020 2020 2020 7065 7263              perc
+00002e90: 656e 745f 656e 636f 6465 3d70 6572 6365  ent_encode=perce
+00002ea0: 6e74 5f65 6e63 6f64 652c 0a20 2020 2020  nt_encode,.     
+00002eb0: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+00002ec0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00002ed0: 3d70 7265 6669 785f 7365 7061 7261 746f  =prefix_separato
+00002ee0: 725f 6974 6572 6174 6f72 0a20 2020 2020  r_iterator.     
+00002ef0: 2020 2029 0a0a 0a63 6c61 7373 2053 7479     )...class Sty
+00002f00: 6c65 5369 6d70 6c65 5365 7269 616c 697a  leSimpleSerializ
+00002f10: 6572 2850 6172 616d 6574 6572 5365 7269  er(ParameterSeri
+00002f20: 616c 697a 6572 4261 7365 293a 0a0a 2020  alizerBase):..  
+00002f30: 2020 6465 6620 5f73 6572 6961 6c69 7a65    def _serialize
+00002f40: 5f73 696d 706c 6528 0a20 2020 2020 2020  _simple(.       
+00002f50: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
+00002f60: 6e5f 6461 7461 3a20 7479 7069 6e67 2e55  n_data: typing.U
+00002f70: 6e69 6f6e 5b4e 6f6e 652c 2069 6e74 2c20  nion[None, int, 
+00002f80: 666c 6f61 742c 2073 7472 2c20 626f 6f6c  float, str, bool
+00002f90: 2c20 6469 6374 2c20 6c69 7374 5d2c 0a20  , dict, list],. 
+00002fa0: 2020 2020 2020 206e 616d 653a 2073 7472         name: str
+00002fb0: 2c0a 2020 2020 2020 2020 6578 706c 6f64  ,.        explod
+00002fc0: 653a 2062 6f6f 6c2c 0a20 2020 2020 2020  e: bool,.       
+00002fd0: 2070 6572 6365 6e74 5f65 6e63 6f64 653a   percent_encode:
+00002fe0: 2062 6f6f 6c0a 2020 2020 2920 2d3e 2073   bool.    ) -> s
+00002ff0: 7472 3a0a 2020 2020 2020 2020 7072 6566  tr:.        pref
+00003000: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00003010: 7261 746f 7220 3d20 5072 6566 6978 5365  rator = PrefixSe
+00003020: 7061 7261 746f 7249 7465 7261 746f 7228  paratorIterator(
+00003030: 2727 2c20 272c 2729 0a20 2020 2020 2020  '', ',').       
+00003040: 2072 6574 7572 6e20 7365 6c66 2e5f 7265   return self._re
+00003050: 6636 3537 305f 6578 7061 6e73 696f 6e28  f6570_expansion(
+00003060: 0a20 2020 2020 2020 2020 2020 2076 6172  .            var
+00003070: 6961 626c 655f 6e61 6d65 3d6e 616d 652c  iable_name=name,
+00003080: 0a20 2020 2020 2020 2020 2020 2069 6e5f  .            in_
+00003090: 6461 7461 3d69 6e5f 6461 7461 2c0a 2020  data=in_data,.  
+000030a0: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
+000030b0: 653d 6578 706c 6f64 652c 0a20 2020 2020  e=explode,.     
+000030c0: 2020 2020 2020 2070 6572 6365 6e74 5f65         percent_e
+000030d0: 6e63 6f64 653d 7065 7263 656e 745f 656e  ncode=percent_en
+000030e0: 636f 6465 2c0a 2020 2020 2020 2020 2020  code,.          
+000030f0: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+00003100: 6f72 5f69 7465 7261 746f 723d 7072 6566  or_iterator=pref
+00003110: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00003120: 7261 746f 720a 2020 2020 2020 2020 290a  rator.        ).
+00003130: 0a0a 636c 6173 7320 4a53 4f4e 4465 7465  ..class JSONDete
+00003140: 6374 6f72 3a0a 2020 2020 2222 220a 2020  ctor:.    """.  
+00003150: 2020 576f 726b 7320 666f 723a 0a20 2020    Works for:.   
+00003160: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
+00003170: 6e0a 2020 2020 6170 706c 6963 6174 696f  n.    applicatio
+00003180: 6e2f 6a73 6f6e 3b20 6368 6172 7365 743d  n/json; charset=
+00003190: 5554 462d 380a 2020 2020 6170 706c 6963  UTF-8.    applic
+000031a0: 6174 696f 6e2f 6a73 6f6e 2d70 6174 6368  ation/json-patch
+000031b0: 2b6a 736f 6e0a 2020 2020 6170 706c 6963  +json.    applic
+000031c0: 6174 696f 6e2f 6765 6f2b 6a73 6f6e 0a20  ation/geo+json. 
+000031d0: 2020 2022 2222 0a20 2020 205f 5f6a 736f     """.    __jso
+000031e0: 6e5f 636f 6e74 656e 745f 7479 7065 5f70  n_content_type_p
+000031f0: 6174 7465 726e 203d 2072 652e 636f 6d70  attern = re.comp
+00003200: 696c 6528 2261 7070 6c69 6361 7469 6f6e  ile("application
+00003210: 2f5b 5e2b 5d2a 5b2b 5d3f 286a 736f 6e29  /[^+]*[+]?(json)
+00003220: 3b3f 2e2a 2229 0a0a 2020 2020 4063 6c61  ;?.*")..    @cla
+00003230: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+00003240: 205f 636f 6e74 656e 745f 7479 7065 5f69   _content_type_i
+00003250: 735f 6a73 6f6e 2863 6c73 2c20 636f 6e74  s_json(cls, cont
+00003260: 656e 745f 7479 7065 3a20 7374 7229 202d  ent_type: str) -
+00003270: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00003280: 6966 2063 6c73 2e5f 5f6a 736f 6e5f 636f  if cls.__json_co
+00003290: 6e74 656e 745f 7479 7065 5f70 6174 7465  ntent_type_patte
+000032a0: 726e 2e6d 6174 6368 2863 6f6e 7465 6e74  rn.match(content
+000032b0: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
+000032c0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000032d0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000032e0: 616c 7365 0a0a 0a40 6461 7461 636c 6173  alse...@dataclas
+000032f0: 730a 636c 6173 7320 5061 7261 6d65 7465  s.class Paramete
+00003300: 7242 6173 6528 4a53 4f4e 4465 7465 6374  rBase(JSONDetect
+00003310: 6f72 293a 0a20 2020 206e 616d 653a 2073  or):.    name: s
+00003320: 7472 0a20 2020 2069 6e5f 7479 7065 3a20  tr.    in_type: 
+00003330: 5061 7261 6d65 7465 7249 6e54 7970 650a  ParameterInType.
+00003340: 2020 2020 7265 7175 6972 6564 3a20 626f      required: bo
+00003350: 6f6c 0a20 2020 2073 7479 6c65 3a20 7479  ol.    style: ty
+00003360: 7069 6e67 2e4f 7074 696f 6e61 6c5b 5061  ping.Optional[Pa
+00003370: 7261 6d65 7465 7253 7479 6c65 5d0a 2020  rameterStyle].  
+00003380: 2020 6578 706c 6f64 653a 2074 7970 696e    explode: typin
+00003390: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
+000033a0: 0a20 2020 2061 6c6c 6f77 5f72 6573 6572  .    allow_reser
+000033b0: 7665 643a 2074 7970 696e 672e 4f70 7469  ved: typing.Opti
+000033c0: 6f6e 616c 5b62 6f6f 6c5d 0a20 2020 2073  onal[bool].    s
+000033d0: 6368 656d 613a 2074 7970 696e 672e 4f70  chema: typing.Op
+000033e0: 7469 6f6e 616c 5b74 7970 696e 672e 5479  tional[typing.Ty
+000033f0: 7065 5b53 6368 656d 615d 5d0a 2020 2020  pe[Schema]].    
+00003400: 636f 6e74 656e 743a 2074 7970 696e 672e  content: typing.
+00003410: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00003420: 4469 6374 5b73 7472 2c20 7479 7069 6e67  Dict[str, typing
+00003430: 2e54 7970 655b 5363 6865 6d61 5d5d 5d0a  .Type[Schema]]].
+00003440: 0a20 2020 205f 5f73 7479 6c65 5f74 6f5f  .    __style_to_
+00003450: 696e 5f74 7970 6520 3d20 7b0a 2020 2020  in_type = {.    
+00003460: 2020 2020 5061 7261 6d65 7465 7253 7479      ParameterSty
+00003470: 6c65 2e4d 4154 5249 583a 207b 5061 7261  le.MATRIX: {Para
+00003480: 6d65 7465 7249 6e54 7970 652e 5041 5448  meterInType.PATH
+00003490: 7d2c 0a20 2020 2020 2020 2050 6172 616d  },.        Param
+000034a0: 6574 6572 5374 796c 652e 4c41 4245 4c3a  eterStyle.LABEL:
 000034b0: 207b 5061 7261 6d65 7465 7249 6e54 7970   {ParameterInTyp
-000034c0: 652e 5155 4552 597d 2c0a 2020 2020 2020  e.QUERY},.      
-000034d0: 2020 5061 7261 6d65 7465 7253 7479 6c65    ParameterStyle
-000034e0: 2e44 4545 505f 4f42 4a45 4354 3a20 7b50  .DEEP_OBJECT: {P
-000034f0: 6172 616d 6574 6572 496e 5479 7065 2e51  arameterInType.Q
-00003500: 5545 5259 7d2c 0a20 2020 207d 0a20 2020  UERY},.    }.   
-00003510: 205f 5f69 6e5f 7479 7065 5f74 6f5f 6465   __in_type_to_de
-00003520: 6661 756c 745f 7374 796c 6520 3d20 7b0a  fault_style = {.
-00003530: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00003540: 7249 6e54 7970 652e 5155 4552 593a 2050  rInType.QUERY: P
-00003550: 6172 616d 6574 6572 5374 796c 652e 464f  arameterStyle.FO
-00003560: 524d 2c0a 2020 2020 2020 2020 5061 7261  RM,.        Para
-00003570: 6d65 7465 7249 6e54 7970 652e 5041 5448  meterInType.PATH
-00003580: 3a20 5061 7261 6d65 7465 7253 7479 6c65  : ParameterStyle
-00003590: 2e53 494d 504c 452c 0a20 2020 2020 2020  .SIMPLE,.       
-000035a0: 2050 6172 616d 6574 6572 496e 5479 7065   ParameterInType
-000035b0: 2e48 4541 4445 523a 2050 6172 616d 6574  .HEADER: Paramet
-000035c0: 6572 5374 796c 652e 5349 4d50 4c45 2c0a  erStyle.SIMPLE,.
-000035d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000035e0: 7249 6e54 7970 652e 434f 4f4b 4945 3a20  rInType.COOKIE: 
-000035f0: 5061 7261 6d65 7465 7253 7479 6c65 2e46  ParameterStyle.F
-00003600: 4f52 4d2c 0a20 2020 207d 0a20 2020 205f  ORM,.    }.    _
-00003610: 5f64 6973 616c 6c6f 7765 645f 6865 6164  _disallowed_head
-00003620: 6572 5f6e 616d 6573 203d 207b 2741 6363  er_names = {'Acc
-00003630: 6570 7427 2c20 2743 6f6e 7465 6e74 2d54  ept', 'Content-T
-00003640: 7970 6527 2c20 2741 7574 686f 7269 7a61  ype', 'Authoriza
-00003650: 7469 6f6e 277d 0a20 2020 205f 6a73 6f6e  tion'}.    _json
-00003660: 5f65 6e63 6f64 6572 203d 204a 534f 4e45  _encoder = JSONE
-00003670: 6e63 6f64 6572 2829 0a0a 2020 2020 4063  ncoder()..    @c
-00003680: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00003690: 6566 205f 5f76 6572 6966 795f 7374 796c  ef __verify_styl
-000036a0: 655f 746f 5f69 6e5f 7479 7065 2863 6c73  e_to_in_type(cls
-000036b0: 2c20 7374 796c 653a 2074 7970 696e 672e  , style: typing.
-000036c0: 4f70 7469 6f6e 616c 5b50 6172 616d 6574  Optional[Paramet
-000036d0: 6572 5374 796c 655d 2c20 696e 5f74 7970  erStyle], in_typ
-000036e0: 653a 2050 6172 616d 6574 6572 496e 5479  e: ParameterInTy
-000036f0: 7065 293a 0a20 2020 2020 2020 2069 6620  pe):.        if 
-00003700: 7374 796c 6520 6973 204e 6f6e 653a 0a20  style is None:. 
-00003710: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003720: 6e0a 2020 2020 2020 2020 696e 5f74 7970  n.        in_typ
-00003730: 655f 7365 7420 3d20 636c 732e 5f5f 7374  e_set = cls.__st
-00003740: 796c 655f 746f 5f69 6e5f 7479 7065 5b73  yle_to_in_type[s
-00003750: 7479 6c65 5d0a 2020 2020 2020 2020 6966  tyle].        if
-00003760: 2069 6e5f 7479 7065 206e 6f74 2069 6e20   in_type not in 
-00003770: 696e 5f74 7970 655f 7365 743a 0a20 2020  in_type_set:.   
-00003780: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00003790: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-000037a0: 2020 2020 2020 2020 2020 2027 496e 7661             'Inva
-000037b0: 6c69 6420 7374 796c 6520 616e 6420 696e  lid style and in
-000037c0: 5f74 7970 6520 636f 6d62 696e 6174 696f  _type combinatio
-000037d0: 6e2e 2046 6f72 2073 7479 6c65 3d7b 7d20  n. For style={} 
-000037e0: 6f6e 6c79 2069 6e5f 7479 7065 3d7b 7d20  only in_type={} 
-000037f0: 6172 6520 616c 6c6f 7765 6427 2e66 6f72  are allowed'.for
-00003800: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
-00003810: 2020 2020 2020 2020 2073 7479 6c65 2c20           style, 
-00003820: 696e 5f74 7970 655f 7365 740a 2020 2020  in_type_set.    
-00003830: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00003840: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00003850: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00003860: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00003870: 2020 2020 206e 616d 653a 2073 7472 2c0a       name: str,.
-00003880: 2020 2020 2020 2020 696e 5f74 7970 653a          in_type:
-00003890: 2050 6172 616d 6574 6572 496e 5479 7065   ParameterInType
-000038a0: 2c0a 2020 2020 2020 2020 7265 7175 6972  ,.        requir
-000038b0: 6564 3a20 626f 6f6c 203d 2046 616c 7365  ed: bool = False
-000038c0: 2c0a 2020 2020 2020 2020 7374 796c 653a  ,.        style:
-000038d0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000038e0: 5b50 6172 616d 6574 6572 5374 796c 655d  [ParameterStyle]
-000038f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00003900: 2065 7870 6c6f 6465 3a20 626f 6f6c 203d   explode: bool =
-00003910: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00003920: 616c 6c6f 775f 7265 7365 7276 6564 3a20  allow_reserved: 
-00003930: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00003940: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020  bool] = None,.  
-00003950: 2020 2020 2020 7363 6865 6d61 3a20 7479        schema: ty
-00003960: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
-00003970: 7069 6e67 2e54 7970 655b 5363 6865 6d61  ping.Type[Schema
-00003980: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00003990: 2020 2063 6f6e 7465 6e74 3a20 7479 7069     content: typi
-000039a0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-000039b0: 6e67 2e44 6963 745b 7374 722c 2074 7970  ng.Dict[str, typ
-000039c0: 696e 672e 5479 7065 5b53 6368 656d 615d  ing.Type[Schema]
-000039d0: 5d5d 203d 204e 6f6e 650a 2020 2020 293a  ]] = None.    ):
-000039e0: 0a20 2020 2020 2020 2069 6620 7363 6865  .        if sche
-000039f0: 6d61 2069 7320 4e6f 6e65 2061 6e64 2063  ma is None and c
-00003a00: 6f6e 7465 6e74 2069 7320 4e6f 6e65 3a0a  ontent is None:.
-00003a10: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00003a20: 6520 5661 6c75 6545 7272 6f72 2827 5661  e ValueError('Va
-00003a30: 6c75 6520 6d69 7373 696e 673b 2050 6173  lue missing; Pas
-00003a40: 7320 696e 2065 6974 6865 7220 7363 6865  s in either sche
-00003a50: 6d61 206f 7220 636f 6e74 656e 7427 290a  ma or content').
-00003a60: 2020 2020 2020 2020 6966 2073 6368 656d          if schem
-00003a70: 6120 616e 6420 636f 6e74 656e 743a 0a20  a and content:. 
-00003a80: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003a90: 2056 616c 7565 4572 726f 7228 2754 6f6f   ValueError('Too
-00003aa0: 206d 616e 7920 7661 6c75 6573 2070 726f   many values pro
-00003ab0: 7669 6465 642e 2042 6f74 6820 7363 6865  vided. Both sche
-00003ac0: 6d61 2061 6e64 2063 6f6e 7465 6e74 2077  ma and content w
-00003ad0: 6572 6520 7072 6f76 6964 6564 2e20 4f6e  ere provided. On
-00003ae0: 6c79 206f 6e65 206d 6179 2062 6520 696e  ly one may be in
-00003af0: 7075 7427 290a 2020 2020 2020 2020 6966  put').        if
-00003b00: 206e 616d 6520 696e 2073 656c 662e 5f5f   name in self.__
-00003b10: 6469 7361 6c6c 6f77 6564 5f68 6561 6465  disallowed_heade
-00003b20: 725f 6e61 6d65 7320 616e 6420 696e 5f74  r_names and in_t
-00003b30: 7970 6520 6973 2050 6172 616d 6574 6572  ype is Parameter
-00003b40: 496e 5479 7065 2e48 4541 4445 523a 0a20  InType.HEADER:. 
-00003b50: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00003b60: 2056 616c 7565 4572 726f 7228 2749 6e76   ValueError('Inv
-00003b70: 616c 6964 206e 616d 652c 206e 616d 6520  alid name, name 
-00003b80: 6d61 7920 6e6f 7420 6265 206f 6e65 206f  may not be one o
-00003b90: 6620 7b7d 272e 666f 726d 6174 2873 656c  f {}'.format(sel
-00003ba0: 662e 5f5f 6469 7361 6c6c 6f77 6564 5f68  f.__disallowed_h
-00003bb0: 6561 6465 725f 6e61 6d65 7329 290a 2020  eader_names)).  
-00003bc0: 2020 2020 2020 7365 6c66 2e5f 5f76 6572        self.__ver
-00003bd0: 6966 795f 7374 796c 655f 746f 5f69 6e5f  ify_style_to_in_
-00003be0: 7479 7065 2873 7479 6c65 2c20 696e 5f74  type(style, in_t
-00003bf0: 7970 6529 0a20 2020 2020 2020 2069 6620  ype).        if 
-00003c00: 636f 6e74 656e 7420 6973 204e 6f6e 6520  content is None 
-00003c10: 616e 6420 7374 796c 6520 6973 204e 6f6e  and style is Non
-00003c20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00003c30: 7479 6c65 203d 2073 656c 662e 5f5f 696e  tyle = self.__in
-00003c40: 5f74 7970 655f 746f 5f64 6566 6175 6c74  _type_to_default
-00003c50: 5f73 7479 6c65 5b69 6e5f 7479 7065 5d0a  _style[in_type].
-00003c60: 2020 2020 2020 2020 6966 2063 6f6e 7465          if conte
-00003c70: 6e74 2069 7320 6e6f 7420 4e6f 6e65 2061  nt is not None a
-00003c80: 6e64 2069 6e5f 7479 7065 2069 6e20 7365  nd in_type in se
-00003c90: 6c66 2e5f 5f69 6e5f 7479 7065 5f74 6f5f  lf.__in_type_to_
-00003ca0: 6465 6661 756c 745f 7374 796c 6520 616e  default_style an
-00003cb0: 6420 6c65 6e28 636f 6e74 656e 7429 2021  d len(content) !
-00003cc0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00003cd0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00003ce0: 7228 2749 6e76 616c 6964 2063 6f6e 7465  r('Invalid conte
-00003cf0: 6e74 206c 656e 6774 682c 2063 6f6e 7465  nt length, conte
-00003d00: 6e74 206c 656e 6774 6820 6d75 7374 2065  nt length must e
-00003d10: 7175 616c 2031 2729 0a20 2020 2020 2020  qual 1').       
-00003d20: 2073 656c 662e 696e 5f74 7970 6520 3d20   self.in_type = 
-00003d30: 696e 5f74 7970 650a 2020 2020 2020 2020  in_type.        
-00003d40: 7365 6c66 2e6e 616d 6520 3d20 6e61 6d65  self.name = name
-00003d50: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00003d60: 7175 6972 6564 203d 2072 6571 7569 7265  quired = require
-00003d70: 640a 2020 2020 2020 2020 7365 6c66 2e73  d.        self.s
-00003d80: 7479 6c65 203d 2073 7479 6c65 0a20 2020  tyle = style.   
-00003d90: 2020 2020 2073 656c 662e 6578 706c 6f64       self.explod
-00003da0: 6520 3d20 6578 706c 6f64 650a 2020 2020  e = explode.    
-00003db0: 2020 2020 7365 6c66 2e61 6c6c 6f77 5f72      self.allow_r
-00003dc0: 6573 6572 7665 6420 3d20 616c 6c6f 775f  eserved = allow_
-00003dd0: 7265 7365 7276 6564 0a20 2020 2020 2020  reserved.       
-00003de0: 2073 656c 662e 7363 6865 6d61 203d 2073   self.schema = s
-00003df0: 6368 656d 610a 2020 2020 2020 2020 7365  chema.        se
-00003e00: 6c66 2e63 6f6e 7465 6e74 203d 2063 6f6e  lf.content = con
-00003e10: 7465 6e74 0a0a 2020 2020 6465 6620 5f73  tent..    def _s
-00003e20: 6572 6961 6c69 7a65 5f6a 736f 6e28 0a20  erialize_json(. 
-00003e30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00003e40: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
-00003e50: 7069 6e67 2e55 6e69 6f6e 5b4e 6f6e 652c  ping.Union[None,
-00003e60: 2069 6e74 2c20 666c 6f61 742c 2073 7472   int, float, str
-00003e70: 2c20 626f 6f6c 2c20 6469 6374 2c20 6c69  , bool, dict, li
-00003e80: 7374 5d2c 0a20 2020 2020 2020 2065 6c69  st],.        eli
-00003e90: 6d69 6e61 7465 5f77 6869 7465 7370 6163  minate_whitespac
-00003ea0: 653a 2062 6f6f 6c20 3d20 4661 6c73 650a  e: bool = False.
-00003eb0: 2020 2020 2920 2d3e 2073 7472 3a0a 2020      ) -> str:.  
-00003ec0: 2020 2020 2020 6966 2065 6c69 6d69 6e61        if elimina
-00003ed0: 7465 5f77 6869 7465 7370 6163 653a 0a20  te_whitespace:. 
-00003ee0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003ef0: 6e20 6a73 6f6e 2e64 756d 7073 2869 6e5f  n json.dumps(in_
-00003f00: 6461 7461 2c20 7365 7061 7261 746f 7273  data, separators
-00003f10: 3d73 656c 662e 5f6a 736f 6e5f 656e 636f  =self._json_enco
-00003f20: 6465 722e 636f 6d70 6163 745f 7365 7061  der.compact_sepa
-00003f30: 7261 746f 7273 290a 2020 2020 2020 2020  rators).        
-00003f40: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
-00003f50: 7328 696e 5f64 6174 6129 0a0a 0a63 6c61  s(in_data)...cla
-00003f60: 7373 2050 6174 6850 6172 616d 6574 6572  ss PathParameter
-00003f70: 2850 6172 616d 6574 6572 4261 7365 2c20  (ParameterBase, 
-00003f80: 5374 796c 6553 696d 706c 6553 6572 6961  StyleSimpleSeria
-00003f90: 6c69 7a65 7229 3a0a 0a20 2020 2064 6566  lizer):..    def
-00003fa0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-00003fb0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00003fc0: 206e 616d 653a 2073 7472 2c0a 2020 2020   name: str,.    
-00003fd0: 2020 2020 7265 7175 6972 6564 3a20 626f      required: bo
-00003fe0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
-00003ff0: 2020 2020 7374 796c 653a 2074 7970 696e      style: typin
-00004000: 672e 4f70 7469 6f6e 616c 5b50 6172 616d  g.Optional[Param
-00004010: 6574 6572 5374 796c 655d 203d 204e 6f6e  eterStyle] = Non
-00004020: 652c 0a20 2020 2020 2020 2065 7870 6c6f  e,.        explo
-00004030: 6465 3a20 626f 6f6c 203d 2046 616c 7365  de: bool = False
-00004040: 2c0a 2020 2020 2020 2020 616c 6c6f 775f  ,.        allow_
-00004050: 7265 7365 7276 6564 3a20 7479 7069 6e67  reserved: typing
-00004060: 2e4f 7074 696f 6e61 6c5b 626f 6f6c 5d20  .Optional[bool] 
-00004070: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00004080: 7363 6865 6d61 3a20 7479 7069 6e67 2e4f  schema: typing.O
-00004090: 7074 696f 6e61 6c5b 7479 7069 6e67 2e54  ptional[typing.T
-000040a0: 7970 655b 5363 6865 6d61 5d5d 203d 204e  ype[Schema]] = N
-000040b0: 6f6e 652c 0a20 2020 2020 2020 2063 6f6e  one,.        con
-000040c0: 7465 6e74 3a20 7479 7069 6e67 2e4f 7074  tent: typing.Opt
-000040d0: 696f 6e61 6c5b 7479 7069 6e67 2e44 6963  ional[typing.Dic
-000040e0: 745b 7374 722c 2074 7970 696e 672e 5479  t[str, typing.Ty
-000040f0: 7065 5b53 6368 656d 615d 5d5d 203d 204e  pe[Schema]]] = N
-00004100: 6f6e 650a 2020 2020 293a 0a20 2020 2020  one.    ):.     
-00004110: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-00004120: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
-00004130: 206e 616d 652c 0a20 2020 2020 2020 2020   name,.         
-00004140: 2020 2069 6e5f 7479 7065 3d50 6172 616d     in_type=Param
-00004150: 6574 6572 496e 5479 7065 2e50 4154 482c  eterInType.PATH,
-00004160: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00004170: 7569 7265 643d 7265 7175 6972 6564 2c0a  uired=required,.
-00004180: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00004190: 653d 7374 796c 652c 0a20 2020 2020 2020  e=style,.       
-000041a0: 2020 2020 2065 7870 6c6f 6465 3d65 7870       explode=exp
-000041b0: 6c6f 6465 2c0a 2020 2020 2020 2020 2020  lode,.          
-000041c0: 2020 616c 6c6f 775f 7265 7365 7276 6564    allow_reserved
-000041d0: 3d61 6c6c 6f77 5f72 6573 6572 7665 642c  =allow_reserved,
-000041e0: 0a20 2020 2020 2020 2020 2020 2073 6368  .            sch
-000041f0: 656d 613d 7363 6865 6d61 2c0a 2020 2020  ema=schema,.    
-00004200: 2020 2020 2020 2020 636f 6e74 656e 743d          content=
-00004210: 636f 6e74 656e 740a 2020 2020 2020 2020  content.        
-00004220: 290a 0a20 2020 2064 6566 205f 5f73 6572  )..    def __ser
-00004230: 6961 6c69 7a65 5f6c 6162 656c 280a 2020  ialize_label(.  
-00004240: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00004250: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
-00004260: 696e 672e 556e 696f 6e5b 4e6f 6e65 2c20  ing.Union[None, 
-00004270: 696e 742c 2066 6c6f 6174 2c20 7374 722c  int, float, str,
-00004280: 2062 6f6f 6c2c 2064 6963 742c 206c 6973   bool, dict, lis
-00004290: 745d 0a20 2020 2029 202d 3e20 7479 7069  t].    ) -> typi
-000042a0: 6e67 2e44 6963 745b 7374 722c 2073 7472  ng.Dict[str, str
-000042b0: 5d3a 0a20 2020 2020 2020 2070 7265 6669  ]:.        prefi
-000042c0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-000042d0: 6174 6f72 203d 2050 7265 6669 7853 6570  ator = PrefixSep
-000042e0: 6172 6174 6f72 4974 6572 6174 6f72 2827  aratorIterator('
-000042f0: 2e27 2c20 272e 2729 0a20 2020 2020 2020  .', '.').       
-00004300: 2076 616c 7565 203d 2073 656c 662e 5f72   value = self._r
-00004310: 6566 3635 3730 5f65 7870 616e 7369 6f6e  ef6570_expansion
-00004320: 280a 2020 2020 2020 2020 2020 2020 7661  (.            va
-00004330: 7269 6162 6c65 5f6e 616d 653d 7365 6c66  riable_name=self
-00004340: 2e6e 616d 652c 0a20 2020 2020 2020 2020  .name,.         
-00004350: 2020 2069 6e5f 6461 7461 3d69 6e5f 6461     in_data=in_da
-00004360: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00004370: 6578 706c 6f64 653d 7365 6c66 2e65 7870  explode=self.exp
-00004380: 6c6f 6465 2c0a 2020 2020 2020 2020 2020  lode,.          
-00004390: 2020 7065 7263 656e 745f 656e 636f 6465    percent_encode
-000043a0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000043b0: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-000043c0: 746f 725f 6974 6572 6174 6f72 3d70 7265  tor_iterator=pre
-000043d0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-000043e0: 6572 6174 6f72 0a20 2020 2020 2020 2029  erator.        )
-000043f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004400: 7365 6c66 2e5f 746f 5f64 6963 7428 7365  self._to_dict(se
-00004410: 6c66 2e6e 616d 652c 2076 616c 7565 290a  lf.name, value).
-00004420: 0a20 2020 2064 6566 205f 5f73 6572 6961  .    def __seria
-00004430: 6c69 7a65 5f6d 6174 7269 7828 0a20 2020  lize_matrix(.   
-00004440: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00004450: 2020 2069 6e5f 6461 7461 3a20 7479 7069     in_data: typi
-00004460: 6e67 2e55 6e69 6f6e 5b4e 6f6e 652c 2069  ng.Union[None, i
-00004470: 6e74 2c20 666c 6f61 742c 2073 7472 2c20  nt, float, str, 
-00004480: 626f 6f6c 2c20 6469 6374 2c20 6c69 7374  bool, dict, list
-00004490: 5d0a 2020 2020 2920 2d3e 2074 7970 696e  ].    ) -> typin
-000044a0: 672e 4469 6374 5b73 7472 2c20 7374 725d  g.Dict[str, str]
-000044b0: 3a0a 2020 2020 2020 2020 7072 6566 6978  :.        prefix
-000044c0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-000044d0: 746f 7220 3d20 5072 6566 6978 5365 7061  tor = PrefixSepa
-000044e0: 7261 746f 7249 7465 7261 746f 7228 273b  ratorIterator(';
-000044f0: 272c 2027 3b27 290a 2020 2020 2020 2020  ', ';').        
-00004500: 7661 6c75 6520 3d20 7365 6c66 2e5f 7265  value = self._re
-00004510: 6636 3537 305f 6578 7061 6e73 696f 6e28  f6570_expansion(
-00004520: 0a20 2020 2020 2020 2020 2020 2076 6172  .            var
-00004530: 6961 626c 655f 6e61 6d65 3d73 656c 662e  iable_name=self.
-00004540: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-00004550: 2020 696e 5f64 6174 613d 696e 5f64 6174    in_data=in_dat
-00004560: 612c 0a20 2020 2020 2020 2020 2020 2065  a,.            e
-00004570: 7870 6c6f 6465 3d73 656c 662e 6578 706c  xplode=self.expl
-00004580: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
-00004590: 2070 6572 6365 6e74 5f65 6e63 6f64 653d   percent_encode=
-000045a0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-000045b0: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
-000045c0: 6f72 5f69 7465 7261 746f 723d 7072 6566  or_iterator=pref
-000045d0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-000045e0: 7261 746f 720a 2020 2020 2020 2020 290a  rator.        ).
-000045f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00004600: 656c 662e 5f74 6f5f 6469 6374 2873 656c  elf._to_dict(sel
-00004610: 662e 6e61 6d65 2c20 7661 6c75 6529 0a0a  f.name, value)..
-00004620: 2020 2020 6465 6620 5f5f 7365 7269 616c      def __serial
-00004630: 697a 655f 7369 6d70 6c65 280a 2020 2020  ize_simple(.    
-00004640: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00004650: 2020 696e 5f64 6174 613a 2074 7970 696e    in_data: typin
-00004660: 672e 556e 696f 6e5b 4e6f 6e65 2c20 696e  g.Union[None, in
-00004670: 742c 2066 6c6f 6174 2c20 7374 722c 2062  t, float, str, b
-00004680: 6f6f 6c2c 2064 6963 742c 206c 6973 745d  ool, dict, list]
-00004690: 2c0a 2020 2020 2920 2d3e 2074 7970 696e  ,.    ) -> typin
-000046a0: 672e 4469 6374 5b73 7472 2c20 7374 725d  g.Dict[str, str]
-000046b0: 3a0a 2020 2020 2020 2020 7661 6c75 6520  :.        value 
-000046c0: 3d20 7365 6c66 2e5f 7365 7269 616c 697a  = self._serializ
-000046d0: 655f 7369 6d70 6c65 280a 2020 2020 2020  e_simple(.      
-000046e0: 2020 2020 2020 696e 5f64 6174 613d 696e        in_data=in
-000046f0: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
-00004700: 2020 206e 616d 653d 7365 6c66 2e6e 616d     name=self.nam
-00004710: 652c 0a20 2020 2020 2020 2020 2020 2065  e,.            e
-00004720: 7870 6c6f 6465 3d73 656c 662e 6578 706c  xplode=self.expl
-00004730: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
-00004740: 2070 6572 6365 6e74 5f65 6e63 6f64 653d   percent_encode=
-00004750: 5472 7565 0a20 2020 2020 2020 2029 0a20  True.        ). 
-00004760: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00004770: 6c66 2e5f 746f 5f64 6963 7428 7365 6c66  lf._to_dict(self
-00004780: 2e6e 616d 652c 2076 616c 7565 290a 0a20  .name, value).. 
-00004790: 2020 2064 6566 2073 6572 6961 6c69 7a65     def serialize
-000047a0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-000047b0: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
-000047c0: 2074 7970 696e 672e 556e 696f 6e5b 0a20   typing.Union[. 
-000047d0: 2020 2020 2020 2020 2020 2053 6368 656d             Schem
-000047e0: 612c 2044 6563 696d 616c 2c20 696e 742c  a, Decimal, int,
-000047f0: 2066 6c6f 6174 2c20 7374 722c 2064 6174   float, str, dat
-00004800: 652c 2064 6174 6574 696d 652c 204e 6f6e  e, datetime, Non
-00004810: 652c 2062 6f6f 6c2c 206c 6973 742c 2074  e, bool, list, t
-00004820: 7570 6c65 2c20 6469 6374 2c20 6672 6f7a  uple, dict, froz
-00004830: 656e 6469 6374 2e66 726f 7a65 6e64 6963  endict.frozendic
-00004840: 745d 0a20 2020 2029 202d 3e20 7479 7069  t].    ) -> typi
-00004850: 6e67 2e44 6963 745b 7374 722c 2073 7472  ng.Dict[str, str
-00004860: 5d3a 0a20 2020 2020 2020 2069 6620 7365  ]:.        if se
-00004870: 6c66 2e73 6368 656d 613a 0a20 2020 2020  lf.schema:.     
-00004880: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
-00004890: 6174 6120 3d20 7365 6c66 2e73 6368 656d  ata = self.schem
-000048a0: 6128 696e 5f64 6174 6129 0a20 2020 2020  a(in_data).     
-000048b0: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
-000048c0: 6174 6120 3d20 7365 6c66 2e5f 6a73 6f6e  ata = self._json
-000048d0: 5f65 6e63 6f64 6572 2e64 6566 6175 6c74  _encoder.default
-000048e0: 2863 6173 745f 696e 5f64 6174 6129 0a20  (cast_in_data). 
-000048f0: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-00004900: 2020 2020 2020 2020 2020 2073 696d 706c             simpl
-00004910: 6520 2d3e 2070 6174 680a 2020 2020 2020  e -> path.      
-00004920: 2020 2020 2020 2020 2020 7061 7468 3a0a            path:.
-00004930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004940: 2020 2020 7265 7475 726e 7320 7061 7468      returns path
-00004950: 5f70 6172 616d 733a 2064 6963 740a 2020  _params: dict.  
-00004960: 2020 2020 2020 2020 2020 6c61 6265 6c20            label 
-00004970: 2d3e 2070 6174 680a 2020 2020 2020 2020  -> path.        
-00004980: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-00004990: 7061 7468 5f70 6172 616d 730a 2020 2020  path_params.    
-000049a0: 2020 2020 2020 2020 6d61 7472 6978 202d          matrix -
-000049b0: 3e20 7061 7468 0a20 2020 2020 2020 2020  > path.         
-000049c0: 2020 2020 2020 2072 6574 7572 6e73 2070         returns p
-000049d0: 6174 685f 7061 7261 6d73 0a20 2020 2020  ath_params.     
-000049e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000049f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00004a00: 7479 6c65 3a0a 2020 2020 2020 2020 2020  tyle:.          
-00004a10: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00004a20: 796c 6520 6973 2050 6172 616d 6574 6572  yle is Parameter
-00004a30: 5374 796c 652e 5349 4d50 4c45 3a0a 2020  Style.SIMPLE:.  
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
-00004a60: 7365 7269 616c 697a 655f 7369 6d70 6c65  serialize_simple
-00004a70: 2863 6173 745f 696e 5f64 6174 6129 0a20  (cast_in_data). 
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00004a90: 6c69 6620 7365 6c66 2e73 7479 6c65 2069  lif self.style i
-00004aa0: 7320 5061 7261 6d65 7465 7253 7479 6c65  s ParameterStyle
-00004ab0: 2e4c 4142 454c 3a0a 2020 2020 2020 2020  .LABEL:.        
-00004ac0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00004ad0: 726e 2073 656c 662e 5f5f 7365 7269 616c  rn self.__serial
-00004ae0: 697a 655f 6c61 6265 6c28 6361 7374 5f69  ize_label(cast_i
-00004af0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
-00004b00: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-00004b10: 662e 7374 796c 6520 6973 2050 6172 616d  f.style is Param
-00004b20: 6574 6572 5374 796c 652e 4d41 5452 4958  eterStyle.MATRIX
-00004b30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004b40: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004b50: 662e 5f5f 7365 7269 616c 697a 655f 6d61  f.__serialize_ma
-00004b60: 7472 6978 2863 6173 745f 696e 5f64 6174  trix(cast_in_dat
-00004b70: 6129 0a20 2020 2020 2020 2023 2073 656c  a).        # sel
-00004b80: 662e 636f 6e74 656e 7420 7769 6c6c 2062  f.content will b
-00004b90: 6520 6c65 6e67 7468 206f 6e65 0a20 2020  e length one.   
-00004ba0: 2020 2020 2066 6f72 2063 6f6e 7465 6e74       for content
-00004bb0: 5f74 7970 652c 2073 6368 656d 6120 696e  _type, schema in
-00004bc0: 2073 656c 662e 636f 6e74 656e 742e 6974   self.content.it
-00004bd0: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00004be0: 2020 2063 6173 745f 696e 5f64 6174 6120     cast_in_data 
-00004bf0: 3d20 7363 6865 6d61 2869 6e5f 6461 7461  = schema(in_data
-00004c00: 290a 2020 2020 2020 2020 2020 2020 6361  ).            ca
-00004c10: 7374 5f69 6e5f 6461 7461 203d 2073 656c  st_in_data = sel
-00004c20: 662e 5f6a 736f 6e5f 656e 636f 6465 722e  f._json_encoder.
-00004c30: 6465 6661 756c 7428 6361 7374 5f69 6e5f  default(cast_in_
-00004c40: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00004c50: 2020 6966 2073 656c 662e 5f63 6f6e 7465    if self._conte
-00004c60: 6e74 5f74 7970 655f 6973 5f6a 736f 6e28  nt_type_is_json(
-00004c70: 636f 6e74 656e 745f 7479 7065 293a 0a20  content_type):. 
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00004c90: 616c 7565 203d 2073 656c 662e 5f73 6572  alue = self._ser
-00004ca0: 6961 6c69 7a65 5f6a 736f 6e28 6361 7374  ialize_json(cast
-00004cb0: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
-00004cc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00004cd0: 2073 656c 662e 5f74 6f5f 6469 6374 2873   self._to_dict(s
-00004ce0: 656c 662e 6e61 6d65 2c20 7661 6c75 6529  elf.name, value)
-00004cf0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00004d00: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00004d10: 6445 7272 6f72 2827 5365 7269 616c 697a  dError('Serializ
-00004d20: 6174 696f 6e20 6f66 207b 7d20 6861 7320  ation of {} has 
-00004d30: 6e6f 7420 7965 7420 6265 656e 2069 6d70  not yet been imp
-00004d40: 6c65 6d65 6e74 6564 272e 666f 726d 6174  lemented'.format
-00004d50: 2863 6f6e 7465 6e74 5f74 7970 6529 290a  (content_type)).
-00004d60: 0a0a 636c 6173 7320 5175 6572 7950 6172  ..class QueryPar
-00004d70: 616d 6574 6572 2850 6172 616d 6574 6572  ameter(Parameter
-00004d80: 4261 7365 2c20 5374 796c 6546 6f72 6d53  Base, StyleFormS
-00004d90: 6572 6961 6c69 7a65 7229 3a0a 0a20 2020  erializer):..   
-00004da0: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-00004db0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00004dc0: 2020 2020 206e 616d 653a 2073 7472 2c0a       name: str,.
-00004dd0: 2020 2020 2020 2020 7265 7175 6972 6564          required
-00004de0: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
-00004df0: 2020 2020 2020 2020 7374 796c 653a 2074          style: t
-00004e00: 7970 696e 672e 4f70 7469 6f6e 616c 5b50  yping.Optional[P
-00004e10: 6172 616d 6574 6572 5374 796c 655d 203d  arameterStyle] =
-00004e20: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00004e30: 7870 6c6f 6465 3a20 7479 7069 6e67 2e4f  xplode: typing.O
-00004e40: 7074 696f 6e61 6c5b 626f 6f6c 5d20 3d20  ptional[bool] = 
-00004e50: 4e6f 6e65 2c0a 2020 2020 2020 2020 616c  None,.        al
-00004e60: 6c6f 775f 7265 7365 7276 6564 3a20 7479  low_reserved: ty
-00004e70: 7069 6e67 2e4f 7074 696f 6e61 6c5b 626f  ping.Optional[bo
-00004e80: 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ol] = None,.    
-00004e90: 2020 2020 7363 6865 6d61 3a20 7479 7069      schema: typi
-00004ea0: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00004eb0: 6e67 2e54 7970 655b 5363 6865 6d61 5d5d  ng.Type[Schema]]
-00004ec0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00004ed0: 2063 6f6e 7465 6e74 3a20 7479 7069 6e67   content: typing
-00004ee0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00004ef0: 2e44 6963 745b 7374 722c 2074 7970 696e  .Dict[str, typin
-00004f00: 672e 5479 7065 5b53 6368 656d 615d 5d5d  g.Type[Schema]]]
-00004f10: 203d 204e 6f6e 650a 2020 2020 293a 0a20   = None.    ):. 
-00004f20: 2020 2020 2020 2075 7365 645f 7374 796c         used_styl
-00004f30: 6520 3d20 5061 7261 6d65 7465 7253 7479  e = ParameterSty
-00004f40: 6c65 2e46 4f52 4d20 6966 2073 7479 6c65  le.FORM if style
-00004f50: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
-00004f60: 796c 650a 2020 2020 2020 2020 7573 6564  yle.        used
-00004f70: 5f65 7870 6c6f 6465 203d 2073 656c 662e  _explode = self.
-00004f80: 5f67 6574 5f64 6566 6175 6c74 5f65 7870  _get_default_exp
-00004f90: 6c6f 6465 2875 7365 645f 7374 796c 6529  lode(used_style)
-00004fa0: 2069 6620 6578 706c 6f64 6520 6973 204e   if explode is N
-00004fb0: 6f6e 6520 656c 7365 2065 7870 6c6f 6465  one else explode
-00004fc0: 0a0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00004fd0: 292e 5f5f 696e 6974 5f5f 280a 2020 2020  ).__init__(.    
-00004fe0: 2020 2020 2020 2020 6e61 6d65 2c0a 2020          name,.  
-00004ff0: 2020 2020 2020 2020 2020 696e 5f74 7970            in_typ
-00005000: 653d 5061 7261 6d65 7465 7249 6e54 7970  e=ParameterInTyp
-00005010: 652e 5155 4552 592c 0a20 2020 2020 2020  e.QUERY,.       
-00005020: 2020 2020 2072 6571 7569 7265 643d 7265       required=re
-00005030: 7175 6972 6564 2c0a 2020 2020 2020 2020  quired,.        
-00005040: 2020 2020 7374 796c 653d 7573 6564 5f73      style=used_s
-00005050: 7479 6c65 2c0a 2020 2020 2020 2020 2020  tyle,.          
-00005060: 2020 6578 706c 6f64 653d 7573 6564 5f65    explode=used_e
-00005070: 7870 6c6f 6465 2c0a 2020 2020 2020 2020  xplode,.        
-00005080: 2020 2020 616c 6c6f 775f 7265 7365 7276      allow_reserv
-00005090: 6564 3d61 6c6c 6f77 5f72 6573 6572 7665  ed=allow_reserve
-000050a0: 642c 0a20 2020 2020 2020 2020 2020 2073  d,.            s
-000050b0: 6368 656d 613d 7363 6865 6d61 2c0a 2020  chema=schema,.  
-000050c0: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-000050d0: 743d 636f 6e74 656e 740a 2020 2020 2020  t=content.      
-000050e0: 2020 290a 0a20 2020 2064 6566 205f 5f73    )..    def __s
-000050f0: 6572 6961 6c69 7a65 5f73 7061 6365 5f64  erialize_space_d
-00005100: 656c 696d 6974 6564 280a 2020 2020 2020  elimited(.      
-00005110: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00005120: 696e 5f64 6174 613a 2074 7970 696e 672e  in_data: typing.
-00005130: 556e 696f 6e5b 4e6f 6e65 2c20 696e 742c  Union[None, int,
-00005140: 2066 6c6f 6174 2c20 7374 722c 2062 6f6f   float, str, boo
-00005150: 6c2c 2064 6963 742c 206c 6973 745d 2c0a  l, dict, list],.
-00005160: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
-00005170: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
-00005180: 723a 2074 7970 696e 672e 4f70 7469 6f6e  r: typing.Option
-00005190: 616c 5b50 7265 6669 7853 6570 6172 6174  al[PrefixSeparat
-000051a0: 6f72 4974 6572 6174 6f72 5d0a 2020 2020  orIterator].    
-000051b0: 2920 2d3e 2074 7970 696e 672e 4469 6374  ) -> typing.Dict
-000051c0: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
-000051d0: 2020 2020 6966 2070 7265 6669 785f 7365      if prefix_se
-000051e0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-000051f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005200: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-00005210: 6172 6174 6f72 5f69 7465 7261 746f 7220  arator_iterator 
-00005220: 3d20 7365 6c66 2e67 6574 5f70 7265 6669  = self.get_prefi
-00005230: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00005240: 6174 6f72 2829 0a20 2020 2020 2020 2076  ator().        v
-00005250: 616c 7565 203d 2073 656c 662e 5f72 6566  alue = self._ref
-00005260: 3635 3730 5f65 7870 616e 7369 6f6e 280a  6570_expansion(.
-00005270: 2020 2020 2020 2020 2020 2020 7661 7269              vari
-00005280: 6162 6c65 5f6e 616d 653d 7365 6c66 2e6e  able_name=self.n
-00005290: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-000052a0: 2069 6e5f 6461 7461 3d69 6e5f 6461 7461   in_data=in_data
-000052b0: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
-000052c0: 706c 6f64 653d 7365 6c66 2e65 7870 6c6f  plode=self.explo
-000052d0: 6465 2c0a 2020 2020 2020 2020 2020 2020  de,.            
-000052e0: 7065 7263 656e 745f 656e 636f 6465 3d54  percent_encode=T
-000052f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00005300: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00005310: 725f 6974 6572 6174 6f72 3d70 7265 6669  r_iterator=prefi
-00005320: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-00005330: 6174 6f72 0a20 2020 2020 2020 2029 0a20  ator.        ). 
-00005340: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00005350: 6c66 2e5f 746f 5f64 6963 7428 7365 6c66  lf._to_dict(self
-00005360: 2e6e 616d 652c 2076 616c 7565 290a 0a20  .name, value).. 
-00005370: 2020 2064 6566 205f 5f73 6572 6961 6c69     def __seriali
-00005380: 7a65 5f70 6970 655f 6465 6c69 6d69 7465  ze_pipe_delimite
-00005390: 6428 0a20 2020 2020 2020 2073 656c 662c  d(.        self,
-000053a0: 0a20 2020 2020 2020 2069 6e5f 6461 7461  .        in_data
-000053b0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b4e  : typing.Union[N
-000053c0: 6f6e 652c 2069 6e74 2c20 666c 6f61 742c  one, int, float,
-000053d0: 2073 7472 2c20 626f 6f6c 2c20 6469 6374   str, bool, dict
-000053e0: 2c20 6c69 7374 5d2c 0a20 2020 2020 2020  , list],.       
-000053f0: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-00005400: 725f 6974 6572 6174 6f72 3a20 7479 7069  r_iterator: typi
-00005410: 6e67 2e4f 7074 696f 6e61 6c5b 5072 6566  ng.Optional[Pref
-00005420: 6978 5365 7061 7261 746f 7249 7465 7261  ixSeparatorItera
-00005430: 746f 725d 0a20 2020 2029 202d 3e20 7479  tor].    ) -> ty
-00005440: 7069 6e67 2e44 6963 745b 7374 722c 2073  ping.Dict[str, s
-00005450: 7472 5d3a 0a20 2020 2020 2020 2069 6620  tr]:.        if 
-00005460: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-00005470: 5f69 7465 7261 746f 7220 6973 204e 6f6e  _iterator is Non
-00005480: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00005490: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-000054a0: 6974 6572 6174 6f72 203d 2073 656c 662e  iterator = self.
-000054b0: 6765 745f 7072 6566 6978 5f73 6570 6172  get_prefix_separ
-000054c0: 6174 6f72 5f69 7465 7261 746f 7228 290a  ator_iterator().
-000054d0: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
-000054e0: 7365 6c66 2e5f 7265 6636 3537 305f 6578  self._ref6570_ex
-000054f0: 7061 6e73 696f 6e28 0a20 2020 2020 2020  pansion(.       
-00005500: 2020 2020 2076 6172 6961 626c 655f 6e61       variable_na
-00005510: 6d65 3d73 656c 662e 6e61 6d65 2c0a 2020  me=self.name,.  
-00005520: 2020 2020 2020 2020 2020 696e 5f64 6174            in_dat
-00005530: 613d 696e 5f64 6174 612c 0a20 2020 2020  a=in_data,.     
-00005540: 2020 2020 2020 2065 7870 6c6f 6465 3d73         explode=s
-00005550: 656c 662e 6578 706c 6f64 652c 0a20 2020  elf.explode,.   
-00005560: 2020 2020 2020 2020 2070 6572 6365 6e74           percent
-00005570: 5f65 6e63 6f64 653d 5472 7565 2c0a 2020  _encode=True,.  
-00005580: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
-00005590: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-000055a0: 746f 723d 7072 6566 6978 5f73 6570 6172  tor=prefix_separ
-000055b0: 6174 6f72 5f69 7465 7261 746f 720a 2020  ator_iterator.  
-000055c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000055d0: 7265 7475 726e 2073 656c 662e 5f74 6f5f  return self._to_
-000055e0: 6469 6374 2873 656c 662e 6e61 6d65 2c20  dict(self.name, 
-000055f0: 7661 6c75 6529 0a0a 2020 2020 6465 6620  value)..    def 
-00005600: 5f5f 7365 7269 616c 697a 655f 666f 726d  __serialize_form
-00005610: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00005620: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
-00005630: 2074 7970 696e 672e 556e 696f 6e5b 4e6f   typing.Union[No
-00005640: 6e65 2c20 696e 742c 2066 6c6f 6174 2c20  ne, int, float, 
-00005650: 7374 722c 2062 6f6f 6c2c 2064 6963 742c  str, bool, dict,
-00005660: 206c 6973 745d 2c0a 2020 2020 2020 2020   list],.        
-00005670: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-00005680: 5f69 7465 7261 746f 723a 2074 7970 696e  _iterator: typin
-00005690: 672e 4f70 7469 6f6e 616c 5b50 7265 6669  g.Optional[Prefi
-000056a0: 7853 6570 6172 6174 6f72 4974 6572 6174  xSeparatorIterat
-000056b0: 6f72 5d0a 2020 2020 2920 2d3e 2074 7970  or].    ) -> typ
-000056c0: 696e 672e 4469 6374 5b73 7472 2c20 7374  ing.Dict[str, st
-000056d0: 725d 3a0a 2020 2020 2020 2020 6966 2070  r]:.        if p
-000056e0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-000056f0: 6974 6572 6174 6f72 2069 7320 4e6f 6e65  iterator is None
-00005700: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00005710: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
-00005720: 7465 7261 746f 7220 3d20 7365 6c66 2e67  terator = self.g
-00005730: 6574 5f70 7265 6669 785f 7365 7061 7261  et_prefix_separa
-00005740: 746f 725f 6974 6572 6174 6f72 2829 0a20  tor_iterator(). 
-00005750: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
-00005760: 656c 662e 5f73 6572 6961 6c69 7a65 5f66  elf._serialize_f
-00005770: 6f72 6d28 0a20 2020 2020 2020 2020 2020  orm(.           
-00005780: 2069 6e5f 6461 7461 2c0a 2020 2020 2020   in_data,.      
-00005790: 2020 2020 2020 6e61 6d65 3d73 656c 662e        name=self.
-000057a0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-000057b0: 2020 6578 706c 6f64 653d 7365 6c66 2e65    explode=self.e
-000057c0: 7870 6c6f 6465 2c0a 2020 2020 2020 2020  xplode,.        
-000057d0: 2020 2020 7065 7263 656e 745f 656e 636f      percent_enco
-000057e0: 6465 3d54 7275 652c 0a20 2020 2020 2020  de=True,.       
-000057f0: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
-00005800: 7261 746f 725f 6974 6572 6174 6f72 3d70  rator_iterator=p
-00005810: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00005820: 6974 6572 6174 6f72 0a20 2020 2020 2020  iterator.       
-00005830: 2029 0a20 2020 2020 2020 2072 6574 7572   ).        retur
-00005840: 6e20 7365 6c66 2e5f 746f 5f64 6963 7428  n self._to_dict(
-00005850: 7365 6c66 2e6e 616d 652c 2076 616c 7565  self.name, value
-00005860: 290a 0a20 2020 2064 6566 2067 6574 5f70  )..    def get_p
-00005870: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
-00005880: 6974 6572 6174 6f72 2873 656c 6629 202d  iterator(self) -
-00005890: 3e20 7479 7069 6e67 2e4f 7074 696f 6e61  > typing.Optiona
-000058a0: 6c5b 5072 6566 6978 5365 7061 7261 746f  l[PrefixSeparato
-000058b0: 7249 7465 7261 746f 725d 3a0a 2020 2020  rIterator]:.    
-000058c0: 2020 2020 6966 2073 656c 662e 7374 796c      if self.styl
-000058d0: 6520 6973 2050 6172 616d 6574 6572 5374  e is ParameterSt
-000058e0: 796c 652e 464f 524d 3a0a 2020 2020 2020  yle.FORM:.      
-000058f0: 2020 2020 2020 7265 7475 726e 2050 7265        return Pre
-00005900: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
-00005910: 6174 6f72 2827 3f27 2c20 2726 2729 0a20  ator('?', '&'). 
-00005920: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00005930: 2e73 7479 6c65 2069 7320 5061 7261 6d65  .style is Parame
-00005940: 7465 7253 7479 6c65 2e53 5041 4345 5f44  terStyle.SPACE_D
-00005950: 454c 494d 4954 4544 3a0a 2020 2020 2020  ELIMITED:.      
-00005960: 2020 2020 2020 7265 7475 726e 2050 7265        return Pre
-00005970: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
-00005980: 6174 6f72 2827 272c 2027 2532 3027 290a  ator('', '%20').
-00005990: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-000059a0: 662e 7374 796c 6520 6973 2050 6172 616d  f.style is Param
-000059b0: 6574 6572 5374 796c 652e 5049 5045 5f44  eterStyle.PIPE_D
-000059c0: 454c 494d 4954 4544 3a0a 2020 2020 2020  ELIMITED:.      
-000059d0: 2020 2020 2020 7265 7475 726e 2050 7265        return Pre
-000059e0: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
-000059f0: 6174 6f72 2827 272c 2027 7c27 290a 0a20  ator('', '|').. 
-00005a00: 2020 2064 6566 2073 6572 6961 6c69 7a65     def serialize
-00005a10: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00005a20: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
-00005a30: 2074 7970 696e 672e 556e 696f 6e5b 0a20   typing.Union[. 
-00005a40: 2020 2020 2020 2020 2020 2053 6368 656d             Schem
-00005a50: 612c 2044 6563 696d 616c 2c20 696e 742c  a, Decimal, int,
-00005a60: 2066 6c6f 6174 2c20 7374 722c 2064 6174   float, str, dat
-00005a70: 652c 2064 6174 6574 696d 652c 204e 6f6e  e, datetime, Non
-00005a80: 652c 2062 6f6f 6c2c 206c 6973 742c 2074  e, bool, list, t
-00005a90: 7570 6c65 2c20 6469 6374 2c20 6672 6f7a  uple, dict, froz
-00005aa0: 656e 6469 6374 2e66 726f 7a65 6e64 6963  endict.frozendic
-00005ab0: 745d 2c0a 2020 2020 2020 2020 7072 6566  t],.        pref
-00005ac0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
-00005ad0: 7261 746f 723a 2074 7970 696e 672e 4f70  rator: typing.Op
-00005ae0: 7469 6f6e 616c 5b50 7265 6669 7853 6570  tional[PrefixSep
-00005af0: 6172 6174 6f72 4974 6572 6174 6f72 5d20  aratorIterator] 
-00005b00: 3d20 4e6f 6e65 0a20 2020 2029 202d 3e20  = None.    ) -> 
-00005b10: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-00005b20: 2073 7472 5d3a 0a20 2020 2020 2020 2069   str]:.        i
-00005b30: 6620 7365 6c66 2e73 6368 656d 613a 0a20  f self.schema:. 
-00005b40: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
-00005b50: 696e 5f64 6174 6120 3d20 7365 6c66 2e73  in_data = self.s
-00005b60: 6368 656d 6128 696e 5f64 6174 6129 0a20  chema(in_data). 
-00005b70: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
-00005b80: 696e 5f64 6174 6120 3d20 7365 6c66 2e5f  in_data = self._
-00005b90: 6a73 6f6e 5f65 6e63 6f64 6572 2e64 6566  json_encoder.def
-00005ba0: 6175 6c74 2863 6173 745f 696e 5f64 6174  ault(cast_in_dat
-00005bb0: 6129 0a20 2020 2020 2020 2020 2020 2022  a).            "
-00005bc0: 2222 0a20 2020 2020 2020 2020 2020 2066  "".            f
-00005bd0: 6f72 6d20 2d3e 2071 7565 7279 0a20 2020  orm -> query.   
-00005be0: 2020 2020 2020 2020 2020 2020 2071 7565               que
-00005bf0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00005c00: 2020 2020 2020 2020 2d20 4745 542f 4845          - GET/HE
-00005c10: 4144 2f44 454c 4554 453a 2063 6f75 6c64  AD/DELETE: could
-00005c20: 2075 7365 2066 6965 6c64 730a 2020 2020   use fields.    
-00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2d20 5055 542f 504f 5354 3a20 6d75 7374  - PUT/POST: must
-00005c50: 2075 7365 2075 726c 656e 636f 6465 2074   use urlencode t
-00005c60: 6f20 7365 6e64 2070 6172 616d 6574 6572  o send parameter
-00005c70: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00005c80: 2020 2020 2020 7265 7475 726e 7320 6669        returns fi
-00005c90: 656c 6473 3a20 7475 706c 650a 2020 2020  elds: tuple.    
-00005ca0: 2020 2020 2020 2020 7370 6163 6544 656c          spaceDel
-00005cb0: 696d 6974 6564 202d 3e20 7175 6572 790a  imited -> query.
-00005cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cd0: 7265 7475 726e 7320 6669 656c 6473 0a20  returns fields. 
-00005ce0: 2020 2020 2020 2020 2020 2070 6970 6544             pipeD
-00005cf0: 656c 696d 6974 6564 202d 3e20 7175 6572  elimited -> quer
-00005d00: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00005d10: 2020 7265 7475 726e 7320 6669 656c 6473    returns fields
-00005d20: 0a20 2020 2020 2020 2020 2020 2064 6565  .            dee
-00005d30: 704f 626a 6563 7420 2d3e 2071 7565 7279  pObject -> query
-00005d40: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00005d50: 2e63 6f6d 2f4f 4149 2f4f 7065 6e41 5049  .com/OAI/OpenAPI
-00005d60: 2d53 7065 6369 6669 6361 7469 6f6e 2f69  -Specification/i
-00005d70: 7373 7565 732f 3137 3036 0a20 2020 2020  ssues/1706.     
-00005d80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005d90: 6e73 2066 6965 6c64 730a 2020 2020 2020  ns fields.      
-00005da0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005db0: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00005dc0: 796c 653a 0a20 2020 2020 2020 2020 2020  yle:.           
-00005dd0: 2020 2020 2023 2054 4f44 4f20 7570 6461       # TODO upda
-00005de0: 7465 2071 7565 7279 206f 6e65 7320 746f  te query ones to
-00005df0: 206f 6d69 7420 7365 7474 696e 6720 7661   omit setting va
-00005e00: 6c75 6573 2077 6865 6e20 5b5d 207b 7d20  lues when [] {} 
-00005e10: 6f72 204e 6f6e 6520 6973 2069 6e70 7574  or None is input
-00005e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005e30: 2069 6620 7365 6c66 2e73 7479 6c65 2069   if self.style i
-00005e40: 7320 5061 7261 6d65 7465 7253 7479 6c65  s ParameterStyle
-00005e50: 2e46 4f52 4d3a 0a20 2020 2020 2020 2020  .FORM:.         
-00005e60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005e70: 6e20 7365 6c66 2e5f 5f73 6572 6961 6c69  n self.__seriali
-00005e80: 7a65 5f66 6f72 6d28 6361 7374 5f69 6e5f  ze_form(cast_in_
-00005e90: 6461 7461 2c20 7072 6566 6978 5f73 6570  data, prefix_sep
-00005ea0: 6172 6174 6f72 5f69 7465 7261 746f 7229  arator_iterator)
-00005eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005ec0: 2065 6c69 6620 7365 6c66 2e73 7479 6c65   elif self.style
-00005ed0: 2069 7320 5061 7261 6d65 7465 7253 7479   is ParameterSty
-00005ee0: 6c65 2e53 5041 4345 5f44 454c 494d 4954  le.SPACE_DELIMIT
-00005ef0: 4544 3a0a 2020 2020 2020 2020 2020 2020  ED:.            
-00005f00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005f10: 656c 662e 5f5f 7365 7269 616c 697a 655f  elf.__serialize_
-00005f20: 7370 6163 655f 6465 6c69 6d69 7465 6428  space_delimited(
-00005f30: 6361 7374 5f69 6e5f 6461 7461 2c20 7072  cast_in_data, pr
-00005f40: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
-00005f50: 7465 7261 746f 7229 0a20 2020 2020 2020  terator).       
-00005f60: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
-00005f70: 6c66 2e73 7479 6c65 2069 7320 5061 7261  lf.style is Para
-00005f80: 6d65 7465 7253 7479 6c65 2e50 4950 455f  meterStyle.PIPE_
-00005f90: 4445 4c49 4d49 5445 443a 0a20 2020 2020  DELIMITED:.     
-00005fa0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00005fb0: 6574 7572 6e20 7365 6c66 2e5f 5f73 6572  eturn self.__ser
-00005fc0: 6961 6c69 7a65 5f70 6970 655f 6465 6c69  ialize_pipe_deli
-00005fd0: 6d69 7465 6428 6361 7374 5f69 6e5f 6461  mited(cast_in_da
-00005fe0: 7461 2c20 7072 6566 6978 5f73 6570 6172  ta, prefix_separ
-00005ff0: 6174 6f72 5f69 7465 7261 746f 7229 0a20  ator_iterator). 
-00006000: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-00006010: 6e74 656e 7420 7769 6c6c 2062 6520 6c65  ntent will be le
-00006020: 6e67 7468 206f 6e65 0a20 2020 2020 2020  ngth one.       
-00006030: 2069 6620 7072 6566 6978 5f73 6570 6172   if prefix_separ
-00006040: 6174 6f72 5f69 7465 7261 746f 7220 6973  ator_iterator is
-00006050: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00006060: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
-00006070: 746f 725f 6974 6572 6174 6f72 203d 2073  tor_iterator = s
-00006080: 656c 662e 6765 745f 7072 6566 6978 5f73  elf.get_prefix_s
-00006090: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
-000060a0: 7228 290a 2020 2020 2020 2020 666f 7220  r().        for 
-000060b0: 636f 6e74 656e 745f 7479 7065 2c20 7363  content_type, sc
-000060c0: 6865 6d61 2069 6e20 7365 6c66 2e63 6f6e  hema in self.con
-000060d0: 7465 6e74 2e69 7465 6d73 2829 3a0a 2020  tent.items():.  
-000060e0: 2020 2020 2020 2020 2020 6361 7374 5f69            cast_i
-000060f0: 6e5f 6461 7461 203d 2073 6368 656d 6128  n_data = schema(
-00006100: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
-00006110: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
-00006120: 6120 3d20 7365 6c66 2e5f 6a73 6f6e 5f65  a = self._json_e
-00006130: 6e63 6f64 6572 2e64 6566 6175 6c74 2863  ncoder.default(c
-00006140: 6173 745f 696e 5f64 6174 6129 0a20 2020  ast_in_data).   
-00006150: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00006160: 2e5f 636f 6e74 656e 745f 7479 7065 5f69  ._content_type_i
-00006170: 735f 6a73 6f6e 2863 6f6e 7465 6e74 5f74  s_json(content_t
-00006180: 7970 6529 3a0a 2020 2020 2020 2020 2020  ype):.          
-00006190: 2020 2020 2020 7661 6c75 6520 3d20 7365        value = se
-000061a0: 6c66 2e5f 7365 7269 616c 697a 655f 6a73  lf._serialize_js
-000061b0: 6f6e 2863 6173 745f 696e 5f64 6174 612c  on(cast_in_data,
-000061c0: 2065 6c69 6d69 6e61 7465 5f77 6869 7465   eliminate_white
-000061d0: 7370 6163 653d 5472 7565 290a 2020 2020  space=True).    
-000061e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000061f0: 726e 2073 656c 662e 5f74 6f5f 6469 6374  rn self._to_dict
-00006200: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006210: 2020 2020 2020 7365 6c66 2e6e 616d 652c        self.name,
-00006220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006230: 2020 2020 206e 6578 7428 7072 6566 6978       next(prefix
-00006240: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
-00006250: 746f 7229 202b 2073 656c 662e 6e61 6d65  tor) + self.name
-00006260: 202b 2027 3d27 202b 2071 756f 7465 2876   + '=' + quote(v
-00006270: 616c 7565 290a 2020 2020 2020 2020 2020  alue).          
-00006280: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006290: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
-000062a0: 6c65 6d65 6e74 6564 4572 726f 7228 2753  lementedError('S
-000062b0: 6572 6961 6c69 7a61 7469 6f6e 206f 6620  erialization of 
-000062c0: 7b7d 2068 6173 206e 6f74 2079 6574 2062  {} has not yet b
-000062d0: 6565 6e20 696d 706c 656d 656e 7465 6427  een implemented'
-000062e0: 2e66 6f72 6d61 7428 636f 6e74 656e 745f  .format(content_
-000062f0: 7479 7065 2929 0a0a 0a63 6c61 7373 2043  type))...class C
-00006300: 6f6f 6b69 6550 6172 616d 6574 6572 2850  ookieParameter(P
-00006310: 6172 616d 6574 6572 4261 7365 2c20 5374  arameterBase, St
-00006320: 796c 6546 6f72 6d53 6572 6961 6c69 7a65  yleFormSerialize
-00006330: 7229 3a0a 0a20 2020 2064 6566 205f 5f69  r):..    def __i
-00006340: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
-00006350: 656c 662c 0a20 2020 2020 2020 206e 616d  elf,.        nam
-00006360: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-00006370: 7265 7175 6972 6564 3a20 626f 6f6c 203d  required: bool =
-00006380: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00006390: 7374 796c 653a 2074 7970 696e 672e 4f70  style: typing.Op
-000063a0: 7469 6f6e 616c 5b50 6172 616d 6574 6572  tional[Parameter
-000063b0: 5374 796c 655d 203d 204e 6f6e 652c 0a20  Style] = None,. 
-000063c0: 2020 2020 2020 2065 7870 6c6f 6465 3a20         explode: 
-000063d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000063e0: 626f 6f6c 5d20 3d20 4e6f 6e65 2c0a 2020  bool] = None,.  
-000063f0: 2020 2020 2020 616c 6c6f 775f 7265 7365        allow_rese
-00006400: 7276 6564 3a20 7479 7069 6e67 2e4f 7074  rved: typing.Opt
-00006410: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 4e6f  ional[bool] = No
-00006420: 6e65 2c0a 2020 2020 2020 2020 7363 6865  ne,.        sche
-00006430: 6d61 3a20 7479 7069 6e67 2e4f 7074 696f  ma: typing.Optio
-00006440: 6e61 6c5b 7479 7069 6e67 2e54 7970 655b  nal[typing.Type[
-00006450: 5363 6865 6d61 5d5d 203d 204e 6f6e 652c  Schema]] = None,
-00006460: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
-00006470: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00006480: 6c5b 7479 7069 6e67 2e44 6963 745b 7374  l[typing.Dict[st
-00006490: 722c 2074 7970 696e 672e 5479 7065 5b53  r, typing.Type[S
-000064a0: 6368 656d 615d 5d5d 203d 204e 6f6e 650a  chema]]] = None.
-000064b0: 2020 2020 293a 0a20 2020 2020 2020 2075      ):.        u
-000064c0: 7365 645f 7374 796c 6520 3d20 5061 7261  sed_style = Para
-000064d0: 6d65 7465 7253 7479 6c65 2e46 4f52 4d20  meterStyle.FORM 
-000064e0: 6966 2073 7479 6c65 2069 7320 4e6f 6e65  if style is None
-000064f0: 2061 6e64 2063 6f6e 7465 6e74 2069 7320   and content is 
-00006500: 4e6f 6e65 2061 6e64 2073 6368 656d 6120  None and schema 
-00006510: 656c 7365 2073 7479 6c65 0a20 2020 2020  else style.     
-00006520: 2020 2075 7365 645f 6578 706c 6f64 6520     used_explode 
-00006530: 3d20 7365 6c66 2e5f 6765 745f 6465 6661  = self._get_defa
-00006540: 756c 745f 6578 706c 6f64 6528 7573 6564  ult_explode(used
-00006550: 5f73 7479 6c65 2920 6966 2065 7870 6c6f  _style) if explo
-00006560: 6465 2069 7320 4e6f 6e65 2065 6c73 6520  de is None else 
-00006570: 6578 706c 6f64 650a 0a20 2020 2020 2020  explode..       
-00006580: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
-00006590: 5f28 0a20 2020 2020 2020 2020 2020 206e  _(.            n
-000065a0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-000065b0: 2069 6e5f 7479 7065 3d50 6172 616d 6574   in_type=Paramet
-000065c0: 6572 496e 5479 7065 2e43 4f4f 4b49 452c  erInType.COOKIE,
-000065d0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-000065e0: 7569 7265 643d 7265 7175 6972 6564 2c0a  uired=required,.
-000065f0: 2020 2020 2020 2020 2020 2020 7374 796c              styl
-00006600: 653d 7573 6564 5f73 7479 6c65 2c0a 2020  e=used_style,.  
-00006610: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
-00006620: 653d 7573 6564 5f65 7870 6c6f 6465 2c0a  e=used_explode,.
-00006630: 2020 2020 2020 2020 2020 2020 616c 6c6f              allo
-00006640: 775f 7265 7365 7276 6564 3d61 6c6c 6f77  w_reserved=allow
-00006650: 5f72 6573 6572 7665 642c 0a20 2020 2020  _reserved,.     
-00006660: 2020 2020 2020 2073 6368 656d 613d 7363         schema=sc
-00006670: 6865 6d61 2c0a 2020 2020 2020 2020 2020  hema,.          
-00006680: 2020 636f 6e74 656e 743d 636f 6e74 656e    content=conten
-00006690: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
-000066a0: 2064 6566 2073 6572 6961 6c69 7a65 280a   def serialize(.
-000066b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-000066c0: 2020 2020 2020 696e 5f64 6174 613a 2074        in_data: t
-000066d0: 7970 696e 672e 556e 696f 6e5b 0a20 2020  yping.Union[.   
-000066e0: 2020 2020 2020 2020 2053 6368 656d 612c           Schema,
-000066f0: 2044 6563 696d 616c 2c20 696e 742c 2066   Decimal, int, f
-00006700: 6c6f 6174 2c20 7374 722c 2064 6174 652c  loat, str, date,
-00006710: 2064 6174 6574 696d 652c 204e 6f6e 652c   datetime, None,
-00006720: 2062 6f6f 6c2c 206c 6973 742c 2074 7570   bool, list, tup
-00006730: 6c65 2c20 6469 6374 2c20 6672 6f7a 656e  le, dict, frozen
-00006740: 6469 6374 2e66 726f 7a65 6e64 6963 745d  dict.frozendict]
-00006750: 0a20 2020 2029 202d 3e20 7479 7069 6e67  .    ) -> typing
-00006760: 2e44 6963 745b 7374 722c 2073 7472 5d3a  .Dict[str, str]:
-00006770: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00006780: 2e73 6368 656d 613a 0a20 2020 2020 2020  .schema:.       
-00006790: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
-000067a0: 6120 3d20 7365 6c66 2e73 6368 656d 6128  a = self.schema(
-000067b0: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
-000067c0: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
-000067d0: 6120 3d20 7365 6c66 2e5f 6a73 6f6e 5f65  a = self._json_e
-000067e0: 6e63 6f64 6572 2e64 6566 6175 6c74 2863  ncoder.default(c
-000067f0: 6173 745f 696e 5f64 6174 6129 0a20 2020  ast_in_data).   
-00006800: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
-00006810: 2020 2020 2020 2020 2066 6f72 6d20 2d3e           form ->
-00006820: 2063 6f6f 6b69 650a 2020 2020 2020 2020   cookie.        
-00006830: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
-00006840: 6669 656c 6473 3a20 7475 706c 650a 2020  fields: tuple.  
-00006850: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-00006860: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00006870: 662e 7374 796c 653a 0a20 2020 2020 2020  f.style:.       
-00006880: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
-00006890: 2020 2020 2020 2020 2020 2020 2054 4f44               TOD
-000068a0: 4f20 6164 6420 6573 6361 7069 6e67 206f  O add escaping o
-000068b0: 6620 636f 6d6d 612c 2073 7061 6365 2c20  f comma, space, 
-000068c0: 6571 7561 6c73 0a20 2020 2020 2020 2020  equals.         
-000068d0: 2020 2020 2020 206f 7220 7475 726e 2065         or turn e
-000068e0: 6e63 6f64 696e 6720 6f6e 0a20 2020 2020  ncoding on.     
-000068f0: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-00006900: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-00006910: 616c 7565 203d 2073 656c 662e 5f73 6572  alue = self._ser
-00006920: 6961 6c69 7a65 5f66 6f72 6d28 0a20 2020  ialize_form(.   
-00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2063 6173 745f 696e 5f64 6174 612c 0a20   cast_in_data,. 
-00006950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006960: 2020 2065 7870 6c6f 6465 3d73 656c 662e     explode=self.
-00006970: 6578 706c 6f64 652c 0a20 2020 2020 2020  explode,.       
-00006980: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00006990: 653d 7365 6c66 2e6e 616d 652c 0a20 2020  e=self.name,.   
-000069a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069b0: 2070 6572 6365 6e74 5f65 6e63 6f64 653d   percent_encode=
-000069c0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-000069d0: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
-000069e0: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
-000069f0: 6174 6f72 3d50 7265 6669 7853 6570 6172  ator=PrefixSepar
-00006a00: 6174 6f72 4974 6572 6174 6f72 2827 272c  atorIterator('',
-00006a10: 2027 2627 290a 2020 2020 2020 2020 2020   '&').          
-00006a20: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006a30: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00006a40: 656c 662e 5f74 6f5f 6469 6374 2873 656c  elf._to_dict(sel
-00006a50: 662e 6e61 6d65 2c20 7661 6c75 6529 0a20  f.name, value). 
-00006a60: 2020 2020 2020 2023 2073 656c 662e 636f         # self.co
-00006a70: 6e74 656e 7420 7769 6c6c 2062 6520 6c65  ntent will be le
-00006a80: 6e67 7468 206f 6e65 0a20 2020 2020 2020  ngth one.       
-00006a90: 2066 6f72 2063 6f6e 7465 6e74 5f74 7970   for content_typ
-00006aa0: 652c 2073 6368 656d 6120 696e 2073 656c  e, schema in sel
-00006ab0: 662e 636f 6e74 656e 742e 6974 656d 7328  f.content.items(
-00006ac0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00006ad0: 6173 745f 696e 5f64 6174 6120 3d20 7363  ast_in_data = sc
-00006ae0: 6865 6d61 2869 6e5f 6461 7461 290a 2020  hema(in_data).  
-00006af0: 2020 2020 2020 2020 2020 6361 7374 5f69            cast_i
-00006b00: 6e5f 6461 7461 203d 2073 656c 662e 5f6a  n_data = self._j
-00006b10: 736f 6e5f 656e 636f 6465 722e 6465 6661  son_encoder.defa
-00006b20: 756c 7428 6361 7374 5f69 6e5f 6461 7461  ult(cast_in_data
-00006b30: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00006b40: 2073 656c 662e 5f63 6f6e 7465 6e74 5f74   self._content_t
-00006b50: 7970 655f 6973 5f6a 736f 6e28 636f 6e74  ype_is_json(cont
-00006b60: 656e 745f 7479 7065 293a 0a20 2020 2020  ent_type):.     
-00006b70: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00006b80: 203d 2073 656c 662e 5f73 6572 6961 6c69   = self._seriali
-00006b90: 7a65 5f6a 736f 6e28 6361 7374 5f69 6e5f  ze_json(cast_in_
-00006ba0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
-00006bb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00006bc0: 662e 5f74 6f5f 6469 6374 2873 656c 662e  f._to_dict(self.
-00006bd0: 6e61 6d65 2c20 7661 6c75 6529 0a20 2020  name, value).   
-00006be0: 2020 2020 2020 2020 2072 6169 7365 204e           raise N
-00006bf0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00006c00: 6f72 2827 5365 7269 616c 697a 6174 696f  or('Serializatio
-00006c10: 6e20 6f66 207b 7d20 6861 7320 6e6f 7420  n of {} has not 
-00006c20: 7965 7420 6265 656e 2069 6d70 6c65 6d65  yet been impleme
-00006c30: 6e74 6564 272e 666f 726d 6174 2863 6f6e  nted'.format(con
-00006c40: 7465 6e74 5f74 7970 6529 290a 0a0a 636c  tent_type))...cl
-00006c50: 6173 7320 4865 6164 6572 5061 7261 6d65  ass HeaderParame
-00006c60: 7465 7228 5061 7261 6d65 7465 7242 6173  ter(ParameterBas
-00006c70: 652c 2053 7479 6c65 5369 6d70 6c65 5365  e, StyleSimpleSe
-00006c80: 7269 616c 697a 6572 293a 0a20 2020 2064  rializer):.    d
-00006c90: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00006ca0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00006cb0: 2020 206e 616d 653a 2073 7472 2c0a 2020     name: str,.  
-00006cc0: 2020 2020 2020 7265 7175 6972 6564 3a20        required: 
-00006cd0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
-00006ce0: 2020 2020 2020 7374 796c 653a 2074 7970        style: typ
-00006cf0: 696e 672e 4f70 7469 6f6e 616c 5b50 6172  ing.Optional[Par
-00006d00: 616d 6574 6572 5374 796c 655d 203d 204e  ameterStyle] = N
-00006d10: 6f6e 652c 0a20 2020 2020 2020 2065 7870  one,.        exp
-00006d20: 6c6f 6465 3a20 626f 6f6c 203d 2046 616c  lode: bool = Fal
-00006d30: 7365 2c0a 2020 2020 2020 2020 616c 6c6f  se,.        allo
-00006d40: 775f 7265 7365 7276 6564 3a20 7479 7069  w_reserved: typi
-00006d50: 6e67 2e4f 7074 696f 6e61 6c5b 626f 6f6c  ng.Optional[bool
-00006d60: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00006d70: 2020 7363 6865 6d61 3a20 7479 7069 6e67    schema: typing
-00006d80: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00006d90: 2e54 7970 655b 5363 6865 6d61 5d5d 203d  .Type[Schema]] =
-00006da0: 204e 6f6e 652c 0a20 2020 2020 2020 2063   None,.        c
-00006db0: 6f6e 7465 6e74 3a20 7479 7069 6e67 2e4f  ontent: typing.O
-00006dc0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e44  ptional[typing.D
-00006dd0: 6963 745b 7374 722c 2074 7970 696e 672e  ict[str, typing.
-00006de0: 5479 7065 5b53 6368 656d 615d 5d5d 203d  Type[Schema]]] =
-00006df0: 204e 6f6e 650a 2020 2020 293a 0a20 2020   None.    ):.   
-00006e00: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00006e10: 6e69 745f 5f28 0a20 2020 2020 2020 2020  nit__(.         
-00006e20: 2020 206e 616d 652c 0a20 2020 2020 2020     name,.       
-00006e30: 2020 2020 2069 6e5f 7479 7065 3d50 6172       in_type=Par
-00006e40: 616d 6574 6572 496e 5479 7065 2e48 4541  ameterInType.HEA
-00006e50: 4445 522c 0a20 2020 2020 2020 2020 2020  DER,.           
-00006e60: 2072 6571 7569 7265 643d 7265 7175 6972   required=requir
-00006e70: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
-00006e80: 7374 796c 653d 7374 796c 652c 0a20 2020  style=style,.   
-00006e90: 2020 2020 2020 2020 2065 7870 6c6f 6465           explode
-00006ea0: 3d65 7870 6c6f 6465 2c0a 2020 2020 2020  =explode,.      
-00006eb0: 2020 2020 2020 616c 6c6f 775f 7265 7365        allow_rese
-00006ec0: 7276 6564 3d61 6c6c 6f77 5f72 6573 6572  rved=allow_reser
-00006ed0: 7665 642c 0a20 2020 2020 2020 2020 2020  ved,.           
-00006ee0: 2073 6368 656d 613d 7363 6865 6d61 2c0a   schema=schema,.
-00006ef0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00006f00: 656e 743d 636f 6e74 656e 740a 2020 2020  ent=content.    
-00006f10: 2020 2020 290a 0a20 2020 2040 7374 6174      )..    @stat
-00006f20: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00006f30: 205f 5f74 6f5f 6865 6164 6572 7328 696e   __to_headers(in
-00006f40: 5f64 6174 613a 2074 7970 696e 672e 5475  _data: typing.Tu
-00006f50: 706c 655b 7479 7069 6e67 2e54 7570 6c65  ple[typing.Tuple
-00006f60: 5b73 7472 2c20 7374 725d 2c20 2e2e 2e5d  [str, str], ...]
-00006f70: 2920 2d3e 2048 5454 5048 6561 6465 7244  ) -> HTTPHeaderD
-00006f80: 6963 743a 0a20 2020 2020 2020 2064 6174  ict:.        dat
-00006f90: 6120 3d20 7475 706c 6528 7420 666f 7220  a = tuple(t for 
-00006fa0: 7420 696e 2069 6e5f 6461 7461 2069 6620  t in in_data if 
-00006fb0: 7429 0a20 2020 2020 2020 2068 6561 6465  t).        heade
-00006fc0: 7273 203d 2048 5454 5048 6561 6465 7244  rs = HTTPHeaderD
-00006fd0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-00006fe0: 206e 6f74 2064 6174 613a 0a20 2020 2020   not data:.     
-00006ff0: 2020 2020 2020 2072 6574 7572 6e20 6865         return he
-00007000: 6164 6572 730a 2020 2020 2020 2020 6865  aders.        he
-00007010: 6164 6572 732e 6578 7465 6e64 2864 6174  aders.extend(dat
-00007020: 6129 0a20 2020 2020 2020 2072 6574 7572  a).        retur
-00007030: 6e20 6865 6164 6572 730a 0a20 2020 2064  n headers..    d
-00007040: 6566 2073 6572 6961 6c69 7a65 280a 2020  ef serialize(.  
-00007050: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00007060: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
-00007070: 696e 672e 556e 696f 6e5b 0a20 2020 2020  ing.Union[.     
-00007080: 2020 2020 2020 2053 6368 656d 612c 2044         Schema, D
-00007090: 6563 696d 616c 2c20 696e 742c 2066 6c6f  ecimal, int, flo
-000070a0: 6174 2c20 7374 722c 2064 6174 652c 2064  at, str, date, d
-000070b0: 6174 6574 696d 652c 204e 6f6e 652c 2062  atetime, None, b
-000070c0: 6f6f 6c2c 206c 6973 742c 2074 7570 6c65  ool, list, tuple
-000070d0: 2c20 6469 6374 2c20 6672 6f7a 656e 6469  , dict, frozendi
-000070e0: 6374 2e66 726f 7a65 6e64 6963 745d 0a20  ct.frozendict]. 
-000070f0: 2020 2029 202d 3e20 4854 5450 4865 6164     ) -> HTTPHead
-00007100: 6572 4469 6374 3a0a 2020 2020 2020 2020  erDict:.        
-00007110: 6966 2073 656c 662e 7363 6865 6d61 3a0a  if self.schema:.
-00007120: 2020 2020 2020 2020 2020 2020 6361 7374              cast
-00007130: 5f69 6e5f 6461 7461 203d 2073 656c 662e  _in_data = self.
-00007140: 7363 6865 6d61 2869 6e5f 6461 7461 290a  schema(in_data).
-00007150: 2020 2020 2020 2020 2020 2020 6361 7374              cast
-00007160: 5f69 6e5f 6461 7461 203d 2073 656c 662e  _in_data = self.
-00007170: 5f6a 736f 6e5f 656e 636f 6465 722e 6465  _json_encoder.de
-00007180: 6661 756c 7428 6361 7374 5f69 6e5f 6461  fault(cast_in_da
-00007190: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
-000071a0: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-000071b0: 7369 6d70 6c65 202d 3e20 6865 6164 6572  simple -> header
-000071c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000071d0: 2068 6561 6465 7273 3a20 506f 6f6c 4d61   headers: PoolMa
-000071e0: 6e61 6765 7220 6e65 6564 7320 6120 6d61  nager needs a ma
-000071f0: 7070 696e 672c 2074 7570 6c65 2069 7320  pping, tuple is 
-00007200: 636c 6f73 650a 2020 2020 2020 2020 2020  close.          
-00007210: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007220: 7320 6865 6164 6572 733a 2064 6963 740a  s headers: dict.
-00007230: 2020 2020 2020 2020 2020 2020 2222 220a              """.
-00007240: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00007250: 656c 662e 7374 796c 653a 0a20 2020 2020  elf.style:.     
-00007260: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00007270: 203d 2073 656c 662e 5f73 6572 6961 6c69   = self._seriali
-00007280: 7a65 5f73 696d 706c 6528 6361 7374 5f69  ze_simple(cast_i
-00007290: 6e5f 6461 7461 2c20 7365 6c66 2e6e 616d  n_data, self.nam
-000072a0: 652c 2073 656c 662e 6578 706c 6f64 652c  e, self.explode,
-000072b0: 2046 616c 7365 290a 2020 2020 2020 2020   False).        
-000072c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000072d0: 656c 662e 5f5f 746f 5f68 6561 6465 7273  elf.__to_headers
-000072e0: 2828 2873 656c 662e 6e61 6d65 2c20 7661  (((self.name, va
-000072f0: 6c75 6529 2c29 290a 2020 2020 2020 2020  lue),)).        
-00007300: 2320 7365 6c66 2e63 6f6e 7465 6e74 2077  # self.content w
-00007310: 696c 6c20 6265 206c 656e 6774 6820 6f6e  ill be length on
-00007320: 650a 2020 2020 2020 2020 666f 7220 636f  e.        for co
-00007330: 6e74 656e 745f 7479 7065 2c20 7363 6865  ntent_type, sche
-00007340: 6d61 2069 6e20 7365 6c66 2e63 6f6e 7465  ma in self.conte
-00007350: 6e74 2e69 7465 6d73 2829 3a0a 2020 2020  nt.items():.    
-00007360: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
-00007370: 6461 7461 203d 2073 6368 656d 6128 696e  data = schema(in
-00007380: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
-00007390: 2020 2063 6173 745f 696e 5f64 6174 6120     cast_in_data 
-000073a0: 3d20 7365 6c66 2e5f 6a73 6f6e 5f65 6e63  = self._json_enc
-000073b0: 6f64 6572 2e64 6566 6175 6c74 2863 6173  oder.default(cas
-000073c0: 745f 696e 5f64 6174 6129 0a20 2020 2020  t_in_data).     
-000073d0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-000073e0: 636f 6e74 656e 745f 7479 7065 5f69 735f  content_type_is_
-000073f0: 6a73 6f6e 2863 6f6e 7465 6e74 5f74 7970  json(content_typ
-00007400: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00007410: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
-00007420: 2e5f 7365 7269 616c 697a 655f 6a73 6f6e  ._serialize_json
-00007430: 2863 6173 745f 696e 5f64 6174 6129 0a20  (cast_in_data). 
-00007440: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007450: 6574 7572 6e20 7365 6c66 2e5f 5f74 6f5f  eturn self.__to_
-00007460: 6865 6164 6572 7328 2828 7365 6c66 2e6e  headers(((self.n
-00007470: 616d 652c 2076 616c 7565 292c 2929 0a20  ame, value),)). 
-00007480: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00007490: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-000074a0: 7272 6f72 2827 5365 7269 616c 697a 6174  rror('Serializat
-000074b0: 696f 6e20 6f66 207b 7d20 6861 7320 6e6f  ion of {} has no
-000074c0: 7420 7965 7420 6265 656e 2069 6d70 6c65  t yet been imple
-000074d0: 6d65 6e74 6564 272e 666f 726d 6174 2863  mented'.format(c
-000074e0: 6f6e 7465 6e74 5f74 7970 6529 290a 0a0a  ontent_type))...
-000074f0: 636c 6173 7320 456e 636f 6469 6e67 3a0a  class Encoding:.
-00007500: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00007510: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00007520: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
-00007530: 7479 7065 3a20 7374 722c 0a20 2020 2020  type: str,.     
-00007540: 2020 2068 6561 6465 7273 3a20 7479 7069     headers: typi
-00007550: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-00007560: 6e67 2e44 6963 745b 7374 722c 2048 6561  ng.Dict[str, Hea
-00007570: 6465 7250 6172 616d 6574 6572 5d5d 203d  derParameter]] =
-00007580: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-00007590: 7479 6c65 3a20 7479 7069 6e67 2e4f 7074  tyle: typing.Opt
-000075a0: 696f 6e61 6c5b 5061 7261 6d65 7465 7253  ional[ParameterS
-000075b0: 7479 6c65 5d20 3d20 4e6f 6e65 2c0a 2020  tyle] = None,.  
-000075c0: 2020 2020 2020 6578 706c 6f64 653a 2062        explode: b
-000075d0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-000075e0: 2020 2020 2061 6c6c 6f77 5f72 6573 6572       allow_reser
-000075f0: 7665 643a 2062 6f6f 6c20 3d20 4661 6c73  ved: bool = Fals
-00007600: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-00007610: 2020 7365 6c66 2e63 6f6e 7465 6e74 5f74    self.content_t
-00007620: 7970 6520 3d20 636f 6e74 656e 745f 7479  ype = content_ty
-00007630: 7065 0a20 2020 2020 2020 2073 656c 662e  pe.        self.
-00007640: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-00007650: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-00007660: 7479 6c65 203d 2073 7479 6c65 0a20 2020  tyle = style.   
-00007670: 2020 2020 2073 656c 662e 6578 706c 6f64       self.explod
-00007680: 6520 3d20 6578 706c 6f64 650a 2020 2020  e = explode.    
-00007690: 2020 2020 7365 6c66 2e61 6c6c 6f77 5f72      self.allow_r
-000076a0: 6573 6572 7665 6420 3d20 616c 6c6f 775f  eserved = allow_
-000076b0: 7265 7365 7276 6564 0a0a 0a40 6461 7461  reserved...@data
-000076c0: 636c 6173 730a 636c 6173 7320 4d65 6469  class.class Medi
-000076d0: 6154 7970 653a 0a20 2020 2022 2222 0a20  aType:.    """. 
-000076e0: 2020 2055 7365 6420 746f 2073 746f 7265     Used to store
-000076f0: 2072 6571 7565 7374 2061 6e64 2072 6573   request and res
-00007700: 706f 6e73 6520 626f 6479 2073 6368 656d  ponse body schem
-00007710: 6120 696e 666f 726d 6174 696f 6e0a 2020  a information.  
-00007720: 2020 656e 636f 6469 6e67 3a0a 2020 2020    encoding:.    
-00007730: 2020 2020 4120 6d61 7020 6265 7477 6565      A map betwee
-00007740: 6e20 6120 7072 6f70 6572 7479 206e 616d  n a property nam
-00007750: 6520 616e 6420 6974 7320 656e 636f 6469  e and its encodi
-00007760: 6e67 2069 6e66 6f72 6d61 7469 6f6e 2e0a  ng information..
-00007770: 2020 2020 2020 2020 5468 6520 6b65 792c          The key,
-00007780: 2062 6569 6e67 2074 6865 2070 726f 7065   being the prope
-00007790: 7274 7920 6e61 6d65 2c20 4d55 5354 2065  rty name, MUST e
-000077a0: 7869 7374 2069 6e20 7468 6520 7363 6865  xist in the sche
-000077b0: 6d61 2061 7320 6120 7072 6f70 6572 7479  ma as a property
-000077c0: 2e0a 2020 2020 2020 2020 5468 6520 656e  ..        The en
-000077d0: 636f 6469 6e67 206f 626a 6563 7420 5348  coding object SH
-000077e0: 414c 4c20 6f6e 6c79 2061 7070 6c79 2074  ALL only apply t
-000077f0: 6f20 7265 7175 6573 7442 6f64 7920 6f62  o requestBody ob
-00007800: 6a65 6374 7320 7768 656e 2074 6865 206d  jects when the m
-00007810: 6564 6961 2074 7970 6520 6973 0a20 2020  edia type is.   
-00007820: 2020 2020 206d 756c 7469 7061 7274 206f       multipart o
-00007830: 7220 6170 706c 6963 6174 696f 6e2f 782d  r application/x-
-00007840: 7777 772d 666f 726d 2d75 726c 656e 636f  www-form-urlenco
-00007850: 6465 642e 0a20 2020 2022 2222 0a20 2020  ded..    """.   
-00007860: 2073 6368 656d 613a 2074 7970 696e 672e   schema: typing.
-00007870: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-00007880: 5479 7065 5b53 6368 656d 615d 5d20 3d20  Type[Schema]] = 
-00007890: 4e6f 6e65 0a20 2020 2065 6e63 6f64 696e  None.    encodin
-000078a0: 673a 2074 7970 696e 672e 4f70 7469 6f6e  g: typing.Option
-000078b0: 616c 5b74 7970 696e 672e 4469 6374 5b73  al[typing.Dict[s
-000078c0: 7472 2c20 456e 636f 6469 6e67 5d5d 203d  tr, Encoding]] =
-000078d0: 204e 6f6e 650a 0a0a 4064 6174 6163 6c61   None...@datacla
-000078e0: 7373 0a63 6c61 7373 2041 7069 5265 7370  ss.class ApiResp
-000078f0: 6f6e 7365 5769 7468 6f75 7444 6573 6572  onseWithoutDeser
-00007900: 6961 6c69 7a61 7469 6f6e 2841 7069 5265  ialization(ApiRe
-00007910: 7370 6f6e 7365 293a 0a20 2020 2072 6573  sponse):.    res
-00007920: 706f 6e73 653a 2075 726c 6c69 6233 2e48  ponse: urllib3.H
-00007930: 5454 5052 6573 706f 6e73 650a 2020 2020  TTPResponse.    
-00007940: 626f 6479 3a20 7479 7069 6e67 2e55 6e69  body: typing.Uni
-00007950: 6f6e 5b55 6e73 6574 2c20 7479 7069 6e67  on[Unset, typing
-00007960: 2e54 7970 655b 5363 6865 6d61 5d5d 203d  .Type[Schema]] =
-00007970: 2075 6e73 6574 0a0a 0a63 6c61 7373 204f   unset...class O
-00007980: 7065 6e41 7069 5265 7370 6f6e 7365 284a  penApiResponse(J
-00007990: 534f 4e44 6574 6563 746f 7229 3a0a 2020  SONDetector):.  
-000079a0: 2020 5f5f 6669 6c65 6e61 6d65 5f63 6f6e    __filename_con
-000079b0: 7465 6e74 5f64 6973 706f 7369 7469 6f6e  tent_disposition
-000079c0: 5f70 6174 7465 726e 203d 2072 652e 636f  _pattern = re.co
-000079d0: 6d70 696c 6528 2766 696c 656e 616d 653d  mpile('filename=
-000079e0: 2228 2e2b 3f29 2227 290a 0a20 2020 2064  "(.+?)"')..    d
-000079f0: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00007a00: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00007a10: 2020 2072 6573 706f 6e73 655f 636c 733a     response_cls:
-00007a20: 2074 7970 696e 672e 5479 7065 5b41 7069   typing.Type[Api
-00007a30: 5265 7370 6f6e 7365 5d20 3d20 4170 6952  Response] = ApiR
-00007a40: 6573 706f 6e73 652c 0a20 2020 2020 2020  esponse,.       
-00007a50: 2063 6f6e 7465 6e74 3a20 7479 7069 6e67   content: typing
-00007a60: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00007a70: 2e44 6963 745b 7374 722c 204d 6564 6961  .Dict[str, Media
-00007a80: 5479 7065 5d5d 203d 204e 6f6e 652c 0a20  Type]] = None,. 
-00007a90: 2020 2020 2020 2068 6561 6465 7273 3a20         headers: 
-00007aa0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00007ab0: 7479 7069 6e67 2e4c 6973 745b 4865 6164  typing.List[Head
-00007ac0: 6572 5061 7261 6d65 7465 725d 5d20 3d20  erParameter]] = 
-00007ad0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-00007ae0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-00007af0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-00007b00: 2020 2020 6966 2063 6f6e 7465 6e74 2069      if content i
-00007b10: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
-00007b20: 656e 2863 6f6e 7465 6e74 2920 3d3d 2030  en(content) == 0
-00007b30: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00007b40: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-00007b50: 496e 7661 6c69 6420 7661 6c75 6520 666f  Invalid value fo
-00007b60: 7220 636f 6e74 656e 742c 2074 6865 2063  r content, the c
-00007b70: 6f6e 7465 6e74 2064 6963 7420 6d75 7374  ontent dict must
-00007b80: 2068 6176 6520 3e3d 2031 2065 6e74 7279   have >= 1 entry
-00007b90: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-00007ba0: 636f 6e74 656e 7420 3d20 636f 6e74 656e  content = conten
-00007bb0: 740a 2020 2020 2020 2020 7365 6c66 2e72  t.        self.r
-00007bc0: 6573 706f 6e73 655f 636c 7320 3d20 7265  esponse_cls = re
-00007bd0: 7370 6f6e 7365 5f63 6c73 0a0a 2020 2020  sponse_cls..    
-00007be0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
-00007bf0: 2020 6465 6620 5f5f 6465 7365 7269 616c    def __deserial
-00007c00: 697a 655f 6a73 6f6e 2872 6573 706f 6e73  ize_json(respons
-00007c10: 653a 2075 726c 6c69 6233 2e48 5454 5052  e: urllib3.HTTPR
-00007c20: 6573 706f 6e73 6529 202d 3e20 7479 7069  esponse) -> typi
-00007c30: 6e67 2e41 6e79 3a0a 2020 2020 2020 2020  ng.Any:.        
-00007c40: 2320 7079 7468 6f6e 206d 7573 7420 6265  # python must be
-00007c50: 203e 3d20 332e 3920 736f 2077 6520 6361   >= 3.9 so we ca
-00007c60: 6e20 7061 7373 2069 6e20 6279 7465 7320  n pass in bytes 
-00007c70: 696e 746f 206a 736f 6e2e 6c6f 6164 730a  into json.loads.
-00007c80: 2020 2020 2020 2020 7265 7475 726e 206a          return j
-00007c90: 736f 6e2e 6c6f 6164 7328 7265 7370 6f6e  son.loads(respon
-00007ca0: 7365 2e64 6174 6129 0a0a 2020 2020 4073  se.data)..    @s
-00007cb0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00007cc0: 6465 6620 5f5f 6669 6c65 5f6e 616d 655f  def __file_name_
-00007cd0: 6672 6f6d 5f72 6573 706f 6e73 655f 7572  from_response_ur
-00007ce0: 6c28 7265 7370 6f6e 7365 5f75 726c 3a20  l(response_url: 
-00007cf0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00007d00: 7374 725d 2920 2d3e 2074 7970 696e 672e  str]) -> typing.
-00007d10: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
-00007d20: 2020 2020 2020 2069 6620 7265 7370 6f6e         if respon
-00007d30: 7365 5f75 726c 2069 7320 4e6f 6e65 3a0a  se_url is None:.
-00007d40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00007d50: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-00007d60: 7572 6c5f 7061 7468 203d 2075 726c 7061  url_path = urlpa
-00007d70: 7273 6528 7265 7370 6f6e 7365 5f75 726c  rse(response_url
-00007d80: 292e 7061 7468 0a20 2020 2020 2020 2069  ).path.        i
-00007d90: 6620 7572 6c5f 7061 7468 3a0a 2020 2020  f url_path:.    
-00007da0: 2020 2020 2020 2020 7061 7468 5f62 6173          path_bas
-00007db0: 656e 616d 6520 3d20 6f73 2e70 6174 682e  ename = os.path.
-00007dc0: 6261 7365 6e61 6d65 2875 726c 5f70 6174  basename(url_pat
-00007dd0: 6829 0a20 2020 2020 2020 2020 2020 2069  h).            i
-00007de0: 6620 7061 7468 5f62 6173 656e 616d 653a  f path_basename:
-00007df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007e00: 205f 6669 6c65 6e61 6d65 2c20 6578 7420   _filename, ext 
-00007e10: 3d20 6f73 2e70 6174 682e 7370 6c69 7465  = os.path.splite
-00007e20: 7874 2870 6174 685f 6261 7365 6e61 6d65  xt(path_basename
-00007e30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00007e40: 2020 6966 2065 7874 3a0a 2020 2020 2020    if ext:.      
-00007e50: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00007e60: 7475 726e 2070 6174 685f 6261 7365 6e61  turn path_basena
-00007e70: 6d65 0a20 2020 2020 2020 2072 6574 7572  me.        retur
-00007e80: 6e20 4e6f 6e65 0a0a 2020 2020 4063 6c61  n None..    @cla
-00007e90: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00007ea0: 205f 5f66 696c 655f 6e61 6d65 5f66 726f   __file_name_fro
-00007eb0: 6d5f 636f 6e74 656e 745f 6469 7370 6f73  m_content_dispos
-00007ec0: 6974 696f 6e28 636c 732c 2063 6f6e 7465  ition(cls, conte
-00007ed0: 6e74 5f64 6973 706f 7369 7469 6f6e 3a20  nt_disposition: 
-00007ee0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00007ef0: 7374 725d 2920 2d3e 2074 7970 696e 672e  str]) -> typing.
-00007f00: 4f70 7469 6f6e 616c 5b73 7472 5d3a 0a20  Optional[str]:. 
-00007f10: 2020 2020 2020 2069 6620 636f 6e74 656e         if conten
-00007f20: 745f 6469 7370 6f73 6974 696f 6e20 6973  t_disposition is
-00007f30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007f40: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
-00007f50: 2020 2020 2020 206d 6174 6368 203d 2063         match = c
-00007f60: 6c73 2e5f 5f66 696c 656e 616d 655f 636f  ls.__filename_co
-00007f70: 6e74 656e 745f 6469 7370 6f73 6974 696f  ntent_dispositio
-00007f80: 6e5f 7061 7474 6572 6e2e 7365 6172 6368  n_pattern.search
-00007f90: 2863 6f6e 7465 6e74 5f64 6973 706f 7369  (content_disposi
-00007fa0: 7469 6f6e 290a 2020 2020 2020 2020 6966  tion).        if
-00007fb0: 206e 6f74 206d 6174 6368 3a0a 2020 2020   not match:.    
-00007fc0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
-00007fd0: 6f6e 650a 2020 2020 2020 2020 7265 7475  one.        retu
-00007fe0: 726e 206d 6174 6368 2e67 726f 7570 2831  rn match.group(1
-00007ff0: 290a 0a20 2020 2064 6566 205f 5f64 6573  )..    def __des
-00008000: 6572 6961 6c69 7a65 5f61 7070 6c69 6361  erialize_applica
-00008010: 7469 6f6e 5f6f 6374 6574 5f73 7472 6561  tion_octet_strea
-00008020: 6d28 0a20 2020 2020 2020 2073 656c 662c  m(.        self,
-00008030: 2072 6573 706f 6e73 653a 2075 726c 6c69   response: urlli
-00008040: 6233 2e48 5454 5052 6573 706f 6e73 650a  b3.HTTPResponse.
-00008050: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
-00008060: 556e 696f 6e5b 6279 7465 732c 2069 6f2e  Union[bytes, io.
-00008070: 4275 6666 6572 6564 5265 6164 6572 5d3a  BufferedReader]:
-00008080: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008090: 2020 2020 2075 726c 6c69 6233 2075 7365       urllib3 use
-000080a0: 2063 6173 6573 3a0a 2020 2020 2020 2020   cases:.        
-000080b0: 312e 2077 6865 6e20 7072 656c 6f61 645f  1. when preload_
-000080c0: 636f 6e74 656e 743d 5472 7565 2028 7374  content=True (st
-000080d0: 7265 616d 3d46 616c 7365 2920 7468 656e  ream=False) then
-000080e0: 2073 7570 706f 7274 735f 6368 756e 6b65   supports_chunke
-000080f0: 645f 7265 6164 7320 6973 2046 616c 7365  d_reads is False
-00008100: 2061 6e64 2062 7974 6573 2061 7265 2072   and bytes are r
-00008110: 6574 7572 6e65 640a 2020 2020 2020 2020  eturned.        
-00008120: 322e 2077 6865 6e20 7072 656c 6f61 645f  2. when preload_
-00008130: 636f 6e74 656e 743d 4661 6c73 6520 2873  content=False (s
-00008140: 7472 6561 6d3d 5472 7565 2920 7468 656e  tream=True) then
-00008150: 2073 7570 706f 7274 735f 6368 756e 6b65   supports_chunke
-00008160: 645f 7265 6164 7320 6973 2054 7275 6520  d_reads is True 
-00008170: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00008180: 6120 6669 6c65 2077 696c 6c20 6265 2077  a file will be w
-00008190: 7269 7474 656e 2061 6e64 2072 6574 7572  ritten and retur
-000081a0: 6e65 640a 2020 2020 2020 2020 2222 220a  ned.        """.
-000081b0: 2020 2020 2020 2020 6966 2072 6573 706f          if respo
-000081c0: 6e73 652e 7375 7070 6f72 7473 5f63 6875  nse.supports_chu
-000081d0: 6e6b 6564 5f72 6561 6473 2829 3a0a 2020  nked_reads():.  
-000081e0: 2020 2020 2020 2020 2020 6669 6c65 5f6e            file_n
-000081f0: 616d 6520 3d20 280a 2020 2020 2020 2020  ame = (.        
-00008200: 2020 2020 2020 2020 7365 6c66 2e5f 5f66          self.__f
-00008210: 696c 655f 6e61 6d65 5f66 726f 6d5f 636f  ile_name_from_co
-00008220: 6e74 656e 745f 6469 7370 6f73 6974 696f  ntent_dispositio
-00008230: 6e28 7265 7370 6f6e 7365 2e68 6561 6465  n(response.heade
-00008240: 7273 2e67 6574 2827 636f 6e74 656e 742d  rs.get('content-
-00008250: 6469 7370 6f73 6974 696f 6e27 2929 0a20  disposition')). 
-00008260: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00008270: 7220 7365 6c66 2e5f 5f66 696c 655f 6e61  r self.__file_na
-00008280: 6d65 5f66 726f 6d5f 7265 7370 6f6e 7365  me_from_response
-00008290: 5f75 726c 2872 6573 706f 6e73 652e 6765  _url(response.ge
-000082a0: 7475 726c 2829 290a 2020 2020 2020 2020  turl()).        
-000082b0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-000082c0: 2020 2069 6620 6669 6c65 5f6e 616d 6520     if file_name 
-000082d0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000082e0: 2020 2020 2020 2020 205f 6664 2c20 7061           _fd, pa
-000082f0: 7468 203d 2074 656d 7066 696c 652e 6d6b  th = tempfile.mk
-00008300: 7374 656d 7028 290a 2020 2020 2020 2020  stemp().        
-00008310: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008320: 2020 2020 2020 2020 2020 7061 7468 203d            path =
-00008330: 206f 732e 7061 7468 2e6a 6f69 6e28 7465   os.path.join(te
-00008340: 6d70 6669 6c65 2e67 6574 7465 6d70 6469  mpfile.gettempdi
-00008350: 7228 292c 2066 696c 655f 6e61 6d65 290a  r(), file_name).
-00008360: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00008370: 6820 6f70 656e 2870 6174 682c 2027 7762  h open(path, 'wb
-00008380: 2729 2061 7320 6e65 775f 6669 6c65 3a0a  ') as new_file:.
-00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083a0: 6368 756e 6b5f 7369 7a65 203d 2031 3032  chunk_size = 102
-000083b0: 340a 2020 2020 2020 2020 2020 2020 2020  4.              
-000083c0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
-000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 2020 6461 7461 203d 2072 6573 706f 6e73    data = respons
-000083f0: 652e 7265 6164 2863 6875 6e6b 5f73 697a  e.read(chunk_siz
-00008400: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00008410: 2020 2020 2020 2069 6620 6e6f 7420 6461         if not da
-00008420: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00008430: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00008440: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-00008450: 2020 2020 2020 6e65 775f 6669 6c65 2e77        new_file.w
-00008460: 7269 7465 2864 6174 6129 0a20 2020 2020  rite(data).     
-00008470: 2020 2020 2020 2023 2072 656c 6561 7365         # release
-00008480: 5f63 6f6e 6e20 6973 206e 6565 6465 6420  _conn is needed 
-00008490: 666f 7220 7374 7265 616d 696e 6720 636f  for streaming co
-000084a0: 6e6e 6563 7469 6f6e 7320 6f6e 6c79 0a20  nnections only. 
-000084b0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-000084c0: 6e73 652e 7265 6c65 6173 655f 636f 6e6e  nse.release_conn
-000084d0: 2829 0a20 2020 2020 2020 2020 2020 206e  ().            n
-000084e0: 6577 5f66 696c 6520 3d20 6f70 656e 2870  ew_file = open(p
-000084f0: 6174 682c 2027 7262 2729 0a20 2020 2020  ath, 'rb').     
-00008500: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
-00008510: 775f 6669 6c65 0a20 2020 2020 2020 2065  w_file.        e
-00008520: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00008530: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00008540: 2e64 6174 610a 0a20 2020 2040 7374 6174  .data..    @stat
-00008550: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
-00008560: 205f 5f64 6573 6572 6961 6c69 7a65 5f6d   __deserialize_m
-00008570: 756c 7469 7061 7274 5f66 6f72 6d5f 6461  ultipart_form_da
-00008580: 7461 280a 2020 2020 2020 2020 7265 7370  ta(.        resp
-00008590: 6f6e 7365 3a20 7572 6c6c 6962 332e 4854  onse: urllib3.HT
-000085a0: 5450 5265 7370 6f6e 7365 0a20 2020 2029  TPResponse.    )
-000085b0: 202d 3e20 7479 7069 6e67 2e44 6963 745b   -> typing.Dict[
-000085c0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
-000085d0: 3a0a 2020 2020 2020 2020 6d73 6720 3d20  :.        msg = 
-000085e0: 656d 6169 6c2e 6d65 7373 6167 655f 6672  email.message_fr
-000085f0: 6f6d 5f62 7974 6573 2872 6573 706f 6e73  om_bytes(respons
-00008600: 652e 6461 7461 290a 2020 2020 2020 2020  e.data).        
-00008610: 7265 7475 726e 207b 0a20 2020 2020 2020  return {.       
-00008620: 2020 2020 2070 6172 742e 6765 745f 7061       part.get_pa
-00008630: 7261 6d28 226e 616d 6522 2c20 6865 6164  ram("name", head
-00008640: 6572 3d22 436f 6e74 656e 742d 4469 7370  er="Content-Disp
-00008650: 6f73 6974 696f 6e22 293a 2070 6172 742e  osition"): part.
-00008660: 6765 745f 7061 796c 6f61 6428 0a20 2020  get_payload(.   
-00008670: 2020 2020 2020 2020 2020 2020 2064 6563               dec
-00008680: 6f64 653d 5472 7565 0a20 2020 2020 2020  ode=True.       
-00008690: 2020 2020 2029 2e64 6563 6f64 6528 7061       ).decode(pa
-000086a0: 7274 2e67 6574 5f63 6f6e 7465 6e74 5f63  rt.get_content_c
-000086b0: 6861 7273 6574 2829 290a 2020 2020 2020  harset()).      
-000086c0: 2020 2020 2020 6966 2070 6172 742e 6765        if part.ge
-000086d0: 745f 636f 6e74 656e 745f 6368 6172 7365  t_content_charse
-000086e0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000086f0: 656c 7365 2070 6172 742e 6765 745f 7061  else part.get_pa
-00008700: 796c 6f61 6428 290a 2020 2020 2020 2020  yload().        
-00008710: 2020 2020 666f 7220 7061 7274 2069 6e20      for part in 
-00008720: 6d73 672e 6765 745f 7061 796c 6f61 6428  msg.get_payload(
-00008730: 290a 2020 2020 2020 2020 7d0a 0a20 2020  ).        }..   
-00008740: 2064 6566 205f 5f67 6574 5f73 6368 656d   def __get_schem
-00008750: 615f 666f 725f 636f 6e74 656e 745f 7479  a_for_content_ty
-00008760: 7065 280a 2020 2020 2020 2020 7365 6c66  pe(.        self
-00008770: 2c0a 2020 2020 2020 2020 636f 6e74 656e  ,.        conten
-00008780: 745f 7479 7065 0a20 2020 2029 202d 3e20  t_type.    ) -> 
-00008790: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000087a0: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
-000087b0: 6d61 5d5d 3a0a 2020 2020 2020 2020 2222  ma]]:.        ""
-000087c0: 220a 2020 2020 2020 2020 4669 6e64 7320  ".        Finds 
-000087d0: 7468 6520 636f 7272 6563 7420 5363 6865  the correct Sche
-000087e0: 6d61 4f62 6a65 6374 2066 6f72 2061 2070  maObject for a p
-000087f0: 6172 7469 6375 6c61 7220 636f 6e74 656e  articular conten
-00008800: 7420 7479 7065 2e20 4861 6e64 6c65 730a  t type. Handles.
-00008810: 2020 2020 2020 2020 7468 6520 6173 7465          the aste
-00008820: 7269 736b 2022 2a22 2063 6861 7261 6374  risk "*" charact
-00008830: 6572 2074 6861 7420 6973 2075 7365 6420  er that is used 
-00008840: 746f 2067 726f 7570 206d 6564 6961 2074  to group media t
-00008850: 7970 6573 2069 6e74 6f20 7261 6e67 6573  ypes into ranges
-00008860: 0a20 2020 2020 2020 2028 6874 7470 733a  .        (https:
-00008870: 2f2f 7777 772e 7266 632d 6564 6974 6f72  //www.rfc-editor
-00008880: 2e6f 7267 2f72 6663 2f72 6663 3732 3331  .org/rfc/rfc7231
-00008890: 2373 6563 7469 6f6e 2d35 2e33 2e32 292e  #section-5.3.2).
-000088a0: 2041 6c73 6f20 6861 6e64 6c65 730a 2020   Also handles.  
-000088b0: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
-000088c0: 2069 6e20 7468 6520 666f 726d 206f 6620   in the form of 
-000088d0: 6e61 6d65 3d76 616c 7565 2070 6169 7273  name=value pairs
-000088e0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-000088f0: 2020 2020 2020 6d65 6469 615f 7479 7065        media_type
-00008900: 7320 3d20 7365 6c66 2e63 6f6e 7465 6e74  s = self.content
-00008910: 2e6b 6579 7328 290a 2020 2020 2020 2020  .keys().        
-00008920: 6d61 7463 6865 645f 6d65 6469 615f 7479  matched_media_ty
-00008930: 7065 203d 204f 7065 6e41 7069 5265 7370  pe = OpenApiResp
-00008940: 6f6e 7365 2e6d 6174 6368 5f63 6f6e 7465  onse.match_conte
-00008950: 6e74 5f74 7970 6528 0a20 2020 2020 2020  nt_type(.       
-00008960: 2020 2020 2063 6f6e 7465 6e74 5f74 7970       content_typ
-00008970: 653d 636f 6e74 656e 745f 7479 7065 2c0a  e=content_type,.
-00008980: 2020 2020 2020 2020 2020 2020 6d65 6469              medi
-00008990: 615f 7479 7065 733d 6d65 6469 615f 7479  a_types=media_ty
-000089a0: 7065 730a 2020 2020 2020 2020 290a 2020  pes.        ).  
-000089b0: 2020 2020 2020 6966 206d 6174 6368 6564        if matched
-000089c0: 5f6d 6564 6961 5f74 7970 6520 6973 204e  _media_type is N
-000089d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000089e0: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
-000089f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00008a00: 2e63 6f6e 7465 6e74 5b6d 6174 6368 6564  .content[matched
-00008a10: 5f6d 6564 6961 5f74 7970 655d 2e73 6368  _media_type].sch
-00008a20: 656d 610a 0a20 2020 2040 7374 6174 6963  ema..    @static
-00008a30: 6d65 7468 6f64 0a20 2020 2064 6566 206d  method.    def m
-00008a40: 6174 6368 5f63 6f6e 7465 6e74 5f74 7970  atch_content_typ
-00008a50: 6528 636f 6e74 656e 745f 7479 7065 3a20  e(content_type: 
-00008a60: 7374 722c 206d 6564 6961 5f74 7970 6573  str, media_types
-00008a70: 3a20 7479 7069 6e67 2e4c 6973 745b 7374  : typing.List[st
-00008a80: 725d 2920 2d3e 2074 7970 696e 672e 4f70  r]) -> typing.Op
-00008a90: 7469 6f6e 616c 5b73 7472 5d3a 0a20 2020  tional[str]:.   
-00008aa0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00008ab0: 204d 6174 6368 6573 2061 2063 6f6e 7465   Matches a conte
-00008ac0: 6e74 2074 7970 6520 746f 2061 206d 6564  nt type to a med
-00008ad0: 6961 2074 7970 6520 696e 2061 206c 6973  ia type in a lis
-00008ae0: 7420 6f66 206d 6564 6961 2074 7970 6573  t of media types
-00008af0: 2c20 6861 6e64 6c69 6e67 206d 6564 6961  , handling media
-00008b00: 2074 7970 6520 7261 6e67 6573 2061 7320   type ranges as 
-00008b10: 6465 6669 6e65 6420 696e 2052 4643 3732  defined in RFC72
-00008b20: 3331 2e0a 0a20 2020 2020 2020 2050 6172  31...        Par
-00008b30: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-00008b40: 2063 6f6e 7465 6e74 5f74 7970 6520 2873   content_type (s
-00008b50: 7472 293a 2054 6865 2063 6f6e 7465 6e74  tr): The content
-00008b60: 2074 7970 6520 746f 206d 6174 6368 2e0a   type to match..
-00008b70: 2020 2020 2020 2020 6d65 6469 615f 7479          media_ty
-00008b80: 7065 7320 286c 6973 7429 3a20 5468 6520  pes (list): The 
-00008b90: 6c69 7374 206f 6620 6d65 6469 6120 7479  list of media ty
-00008ba0: 7065 7320 746f 2073 6561 7263 682e 0a0a  pes to search...
-00008bb0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00008bc0: 0a20 2020 2020 2020 2073 7472 3a20 5468  .        str: Th
-00008bd0: 6520 6669 7273 7420 6d65 6469 6120 7479  e first media ty
-00008be0: 7065 2074 6861 7420 6d61 7463 6865 7320  pe that matches 
-00008bf0: 7468 6520 636f 6e74 656e 7420 7479 7065  the content type
-00008c00: 2c20 6f72 204e 6f6e 6520 6966 206e 6f20  , or None if no 
-00008c10: 6d61 7463 6820 6973 2066 6f75 6e64 2e0a  match is found..
-00008c20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008c30: 2020 2020 666f 7220 6d65 6469 615f 7479      for media_ty
-00008c40: 7065 2069 6e20 6d65 6469 615f 7479 7065  pe in media_type
-00008c50: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00008c60: 6620 6d65 6469 615f 7479 7065 203d 3d20  f media_type == 
-00008c70: 272a 2f2a 2720 6f72 206d 6564 6961 5f74  '*/*' or media_t
-00008c80: 7970 6520 3d3d 2063 6f6e 7465 6e74 5f74  ype == content_t
-00008c90: 7970 653a 0a20 2020 2020 2020 2020 2020  ype:.           
-00008ca0: 2020 2020 2072 6574 7572 6e20 6d65 6469       return medi
-00008cb0: 615f 7479 7065 0a20 2020 2020 2020 2020  a_type.         
-00008cc0: 2020 2065 6c69 6620 272f 2720 696e 206d     elif '/' in m
-00008cd0: 6564 6961 5f74 7970 653a 0a20 2020 2020  edia_type:.     
-00008ce0: 2020 2020 2020 2020 2020 2074 7970 655f             type_
-00008cf0: 2c20 7375 6274 7970 6520 3d20 6d65 6469  , subtype = medi
-00008d00: 615f 7479 7065 2e73 706c 6974 2827 2f27  a_type.split('/'
-00008d10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008d20: 2020 6966 2028 7479 7065 5f20 3d3d 2027    if (type_ == '
-00008d30: 2a27 206f 7220 7479 7065 5f20 3d3d 2063  *' or type_ == c
-00008d40: 6f6e 7465 6e74 5f74 7970 652e 7370 6c69  ontent_type.spli
-00008d50: 7428 272f 2729 5b30 5d29 2061 6e64 205c  t('/')[0]) and \
-00008d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d70: 2028 7375 6274 7970 6520 3d3d 2027 2a27   (subtype == '*'
-00008d80: 206f 7220 7375 6274 7970 6520 3d3d 2063   or subtype == c
-00008d90: 6f6e 7465 6e74 5f74 7970 652e 7370 6c69  ontent_type.spli
-00008da0: 7428 272f 2729 5b31 5d2e 7370 6c69 7428  t('/')[1].split(
-00008db0: 273b 2729 5b30 5d29 3a0a 2020 2020 2020  ';')[0]):.      
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00008dd0: 7475 726e 206d 6564 6961 5f74 7970 650a  turn media_type.
-00008de0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008df0: 4e6f 6e65 0a0a 2020 2020 6465 6620 6465  None..    def de
-00008e00: 7365 7269 616c 697a 6528 7365 6c66 2c20  serialize(self, 
-00008e10: 7265 7370 6f6e 7365 3a20 5265 7370 6f6e  response: Respon
-00008e20: 7365 5772 6170 7065 722c 2063 6f6e 6669  seWrapper, confi
-00008e30: 6775 7261 7469 6f6e 3a20 436f 6e66 6967  guration: Config
-00008e40: 7572 6174 696f 6e2c 2073 6b69 705f 6465  uration, skip_de
-00008e50: 7365 7269 616c 697a 6174 696f 6e20 3d20  serialization = 
-00008e60: 4661 6c73 6529 202d 3e20 4170 6952 6573  False) -> ApiRes
-00008e70: 706f 6e73 653a 0a20 2020 2020 2020 2063  ponse:.        c
-00008e80: 6f6e 7465 6e74 5f74 7970 6520 3d20 7265  ontent_type = re
-00008e90: 7370 6f6e 7365 2e68 7474 705f 7265 7370  sponse.http_resp
-00008ea0: 6f6e 7365 2e68 6561 6465 7273 2e67 6574  onse.headers.get
-00008eb0: 2827 636f 6e74 656e 742d 7479 7065 2729  ('content-type')
-00008ec0: 0a20 2020 2020 2020 2064 6573 6572 6961  .        deseria
-00008ed0: 6c69 7a65 645f 626f 6479 203d 2075 6e73  lized_body = uns
-00008ee0: 6574 0a20 2020 2020 2020 2073 7472 6561  et.        strea
-00008ef0: 6d65 6420 3d20 7265 7370 6f6e 7365 2e68  med = response.h
-00008f00: 7474 705f 7265 7370 6f6e 7365 2e73 7570  ttp_response.sup
-00008f10: 706f 7274 735f 6368 756e 6b65 645f 7265  ports_chunked_re
-00008f20: 6164 7328 290a 0a20 2020 2020 2020 2064  ads()..        d
-00008f30: 6573 6572 6961 6c69 7a65 645f 6865 6164  eserialized_head
-00008f40: 6572 7320 3d20 756e 7365 740a 2020 2020  ers = unset.    
-00008f50: 2020 2020 6966 2073 656c 662e 6865 6164      if self.head
-00008f60: 6572 7320 6973 206e 6f74 204e 6f6e 653a  ers is not None:
-00008f70: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00008f80: 4f44 4f20 6164 6420 6865 6164 6572 2064  ODO add header d
-00008f90: 6573 6572 6961 6c69 6174 696f 6e20 6865  eserialiation he
-00008fa0: 7265 0a20 2020 2020 2020 2020 2020 2070  re.            p
-00008fb0: 6173 730a 0a20 2020 2020 2020 2069 6620  ass..        if 
-00008fc0: 7365 6c66 2e63 6f6e 7465 6e74 2069 7320  self.content is 
-00008fd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00008fe0: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
-00008ff0: 662e 636f 6e74 656e 7429 203d 3d20 303a  f.content) == 0:
-00009000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009010: 2023 2073 6f6d 6520 7370 6563 7320 646f   # some specs do
-00009020: 206e 6f74 2064 6566 696e 6520 7265 7370   not define resp
-00009030: 6f6e 7365 2063 6f6e 7465 6e74 206d 6564  onse content med
-00009040: 6961 2074 7970 6520 7363 6865 6d61 730a  ia type schemas.
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 7265 7475 726e 2073 656c 662e 7265 7370  return self.resp
-00009070: 6f6e 7365 5f63 6c73 280a 2020 2020 2020  onse_cls(.      
-00009080: 2020 2020 2020 2020 2020 2020 2020 726f                ro
-00009090: 756e 645f 7472 6970 5f74 696d 653d 7265  und_trip_time=re
-000090a0: 7370 6f6e 7365 2e72 6f75 6e64 5f74 7269  sponse.round_tri
-000090b0: 705f 7469 6d65 2c0a 2020 2020 2020 2020  p_time,.        
-000090c0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-000090d0: 6f6e 7365 3d72 6573 706f 6e73 652e 6874  onse=response.ht
-000090e0: 7470 5f72 6573 706f 6e73 652c 0a20 2020  tp_response,.   
-000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009100: 2062 6f64 793d 756e 7365 742c 0a20 2020   body=unset,.   
-00009110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009120: 2068 6561 6465 7273 3d72 6573 706f 6e73   headers=respons
-00009130: 652e 6874 7470 5f72 6573 706f 6e73 652e  e.http_response.
-00009140: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
-00009150: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00009160: 7475 733d 7265 7370 6f6e 7365 2e68 7474  tus=response.htt
-00009170: 705f 7265 7370 6f6e 7365 2e73 7461 7475  p_response.statu
-00009180: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00009190: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000091a0: 626f 6479 5f73 6368 656d 6120 3d20 7365  body_schema = se
-000091b0: 6c66 2e5f 5f67 6574 5f73 6368 656d 615f  lf.__get_schema_
-000091c0: 666f 725f 636f 6e74 656e 745f 7479 7065  for_content_type
-000091d0: 2863 6f6e 7465 6e74 5f74 7970 6529 0a20  (content_type). 
-000091e0: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
-000091f0: 6479 5f73 6368 656d 6120 6973 204e 6f6e  dy_schema is Non
-00009200: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009210: 2020 2072 6169 7365 2041 7069 5661 6c75     raise ApiValu
-00009220: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00009230: 2020 2020 2020 2020 2020 2020 6622 496e              f"In
-00009240: 7661 6c69 6420 636f 6e74 656e 745f 7479  valid content_ty
-00009250: 7065 2072 6574 7572 6e65 642e 2043 6f6e  pe returned. Con
-00009260: 7465 6e74 5f74 7970 653d 277b 636f 6e74  tent_type='{cont
-00009270: 656e 745f 7479 7065 7d27 2077 6173 2072  ent_type}' was r
-00009280: 6574 7572 6e65 6420 220a 2020 2020 2020  eturned ".      
-00009290: 2020 2020 2020 2020 2020 2020 2020 6622                f"
-000092a0: 7768 656e 206f 6e6c 7920 7b73 7472 2873  when only {str(s
-000092b0: 6574 2873 656c 662e 636f 6e74 656e 7429  et(self.content)
-000092c0: 297d 2061 7265 2064 6566 696e 6564 2066  )} are defined f
-000092d0: 6f72 2073 7461 7475 735f 636f 6465 3d7b  or status_code={
-000092e0: 7374 7228 7265 7370 6f6e 7365 2e68 7474  str(response.htt
-000092f0: 705f 7265 7370 6f6e 7365 2e73 7461 7475  p_response.statu
-00009300: 7329 7d22 0a20 2020 2020 2020 2020 2020  s)}".           
-00009310: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00009320: 2020 2020 6966 2073 656c 662e 5f63 6f6e      if self._con
-00009330: 7465 6e74 5f74 7970 655f 6973 5f6a 736f  tent_type_is_jso
-00009340: 6e28 636f 6e74 656e 745f 7479 7065 293a  n(content_type):
-00009350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009360: 2062 6f64 795f 6461 7461 203d 2073 656c   body_data = sel
-00009370: 662e 5f5f 6465 7365 7269 616c 697a 655f  f.__deserialize_
-00009380: 6a73 6f6e 2872 6573 706f 6e73 652e 6874  json(response.ht
-00009390: 7470 5f72 6573 706f 6e73 6529 0a20 2020  tp_response).   
-000093a0: 2020 2020 2020 2020 2065 6c69 6620 636f           elif co
-000093b0: 6e74 656e 745f 7479 7065 203d 3d20 2761  ntent_type == 'a
-000093c0: 7070 6c69 6361 7469 6f6e 2f6f 6374 6574  pplication/octet
-000093d0: 2d73 7472 6561 6d27 3a0a 2020 2020 2020  -stream':.      
-000093e0: 2020 2020 2020 2020 2020 626f 6479 5f64            body_d
-000093f0: 6174 6120 3d20 7365 6c66 2e5f 5f64 6573  ata = self.__des
-00009400: 6572 6961 6c69 7a65 5f61 7070 6c69 6361  erialize_applica
-00009410: 7469 6f6e 5f6f 6374 6574 5f73 7472 6561  tion_octet_strea
-00009420: 6d28 7265 7370 6f6e 7365 2e68 7474 705f  m(response.http_
-00009430: 7265 7370 6f6e 7365 290a 2020 2020 2020  response).      
-00009440: 2020 2020 2020 656c 6966 2063 6f6e 7465        elif conte
-00009450: 6e74 5f74 7970 652e 7374 6172 7473 7769  nt_type.startswi
-00009460: 7468 2827 6d75 6c74 6970 6172 742f 666f  th('multipart/fo
-00009470: 726d 2d64 6174 6127 293a 0a20 2020 2020  rm-data'):.     
-00009480: 2020 2020 2020 2020 2020 2062 6f64 795f             body_
-00009490: 6461 7461 203d 2073 656c 662e 5f5f 6465  data = self.__de
-000094a0: 7365 7269 616c 697a 655f 6d75 6c74 6970  serialize_multip
-000094b0: 6172 745f 666f 726d 5f64 6174 6128 7265  art_form_data(re
-000094c0: 7370 6f6e 7365 2e68 7474 705f 7265 7370  sponse.http_resp
-000094d0: 6f6e 7365 290a 2020 2020 2020 2020 2020  onse).          
-000094e0: 2020 2020 2020 636f 6e74 656e 745f 7479        content_ty
-000094f0: 7065 203d 2027 6d75 6c74 6970 6172 742f  pe = 'multipart/
-00009500: 666f 726d 2d64 6174 6127 0a20 2020 2020  form-data'.     
-00009510: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00009520: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00009530: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00009540: 6445 7272 6f72 2827 4465 7365 7269 616c  dError('Deserial
-00009550: 697a 6174 696f 6e20 6f66 207b 7d20 6861  ization of {} ha
-00009560: 7320 6e6f 7420 7965 7420 6265 656e 2069  s not yet been i
-00009570: 6d70 6c65 6d65 6e74 6564 272e 666f 726d  mplemented'.form
-00009580: 6174 2863 6f6e 7465 6e74 5f74 7970 6529  at(content_type)
-00009590: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-000095a0: 2073 6b69 705f 6465 7365 7269 616c 697a   skip_deserializ
-000095b0: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
-000095c0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000095d0: 6c66 2e72 6573 706f 6e73 655f 636c 7328  lf.response_cls(
-000095e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000095f0: 2020 2020 2072 6f75 6e64 5f74 7269 705f       round_trip_
-00009600: 7469 6d65 3d72 6573 706f 6e73 652e 726f  time=response.ro
-00009610: 756e 645f 7472 6970 5f74 696d 652c 0a20  und_trip_time,. 
-00009620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009630: 2020 2072 6573 706f 6e73 653d 7265 7370     response=resp
-00009640: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
-00009650: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00009660: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
-00009670: 795f 6461 7461 2c0a 2020 2020 2020 2020  y_data,.        
-00009680: 2020 2020 2020 2020 2020 2020 6865 6164              head
-00009690: 6572 733d 7265 7370 6f6e 7365 2e68 7474  ers=response.htt
-000096a0: 705f 7265 7370 6f6e 7365 2e68 6561 6465  p_response.heade
-000096b0: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
-000096c0: 2020 2020 2020 2020 7374 6174 7573 3d72          status=r
-000096d0: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
-000096e0: 706f 6e73 652e 7374 6174 7573 0a20 2020  ponse.status.   
-000096f0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00009700: 2020 2020 2020 2020 2020 2020 2320 4578              # Ex
-00009710: 6563 7574 6520 7661 6c69 6461 7469 6f6e  ecute validation
-00009720: 2061 6e64 2074 6872 6f77 2061 7320 6120   and throw as a 
-00009730: 7369 6465 2065 6666 6563 7420 6966 2076  side effect if v
-00009740: 616c 6964 6174 696f 6e20 6661 696c 730a  alidation fails.
-00009750: 2020 2020 2020 2020 2020 2020 626f 6479              body
-00009760: 5f73 6368 656d 612e 6672 6f6d 5f6f 7065  _schema.from_ope
-00009770: 6e61 7069 5f64 6174 615f 6f61 7067 280a  napi_data_oapg(.
-00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 626f 6479 5f64 6174 612c 0a20 2020 2020  body_data,.     
-000097a0: 2020 2020 2020 2020 2020 205f 636f 6e66             _conf
-000097b0: 6967 7572 6174 696f 6e3d 636f 6e66 6967  iguration=config
-000097c0: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-000097d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000097e0: 2020 2320 5661 6c69 6461 7469 6f6e 2070    # Validation p
-000097f0: 6173 7365 642c 2073 6574 2064 6573 6572  assed, set deser
-00009800: 6961 6c69 7a65 645f 626f 6479 2074 6f20  ialized_body to 
-00009810: 706c 6169 6e20 6f6c 6420 6465 7365 7269  plain old deseri
-00009820: 616c 697a 6564 2064 6174 610a 2020 2020  alized data.    
-00009830: 2020 2020 2020 2020 6465 7365 7269 616c          deserial
-00009840: 697a 6564 5f62 6f64 7920 3d20 626f 6479  ized_body = body
-00009850: 5f64 6174 610a 2020 2020 2020 2020 656c  _data.        el
-00009860: 6966 2073 7472 6561 6d65 643a 0a20 2020  if streamed:.   
-00009870: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00009880: 652e 6874 7470 5f72 6573 706f 6e73 652e  e.http_response.
-00009890: 7265 6c65 6173 655f 636f 6e6e 2829 0a0a  release_conn()..
-000098a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000098b0: 656c 662e 7265 7370 6f6e 7365 5f63 6c73  elf.response_cls
-000098c0: 280a 2020 2020 2020 2020 2020 2020 726f  (.            ro
-000098d0: 756e 645f 7472 6970 5f74 696d 653d 7265  und_trip_time=re
-000098e0: 7370 6f6e 7365 2e72 6f75 6e64 5f74 7269  sponse.round_tri
-000098f0: 705f 7469 6d65 2c0a 2020 2020 2020 2020  p_time,.        
-00009900: 2020 2020 7265 7370 6f6e 7365 3d72 6573      response=res
-00009910: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
-00009920: 6e73 652c 0a20 2020 2020 2020 2020 2020  nse,.           
-00009930: 2062 6f64 793d 6465 7365 7269 616c 697a   body=deserializ
-00009940: 6564 5f62 6f64 792c 0a20 2020 2020 2020  ed_body,.       
-00009950: 2020 2020 2068 6561 6465 7273 3d72 6573       headers=res
-00009960: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
-00009970: 6e73 652e 6865 6164 6572 732c 0a20 2020  nse.headers,.   
-00009980: 2020 2020 2020 2020 2073 7461 7475 733d           status=
-00009990: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
-000099a0: 7370 6f6e 7365 2e73 7461 7475 730a 2020  sponse.status.  
-000099b0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-000099c0: 4170 6943 6c69 656e 743a 0a20 2020 2022  ApiClient:.    "
-000099d0: 2222 4765 6e65 7269 6320 4150 4920 636c  ""Generic API cl
-000099e0: 6965 6e74 2066 6f72 204f 7065 6e41 5049  ient for OpenAPI
-000099f0: 2063 6c69 656e 7420 6c69 6272 6172 7920   client library 
-00009a00: 6275 696c 6473 2e0a 0a20 2020 204f 7065  builds...    Ope
-00009a10: 6e41 5049 2067 656e 6572 6963 2041 5049  nAPI generic API
-00009a20: 2063 6c69 656e 742e 2054 6869 7320 636c   client. This cl
-00009a30: 6965 6e74 2068 616e 646c 6573 2074 6865  ient handles the
-00009a40: 2063 6c69 656e 742d 0a20 2020 2073 6572   client-.    ser
-00009a50: 7665 7220 636f 6d6d 756e 6963 6174 696f  ver communicatio
-00009a60: 6e2c 2061 6e64 2069 7320 696e 7661 7269  n, and is invari
-00009a70: 616e 7420 6163 726f 7373 2069 6d70 6c65  ant across imple
-00009a80: 6d65 6e74 6174 696f 6e73 2e20 5370 6563  mentations. Spec
-00009a90: 6966 6963 7320 6f66 0a20 2020 2074 6865  ifics of.    the
-00009aa0: 206d 6574 686f 6473 2061 6e64 206d 6f64   methods and mod
-00009ab0: 656c 7320 666f 7220 6561 6368 2061 7070  els for each app
-00009ac0: 6c69 6361 7469 6f6e 2061 7265 2067 656e  lication are gen
-00009ad0: 6572 6174 6564 2066 726f 6d20 7468 6520  erated from the 
-00009ae0: 4f70 656e 4150 490a 2020 2020 7465 6d70  OpenAPI.    temp
-00009af0: 6c61 7465 732e 0a0a 2020 2020 5468 6973  lates...    This
-00009b00: 2063 6c61 7373 2069 7320 6175 746f 2067   class is auto g
-00009b10: 656e 6572 6174 6564 0a0a 2020 2020 3a70  enerated..    :p
-00009b20: 6172 616d 2063 6f6e 6669 6775 7261 7469  aram configurati
-00009b30: 6f6e 3a20 2e43 6f6e 6669 6775 7261 7469  on: .Configurati
-00009b40: 6f6e 206f 626a 6563 7420 666f 7220 7468  on object for th
-00009b50: 6973 2063 6c69 656e 740a 2020 2020 3a70  is client.    :p
-00009b60: 6172 616d 2068 6561 6465 725f 6e61 6d65  aram header_name
-00009b70: 3a20 6120 6865 6164 6572 2074 6f20 7061  : a header to pa
-00009b80: 7373 2077 6865 6e20 6d61 6b69 6e67 2063  ss when making c
-00009b90: 616c 6c73 2074 6f20 7468 6520 4150 492e  alls to the API.
-00009ba0: 0a20 2020 203a 7061 7261 6d20 6865 6164  .    :param head
-00009bb0: 6572 5f76 616c 7565 3a20 6120 6865 6164  er_value: a head
-00009bc0: 6572 2076 616c 7565 2074 6f20 7061 7373  er value to pass
-00009bd0: 2077 6865 6e20 6d61 6b69 6e67 2063 616c   when making cal
-00009be0: 6c73 2074 6f0a 2020 2020 2020 2020 7468  ls to.        th
-00009bf0: 6520 4150 492e 0a20 2020 203a 7061 7261  e API..    :para
-00009c00: 6d20 636f 6f6b 6965 3a20 6120 636f 6f6b  m cookie: a cook
-00009c10: 6965 2074 6f20 696e 636c 7564 6520 696e  ie to include in
-00009c20: 2074 6865 2068 6561 6465 7220 7768 656e   the header when
-00009c30: 206d 616b 696e 6720 6361 6c6c 730a 2020   making calls.  
-00009c40: 2020 2020 2020 746f 2074 6865 2041 5049        to the API
-00009c50: 0a20 2020 203a 7061 7261 6d20 706f 6f6c  .    :param pool
-00009c60: 5f74 6872 6561 6473 3a20 5468 6520 6e75  _threads: The nu
-00009c70: 6d62 6572 206f 6620 7468 7265 6164 7320  mber of threads 
-00009c80: 746f 2075 7365 2066 6f72 2061 7379 6e63  to use for async
-00009c90: 2072 6571 7565 7374 730a 2020 2020 2020   requests.      
-00009ca0: 2020 746f 2074 6865 2041 5049 2e20 4d6f    to the API. Mo
-00009cb0: 7265 2074 6872 6561 6473 206d 6561 6e73  re threads means
-00009cc0: 206d 6f72 6520 636f 6e63 7572 7265 6e74   more concurrent
-00009cd0: 2041 5049 2072 6571 7565 7374 732e 0a20   API requests.. 
-00009ce0: 2020 2022 2222 0a0a 2020 2020 5f70 6f6f     """..    _poo
-00009cf0: 6c20 3d20 4e6f 6e65 0a0a 2020 2020 6465  l = None..    de
-00009d00: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-00009d10: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-00009d20: 2020 636f 6e66 6967 7572 6174 696f 6e3a    configuration:
-00009d30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00009d40: 5b43 6f6e 6669 6775 7261 7469 6f6e 5d20  [Configuration] 
-00009d50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00009d60: 6865 6164 6572 5f6e 616d 653a 2074 7970  header_name: typ
-00009d70: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00009d80: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00009d90: 2020 6865 6164 6572 5f76 616c 7565 3a20    header_value: 
-00009da0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00009db0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00009dc0: 2020 2020 2063 6f6f 6b69 653a 2074 7970       cookie: typ
-00009dd0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00009de0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-00009df0: 2020 706f 6f6c 5f74 6872 6561 6473 3a20    pool_threads: 
-00009e00: 696e 7420 3d20 310a 2020 2020 293a 0a20  int = 1.    ):. 
-00009e10: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00009e20: 7572 6174 696f 6e20 6973 204e 6f6e 653a  uration is None:
-00009e30: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00009e40: 6669 6775 7261 7469 6f6e 203d 2043 6f6e  figuration = Con
-00009e50: 6669 6775 7261 7469 6f6e 2829 0a20 2020  figuration().   
-00009e60: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-00009e70: 7572 6174 696f 6e20 3d20 636f 6e66 6967  uration = config
-00009e80: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
-00009e90: 7365 6c66 2e70 6f6f 6c5f 7468 7265 6164  self.pool_thread
-00009ea0: 7320 3d20 706f 6f6c 5f74 6872 6561 6473  s = pool_threads
-00009eb0: 0a0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00009ec0: 6573 745f 636c 6965 6e74 203d 2072 6573  est_client = res
-00009ed0: 742e 5245 5354 436c 6965 6e74 4f62 6a65  t.RESTClientObje
-00009ee0: 6374 2863 6f6e 6669 6775 7261 7469 6f6e  ct(configuration
-00009ef0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
-00009f00: 6566 6175 6c74 5f68 6561 6465 7273 203d  efault_headers =
-00009f10: 2048 5454 5048 6561 6465 7244 6963 7428   HTTPHeaderDict(
-00009f20: 290a 2020 2020 2020 2020 6966 2068 6561  ).        if hea
-00009f30: 6465 725f 6e61 6d65 2069 7320 6e6f 7420  der_name is not 
-00009f40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00009f50: 2020 7365 6c66 2e64 6566 6175 6c74 5f68    self.default_h
-00009f60: 6561 6465 7273 5b68 6561 6465 725f 6e61  eaders[header_na
-00009f70: 6d65 5d20 3d20 6865 6164 6572 5f76 616c  me] = header_val
-00009f80: 7565 0a20 2020 2020 2020 2073 656c 662e  ue.        self.
-00009f90: 636f 6f6b 6965 203d 2063 6f6f 6b69 650a  cookie = cookie.
-00009fa0: 2020 2020 2020 2020 2320 5365 7420 6465          # Set de
-00009fb0: 6661 756c 7420 5573 6572 2d41 6765 6e74  fault User-Agent
-00009fc0: 2e0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
-00009fd0: 7365 725f 6167 656e 7420 3d20 274b 6f6e  ser_agent = 'Kon
-00009fe0: 6669 672f 342e 332e 302f 7079 7468 6f6e  fig/4.3.0/python
-00009ff0: 270a 0a20 2020 2064 6566 205f 5f65 6e74  '..    def __ent
-0000a000: 6572 5f5f 2873 656c 6629 3a0a 2020 2020  er__(self):.    
-0000a010: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0000a020: 0a20 2020 2064 6566 205f 5f65 7869 745f  .    def __exit_
-0000a030: 5f28 7365 6c66 2c20 6578 635f 7479 7065  _(self, exc_type
-0000a040: 2c20 6578 635f 7661 6c75 652c 2074 7261  , exc_value, tra
-0000a050: 6365 6261 636b 293a 0a20 2020 2020 2020  ceback):.       
-0000a060: 2073 656c 662e 636c 6f73 6528 290a 0a20   self.close().. 
-0000a070: 2020 2064 6566 2063 6c6f 7365 2873 656c     def close(sel
-0000a080: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-0000a090: 656c 662e 5f70 6f6f 6c3a 0a20 2020 2020  elf._pool:.     
-0000a0a0: 2020 2020 2020 2073 656c 662e 5f70 6f6f         self._poo
-0000a0b0: 6c2e 636c 6f73 6528 290a 2020 2020 2020  l.close().      
-0000a0c0: 2020 2020 2020 7365 6c66 2e5f 706f 6f6c        self._pool
-0000a0d0: 2e6a 6f69 6e28 290a 2020 2020 2020 2020  .join().        
-0000a0e0: 2020 2020 7365 6c66 2e5f 706f 6f6c 203d      self._pool =
-0000a0f0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000a100: 2020 6966 2068 6173 6174 7472 2861 7465    if hasattr(ate
-0000a110: 7869 742c 2027 756e 7265 6769 7374 6572  xit, 'unregister
-0000a120: 2729 3a0a 2020 2020 2020 2020 2020 2020  '):.            
-0000a130: 2020 2020 6174 6578 6974 2e75 6e72 6567      atexit.unreg
-0000a140: 6973 7465 7228 7365 6c66 2e63 6c6f 7365  ister(self.close
-0000a150: 290a 0a20 2020 2040 7072 6f70 6572 7479  )..    @property
-0000a160: 0a20 2020 2064 6566 2070 6f6f 6c28 7365  .    def pool(se
-0000a170: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000a180: 4372 6561 7465 2074 6872 6561 6420 706f  Create thread po
-0000a190: 6f6c 206f 6e20 6669 7273 7420 7265 7175  ol on first requ
-0000a1a0: 6573 740a 2020 2020 2020 2020 2061 766f  est.         avo
-0000a1b0: 6964 7320 696e 7374 616e 7469 6174 696e  ids instantiatin
-0000a1c0: 6720 756e 7573 6564 2074 6872 6561 6470  g unused threadp
-0000a1d0: 6f6f 6c20 666f 7220 626c 6f63 6b69 6e67  ool for blocking
-0000a1e0: 2063 6c69 656e 7473 2e0a 2020 2020 2020   clients..      
-0000a1f0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-0000a200: 2073 656c 662e 5f70 6f6f 6c20 6973 204e   self._pool is N
-0000a210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000a220: 2061 7465 7869 742e 7265 6769 7374 6572   atexit.register
-0000a230: 2873 656c 662e 636c 6f73 6529 0a20 2020  (self.close).   
-0000a240: 2020 2020 2020 2020 2073 656c 662e 5f70           self._p
-0000a250: 6f6f 6c20 3d20 5468 7265 6164 506f 6f6c  ool = ThreadPool
-0000a260: 2873 656c 662e 706f 6f6c 5f74 6872 6561  (self.pool_threa
-0000a270: 6473 290a 2020 2020 2020 2020 7265 7475  ds).        retu
-0000a280: 726e 2073 656c 662e 5f70 6f6f 6c0a 0a20  rn self._pool.. 
-0000a290: 2020 2040 7072 6f70 6572 7479 0a20 2020     @property.   
-0000a2a0: 2064 6566 2075 7365 725f 6167 656e 7428   def user_agent(
-0000a2b0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-0000a2c0: 2222 5573 6572 2061 6765 6e74 2066 6f72  ""User agent for
-0000a2d0: 2074 6869 7320 4150 4920 636c 6965 6e74   this API client
-0000a2e0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-0000a2f0: 726e 2073 656c 662e 6465 6661 756c 745f  rn self.default_
-0000a300: 6865 6164 6572 735b 2755 7365 722d 4167  headers['User-Ag
-0000a310: 656e 7427 5d0a 0a20 2020 2040 7573 6572  ent']..    @user
-0000a320: 5f61 6765 6e74 2e73 6574 7465 720a 2020  _agent.setter.  
-0000a330: 2020 6465 6620 7573 6572 5f61 6765 6e74    def user_agent
-0000a340: 2873 656c 662c 2076 616c 7565 293a 0a20  (self, value):. 
-0000a350: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
-0000a360: 756c 745f 6865 6164 6572 735b 2755 7365  ult_headers['Use
-0000a370: 722d 4167 656e 7427 5d20 3d20 7661 6c75  r-Agent'] = valu
-0000a380: 650a 0a20 2020 2064 6566 2073 6574 5f64  e..    def set_d
-0000a390: 6566 6175 6c74 5f68 6561 6465 7228 7365  efault_header(se
-0000a3a0: 6c66 2c20 6865 6164 6572 5f6e 616d 652c  lf, header_name,
-0000a3b0: 2068 6561 6465 725f 7661 6c75 6529 3a0a   header_value):.
-0000a3c0: 2020 2020 2020 2020 7365 6c66 2e64 6566          self.def
-0000a3d0: 6175 6c74 5f68 6561 6465 7273 5b68 6561  ault_headers[hea
-0000a3e0: 6465 725f 6e61 6d65 5d20 3d20 6865 6164  der_name] = head
-0000a3f0: 6572 5f76 616c 7565 0a0a 2020 2020 6465  er_value..    de
-0000a400: 6620 5f5f 6361 6c6c 5f61 7069 280a 2020  f __call_api(.  
-0000a410: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000a420: 2020 2020 7265 736f 7572 6365 5f70 6174      resource_pat
-0000a430: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-0000a440: 6d65 7468 6f64 3a20 7374 722c 0a20 2020  method: str,.   
-0000a450: 2020 2020 2068 6561 6465 7273 3a20 7479       headers: ty
-0000a460: 7069 6e67 2e4f 7074 696f 6e61 6c5b 4854  ping.Optional[HT
-0000a470: 5450 4865 6164 6572 4469 6374 5d20 3d20  TPHeaderDict] = 
-0000a480: 4e6f 6e65 2c0a 2020 2020 2020 2020 7365  None,.        se
-0000a490: 7269 616c 697a 6564 5f62 6f64 793a 2074  rialized_body: t
-0000a4a0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0000a4b0: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
-0000a4c0: 2062 7974 6573 5d5d 203d 204e 6f6e 652c   bytes]] = None,
-0000a4d0: 0a20 2020 2020 2020 2062 6f64 793a 2074  .        body: t
-0000a4e0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
-0000a4f0: 2c0a 2020 2020 2020 2020 6669 656c 6473  ,.        fields
-0000a500: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000a510: 6c5b 7479 7069 6e67 2e54 7570 6c65 5b74  l[typing.Tuple[t
-0000a520: 7970 696e 672e 5475 706c 655b 7374 722c  yping.Tuple[str,
-0000a530: 2073 7472 5d2c 202e 2e2e 5d5d 203d 204e   str], ...]] = N
-0000a540: 6f6e 652c 0a20 2020 2020 2020 2061 7574  one,.        aut
-0000a550: 685f 7365 7474 696e 6773 3a20 7479 7069  h_settings: typi
-0000a560: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0000a570: 6e67 2e4c 6973 745b 7374 725d 5d20 3d20  ng.List[str]] = 
-0000a580: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-0000a590: 7265 616d 3a20 626f 6f6c 203d 2046 616c  ream: bool = Fal
-0000a5a0: 7365 2c0a 2020 2020 2020 2020 7469 6d65  se,.        time
-0000a5b0: 6f75 743a 2074 7970 696e 672e 4f70 7469  out: typing.Opti
-0000a5c0: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
-0000a5d0: 6e5b 696e 742c 2074 7970 696e 672e 5475  n[int, typing.Tu
-0000a5e0: 706c 655d 5d20 3d20 4e6f 6e65 2c0a 2020  ple]] = None,.  
-0000a5f0: 2020 2020 2020 686f 7374 3a20 7479 7069        host: typi
-0000a600: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
-0000a610: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000a620: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
-0000a630: 725f 6974 6572 6174 6f72 3a20 5072 6566  r_iterator: Pref
-0000a640: 6978 5365 7061 7261 746f 7249 7465 7261  ixSeparatorItera
-0000a650: 746f 7220 3d20 4e6f 6e65 2c0a 2020 2020  tor = None,.    
-0000a660: 2920 2d3e 2052 6573 706f 6e73 6557 7261  ) -> ResponseWra
-0000a670: 7070 6572 3a0a 0a20 2020 2020 2020 2072  pper:..        r
-0000a680: 6571 7565 7374 5f62 6566 6f72 655f 686f  equest_before_ho
-0000a690: 6f6b 280a 2020 2020 2020 2020 2020 2020  ok(.            
-0000a6a0: 7265 736f 7572 6365 5f70 6174 683d 7265  resource_path=re
-0000a6b0: 736f 7572 6365 5f70 6174 682c 0a20 2020  source_path,.   
-0000a6c0: 2020 2020 2020 2020 206d 6574 686f 643d           method=
-0000a6d0: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
-0000a6e0: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
-0000a6f0: 6e3d 7365 6c66 2e63 6f6e 6669 6775 7261  n=self.configura
-0000a700: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
-0000a710: 2020 626f 6479 3d62 6f64 792c 0a20 2020    body=body,.   
-0000a720: 2020 2020 2020 2020 2066 6965 6c64 733d           fields=
-0000a730: 6669 656c 6473 2c0a 2020 2020 2020 2020  fields,.        
-0000a740: 2020 2020 6175 7468 5f73 6574 7469 6e67      auth_setting
-0000a750: 733d 6175 7468 5f73 6574 7469 6e67 732c  s=auth_settings,
-0000a760: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
-0000a770: 6465 7273 3d68 6561 6465 7273 2c0a 2020  ders=headers,.  
-0000a780: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000a790: 2023 2068 6561 6465 7220 7061 7261 6d65   # header parame
-0000a7a0: 7465 7273 0a20 2020 2020 2020 2075 7365  ters.        use
-0000a7b0: 645f 6865 6164 6572 7320 3d20 4854 5450  d_headers = HTTP
-0000a7c0: 4865 6164 6572 4469 6374 2873 656c 662e  HeaderDict(self.
-0000a7d0: 6465 6661 756c 745f 6865 6164 6572 7329  default_headers)
-0000a7e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000a7f0: 2e63 6f6f 6b69 653a 0a20 2020 2020 2020  .cookie:.       
-0000a800: 2020 2020 2068 6561 6465 7273 5b27 436f       headers['Co
-0000a810: 6f6b 6965 275d 203d 2073 656c 662e 636f  okie'] = self.co
-0000a820: 6f6b 6965 0a0a 2020 2020 2020 2020 2320  okie..        # 
-0000a830: 6175 7468 2073 6574 7469 6e67 0a20 2020  auth setting.   
-0000a840: 2020 2020 2072 6573 6f75 7263 655f 7061       resource_pa
-0000a850: 7468 203d 2073 656c 662e 7570 6461 7465  th = self.update
-0000a860: 5f70 6172 616d 735f 666f 725f 6175 7468  _params_for_auth
-0000a870: 280a 2020 2020 2020 2020 2020 2020 7573  (.            us
-0000a880: 6564 5f68 6561 6465 7273 2c0a 2020 2020  ed_headers,.    
-0000a890: 2020 2020 2020 2020 6175 7468 5f73 6574          auth_set
-0000a8a0: 7469 6e67 732c 0a20 2020 2020 2020 2020  tings,.         
-0000a8b0: 2020 2072 6573 6f75 7263 655f 7061 7468     resource_path
-0000a8c0: 2c0a 2020 2020 2020 2020 2020 2020 6d65  ,.            me
-0000a8d0: 7468 6f64 2c0a 2020 2020 2020 2020 2020  thod,.          
-0000a8e0: 2020 626f 6479 2c0a 2020 2020 2020 2020    body,.        
-0000a8f0: 2020 2020 7072 6566 6978 5f73 6570 6172      prefix_separ
-0000a900: 6174 6f72 5f69 7465 7261 746f 720a 2020  ator_iterator.  
-0000a910: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000a920: 2023 206d 7573 7420 6861 7070 656e 2061   # must happen a
-0000a930: 6674 6572 2063 6f6f 6b69 6520 7365 7474  fter cookie sett
-0000a940: 696e 6720 616e 6420 6175 7468 2073 6574  ing and auth set
-0000a950: 7469 6e67 2069 6e20 6361 7365 2075 7365  ting in case use
-0000a960: 7220 6973 206f 7665 7272 6964 696e 6720  r is overriding 
-0000a970: 7468 6f73 650a 2020 2020 2020 2020 6966  those.        if
-0000a980: 2068 6561 6465 7273 3a0a 2020 2020 2020   headers:.      
-0000a990: 2020 2020 2020 7573 6564 5f68 6561 6465        used_heade
-0000a9a0: 7273 2e75 7064 6174 6528 6865 6164 6572  rs.update(header
-0000a9b0: 7329 0a0a 2020 2020 2020 2020 2320 7265  s)..        # re
-0000a9c0: 7175 6573 7420 7572 6c0a 2020 2020 2020  quest url.      
-0000a9d0: 2020 6966 2068 6f73 7420 6973 204e 6f6e    if host is Non
-0000a9e0: 653a 0a20 2020 2020 2020 2020 2020 2075  e:.            u
-0000a9f0: 726c 203d 2073 656c 662e 636f 6e66 6967  rl = self.config
-0000aa00: 7572 6174 696f 6e2e 686f 7374 202b 2072  uration.host + r
-0000aa10: 6573 6f75 7263 655f 7061 7468 0a20 2020  esource_path.   
-0000aa20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000aa30: 2020 2020 2020 2023 2075 7365 2073 6572         # use ser
-0000aa40: 7665 722f 686f 7374 2064 6566 696e 6564  ver/host defined
-0000aa50: 2069 6e20 7061 7468 206f 7220 6f70 6572   in path or oper
-0000aa60: 6174 696f 6e20 696e 7374 6561 640a 2020  ation instead.  
-0000aa70: 2020 2020 2020 2020 2020 7572 6c20 3d20            url = 
-0000aa80: 686f 7374 202b 2072 6573 6f75 7263 655f  host + resource_
-0000aa90: 7061 7468 0a0a 2020 2020 2020 2020 7265  path..        re
-0000aaa0: 7175 6573 745f 6166 7465 725f 686f 6f6b  quest_after_hook
-0000aab0: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-0000aac0: 736f 7572 6365 5f70 6174 683d 7265 736f  source_path=reso
-0000aad0: 7572 6365 5f70 6174 682c 0a20 2020 2020  urce_path,.     
-0000aae0: 2020 2020 2020 206d 6574 686f 643d 6d65         method=me
-0000aaf0: 7468 6f64 2c0a 2020 2020 2020 2020 2020  thod,.          
-0000ab00: 2020 636f 6e66 6967 7572 6174 696f 6e3d    configuration=
-0000ab10: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
-0000ab20: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-0000ab30: 626f 6479 3d62 6f64 792c 0a20 2020 2020  body=body,.     
-0000ab40: 2020 2020 2020 2066 6965 6c64 733d 6669         fields=fi
-0000ab50: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
-0000ab60: 2020 6175 7468 5f73 6574 7469 6e67 733d    auth_settings=
-0000ab70: 6175 7468 5f73 6574 7469 6e67 732c 0a20  auth_settings,. 
-0000ab80: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-0000ab90: 7273 3d75 7365 645f 6865 6164 6572 732c  rs=used_headers,
-0000aba0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000abb0: 2020 2020 2320 7065 7266 6f72 6d20 7265      # perform re
-0000abc0: 7175 6573 7420 616e 6420 7265 7475 726e  quest and return
-0000abd0: 2072 6573 706f 6e73 650a 2020 2020 2020   response.      
-0000abe0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-0000abf0: 662e 7265 7175 6573 7428 0a20 2020 2020  f.request(.     
-0000ac00: 2020 2020 2020 206d 6574 686f 642c 0a20         method,. 
-0000ac10: 2020 2020 2020 2020 2020 2075 726c 2c0a             url,.
-0000ac20: 2020 2020 2020 2020 2020 2020 6865 6164              head
-0000ac30: 6572 733d 7573 6564 5f68 6561 6465 7273  ers=used_headers
-0000ac40: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-0000ac50: 656c 6473 3d66 6965 6c64 732c 0a20 2020  elds=fields,.   
-0000ac60: 2020 2020 2020 2020 2062 6f64 793d 7365           body=se
-0000ac70: 7269 616c 697a 6564 5f62 6f64 792c 0a20  rialized_body,. 
-0000ac80: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-0000ac90: 6d3d 7374 7265 616d 2c0a 2020 2020 2020  m=stream,.      
-0000aca0: 2020 2020 2020 7469 6d65 6f75 743d 7469        timeout=ti
-0000acb0: 6d65 6f75 742c 0a20 2020 2020 2020 2029  meout,.        )
-0000acc0: 0a0a 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0000acd0: 6e20 7265 7370 6f6e 7365 0a0a 2020 2020  n response..    
-0000ace0: 6465 6620 6361 6c6c 5f61 7069 280a 2020  def call_api(.  
-0000acf0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000ad00: 2020 2020 7265 736f 7572 6365 5f70 6174      resource_pat
-0000ad10: 683a 2073 7472 2c0a 2020 2020 2020 2020  h: str,.        
-0000ad20: 6d65 7468 6f64 3a20 7374 722c 0a20 2020  method: str,.   
-0000ad30: 2020 2020 2068 6561 6465 7273 3a20 7479       headers: ty
-0000ad40: 7069 6e67 2e4f 7074 696f 6e61 6c5b 4854  ping.Optional[HT
-0000ad50: 5450 4865 6164 6572 4469 6374 5d20 3d20  TPHeaderDict] = 
-0000ad60: 4e6f 6e65 2c0a 2020 2020 2020 2020 7365  None,.        se
-0000ad70: 7269 616c 697a 6564 5f62 6f64 793a 2074  rialized_body: t
-0000ad80: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-0000ad90: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
-0000ada0: 2062 7974 6573 5d5d 203d 204e 6f6e 652c   bytes]] = None,
-0000adb0: 0a20 2020 2020 2020 2062 6f64 793a 2074  .        body: t
-0000adc0: 7970 696e 672e 416e 7920 3d20 4e6f 6e65  yping.Any = None
-0000add0: 2c0a 2020 2020 2020 2020 6669 656c 6473  ,.        fields
-0000ade0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-0000adf0: 6c5b 7479 7069 6e67 2e54 7570 6c65 5b74  l[typing.Tuple[t
-0000ae00: 7970 696e 672e 5475 706c 655b 7374 722c  yping.Tuple[str,
-0000ae10: 2073 7472 5d2c 202e 2e2e 5d5d 203d 204e   str], ...]] = N
-0000ae20: 6f6e 652c 0a20 2020 2020 2020 2061 7574  one,.        aut
-0000ae30: 685f 7365 7474 696e 6773 3a20 7479 7069  h_settings: typi
-0000ae40: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
-0000ae50: 6e67 2e4c 6973 745b 7374 725d 5d20 3d20  ng.List[str]] = 
-0000ae60: 4e6f 6e65 2c0a 2020 2020 2020 2020 6173  None,.        as
-0000ae70: 796e 635f 7265 713a 2074 7970 696e 672e  ync_req: typing.
-0000ae80: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
-0000ae90: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-0000aea0: 7472 6561 6d3a 2062 6f6f 6c20 3d20 4661  tream: bool = Fa
-0000aeb0: 6c73 652c 0a20 2020 2020 2020 2074 696d  lse,.        tim
-0000aec0: 656f 7574 3a20 7479 7069 6e67 2e4f 7074  eout: typing.Opt
-0000aed0: 696f 6e61 6c5b 7479 7069 6e67 2e55 6e69  ional[typing.Uni
-0000aee0: 6f6e 5b69 6e74 2c20 7479 7069 6e67 2e54  on[int, typing.T
-0000aef0: 7570 6c65 5d5d 203d 204e 6f6e 652c 0a20  uple]] = None,. 
-0000af00: 2020 2020 2020 2068 6f73 743a 2074 7970         host: typ
-0000af10: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-0000af20: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000af30: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
-0000af40: 6f72 5f69 7465 7261 746f 723a 2050 7265  or_iterator: Pre
-0000af50: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
-0000af60: 6174 6f72 203d 204e 6f6e 652c 0a20 2020  ator = None,.   
-0000af70: 2029 202d 3e20 5265 7370 6f6e 7365 5772   ) -> ResponseWr
-0000af80: 6170 7065 723a 0a20 2020 2020 2020 2022  apper:.        "
-0000af90: 2222 4d61 6b65 7320 7468 6520 4854 5450  ""Makes the HTTP
-0000afa0: 2072 6571 7565 7374 2028 7379 6e63 6872   request (synchr
-0000afb0: 6f6e 6f75 7329 2061 6e64 2072 6574 7572  onous) and retur
-0000afc0: 6e73 2064 6573 6572 6961 6c69 7a65 6420  ns deserialized 
-0000afd0: 6461 7461 2e0a 0a20 2020 2020 2020 2054  data...        T
-0000afe0: 6f20 6d61 6b65 2061 6e20 6173 796e 635f  o make an async_
-0000aff0: 7265 7120 7265 7175 6573 742c 2073 6574  req request, set
-0000b000: 2074 6865 2061 7379 6e63 5f72 6571 2070   the async_req p
-0000b010: 6172 616d 6574 6572 2e0a 0a20 2020 2020  arameter...     
-0000b020: 2020 203a 7061 7261 6d20 7265 736f 7572     :param resour
-0000b030: 6365 5f70 6174 683a 2050 6174 6820 746f  ce_path: Path to
-0000b040: 206d 6574 686f 6420 656e 6470 6f69 6e74   method endpoint
-0000b050: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-0000b060: 206d 6574 686f 643a 204d 6574 686f 6420   method: Method 
-0000b070: 746f 2063 616c 6c2e 0a20 2020 2020 2020  to call..       
-0000b080: 203a 7061 7261 6d20 6865 6164 6572 733a   :param headers:
-0000b090: 2048 6561 6465 7220 7061 7261 6d65 7465   Header paramete
-0000b0a0: 7273 2074 6f20 6265 0a20 2020 2020 2020  rs to be.       
-0000b0b0: 2020 2020 2070 6c61 6365 6420 696e 2074       placed in t
-0000b0c0: 6865 2072 6571 7565 7374 2068 6561 6465  he request heade
-0000b0d0: 722e 0a20 2020 2020 2020 203a 7061 7261  r..        :para
-0000b0e0: 6d20 626f 6479 3a20 5265 7175 6573 7420  m body: Request 
-0000b0f0: 626f 6479 2e0a 2020 2020 2020 2020 3a70  body..        :p
-0000b100: 6172 616d 2066 6965 6c64 733a 2052 6571  aram fields: Req
-0000b110: 7565 7374 2070 6f73 7420 666f 726d 2070  uest post form p
-0000b120: 6172 616d 6574 6572 732c 0a20 2020 2020  arameters,.     
-0000b130: 2020 2020 2020 2066 6f72 2060 6170 706c         for `appl
-0000b140: 6963 6174 696f 6e2f 782d 7777 772d 666f  ication/x-www-fo
-0000b150: 726d 2d75 726c 656e 636f 6465 6460 2c20  rm-urlencoded`, 
-0000b160: 606d 756c 7469 7061 7274 2f66 6f72 6d2d  `multipart/form-
-0000b170: 6461 7461 602e 0a20 2020 2020 2020 203a  data`..        :
-0000b180: 7061 7261 6d20 6175 7468 5f73 6574 7469  param auth_setti
-0000b190: 6e67 733a 2041 7574 6820 5365 7474 696e  ngs: Auth Settin
-0000b1a0: 6773 206e 616d 6573 2066 6f72 2074 6865  gs names for the
-0000b1b0: 2072 6571 7565 7374 2e0a 2020 2020 2020   request..      
-0000b1c0: 2020 3a70 6172 616d 2061 7379 6e63 5f72    :param async_r
-0000b1d0: 6571 3a20 6578 6563 7574 6520 7265 7175  eq: execute requ
-0000b1e0: 6573 7420 6173 796e 6368 726f 6e6f 7573  est asynchronous
-0000b1f0: 6c79 0a20 2020 2020 2020 203a 7479 7065  ly.        :type
-0000b200: 2061 7379 6e63 5f72 6571 3a20 626f 6f6c   async_req: bool
-0000b210: 2c20 6f70 7469 6f6e 616c 2054 4f44 4f20  , optional TODO 
-0000b220: 7265 6d6f 7665 2c20 756e 7573 6564 0a20  remove, unused. 
-0000b230: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-0000b240: 7265 616d 3a20 6966 2054 7275 652c 2074  ream: if True, t
-0000b250: 6865 2075 726c 6c69 6233 2e48 5454 5052  he urllib3.HTTPR
-0000b260: 6573 706f 6e73 6520 6f62 6a65 6374 2077  esponse object w
-0000b270: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
-0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 2020 2020 2062 6520 7265 7475 726e 6564       be returned
-0000b2a0: 2077 6974 686f 7574 2072 6561 6469 6e67   without reading
-0000b2b0: 2f64 6563 6f64 696e 6720 7265 7370 6f6e  /decoding respon
-0000b2c0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 2020 6461 7461 2e20 416c 736f 2077      data. Also w
-0000b2f0: 6865 6e20 5472 7565 2c20 6966 2074 6865  hen True, if the
-0000b300: 206f 7065 6e61 7069 2073 7065 6320 6465   openapi spec de
-0000b310: 7363 7269 6265 7320 6120 6669 6c65 2064  scribes a file d
-0000b320: 6f77 6e6c 6f61 642c 0a20 2020 2020 2020  ownload,.       
-0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b340: 2020 2020 2020 2020 2020 7468 6520 6461            the da
-0000b350: 7461 2077 696c 6c20 6265 2077 7269 7474  ta will be writt
-0000b360: 656e 2074 6f20 6120 6c6f 6361 6c20 6669  en to a local fi
-0000b370: 6c65 7379 7374 6d65 2066 696c 6520 616e  lesystme file an
-0000b380: 6420 7468 6520 4269 6e61 7279 5363 6865  d the BinarySche
-0000b390: 6d61 0a20 2020 2020 2020 2020 2020 2020  ma.             
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 2020 696e 7374 616e 6365 2077 696c      instance wil
-0000b3c0: 6c20 616c 736f 2069 6e68 6572 6974 2066  l also inherit f
-0000b3d0: 726f 6d20 4669 6c65 5363 6865 6d61 2061  rom FileSchema a
-0000b3e0: 6e64 2046 696c 6549 4f0a 2020 2020 2020  nd FileIO.      
-0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b400: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-0000b410: 6c74 2069 7320 4661 6c73 652e 0a20 2020  lt is False..   
-0000b420: 2020 2020 203a 7479 7065 2073 7472 6561       :type strea
-0000b430: 6d3a 2062 6f6f 6c2c 206f 7074 696f 6e61  m: bool, optiona
-0000b440: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
-0000b450: 2074 696d 656f 7574 3a20 7469 6d65 6f75   timeout: timeou
-0000b460: 7420 7365 7474 696e 6720 666f 7220 7468  t setting for th
-0000b470: 6973 2072 6571 7565 7374 2e20 4966 206f  is request. If o
-0000b480: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4a0: 2020 2020 6e75 6d62 6572 2070 726f 7669      number provi
-0000b4b0: 6465 642c 2069 7420 7769 6c6c 2062 6520  ded, it will be 
-0000b4c0: 746f 7461 6c20 7265 7175 6573 740a 2020  total request.  
-0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000b4f0: 696d 656f 7574 2e20 4974 2063 616e 2061  imeout. It can a
-0000b500: 6c73 6f20 6265 2061 2070 6169 7220 2874  lso be a pair (t
-0000b510: 7570 6c65 2920 6f66 0a20 2020 2020 2020  uple) of.       
-0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b530: 2020 2020 2020 2020 2020 2863 6f6e 6e65            (conne
-0000b540: 6374 696f 6e2c 2072 6561 6429 2074 696d  ction, read) tim
-0000b550: 656f 7574 732e 0a20 2020 2020 2020 203a  eouts..        :
-0000b560: 7061 7261 6d20 686f 7374 3a20 6170 6920  param host: api 
-0000b570: 656e 6470 6f69 6e74 2068 6f73 740a 2020  endpoint host.  
-0000b580: 2020 2020 2020 3a72 6574 7572 6e3a 0a20        :return:. 
-0000b590: 2020 2020 2020 2020 2020 2049 6620 6173             If as
-0000b5a0: 796e 635f 7265 7120 7061 7261 6d65 7465  ync_req paramete
-0000b5b0: 7220 6973 2054 7275 652c 0a20 2020 2020  r is True,.     
-0000b5c0: 2020 2020 2020 2074 6865 2072 6571 7565         the reque
-0000b5d0: 7374 2077 696c 6c20 6265 2063 616c 6c65  st will be calle
-0000b5e0: 6420 6173 796e 6368 726f 6e6f 7573 6c79  d asynchronously
-0000b5f0: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-0000b600: 6520 6d65 7468 6f64 2077 696c 6c20 7265  e method will re
-0000b610: 7475 726e 2074 6865 2072 6571 7565 7374  turn the request
-0000b620: 2074 6872 6561 642e 0a20 2020 2020 2020   thread..       
-0000b630: 2020 2020 2049 6620 7061 7261 6d65 7465       If paramete
-0000b640: 7220 6173 796e 635f 7265 7120 6973 2046  r async_req is F
-0000b650: 616c 7365 206f 7220 6d69 7373 696e 672c  alse or missing,
-0000b660: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-0000b670: 6e20 7468 6520 6d65 7468 6f64 2077 696c  n the method wil
-0000b680: 6c20 7265 7475 726e 2074 6865 2072 6573  l return the res
-0000b690: 706f 6e73 6520 6469 7265 6374 6c79 2e0a  ponse directly..
-0000b6a0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000b6b0: 2020 2020 2069 6620 6e6f 7420 6173 796e       if not asyn
-0000b6c0: 635f 7265 713a 0a20 2020 2020 2020 2020  c_req:.         
-0000b6d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000b6e0: 5f63 616c 6c5f 6170 6928 0a20 2020 2020  _call_api(.     
-0000b6f0: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-0000b700: 7263 655f 7061 7468 2c0a 2020 2020 2020  rce_path,.      
-0000b710: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-0000b720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b730: 2020 6865 6164 6572 732c 0a20 2020 2020    headers,.     
-0000b740: 2020 2020 2020 2020 2020 2073 6572 6961             seria
-0000b750: 6c69 7a65 645f 626f 6479 2c0a 2020 2020  lized_body,.    
-0000b760: 2020 2020 2020 2020 2020 2020 626f 6479              body
-0000b770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b780: 2020 6669 656c 6473 2c0a 2020 2020 2020    fields,.      
-0000b790: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
-0000b7a0: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
-0000b7b0: 2020 2020 2020 2020 2073 7472 6561 6d2c           stream,
-0000b7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b7d0: 2074 696d 656f 7574 2c0a 2020 2020 2020   timeout,.      
-0000b7e0: 2020 2020 2020 2020 2020 686f 7374 2c0a            host,.
-0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b800: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
-0000b810: 5f69 7465 7261 746f 722c 0a20 2020 2020  _iterator,.     
-0000b820: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000b830: 2020 7265 7475 726e 2073 656c 662e 706f    return self.po
-0000b840: 6f6c 2e61 7070 6c79 5f61 7379 6e63 280a  ol.apply_async(.
-0000b850: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b860: 2e5f 5f63 616c 6c5f 6170 692c 0a20 2020  .__call_api,.   
-0000b870: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-0000b880: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-0000b890: 7263 655f 7061 7468 2c0a 2020 2020 2020  rce_path,.      
-0000b8a0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-0000b8b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b8c0: 2020 6865 6164 6572 732c 0a20 2020 2020    headers,.     
-0000b8d0: 2020 2020 2020 2020 2020 2073 6572 6961             seria
-0000b8e0: 6c69 7a65 645f 626f 6479 2c0a 2020 2020  lized_body,.    
-0000b8f0: 2020 2020 2020 2020 2020 2020 626f 6479              body
-0000b900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b910: 2020 6a73 6f6e 2c0a 2020 2020 2020 2020    json,.        
-0000b920: 2020 2020 2020 2020 6669 656c 6473 2c0a          fields,.
-0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b940: 6175 7468 5f73 6574 7469 6e67 732c 0a20  auth_settings,. 
-0000b950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000b960: 7472 6561 6d2c 0a20 2020 2020 2020 2020  tream,.         
-0000b970: 2020 2020 2020 2074 696d 656f 7574 2c0a         timeout,.
-0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b990: 686f 7374 2c0a 2020 2020 2020 2020 2020  host,.          
-0000b9a0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-0000b9b0: 6172 6174 6f72 5f69 7465 7261 746f 722c  arator_iterator,
-0000b9c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000b9d0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0000b9e0: 6620 7265 7175 6573 7428 0a20 2020 2020  f request(.     
-0000b9f0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000ba00: 206d 6574 686f 643a 2073 7472 2c0a 2020   method: str,.  
-0000ba10: 2020 2020 2020 7572 6c3a 2073 7472 2c0a        url: str,.
-0000ba20: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0000ba30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0000ba40: 5b48 5454 5048 6561 6465 7244 6963 745d  [HTTPHeaderDict]
-0000ba50: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0000ba60: 2066 6965 6c64 733a 2074 7970 696e 672e   fields: typing.
-0000ba70: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
-0000ba80: 5475 706c 655b 7479 7069 6e67 2e54 7570  Tuple[typing.Tup
-0000ba90: 6c65 5b73 7472 2c20 7374 725d 2c20 2e2e  le[str, str], ..
-0000baa0: 2e5d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  .]] = None,.    
-0000bab0: 2020 2020 626f 6479 3a20 7479 7069 6e67      body: typing
-0000bac0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-0000bad0: 2e55 6e69 6f6e 5b73 7472 2c20 6279 7465  .Union[str, byte
-0000bae0: 735d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  s]] = None,.    
-0000baf0: 2020 2020 7374 7265 616d 3a20 626f 6f6c      stream: bool
-0000bb00: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000bb10: 2020 7469 6d65 6f75 743a 2074 7970 696e    timeout: typin
-0000bb20: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-0000bb30: 672e 556e 696f 6e5b 696e 742c 2074 7970  g.Union[int, typ
-0000bb40: 696e 672e 5475 706c 655d 5d20 3d20 4e6f  ing.Tuple]] = No
-0000bb50: 6e65 2c0a 2020 2020 2920 2d3e 2052 6573  ne,.    ) -> Res
-0000bb60: 706f 6e73 6557 7261 7070 6572 3a0a 2020  ponseWrapper:.  
-0000bb70: 2020 2020 2020 2222 224d 616b 6573 2074        """Makes t
-0000bb80: 6865 2048 5454 5020 7265 7175 6573 7420  he HTTP request 
-0000bb90: 7573 696e 6720 5245 5354 436c 6965 6e74  using RESTClient
-0000bba0: 2e22 2222 0a20 2020 2020 2020 2069 6620  .""".        if 
-0000bbb0: 6d65 7468 6f64 203d 3d20 2247 4554 223a  method == "GET":
-0000bbc0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0000bbd0: 7572 6e20 7365 6c66 2e72 6573 745f 636c  urn self.rest_cl
-0000bbe0: 6965 6e74 2e47 4554 2875 726c 2c0a 2020  ient.GET(url,.  
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc10: 2020 2020 2020 7374 7265 616d 3d73 7472        stream=str
-0000bc20: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-0000bc50: 656f 7574 3d74 696d 656f 7574 2c0a 2020  eout=timeout,.  
-0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc80: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
-0000bc90: 6164 6572 7329 0a20 2020 2020 2020 2065  aders).        e
-0000bca0: 6c69 6620 6d65 7468 6f64 203d 3d20 2248  lif method == "H
-0000bcb0: 4541 4422 3a0a 2020 2020 2020 2020 2020  EAD":.          
-0000bcc0: 2020 7265 7475 726e 2073 656c 662e 7265    return self.re
-0000bcd0: 7374 5f63 6c69 656e 742e 4845 4144 2875  st_client.HEAD(u
-0000bce0: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
-0000bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd00: 2020 2020 2020 2020 2020 2020 2073 7472               str
-0000bd10: 6561 6d3d 7374 7265 616d 2c0a 2020 2020  eam=stream,.    
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd40: 2020 2020 2074 696d 656f 7574 3d74 696d       timeout=tim
-0000bd50: 656f 7574 2c0a 2020 2020 2020 2020 2020  eout,.          
-0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000bd80: 6561 6465 7273 3d68 6561 6465 7273 290a  eaders=headers).
-0000bd90: 2020 2020 2020 2020 656c 6966 206d 6574          elif met
-0000bda0: 686f 6420 3d3d 2022 4f50 5449 4f4e 5322  hod == "OPTIONS"
-0000bdb0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000bdc0: 7475 726e 2073 656c 662e 7265 7374 5f63  turn self.rest_c
-0000bdd0: 6c69 656e 742e 4f50 5449 4f4e 5328 7572  lient.OPTIONS(ur
-0000bde0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be00: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000be10: 6561 6465 7273 3d68 6561 6465 7273 2c0a  eaders=headers,.
-0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be40: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
-0000be50: 6473 3d66 6965 6c64 732c 0a20 2020 2020  ds=fields,.     
-0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2020 2020 2020 2073 7472 6561 6d3d 7374         stream=st
-0000be90: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
-0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
-0000bed0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000bf00: 6f64 793d 626f 6479 290a 2020 2020 2020  ody=body).      
-0000bf10: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
-0000bf20: 2022 504f 5354 223a 0a20 2020 2020 2020   "POST":.       
-0000bf30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000bf40: 2e72 6573 745f 636c 6965 6e74 2e50 4f53  .rest_client.POS
-0000bf50: 5428 7572 6c2c 0a20 2020 2020 2020 2020  T(url,.         
-0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf80: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
-0000bf90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2020 2020 2020 2020 2020 6669 656c 6473            fields
-0000bfc0: 3d66 6965 6c64 732c 0a20 2020 2020 2020  =fields,.       
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bff0: 2020 7374 7265 616d 3d73 7472 6561 6d2c    stream=stream,
-0000c000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c020: 2020 2020 2020 2020 2020 7469 6d65 6f75            timeou
-0000c030: 743d 7469 6d65 6f75 742c 0a20 2020 2020  t=timeout,.     
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2020 2020 626f 6479 3d62 6f64 7929 0a20      body=body). 
-0000c070: 2020 2020 2020 2065 6c69 6620 6d65 7468         elif meth
-0000c080: 6f64 203d 3d20 2250 5554 223a 0a20 2020  od == "PUT":.   
-0000c090: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c0a0: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
-0000c0b0: 2e50 5554 2875 726c 2c0a 2020 2020 2020  .PUT(url,.      
-0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0e0: 2020 6865 6164 6572 733d 6865 6164 6572    headers=header
-0000c0f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c110: 2020 2020 2020 2020 2020 2066 6965 6c64             field
-0000c120: 733d 6669 656c 6473 2c0a 2020 2020 2020  s=fields,.      
-0000c130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 7374 7265 616d 3d73 7472 6561 6d2c    stream=stream,
-0000c160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c180: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
-0000c190: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
-0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1c0: 2020 626f 6479 3d62 6f64 7929 0a20 2020    body=body).   
-0000c1d0: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
-0000c1e0: 203d 3d20 2250 4154 4348 223a 0a20 2020   == "PATCH":.   
-0000c1f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c200: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
-0000c210: 2e50 4154 4348 2875 726c 2c0a 2020 2020  .PATCH(url,.    
-0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c240: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
-0000c250: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
-0000c260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c280: 2066 6965 6c64 733d 6669 656c 6473 2c0a   fields=fields,.
-0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2b0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-0000c2c0: 3d73 7472 6561 6d2c 0a20 2020 2020 2020  =stream,.       
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2f0: 2020 2074 696d 656f 7574 3d74 696d 656f     timeout=timeo
-0000c300: 7574 2c0a 2020 2020 2020 2020 2020 2020  ut,.            
-0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c320: 2020 2020 2020 2020 2020 2020 2020 626f                bo
-0000c330: 6479 3d62 6f64 7929 0a20 2020 2020 2020  dy=body).       
-0000c340: 2065 6c69 6620 6d65 7468 6f64 203d 3d20   elif method == 
-0000c350: 2244 454c 4554 4522 3a0a 2020 2020 2020  "DELETE":.      
-0000c360: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000c370: 662e 7265 7374 5f63 6c69 656e 742e 4445  f.rest_client.DE
-0000c380: 4c45 5445 2875 726c 2c0a 2020 2020 2020  LETE(url,.      
-0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3b0: 2020 2020 2068 6561 6465 7273 3d68 6561       headers=hea
-0000c3c0: 6465 7273 2c0a 2020 2020 2020 2020 2020  ders,.          
-0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
-0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c420: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
-0000c430: 7574 3d74 696d 656f 7574 2c0a 2020 2020  ut=timeout,.    
-0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 2020 2020 2062 6f64 793d 626f 6479         body=body
-0000c470: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-0000c480: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000c490: 6520 4170 6956 616c 7565 4572 726f 7228  e ApiValueError(
-0000c4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4b0: 2022 6874 7470 206d 6574 686f 6420 6d75   "http method mu
-0000c4c0: 7374 2062 6520 6047 4554 602c 2060 4845  st be `GET`, `HE
-0000c4d0: 4144 602c 2060 4f50 5449 4f4e 5360 2c22  AD`, `OPTIONS`,"
-0000c4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4f0: 2022 2060 504f 5354 602c 2060 5041 5443   " `POST`, `PATC
-0000c500: 4860 2c20 6050 5554 6020 6f72 2060 4445  H`, `PUT` or `DE
-0000c510: 4c45 5445 602e 220a 2020 2020 2020 2020  LETE`.".        
-0000c520: 2020 2020 290a 0a20 2020 2064 6566 2075      )..    def u
-0000c530: 7064 6174 655f 7061 7261 6d73 5f66 6f72  pdate_params_for
-0000c540: 5f61 7574 6828 0a20 2020 2020 2020 2020  _auth(.         
-0000c550: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000c560: 2020 2020 2068 6561 6465 7273 2c0a 2020       headers,.  
-0000c570: 2020 2020 2020 2020 2020 6175 7468 5f73            auth_s
-0000c580: 6574 7469 6e67 732c 0a20 2020 2020 2020  ettings,.       
-0000c590: 2020 2020 2072 6573 6f75 7263 655f 7061       resource_pa
-0000c5a0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000c5b0: 6d65 7468 6f64 2c0a 2020 2020 2020 2020  method,.        
-0000c5c0: 2020 2020 626f 6479 2c0a 2020 2020 2020      body,.      
-0000c5d0: 2020 2020 2020 7072 6566 6978 5f73 6570        prefix_sep
-0000c5e0: 6172 6174 6f72 5f69 7465 7261 746f 723a  arator_iterator:
-0000c5f0: 2050 7265 6669 7853 6570 6172 6174 6f72   PrefixSeparator
-0000c600: 4974 6572 6174 6f72 203d 204e 6f6e 650a  Iterator = None.
-0000c610: 2020 2020 2020 2020 2920 2d3e 2073 7472          ) -> str
-0000c620: 3a0a 2020 2020 2020 2020 2222 2255 7064  :.        """Upd
-0000c630: 6174 6573 2068 6561 6465 7220 616e 6420  ates header and 
-0000c640: 7175 6572 7920 7061 7261 6d73 2062 6173  query params bas
-0000c650: 6564 206f 6e20 6175 7468 656e 7469 6361  ed on authentica
-0000c660: 7469 6f6e 2073 6574 7469 6e67 2e0a 0a20  tion setting... 
-0000c670: 2020 2020 2020 203a 7061 7261 6d20 6865         :param he
-0000c680: 6164 6572 733a 2048 6561 6465 7220 7061  aders: Header pa
-0000c690: 7261 6d65 7465 7273 2064 6963 7420 746f  rameters dict to
-0000c6a0: 2062 6520 7570 6461 7465 642e 0a20 2020   be updated..   
-0000c6b0: 2020 2020 203a 7061 7261 6d20 6175 7468       :param auth
-0000c6c0: 5f73 6574 7469 6e67 733a 2041 7574 6865  _settings: Authe
-0000c6d0: 6e74 6963 6174 696f 6e20 7365 7474 696e  ntication settin
-0000c6e0: 6720 6964 656e 7469 6669 6572 7320 6c69  g identifiers li
-0000c6f0: 7374 2e0a 2020 2020 2020 2020 3a70 6172  st..        :par
-0000c700: 616d 2072 6573 6f75 7263 655f 7061 7468  am resource_path
-0000c710: 3a20 4120 7374 7269 6e67 2072 6570 7265  : A string repre
-0000c720: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
-0000c730: 2048 5454 5020 7265 7175 6573 7420 7265   HTTP request re
-0000c740: 736f 7572 6365 2070 6174 682e 0a20 2020  source path..   
-0000c750: 2020 2020 203a 7061 7261 6d20 6d65 7468       :param meth
-0000c760: 6f64 3a20 4120 7374 7269 6e67 2072 6570  od: A string rep
-0000c770: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
-0000c780: 6865 2048 5454 5020 7265 7175 6573 7420  he HTTP request 
-0000c790: 6d65 7468 6f64 2e0a 2020 2020 2020 2020  method..        
-0000c7a0: 3a70 6172 616d 2062 6f64 793a 2041 206f  :param body: A o
-0000c7b0: 626a 6563 7420 7265 7072 6573 656e 7469  bject representi
-0000c7c0: 6e67 2074 6865 2062 6f64 7920 6f66 2074  ng the body of t
-0000c7d0: 6865 2048 5454 5020 7265 7175 6573 742e  he HTTP request.
-0000c7e0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-0000c7f0: 206f 626a 6563 7420 7479 7065 2069 7320   object type is 
-0000c800: 7468 6520 7265 7475 726e 2076 616c 7565  the return value
-0000c810: 206f 6620 5f65 6e63 6f64 6572 2e64 6566   of _encoder.def
-0000c820: 6175 6c74 2829 2e0a 2020 2020 2020 2020  ault()..        
-0000c830: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
-0000c840: 6f74 2061 7574 685f 7365 7474 696e 6773  ot auth_settings
-0000c850: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000c860: 7475 726e 2072 6573 6f75 7263 655f 7061  turn resource_pa
-0000c870: 7468 0a20 2020 2020 2020 2069 6620 7072  th.        if pr
-0000c880: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
-0000c890: 7465 7261 746f 7220 6973 204e 6f6e 653a  terator is None:
-0000c8a0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-0000c8b0: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
-0000c8c0: 6572 6174 6f72 203d 2050 7265 6669 7853  erator = PrefixS
-0000c8d0: 6570 6172 6174 6f72 4974 6572 6174 6f72  eparatorIterator
-0000c8e0: 2822 3f22 2c20 2226 2229 0a0a 2020 2020  ("?", "&")..    
-0000c8f0: 2020 2020 666f 7220 6175 7468 2069 6e20      for auth in 
-0000c900: 6175 7468 5f73 6574 7469 6e67 733a 0a20  auth_settings:. 
-0000c910: 2020 2020 2020 2020 2020 2061 7574 685f             auth_
-0000c920: 7365 7474 696e 6720 3d20 7365 6c66 2e63  setting = self.c
-0000c930: 6f6e 6669 6775 7261 7469 6f6e 2e61 7574  onfiguration.aut
-0000c940: 685f 7365 7474 696e 6773 2829 2e67 6574  h_settings().get
-0000c950: 2861 7574 6829 0a20 2020 2020 2020 2020  (auth).         
-0000c960: 2020 2069 6620 6e6f 7420 6175 7468 5f73     if not auth_s
-0000c970: 6574 7469 6e67 3a0a 2020 2020 2020 2020  etting:.        
-0000c980: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0000c990: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c9a0: 6175 7468 5f73 6574 7469 6e67 5b27 696e  auth_setting['in
-0000c9b0: 275d 203d 3d20 2763 6f6f 6b69 6527 3a0a  '] == 'cookie':.
-0000c9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9d0: 6865 6164 6572 732e 6164 6428 2743 6f6f  headers.add('Coo
-0000c9e0: 6b69 6527 2c20 6175 7468 5f73 6574 7469  kie', auth_setti
-0000c9f0: 6e67 5b27 7661 6c75 6527 5d29 0a20 2020  ng['value']).   
-0000ca00: 2020 2020 2020 2020 2065 6c69 6620 6175           elif au
-0000ca10: 7468 5f73 6574 7469 6e67 5b27 696e 275d  th_setting['in']
-0000ca20: 203d 3d20 2768 6561 6465 7227 3a0a 2020   == 'header':.  
-0000ca30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000ca40: 2061 7574 685f 7365 7474 696e 675b 2774   auth_setting['t
-0000ca50: 7970 6527 5d20 213d 2027 6874 7470 2d73  ype'] != 'http-s
-0000ca60: 6967 6e61 7475 7265 273a 0a20 2020 2020  ignature':.     
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-0000ca80: 6561 6465 7273 2e61 6464 2861 7574 685f  eaders.add(auth_
-0000ca90: 7365 7474 696e 675b 276b 6579 275d 2c20  setting['key'], 
-0000caa0: 6175 7468 5f73 6574 7469 6e67 5b27 7661  auth_setting['va
-0000cab0: 6c75 6527 5d29 0a20 2020 2020 2020 2020  lue']).         
-0000cac0: 2020 2065 6c69 6620 6175 7468 5f73 6574     elif auth_set
-0000cad0: 7469 6e67 5b27 696e 275d 203d 3d20 2771  ting['in'] == 'q
-0000cae0: 7565 7279 273a 0a20 2020 2020 2020 2020  uery':.         
-0000caf0: 2020 2020 2020 2022 2222 2054 4f44 4f20         """ TODO 
-0000cb00: 696d 706c 656d 656e 7420 6175 7468 2069  implement auth i
-0000cb10: 6e20 7175 6572 790a 2020 2020 2020 2020  n query.        
-0000cb20: 2020 2020 2020 2020 6e65 6564 2074 6f20          need to 
-0000cb30: 7061 7373 2069 6e20 7072 6566 6978 5f73  pass in prefix_s
-0000cb40: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
-0000cb50: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000cb60: 2020 616e 6420 6e65 6564 2074 6f20 6f75    and need to ou
-0000cb70: 7470 7574 2072 6573 6f75 7263 655f 7061  tput resource_pa
-0000cb80: 7468 2077 6974 6820 7175 6572 7920 7061  th with query pa
-0000cb90: 7261 6d73 2061 6464 6564 0a20 2020 2020  rams added.     
-0000cba0: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000cbc0: 6573 6f75 7263 655f 7061 7468 202b 3d20  esource_path += 
-0000cbd0: 5061 7261 6d65 7465 7253 6572 6961 6c69  ParameterSeriali
-0000cbe0: 7a65 7242 6173 652e 5f72 6566 3635 3730  zerBase._ref6570
-0000cbf0: 5f65 7870 616e 7369 6f6e 280a 2020 2020  _expansion(.    
-0000cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc10: 7661 7269 6162 6c65 5f6e 616d 653d 6175  variable_name=au
-0000cc20: 7468 5f73 6574 7469 6e67 5b27 6b65 7927  th_setting['key'
-0000cc30: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000cc40: 2020 2020 2020 2069 6e5f 6461 7461 3d61         in_data=a
-0000cc50: 7574 685f 7365 7474 696e 675b 2776 616c  uth_setting['val
-0000cc60: 7565 275d 2c0a 2020 2020 2020 2020 2020  ue'],.          
-0000cc70: 2020 2020 2020 2020 2020 6578 706c 6f64            explod
-0000cc80: 653d 4661 6c73 652c 0a20 2020 2020 2020  e=False,.       
-0000cc90: 2020 2020 2020 2020 2020 2020 2070 6572               per
-0000cca0: 6365 6e74 5f65 6e63 6f64 653d 4661 6c73  cent_encode=Fals
-0000ccb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000ccc0: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
-0000ccd0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
-0000cce0: 3d70 7265 6669 785f 7365 7061 7261 746f  =prefix_separato
-0000ccf0: 725f 6974 6572 6174 6f72 0a20 2020 2020  r_iterator.     
-0000cd00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000cd10: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000cd20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000cd30: 6169 7365 2041 7069 5661 6c75 6545 7272  aise ApiValueErr
-0000cd40: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000cd50: 2020 2020 2020 2020 2741 7574 6865 6e74          'Authent
-0000cd60: 6963 6174 696f 6e20 746f 6b65 6e20 6d75  ication token mu
-0000cd70: 7374 2062 6520 696e 2060 7175 6572 7960  st be in `query`
-0000cd80: 206f 7220 6068 6561 6465 7260 270a 2020   or `header`'.  
-0000cd90: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000cda0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000cdb0: 6573 6f75 7263 655f 7061 7468 0a0a 0a63  esource_path...c
-0000cdc0: 6c61 7373 2041 7069 3a0a 2020 2020 2222  lass Api:.    ""
-0000cdd0: 224e 4f54 453a 0a20 2020 2054 6869 7320  "NOTE:.    This 
-0000cde0: 636c 6173 7320 6973 2061 7574 6f20 6765  class is auto ge
-0000cdf0: 6e65 7261 7465 640a 2020 2020 2222 220a  nerated.    """.
-0000ce00: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0000ce10: 5f28 7365 6c66 2c20 6170 695f 636c 6965  _(self, api_clie
-0000ce20: 6e74 3a20 7479 7069 6e67 2e4f 7074 696f  nt: typing.Optio
-0000ce30: 6e61 6c5b 4170 6943 6c69 656e 745d 203d  nal[ApiClient] =
-0000ce40: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-0000ce50: 6966 2061 7069 5f63 6c69 656e 7420 6973  if api_client is
-0000ce60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000ce70: 2020 2061 7069 5f63 6c69 656e 7420 3d20     api_client = 
-0000ce80: 4170 6943 6c69 656e 7428 290a 2020 2020  ApiClient().    
-0000ce90: 2020 2020 7365 6c66 2e61 7069 5f63 6c69      self.api_cli
-0000cea0: 656e 7420 3d20 6170 695f 636c 6965 6e74  ent = api_client
-0000ceb0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-0000cec0: 686f 640a 2020 2020 6465 6620 5f76 6572  hod.    def _ver
-0000ced0: 6966 795f 7479 7065 645f 6469 6374 5f69  ify_typed_dict_i
-0000cee0: 6e70 7574 735f 6f61 7067 2863 6c73 3a20  nputs_oapg(cls: 
-0000cef0: 7479 7069 6e67 2e54 7970 655b 7479 7069  typing.Type[typi
-0000cf00: 6e67 5f65 7874 656e 7369 6f6e 732e 5479  ng_extensions.Ty
-0000cf10: 7065 6444 6963 745d 2c20 6461 7461 3a20  pedDict], data: 
-0000cf20: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-0000cf30: 2074 7970 696e 672e 416e 795d 293a 0a20   typing.Any]):. 
-0000cf40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cf50: 2020 2045 6e73 7572 6573 2074 6861 743a     Ensures that:
-0000cf60: 0a20 2020 2020 2020 202d 2072 6571 7569  .        - requi
-0000cf70: 7265 6420 6b65 7973 2061 7265 2070 7265  red keys are pre
-0000cf80: 7365 6e74 0a20 2020 2020 2020 202d 2061  sent.        - a
-0000cf90: 6464 6974 696f 6e61 6c20 7072 6f70 6572  dditional proper
-0000cfa0: 7469 6573 2061 7265 206e 6f74 2069 6e70  ties are not inp
-0000cfb0: 7574 0a20 2020 2020 2020 202d 2076 616c  ut.        - val
-0000cfc0: 7565 2073 746f 7265 6420 756e 6465 7220  ue stored under 
-0000cfd0: 7265 7175 6972 6564 206b 6579 7320 646f  required keys do
-0000cfe0: 206e 6f74 2068 6176 6520 7468 6520 7661   not have the va
-0000cff0: 6c75 6520 756e 7365 740a 2020 2020 2020  lue unset.      
-0000d000: 2020 4e6f 7465 3a20 6465 7461 696c 6564    Note: detailed
-0000d010: 2076 616c 7565 2063 6865 636b 696e 6720   value checking 
-0000d020: 6973 2064 6f6e 6520 696e 2073 6368 656d  is done in schem
-0000d030: 6120 636c 6173 7365 730a 2020 2020 2020  a classes.      
-0000d040: 2020 2222 220a 2020 2020 2020 2020 6d69    """.        mi
-0000d050: 7373 696e 675f 7265 7175 6972 6564 5f6b  ssing_required_k
-0000d060: 6579 7320 3d20 5b5d 0a20 2020 2020 2020  eys = [].       
-0000d070: 2072 6571 7569 7265 645f 6b65 7973 5f77   required_keys_w
-0000d080: 6974 685f 756e 7365 745f 7661 6c75 6573  ith_unset_values
-0000d090: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
-0000d0a0: 7220 7265 7175 6972 6564 5f6b 6579 2069  r required_key i
-0000d0b0: 6e20 636c 732e 5f5f 7265 7175 6972 6564  n cls.__required
-0000d0c0: 5f6b 6579 735f 5f3a 0a20 2020 2020 2020  _keys__:.       
-0000d0d0: 2020 2020 2069 6620 7265 7175 6972 6564       if required
-0000d0e0: 5f6b 6579 206e 6f74 2069 6e20 6461 7461  _key not in data
-0000d0f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d100: 2020 6d69 7373 696e 675f 7265 7175 6972    missing_requir
-0000d110: 6564 5f6b 6579 732e 6170 7065 6e64 2872  ed_keys.append(r
-0000d120: 6571 7569 7265 645f 6b65 7929 0a20 2020  equired_key).   
-0000d130: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000d140: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-0000d150: 2020 7661 6c75 6520 3d20 6461 7461 5b72    value = data[r
-0000d160: 6571 7569 7265 645f 6b65 795d 0a20 2020  equired_key].   
-0000d170: 2020 2020 2020 2020 2069 6620 7661 6c75           if valu
-0000d180: 6520 6973 2075 6e73 6574 3a0a 2020 2020  e is unset:.    
-0000d190: 2020 2020 2020 2020 2020 2020 7265 7175              requ
-0000d1a0: 6972 6564 5f6b 6579 735f 7769 7468 5f75  ired_keys_with_u
-0000d1b0: 6e73 6574 5f76 616c 7565 732e 6170 7065  nset_values.appe
-0000d1c0: 6e64 2872 6571 7569 7265 645f 6b65 7929  nd(required_key)
-0000d1d0: 0a20 2020 2020 2020 2069 6620 6d69 7373  .        if miss
-0000d1e0: 696e 675f 7265 7175 6972 6564 5f6b 6579  ing_required_key
-0000d1f0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-0000d200: 6169 7365 2041 7069 5479 7065 4572 726f  aise ApiTypeErro
-0000d210: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000d220: 2020 2027 7b7d 206d 6973 7369 6e67 207b     '{} missing {
-0000d230: 7d20 7265 7175 6972 6564 2061 7267 756d  } required argum
-0000d240: 656e 7473 3a20 7b7d 272e 666f 726d 6174  ents: {}'.format
-0000d250: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d260: 2020 2020 2020 636c 732e 5f5f 6e61 6d65        cls.__name
-0000d270: 5f5f 2c20 6c65 6e28 6d69 7373 696e 675f  __, len(missing_
-0000d280: 7265 7175 6972 6564 5f6b 6579 7329 2c20  required_keys), 
-0000d290: 6d69 7373 696e 675f 7265 7175 6972 6564  missing_required
-0000d2a0: 5f6b 6579 730a 2020 2020 2020 2020 2020  _keys.          
-0000d2b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d2c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000d2d0: 6966 2072 6571 7569 7265 645f 6b65 7973  if required_keys
-0000d2e0: 5f77 6974 685f 756e 7365 745f 7661 6c75  _with_unset_valu
-0000d2f0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000d300: 7261 6973 6520 4170 6956 616c 7565 4572  raise ApiValueEr
-0000d310: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-0000d320: 2020 2020 2027 7b7d 2063 6f6e 7461 696e       '{} contain
-0000d330: 7320 696e 7661 6c69 6420 756e 7365 7420  s invalid unset 
-0000d340: 7661 6c75 6573 2066 6f72 207b 7d20 7265  values for {} re
-0000d350: 7175 6972 6564 206b 6579 733a 207b 7d27  quired keys: {}'
-0000d360: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0000d370: 2020 2020 2020 2020 2020 2020 2063 6c73               cls
-0000d380: 2e5f 5f6e 616d 655f 5f2c 206c 656e 2872  .__name__, len(r
-0000d390: 6571 7569 7265 645f 6b65 7973 5f77 6974  equired_keys_wit
-0000d3a0: 685f 756e 7365 745f 7661 6c75 6573 292c  h_unset_values),
-0000d3b0: 2072 6571 7569 7265 645f 6b65 7973 5f77   required_keys_w
-0000d3c0: 6974 685f 756e 7365 745f 7661 6c75 6573  ith_unset_values
-0000d3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d3e0: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-0000d3f0: 0a0a 2020 2020 2020 2020 6469 7361 6c6c  ..        disall
-0000d400: 6f77 6564 5f61 6464 6974 696f 6e61 6c5f  owed_additional_
-0000d410: 6b65 7973 203d 205b 5d0a 2020 2020 2020  keys = [].      
-0000d420: 2020 666f 7220 6b65 7920 696e 2064 6174    for key in dat
-0000d430: 613a 0a20 2020 2020 2020 2020 2020 2069  a:.            i
-0000d440: 6620 6b65 7920 696e 2063 6c73 2e5f 5f72  f key in cls.__r
-0000d450: 6571 7569 7265 645f 6b65 7973 5f5f 206f  equired_keys__ o
-0000d460: 7220 6b65 7920 696e 2063 6c73 2e5f 5f6f  r key in cls.__o
-0000d470: 7074 696f 6e61 6c5f 6b65 7973 5f5f 3a0a  ptional_keys__:.
-0000d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d490: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0000d4a0: 2020 2020 2064 6973 616c 6c6f 7765 645f       disallowed_
-0000d4b0: 6164 6469 7469 6f6e 616c 5f6b 6579 732e  additional_keys.
-0000d4c0: 6170 7065 6e64 286b 6579 290a 2020 2020  append(key).    
-0000d4d0: 2020 2020 6966 2064 6973 616c 6c6f 7765      if disallowe
-0000d4e0: 645f 6164 6469 7469 6f6e 616c 5f6b 6579  d_additional_key
-0000d4f0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
-0000d500: 6169 7365 2041 7069 5479 7065 4572 726f  aise ApiTypeErro
-0000d510: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000d520: 2020 2027 7b7d 2067 6f74 207b 7d20 756e     '{} got {} un
-0000d530: 6578 7065 6374 6564 206b 6579 776f 7264  expected keyword
-0000d540: 2061 7267 756d 656e 7473 3a20 7b7d 272e   arguments: {}'.
-0000d550: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-0000d560: 2020 2020 2020 2020 2020 2020 636c 732e              cls.
-0000d570: 5f5f 6e61 6d65 5f5f 2c20 6c65 6e28 6469  __name__, len(di
-0000d580: 7361 6c6c 6f77 6564 5f61 6464 6974 696f  sallowed_additio
-0000d590: 6e61 6c5f 6b65 7973 292c 2064 6973 616c  nal_keys), disal
-0000d5a0: 6c6f 7765 645f 6164 6469 7469 6f6e 616c  lowed_additional
-0000d5b0: 5f6b 6579 730a 2020 2020 2020 2020 2020  _keys.          
-0000d5c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000d5d0: 2020 2020 290a 0a20 2020 2064 6566 205f      )..    def _
-0000d5e0: 6765 745f 686f 7374 5f6f 6170 6728 0a20  get_host_oapg(. 
-0000d5f0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0000d600: 2020 2020 206f 7065 7261 7469 6f6e 5f69       operation_i
-0000d610: 643a 2073 7472 2c0a 2020 2020 2020 2020  d: str,.        
-0000d620: 7365 7276 6572 733a 2074 7970 696e 672e  servers: typing.
-0000d630: 5475 706c 655b 7479 7069 6e67 2e44 6963  Tuple[typing.Dic
-0000d640: 745b 7374 722c 2073 7472 5d2c 202e 2e2e  t[str, str], ...
-0000d650: 5d20 3d20 7475 706c 6528 292c 0a20 2020  ] = tuple(),.   
-0000d660: 2020 2020 2068 6f73 745f 696e 6465 783a       host_index:
-0000d670: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-0000d680: 5b69 6e74 5d20 3d20 4e6f 6e65 0a20 2020  [int] = None.   
-0000d690: 2029 202d 3e20 7479 7069 6e67 2e4f 7074   ) -> typing.Opt
-0000d6a0: 696f 6e61 6c5b 7374 725d 3a0a 2020 2020  ional[str]:.    
-0000d6b0: 2020 2020 636f 6e66 6967 7572 6174 696f      configuratio
-0000d6c0: 6e20 3d20 7365 6c66 2e61 7069 5f63 6c69  n = self.api_cli
-0000d6d0: 656e 742e 636f 6e66 6967 7572 6174 696f  ent.configuratio
-0000d6e0: 6e0a 2020 2020 2020 2020 7472 793a 0a20  n.        try:. 
-0000d6f0: 2020 2020 2020 2020 2020 2069 6620 686f             if ho
-0000d700: 7374 5f69 6e64 6578 2069 7320 4e6f 6e65  st_index is None
-0000d710: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d720: 2020 696e 6465 7820 3d20 636f 6e66 6967    index = config
-0000d730: 7572 6174 696f 6e2e 7365 7276 6572 5f6f  uration.server_o
-0000d740: 7065 7261 7469 6f6e 5f69 6e64 6578 2e67  peration_index.g
-0000d750: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
-0000d760: 2020 2020 2020 2020 6f70 6572 6174 696f          operatio
-0000d770: 6e5f 6964 2c20 636f 6e66 6967 7572 6174  n_id, configurat
-0000d780: 696f 6e2e 7365 7276 6572 5f69 6e64 6578  ion.server_index
-0000d790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d7a0: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-0000d7b0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000d7c0: 2020 2020 2069 6e64 6578 203d 2068 6f73       index = hos
-0000d7d0: 745f 696e 6465 780a 2020 2020 2020 2020  t_index.        
-0000d7e0: 2020 2020 7365 7276 6572 5f76 6172 6961      server_varia
-0000d7f0: 626c 6573 203d 2063 6f6e 6669 6775 7261  bles = configura
-0000d800: 7469 6f6e 2e73 6572 7665 725f 6f70 6572  tion.server_oper
-0000d810: 6174 696f 6e5f 7661 7269 6162 6c65 732e  ation_variables.
-0000d820: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-0000d830: 2020 2020 206f 7065 7261 7469 6f6e 5f69       operation_i
-0000d840: 642c 2063 6f6e 6669 6775 7261 7469 6f6e  d, configuration
-0000d850: 2e73 6572 7665 725f 7661 7269 6162 6c65  .server_variable
-0000d860: 730a 2020 2020 2020 2020 2020 2020 290a  s.            ).
-0000d870: 2020 2020 2020 2020 2020 2020 686f 7374              host
-0000d880: 203d 2063 6f6e 6669 6775 7261 7469 6f6e   = configuration
-0000d890: 2e67 6574 5f68 6f73 745f 6672 6f6d 5f73  .get_host_from_s
-0000d8a0: 6574 7469 6e67 7328 0a20 2020 2020 2020  ettings(.       
-0000d8b0: 2020 2020 2020 2020 2069 6e64 6578 2c20           index, 
-0000d8c0: 7661 7269 6162 6c65 733d 7365 7276 6572  variables=server
-0000d8d0: 5f76 6172 6961 626c 6573 2c20 7365 7276  _variables, serv
-0000d8e0: 6572 733d 7365 7276 6572 730a 2020 2020  ers=servers.    
-0000d8f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d900: 2020 6578 6365 7074 2049 6e64 6578 4572    except IndexEr
-0000d910: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-0000d920: 2069 6620 7365 7276 6572 733a 0a20 2020   if servers:.   
-0000d930: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000d940: 7365 2041 7069 5661 6c75 6545 7272 6f72  se ApiValueError
-0000d950: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d960: 2020 2020 2020 2249 6e76 616c 6964 2068        "Invalid h
-0000d970: 6f73 7420 696e 6465 782e 204d 7573 7420  ost index. Must 
-0000d980: 6265 2030 203c 3d20 696e 6465 7820 3c20  be 0 <= index < 
-0000d990: 2573 2220 250a 2020 2020 2020 2020 2020  %s" %.          
-0000d9a0: 2020 2020 2020 2020 2020 6c65 6e28 7365            len(se
-0000d9b0: 7276 6572 7329 0a20 2020 2020 2020 2020  rvers).         
-0000d9c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d9d0: 2020 2020 2068 6f73 7420 3d20 4e6f 6e65       host = None
-0000d9e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000d9f0: 686f 7374 0a0a 0a63 6c61 7373 2053 6572  host...class Ser
-0000da00: 6961 6c69 7a65 6452 6571 7565 7374 426f  ializedRequestBo
-0000da10: 6479 2874 7970 696e 675f 6578 7465 6e73  dy(typing_extens
-0000da20: 696f 6e73 2e54 7970 6564 4469 6374 2c20  ions.TypedDict, 
-0000da30: 746f 7461 6c3d 4661 6c73 6529 3a0a 2020  total=False):.  
-0000da40: 2020 626f 6479 3a20 7479 7069 6e67 2e55    body: typing.U
-0000da50: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
-0000da60: 0a20 2020 2066 6965 6c64 733a 2074 7970  .    fields: typ
-0000da70: 696e 672e 5475 706c 655b 7479 7069 6e67  ing.Tuple[typing
-0000da80: 2e55 6e69 6f6e 5b52 6571 7565 7374 4669  .Union[RequestFi
-0000da90: 656c 642c 2074 7970 696e 672e 5475 706c  eld, typing.Tupl
-0000daa0: 655b 7374 722c 2073 7472 5d5d 2c20 2e2e  e[str, str]], ..
-0000dab0: 2e5d 0a0a 0a63 6c61 7373 2052 6571 7565  .]...class Reque
-0000dac0: 7374 426f 6479 2853 7479 6c65 466f 726d  stBody(StyleForm
-0000dad0: 5365 7269 616c 697a 6572 2c20 4a53 4f4e  Serializer, JSON
-0000dae0: 4465 7465 6374 6f72 293a 0a20 2020 2022  Detector):.    "
-0000daf0: 2222 0a20 2020 2041 2072 6571 7565 7374  "".    A request
-0000db00: 2062 6f64 7920 7061 7261 6d65 7465 720a   body parameter.
-0000db10: 2020 2020 636f 6e74 656e 743a 2063 6f6e      content: con
-0000db20: 7465 6e74 5f74 7970 6520 746f 204d 6564  tent_type to Med
-0000db30: 6961 5479 7065 2053 6368 656d 6120 696e  iaType Schema in
-0000db40: 666f 0a20 2020 2022 2222 0a20 2020 205f  fo.    """.    _
-0000db50: 5f6a 736f 6e5f 656e 636f 6465 7220 3d20  _json_encoder = 
-0000db60: 4a53 4f4e 456e 636f 6465 7228 290a 0a20  JSONEncoder().. 
-0000db70: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0000db80: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
-0000db90: 2020 2020 2020 2063 6f6e 7465 6e74 3a20         content: 
-0000dba0: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
-0000dbb0: 204d 6564 6961 5479 7065 5d2c 0a20 2020   MediaType],.   
-0000dbc0: 2020 2020 2072 6571 7569 7265 643a 2062       required: b
-0000dbd0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
-0000dbe0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-0000dbf0: 2e72 6571 7569 7265 6420 3d20 7265 7175  .required = requ
-0000dc00: 6972 6564 0a20 2020 2020 2020 2069 6620  ired.        if 
-0000dc10: 6c65 6e28 636f 6e74 656e 7429 203d 3d20  len(content) == 
-0000dc20: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-0000dc30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000dc40: 2749 6e76 616c 6964 2076 616c 7565 2066  'Invalid value f
-0000dc50: 6f72 2063 6f6e 7465 6e74 2c20 7468 6520  or content, the 
-0000dc60: 636f 6e74 656e 7420 6469 6374 206d 7573  content dict mus
-0000dc70: 7420 6861 7665 203e 3d20 3120 656e 7472  t have >= 1 entr
-0000dc80: 7927 290a 2020 2020 2020 2020 7365 6c66  y').        self
-0000dc90: 2e63 6f6e 7465 6e74 203d 2063 6f6e 7465  .content = conte
-0000dca0: 6e74 0a0a 2020 2020 6465 6620 5f5f 7365  nt..    def __se
-0000dcb0: 7269 616c 697a 655f 6a73 6f6e 280a 2020  rialize_json(.  
-0000dcc0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0000dcd0: 2020 2020 696e 5f64 6174 613a 2074 7970      in_data: typ
-0000dce0: 696e 672e 416e 790a 2020 2020 2920 2d3e  ing.Any.    ) ->
-0000dcf0: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
-0000dd00: 2c20 6279 7465 735d 3a0a 2020 2020 2020  , bytes]:.      
-0000dd10: 2020 696e 5f64 6174 6120 3d20 7365 6c66    in_data = self
-0000dd20: 2e5f 5f6a 736f 6e5f 656e 636f 6465 722e  .__json_encoder.
-0000dd30: 6465 6661 756c 7428 696e 5f64 6174 6129  default(in_data)
-0000dd40: 0a20 2020 2020 2020 206a 736f 6e5f 7374  .        json_st
-0000dd50: 7220 3d20 6a73 6f6e 2e64 756d 7073 2869  r = json.dumps(i
-0000dd60: 6e5f 6461 7461 2c20 7365 7061 7261 746f  n_data, separato
-0000dd70: 7273 3d28 222c 222c 2022 3a22 292c 2065  rs=(",", ":"), e
-0000dd80: 6e73 7572 655f 6173 6369 693d 4661 6c73  nsure_ascii=Fals
-0000dd90: 6529 2e65 6e63 6f64 6528 0a20 2020 2020  e).encode(.     
-0000dda0: 2020 2020 2020 2022 7574 662d 3822 0a20         "utf-8". 
-0000ddb0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000ddc0: 2072 6574 7572 6e20 6469 6374 2862 6f64   return dict(bod
-0000ddd0: 793d 6a73 6f6e 5f73 7472 290a 0a20 2020  y=json_str)..   
-0000dde0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-0000ddf0: 2020 2064 6566 205f 5f73 6572 6961 6c69     def __seriali
-0000de00: 7a65 5f74 6578 745f 706c 6169 6e28 696e  ze_text_plain(in
-0000de10: 5f64 6174 613a 2074 7970 696e 672e 416e  _data: typing.An
-0000de20: 7929 202d 3e20 7479 7069 6e67 2e44 6963  y) -> typing.Dic
-0000de30: 745b 7374 722c 2073 7472 5d3a 0a20 2020  t[str, str]:.   
-0000de40: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
-0000de50: 6365 2869 6e5f 6461 7461 2c20 6672 6f7a  ce(in_data, froz
-0000de60: 656e 6469 6374 2e66 726f 7a65 6e64 6963  endict.frozendic
-0000de70: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0000de80: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000de90: 2827 556e 6162 6c65 2074 6f20 7365 7269  ('Unable to seri
-0000dea0: 616c 697a 6520 7479 7065 2066 726f 7a65  alize type froze
-0000deb0: 6e64 6963 742e 6672 6f7a 656e 6469 6374  ndict.frozendict
-0000dec0: 2074 6f20 7465 7874 2f70 6c61 696e 2729   to text/plain')
-0000ded0: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-0000dee0: 696e 7374 616e 6365 2869 6e5f 6461 7461  instance(in_data
-0000def0: 2c20 7475 706c 6529 3a0a 2020 2020 2020  , tuple):.      
-0000df00: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000df10: 6545 7272 6f72 2827 556e 6162 6c65 2074  eError('Unable t
-0000df20: 6f20 7365 7269 616c 697a 6520 7479 7065  o serialize type
-0000df30: 2074 7570 6c65 2074 6f20 7465 7874 2f70   tuple to text/p
-0000df40: 6c61 696e 2729 0a20 2020 2020 2020 2065  lain').        e
-0000df50: 6c69 6620 6973 696e 7374 616e 6365 2869  lif isinstance(i
-0000df60: 6e5f 6461 7461 2c20 4e6f 6e65 436c 6173  n_data, NoneClas
-0000df70: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000df80: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000df90: 2827 556e 6162 6c65 2074 6f20 7365 7269  ('Unable to seri
-0000dfa0: 616c 697a 6520 7479 7065 204e 6f6e 6543  alize type NoneC
-0000dfb0: 6c61 7373 2074 6f20 7465 7874 2f70 6c61  lass to text/pla
-0000dfc0: 696e 2729 0a20 2020 2020 2020 2065 6c69  in').        eli
-0000dfd0: 6620 6973 696e 7374 616e 6365 2869 6e5f  f isinstance(in_
-0000dfe0: 6461 7461 2c20 426f 6f6c 436c 6173 7329  data, BoolClass)
-0000dff0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000e000: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
-0000e010: 556e 6162 6c65 2074 6f20 7365 7269 616c  Unable to serial
-0000e020: 697a 6520 7479 7065 2042 6f6f 6c43 6c61  ize type BoolCla
-0000e030: 7373 2074 6f20 7465 7874 2f70 6c61 696e  ss to text/plain
-0000e040: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0000e050: 6e20 6469 6374 2862 6f64 793d 7374 7228  n dict(body=str(
-0000e060: 696e 5f64 6174 6129 290a 0a20 2020 2064  in_data))..    d
-0000e070: 6566 205f 5f6d 756c 7469 7061 7274 5f6a  ef __multipart_j
-0000e080: 736f 6e5f 6974 656d 2873 656c 662c 206b  son_item(self, k
-0000e090: 6579 3a20 7374 722c 2076 616c 7565 3a20  ey: str, value: 
-0000e0a0: 5363 6865 6d61 2920 2d3e 2052 6571 7565  Schema) -> Reque
-0000e0b0: 7374 4669 656c 643a 0a20 2020 2020 2020  stField:.       
-0000e0c0: 206a 736f 6e5f 7661 6c75 6520 3d20 7365   json_value = se
-0000e0d0: 6c66 2e5f 5f6a 736f 6e5f 656e 636f 6465  lf.__json_encode
-0000e0e0: 722e 6465 6661 756c 7428 7661 6c75 6529  r.default(value)
-0000e0f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000e100: 5265 7175 6573 7446 6965 6c64 286e 616d  RequestField(nam
-0000e110: 653d 6b65 792c 2064 6174 613d 6a73 6f6e  e=key, data=json
-0000e120: 2e64 756d 7073 286a 736f 6e5f 7661 6c75  .dumps(json_valu
-0000e130: 6529 2c20 6865 6164 6572 733d 7b27 436f  e), headers={'Co
-0000e140: 6e74 656e 742d 5479 7065 273a 2027 6170  ntent-Type': 'ap
-0000e150: 706c 6963 6174 696f 6e2f 6a73 6f6e 277d  plication/json'}
-0000e160: 290a 0a20 2020 2064 6566 205f 5f6d 756c  )..    def __mul
-0000e170: 7469 7061 7274 5f66 6f72 6d5f 6974 656d  tipart_form_item
-0000e180: 2873 656c 662c 206b 6579 3a20 7374 722c  (self, key: str,
-0000e190: 2076 616c 7565 3a20 5363 6865 6d61 2920   value: Schema) 
-0000e1a0: 2d3e 2052 6571 7565 7374 4669 656c 643a  -> RequestField:
-0000e1b0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-0000e1c0: 7374 616e 6365 2876 616c 7565 2c20 7374  stance(value, st
-0000e1d0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000e1e0: 7265 7475 726e 2052 6571 7565 7374 4669  return RequestFi
-0000e1f0: 656c 6428 6e61 6d65 3d6b 6579 2c20 6461  eld(name=key, da
-0000e200: 7461 3d73 7472 2876 616c 7565 292c 2068  ta=str(value), h
-0000e210: 6561 6465 7273 3d7b 2743 6f6e 7465 6e74  eaders={'Content
-0000e220: 2d54 7970 6527 3a20 2774 6578 742f 706c  -Type': 'text/pl
-0000e230: 6169 6e27 7d29 0a20 2020 2020 2020 2065  ain'}).        e
-0000e240: 6c69 6620 6973 696e 7374 616e 6365 2876  lif isinstance(v
-0000e250: 616c 7565 2c20 6279 7465 7329 3a0a 2020  alue, bytes):.  
-0000e260: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e270: 2052 6571 7565 7374 4669 656c 6428 6e61   RequestField(na
-0000e280: 6d65 3d6b 6579 2c20 6461 7461 3d76 616c  me=key, data=val
-0000e290: 7565 2c20 6865 6164 6572 733d 7b27 436f  ue, headers={'Co
-0000e2a0: 6e74 656e 742d 5479 7065 273a 2027 6170  ntent-Type': 'ap
-0000e2b0: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-0000e2c0: 7374 7265 616d 277d 290a 2020 2020 2020  stream'}).      
-0000e2d0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
-0000e2e0: 6528 7661 6c75 652c 2046 696c 6549 4f29  e(value, FileIO)
-0000e2f0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-0000e300: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
-0000e310: 2e62 6173 656e 616d 6528 7661 6c75 652e  .basename(value.
-0000e320: 6e61 6d65 290a 2020 2020 2020 2020 2020  name).          
-0000e330: 2020 7265 7175 6573 745f 6669 656c 6420    request_field 
-0000e340: 3d20 5265 7175 6573 7446 6965 6c64 280a  = RequestField(.
+000034c0: 652e 5041 5448 7d2c 0a20 2020 2020 2020  e.PATH},.       
+000034d0: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
+000034e0: 464f 524d 3a20 7b50 6172 616d 6574 6572  FORM: {Parameter
+000034f0: 496e 5479 7065 2e51 5545 5259 2c20 5061  InType.QUERY, Pa
+00003500: 7261 6d65 7465 7249 6e54 7970 652e 434f  rameterInType.CO
+00003510: 4f4b 4945 7d2c 0a20 2020 2020 2020 2050  OKIE},.        P
+00003520: 6172 616d 6574 6572 5374 796c 652e 5349  arameterStyle.SI
+00003530: 4d50 4c45 3a20 7b50 6172 616d 6574 6572  MPLE: {Parameter
+00003540: 496e 5479 7065 2e50 4154 482c 2050 6172  InType.PATH, Par
+00003550: 616d 6574 6572 496e 5479 7065 2e48 4541  ameterInType.HEA
+00003560: 4445 527d 2c0a 2020 2020 2020 2020 5061  DER},.        Pa
+00003570: 7261 6d65 7465 7253 7479 6c65 2e53 5041  rameterStyle.SPA
+00003580: 4345 5f44 454c 494d 4954 4544 3a20 7b50  CE_DELIMITED: {P
+00003590: 6172 616d 6574 6572 496e 5479 7065 2e51  arameterInType.Q
+000035a0: 5545 5259 7d2c 0a20 2020 2020 2020 2050  UERY},.        P
+000035b0: 6172 616d 6574 6572 5374 796c 652e 5049  arameterStyle.PI
+000035c0: 5045 5f44 454c 494d 4954 4544 3a20 7b50  PE_DELIMITED: {P
+000035d0: 6172 616d 6574 6572 496e 5479 7065 2e51  arameterInType.Q
+000035e0: 5545 5259 7d2c 0a20 2020 2020 2020 2050  UERY},.        P
+000035f0: 6172 616d 6574 6572 5374 796c 652e 4445  arameterStyle.DE
+00003600: 4550 5f4f 424a 4543 543a 207b 5061 7261  EP_OBJECT: {Para
+00003610: 6d65 7465 7249 6e54 7970 652e 5155 4552  meterInType.QUER
+00003620: 597d 2c0a 2020 2020 7d0a 2020 2020 5f5f  Y},.    }.    __
+00003630: 696e 5f74 7970 655f 746f 5f64 6566 6175  in_type_to_defau
+00003640: 6c74 5f73 7479 6c65 203d 207b 0a20 2020  lt_style = {.   
+00003650: 2020 2020 2050 6172 616d 6574 6572 496e       ParameterIn
+00003660: 5479 7065 2e51 5545 5259 3a20 5061 7261  Type.QUERY: Para
+00003670: 6d65 7465 7253 7479 6c65 2e46 4f52 4d2c  meterStyle.FORM,
+00003680: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00003690: 6572 496e 5479 7065 2e50 4154 483a 2050  erInType.PATH: P
+000036a0: 6172 616d 6574 6572 5374 796c 652e 5349  arameterStyle.SI
+000036b0: 4d50 4c45 2c0a 2020 2020 2020 2020 5061  MPLE,.        Pa
+000036c0: 7261 6d65 7465 7249 6e54 7970 652e 4845  rameterInType.HE
+000036d0: 4144 4552 3a20 5061 7261 6d65 7465 7253  ADER: ParameterS
+000036e0: 7479 6c65 2e53 494d 504c 452c 0a20 2020  tyle.SIMPLE,.   
+000036f0: 2020 2020 2050 6172 616d 6574 6572 496e       ParameterIn
+00003700: 5479 7065 2e43 4f4f 4b49 453a 2050 6172  Type.COOKIE: Par
+00003710: 616d 6574 6572 5374 796c 652e 464f 524d  ameterStyle.FORM
+00003720: 2c0a 2020 2020 7d0a 2020 2020 5f5f 6469  ,.    }.    __di
+00003730: 7361 6c6c 6f77 6564 5f68 6561 6465 725f  sallowed_header_
+00003740: 6e61 6d65 7320 3d20 7b27 4163 6365 7074  names = {'Accept
+00003750: 272c 2027 436f 6e74 656e 742d 5479 7065  ', 'Content-Type
+00003760: 272c 2027 4175 7468 6f72 697a 6174 696f  ', 'Authorizatio
+00003770: 6e27 7d0a 2020 2020 5f6a 736f 6e5f 656e  n'}.    _json_en
+00003780: 636f 6465 7220 3d20 4a53 4f4e 456e 636f  coder = JSONEnco
+00003790: 6465 7228 290a 0a20 2020 2040 636c 6173  der()..    @clas
+000037a0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+000037b0: 5f5f 7665 7269 6679 5f73 7479 6c65 5f74  __verify_style_t
+000037c0: 6f5f 696e 5f74 7970 6528 636c 732c 2073  o_in_type(cls, s
+000037d0: 7479 6c65 3a20 7479 7069 6e67 2e4f 7074  tyle: typing.Opt
+000037e0: 696f 6e61 6c5b 5061 7261 6d65 7465 7253  ional[ParameterS
+000037f0: 7479 6c65 5d2c 2069 6e5f 7479 7065 3a20  tyle], in_type: 
+00003800: 5061 7261 6d65 7465 7249 6e54 7970 6529  ParameterInType)
+00003810: 3a0a 2020 2020 2020 2020 6966 2073 7479  :.        if sty
+00003820: 6c65 2069 7320 4e6f 6e65 3a0a 2020 2020  le is None:.    
+00003830: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00003840: 2020 2020 2020 2069 6e5f 7479 7065 5f73         in_type_s
+00003850: 6574 203d 2063 6c73 2e5f 5f73 7479 6c65  et = cls.__style
+00003860: 5f74 6f5f 696e 5f74 7970 655b 7374 796c  _to_in_type[styl
+00003870: 655d 0a20 2020 2020 2020 2069 6620 696e  e].        if in
+00003880: 5f74 7970 6520 6e6f 7420 696e 2069 6e5f  _type not in in_
+00003890: 7479 7065 5f73 6574 3a0a 2020 2020 2020  type_set:.      
+000038a0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000038b0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+000038c0: 2020 2020 2020 2020 2749 6e76 616c 6964          'Invalid
+000038d0: 2073 7479 6c65 2061 6e64 2069 6e5f 7479   style and in_ty
+000038e0: 7065 2063 6f6d 6269 6e61 7469 6f6e 2e20  pe combination. 
+000038f0: 466f 7220 7374 796c 653d 7b7d 206f 6e6c  For style={} onl
+00003900: 7920 696e 5f74 7970 653d 7b7d 2061 7265  y in_type={} are
+00003910: 2061 6c6c 6f77 6564 272e 666f 726d 6174   allowed'.format
+00003920: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003930: 2020 2020 2020 7374 796c 652c 2069 6e5f        style, in_
+00003940: 7479 7065 5f73 6574 0a20 2020 2020 2020  type_set.       
+00003950: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00003960: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00003970: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00003980: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00003990: 2020 6e61 6d65 3a20 7374 722c 0a20 2020    name: str,.   
+000039a0: 2020 2020 2069 6e5f 7479 7065 3a20 5061       in_type: Pa
+000039b0: 7261 6d65 7465 7249 6e54 7970 652c 0a20  rameterInType,. 
+000039c0: 2020 2020 2020 2072 6571 7569 7265 643a         required:
+000039d0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+000039e0: 2020 2020 2020 2073 7479 6c65 3a20 7479         style: ty
+000039f0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 5061  ping.Optional[Pa
+00003a00: 7261 6d65 7465 7253 7479 6c65 5d20 3d20  rameterStyle] = 
+00003a10: 4e6f 6e65 2c0a 2020 2020 2020 2020 6578  None,.        ex
+00003a20: 706c 6f64 653a 2062 6f6f 6c20 3d20 4661  plode: bool = Fa
+00003a30: 6c73 652c 0a20 2020 2020 2020 2061 6c6c  lse,.        all
+00003a40: 6f77 5f72 6573 6572 7665 643a 2074 7970  ow_reserved: typ
+00003a50: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
+00003a60: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
+00003a70: 2020 2073 6368 656d 613a 2074 7970 696e     schema: typin
+00003a80: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00003a90: 672e 5479 7065 5b53 6368 656d 615d 5d20  g.Type[Schema]] 
+00003aa0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00003ab0: 636f 6e74 656e 743a 2074 7970 696e 672e  content: typing.
+00003ac0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00003ad0: 4469 6374 5b73 7472 2c20 7479 7069 6e67  Dict[str, typing
+00003ae0: 2e54 7970 655b 5363 6865 6d61 5d5d 5d20  .Type[Schema]]] 
+00003af0: 3d20 4e6f 6e65 0a20 2020 2029 3a0a 2020  = None.    ):.  
+00003b00: 2020 2020 2020 6966 2073 6368 656d 6120        if schema 
+00003b10: 6973 204e 6f6e 6520 616e 6420 636f 6e74  is None and cont
+00003b20: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
+00003b30: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00003b40: 616c 7565 4572 726f 7228 2756 616c 7565  alueError('Value
+00003b50: 206d 6973 7369 6e67 3b20 5061 7373 2069   missing; Pass i
+00003b60: 6e20 6569 7468 6572 2073 6368 656d 6120  n either schema 
+00003b70: 6f72 2063 6f6e 7465 6e74 2729 0a20 2020  or content').   
+00003b80: 2020 2020 2069 6620 7363 6865 6d61 2061       if schema a
+00003b90: 6e64 2063 6f6e 7465 6e74 3a0a 2020 2020  nd content:.    
+00003ba0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00003bb0: 6c75 6545 7272 6f72 2827 546f 6f20 6d61  lueError('Too ma
+00003bc0: 6e79 2076 616c 7565 7320 7072 6f76 6964  ny values provid
+00003bd0: 6564 2e20 426f 7468 2073 6368 656d 6120  ed. Both schema 
+00003be0: 616e 6420 636f 6e74 656e 7420 7765 7265  and content were
+00003bf0: 2070 726f 7669 6465 642e 204f 6e6c 7920   provided. Only 
+00003c00: 6f6e 6520 6d61 7920 6265 2069 6e70 7574  one may be input
+00003c10: 2729 0a20 2020 2020 2020 2069 6620 6e61  ').        if na
+00003c20: 6d65 2069 6e20 7365 6c66 2e5f 5f64 6973  me in self.__dis
+00003c30: 616c 6c6f 7765 645f 6865 6164 6572 5f6e  allowed_header_n
+00003c40: 616d 6573 2061 6e64 2069 6e5f 7479 7065  ames and in_type
+00003c50: 2069 7320 5061 7261 6d65 7465 7249 6e54   is ParameterInT
+00003c60: 7970 652e 4845 4144 4552 3a0a 2020 2020  ype.HEADER:.    
+00003c70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00003c80: 6c75 6545 7272 6f72 2827 496e 7661 6c69  lueError('Invali
+00003c90: 6420 6e61 6d65 2c20 6e61 6d65 206d 6179  d name, name may
+00003ca0: 206e 6f74 2062 6520 6f6e 6520 6f66 207b   not be one of {
+00003cb0: 7d27 2e66 6f72 6d61 7428 7365 6c66 2e5f  }'.format(self._
+00003cc0: 5f64 6973 616c 6c6f 7765 645f 6865 6164  _disallowed_head
+00003cd0: 6572 5f6e 616d 6573 2929 0a20 2020 2020  er_names)).     
+00003ce0: 2020 2073 656c 662e 5f5f 7665 7269 6679     self.__verify
+00003cf0: 5f73 7479 6c65 5f74 6f5f 696e 5f74 7970  _style_to_in_typ
+00003d00: 6528 7374 796c 652c 2069 6e5f 7479 7065  e(style, in_type
+00003d10: 290a 2020 2020 2020 2020 6966 2063 6f6e  ).        if con
+00003d20: 7465 6e74 2069 7320 4e6f 6e65 2061 6e64  tent is None and
+00003d30: 2073 7479 6c65 2069 7320 4e6f 6e65 3a0a   style is None:.
+00003d40: 2020 2020 2020 2020 2020 2020 7374 796c              styl
+00003d50: 6520 3d20 7365 6c66 2e5f 5f69 6e5f 7479  e = self.__in_ty
+00003d60: 7065 5f74 6f5f 6465 6661 756c 745f 7374  pe_to_default_st
+00003d70: 796c 655b 696e 5f74 7970 655d 0a20 2020  yle[in_type].   
+00003d80: 2020 2020 2069 6620 636f 6e74 656e 7420       if content 
+00003d90: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+00003da0: 696e 5f74 7970 6520 696e 2073 656c 662e  in_type in self.
+00003db0: 5f5f 696e 5f74 7970 655f 746f 5f64 6566  __in_type_to_def
+00003dc0: 6175 6c74 5f73 7479 6c65 2061 6e64 206c  ault_style and l
+00003dd0: 656e 2863 6f6e 7465 6e74 2920 213d 2031  en(content) != 1
+00003de0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00003df0: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00003e00: 496e 7661 6c69 6420 636f 6e74 656e 7420  Invalid content 
+00003e10: 6c65 6e67 7468 2c20 636f 6e74 656e 7420  length, content 
+00003e20: 6c65 6e67 7468 206d 7573 7420 6571 7561  length must equa
+00003e30: 6c20 3127 290a 2020 2020 2020 2020 7365  l 1').        se
+00003e40: 6c66 2e69 6e5f 7479 7065 203d 2069 6e5f  lf.in_type = in_
+00003e50: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
+00003e60: 662e 6e61 6d65 203d 206e 616d 650a 2020  f.name = name.  
+00003e70: 2020 2020 2020 7365 6c66 2e72 6571 7569        self.requi
+00003e80: 7265 6420 3d20 7265 7175 6972 6564 0a20  red = required. 
+00003e90: 2020 2020 2020 2073 656c 662e 7374 796c         self.styl
+00003ea0: 6520 3d20 7374 796c 650a 2020 2020 2020  e = style.      
+00003eb0: 2020 7365 6c66 2e65 7870 6c6f 6465 203d    self.explode =
+00003ec0: 2065 7870 6c6f 6465 0a20 2020 2020 2020   explode.       
+00003ed0: 2073 656c 662e 616c 6c6f 775f 7265 7365   self.allow_rese
+00003ee0: 7276 6564 203d 2061 6c6c 6f77 5f72 6573  rved = allow_res
+00003ef0: 6572 7665 640a 2020 2020 2020 2020 7365  erved.        se
+00003f00: 6c66 2e73 6368 656d 6120 3d20 7363 6865  lf.schema = sche
+00003f10: 6d61 0a20 2020 2020 2020 2073 656c 662e  ma.        self.
+00003f20: 636f 6e74 656e 7420 3d20 636f 6e74 656e  content = conten
+00003f30: 740a 0a20 2020 2064 6566 205f 7365 7269  t..    def _seri
+00003f40: 616c 697a 655f 6a73 6f6e 280a 2020 2020  alize_json(.    
+00003f50: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00003f60: 2020 696e 5f64 6174 613a 2074 7970 696e    in_data: typin
+00003f70: 672e 556e 696f 6e5b 4e6f 6e65 2c20 696e  g.Union[None, in
+00003f80: 742c 2066 6c6f 6174 2c20 7374 722c 2062  t, float, str, b
+00003f90: 6f6f 6c2c 2064 6963 742c 206c 6973 745d  ool, dict, list]
+00003fa0: 2c0a 2020 2020 2020 2020 656c 696d 696e  ,.        elimin
+00003fb0: 6174 655f 7768 6974 6573 7061 6365 3a20  ate_whitespace: 
+00003fc0: 626f 6f6c 203d 2046 616c 7365 0a20 2020  bool = False.   
+00003fd0: 2029 202d 3e20 7374 723a 0a20 2020 2020   ) -> str:.     
+00003fe0: 2020 2069 6620 656c 696d 696e 6174 655f     if eliminate_
+00003ff0: 7768 6974 6573 7061 6365 3a0a 2020 2020  whitespace:.    
+00004000: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+00004010: 736f 6e2e 6475 6d70 7328 696e 5f64 6174  son.dumps(in_dat
+00004020: 612c 2073 6570 6172 6174 6f72 733d 7365  a, separators=se
+00004030: 6c66 2e5f 6a73 6f6e 5f65 6e63 6f64 6572  lf._json_encoder
+00004040: 2e63 6f6d 7061 6374 5f73 6570 6172 6174  .compact_separat
+00004050: 6f72 7329 0a20 2020 2020 2020 2072 6574  ors).        ret
+00004060: 7572 6e20 6a73 6f6e 2e64 756d 7073 2869  urn json.dumps(i
+00004070: 6e5f 6461 7461 290a 0a0a 636c 6173 7320  n_data)...class 
+00004080: 5061 7468 5061 7261 6d65 7465 7228 5061  PathParameter(Pa
+00004090: 7261 6d65 7465 7242 6173 652c 2053 7479  rameterBase, Sty
+000040a0: 6c65 5369 6d70 6c65 5365 7269 616c 697a  leSimpleSerializ
+000040b0: 6572 293a 0a0a 2020 2020 6465 6620 5f5f  er):..    def __
+000040c0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+000040d0: 7365 6c66 2c0a 2020 2020 2020 2020 6e61  self,.        na
+000040e0: 6d65 3a20 7374 722c 0a20 2020 2020 2020  me: str,.       
+000040f0: 2072 6571 7569 7265 643a 2062 6f6f 6c20   required: bool 
+00004100: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+00004110: 2073 7479 6c65 3a20 7479 7069 6e67 2e4f   style: typing.O
+00004120: 7074 696f 6e61 6c5b 5061 7261 6d65 7465  ptional[Paramete
+00004130: 7253 7479 6c65 5d20 3d20 4e6f 6e65 2c0a  rStyle] = None,.
+00004140: 2020 2020 2020 2020 6578 706c 6f64 653a          explode:
+00004150: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00004160: 2020 2020 2020 2061 6c6c 6f77 5f72 6573         allow_res
+00004170: 6572 7665 643a 2074 7970 696e 672e 4f70  erved: typing.Op
+00004180: 7469 6f6e 616c 5b62 6f6f 6c5d 203d 204e  tional[bool] = N
+00004190: 6f6e 652c 0a20 2020 2020 2020 2073 6368  one,.        sch
+000041a0: 656d 613a 2074 7970 696e 672e 4f70 7469  ema: typing.Opti
+000041b0: 6f6e 616c 5b74 7970 696e 672e 5479 7065  onal[typing.Type
+000041c0: 5b53 6368 656d 615d 5d20 3d20 4e6f 6e65  [Schema]] = None
+000041d0: 2c0a 2020 2020 2020 2020 636f 6e74 656e  ,.        conten
+000041e0: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
+000041f0: 616c 5b74 7970 696e 672e 4469 6374 5b73  al[typing.Dict[s
+00004200: 7472 2c20 7479 7069 6e67 2e54 7970 655b  tr, typing.Type[
+00004210: 5363 6865 6d61 5d5d 5d20 3d20 4e6f 6e65  Schema]]] = None
+00004220: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00004230: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+00004240: 280a 2020 2020 2020 2020 2020 2020 6e61  (.            na
+00004250: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00004260: 696e 5f74 7970 653d 5061 7261 6d65 7465  in_type=Paramete
+00004270: 7249 6e54 7970 652e 5041 5448 2c0a 2020  rInType.PATH,.  
+00004280: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+00004290: 6564 3d72 6571 7569 7265 642c 0a20 2020  ed=required,.   
+000042a0: 2020 2020 2020 2020 2073 7479 6c65 3d73           style=s
+000042b0: 7479 6c65 2c0a 2020 2020 2020 2020 2020  tyle,.          
+000042c0: 2020 6578 706c 6f64 653d 6578 706c 6f64    explode=explod
+000042d0: 652c 0a20 2020 2020 2020 2020 2020 2061  e,.            a
+000042e0: 6c6c 6f77 5f72 6573 6572 7665 643d 616c  llow_reserved=al
+000042f0: 6c6f 775f 7265 7365 7276 6564 2c0a 2020  low_reserved,.  
+00004300: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
+00004310: 3d73 6368 656d 612c 0a20 2020 2020 2020  =schema,.       
+00004320: 2020 2020 2063 6f6e 7465 6e74 3d63 6f6e       content=con
+00004330: 7465 6e74 0a20 2020 2020 2020 2029 0a0a  tent.        )..
+00004340: 2020 2020 6465 6620 5f5f 7365 7269 616c      def __serial
+00004350: 697a 655f 6c61 6265 6c28 0a20 2020 2020  ize_label(.     
+00004360: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00004370: 2069 6e5f 6461 7461 3a20 7479 7069 6e67   in_data: typing
+00004380: 2e55 6e69 6f6e 5b4e 6f6e 652c 2069 6e74  .Union[None, int
+00004390: 2c20 666c 6f61 742c 2073 7472 2c20 626f  , float, str, bo
+000043a0: 6f6c 2c20 6469 6374 2c20 6c69 7374 5d0a  ol, dict, list].
+000043b0: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
+000043c0: 4469 6374 5b73 7472 2c20 7374 725d 3a0a  Dict[str, str]:.
+000043d0: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+000043e0: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+000043f0: 7220 3d20 5072 6566 6978 5365 7061 7261  r = PrefixSepara
+00004400: 746f 7249 7465 7261 746f 7228 272e 272c  torIterator('.',
+00004410: 2027 2e27 290a 2020 2020 2020 2020 7661   '.').        va
+00004420: 6c75 6520 3d20 7365 6c66 2e5f 7265 6636  lue = self._ref6
+00004430: 3537 305f 6578 7061 6e73 696f 6e28 0a20  570_expansion(. 
+00004440: 2020 2020 2020 2020 2020 2076 6172 6961             varia
+00004450: 626c 655f 6e61 6d65 3d73 656c 662e 6e61  ble_name=self.na
+00004460: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00004470: 696e 5f64 6174 613d 696e 5f64 6174 612c  in_data=in_data,
+00004480: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+00004490: 6c6f 6465 3d73 656c 662e 6578 706c 6f64  lode=self.explod
+000044a0: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
+000044b0: 6572 6365 6e74 5f65 6e63 6f64 653d 5472  ercent_encode=Tr
+000044c0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000044d0: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+000044e0: 5f69 7465 7261 746f 723d 7072 6566 6978  _iterator=prefix
+000044f0: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+00004500: 746f 720a 2020 2020 2020 2020 290a 2020  tor.        ).  
+00004510: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00004520: 662e 5f74 6f5f 6469 6374 2873 656c 662e  f._to_dict(self.
+00004530: 6e61 6d65 2c20 7661 6c75 6529 0a0a 2020  name, value)..  
+00004540: 2020 6465 6620 5f5f 7365 7269 616c 697a    def __serializ
+00004550: 655f 6d61 7472 6978 280a 2020 2020 2020  e_matrix(.      
+00004560: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00004570: 696e 5f64 6174 613a 2074 7970 696e 672e  in_data: typing.
+00004580: 556e 696f 6e5b 4e6f 6e65 2c20 696e 742c  Union[None, int,
+00004590: 2066 6c6f 6174 2c20 7374 722c 2062 6f6f   float, str, boo
+000045a0: 6c2c 2064 6963 742c 206c 6973 745d 0a20  l, dict, list]. 
+000045b0: 2020 2029 202d 3e20 7479 7069 6e67 2e44     ) -> typing.D
+000045c0: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
+000045d0: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+000045e0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+000045f0: 203d 2050 7265 6669 7853 6570 6172 6174   = PrefixSeparat
+00004600: 6f72 4974 6572 6174 6f72 2827 3b27 2c20  orIterator(';', 
+00004610: 273b 2729 0a20 2020 2020 2020 2076 616c  ';').        val
+00004620: 7565 203d 2073 656c 662e 5f72 6566 3635  ue = self._ref65
+00004630: 3730 5f65 7870 616e 7369 6f6e 280a 2020  70_expansion(.  
+00004640: 2020 2020 2020 2020 2020 7661 7269 6162            variab
+00004650: 6c65 5f6e 616d 653d 7365 6c66 2e6e 616d  le_name=self.nam
+00004660: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
+00004670: 6e5f 6461 7461 3d69 6e5f 6461 7461 2c0a  n_data=in_data,.
+00004680: 2020 2020 2020 2020 2020 2020 6578 706c              expl
+00004690: 6f64 653d 7365 6c66 2e65 7870 6c6f 6465  ode=self.explode
+000046a0: 2c0a 2020 2020 2020 2020 2020 2020 7065  ,.            pe
+000046b0: 7263 656e 745f 656e 636f 6465 3d54 7275  rcent_encode=Tru
+000046c0: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
+000046d0: 7265 6669 785f 7365 7061 7261 746f 725f  refix_separator_
+000046e0: 6974 6572 6174 6f72 3d70 7265 6669 785f  iterator=prefix_
+000046f0: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+00004700: 6f72 0a20 2020 2020 2020 2029 0a20 2020  or.        ).   
+00004710: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00004720: 2e5f 746f 5f64 6963 7428 7365 6c66 2e6e  ._to_dict(self.n
+00004730: 616d 652c 2076 616c 7565 290a 0a20 2020  ame, value)..   
+00004740: 2064 6566 205f 5f73 6572 6961 6c69 7a65   def __serialize
+00004750: 5f73 696d 706c 6528 0a20 2020 2020 2020  _simple(.       
+00004760: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
+00004770: 6e5f 6461 7461 3a20 7479 7069 6e67 2e55  n_data: typing.U
+00004780: 6e69 6f6e 5b4e 6f6e 652c 2069 6e74 2c20  nion[None, int, 
+00004790: 666c 6f61 742c 2073 7472 2c20 626f 6f6c  float, str, bool
+000047a0: 2c20 6469 6374 2c20 6c69 7374 5d2c 0a20  , dict, list],. 
+000047b0: 2020 2029 202d 3e20 7479 7069 6e67 2e44     ) -> typing.D
+000047c0: 6963 745b 7374 722c 2073 7472 5d3a 0a20  ict[str, str]:. 
+000047d0: 2020 2020 2020 2076 616c 7565 203d 2073         value = s
+000047e0: 656c 662e 5f73 6572 6961 6c69 7a65 5f73  elf._serialize_s
+000047f0: 696d 706c 6528 0a20 2020 2020 2020 2020  imple(.         
+00004800: 2020 2069 6e5f 6461 7461 3d69 6e5f 6461     in_data=in_da
+00004810: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00004820: 6e61 6d65 3d73 656c 662e 6e61 6d65 2c0a  name=self.name,.
+00004830: 2020 2020 2020 2020 2020 2020 6578 706c              expl
+00004840: 6f64 653d 7365 6c66 2e65 7870 6c6f 6465  ode=self.explode
+00004850: 2c0a 2020 2020 2020 2020 2020 2020 7065  ,.            pe
+00004860: 7263 656e 745f 656e 636f 6465 3d54 7275  rcent_encode=Tru
+00004870: 650a 2020 2020 2020 2020 290a 2020 2020  e.        ).    
+00004880: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004890: 5f74 6f5f 6469 6374 2873 656c 662e 6e61  _to_dict(self.na
+000048a0: 6d65 2c20 7661 6c75 6529 0a0a 2020 2020  me, value)..    
+000048b0: 6465 6620 7365 7269 616c 697a 6528 0a20  def serialize(. 
+000048c0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000048d0: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
+000048e0: 7069 6e67 2e55 6e69 6f6e 5b0a 2020 2020  ping.Union[.    
+000048f0: 2020 2020 2020 2020 5363 6865 6d61 2c20          Schema, 
+00004900: 4465 6369 6d61 6c2c 2069 6e74 2c20 666c  Decimal, int, fl
+00004910: 6f61 742c 2073 7472 2c20 6461 7465 2c20  oat, str, date, 
+00004920: 6461 7465 7469 6d65 2c20 4e6f 6e65 2c20  datetime, None, 
+00004930: 626f 6f6c 2c20 6c69 7374 2c20 7475 706c  bool, list, tupl
+00004940: 652c 2064 6963 742c 2066 726f 7a65 6e64  e, dict, frozend
+00004950: 6963 742e 6672 6f7a 656e 6469 6374 5d0a  ict.frozendict].
+00004960: 2020 2020 2920 2d3e 2074 7970 696e 672e      ) -> typing.
+00004970: 4469 6374 5b73 7472 2c20 7374 725d 3a0a  Dict[str, str]:.
+00004980: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00004990: 7363 6865 6d61 3a0a 2020 2020 2020 2020  schema:.        
+000049a0: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
+000049b0: 203d 2073 656c 662e 7363 6865 6d61 2869   = self.schema(i
+000049c0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+000049d0: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
+000049e0: 203d 2073 656c 662e 5f6a 736f 6e5f 656e   = self._json_en
+000049f0: 636f 6465 722e 6465 6661 756c 7428 6361  coder.default(ca
+00004a00: 7374 5f69 6e5f 6461 7461 290a 2020 2020  st_in_data).    
+00004a10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00004a20: 2020 2020 2020 2020 7369 6d70 6c65 202d          simple -
+00004a30: 3e20 7061 7468 0a20 2020 2020 2020 2020  > path.         
+00004a40: 2020 2020 2020 2070 6174 683a 0a20 2020         path:.   
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a60: 2072 6574 7572 6e73 2070 6174 685f 7061   returns path_pa
+00004a70: 7261 6d73 3a20 6469 6374 0a20 2020 2020  rams: dict.     
+00004a80: 2020 2020 2020 206c 6162 656c 202d 3e20         label -> 
+00004a90: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00004aa0: 2020 2020 2072 6574 7572 6e73 2070 6174       returns pat
+00004ab0: 685f 7061 7261 6d73 0a20 2020 2020 2020  h_params.       
+00004ac0: 2020 2020 206d 6174 7269 7820 2d3e 2070       matrix -> p
+00004ad0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00004ae0: 2020 2020 7265 7475 726e 7320 7061 7468      returns path
+00004af0: 5f70 6172 616d 730a 2020 2020 2020 2020  _params.        
+00004b00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00004b10: 2020 2020 6966 2073 656c 662e 7374 796c      if self.styl
+00004b20: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00004b30: 2020 2069 6620 7365 6c66 2e73 7479 6c65     if self.style
+00004b40: 2069 7320 5061 7261 6d65 7465 7253 7479   is ParameterSty
+00004b50: 6c65 2e53 494d 504c 453a 0a20 2020 2020  le.SIMPLE:.     
+00004b60: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004b70: 6574 7572 6e20 7365 6c66 2e5f 5f73 6572  eturn self.__ser
+00004b80: 6961 6c69 7a65 5f73 696d 706c 6528 6361  ialize_simple(ca
+00004b90: 7374 5f69 6e5f 6461 7461 290a 2020 2020  st_in_data).    
+00004ba0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00004bb0: 2073 656c 662e 7374 796c 6520 6973 2050   self.style is P
+00004bc0: 6172 616d 6574 6572 5374 796c 652e 4c41  arameterStyle.LA
+00004bd0: 4245 4c3a 0a20 2020 2020 2020 2020 2020  BEL:.           
+00004be0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00004bf0: 7365 6c66 2e5f 5f73 6572 6961 6c69 7a65  self.__serialize
+00004c00: 5f6c 6162 656c 2863 6173 745f 696e 5f64  _label(cast_in_d
+00004c10: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00004c20: 2020 2020 2065 6c69 6620 7365 6c66 2e73       elif self.s
+00004c30: 7479 6c65 2069 7320 5061 7261 6d65 7465  tyle is Paramete
+00004c40: 7253 7479 6c65 2e4d 4154 5249 583a 0a20  rStyle.MATRIX:. 
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00004c70: 5f73 6572 6961 6c69 7a65 5f6d 6174 7269  _serialize_matri
+00004c80: 7828 6361 7374 5f69 6e5f 6461 7461 290a  x(cast_in_data).
+00004c90: 2020 2020 2020 2020 2320 7365 6c66 2e63          # self.c
+00004ca0: 6f6e 7465 6e74 2077 696c 6c20 6265 206c  ontent will be l
+00004cb0: 656e 6774 6820 6f6e 650a 2020 2020 2020  ength one.      
+00004cc0: 2020 666f 7220 636f 6e74 656e 745f 7479    for content_ty
+00004cd0: 7065 2c20 7363 6865 6d61 2069 6e20 7365  pe, schema in se
+00004ce0: 6c66 2e63 6f6e 7465 6e74 2e69 7465 6d73  lf.content.items
+00004cf0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00004d00: 6361 7374 5f69 6e5f 6461 7461 203d 2073  cast_in_data = s
+00004d10: 6368 656d 6128 696e 5f64 6174 6129 0a20  chema(in_data). 
+00004d20: 2020 2020 2020 2020 2020 2063 6173 745f             cast_
+00004d30: 696e 5f64 6174 6120 3d20 7365 6c66 2e5f  in_data = self._
+00004d40: 6a73 6f6e 5f65 6e63 6f64 6572 2e64 6566  json_encoder.def
+00004d50: 6175 6c74 2863 6173 745f 696e 5f64 6174  ault(cast_in_dat
+00004d60: 6129 0a20 2020 2020 2020 2020 2020 2069  a).            i
+00004d70: 6620 7365 6c66 2e5f 636f 6e74 656e 745f  f self._content_
+00004d80: 7479 7065 5f69 735f 6a73 6f6e 2863 6f6e  type_is_json(con
+00004d90: 7465 6e74 5f74 7970 6529 3a0a 2020 2020  tent_type):.    
+00004da0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00004db0: 6520 3d20 7365 6c66 2e5f 7365 7269 616c  e = self._serial
+00004dc0: 697a 655f 6a73 6f6e 2863 6173 745f 696e  ize_json(cast_in
+00004dd0: 5f64 6174 6129 0a20 2020 2020 2020 2020  _data).         
+00004de0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00004df0: 6c66 2e5f 746f 5f64 6963 7428 7365 6c66  lf._to_dict(self
+00004e00: 2e6e 616d 652c 2076 616c 7565 290a 2020  .name, value).  
+00004e10: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00004e20: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00004e30: 726f 7228 2753 6572 6961 6c69 7a61 7469  ror('Serializati
+00004e40: 6f6e 206f 6620 7b7d 2068 6173 206e 6f74  on of {} has not
+00004e50: 2079 6574 2062 6565 6e20 696d 706c 656d   yet been implem
+00004e60: 656e 7465 6427 2e66 6f72 6d61 7428 636f  ented'.format(co
+00004e70: 6e74 656e 745f 7479 7065 2929 0a0a 0a63  ntent_type))...c
+00004e80: 6c61 7373 2051 7565 7279 5061 7261 6d65  lass QueryParame
+00004e90: 7465 7228 5061 7261 6d65 7465 7242 6173  ter(ParameterBas
+00004ea0: 652c 2053 7479 6c65 466f 726d 5365 7269  e, StyleFormSeri
+00004eb0: 616c 697a 6572 293a 0a0a 2020 2020 6465  alizer):..    de
+00004ec0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00004ed0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00004ee0: 2020 6e61 6d65 3a20 7374 722c 0a20 2020    name: str,.   
+00004ef0: 2020 2020 2072 6571 7569 7265 643a 2062       required: b
+00004f00: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+00004f10: 2020 2020 2073 7479 6c65 3a20 7479 7069       style: typi
+00004f20: 6e67 2e4f 7074 696f 6e61 6c5b 5061 7261  ng.Optional[Para
+00004f30: 6d65 7465 7253 7479 6c65 5d20 3d20 4e6f  meterStyle] = No
+00004f40: 6e65 2c0a 2020 2020 2020 2020 6578 706c  ne,.        expl
+00004f50: 6f64 653a 2074 7970 696e 672e 4f70 7469  ode: typing.Opti
+00004f60: 6f6e 616c 5b62 6f6f 6c5d 203d 204e 6f6e  onal[bool] = Non
+00004f70: 652c 0a20 2020 2020 2020 2061 6c6c 6f77  e,.        allow
+00004f80: 5f72 6573 6572 7665 643a 2074 7970 696e  _reserved: typin
+00004f90: 672e 4f70 7469 6f6e 616c 5b62 6f6f 6c5d  g.Optional[bool]
+00004fa0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00004fb0: 2073 6368 656d 613a 2074 7970 696e 672e   schema: typing.
+00004fc0: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00004fd0: 5479 7065 5b53 6368 656d 615d 5d20 3d20  Type[Schema]] = 
+00004fe0: 4e6f 6e65 2c0a 2020 2020 2020 2020 636f  None,.        co
+00004ff0: 6e74 656e 743a 2074 7970 696e 672e 4f70  ntent: typing.Op
+00005000: 7469 6f6e 616c 5b74 7970 696e 672e 4469  tional[typing.Di
+00005010: 6374 5b73 7472 2c20 7479 7069 6e67 2e54  ct[str, typing.T
+00005020: 7970 655b 5363 6865 6d61 5d5d 5d20 3d20  ype[Schema]]] = 
+00005030: 4e6f 6e65 0a20 2020 2029 3a0a 2020 2020  None.    ):.    
+00005040: 2020 2020 7573 6564 5f73 7479 6c65 203d      used_style =
+00005050: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
+00005060: 464f 524d 2069 6620 7374 796c 6520 6973  FORM if style is
+00005070: 204e 6f6e 6520 656c 7365 2073 7479 6c65   None else style
+00005080: 0a20 2020 2020 2020 2075 7365 645f 6578  .        used_ex
+00005090: 706c 6f64 6520 3d20 7365 6c66 2e5f 6765  plode = self._ge
+000050a0: 745f 6465 6661 756c 745f 6578 706c 6f64  t_default_explod
+000050b0: 6528 7573 6564 5f73 7479 6c65 2920 6966  e(used_style) if
+000050c0: 2065 7870 6c6f 6465 2069 7320 4e6f 6e65   explode is None
+000050d0: 2065 6c73 6520 6578 706c 6f64 650a 0a20   else explode.. 
+000050e0: 2020 2020 2020 2073 7570 6572 2829 2e5f         super()._
+000050f0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00005100: 2020 2020 206e 616d 652c 0a20 2020 2020       name,.     
+00005110: 2020 2020 2020 2069 6e5f 7479 7065 3d50         in_type=P
+00005120: 6172 616d 6574 6572 496e 5479 7065 2e51  arameterInType.Q
+00005130: 5545 5259 2c0a 2020 2020 2020 2020 2020  UERY,.          
+00005140: 2020 7265 7175 6972 6564 3d72 6571 7569    required=requi
+00005150: 7265 642c 0a20 2020 2020 2020 2020 2020  red,.           
+00005160: 2073 7479 6c65 3d75 7365 645f 7374 796c   style=used_styl
+00005170: 652c 0a20 2020 2020 2020 2020 2020 2065  e,.            e
+00005180: 7870 6c6f 6465 3d75 7365 645f 6578 706c  xplode=used_expl
+00005190: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
+000051a0: 2061 6c6c 6f77 5f72 6573 6572 7665 643d   allow_reserved=
+000051b0: 616c 6c6f 775f 7265 7365 7276 6564 2c0a  allow_reserved,.
+000051c0: 2020 2020 2020 2020 2020 2020 7363 6865              sche
+000051d0: 6d61 3d73 6368 656d 612c 0a20 2020 2020  ma=schema,.     
+000051e0: 2020 2020 2020 2063 6f6e 7465 6e74 3d63         content=c
+000051f0: 6f6e 7465 6e74 0a20 2020 2020 2020 2029  ontent.        )
+00005200: 0a0a 2020 2020 6465 6620 5f5f 7365 7269  ..    def __seri
+00005210: 616c 697a 655f 7370 6163 655f 6465 6c69  alize_space_deli
+00005220: 6d69 7465 6428 0a20 2020 2020 2020 2073  mited(.        s
+00005230: 656c 662c 0a20 2020 2020 2020 2069 6e5f  elf,.        in_
+00005240: 6461 7461 3a20 7479 7069 6e67 2e55 6e69  data: typing.Uni
+00005250: 6f6e 5b4e 6f6e 652c 2069 6e74 2c20 666c  on[None, int, fl
+00005260: 6f61 742c 2073 7472 2c20 626f 6f6c 2c20  oat, str, bool, 
+00005270: 6469 6374 2c20 6c69 7374 5d2c 0a20 2020  dict, list],.   
+00005280: 2020 2020 2070 7265 6669 785f 7365 7061       prefix_sepa
+00005290: 7261 746f 725f 6974 6572 6174 6f72 3a20  rator_iterator: 
+000052a0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000052b0: 5072 6566 6978 5365 7061 7261 746f 7249  PrefixSeparatorI
+000052c0: 7465 7261 746f 725d 0a20 2020 2029 202d  terator].    ) -
+000052d0: 3e20 7479 7069 6e67 2e44 6963 745b 7374  > typing.Dict[st
+000052e0: 722c 2073 7472 5d3a 0a20 2020 2020 2020  r, str]:.       
+000052f0: 2069 6620 7072 6566 6978 5f73 6570 6172   if prefix_separ
+00005300: 6174 6f72 5f69 7465 7261 746f 7220 6973  ator_iterator is
+00005310: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005320: 2020 2070 7265 6669 785f 7365 7061 7261     prefix_separa
+00005330: 746f 725f 6974 6572 6174 6f72 203d 2073  tor_iterator = s
+00005340: 656c 662e 6765 745f 7072 6566 6978 5f73  elf.get_prefix_s
+00005350: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00005360: 7228 290a 2020 2020 2020 2020 7661 6c75  r().        valu
+00005370: 6520 3d20 7365 6c66 2e5f 7265 6636 3537  e = self._ref657
+00005380: 305f 6578 7061 6e73 696f 6e28 0a20 2020  0_expansion(.   
+00005390: 2020 2020 2020 2020 2076 6172 6961 626c           variabl
+000053a0: 655f 6e61 6d65 3d73 656c 662e 6e61 6d65  e_name=self.name
+000053b0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+000053c0: 5f64 6174 613d 696e 5f64 6174 612c 0a20  _data=in_data,. 
+000053d0: 2020 2020 2020 2020 2020 2065 7870 6c6f             explo
+000053e0: 6465 3d73 656c 662e 6578 706c 6f64 652c  de=self.explode,
+000053f0: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
+00005400: 6365 6e74 5f65 6e63 6f64 653d 5472 7565  cent_encode=True
+00005410: 2c0a 2020 2020 2020 2020 2020 2020 7072  ,.            pr
+00005420: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00005430: 7465 7261 746f 723d 7072 6566 6978 5f73  terator=prefix_s
+00005440: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00005450: 720a 2020 2020 2020 2020 290a 2020 2020  r.        ).    
+00005460: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00005470: 5f74 6f5f 6469 6374 2873 656c 662e 6e61  _to_dict(self.na
+00005480: 6d65 2c20 7661 6c75 6529 0a0a 2020 2020  me, value)..    
+00005490: 6465 6620 5f5f 7365 7269 616c 697a 655f  def __serialize_
+000054a0: 7069 7065 5f64 656c 696d 6974 6564 280a  pipe_delimited(.
+000054b0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+000054c0: 2020 2020 2020 696e 5f64 6174 613a 2074        in_data: t
+000054d0: 7970 696e 672e 556e 696f 6e5b 4e6f 6e65  yping.Union[None
+000054e0: 2c20 696e 742c 2066 6c6f 6174 2c20 7374  , int, float, st
+000054f0: 722c 2062 6f6f 6c2c 2064 6963 742c 206c  r, bool, dict, l
+00005500: 6973 745d 2c0a 2020 2020 2020 2020 7072  ist],.        pr
+00005510: 6566 6978 5f73 6570 6172 6174 6f72 5f69  efix_separator_i
+00005520: 7465 7261 746f 723a 2074 7970 696e 672e  terator: typing.
+00005530: 4f70 7469 6f6e 616c 5b50 7265 6669 7853  Optional[PrefixS
+00005540: 6570 6172 6174 6f72 4974 6572 6174 6f72  eparatorIterator
+00005550: 5d0a 2020 2020 2920 2d3e 2074 7970 696e  ].    ) -> typin
+00005560: 672e 4469 6374 5b73 7472 2c20 7374 725d  g.Dict[str, str]
+00005570: 3a0a 2020 2020 2020 2020 6966 2070 7265  :.        if pre
+00005580: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+00005590: 6572 6174 6f72 2069 7320 4e6f 6e65 3a0a  erator is None:.
+000055a0: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+000055b0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+000055c0: 7261 746f 7220 3d20 7365 6c66 2e67 6574  rator = self.get
+000055d0: 5f70 7265 6669 785f 7365 7061 7261 746f  _prefix_separato
+000055e0: 725f 6974 6572 6174 6f72 2829 0a20 2020  r_iterator().   
+000055f0: 2020 2020 2076 616c 7565 203d 2073 656c       value = sel
+00005600: 662e 5f72 6566 3635 3730 5f65 7870 616e  f._ref6570_expan
+00005610: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+00005620: 2020 7661 7269 6162 6c65 5f6e 616d 653d    variable_name=
+00005630: 7365 6c66 2e6e 616d 652c 0a20 2020 2020  self.name,.     
+00005640: 2020 2020 2020 2069 6e5f 6461 7461 3d69         in_data=i
+00005650: 6e5f 6461 7461 2c0a 2020 2020 2020 2020  n_data,.        
+00005660: 2020 2020 6578 706c 6f64 653d 7365 6c66      explode=self
+00005670: 2e65 7870 6c6f 6465 2c0a 2020 2020 2020  .explode,.      
+00005680: 2020 2020 2020 7065 7263 656e 745f 656e        percent_en
+00005690: 636f 6465 3d54 7275 652c 0a20 2020 2020  code=True,.     
+000056a0: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+000056b0: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+000056c0: 3d70 7265 6669 785f 7365 7061 7261 746f  =prefix_separato
+000056d0: 725f 6974 6572 6174 6f72 0a20 2020 2020  r_iterator.     
+000056e0: 2020 2029 0a20 2020 2020 2020 2072 6574     ).        ret
+000056f0: 7572 6e20 7365 6c66 2e5f 746f 5f64 6963  urn self._to_dic
+00005700: 7428 7365 6c66 2e6e 616d 652c 2076 616c  t(self.name, val
+00005710: 7565 290a 0a20 2020 2064 6566 205f 5f73  ue)..    def __s
+00005720: 6572 6961 6c69 7a65 5f66 6f72 6d28 0a20  erialize_form(. 
+00005730: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00005740: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
+00005750: 7069 6e67 2e55 6e69 6f6e 5b4e 6f6e 652c  ping.Union[None,
+00005760: 2069 6e74 2c20 666c 6f61 742c 2073 7472   int, float, str
+00005770: 2c20 626f 6f6c 2c20 6469 6374 2c20 6c69  , bool, dict, li
+00005780: 7374 5d2c 0a20 2020 2020 2020 2070 7265  st],.        pre
+00005790: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+000057a0: 6572 6174 6f72 3a20 7479 7069 6e67 2e4f  erator: typing.O
+000057b0: 7074 696f 6e61 6c5b 5072 6566 6978 5365  ptional[PrefixSe
+000057c0: 7061 7261 746f 7249 7465 7261 746f 725d  paratorIterator]
+000057d0: 0a20 2020 2029 202d 3e20 7479 7069 6e67  .    ) -> typing
+000057e0: 2e44 6963 745b 7374 722c 2073 7472 5d3a  .Dict[str, str]:
+000057f0: 0a20 2020 2020 2020 2069 6620 7072 6566  .        if pref
+00005800: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00005810: 7261 746f 7220 6973 204e 6f6e 653a 0a20  rator is None:. 
+00005820: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+00005830: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
+00005840: 6174 6f72 203d 2073 656c 662e 6765 745f  ator = self.get_
+00005850: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00005860: 5f69 7465 7261 746f 7228 290a 2020 2020  _iterator().    
+00005870: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+00005880: 2e5f 7365 7269 616c 697a 655f 666f 726d  ._serialize_form
+00005890: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+000058a0: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
+000058b0: 2020 206e 616d 653d 7365 6c66 2e6e 616d     name=self.nam
+000058c0: 652c 0a20 2020 2020 2020 2020 2020 2065  e,.            e
+000058d0: 7870 6c6f 6465 3d73 656c 662e 6578 706c  xplode=self.expl
+000058e0: 6f64 652c 0a20 2020 2020 2020 2020 2020  ode,.           
+000058f0: 2070 6572 6365 6e74 5f65 6e63 6f64 653d   percent_encode=
+00005900: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00005910: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+00005920: 6f72 5f69 7465 7261 746f 723d 7072 6566  or_iterator=pref
+00005930: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+00005940: 7261 746f 720a 2020 2020 2020 2020 290a  rator.        ).
+00005950: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005960: 656c 662e 5f74 6f5f 6469 6374 2873 656c  elf._to_dict(sel
+00005970: 662e 6e61 6d65 2c20 7661 6c75 6529 0a0a  f.name, value)..
+00005980: 2020 2020 6465 6620 6765 745f 7072 6566      def get_pref
+00005990: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+000059a0: 7261 746f 7228 7365 6c66 2920 2d3e 2074  rator(self) -> t
+000059b0: 7970 696e 672e 4f70 7469 6f6e 616c 5b50  yping.Optional[P
+000059c0: 7265 6669 7853 6570 6172 6174 6f72 4974  refixSeparatorIt
+000059d0: 6572 6174 6f72 5d3a 0a20 2020 2020 2020  erator]:.       
+000059e0: 2069 6620 7365 6c66 2e73 7479 6c65 2069   if self.style i
+000059f0: 7320 5061 7261 6d65 7465 7253 7479 6c65  s ParameterStyle
+00005a00: 2e46 4f52 4d3a 0a20 2020 2020 2020 2020  .FORM:.         
+00005a10: 2020 2072 6574 7572 6e20 5072 6566 6978     return Prefix
+00005a20: 5365 7061 7261 746f 7249 7465 7261 746f  SeparatorIterato
+00005a30: 7228 273f 272c 2027 2627 290a 2020 2020  r('?', '&').    
+00005a40: 2020 2020 656c 6966 2073 656c 662e 7374      elif self.st
+00005a50: 796c 6520 6973 2050 6172 616d 6574 6572  yle is Parameter
+00005a60: 5374 796c 652e 5350 4143 455f 4445 4c49  Style.SPACE_DELI
+00005a70: 4d49 5445 443a 0a20 2020 2020 2020 2020  MITED:.         
+00005a80: 2020 2072 6574 7572 6e20 5072 6566 6978     return Prefix
+00005a90: 5365 7061 7261 746f 7249 7465 7261 746f  SeparatorIterato
+00005aa0: 7228 2727 2c20 2725 3230 2729 0a20 2020  r('', '%20').   
+00005ab0: 2020 2020 2065 6c69 6620 7365 6c66 2e73       elif self.s
+00005ac0: 7479 6c65 2069 7320 5061 7261 6d65 7465  tyle is Paramete
+00005ad0: 7253 7479 6c65 2e50 4950 455f 4445 4c49  rStyle.PIPE_DELI
+00005ae0: 4d49 5445 443a 0a20 2020 2020 2020 2020  MITED:.         
+00005af0: 2020 2072 6574 7572 6e20 5072 6566 6978     return Prefix
+00005b00: 5365 7061 7261 746f 7249 7465 7261 746f  SeparatorIterato
+00005b10: 7228 2727 2c20 277c 2729 0a0a 2020 2020  r('', '|')..    
+00005b20: 6465 6620 7365 7269 616c 697a 6528 0a20  def serialize(. 
+00005b30: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00005b40: 2020 2020 2069 6e5f 6461 7461 3a20 7479       in_data: ty
+00005b50: 7069 6e67 2e55 6e69 6f6e 5b0a 2020 2020  ping.Union[.    
+00005b60: 2020 2020 2020 2020 5363 6865 6d61 2c20          Schema, 
+00005b70: 4465 6369 6d61 6c2c 2069 6e74 2c20 666c  Decimal, int, fl
+00005b80: 6f61 742c 2073 7472 2c20 6461 7465 2c20  oat, str, date, 
+00005b90: 6461 7465 7469 6d65 2c20 4e6f 6e65 2c20  datetime, None, 
+00005ba0: 626f 6f6c 2c20 6c69 7374 2c20 7475 706c  bool, list, tupl
+00005bb0: 652c 2064 6963 742c 2066 726f 7a65 6e64  e, dict, frozend
+00005bc0: 6963 742e 6672 6f7a 656e 6469 6374 5d2c  ict.frozendict],
+00005bd0: 0a20 2020 2020 2020 2070 7265 6669 785f  .        prefix_
+00005be0: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+00005bf0: 6f72 3a20 7479 7069 6e67 2e4f 7074 696f  or: typing.Optio
+00005c00: 6e61 6c5b 5072 6566 6978 5365 7061 7261  nal[PrefixSepara
+00005c10: 746f 7249 7465 7261 746f 725d 203d 204e  torIterator] = N
+00005c20: 6f6e 650a 2020 2020 2920 2d3e 2074 7970  one.    ) -> typ
+00005c30: 696e 672e 4469 6374 5b73 7472 2c20 7374  ing.Dict[str, st
+00005c40: 725d 3a0a 2020 2020 2020 2020 6966 2073  r]:.        if s
+00005c50: 656c 662e 7363 6865 6d61 3a0a 2020 2020  elf.schema:.    
+00005c60: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+00005c70: 6461 7461 203d 2073 656c 662e 7363 6865  data = self.sche
+00005c80: 6d61 2869 6e5f 6461 7461 290a 2020 2020  ma(in_data).    
+00005c90: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+00005ca0: 6461 7461 203d 2073 656c 662e 5f6a 736f  data = self._jso
+00005cb0: 6e5f 656e 636f 6465 722e 6465 6661 756c  n_encoder.defaul
+00005cc0: 7428 6361 7374 5f69 6e5f 6461 7461 290a  t(cast_in_data).
+00005cd0: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00005ce0: 2020 2020 2020 2020 2020 2020 666f 726d              form
+00005cf0: 202d 3e20 7175 6572 790a 2020 2020 2020   -> query.      
+00005d00: 2020 2020 2020 2020 2020 7175 6572 793a            query:
+00005d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005d20: 2020 2020 202d 2047 4554 2f48 4541 442f       - GET/HEAD/
+00005d30: 4445 4c45 5445 3a20 636f 756c 6420 7573  DELETE: could us
+00005d40: 6520 6669 656c 6473 0a20 2020 2020 2020  e fields.       
+00005d50: 2020 2020 2020 2020 2020 2020 202d 2050               - P
+00005d60: 5554 2f50 4f53 543a 206d 7573 7420 7573  UT/POST: must us
+00005d70: 6520 7572 6c65 6e63 6f64 6520 746f 2073  e urlencode to s
+00005d80: 656e 6420 7061 7261 6d65 7465 7273 0a20  end parameters. 
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2072 6574 7572 6e73 2066 6965 6c64     returns field
+00005db0: 733a 2074 7570 6c65 0a20 2020 2020 2020  s: tuple.       
+00005dc0: 2020 2020 2073 7061 6365 4465 6c69 6d69       spaceDelimi
+00005dd0: 7465 6420 2d3e 2071 7565 7279 0a20 2020  ted -> query.   
+00005de0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00005df0: 7572 6e73 2066 6965 6c64 730a 2020 2020  urns fields.    
+00005e00: 2020 2020 2020 2020 7069 7065 4465 6c69          pipeDeli
+00005e10: 6d69 7465 6420 2d3e 2071 7565 7279 0a20  mited -> query. 
+00005e20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00005e30: 6574 7572 6e73 2066 6965 6c64 730a 2020  eturns fields.  
+00005e40: 2020 2020 2020 2020 2020 6465 6570 4f62            deepOb
+00005e50: 6a65 6374 202d 3e20 7175 6572 792c 2068  ject -> query, h
+00005e60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00005e70: 6d2f 4f41 492f 4f70 656e 4150 492d 5370  m/OAI/OpenAPI-Sp
+00005e80: 6563 6966 6963 6174 696f 6e2f 6973 7375  ecification/issu
+00005e90: 6573 2f31 3730 360a 2020 2020 2020 2020  es/1706.        
+00005ea0: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+00005eb0: 6669 656c 6473 0a20 2020 2020 2020 2020  fields.         
+00005ec0: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
+00005ed0: 2020 2069 6620 7365 6c66 2e73 7479 6c65     if self.style
+00005ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005ef0: 2020 2320 544f 444f 2075 7064 6174 6520    # TODO update 
+00005f00: 7175 6572 7920 6f6e 6573 2074 6f20 6f6d  query ones to om
+00005f10: 6974 2073 6574 7469 6e67 2076 616c 7565  it setting value
+00005f20: 7320 7768 656e 205b 5d20 7b7d 206f 7220  s when [] {} or 
+00005f30: 4e6f 6e65 2069 7320 696e 7075 740a 2020  None is input.  
+00005f40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005f50: 2073 656c 662e 7374 796c 6520 6973 2050   self.style is P
+00005f60: 6172 616d 6574 6572 5374 796c 652e 464f  arameterStyle.FO
+00005f70: 524d 3a0a 2020 2020 2020 2020 2020 2020  RM:.            
+00005f80: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005f90: 656c 662e 5f5f 7365 7269 616c 697a 655f  elf.__serialize_
+00005fa0: 666f 726d 2863 6173 745f 696e 5f64 6174  form(cast_in_dat
+00005fb0: 612c 2070 7265 6669 785f 7365 7061 7261  a, prefix_separa
+00005fc0: 746f 725f 6974 6572 6174 6f72 290a 2020  tor_iterator).  
+00005fd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005fe0: 6966 2073 656c 662e 7374 796c 6520 6973  if self.style is
+00005ff0: 2050 6172 616d 6574 6572 5374 796c 652e   ParameterStyle.
+00006000: 5350 4143 455f 4445 4c49 4d49 5445 443a  SPACE_DELIMITED:
+00006010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006020: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00006030: 2e5f 5f73 6572 6961 6c69 7a65 5f73 7061  .__serialize_spa
+00006040: 6365 5f64 656c 696d 6974 6564 2863 6173  ce_delimited(cas
+00006050: 745f 696e 5f64 6174 612c 2070 7265 6669  t_in_data, prefi
+00006060: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
+00006070: 6174 6f72 290a 2020 2020 2020 2020 2020  ator).          
+00006080: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00006090: 7374 796c 6520 6973 2050 6172 616d 6574  style is Paramet
+000060a0: 6572 5374 796c 652e 5049 5045 5f44 454c  erStyle.PIPE_DEL
+000060b0: 494d 4954 4544 3a0a 2020 2020 2020 2020  IMITED:.        
+000060c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000060d0: 726e 2073 656c 662e 5f5f 7365 7269 616c  rn self.__serial
+000060e0: 697a 655f 7069 7065 5f64 656c 696d 6974  ize_pipe_delimit
+000060f0: 6564 2863 6173 745f 696e 5f64 6174 612c  ed(cast_in_data,
+00006100: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
+00006110: 725f 6974 6572 6174 6f72 290a 2020 2020  r_iterator).    
+00006120: 2020 2020 2320 7365 6c66 2e63 6f6e 7465      # self.conte
+00006130: 6e74 2077 696c 6c20 6265 206c 656e 6774  nt will be lengt
+00006140: 6820 6f6e 650a 2020 2020 2020 2020 6966  h one.        if
+00006150: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
+00006160: 725f 6974 6572 6174 6f72 2069 7320 4e6f  r_iterator is No
+00006170: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00006180: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+00006190: 5f69 7465 7261 746f 7220 3d20 7365 6c66  _iterator = self
+000061a0: 2e67 6574 5f70 7265 6669 785f 7365 7061  .get_prefix_sepa
+000061b0: 7261 746f 725f 6974 6572 6174 6f72 2829  rator_iterator()
+000061c0: 0a20 2020 2020 2020 2066 6f72 2063 6f6e  .        for con
+000061d0: 7465 6e74 5f74 7970 652c 2073 6368 656d  tent_type, schem
+000061e0: 6120 696e 2073 656c 662e 636f 6e74 656e  a in self.conten
+000061f0: 742e 6974 656d 7328 293a 0a20 2020 2020  t.items():.     
+00006200: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
+00006210: 6174 6120 3d20 7363 6865 6d61 2869 6e5f  ata = schema(in_
+00006220: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+00006230: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
+00006240: 2073 656c 662e 5f6a 736f 6e5f 656e 636f   self._json_enco
+00006250: 6465 722e 6465 6661 756c 7428 6361 7374  der.default(cast
+00006260: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
+00006270: 2020 2020 2020 6966 2073 656c 662e 5f63        if self._c
+00006280: 6f6e 7465 6e74 5f74 7970 655f 6973 5f6a  ontent_type_is_j
+00006290: 736f 6e28 636f 6e74 656e 745f 7479 7065  son(content_type
+000062a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000062b0: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
+000062c0: 5f73 6572 6961 6c69 7a65 5f6a 736f 6e28  _serialize_json(
+000062d0: 6361 7374 5f69 6e5f 6461 7461 2c20 656c  cast_in_data, el
+000062e0: 696d 696e 6174 655f 7768 6974 6573 7061  iminate_whitespa
+000062f0: 6365 3d54 7275 6529 0a20 2020 2020 2020  ce=True).       
+00006300: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00006310: 7365 6c66 2e5f 746f 5f64 6963 7428 0a20  self._to_dict(. 
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2073 656c 662e 6e61 6d65 2c0a 2020     self.name,.  
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 2020 6e65 7874 2870 7265 6669 785f 7365    next(prefix_se
+00006360: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+00006370: 2920 2b20 7365 6c66 2e6e 616d 6520 2b20  ) + self.name + 
+00006380: 273d 2720 2b20 7175 6f74 6528 7661 6c75  '=' + quote(valu
+00006390: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+000063a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000063b0: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
+000063c0: 656e 7465 6445 7272 6f72 2827 5365 7269  entedError('Seri
+000063d0: 616c 697a 6174 696f 6e20 6f66 207b 7d20  alization of {} 
+000063e0: 6861 7320 6e6f 7420 7965 7420 6265 656e  has not yet been
+000063f0: 2069 6d70 6c65 6d65 6e74 6564 272e 666f   implemented'.fo
+00006400: 726d 6174 2863 6f6e 7465 6e74 5f74 7970  rmat(content_typ
+00006410: 6529 290a 0a0a 636c 6173 7320 436f 6f6b  e))...class Cook
+00006420: 6965 5061 7261 6d65 7465 7228 5061 7261  ieParameter(Para
+00006430: 6d65 7465 7242 6173 652c 2053 7479 6c65  meterBase, Style
+00006440: 466f 726d 5365 7269 616c 697a 6572 293a  FormSerializer):
+00006450: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00006460: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+00006470: 2c0a 2020 2020 2020 2020 6e61 6d65 3a20  ,.        name: 
+00006480: 7374 722c 0a20 2020 2020 2020 2072 6571  str,.        req
+00006490: 7569 7265 643a 2062 6f6f 6c20 3d20 4661  uired: bool = Fa
+000064a0: 6c73 652c 0a20 2020 2020 2020 2073 7479  lse,.        sty
+000064b0: 6c65 3a20 7479 7069 6e67 2e4f 7074 696f  le: typing.Optio
+000064c0: 6e61 6c5b 5061 7261 6d65 7465 7253 7479  nal[ParameterSty
+000064d0: 6c65 5d20 3d20 4e6f 6e65 2c0a 2020 2020  le] = None,.    
+000064e0: 2020 2020 6578 706c 6f64 653a 2074 7970      explode: typ
+000064f0: 696e 672e 4f70 7469 6f6e 616c 5b62 6f6f  ing.Optional[boo
+00006500: 6c5d 203d 204e 6f6e 652c 0a20 2020 2020  l] = None,.     
+00006510: 2020 2061 6c6c 6f77 5f72 6573 6572 7665     allow_reserve
+00006520: 643a 2074 7970 696e 672e 4f70 7469 6f6e  d: typing.Option
+00006530: 616c 5b62 6f6f 6c5d 203d 204e 6f6e 652c  al[bool] = None,
+00006540: 0a20 2020 2020 2020 2073 6368 656d 613a  .        schema:
+00006550: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00006560: 5b74 7970 696e 672e 5479 7065 5b53 6368  [typing.Type[Sch
+00006570: 656d 615d 5d20 3d20 4e6f 6e65 2c0a 2020  ema]] = None,.  
+00006580: 2020 2020 2020 636f 6e74 656e 743a 2074        content: t
+00006590: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+000065a0: 7970 696e 672e 4469 6374 5b73 7472 2c20  yping.Dict[str, 
+000065b0: 7479 7069 6e67 2e54 7970 655b 5363 6865  typing.Type[Sche
+000065c0: 6d61 5d5d 5d20 3d20 4e6f 6e65 0a20 2020  ma]]] = None.   
+000065d0: 2029 3a0a 2020 2020 2020 2020 7573 6564   ):.        used
+000065e0: 5f73 7479 6c65 203d 2050 6172 616d 6574  _style = Paramet
+000065f0: 6572 5374 796c 652e 464f 524d 2069 6620  erStyle.FORM if 
+00006600: 7374 796c 6520 6973 204e 6f6e 6520 616e  style is None an
+00006610: 6420 636f 6e74 656e 7420 6973 204e 6f6e  d content is Non
+00006620: 6520 616e 6420 7363 6865 6d61 2065 6c73  e and schema els
+00006630: 6520 7374 796c 650a 2020 2020 2020 2020  e style.        
+00006640: 7573 6564 5f65 7870 6c6f 6465 203d 2073  used_explode = s
+00006650: 656c 662e 5f67 6574 5f64 6566 6175 6c74  elf._get_default
+00006660: 5f65 7870 6c6f 6465 2875 7365 645f 7374  _explode(used_st
+00006670: 796c 6529 2069 6620 6578 706c 6f64 6520  yle) if explode 
+00006680: 6973 204e 6f6e 6520 656c 7365 2065 7870  is None else exp
+00006690: 6c6f 6465 0a0a 2020 2020 2020 2020 7375  lode..        su
+000066a0: 7065 7228 292e 5f5f 696e 6974 5f5f 280a  per().__init__(.
+000066b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000066c0: 2c0a 2020 2020 2020 2020 2020 2020 696e  ,.            in
+000066d0: 5f74 7970 653d 5061 7261 6d65 7465 7249  _type=ParameterI
+000066e0: 6e54 7970 652e 434f 4f4b 4945 2c0a 2020  nType.COOKIE,.  
+000066f0: 2020 2020 2020 2020 2020 7265 7175 6972            requir
+00006700: 6564 3d72 6571 7569 7265 642c 0a20 2020  ed=required,.   
+00006710: 2020 2020 2020 2020 2073 7479 6c65 3d75           style=u
+00006720: 7365 645f 7374 796c 652c 0a20 2020 2020  sed_style,.     
+00006730: 2020 2020 2020 2065 7870 6c6f 6465 3d75         explode=u
+00006740: 7365 645f 6578 706c 6f64 652c 0a20 2020  sed_explode,.   
+00006750: 2020 2020 2020 2020 2061 6c6c 6f77 5f72           allow_r
+00006760: 6573 6572 7665 643d 616c 6c6f 775f 7265  eserved=allow_re
+00006770: 7365 7276 6564 2c0a 2020 2020 2020 2020  served,.        
+00006780: 2020 2020 7363 6865 6d61 3d73 6368 656d      schema=schem
+00006790: 612c 0a20 2020 2020 2020 2020 2020 2063  a,.            c
+000067a0: 6f6e 7465 6e74 3d63 6f6e 7465 6e74 0a20  ontent=content. 
+000067b0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+000067c0: 6620 7365 7269 616c 697a 6528 0a20 2020  f serialize(.   
+000067d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000067e0: 2020 2069 6e5f 6461 7461 3a20 7479 7069     in_data: typi
+000067f0: 6e67 2e55 6e69 6f6e 5b0a 2020 2020 2020  ng.Union[.      
+00006800: 2020 2020 2020 5363 6865 6d61 2c20 4465        Schema, De
+00006810: 6369 6d61 6c2c 2069 6e74 2c20 666c 6f61  cimal, int, floa
+00006820: 742c 2073 7472 2c20 6461 7465 2c20 6461  t, str, date, da
+00006830: 7465 7469 6d65 2c20 4e6f 6e65 2c20 626f  tetime, None, bo
+00006840: 6f6c 2c20 6c69 7374 2c20 7475 706c 652c  ol, list, tuple,
+00006850: 2064 6963 742c 2066 726f 7a65 6e64 6963   dict, frozendic
+00006860: 742e 6672 6f7a 656e 6469 6374 5d0a 2020  t.frozendict].  
+00006870: 2020 2920 2d3e 2074 7970 696e 672e 4469    ) -> typing.Di
+00006880: 6374 5b73 7472 2c20 7374 725d 3a0a 2020  ct[str, str]:.  
+00006890: 2020 2020 2020 6966 2073 656c 662e 7363        if self.sc
+000068a0: 6865 6d61 3a0a 2020 2020 2020 2020 2020  hema:.          
+000068b0: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
+000068c0: 2073 656c 662e 7363 6865 6d61 2869 6e5f   self.schema(in_
+000068d0: 6461 7461 290a 2020 2020 2020 2020 2020  data).          
+000068e0: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
+000068f0: 2073 656c 662e 5f6a 736f 6e5f 656e 636f   self._json_enco
+00006900: 6465 722e 6465 6661 756c 7428 6361 7374  der.default(cast
+00006910: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
+00006920: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00006930: 2020 2020 2020 666f 726d 202d 3e20 636f        form -> co
+00006940: 6f6b 6965 0a20 2020 2020 2020 2020 2020  okie.           
+00006950: 2020 2020 2072 6574 7572 6e73 2066 6965       returns fie
+00006960: 6c64 733a 2074 7570 6c65 0a20 2020 2020  lds: tuple.     
+00006970: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006980: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00006990: 7479 6c65 3a0a 2020 2020 2020 2020 2020  tyle:.          
+000069a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000069b0: 2020 2020 2020 2020 2020 544f 444f 2061            TODO a
+000069c0: 6464 2065 7363 6170 696e 6720 6f66 2063  dd escaping of c
+000069d0: 6f6d 6d61 2c20 7370 6163 652c 2065 7175  omma, space, equ
+000069e0: 616c 730a 2020 2020 2020 2020 2020 2020  als.            
+000069f0: 2020 2020 6f72 2074 7572 6e20 656e 636f      or turn enco
+00006a00: 6469 6e67 206f 6e0a 2020 2020 2020 2020  ding on.        
+00006a10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00006a20: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00006a30: 6520 3d20 7365 6c66 2e5f 7365 7269 616c  e = self._serial
+00006a40: 697a 655f 666f 726d 280a 2020 2020 2020  ize_form(.      
+00006a50: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00006a60: 7374 5f69 6e5f 6461 7461 2c0a 2020 2020  st_in_data,.    
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 6578 706c 6f64 653d 7365 6c66 2e65 7870  explode=self.exp
+00006a90: 6c6f 6465 2c0a 2020 2020 2020 2020 2020  lode,.          
+00006aa0: 2020 2020 2020 2020 2020 6e61 6d65 3d73            name=s
+00006ab0: 656c 662e 6e61 6d65 2c0a 2020 2020 2020  elf.name,.      
+00006ac0: 2020 2020 2020 2020 2020 2020 2020 7065                pe
+00006ad0: 7263 656e 745f 656e 636f 6465 3d46 616c  rcent_encode=Fal
+00006ae0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00006af0: 2020 2020 2020 2020 7072 6566 6978 5f73          prefix_s
+00006b00: 6570 6172 6174 6f72 5f69 7465 7261 746f  eparator_iterato
+00006b10: 723d 5072 6566 6978 5365 7061 7261 746f  r=PrefixSeparato
+00006b20: 7249 7465 7261 746f 7228 2727 2c20 2726  rIterator('', '&
+00006b30: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00006b40: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00006b50: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00006b60: 2e5f 746f 5f64 6963 7428 7365 6c66 2e6e  ._to_dict(self.n
+00006b70: 616d 652c 2076 616c 7565 290a 2020 2020  ame, value).    
+00006b80: 2020 2020 2320 7365 6c66 2e63 6f6e 7465      # self.conte
+00006b90: 6e74 2077 696c 6c20 6265 206c 656e 6774  nt will be lengt
+00006ba0: 6820 6f6e 650a 2020 2020 2020 2020 666f  h one.        fo
+00006bb0: 7220 636f 6e74 656e 745f 7479 7065 2c20  r content_type, 
+00006bc0: 7363 6865 6d61 2069 6e20 7365 6c66 2e63  schema in self.c
+00006bd0: 6f6e 7465 6e74 2e69 7465 6d73 2829 3a0a  ontent.items():.
+00006be0: 2020 2020 2020 2020 2020 2020 6361 7374              cast
+00006bf0: 5f69 6e5f 6461 7461 203d 2073 6368 656d  _in_data = schem
+00006c00: 6128 696e 5f64 6174 6129 0a20 2020 2020  a(in_data).     
+00006c10: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
+00006c20: 6174 6120 3d20 7365 6c66 2e5f 6a73 6f6e  ata = self._json
+00006c30: 5f65 6e63 6f64 6572 2e64 6566 6175 6c74  _encoder.default
+00006c40: 2863 6173 745f 696e 5f64 6174 6129 0a20  (cast_in_data). 
+00006c50: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00006c60: 6c66 2e5f 636f 6e74 656e 745f 7479 7065  lf._content_type
+00006c70: 5f69 735f 6a73 6f6e 2863 6f6e 7465 6e74  _is_json(content
+00006c80: 5f74 7970 6529 3a0a 2020 2020 2020 2020  _type):.        
+00006c90: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00006ca0: 7365 6c66 2e5f 7365 7269 616c 697a 655f  self._serialize_
+00006cb0: 6a73 6f6e 2863 6173 745f 696e 5f64 6174  json(cast_in_dat
+00006cc0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+00006cd0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
+00006ce0: 746f 5f64 6963 7428 7365 6c66 2e6e 616d  to_dict(self.nam
+00006cf0: 652c 2076 616c 7565 290a 2020 2020 2020  e, value).      
+00006d00: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+00006d10: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+00006d20: 2753 6572 6961 6c69 7a61 7469 6f6e 206f  'Serialization o
+00006d30: 6620 7b7d 2068 6173 206e 6f74 2079 6574  f {} has not yet
+00006d40: 2062 6565 6e20 696d 706c 656d 656e 7465   been implemente
+00006d50: 6427 2e66 6f72 6d61 7428 636f 6e74 656e  d'.format(conten
+00006d60: 745f 7479 7065 2929 0a0a 0a63 6c61 7373  t_type))...class
+00006d70: 2048 6561 6465 7250 6172 616d 6574 6572   HeaderParameter
+00006d80: 2850 6172 616d 6574 6572 4261 7365 2c20  (ParameterBase, 
+00006d90: 5374 796c 6553 696d 706c 6553 6572 6961  StyleSimpleSeria
+00006da0: 6c69 7a65 7229 3a0a 2020 2020 6465 6620  lizer):.    def 
+00006db0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00006dc0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00006dd0: 6e61 6d65 3a20 7374 722c 0a20 2020 2020  name: str,.     
+00006de0: 2020 2072 6571 7569 7265 643a 2062 6f6f     required: boo
+00006df0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
+00006e00: 2020 2073 7479 6c65 3a20 7479 7069 6e67     style: typing
+00006e10: 2e4f 7074 696f 6e61 6c5b 5061 7261 6d65  .Optional[Parame
+00006e20: 7465 7253 7479 6c65 5d20 3d20 4e6f 6e65  terStyle] = None
+00006e30: 2c0a 2020 2020 2020 2020 6578 706c 6f64  ,.        explod
+00006e40: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00006e50: 0a20 2020 2020 2020 2061 6c6c 6f77 5f72  .        allow_r
+00006e60: 6573 6572 7665 643a 2074 7970 696e 672e  eserved: typing.
+00006e70: 4f70 7469 6f6e 616c 5b62 6f6f 6c5d 203d  Optional[bool] =
+00006e80: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
+00006e90: 6368 656d 613a 2074 7970 696e 672e 4f70  chema: typing.Op
+00006ea0: 7469 6f6e 616c 5b74 7970 696e 672e 5479  tional[typing.Ty
+00006eb0: 7065 5b53 6368 656d 615d 5d20 3d20 4e6f  pe[Schema]] = No
+00006ec0: 6e65 2c0a 2020 2020 2020 2020 636f 6e74  ne,.        cont
+00006ed0: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
+00006ee0: 6f6e 616c 5b74 7970 696e 672e 4469 6374  onal[typing.Dict
+00006ef0: 5b73 7472 2c20 7479 7069 6e67 2e54 7970  [str, typing.Typ
+00006f00: 655b 5363 6865 6d61 5d5d 5d20 3d20 4e6f  e[Schema]]] = No
+00006f10: 6e65 0a20 2020 2029 3a0a 2020 2020 2020  ne.    ):.      
+00006f20: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+00006f30: 5f5f 280a 2020 2020 2020 2020 2020 2020  __(.            
+00006f40: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00006f50: 2020 696e 5f74 7970 653d 5061 7261 6d65    in_type=Parame
+00006f60: 7465 7249 6e54 7970 652e 4845 4144 4552  terInType.HEADER
+00006f70: 2c0a 2020 2020 2020 2020 2020 2020 7265  ,.            re
+00006f80: 7175 6972 6564 3d72 6571 7569 7265 642c  quired=required,
+00006f90: 0a20 2020 2020 2020 2020 2020 2073 7479  .            sty
+00006fa0: 6c65 3d73 7479 6c65 2c0a 2020 2020 2020  le=style,.      
+00006fb0: 2020 2020 2020 6578 706c 6f64 653d 6578        explode=ex
+00006fc0: 706c 6f64 652c 0a20 2020 2020 2020 2020  plode,.         
+00006fd0: 2020 2061 6c6c 6f77 5f72 6573 6572 7665     allow_reserve
+00006fe0: 643d 616c 6c6f 775f 7265 7365 7276 6564  d=allow_reserved
+00006ff0: 2c0a 2020 2020 2020 2020 2020 2020 7363  ,.            sc
+00007000: 6865 6d61 3d73 6368 656d 612c 0a20 2020  hema=schema,.   
+00007010: 2020 2020 2020 2020 2063 6f6e 7465 6e74           content
+00007020: 3d63 6f6e 7465 6e74 0a20 2020 2020 2020  =content.       
+00007030: 2029 0a0a 2020 2020 4073 7461 7469 636d   )..    @staticm
+00007040: 6574 686f 640a 2020 2020 6465 6620 5f5f  ethod.    def __
+00007050: 746f 5f68 6561 6465 7273 2869 6e5f 6461  to_headers(in_da
+00007060: 7461 3a20 7479 7069 6e67 2e54 7570 6c65  ta: typing.Tuple
+00007070: 5b74 7970 696e 672e 5475 706c 655b 7374  [typing.Tuple[st
+00007080: 722c 2073 7472 5d2c 202e 2e2e 5d29 202d  r, str], ...]) -
+00007090: 3e20 4854 5450 4865 6164 6572 4469 6374  > HTTPHeaderDict
+000070a0: 3a0a 2020 2020 2020 2020 6461 7461 203d  :.        data =
+000070b0: 2074 7570 6c65 2874 2066 6f72 2074 2069   tuple(t for t i
+000070c0: 6e20 696e 5f64 6174 6120 6966 2074 290a  n in_data if t).
+000070d0: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
+000070e0: 3d20 4854 5450 4865 6164 6572 4469 6374  = HTTPHeaderDict
+000070f0: 2829 0a20 2020 2020 2020 2069 6620 6e6f  ().        if no
+00007100: 7420 6461 7461 3a0a 2020 2020 2020 2020  t data:.        
+00007110: 2020 2020 7265 7475 726e 2068 6561 6465      return heade
+00007120: 7273 0a20 2020 2020 2020 2068 6561 6465  rs.        heade
+00007130: 7273 2e65 7874 656e 6428 6461 7461 290a  rs.extend(data).
+00007140: 2020 2020 2020 2020 7265 7475 726e 2068          return h
+00007150: 6561 6465 7273 0a0a 2020 2020 6465 6620  eaders..    def 
+00007160: 7365 7269 616c 697a 6528 0a20 2020 2020  serialize(.     
+00007170: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00007180: 2069 6e5f 6461 7461 3a20 7479 7069 6e67   in_data: typing
+00007190: 2e55 6e69 6f6e 5b0a 2020 2020 2020 2020  .Union[.        
+000071a0: 2020 2020 5363 6865 6d61 2c20 4465 6369      Schema, Deci
+000071b0: 6d61 6c2c 2069 6e74 2c20 666c 6f61 742c  mal, int, float,
+000071c0: 2073 7472 2c20 6461 7465 2c20 6461 7465   str, date, date
+000071d0: 7469 6d65 2c20 4e6f 6e65 2c20 626f 6f6c  time, None, bool
+000071e0: 2c20 6c69 7374 2c20 7475 706c 652c 2064  , list, tuple, d
+000071f0: 6963 742c 2066 726f 7a65 6e64 6963 742e  ict, frozendict.
+00007200: 6672 6f7a 656e 6469 6374 5d0a 2020 2020  frozendict].    
+00007210: 2920 2d3e 2048 5454 5048 6561 6465 7244  ) -> HTTPHeaderD
+00007220: 6963 743a 0a20 2020 2020 2020 2069 6620  ict:.        if 
+00007230: 7365 6c66 2e73 6368 656d 613a 0a20 2020  self.schema:.   
+00007240: 2020 2020 2020 2020 2063 6173 745f 696e           cast_in
+00007250: 5f64 6174 6120 3d20 7365 6c66 2e73 6368  _data = self.sch
+00007260: 656d 6128 696e 5f64 6174 6129 0a20 2020  ema(in_data).   
+00007270: 2020 2020 2020 2020 2063 6173 745f 696e           cast_in
+00007280: 5f64 6174 6120 3d20 7365 6c66 2e5f 6a73  _data = self._js
+00007290: 6f6e 5f65 6e63 6f64 6572 2e64 6566 6175  on_encoder.defau
+000072a0: 6c74 2863 6173 745f 696e 5f64 6174 6129  lt(cast_in_data)
+000072b0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+000072c0: 0a20 2020 2020 2020 2020 2020 2073 696d  .            sim
+000072d0: 706c 6520 2d3e 2068 6561 6465 720a 2020  ple -> header.  
+000072e0: 2020 2020 2020 2020 2020 2020 2020 6865                he
+000072f0: 6164 6572 733a 2050 6f6f 6c4d 616e 6167  aders: PoolManag
+00007300: 6572 206e 6565 6473 2061 206d 6170 7069  er needs a mappi
+00007310: 6e67 2c20 7475 706c 6520 6973 2063 6c6f  ng, tuple is clo
+00007320: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+00007330: 2020 2020 2020 2072 6574 7572 6e73 2068         returns h
+00007340: 6561 6465 7273 3a20 6469 6374 0a20 2020  eaders: dict.   
+00007350: 2020 2020 2020 2020 2022 2222 0a20 2020           """.   
+00007360: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00007370: 2e73 7479 6c65 3a0a 2020 2020 2020 2020  .style:.        
+00007380: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+00007390: 7365 6c66 2e5f 7365 7269 616c 697a 655f  self._serialize_
+000073a0: 7369 6d70 6c65 2863 6173 745f 696e 5f64  simple(cast_in_d
+000073b0: 6174 612c 2073 656c 662e 6e61 6d65 2c20  ata, self.name, 
+000073c0: 7365 6c66 2e65 7870 6c6f 6465 2c20 4661  self.explode, Fa
+000073d0: 6c73 6529 0a20 2020 2020 2020 2020 2020  lse).           
+000073e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000073f0: 2e5f 5f74 6f5f 6865 6164 6572 7328 2828  .__to_headers(((
+00007400: 7365 6c66 2e6e 616d 652c 2076 616c 7565  self.name, value
+00007410: 292c 2929 0a20 2020 2020 2020 2023 2073  ),)).        # s
+00007420: 656c 662e 636f 6e74 656e 7420 7769 6c6c  elf.content will
+00007430: 2062 6520 6c65 6e67 7468 206f 6e65 0a20   be length one. 
+00007440: 2020 2020 2020 2066 6f72 2063 6f6e 7465         for conte
+00007450: 6e74 5f74 7970 652c 2073 6368 656d 6120  nt_type, schema 
+00007460: 696e 2073 656c 662e 636f 6e74 656e 742e  in self.content.
+00007470: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00007480: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
+00007490: 6120 3d20 7363 6865 6d61 2869 6e5f 6461  a = schema(in_da
+000074a0: 7461 290a 2020 2020 2020 2020 2020 2020  ta).            
+000074b0: 6361 7374 5f69 6e5f 6461 7461 203d 2073  cast_in_data = s
+000074c0: 656c 662e 5f6a 736f 6e5f 656e 636f 6465  elf._json_encode
+000074d0: 722e 6465 6661 756c 7428 6361 7374 5f69  r.default(cast_i
+000074e0: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+000074f0: 2020 2020 6966 2073 656c 662e 5f63 6f6e      if self._con
+00007500: 7465 6e74 5f74 7970 655f 6973 5f6a 736f  tent_type_is_jso
+00007510: 6e28 636f 6e74 656e 745f 7479 7065 293a  n(content_type):
+00007520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007530: 2076 616c 7565 203d 2073 656c 662e 5f73   value = self._s
+00007540: 6572 6961 6c69 7a65 5f6a 736f 6e28 6361  erialize_json(ca
+00007550: 7374 5f69 6e5f 6461 7461 290a 2020 2020  st_in_data).    
+00007560: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00007570: 726e 2073 656c 662e 5f5f 746f 5f68 6561  rn self.__to_hea
+00007580: 6465 7273 2828 2873 656c 662e 6e61 6d65  ders(((self.name
+00007590: 2c20 7661 6c75 6529 2c29 290a 2020 2020  , value),)).    
+000075a0: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
+000075b0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+000075c0: 7228 2753 6572 6961 6c69 7a61 7469 6f6e  r('Serialization
+000075d0: 206f 6620 7b7d 2068 6173 206e 6f74 2079   of {} has not y
+000075e0: 6574 2062 6565 6e20 696d 706c 656d 656e  et been implemen
+000075f0: 7465 6427 2e66 6f72 6d61 7428 636f 6e74  ted'.format(cont
+00007600: 656e 745f 7479 7065 2929 0a0a 0a63 6c61  ent_type))...cla
+00007610: 7373 2045 6e63 6f64 696e 673a 0a20 2020  ss Encoding:.   
+00007620: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
+00007630: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+00007640: 2020 2020 2063 6f6e 7465 6e74 5f74 7970       content_typ
+00007650: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+00007660: 6865 6164 6572 733a 2074 7970 696e 672e  headers: typing.
+00007670: 4f70 7469 6f6e 616c 5b74 7970 696e 672e  Optional[typing.
+00007680: 4469 6374 5b73 7472 2c20 4865 6164 6572  Dict[str, Header
+00007690: 5061 7261 6d65 7465 725d 5d20 3d20 4e6f  Parameter]] = No
+000076a0: 6e65 2c0a 2020 2020 2020 2020 7374 796c  ne,.        styl
+000076b0: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
+000076c0: 616c 5b50 6172 616d 6574 6572 5374 796c  al[ParameterStyl
+000076d0: 655d 203d 204e 6f6e 652c 0a20 2020 2020  e] = None,.     
+000076e0: 2020 2065 7870 6c6f 6465 3a20 626f 6f6c     explode: bool
+000076f0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+00007700: 2020 616c 6c6f 775f 7265 7365 7276 6564    allow_reserved
+00007710: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+00007720: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+00007730: 656c 662e 636f 6e74 656e 745f 7479 7065  elf.content_type
+00007740: 203d 2063 6f6e 7465 6e74 5f74 7970 650a   = content_type.
+00007750: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+00007760: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+00007770: 2020 2020 2020 2073 656c 662e 7374 796c         self.styl
+00007780: 6520 3d20 7374 796c 650a 2020 2020 2020  e = style.      
+00007790: 2020 7365 6c66 2e65 7870 6c6f 6465 203d    self.explode =
+000077a0: 2065 7870 6c6f 6465 0a20 2020 2020 2020   explode.       
+000077b0: 2073 656c 662e 616c 6c6f 775f 7265 7365   self.allow_rese
+000077c0: 7276 6564 203d 2061 6c6c 6f77 5f72 6573  rved = allow_res
+000077d0: 6572 7665 640a 0a0a 4064 6174 6163 6c61  erved...@datacla
+000077e0: 7373 0a63 6c61 7373 204d 6564 6961 5479  ss.class MediaTy
+000077f0: 7065 3a0a 2020 2020 2222 220a 2020 2020  pe:.    """.    
+00007800: 5573 6564 2074 6f20 7374 6f72 6520 7265  Used to store re
+00007810: 7175 6573 7420 616e 6420 7265 7370 6f6e  quest and respon
+00007820: 7365 2062 6f64 7920 7363 6865 6d61 2069  se body schema i
+00007830: 6e66 6f72 6d61 7469 6f6e 0a20 2020 2065  nformation.    e
+00007840: 6e63 6f64 696e 673a 0a20 2020 2020 2020  ncoding:.       
+00007850: 2041 206d 6170 2062 6574 7765 656e 2061   A map between a
+00007860: 2070 726f 7065 7274 7920 6e61 6d65 2061   property name a
+00007870: 6e64 2069 7473 2065 6e63 6f64 696e 6720  nd its encoding 
+00007880: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
+00007890: 2020 2020 2054 6865 206b 6579 2c20 6265       The key, be
+000078a0: 696e 6720 7468 6520 7072 6f70 6572 7479  ing the property
+000078b0: 206e 616d 652c 204d 5553 5420 6578 6973   name, MUST exis
+000078c0: 7420 696e 2074 6865 2073 6368 656d 6120  t in the schema 
+000078d0: 6173 2061 2070 726f 7065 7274 792e 0a20  as a property.. 
+000078e0: 2020 2020 2020 2054 6865 2065 6e63 6f64         The encod
+000078f0: 696e 6720 6f62 6a65 6374 2053 4841 4c4c  ing object SHALL
+00007900: 206f 6e6c 7920 6170 706c 7920 746f 2072   only apply to r
+00007910: 6571 7565 7374 426f 6479 206f 626a 6563  equestBody objec
+00007920: 7473 2077 6865 6e20 7468 6520 6d65 6469  ts when the medi
+00007930: 6120 7479 7065 2069 730a 2020 2020 2020  a type is.      
+00007940: 2020 6d75 6c74 6970 6172 7420 6f72 2061    multipart or a
+00007950: 7070 6c69 6361 7469 6f6e 2f78 2d77 7777  pplication/x-www
+00007960: 2d66 6f72 6d2d 7572 6c65 6e63 6f64 6564  -form-urlencoded
+00007970: 2e0a 2020 2020 2222 220a 2020 2020 7363  ..    """.    sc
+00007980: 6865 6d61 3a20 7479 7069 6e67 2e4f 7074  hema: typing.Opt
+00007990: 696f 6e61 6c5b 7479 7069 6e67 2e54 7970  ional[typing.Typ
+000079a0: 655b 5363 6865 6d61 5d5d 203d 204e 6f6e  e[Schema]] = Non
+000079b0: 650a 2020 2020 656e 636f 6469 6e67 3a20  e.    encoding: 
+000079c0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+000079d0: 7479 7069 6e67 2e44 6963 745b 7374 722c  typing.Dict[str,
+000079e0: 2045 6e63 6f64 696e 675d 5d20 3d20 4e6f   Encoding]] = No
+000079f0: 6e65 0a0a 0a40 6461 7461 636c 6173 730a  ne...@dataclass.
+00007a00: 636c 6173 7320 4170 6952 6573 706f 6e73  class ApiRespons
+00007a10: 6557 6974 686f 7574 4465 7365 7269 616c  eWithoutDeserial
+00007a20: 697a 6174 696f 6e28 4170 6952 6573 706f  ization(ApiRespo
+00007a30: 6e73 6529 3a0a 2020 2020 7061 7373 0a0a  nse):.    pass..
+00007a40: 4064 6174 6163 6c61 7373 0a63 6c61 7373  @dataclass.class
+00007a50: 2041 7069 5265 7370 6f6e 7365 5769 7468   ApiResponseWith
+00007a60: 6f75 7444 6573 6572 6961 6c69 7a61 7469  outDeserializati
+00007a70: 6f6e 4173 796e 6328 4173 796e 6341 7069  onAsync(AsyncApi
+00007a80: 5265 7370 6f6e 7365 293a 0a20 2020 2070  Response):.    p
+00007a90: 6173 730a 0a0a 636c 6173 7320 4f70 656e  ass...class Open
+00007aa0: 4170 6952 6573 706f 6e73 6528 4a53 4f4e  ApiResponse(JSON
+00007ab0: 4465 7465 6374 6f72 293a 0a20 2020 205f  Detector):.    _
+00007ac0: 5f66 696c 656e 616d 655f 636f 6e74 656e  _filename_conten
+00007ad0: 745f 6469 7370 6f73 6974 696f 6e5f 7061  t_disposition_pa
+00007ae0: 7474 6572 6e20 3d20 7265 2e63 6f6d 7069  ttern = re.compi
+00007af0: 6c65 2827 6669 6c65 6e61 6d65 3d22 282e  le('filename="(.
+00007b00: 2b3f 2922 2729 0a0a 2020 2020 6465 6620  +?)"')..    def 
+00007b10: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+00007b20: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+00007b30: 7265 7370 6f6e 7365 5f63 6c73 3a20 7479  response_cls: ty
+00007b40: 7069 6e67 2e54 7970 655b 4170 6952 6573  ping.Type[ApiRes
+00007b50: 706f 6e73 655d 203d 2041 7069 5265 7370  ponse] = ApiResp
+00007b60: 6f6e 7365 2c0a 2020 2020 2020 2020 7265  onse,.        re
+00007b70: 7370 6f6e 7365 5f63 6c73 5f61 7379 6e63  sponse_cls_async
+00007b80: 3a20 7479 7069 6e67 2e54 7970 655b 4173  : typing.Type[As
+00007b90: 796e 6341 7069 5265 7370 6f6e 7365 5d20  yncApiResponse] 
+00007ba0: 3d20 4173 796e 6341 7069 5265 7370 6f6e  = AsyncApiRespon
+00007bb0: 7365 2c0a 2020 2020 2020 2020 636f 6e74  se,.        cont
+00007bc0: 656e 743a 2074 7970 696e 672e 4f70 7469  ent: typing.Opti
+00007bd0: 6f6e 616c 5b74 7970 696e 672e 4469 6374  onal[typing.Dict
+00007be0: 5b73 7472 2c20 4d65 6469 6154 7970 655d  [str, MediaType]
+00007bf0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00007c00: 2020 6865 6164 6572 733a 2074 7970 696e    headers: typin
+00007c10: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00007c20: 672e 4c69 7374 5b48 6561 6465 7250 6172  g.List[HeaderPar
+00007c30: 616d 6574 6572 5d5d 203d 204e 6f6e 652c  ameter]] = None,
+00007c40: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00007c50: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+00007c60: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+00007c70: 6620 636f 6e74 656e 7420 6973 206e 6f74  f content is not
+00007c80: 204e 6f6e 6520 616e 6420 6c65 6e28 636f   None and len(co
+00007c90: 6e74 656e 7429 203d 3d20 303a 0a20 2020  ntent) == 0:.   
+00007ca0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00007cb0: 616c 7565 4572 726f 7228 2749 6e76 616c  alueError('Inval
+00007cc0: 6964 2076 616c 7565 2066 6f72 2063 6f6e  id value for con
+00007cd0: 7465 6e74 2c20 7468 6520 636f 6e74 656e  tent, the conten
+00007ce0: 7420 6469 6374 206d 7573 7420 6861 7665  t dict must have
+00007cf0: 203e 3d20 3120 656e 7472 7927 290a 2020   >= 1 entry').  
+00007d00: 2020 2020 2020 7365 6c66 2e63 6f6e 7465        self.conte
+00007d10: 6e74 203d 2063 6f6e 7465 6e74 0a20 2020  nt = content.   
+00007d20: 2020 2020 2073 656c 662e 7265 7370 6f6e       self.respon
+00007d30: 7365 5f63 6c73 203d 2072 6573 706f 6e73  se_cls = respons
+00007d40: 655f 636c 730a 2020 2020 2020 2020 7365  e_cls.        se
+00007d50: 6c66 2e72 6573 706f 6e73 655f 636c 735f  lf.response_cls_
+00007d60: 6173 796e 6320 3d20 7265 7370 6f6e 7365  async = response
+00007d70: 5f63 6c73 5f61 7379 6e63 0a0a 2020 2020  _cls_async..    
+00007d80: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00007d90: 2020 6465 6620 5f5f 6465 7365 7269 616c    def __deserial
+00007da0: 697a 655f 6a73 6f6e 2872 6573 706f 6e73  ize_json(respons
+00007db0: 653a 2062 7974 6573 2920 2d3e 2074 7970  e: bytes) -> typ
+00007dc0: 696e 672e 416e 793a 0a20 2020 2020 2020  ing.Any:.       
+00007dd0: 2023 2070 7974 686f 6e20 6d75 7374 2062   # python must b
+00007de0: 6520 3e3d 2033 2e39 2073 6f20 7765 2063  e >= 3.9 so we c
+00007df0: 616e 2070 6173 7320 696e 2062 7974 6573  an pass in bytes
+00007e00: 2069 6e74 6f20 6a73 6f6e 2e6c 6f61 6473   into json.loads
+00007e10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00007e20: 6a73 6f6e 2e6c 6f61 6473 2872 6573 706f  json.loads(respo
+00007e30: 6e73 6529 0a0a 2020 2020 4073 7461 7469  nse)..    @stati
+00007e40: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00007e50: 5f5f 6669 6c65 5f6e 616d 655f 6672 6f6d  __file_name_from
+00007e60: 5f72 6573 706f 6e73 655f 7572 6c28 7265  _response_url(re
+00007e70: 7370 6f6e 7365 5f75 726c 3a20 7479 7069  sponse_url: typi
+00007e80: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00007e90: 2920 2d3e 2074 7970 696e 672e 4f70 7469  ) -> typing.Opti
+00007ea0: 6f6e 616c 5b73 7472 5d3a 0a20 2020 2020  onal[str]:.     
+00007eb0: 2020 2069 6620 7265 7370 6f6e 7365 5f75     if response_u
+00007ec0: 726c 2069 7320 4e6f 6e65 3a0a 2020 2020  rl is None:.    
+00007ed0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00007ee0: 6f6e 650a 2020 2020 2020 2020 7572 6c5f  one.        url_
+00007ef0: 7061 7468 203d 2075 726c 7061 7273 6528  path = urlparse(
+00007f00: 7265 7370 6f6e 7365 5f75 726c 292e 7061  response_url).pa
+00007f10: 7468 0a20 2020 2020 2020 2069 6620 7572  th.        if ur
+00007f20: 6c5f 7061 7468 3a0a 2020 2020 2020 2020  l_path:.        
+00007f30: 2020 2020 7061 7468 5f62 6173 656e 616d      path_basenam
+00007f40: 6520 3d20 6f73 2e70 6174 682e 6261 7365  e = os.path.base
+00007f50: 6e61 6d65 2875 726c 5f70 6174 6829 0a20  name(url_path). 
+00007f60: 2020 2020 2020 2020 2020 2069 6620 7061             if pa
+00007f70: 7468 5f62 6173 656e 616d 653a 0a20 2020  th_basename:.   
+00007f80: 2020 2020 2020 2020 2020 2020 205f 6669               _fi
+00007f90: 6c65 6e61 6d65 2c20 6578 7420 3d20 6f73  lename, ext = os
+00007fa0: 2e70 6174 682e 7370 6c69 7465 7874 2870  .path.splitext(p
+00007fb0: 6174 685f 6261 7365 6e61 6d65 290a 2020  ath_basename).  
+00007fc0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007fd0: 2065 7874 3a0a 2020 2020 2020 2020 2020   ext:.          
+00007fe0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007ff0: 2070 6174 685f 6261 7365 6e61 6d65 0a20   path_basename. 
+00008000: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00008010: 6e65 0a0a 2020 2020 4063 6c61 7373 6d65  ne..    @classme
+00008020: 7468 6f64 0a20 2020 2064 6566 205f 5f66  thod.    def __f
+00008030: 696c 655f 6e61 6d65 5f66 726f 6d5f 636f  ile_name_from_co
+00008040: 6e74 656e 745f 6469 7370 6f73 6974 696f  ntent_dispositio
+00008050: 6e28 636c 732c 2063 6f6e 7465 6e74 5f64  n(cls, content_d
+00008060: 6973 706f 7369 7469 6f6e 3a20 7479 7069  isposition: typi
+00008070: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00008080: 2920 2d3e 2074 7970 696e 672e 4f70 7469  ) -> typing.Opti
+00008090: 6f6e 616c 5b73 7472 5d3a 0a20 2020 2020  onal[str]:.     
+000080a0: 2020 2069 6620 636f 6e74 656e 745f 6469     if content_di
+000080b0: 7370 6f73 6974 696f 6e20 6973 204e 6f6e  sposition is Non
+000080c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000080d0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+000080e0: 2020 206d 6174 6368 203d 2063 6c73 2e5f     match = cls._
+000080f0: 5f66 696c 656e 616d 655f 636f 6e74 656e  _filename_conten
+00008100: 745f 6469 7370 6f73 6974 696f 6e5f 7061  t_disposition_pa
+00008110: 7474 6572 6e2e 7365 6172 6368 2863 6f6e  ttern.search(con
+00008120: 7465 6e74 5f64 6973 706f 7369 7469 6f6e  tent_disposition
+00008130: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00008140: 206d 6174 6368 3a0a 2020 2020 2020 2020   match:.        
+00008150: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00008160: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+00008170: 6174 6368 2e67 726f 7570 2831 290a 0a20  atch.group(1).. 
+00008180: 2020 2064 6566 205f 5f64 6573 6572 6961     def __deseria
+00008190: 6c69 7a65 5f61 7070 6c69 6361 7469 6f6e  lize_application
+000081a0: 5f6f 6374 6574 5f73 7472 6561 6d28 0a20  _octet_stream(. 
+000081b0: 2020 2020 2020 2073 656c 662c 2072 6573         self, res
+000081c0: 706f 6e73 653a 2075 726c 6c69 6233 2e48  ponse: urllib3.H
+000081d0: 5454 5052 6573 706f 6e73 650a 2020 2020  TTPResponse.    
+000081e0: 2920 2d3e 2074 7970 696e 672e 556e 696f  ) -> typing.Unio
+000081f0: 6e5b 6279 7465 732c 2069 6f2e 4275 6666  n[bytes, io.Buff
+00008200: 6572 6564 5265 6164 6572 5d3a 0a20 2020  eredReader]:.   
+00008210: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00008220: 2075 726c 6c69 6233 2075 7365 2063 6173   urllib3 use cas
+00008230: 6573 3a0a 2020 2020 2020 2020 312e 2077  es:.        1. w
+00008240: 6865 6e20 7072 656c 6f61 645f 636f 6e74  hen preload_cont
+00008250: 656e 743d 5472 7565 2028 7374 7265 616d  ent=True (stream
+00008260: 3d46 616c 7365 2920 7468 656e 2073 7570  =False) then sup
+00008270: 706f 7274 735f 6368 756e 6b65 645f 7265  ports_chunked_re
+00008280: 6164 7320 6973 2046 616c 7365 2061 6e64  ads is False and
+00008290: 2062 7974 6573 2061 7265 2072 6574 7572   bytes are retur
+000082a0: 6e65 640a 2020 2020 2020 2020 322e 2077  ned.        2. w
+000082b0: 6865 6e20 7072 656c 6f61 645f 636f 6e74  hen preload_cont
+000082c0: 656e 743d 4661 6c73 6520 2873 7472 6561  ent=False (strea
+000082d0: 6d3d 5472 7565 2920 7468 656e 2073 7570  m=True) then sup
+000082e0: 706f 7274 735f 6368 756e 6b65 645f 7265  ports_chunked_re
+000082f0: 6164 7320 6973 2054 7275 6520 616e 640a  ads is True and.
+00008300: 2020 2020 2020 2020 2020 2020 6120 6669              a fi
+00008310: 6c65 2077 696c 6c20 6265 2077 7269 7474  le will be writt
+00008320: 656e 2061 6e64 2072 6574 7572 6e65 640a  en and returned.
+00008330: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008340: 2020 2020 6966 2072 6573 706f 6e73 652e      if response.
+00008350: 7375 7070 6f72 7473 5f63 6875 6e6b 6564  supports_chunked
+00008360: 5f72 6561 6473 2829 3a0a 2020 2020 2020  _reads():.      
+00008370: 2020 2020 2020 6669 6c65 5f6e 616d 6520        file_name 
+00008380: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+00008390: 2020 2020 7365 6c66 2e5f 5f66 696c 655f      self.__file_
+000083a0: 6e61 6d65 5f66 726f 6d5f 636f 6e74 656e  name_from_conten
+000083b0: 745f 6469 7370 6f73 6974 696f 6e28 7265  t_disposition(re
+000083c0: 7370 6f6e 7365 2e68 6561 6465 7273 2e67  sponse.headers.g
+000083d0: 6574 2827 636f 6e74 656e 742d 6469 7370  et('content-disp
+000083e0: 6f73 6974 696f 6e27 2929 0a20 2020 2020  osition')).     
+000083f0: 2020 2020 2020 2020 2020 206f 7220 7365             or se
+00008400: 6c66 2e5f 5f66 696c 655f 6e61 6d65 5f66  lf.__file_name_f
+00008410: 726f 6d5f 7265 7370 6f6e 7365 5f75 726c  rom_response_url
+00008420: 2872 6573 706f 6e73 652e 6765 7475 726c  (response.geturl
+00008430: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00008440: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00008450: 6620 6669 6c65 5f6e 616d 6520 6973 204e  f file_name is N
+00008460: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00008470: 2020 2020 205f 6664 2c20 7061 7468 203d       _fd, path =
+00008480: 2074 656d 7066 696c 652e 6d6b 7374 656d   tempfile.mkstem
+00008490: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+000084a0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000084b0: 2020 2020 2020 7061 7468 203d 206f 732e        path = os.
+000084c0: 7061 7468 2e6a 6f69 6e28 7465 6d70 6669  path.join(tempfi
+000084d0: 6c65 2e67 6574 7465 6d70 6469 7228 292c  le.gettempdir(),
+000084e0: 2066 696c 655f 6e61 6d65 290a 0a20 2020   file_name)..   
+000084f0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+00008500: 656e 2870 6174 682c 2027 7762 2729 2061  en(path, 'wb') a
+00008510: 7320 6e65 775f 6669 6c65 3a0a 2020 2020  s new_file:.    
+00008520: 2020 2020 2020 2020 2020 2020 6368 756e              chun
+00008530: 6b5f 7369 7a65 203d 2031 3032 340a 2020  k_size = 1024.  
+00008540: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+00008550: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+00008560: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00008570: 7461 203d 2072 6573 706f 6e73 652e 7265  ta = response.re
+00008580: 6164 2863 6875 6e6b 5f73 697a 6529 0a20  ad(chunk_size). 
+00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085a0: 2020 2069 6620 6e6f 7420 6461 7461 3a0a     if not data:.
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085e0: 2020 6e65 775f 6669 6c65 2e77 7269 7465    new_file.write
+000085f0: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
+00008600: 2020 2023 2072 656c 6561 7365 5f63 6f6e     # release_con
+00008610: 6e20 6973 206e 6565 6465 6420 666f 7220  n is needed for 
+00008620: 7374 7265 616d 696e 6720 636f 6e6e 6563  streaming connec
+00008630: 7469 6f6e 7320 6f6e 6c79 0a20 2020 2020  tions only.     
+00008640: 2020 2020 2020 2072 6573 706f 6e73 652e         response.
+00008650: 7265 6c65 6173 655f 636f 6e6e 2829 0a20  release_conn(). 
+00008660: 2020 2020 2020 2020 2020 206e 6577 5f66             new_f
+00008670: 696c 6520 3d20 6f70 656e 2870 6174 682c  ile = open(path,
+00008680: 2027 7262 2729 0a20 2020 2020 2020 2020   'rb').         
+00008690: 2020 2072 6574 7572 6e20 6e65 775f 6669     return new_fi
+000086a0: 6c65 0a20 2020 2020 2020 2065 6c73 653a  le.        else:
+000086b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000086c0: 7572 6e20 7265 7370 6f6e 7365 2e64 6174  urn response.dat
+000086d0: 610a 0a20 2020 2040 7374 6174 6963 6d65  a..    @staticme
+000086e0: 7468 6f64 0a20 2020 2064 6566 205f 5f64  thod.    def __d
+000086f0: 6573 6572 6961 6c69 7a65 5f6d 756c 7469  eserialize_multi
+00008700: 7061 7274 5f66 6f72 6d5f 6461 7461 280a  part_form_data(.
+00008710: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00008720: 3a20 6279 7465 730a 2020 2020 2920 2d3e  : bytes.    ) ->
+00008730: 2074 7970 696e 672e 4469 6374 5b73 7472   typing.Dict[str
+00008740: 2c20 7479 7069 6e67 2e41 6e79 5d3a 0a20  , typing.Any]:. 
+00008750: 2020 2020 2020 206d 7367 203d 2065 6d61         msg = ema
+00008760: 696c 2e6d 6573 7361 6765 5f66 726f 6d5f  il.message_from_
+00008770: 6279 7465 7328 7265 7370 6f6e 7365 290a  bytes(response).
+00008780: 2020 2020 2020 2020 7265 7475 726e 207b          return {
+00008790: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
+000087a0: 742e 6765 745f 7061 7261 6d28 226e 616d  t.get_param("nam
+000087b0: 6522 2c20 6865 6164 6572 3d22 436f 6e74  e", header="Cont
+000087c0: 656e 742d 4469 7370 6f73 6974 696f 6e22  ent-Disposition"
+000087d0: 293a 2070 6172 742e 6765 745f 7061 796c  ): part.get_payl
+000087e0: 6f61 6428 0a20 2020 2020 2020 2020 2020  oad(.           
+000087f0: 2020 2020 2064 6563 6f64 653d 5472 7565       decode=True
+00008800: 0a20 2020 2020 2020 2020 2020 2029 2e64  .            ).d
+00008810: 6563 6f64 6528 7061 7274 2e67 6574 5f63  ecode(part.get_c
+00008820: 6f6e 7465 6e74 5f63 6861 7273 6574 2829  ontent_charset()
+00008830: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00008840: 2070 6172 742e 6765 745f 636f 6e74 656e   part.get_conten
+00008850: 745f 6368 6172 7365 7428 290a 2020 2020  t_charset().    
+00008860: 2020 2020 2020 2020 656c 7365 2070 6172          else par
+00008870: 742e 6765 745f 7061 796c 6f61 6428 290a  t.get_payload().
+00008880: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00008890: 7061 7274 2069 6e20 6d73 672e 6765 745f  part in msg.get_
+000088a0: 7061 796c 6f61 6428 290a 2020 2020 2020  payload().      
+000088b0: 2020 7d0a 0a20 2020 2064 6566 205f 5f67    }..    def __g
+000088c0: 6574 5f73 6368 656d 615f 666f 725f 636f  et_schema_for_co
+000088d0: 6e74 656e 745f 7479 7065 280a 2020 2020  ntent_type(.    
+000088e0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000088f0: 2020 636f 6e74 656e 745f 7479 7065 0a20    content_type. 
+00008900: 2020 2029 202d 3e20 7479 7069 6e67 2e4f     ) -> typing.O
+00008910: 7074 696f 6e61 6c5b 7479 7069 6e67 2e54  ptional[typing.T
+00008920: 7970 655b 5363 6865 6d61 5d5d 3a0a 2020  ype[Schema]]:.  
+00008930: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00008940: 2020 4669 6e64 7320 7468 6520 636f 7272    Finds the corr
+00008950: 6563 7420 5363 6865 6d61 4f62 6a65 6374  ect SchemaObject
+00008960: 2066 6f72 2061 2070 6172 7469 6375 6c61   for a particula
+00008970: 7220 636f 6e74 656e 7420 7479 7065 2e20  r content type. 
+00008980: 4861 6e64 6c65 730a 2020 2020 2020 2020  Handles.        
+00008990: 7468 6520 6173 7465 7269 736b 2022 2a22  the asterisk "*"
+000089a0: 2063 6861 7261 6374 6572 2074 6861 7420   character that 
+000089b0: 6973 2075 7365 6420 746f 2067 726f 7570  is used to group
+000089c0: 206d 6564 6961 2074 7970 6573 2069 6e74   media types int
+000089d0: 6f20 7261 6e67 6573 0a20 2020 2020 2020  o ranges.       
+000089e0: 2028 6874 7470 733a 2f2f 7777 772e 7266   (https://www.rf
+000089f0: 632d 6564 6974 6f72 2e6f 7267 2f72 6663  c-editor.org/rfc
+00008a00: 2f72 6663 3732 3331 2373 6563 7469 6f6e  /rfc7231#section
+00008a10: 2d35 2e33 2e32 292e 2041 6c73 6f20 6861  -5.3.2). Also ha
+00008a20: 6e64 6c65 730a 2020 2020 2020 2020 7061  ndles.        pa
+00008a30: 7261 6d65 7465 7273 2069 6e20 7468 6520  rameters in the 
+00008a40: 666f 726d 206f 6620 6e61 6d65 3d76 616c  form of name=val
+00008a50: 7565 2070 6169 7273 2e0a 2020 2020 2020  ue pairs..      
+00008a60: 2020 2222 220a 2020 2020 2020 2020 6d65    """.        me
+00008a70: 6469 615f 7479 7065 7320 3d20 7365 6c66  dia_types = self
+00008a80: 2e63 6f6e 7465 6e74 2e6b 6579 7328 290a  .content.keys().
+00008a90: 2020 2020 2020 2020 6d61 7463 6865 645f          matched_
+00008aa0: 6d65 6469 615f 7479 7065 203d 204f 7065  media_type = Ope
+00008ab0: 6e41 7069 5265 7370 6f6e 7365 2e6d 6174  nApiResponse.mat
+00008ac0: 6368 5f63 6f6e 7465 6e74 5f74 7970 6528  ch_content_type(
+00008ad0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00008ae0: 7465 6e74 5f74 7970 653d 636f 6e74 656e  tent_type=conten
+00008af0: 745f 7479 7065 2c0a 2020 2020 2020 2020  t_type,.        
+00008b00: 2020 2020 6d65 6469 615f 7479 7065 733d      media_types=
+00008b10: 6d65 6469 615f 7479 7065 730a 2020 2020  media_types.    
+00008b20: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+00008b30: 206d 6174 6368 6564 5f6d 6564 6961 5f74   matched_media_t
+00008b40: 7970 6520 6973 204e 6f6e 653a 0a20 2020  ype is None:.   
+00008b50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00008b60: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+00008b70: 7572 6e20 7365 6c66 2e63 6f6e 7465 6e74  urn self.content
+00008b80: 5b6d 6174 6368 6564 5f6d 6564 6961 5f74  [matched_media_t
+00008b90: 7970 655d 2e73 6368 656d 610a 0a20 2020  ype].schema..   
+00008ba0: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+00008bb0: 2020 2064 6566 206d 6174 6368 5f63 6f6e     def match_con
+00008bc0: 7465 6e74 5f74 7970 6528 636f 6e74 656e  tent_type(conten
+00008bd0: 745f 7479 7065 3a20 7374 722c 206d 6564  t_type: str, med
+00008be0: 6961 5f74 7970 6573 3a20 7479 7069 6e67  ia_types: typing
+00008bf0: 2e4c 6973 745b 7374 725d 2920 2d3e 2074  .List[str]) -> t
+00008c00: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
+00008c10: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
+00008c20: 0a20 2020 2020 2020 204d 6174 6368 6573  .        Matches
+00008c30: 2061 2063 6f6e 7465 6e74 2074 7970 6520   a content type 
+00008c40: 746f 2061 206d 6564 6961 2074 7970 6520  to a media type 
+00008c50: 696e 2061 206c 6973 7420 6f66 206d 6564  in a list of med
+00008c60: 6961 2074 7970 6573 2c20 6861 6e64 6c69  ia types, handli
+00008c70: 6e67 206d 6564 6961 2074 7970 6520 7261  ng media type ra
+00008c80: 6e67 6573 2061 7320 6465 6669 6e65 6420  nges as defined 
+00008c90: 696e 2052 4643 3732 3331 2e0a 0a20 2020  in RFC7231...   
+00008ca0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+00008cb0: 0a20 2020 2020 2020 2063 6f6e 7465 6e74  .        content
+00008cc0: 5f74 7970 6520 2873 7472 293a 2054 6865  _type (str): The
+00008cd0: 2063 6f6e 7465 6e74 2074 7970 6520 746f   content type to
+00008ce0: 206d 6174 6368 2e0a 2020 2020 2020 2020   match..        
+00008cf0: 6d65 6469 615f 7479 7065 7320 286c 6973  media_types (lis
+00008d00: 7429 3a20 5468 6520 6c69 7374 206f 6620  t): The list of 
+00008d10: 6d65 6469 6120 7479 7065 7320 746f 2073  media types to s
+00008d20: 6561 7263 682e 0a0a 2020 2020 2020 2020  earch...        
+00008d30: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00008d40: 2073 7472 3a20 5468 6520 6669 7273 7420   str: The first 
+00008d50: 6d65 6469 6120 7479 7065 2074 6861 7420  media type that 
+00008d60: 6d61 7463 6865 7320 7468 6520 636f 6e74  matches the cont
+00008d70: 656e 7420 7479 7065 2c20 6f72 204e 6f6e  ent type, or Non
+00008d80: 6520 6966 206e 6f20 6d61 7463 6820 6973  e if no match is
+00008d90: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
+00008da0: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
+00008db0: 6d65 6469 615f 7479 7065 2069 6e20 6d65  media_type in me
+00008dc0: 6469 615f 7479 7065 733a 0a20 2020 2020  dia_types:.     
+00008dd0: 2020 2020 2020 2069 6620 6d65 6469 615f         if media_
+00008de0: 7479 7065 203d 3d20 272a 2f2a 2720 6f72  type == '*/*' or
+00008df0: 206d 6564 6961 5f74 7970 6520 3d3d 2063   media_type == c
+00008e00: 6f6e 7465 6e74 5f74 7970 653a 0a20 2020  ontent_type:.   
+00008e10: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00008e20: 7572 6e20 6d65 6469 615f 7479 7065 0a20  urn media_type. 
+00008e30: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00008e40: 272f 2720 696e 206d 6564 6961 5f74 7970  '/' in media_typ
+00008e50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00008e60: 2020 2074 7970 655f 2c20 7375 6274 7970     type_, subtyp
+00008e70: 6520 3d20 6d65 6469 615f 7479 7065 2e73  e = media_type.s
+00008e80: 706c 6974 2827 2f27 290a 2020 2020 2020  plit('/').      
+00008e90: 2020 2020 2020 2020 2020 6966 2028 7479            if (ty
+00008ea0: 7065 5f20 3d3d 2027 2a27 206f 7220 7479  pe_ == '*' or ty
+00008eb0: 7065 5f20 3d3d 2063 6f6e 7465 6e74 5f74  pe_ == content_t
+00008ec0: 7970 652e 7370 6c69 7428 272f 2729 5b30  ype.split('/')[0
+00008ed0: 5d29 2061 6e64 205c 0a20 2020 2020 2020  ]) and \.       
+00008ee0: 2020 2020 2020 2020 2028 7375 6274 7970           (subtyp
+00008ef0: 6520 3d3d 2027 2a27 206f 7220 7375 6274  e == '*' or subt
+00008f00: 7970 6520 3d3d 2063 6f6e 7465 6e74 5f74  ype == content_t
+00008f10: 7970 652e 7370 6c69 7428 272f 2729 5b31  ype.split('/')[1
+00008f20: 5d2e 7370 6c69 7428 273b 2729 5b30 5d29  ].split(';')[0])
+00008f30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008f40: 2020 2020 2020 7265 7475 726e 206d 6564        return med
+00008f50: 6961 5f74 7970 650a 0a20 2020 2020 2020  ia_type..       
+00008f60: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
+00008f70: 2020 6173 796e 6320 6465 6620 6465 7365    async def dese
+00008f80: 7269 616c 697a 655f 6173 796e 6328 7365  rialize_async(se
+00008f90: 6c66 2c20 7265 7370 6f6e 7365 3a20 4173  lf, response: As
+00008fa0: 796e 6352 6573 706f 6e73 6557 7261 7070  yncResponseWrapp
+00008fb0: 6572 2c20 636f 6e66 6967 7572 6174 696f  er, configuratio
+00008fc0: 6e3a 2043 6f6e 6669 6775 7261 7469 6f6e  n: Configuration
+00008fd0: 2c20 736b 6970 5f64 6573 6572 6961 6c69  , skip_deseriali
+00008fe0: 7a61 7469 6f6e 203d 2046 616c 7365 2920  zation = False) 
+00008ff0: 2d3e 2041 7379 6e63 4170 6952 6573 706f  -> AsyncApiRespo
+00009000: 6e73 653a 0a20 2020 2020 2020 2022 2222  nse:.        """
+00009010: 0a20 2020 2020 2020 2044 6573 6572 6961  .        Deseria
+00009020: 6c69 7a65 7320 616e 2048 5454 5020 7265  lizes an HTTP re
+00009030: 7370 6f6e 7365 2062 6f64 7920 696e 746f  sponse body into
+00009040: 2061 6e20 6f62 6a65 6374 2e0a 2020 2020   an object..    
+00009050: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00009060: 636f 6e74 656e 745f 7479 7065 203d 2072  content_type = r
+00009070: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+00009080: 706f 6e73 652e 636f 6e74 656e 745f 7479  ponse.content_ty
+00009090: 7065 0a20 2020 2020 2020 2064 6573 6572  pe.        deser
+000090a0: 6961 6c69 7a65 645f 626f 6479 203d 2075  ialized_body = u
+000090b0: 6e73 6574 0a20 2020 2020 2020 2069 6620  nset.        if 
+000090c0: 7365 6c66 2e63 6f6e 7465 6e74 2069 7320  self.content is 
+000090d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000090e0: 2020 2020 2020 6966 206c 656e 2873 656c        if len(sel
+000090f0: 662e 636f 6e74 656e 7429 203d 3d20 303a  f.content) == 0:
+00009100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009110: 2023 2073 6f6d 6520 7370 6563 7320 646f   # some specs do
+00009120: 206e 6f74 2064 6566 696e 6520 7265 7370   not define resp
+00009130: 6f6e 7365 2063 6f6e 7465 6e74 206d 6564  onse content med
+00009140: 6961 2074 7970 6520 7363 6865 6d61 730a  ia type schemas.
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 7265 7475 726e 2073 656c 662e 7265 7370  return self.resp
+00009170: 6f6e 7365 5f63 6c73 5f61 7379 6e63 280a  onse_cls_async(.
+00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009190: 2020 2020 726f 756e 645f 7472 6970 5f74      round_trip_t
+000091a0: 696d 653d 7265 7370 6f6e 7365 2e72 6f75  ime=response.rou
+000091b0: 6e64 5f74 7269 705f 7469 6d65 2c0a 2020  nd_trip_time,.  
+000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091d0: 2020 7265 7370 6f6e 7365 3d72 6573 706f    response=respo
+000091e0: 6e73 652e 6874 7470 5f72 6573 706f 6e73  nse.http_respons
+000091f0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00009200: 2020 2020 2020 2062 6f64 793d 756e 7365         body=unse
+00009210: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00009220: 2020 2020 2020 2068 6561 6465 7273 3d72         headers=r
+00009230: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+00009240: 706f 6e73 652e 6865 6164 6572 732c 0a20  ponse.headers,. 
+00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009260: 2020 2073 7461 7475 733d 7265 7370 6f6e     status=respon
+00009270: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
+00009280: 2e73 7461 7475 730a 2020 2020 2020 2020  .status.        
+00009290: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000092a0: 2020 2020 2020 626f 6479 5f73 6368 656d        body_schem
+000092b0: 6120 3d20 7365 6c66 2e5f 5f67 6574 5f73  a = self.__get_s
+000092c0: 6368 656d 615f 666f 725f 636f 6e74 656e  chema_for_conten
+000092d0: 745f 7479 7065 2863 6f6e 7465 6e74 5f74  t_type(content_t
+000092e0: 7970 6529 0a20 2020 2020 2020 2020 2020  ype).           
+000092f0: 2069 6620 626f 6479 5f73 6368 656d 6120   if body_schema 
+00009300: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00009310: 2020 2020 2020 2020 2072 6169 7365 2041           raise A
+00009320: 7069 5661 6c75 6545 7272 6f72 280a 2020  piValueError(.  
+00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009340: 2020 6622 496e 7661 6c69 6420 636f 6e74    f"Invalid cont
+00009350: 656e 745f 7479 7065 2072 6574 7572 6e65  ent_type returne
+00009360: 642e 2043 6f6e 7465 6e74 5f74 7970 653d  d. Content_type=
+00009370: 277b 636f 6e74 656e 745f 7479 7065 7d27  '{content_type}'
+00009380: 2077 6173 2072 6574 7572 6e65 6420 220a   was returned ".
+00009390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093a0: 2020 2020 6622 7768 656e 206f 6e6c 7920      f"when only 
+000093b0: 7b73 7472 2873 6574 2873 656c 662e 636f  {str(set(self.co
+000093c0: 6e74 656e 7429 297d 2061 7265 2064 6566  ntent))} are def
+000093d0: 696e 6564 2066 6f72 2073 7461 7475 735f  ined for status_
+000093e0: 636f 6465 3d7b 7374 7228 7265 7370 6f6e  code={str(respon
+000093f0: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
+00009400: 2e73 7461 7475 7329 7d22 0a20 2020 2020  .status)}".     
+00009410: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00009420: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00009430: 2e5f 636f 6e74 656e 745f 7479 7065 5f69  ._content_type_i
+00009440: 735f 6a73 6f6e 2863 6f6e 7465 6e74 5f74  s_json(content_t
+00009450: 7970 6529 3a0a 2020 2020 2020 2020 2020  ype):.          
+00009460: 2020 2020 2020 626f 6479 5f64 6174 6120        body_data 
+00009470: 3d20 7365 6c66 2e5f 5f64 6573 6572 6961  = self.__deseria
+00009480: 6c69 7a65 5f6a 736f 6e28 6177 6169 7420  lize_json(await 
+00009490: 7265 7370 6f6e 7365 2e68 7474 705f 7265  response.http_re
+000094a0: 7370 6f6e 7365 2e72 6561 6428 2929 0a20  sponse.read()). 
+000094b0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000094c0: 636f 6e74 656e 745f 7479 7065 2e73 7461  content_type.sta
+000094d0: 7274 7377 6974 6828 276d 756c 7469 7061  rtswith('multipa
+000094e0: 7274 2f66 6f72 6d2d 6461 7461 2729 3a0a  rt/form-data'):.
+000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009500: 626f 6479 5f64 6174 6120 3d20 7365 6c66  body_data = self
+00009510: 2e5f 5f64 6573 6572 6961 6c69 7a65 5f6d  .__deserialize_m
+00009520: 756c 7469 7061 7274 5f66 6f72 6d5f 6461  ultipart_form_da
+00009530: 7461 2861 7761 6974 2072 6573 706f 6e73  ta(await respons
+00009540: 652e 6874 7470 5f72 6573 706f 6e73 652e  e.http_response.
+00009550: 7265 6164 2829 290a 2020 2020 2020 2020  read()).        
+00009560: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00009570: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00009580: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00009590: 726f 7228 2744 6573 6572 6961 6c69 7a61  ror('Deserializa
+000095a0: 7469 6f6e 206f 6620 7b7d 2068 6173 206e  tion of {} has n
+000095b0: 6f74 2079 6574 2062 6565 6e20 696d 706c  ot yet been impl
+000095c0: 656d 656e 7465 6427 2e66 6f72 6d61 7428  emented'.format(
+000095d0: 636f 6e74 656e 745f 7479 7065 2929 0a20  content_type)). 
+000095e0: 2020 2020 2020 2020 2020 2069 6620 736b             if sk
+000095f0: 6970 5f64 6573 6572 6961 6c69 7a61 7469  ip_deserializati
+00009600: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00009610: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00009620: 7265 7370 6f6e 7365 5f63 6c73 5f61 7379  response_cls_asy
+00009630: 6e63 280a 2020 2020 2020 2020 2020 2020  nc(.            
+00009640: 2020 2020 2020 2020 726f 756e 645f 7472          round_tr
+00009650: 6970 5f74 696d 653d 7265 7370 6f6e 7365  ip_time=response
+00009660: 2e72 6f75 6e64 5f74 7269 705f 7469 6d65  .round_trip_time
+00009670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009680: 2020 2020 2020 7265 7370 6f6e 7365 3d72        response=r
+00009690: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+000096a0: 706f 6e73 652c 0a20 2020 2020 2020 2020  ponse,.         
+000096b0: 2020 2020 2020 2020 2020 2062 6f64 793d             body=
+000096c0: 626f 6479 5f64 6174 612c 0a20 2020 2020  body_data,.     
+000096d0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+000096e0: 6561 6465 7273 3d72 6573 706f 6e73 652e  eaders=response.
+000096f0: 6874 7470 5f72 6573 706f 6e73 652e 6865  http_response.he
+00009700: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+00009710: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00009720: 733d 7265 7370 6f6e 7365 2e68 7474 705f  s=response.http_
+00009730: 7265 7370 6f6e 7365 2e73 7461 7475 730a  response.status.
+00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+00009760: 4578 6563 7574 6520 7661 6c69 6461 7469  Execute validati
+00009770: 6f6e 2061 6e64 2074 6872 6f77 2061 7320  on and throw as 
+00009780: 6120 7369 6465 2065 6666 6563 7420 6966  a side effect if
+00009790: 2076 616c 6964 6174 696f 6e20 6661 696c   validation fail
+000097a0: 730a 2020 2020 2020 2020 2020 2020 626f  s.            bo
+000097b0: 6479 5f73 6368 656d 612e 6672 6f6d 5f6f  dy_schema.from_o
+000097c0: 7065 6e61 7069 5f64 6174 615f 6f61 7067  penapi_data_oapg
+000097d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000097e0: 2020 626f 6479 5f64 6174 612c 0a20 2020    body_data,.   
+000097f0: 2020 2020 2020 2020 2020 2020 205f 636f               _co
+00009800: 6e66 6967 7572 6174 696f 6e3d 636f 6e66  nfiguration=conf
+00009810: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
+00009820: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00009830: 2020 2020 2320 5661 6c69 6461 7469 6f6e      # Validation
+00009840: 2070 6173 7365 642c 2073 6574 2064 6573   passed, set des
+00009850: 6572 6961 6c69 7a65 645f 626f 6479 2074  erialized_body t
+00009860: 6f20 706c 6169 6e20 6f6c 6420 6465 7365  o plain old dese
+00009870: 7269 616c 697a 6564 2064 6174 610a 2020  rialized data.  
+00009880: 2020 2020 2020 2020 2020 6465 7365 7269            deseri
+00009890: 616c 697a 6564 5f62 6f64 7920 3d20 626f  alized_body = bo
+000098a0: 6479 5f64 6174 610a 0a20 2020 2020 2020  dy_data..       
+000098b0: 2072 6574 7572 6e20 7365 6c66 2e72 6573   return self.res
+000098c0: 706f 6e73 655f 636c 735f 6173 796e 6328  ponse_cls_async(
+000098d0: 0a20 2020 2020 2020 2020 2020 2072 6f75  .            rou
+000098e0: 6e64 5f74 7269 705f 7469 6d65 3d72 6573  nd_trip_time=res
+000098f0: 706f 6e73 652e 726f 756e 645f 7472 6970  ponse.round_trip
+00009900: 5f74 696d 652c 0a20 2020 2020 2020 2020  _time,.         
+00009910: 2020 2072 6573 706f 6e73 653d 7265 7370     response=resp
+00009920: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
+00009930: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00009940: 626f 6479 3d64 6573 6572 6961 6c69 7a65  body=deserialize
+00009950: 645f 626f 6479 2c0a 2020 2020 2020 2020  d_body,.        
+00009960: 2020 2020 6865 6164 6572 733d 7265 7370      headers=resp
+00009970: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
+00009980: 7365 2e68 6561 6465 7273 2c0a 2020 2020  se.headers,.    
+00009990: 2020 2020 2020 2020 7374 6174 7573 3d72          status=r
+000099a0: 6573 706f 6e73 652e 6874 7470 5f72 6573  esponse.http_res
+000099b0: 706f 6e73 652e 7374 6174 7573 0a20 2020  ponse.status.   
+000099c0: 2020 2020 2029 0a0a 0a20 2020 2064 6566       )...    def
+000099d0: 2064 6573 6572 6961 6c69 7a65 2873 656c   deserialize(sel
+000099e0: 662c 2072 6573 706f 6e73 653a 2052 6573  f, response: Res
+000099f0: 706f 6e73 6557 7261 7070 6572 2c20 636f  ponseWrapper, co
+00009a00: 6e66 6967 7572 6174 696f 6e3a 2043 6f6e  nfiguration: Con
+00009a10: 6669 6775 7261 7469 6f6e 2c20 736b 6970  figuration, skip
+00009a20: 5f64 6573 6572 6961 6c69 7a61 7469 6f6e  _deserialization
+00009a30: 203d 2046 616c 7365 2920 2d3e 2041 7069   = False) -> Api
+00009a40: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
+00009a50: 2020 636f 6e74 656e 745f 7479 7065 203d    content_type =
+00009a60: 2072 6573 706f 6e73 652e 6874 7470 5f72   response.http_r
+00009a70: 6573 706f 6e73 652e 6865 6164 6572 732e  esponse.headers.
+00009a80: 6765 7428 2763 6f6e 7465 6e74 2d74 7970  get('content-typ
+00009a90: 6527 290a 2020 2020 2020 2020 6465 7365  e').        dese
+00009aa0: 7269 616c 697a 6564 5f62 6f64 7920 3d20  rialized_body = 
+00009ab0: 756e 7365 740a 2020 2020 2020 2020 7374  unset.        st
+00009ac0: 7265 616d 6564 203d 2072 6573 706f 6e73  reamed = respons
+00009ad0: 652e 6874 7470 5f72 6573 706f 6e73 652e  e.http_response.
+00009ae0: 7375 7070 6f72 7473 5f63 6875 6e6b 6564  supports_chunked
+00009af0: 5f72 6561 6473 2829 0a0a 2020 2020 2020  _reads()..      
+00009b00: 2020 6465 7365 7269 616c 697a 6564 5f68    deserialized_h
+00009b10: 6561 6465 7273 203d 2075 6e73 6574 0a20  eaders = unset. 
+00009b20: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00009b30: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00009b40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00009b50: 2320 544f 444f 2061 6464 2068 6561 6465  # TODO add heade
+00009b60: 7220 6465 7365 7269 616c 6961 7469 6f6e  r deserialiation
+00009b70: 2068 6572 650a 2020 2020 2020 2020 2020   here.          
+00009b80: 2020 7061 7373 0a0a 2020 2020 2020 2020    pass..        
+00009b90: 6966 2073 656c 662e 636f 6e74 656e 7420  if self.content 
+00009ba0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00009bb0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00009bc0: 7365 6c66 2e63 6f6e 7465 6e74 2920 3d3d  self.content) ==
+00009bd0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00009be0: 2020 2020 2320 736f 6d65 2073 7065 6373      # some specs
+00009bf0: 2064 6f20 6e6f 7420 6465 6669 6e65 2072   do not define r
+00009c00: 6573 706f 6e73 6520 636f 6e74 656e 7420  esponse content 
+00009c10: 6d65 6469 6120 7479 7065 2073 6368 656d  media type schem
+00009c20: 6173 0a20 2020 2020 2020 2020 2020 2020  as.             
+00009c30: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
+00009c40: 6573 706f 6e73 655f 636c 7328 0a20 2020  esponse_cls(.   
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2072 6f75 6e64 5f74 7269 705f 7469 6d65   round_trip_time
+00009c70: 3d72 6573 706f 6e73 652e 726f 756e 645f  =response.round_
+00009c80: 7472 6970 5f74 696d 652c 0a20 2020 2020  trip_time,.     
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009ca0: 6573 706f 6e73 653d 7265 7370 6f6e 7365  esponse=response
+00009cb0: 2e68 7474 705f 7265 7370 6f6e 7365 2c0a  .http_response,.
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 2020 2020 626f 6479 3d75 6e73 6574 2c0a      body=unset,.
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 2020 6865 6164 6572 733d 7265 7370      headers=resp
+00009d00: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
+00009d10: 7365 2e68 6561 6465 7273 2c0a 2020 2020  se.headers,.    
+00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d30: 7374 6174 7573 3d72 6573 706f 6e73 652e  status=response.
+00009d40: 6874 7470 5f72 6573 706f 6e73 652e 7374  http_response.st
+00009d50: 6174 7573 0a20 2020 2020 2020 2020 2020  atus.           
+00009d60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00009d70: 2020 2062 6f64 795f 7363 6865 6d61 203d     body_schema =
+00009d80: 2073 656c 662e 5f5f 6765 745f 7363 6865   self.__get_sche
+00009d90: 6d61 5f66 6f72 5f63 6f6e 7465 6e74 5f74  ma_for_content_t
+00009da0: 7970 6528 636f 6e74 656e 745f 7479 7065  ype(content_type
+00009db0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00009dc0: 2062 6f64 795f 7363 6865 6d61 2069 7320   body_schema is 
+00009dd0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009de0: 2020 2020 2020 7261 6973 6520 4170 6956        raise ApiV
+00009df0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00009e10: 2249 6e76 616c 6964 2063 6f6e 7465 6e74  "Invalid content
+00009e20: 5f74 7970 6520 7265 7475 726e 6564 2e20  _type returned. 
+00009e30: 436f 6e74 656e 745f 7479 7065 3d27 7b63  Content_type='{c
+00009e40: 6f6e 7465 6e74 5f74 7970 657d 2720 7761  ontent_type}' wa
+00009e50: 7320 7265 7475 726e 6564 2022 0a20 2020  s returned ".   
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 2066 2277 6865 6e20 6f6e 6c79 207b 7374   f"when only {st
+00009e80: 7228 7365 7428 7365 6c66 2e63 6f6e 7465  r(set(self.conte
+00009e90: 6e74 2929 7d20 6172 6520 6465 6669 6e65  nt))} are define
+00009ea0: 6420 666f 7220 7374 6174 7573 5f63 6f64  d for status_cod
+00009eb0: 653d 7b73 7472 2872 6573 706f 6e73 652e  e={str(response.
+00009ec0: 6874 7470 5f72 6573 706f 6e73 652e 7374  http_response.st
+00009ed0: 6174 7573 297d 220a 2020 2020 2020 2020  atus)}".        
+00009ee0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00009ef0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+00009f00: 636f 6e74 656e 745f 7479 7065 5f69 735f  content_type_is_
+00009f10: 6a73 6f6e 2863 6f6e 7465 6e74 5f74 7970  json(content_typ
+00009f20: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00009f30: 2020 2020 626f 6479 5f64 6174 6120 3d20      body_data = 
+00009f40: 7365 6c66 2e5f 5f64 6573 6572 6961 6c69  self.__deseriali
+00009f50: 7a65 5f6a 736f 6e28 7265 7370 6f6e 7365  ze_json(response
+00009f60: 2e68 7474 705f 7265 7370 6f6e 7365 2e64  .http_response.d
+00009f70: 6174 6129 0a20 2020 2020 2020 2020 2020  ata).           
+00009f80: 2065 6c69 6620 636f 6e74 656e 745f 7479   elif content_ty
+00009f90: 7065 203d 3d20 2761 7070 6c69 6361 7469  pe == 'applicati
+00009fa0: 6f6e 2f6f 6374 6574 2d73 7472 6561 6d27  on/octet-stream'
+00009fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009fc0: 2020 626f 6479 5f64 6174 6120 3d20 7365    body_data = se
+00009fd0: 6c66 2e5f 5f64 6573 6572 6961 6c69 7a65  lf.__deserialize
+00009fe0: 5f61 7070 6c69 6361 7469 6f6e 5f6f 6374  _application_oct
+00009ff0: 6574 5f73 7472 6561 6d28 7265 7370 6f6e  et_stream(respon
+0000a000: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
+0000a010: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000a020: 6966 2063 6f6e 7465 6e74 5f74 7970 652e  if content_type.
+0000a030: 7374 6172 7473 7769 7468 2827 6d75 6c74  startswith('mult
+0000a040: 6970 6172 742f 666f 726d 2d64 6174 6127  ipart/form-data'
+0000a050: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a060: 2020 2062 6f64 795f 6461 7461 203d 2073     body_data = s
+0000a070: 656c 662e 5f5f 6465 7365 7269 616c 697a  elf.__deserializ
+0000a080: 655f 6d75 6c74 6970 6172 745f 666f 726d  e_multipart_form
+0000a090: 5f64 6174 6128 7265 7370 6f6e 7365 2e68  _data(response.h
+0000a0a0: 7474 705f 7265 7370 6f6e 7365 2e64 6174  ttp_response.dat
+0000a0b0: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+0000a0c0: 2020 2063 6f6e 7465 6e74 5f74 7970 6520     content_type 
+0000a0d0: 3d20 276d 756c 7469 7061 7274 2f66 6f72  = 'multipart/for
+0000a0e0: 6d2d 6461 7461 270a 2020 2020 2020 2020  m-data'.        
+0000a0f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a100: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000a110: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+0000a120: 726f 7228 2744 6573 6572 6961 6c69 7a61  ror('Deserializa
+0000a130: 7469 6f6e 206f 6620 7b7d 2068 6173 206e  tion of {} has n
+0000a140: 6f74 2079 6574 2062 6565 6e20 696d 706c  ot yet been impl
+0000a150: 656d 656e 7465 6427 2e66 6f72 6d61 7428  emented'.format(
+0000a160: 636f 6e74 656e 745f 7479 7065 2929 0a20  content_type)). 
+0000a170: 2020 2020 2020 2020 2020 2069 6620 736b             if sk
+0000a180: 6970 5f64 6573 6572 6961 6c69 7a61 7469  ip_deserializati
+0000a190: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+0000a1a0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0000a1b0: 7265 7370 6f6e 7365 5f63 6c73 280a 2020  response_cls(.  
+0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1d0: 2020 726f 756e 645f 7472 6970 5f74 696d    round_trip_tim
+0000a1e0: 653d 7265 7370 6f6e 7365 2e72 6f75 6e64  e=response.round
+0000a1f0: 5f74 7269 705f 7469 6d65 2c0a 2020 2020  _trip_time,.    
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 7265 7370 6f6e 7365 3d72 6573 706f 6e73  response=respons
+0000a220: 652e 6874 7470 5f72 6573 706f 6e73 652c  e.http_response,
+0000a230: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a240: 2020 2020 2062 6f64 793d 626f 6479 5f64       body=body_d
+0000a250: 6174 612c 0a20 2020 2020 2020 2020 2020  ata,.           
+0000a260: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0000a270: 3d72 6573 706f 6e73 652e 6874 7470 5f72  =response.http_r
+0000a280: 6573 706f 6e73 652e 6865 6164 6572 732c  esponse.headers,
+0000a290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a2a0: 2020 2020 2073 7461 7475 733d 7265 7370       status=resp
+0000a2b0: 6f6e 7365 2e68 7474 705f 7265 7370 6f6e  onse.http_respon
+0000a2c0: 7365 2e73 7461 7475 730a 2020 2020 2020  se.status.      
+0000a2d0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000a2e0: 2020 2020 2020 2020 2023 2045 7865 6375           # Execu
+0000a2f0: 7465 2076 616c 6964 6174 696f 6e20 616e  te validation an
+0000a300: 6420 7468 726f 7720 6173 2061 2073 6964  d throw as a sid
+0000a310: 6520 6566 6665 6374 2069 6620 7661 6c69  e effect if vali
+0000a320: 6461 7469 6f6e 2066 6169 6c73 0a20 2020  dation fails.   
+0000a330: 2020 2020 2020 2020 2062 6f64 795f 7363           body_sc
+0000a340: 6865 6d61 2e66 726f 6d5f 6f70 656e 6170  hema.from_openap
+0000a350: 695f 6461 7461 5f6f 6170 6728 0a20 2020  i_data_oapg(.   
+0000a360: 2020 2020 2020 2020 2020 2020 2062 6f64               bod
+0000a370: 795f 6461 7461 2c0a 2020 2020 2020 2020  y_data,.        
+0000a380: 2020 2020 2020 2020 5f63 6f6e 6669 6775          _configu
+0000a390: 7261 7469 6f6e 3d63 6f6e 6669 6775 7261  ration=configura
+0000a3a0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+0000a3b0: 2029 0a20 2020 2020 2020 2020 2020 2023   ).            #
+0000a3c0: 2056 616c 6964 6174 696f 6e20 7061 7373   Validation pass
+0000a3d0: 6564 2c20 7365 7420 6465 7365 7269 616c  ed, set deserial
+0000a3e0: 697a 6564 5f62 6f64 7920 746f 2070 6c61  ized_body to pla
+0000a3f0: 696e 206f 6c64 2064 6573 6572 6961 6c69  in old deseriali
+0000a400: 7a65 6420 6461 7461 0a20 2020 2020 2020  zed data.       
+0000a410: 2020 2020 2064 6573 6572 6961 6c69 7a65       deserialize
+0000a420: 645f 626f 6479 203d 2062 6f64 795f 6461  d_body = body_da
+0000a430: 7461 0a20 2020 2020 2020 2065 6c69 6620  ta.        elif 
+0000a440: 7374 7265 616d 6564 3a0a 2020 2020 2020  streamed:.      
+0000a450: 2020 2020 2020 7265 7370 6f6e 7365 2e68        response.h
+0000a460: 7474 705f 7265 7370 6f6e 7365 2e72 656c  ttp_response.rel
+0000a470: 6561 7365 5f63 6f6e 6e28 290a 0a20 2020  ease_conn()..   
+0000a480: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0000a490: 2e72 6573 706f 6e73 655f 636c 7328 0a20  .response_cls(. 
+0000a4a0: 2020 2020 2020 2020 2020 2072 6f75 6e64             round
+0000a4b0: 5f74 7269 705f 7469 6d65 3d72 6573 706f  _trip_time=respo
+0000a4c0: 6e73 652e 726f 756e 645f 7472 6970 5f74  nse.round_trip_t
+0000a4d0: 696d 652c 0a20 2020 2020 2020 2020 2020  ime,.           
+0000a4e0: 2072 6573 706f 6e73 653d 7265 7370 6f6e   response=respon
+0000a4f0: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
+0000a500: 2c0a 2020 2020 2020 2020 2020 2020 626f  ,.            bo
+0000a510: 6479 3d64 6573 6572 6961 6c69 7a65 645f  dy=deserialized_
+0000a520: 626f 6479 2c0a 2020 2020 2020 2020 2020  body,.          
+0000a530: 2020 6865 6164 6572 733d 7265 7370 6f6e    headers=respon
+0000a540: 7365 2e68 7474 705f 7265 7370 6f6e 7365  se.http_response
+0000a550: 2e68 6561 6465 7273 2c0a 2020 2020 2020  .headers,.      
+0000a560: 2020 2020 2020 7374 6174 7573 3d72 6573        status=res
+0000a570: 706f 6e73 652e 6874 7470 5f72 6573 706f  ponse.http_respo
+0000a580: 6e73 652e 7374 6174 7573 0a20 2020 2020  nse.status.     
+0000a590: 2020 2029 0a0a 0a63 6c61 7373 2041 7069     )...class Api
+0000a5a0: 436c 6965 6e74 3a0a 2020 2020 2222 2247  Client:.    """G
+0000a5b0: 656e 6572 6963 2041 5049 2063 6c69 656e  eneric API clien
+0000a5c0: 7420 666f 7220 4f70 656e 4150 4920 636c  t for OpenAPI cl
+0000a5d0: 6965 6e74 206c 6962 7261 7279 2062 7569  ient library bui
+0000a5e0: 6c64 732e 0a0a 2020 2020 4f70 656e 4150  lds...    OpenAP
+0000a5f0: 4920 6765 6e65 7269 6320 4150 4920 636c  I generic API cl
+0000a600: 6965 6e74 2e20 5468 6973 2063 6c69 656e  ient. This clien
+0000a610: 7420 6861 6e64 6c65 7320 7468 6520 636c  t handles the cl
+0000a620: 6965 6e74 2d0a 2020 2020 7365 7276 6572  ient-.    server
+0000a630: 2063 6f6d 6d75 6e69 6361 7469 6f6e 2c20   communication, 
+0000a640: 616e 6420 6973 2069 6e76 6172 6961 6e74  and is invariant
+0000a650: 2061 6372 6f73 7320 696d 706c 656d 656e   across implemen
+0000a660: 7461 7469 6f6e 732e 2053 7065 6369 6669  tations. Specifi
+0000a670: 6373 206f 660a 2020 2020 7468 6520 6d65  cs of.    the me
+0000a680: 7468 6f64 7320 616e 6420 6d6f 6465 6c73  thods and models
+0000a690: 2066 6f72 2065 6163 6820 6170 706c 6963   for each applic
+0000a6a0: 6174 696f 6e20 6172 6520 6765 6e65 7261  ation are genera
+0000a6b0: 7465 6420 6672 6f6d 2074 6865 204f 7065  ted from the Ope
+0000a6c0: 6e41 5049 0a20 2020 2074 656d 706c 6174  nAPI.    templat
+0000a6d0: 6573 2e0a 0a20 2020 2054 6869 7320 636c  es...    This cl
+0000a6e0: 6173 7320 6973 2061 7574 6f20 6765 6e65  ass is auto gene
+0000a6f0: 7261 7465 640a 0a20 2020 203a 7061 7261  rated..    :para
+0000a700: 6d20 636f 6e66 6967 7572 6174 696f 6e3a  m configuration:
+0000a710: 202e 436f 6e66 6967 7572 6174 696f 6e20   .Configuration 
+0000a720: 6f62 6a65 6374 2066 6f72 2074 6869 7320  object for this 
+0000a730: 636c 6965 6e74 0a20 2020 203a 7061 7261  client.    :para
+0000a740: 6d20 6865 6164 6572 5f6e 616d 653a 2061  m header_name: a
+0000a750: 2068 6561 6465 7220 746f 2070 6173 7320   header to pass 
+0000a760: 7768 656e 206d 616b 696e 6720 6361 6c6c  when making call
+0000a770: 7320 746f 2074 6865 2041 5049 2e0a 2020  s to the API..  
+0000a780: 2020 3a70 6172 616d 2068 6561 6465 725f    :param header_
+0000a790: 7661 6c75 653a 2061 2068 6561 6465 7220  value: a header 
+0000a7a0: 7661 6c75 6520 746f 2070 6173 7320 7768  value to pass wh
+0000a7b0: 656e 206d 616b 696e 6720 6361 6c6c 7320  en making calls 
+0000a7c0: 746f 0a20 2020 2020 2020 2074 6865 2041  to.        the A
+0000a7d0: 5049 2e0a 2020 2020 3a70 6172 616d 2063  PI..    :param c
+0000a7e0: 6f6f 6b69 653a 2061 2063 6f6f 6b69 6520  ookie: a cookie 
+0000a7f0: 746f 2069 6e63 6c75 6465 2069 6e20 7468  to include in th
+0000a800: 6520 6865 6164 6572 2077 6865 6e20 6d61  e header when ma
+0000a810: 6b69 6e67 2063 616c 6c73 0a20 2020 2020  king calls.     
+0000a820: 2020 2074 6f20 7468 6520 4150 490a 2020     to the API.  
+0000a830: 2020 3a70 6172 616d 2070 6f6f 6c5f 7468    :param pool_th
+0000a840: 7265 6164 733a 2054 6865 206e 756d 6265  reads: The numbe
+0000a850: 7220 6f66 2074 6872 6561 6473 2074 6f20  r of threads to 
+0000a860: 7573 6520 666f 7220 6173 796e 6320 7265  use for async re
+0000a870: 7175 6573 7473 0a20 2020 2020 2020 2074  quests.        t
+0000a880: 6f20 7468 6520 4150 492e 204d 6f72 6520  o the API. More 
+0000a890: 7468 7265 6164 7320 6d65 616e 7320 6d6f  threads means mo
+0000a8a0: 7265 2063 6f6e 6375 7272 656e 7420 4150  re concurrent AP
+0000a8b0: 4920 7265 7175 6573 7473 2e0a 2020 2020  I requests..    
+0000a8c0: 2222 220a 0a20 2020 205f 706f 6f6c 203d  """..    _pool =
+0000a8d0: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
+0000a8e0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0000a8f0: 2073 656c 662c 0a20 2020 2020 2020 2063   self,.        c
+0000a900: 6f6e 6669 6775 7261 7469 6f6e 3a20 7479  onfiguration: ty
+0000a910: 7069 6e67 2e4f 7074 696f 6e61 6c5b 436f  ping.Optional[Co
+0000a920: 6e66 6967 7572 6174 696f 6e5d 203d 204e  nfiguration] = N
+0000a930: 6f6e 652c 0a20 2020 2020 2020 2068 6561  one,.        hea
+0000a940: 6465 725f 6e61 6d65 3a20 7479 7069 6e67  der_name: typing
+0000a950: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
+0000a960: 204e 6f6e 652c 0a20 2020 2020 2020 2068   None,.        h
+0000a970: 6561 6465 725f 7661 6c75 653a 2074 7970  eader_value: typ
+0000a980: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
+0000a990: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000a9a0: 2020 636f 6f6b 6965 3a20 7479 7069 6e67    cookie: typing
+0000a9b0: 2e4f 7074 696f 6e61 6c5b 7374 725d 203d  .Optional[str] =
+0000a9c0: 204e 6f6e 652c 0a20 2020 2020 2020 2070   None,.        p
+0000a9d0: 6f6f 6c5f 7468 7265 6164 733a 2069 6e74  ool_threads: int
+0000a9e0: 203d 2031 0a20 2020 2029 3a0a 2020 2020   = 1.    ):.    
+0000a9f0: 2020 2020 6966 2063 6f6e 6669 6775 7261      if configura
+0000aa00: 7469 6f6e 2069 7320 4e6f 6e65 3a0a 2020  tion is None:.  
+0000aa10: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000aa20: 7572 6174 696f 6e20 3d20 436f 6e66 6967  uration = Config
+0000aa30: 7572 6174 696f 6e28 290a 2020 2020 2020  uration().      
+0000aa40: 2020 7365 6c66 2e63 6f6e 6669 6775 7261    self.configura
+0000aa50: 7469 6f6e 203d 2063 6f6e 6669 6775 7261  tion = configura
+0000aa60: 7469 6f6e 0a20 2020 2020 2020 2073 656c  tion.        sel
+0000aa70: 662e 706f 6f6c 5f74 6872 6561 6473 203d  f.pool_threads =
+0000aa80: 2070 6f6f 6c5f 7468 7265 6164 730a 0a20   pool_threads.. 
+0000aa90: 2020 2020 2020 2073 656c 662e 7265 7374         self.rest
+0000aaa0: 5f63 6c69 656e 7420 3d20 7265 7374 2e52  _client = rest.R
+0000aab0: 4553 5443 6c69 656e 744f 626a 6563 7428  ESTClientObject(
+0000aac0: 636f 6e66 6967 7572 6174 696f 6e29 0a20  configuration). 
+0000aad0: 2020 2020 2020 2073 656c 662e 6465 6661         self.defa
+0000aae0: 756c 745f 6865 6164 6572 7320 3d20 4854  ult_headers = HT
+0000aaf0: 5450 4865 6164 6572 4469 6374 2829 0a20  TPHeaderDict(). 
+0000ab00: 2020 2020 2020 2069 6620 6865 6164 6572         if header
+0000ab10: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+0000ab20: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0000ab30: 656c 662e 6465 6661 756c 745f 6865 6164  elf.default_head
+0000ab40: 6572 735b 6865 6164 6572 5f6e 616d 655d  ers[header_name]
+0000ab50: 203d 2068 6561 6465 725f 7661 6c75 650a   = header_value.
+0000ab60: 2020 2020 2020 2020 7365 6c66 2e63 6f6f          self.coo
+0000ab70: 6b69 6520 3d20 636f 6f6b 6965 0a20 2020  kie = cookie.   
+0000ab80: 2020 2020 2023 2053 6574 2064 6566 6175       # Set defau
+0000ab90: 6c74 2055 7365 722d 4167 656e 742e 0a20  lt User-Agent.. 
+0000aba0: 2020 2020 2020 2073 656c 662e 7573 6572         self.user
+0000abb0: 5f61 6765 6e74 203d 2027 4b6f 6e66 6967  _agent = 'Konfig
+0000abc0: 2f34 2e34 2e30 2f70 7974 686f 6e27 0a0a  /4.4.0/python'..
+0000abd0: 2020 2020 6465 6620 5f5f 656e 7465 725f      def __enter_
+0000abe0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+0000abf0: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+0000ac00: 2020 6465 6620 5f5f 6578 6974 5f5f 2873    def __exit__(s
+0000ac10: 656c 662c 2065 7863 5f74 7970 652c 2065  elf, exc_type, e
+0000ac20: 7863 5f76 616c 7565 2c20 7472 6163 6562  xc_value, traceb
+0000ac30: 6163 6b29 3a0a 2020 2020 2020 2020 7365  ack):.        se
+0000ac40: 6c66 2e63 6c6f 7365 2829 0a0a 2020 2020  lf.close()..    
+0000ac50: 6465 6620 636c 6f73 6528 7365 6c66 293a  def close(self):
+0000ac60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000ac70: 2e5f 706f 6f6c 3a0a 2020 2020 2020 2020  ._pool:.        
+0000ac80: 2020 2020 7365 6c66 2e5f 706f 6f6c 2e63      self._pool.c
+0000ac90: 6c6f 7365 2829 0a20 2020 2020 2020 2020  lose().         
+0000aca0: 2020 2073 656c 662e 5f70 6f6f 6c2e 6a6f     self._pool.jo
+0000acb0: 696e 2829 0a20 2020 2020 2020 2020 2020  in().           
+0000acc0: 2073 656c 662e 5f70 6f6f 6c20 3d20 4e6f   self._pool = No
+0000acd0: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
+0000ace0: 6620 6861 7361 7474 7228 6174 6578 6974  f hasattr(atexit
+0000acf0: 2c20 2775 6e72 6567 6973 7465 7227 293a  , 'unregister'):
+0000ad00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ad10: 2061 7465 7869 742e 756e 7265 6769 7374   atexit.unregist
+0000ad20: 6572 2873 656c 662e 636c 6f73 6529 0a0a  er(self.close)..
+0000ad30: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+0000ad40: 2020 6465 6620 706f 6f6c 2873 656c 6629    def pool(self)
+0000ad50: 3a0a 2020 2020 2020 2020 2222 2243 7265  :.        """Cre
+0000ad60: 6174 6520 7468 7265 6164 2070 6f6f 6c20  ate thread pool 
+0000ad70: 6f6e 2066 6972 7374 2072 6571 7565 7374  on first request
+0000ad80: 0a20 2020 2020 2020 2020 6176 6f69 6473  .         avoids
+0000ad90: 2069 6e73 7461 6e74 6961 7469 6e67 2075   instantiating u
+0000ada0: 6e75 7365 6420 7468 7265 6164 706f 6f6c  nused threadpool
+0000adb0: 2066 6f72 2062 6c6f 636b 696e 6720 636c   for blocking cl
+0000adc0: 6965 6e74 732e 0a20 2020 2020 2020 2022  ients..        "
+0000add0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+0000ade0: 6c66 2e5f 706f 6f6c 2069 7320 4e6f 6e65  lf._pool is None
+0000adf0: 3a0a 2020 2020 2020 2020 2020 2020 6174  :.            at
+0000ae00: 6578 6974 2e72 6567 6973 7465 7228 7365  exit.register(se
+0000ae10: 6c66 2e63 6c6f 7365 290a 2020 2020 2020  lf.close).      
+0000ae20: 2020 2020 2020 7365 6c66 2e5f 706f 6f6c        self._pool
+0000ae30: 203d 2054 6872 6561 6450 6f6f 6c28 7365   = ThreadPool(se
+0000ae40: 6c66 2e70 6f6f 6c5f 7468 7265 6164 7329  lf.pool_threads)
+0000ae50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ae60: 7365 6c66 2e5f 706f 6f6c 0a0a 2020 2020  self._pool..    
+0000ae70: 4070 726f 7065 7274 790a 2020 2020 6465  @property.    de
+0000ae80: 6620 7573 6572 5f61 6765 6e74 2873 656c  f user_agent(sel
+0000ae90: 6629 3a0a 2020 2020 2020 2020 2222 2255  f):.        """U
+0000aea0: 7365 7220 6167 656e 7420 666f 7220 7468  ser agent for th
+0000aeb0: 6973 2041 5049 2063 6c69 656e 7422 2222  is API client"""
+0000aec0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000aed0: 7365 6c66 2e64 6566 6175 6c74 5f68 6561  self.default_hea
+0000aee0: 6465 7273 5b27 5573 6572 2d41 6765 6e74  ders['User-Agent
+0000aef0: 275d 0a0a 2020 2020 4075 7365 725f 6167  ']..    @user_ag
+0000af00: 656e 742e 7365 7474 6572 0a20 2020 2064  ent.setter.    d
+0000af10: 6566 2075 7365 725f 6167 656e 7428 7365  ef user_agent(se
+0000af20: 6c66 2c20 7661 6c75 6529 3a0a 2020 2020  lf, value):.    
+0000af30: 2020 2020 7365 6c66 2e64 6566 6175 6c74      self.default
+0000af40: 5f68 6561 6465 7273 5b27 5573 6572 2d41  _headers['User-A
+0000af50: 6765 6e74 275d 203d 2076 616c 7565 0a0a  gent'] = value..
+0000af60: 2020 2020 6465 6620 7365 745f 6465 6661      def set_defa
+0000af70: 756c 745f 6865 6164 6572 2873 656c 662c  ult_header(self,
+0000af80: 2068 6561 6465 725f 6e61 6d65 2c20 6865   header_name, he
+0000af90: 6164 6572 5f76 616c 7565 293a 0a20 2020  ader_value):.   
+0000afa0: 2020 2020 2073 656c 662e 6465 6661 756c       self.defaul
+0000afb0: 745f 6865 6164 6572 735b 6865 6164 6572  t_headers[header
+0000afc0: 5f6e 616d 655d 203d 2068 6561 6465 725f  _name] = header_
+0000afd0: 7661 6c75 650a 0a20 2020 2061 7379 6e63  value..    async
+0000afe0: 2064 6566 205f 5f61 7379 6e63 5f63 616c   def __async_cal
+0000aff0: 6c5f 6170 6928 0a20 2020 2020 2020 2073  l_api(.        s
+0000b000: 656c 662c 0a20 2020 2020 2020 2072 6573  elf,.        res
+0000b010: 6f75 7263 655f 7061 7468 3a20 7374 722c  ource_path: str,
+0000b020: 0a20 2020 2020 2020 206d 6574 686f 643a  .        method:
+0000b030: 2073 7472 2c0a 2020 2020 2020 2020 6865   str,.        he
+0000b040: 6164 6572 733a 2074 7970 696e 672e 4f70  aders: typing.Op
+0000b050: 7469 6f6e 616c 5b48 5454 5048 6561 6465  tional[HTTPHeade
+0000b060: 7244 6963 745d 203d 204e 6f6e 652c 0a20  rDict] = None,. 
+0000b070: 2020 2020 2020 2073 6572 6961 6c69 7a65         serialize
+0000b080: 645f 626f 6479 3a20 7479 7069 6e67 2e4f  d_body: typing.O
+0000b090: 7074 696f 6e61 6c5b 7479 7069 6e67 2e55  ptional[typing.U
+0000b0a0: 6e69 6f6e 5b73 7472 2c20 6279 7465 735d  nion[str, bytes]
+0000b0b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000b0c0: 2020 626f 6479 3a20 7479 7069 6e67 2e41    body: typing.A
+0000b0d0: 6e79 203d 204e 6f6e 652c 0a20 2020 2020  ny = None,.     
+0000b0e0: 2020 2066 6965 6c64 733a 2074 7970 696e     fields: typin
+0000b0f0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0000b100: 672e 5475 706c 655b 7479 7069 6e67 2e54  g.Tuple[typing.T
+0000b110: 7570 6c65 5b73 7472 2c20 7374 725d 2c20  uple[str, str], 
+0000b120: 2e2e 2e5d 5d20 3d20 4e6f 6e65 2c0a 2020  ...]] = None,.  
+0000b130: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
+0000b140: 6e67 733a 2074 7970 696e 672e 4f70 7469  ngs: typing.Opti
+0000b150: 6f6e 616c 5b74 7970 696e 672e 4c69 7374  onal[typing.List
+0000b160: 5b73 7472 5d5d 203d 204e 6f6e 652c 0a20  [str]] = None,. 
+0000b170: 2020 2020 2020 2073 7472 6561 6d3a 2062         stream: b
+0000b180: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000b190: 2020 2020 2074 696d 656f 7574 3a20 7479       timeout: ty
+0000b1a0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000b1b0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+0000b1c0: 7479 7069 6e67 2e54 7570 6c65 5d5d 203d  typing.Tuple]] =
+0000b1d0: 204e 6f6e 652c 0a20 2020 2020 2020 2068   None,.        h
+0000b1e0: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
+0000b1f0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+0000b200: 2c0a 2020 2020 2020 2020 7072 6566 6978  ,.        prefix
+0000b210: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+0000b220: 746f 723a 2050 7265 6669 7853 6570 6172  tor: PrefixSepar
+0000b230: 6174 6f72 4974 6572 6174 6f72 203d 204e  atorIterator = N
+0000b240: 6f6e 652c 0a20 2020 2029 202d 3e20 4173  one,.    ) -> As
+0000b250: 796e 6352 6573 706f 6e73 6557 7261 7070  yncResponseWrapp
+0000b260: 6572 3a0a 0a20 2020 2020 2020 2072 6571  er:..        req
+0000b270: 7565 7374 5f62 6566 6f72 655f 686f 6f6b  uest_before_hook
+0000b280: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+0000b290: 736f 7572 6365 5f70 6174 683d 7265 736f  source_path=reso
+0000b2a0: 7572 6365 5f70 6174 682c 0a20 2020 2020  urce_path,.     
+0000b2b0: 2020 2020 2020 206d 6574 686f 643d 6d65         method=me
+0000b2c0: 7468 6f64 2c0a 2020 2020 2020 2020 2020  thod,.          
+0000b2d0: 2020 636f 6e66 6967 7572 6174 696f 6e3d    configuration=
+0000b2e0: 7365 6c66 2e63 6f6e 6669 6775 7261 7469  self.configurati
+0000b2f0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0000b300: 626f 6479 3d62 6f64 792c 0a20 2020 2020  body=body,.     
+0000b310: 2020 2020 2020 2066 6965 6c64 733d 6669         fields=fi
+0000b320: 656c 6473 2c0a 2020 2020 2020 2020 2020  elds,.          
+0000b330: 2020 6175 7468 5f73 6574 7469 6e67 733d    auth_settings=
+0000b340: 6175 7468 5f73 6574 7469 6e67 732c 0a20  auth_settings,. 
+0000b350: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+0000b360: 7273 3d68 6561 6465 7273 2c0a 2020 2020  rs=headers,.    
+0000b370: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+0000b380: 2068 6561 6465 7220 7061 7261 6d65 7465   header paramete
+0000b390: 7273 0a20 2020 2020 2020 2075 7365 645f  rs.        used_
+0000b3a0: 6865 6164 6572 7320 3d20 4854 5450 4865  headers = HTTPHe
+0000b3b0: 6164 6572 4469 6374 2873 656c 662e 6465  aderDict(self.de
+0000b3c0: 6661 756c 745f 6865 6164 6572 7329 0a20  fault_headers). 
+0000b3d0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0000b3e0: 6f6f 6b69 653a 0a20 2020 2020 2020 2020  ookie:.         
+0000b3f0: 2020 2068 6561 6465 7273 5b27 436f 6f6b     headers['Cook
+0000b400: 6965 275d 203d 2073 656c 662e 636f 6f6b  ie'] = self.cook
+0000b410: 6965 0a0a 2020 2020 2020 2020 2320 6175  ie..        # au
+0000b420: 7468 2073 6574 7469 6e67 0a20 2020 2020  th setting.     
+0000b430: 2020 2072 6573 6f75 7263 655f 7061 7468     resource_path
+0000b440: 203d 2073 656c 662e 7570 6461 7465 5f70   = self.update_p
+0000b450: 6172 616d 735f 666f 725f 6175 7468 280a  arams_for_auth(.
+0000b460: 2020 2020 2020 2020 2020 2020 7573 6564              used
+0000b470: 5f68 6561 6465 7273 2c0a 2020 2020 2020  _headers,.      
+0000b480: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
+0000b490: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
+0000b4a0: 2072 6573 6f75 7263 655f 7061 7468 2c0a   resource_path,.
+0000b4b0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+0000b4c0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
+0000b4d0: 626f 6479 2c0a 2020 2020 2020 2020 2020  body,.          
+0000b4e0: 2020 7072 6566 6978 5f73 6570 6172 6174    prefix_separat
+0000b4f0: 6f72 5f69 7465 7261 746f 720a 2020 2020  or_iterator.    
+0000b500: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+0000b510: 206d 7573 7420 6861 7070 656e 2061 6674   must happen aft
+0000b520: 6572 2063 6f6f 6b69 6520 7365 7474 696e  er cookie settin
+0000b530: 6720 616e 6420 6175 7468 2073 6574 7469  g and auth setti
+0000b540: 6e67 2069 6e20 6361 7365 2075 7365 7220  ng in case user 
+0000b550: 6973 206f 7665 7272 6964 696e 6720 7468  is overriding th
+0000b560: 6f73 650a 2020 2020 2020 2020 6966 2068  ose.        if h
+0000b570: 6561 6465 7273 3a0a 2020 2020 2020 2020  eaders:.        
+0000b580: 2020 2020 7573 6564 5f68 6561 6465 7273      used_headers
+0000b590: 2e75 7064 6174 6528 6865 6164 6572 7329  .update(headers)
+0000b5a0: 0a0a 2020 2020 2020 2020 2320 7265 7175  ..        # requ
+0000b5b0: 6573 7420 7572 6c0a 2020 2020 2020 2020  est url.        
+0000b5c0: 6966 2068 6f73 7420 6973 204e 6f6e 653a  if host is None:
+0000b5d0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
+0000b5e0: 203d 2073 656c 662e 636f 6e66 6967 7572   = self.configur
+0000b5f0: 6174 696f 6e2e 686f 7374 202b 2072 6573  ation.host + res
+0000b600: 6f75 7263 655f 7061 7468 0a20 2020 2020  ource_path.     
+0000b610: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b620: 2020 2020 2023 2075 7365 2073 6572 7665       # use serve
+0000b630: 722f 686f 7374 2064 6566 696e 6564 2069  r/host defined i
+0000b640: 6e20 7061 7468 206f 7220 6f70 6572 6174  n path or operat
+0000b650: 696f 6e20 696e 7374 6561 640a 2020 2020  ion instead.    
+0000b660: 2020 2020 2020 2020 7572 6c20 3d20 686f          url = ho
+0000b670: 7374 202b 2072 6573 6f75 7263 655f 7061  st + resource_pa
+0000b680: 7468 0a0a 2020 2020 2020 2020 7265 7175  th..        requ
+0000b690: 6573 745f 6166 7465 725f 686f 6f6b 280a  est_after_hook(.
+0000b6a0: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000b6b0: 7572 6365 5f70 6174 683d 7265 736f 7572  urce_path=resour
+0000b6c0: 6365 5f70 6174 682c 0a20 2020 2020 2020  ce_path,.       
+0000b6d0: 2020 2020 206d 6574 686f 643d 6d65 7468       method=meth
+0000b6e0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
+0000b6f0: 636f 6e66 6967 7572 6174 696f 6e3d 7365  configuration=se
+0000b700: 6c66 2e63 6f6e 6669 6775 7261 7469 6f6e  lf.configuration
+0000b710: 2c0a 2020 2020 2020 2020 2020 2020 626f  ,.            bo
+0000b720: 6479 3d62 6f64 792c 0a20 2020 2020 2020  dy=body,.       
+0000b730: 2020 2020 2066 6965 6c64 733d 6669 656c       fields=fiel
+0000b740: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+0000b750: 6175 7468 5f73 6574 7469 6e67 733d 6175  auth_settings=au
+0000b760: 7468 5f73 6574 7469 6e67 732c 0a20 2020  th_settings,.   
+0000b770: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0000b780: 3d75 7365 645f 6865 6164 6572 732c 0a20  =used_headers,. 
+0000b790: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000b7a0: 2020 2320 7065 7266 6f72 6d20 7265 7175    # perform requ
+0000b7b0: 6573 7420 616e 6420 7265 7475 726e 2072  est and return r
+0000b7c0: 6573 706f 6e73 650a 2020 2020 2020 2020  esponse.        
+0000b7d0: 7265 7370 6f6e 7365 203d 2061 7761 6974  response = await
+0000b7e0: 2073 656c 662e 6173 796e 635f 7265 7175   self.async_requ
+0000b7f0: 6573 7428 0a20 2020 2020 2020 2020 2020  est(.           
+0000b800: 206d 6574 686f 642c 0a20 2020 2020 2020   method,.       
+0000b810: 2020 2020 2075 726c 2c0a 2020 2020 2020       url,.      
+0000b820: 2020 2020 2020 6865 6164 6572 733d 7573        headers=us
+0000b830: 6564 5f68 6561 6465 7273 2c0a 2020 2020  ed_headers,.    
+0000b840: 2020 2020 2020 2020 6669 656c 6473 3d66          fields=f
+0000b850: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
+0000b860: 2020 2062 6f64 793d 7365 7269 616c 697a     body=serializ
+0000b870: 6564 5f62 6f64 792c 0a20 2020 2020 2020  ed_body,.       
+0000b880: 2020 2020 2073 7472 6561 6d3d 7374 7265       stream=stre
+0000b890: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
+0000b8a0: 7469 6d65 6f75 743d 7469 6d65 6f75 742c  timeout=timeout,
+0000b8b0: 0a20 2020 2020 2020 2029 0a0a 0a20 2020  .        )...   
+0000b8c0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+0000b8d0: 6f6e 7365 0a0a 2020 2020 6465 6620 5f5f  onse..    def __
+0000b8e0: 6361 6c6c 5f61 7069 280a 2020 2020 2020  call_api(.      
+0000b8f0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0000b900: 7265 736f 7572 6365 5f70 6174 683a 2073  resource_path: s
+0000b910: 7472 2c0a 2020 2020 2020 2020 6d65 7468  tr,.        meth
+0000b920: 6f64 3a20 7374 722c 0a20 2020 2020 2020  od: str,.       
+0000b930: 2068 6561 6465 7273 3a20 7479 7069 6e67   headers: typing
+0000b940: 2e4f 7074 696f 6e61 6c5b 4854 5450 4865  .Optional[HTTPHe
+0000b950: 6164 6572 4469 6374 5d20 3d20 4e6f 6e65  aderDict] = None
+0000b960: 2c0a 2020 2020 2020 2020 7365 7269 616c  ,.        serial
+0000b970: 697a 6564 5f62 6f64 793a 2074 7970 696e  ized_body: typin
+0000b980: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0000b990: 672e 556e 696f 6e5b 7374 722c 2062 7974  g.Union[str, byt
+0000b9a0: 6573 5d5d 203d 204e 6f6e 652c 0a20 2020  es]] = None,.   
+0000b9b0: 2020 2020 2062 6f64 793a 2074 7970 696e       body: typin
+0000b9c0: 672e 416e 7920 3d20 4e6f 6e65 2c0a 2020  g.Any = None,.  
+0000b9d0: 2020 2020 2020 6669 656c 6473 3a20 7479        fields: ty
+0000b9e0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000b9f0: 7069 6e67 2e54 7570 6c65 5b74 7970 696e  ping.Tuple[typin
+0000ba00: 672e 5475 706c 655b 7374 722c 2073 7472  g.Tuple[str, str
+0000ba10: 5d2c 202e 2e2e 5d5d 203d 204e 6f6e 652c  ], ...]] = None,
+0000ba20: 0a20 2020 2020 2020 2061 7574 685f 7365  .        auth_se
+0000ba30: 7474 696e 6773 3a20 7479 7069 6e67 2e4f  ttings: typing.O
+0000ba40: 7074 696f 6e61 6c5b 7479 7069 6e67 2e4c  ptional[typing.L
+0000ba50: 6973 745b 7374 725d 5d20 3d20 4e6f 6e65  ist[str]] = None
+0000ba60: 2c0a 2020 2020 2020 2020 7374 7265 616d  ,.        stream
+0000ba70: 3a20 626f 6f6c 203d 2046 616c 7365 2c0a  : bool = False,.
+0000ba80: 2020 2020 2020 2020 7469 6d65 6f75 743a          timeout:
+0000ba90: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+0000baa0: 5b74 7970 696e 672e 556e 696f 6e5b 696e  [typing.Union[in
+0000bab0: 742c 2074 7970 696e 672e 5475 706c 655d  t, typing.Tuple]
+0000bac0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000bad0: 2020 686f 7374 3a20 7479 7069 6e67 2e4f    host: typing.O
+0000bae0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+0000baf0: 6f6e 652c 0a20 2020 2020 2020 2070 7265  one,.        pre
+0000bb00: 6669 785f 7365 7061 7261 746f 725f 6974  fix_separator_it
+0000bb10: 6572 6174 6f72 3a20 5072 6566 6978 5365  erator: PrefixSe
+0000bb20: 7061 7261 746f 7249 7465 7261 746f 7220  paratorIterator 
+0000bb30: 3d20 4e6f 6e65 2c0a 2020 2020 2920 2d3e  = None,.    ) ->
+0000bb40: 2052 6573 706f 6e73 6557 7261 7070 6572   ResponseWrapper
+0000bb50: 3a0a 0a20 2020 2020 2020 2072 6571 7565  :..        reque
+0000bb60: 7374 5f62 6566 6f72 655f 686f 6f6b 280a  st_before_hook(.
+0000bb70: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000bb80: 7572 6365 5f70 6174 683d 7265 736f 7572  urce_path=resour
+0000bb90: 6365 5f70 6174 682c 0a20 2020 2020 2020  ce_path,.       
+0000bba0: 2020 2020 206d 6574 686f 643d 6d65 7468       method=meth
+0000bbb0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
+0000bbc0: 636f 6e66 6967 7572 6174 696f 6e3d 7365  configuration=se
+0000bbd0: 6c66 2e63 6f6e 6669 6775 7261 7469 6f6e  lf.configuration
+0000bbe0: 2c0a 2020 2020 2020 2020 2020 2020 626f  ,.            bo
+0000bbf0: 6479 3d62 6f64 792c 0a20 2020 2020 2020  dy=body,.       
+0000bc00: 2020 2020 2066 6965 6c64 733d 6669 656c       fields=fiel
+0000bc10: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+0000bc20: 6175 7468 5f73 6574 7469 6e67 733d 6175  auth_settings=au
+0000bc30: 7468 5f73 6574 7469 6e67 732c 0a20 2020  th_settings,.   
+0000bc40: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0000bc50: 3d68 6561 6465 7273 2c0a 2020 2020 2020  =headers,.      
+0000bc60: 2020 290a 0a20 2020 2020 2020 2023 2068    )..        # h
+0000bc70: 6561 6465 7220 7061 7261 6d65 7465 7273  eader parameters
+0000bc80: 0a20 2020 2020 2020 2075 7365 645f 6865  .        used_he
+0000bc90: 6164 6572 7320 3d20 4854 5450 4865 6164  aders = HTTPHead
+0000bca0: 6572 4469 6374 2873 656c 662e 6465 6661  erDict(self.defa
+0000bcb0: 756c 745f 6865 6164 6572 7329 0a20 2020  ult_headers).   
+0000bcc0: 2020 2020 2069 6620 7365 6c66 2e63 6f6f       if self.coo
+0000bcd0: 6b69 653a 0a20 2020 2020 2020 2020 2020  kie:.           
+0000bce0: 2068 6561 6465 7273 5b27 436f 6f6b 6965   headers['Cookie
+0000bcf0: 275d 203d 2073 656c 662e 636f 6f6b 6965  '] = self.cookie
+0000bd00: 0a0a 2020 2020 2020 2020 2320 6175 7468  ..        # auth
+0000bd10: 2073 6574 7469 6e67 0a20 2020 2020 2020   setting.       
+0000bd20: 2072 6573 6f75 7263 655f 7061 7468 203d   resource_path =
+0000bd30: 2073 656c 662e 7570 6461 7465 5f70 6172   self.update_par
+0000bd40: 616d 735f 666f 725f 6175 7468 280a 2020  ams_for_auth(.  
+0000bd50: 2020 2020 2020 2020 2020 7573 6564 5f68            used_h
+0000bd60: 6561 6465 7273 2c0a 2020 2020 2020 2020  eaders,.        
+0000bd70: 2020 2020 6175 7468 5f73 6574 7469 6e67      auth_setting
+0000bd80: 732c 0a20 2020 2020 2020 2020 2020 2072  s,.            r
+0000bd90: 6573 6f75 7263 655f 7061 7468 2c0a 2020  esource_path,.  
+0000bda0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+0000bdb0: 2c0a 2020 2020 2020 2020 2020 2020 626f  ,.            bo
+0000bdc0: 6479 2c0a 2020 2020 2020 2020 2020 2020  dy,.            
+0000bdd0: 7072 6566 6978 5f73 6570 6172 6174 6f72  prefix_separator
+0000bde0: 5f69 7465 7261 746f 720a 2020 2020 2020  _iterator.      
+0000bdf0: 2020 290a 0a20 2020 2020 2020 2023 206d    )..        # m
+0000be00: 7573 7420 6861 7070 656e 2061 6674 6572  ust happen after
+0000be10: 2063 6f6f 6b69 6520 7365 7474 696e 6720   cookie setting 
+0000be20: 616e 6420 6175 7468 2073 6574 7469 6e67  and auth setting
+0000be30: 2069 6e20 6361 7365 2075 7365 7220 6973   in case user is
+0000be40: 206f 7665 7272 6964 696e 6720 7468 6f73   overriding thos
+0000be50: 650a 2020 2020 2020 2020 6966 2068 6561  e.        if hea
+0000be60: 6465 7273 3a0a 2020 2020 2020 2020 2020  ders:.          
+0000be70: 2020 7573 6564 5f68 6561 6465 7273 2e75    used_headers.u
+0000be80: 7064 6174 6528 6865 6164 6572 7329 0a0a  pdate(headers)..
+0000be90: 2020 2020 2020 2020 2320 7265 7175 6573          # reques
+0000bea0: 7420 7572 6c0a 2020 2020 2020 2020 6966  t url.        if
+0000beb0: 2068 6f73 7420 6973 204e 6f6e 653a 0a20   host is None:. 
+0000bec0: 2020 2020 2020 2020 2020 2075 726c 203d             url =
+0000bed0: 2073 656c 662e 636f 6e66 6967 7572 6174   self.configurat
+0000bee0: 696f 6e2e 686f 7374 202b 2072 6573 6f75  ion.host + resou
+0000bef0: 7263 655f 7061 7468 0a20 2020 2020 2020  rce_path.       
+0000bf00: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000bf10: 2020 2023 2075 7365 2073 6572 7665 722f     # use server/
+0000bf20: 686f 7374 2064 6566 696e 6564 2069 6e20  host defined in 
+0000bf30: 7061 7468 206f 7220 6f70 6572 6174 696f  path or operatio
+0000bf40: 6e20 696e 7374 6561 640a 2020 2020 2020  n instead.      
+0000bf50: 2020 2020 2020 7572 6c20 3d20 686f 7374        url = host
+0000bf60: 202b 2072 6573 6f75 7263 655f 7061 7468   + resource_path
+0000bf70: 0a0a 2020 2020 2020 2020 7265 7175 6573  ..        reques
+0000bf80: 745f 6166 7465 725f 686f 6f6b 280a 2020  t_after_hook(.  
+0000bf90: 2020 2020 2020 2020 2020 7265 736f 7572            resour
+0000bfa0: 6365 5f70 6174 683d 7265 736f 7572 6365  ce_path=resource
+0000bfb0: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0000bfc0: 2020 206d 6574 686f 643d 6d65 7468 6f64     method=method
+0000bfd0: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+0000bfe0: 6e66 6967 7572 6174 696f 6e3d 7365 6c66  nfiguration=self
+0000bff0: 2e63 6f6e 6669 6775 7261 7469 6f6e 2c0a  .configuration,.
+0000c000: 2020 2020 2020 2020 2020 2020 626f 6479              body
+0000c010: 3d62 6f64 792c 0a20 2020 2020 2020 2020  =body,.         
+0000c020: 2020 2066 6965 6c64 733d 6669 656c 6473     fields=fields
+0000c030: 2c0a 2020 2020 2020 2020 2020 2020 6175  ,.            au
+0000c040: 7468 5f73 6574 7469 6e67 733d 6175 7468  th_settings=auth
+0000c050: 5f73 6574 7469 6e67 732c 0a20 2020 2020  _settings,.     
+0000c060: 2020 2020 2020 2068 6561 6465 7273 3d75         headers=u
+0000c070: 7365 645f 6865 6164 6572 732c 0a20 2020  sed_headers,.   
+0000c080: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000c090: 2320 7065 7266 6f72 6d20 7265 7175 6573  # perform reques
+0000c0a0: 7420 616e 6420 7265 7475 726e 2072 6573  t and return res
+0000c0b0: 706f 6e73 650a 2020 2020 2020 2020 7265  ponse.        re
+0000c0c0: 7370 6f6e 7365 203d 2073 656c 662e 7265  sponse = self.re
+0000c0d0: 7175 6573 7428 0a20 2020 2020 2020 2020  quest(.         
+0000c0e0: 2020 206d 6574 686f 642c 0a20 2020 2020     method,.     
+0000c0f0: 2020 2020 2020 2075 726c 2c0a 2020 2020         url,.    
+0000c100: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
+0000c110: 7573 6564 5f68 6561 6465 7273 2c0a 2020  used_headers,.  
+0000c120: 2020 2020 2020 2020 2020 6669 656c 6473            fields
+0000c130: 3d66 6965 6c64 732c 0a20 2020 2020 2020  =fields,.       
+0000c140: 2020 2020 2062 6f64 793d 7365 7269 616c       body=serial
+0000c150: 697a 6564 5f62 6f64 792c 0a20 2020 2020  ized_body,.     
+0000c160: 2020 2020 2020 2073 7472 6561 6d3d 7374         stream=st
+0000c170: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
+0000c180: 2020 7469 6d65 6f75 743d 7469 6d65 6f75    timeout=timeou
+0000c190: 742c 0a20 2020 2020 2020 2029 0a0a 0a20  t,.        )... 
+0000c1a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000c1b0: 7370 6f6e 7365 0a0a 2020 2020 6173 796e  sponse..    asyn
+0000c1c0: 6320 6465 6620 6173 796e 635f 6361 6c6c  c def async_call
+0000c1d0: 5f61 7069 280a 2020 2020 2020 2020 7365  _api(.        se
+0000c1e0: 6c66 2c0a 2020 2020 2020 2020 7265 736f  lf,.        reso
+0000c1f0: 7572 6365 5f70 6174 683a 2073 7472 2c0a  urce_path: str,.
+0000c200: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
+0000c210: 7374 722c 0a20 2020 2020 2020 2068 6561  str,.        hea
+0000c220: 6465 7273 3a20 7479 7069 6e67 2e4f 7074  ders: typing.Opt
+0000c230: 696f 6e61 6c5b 4854 5450 4865 6164 6572  ional[HTTPHeader
+0000c240: 4469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  Dict] = None,.  
+0000c250: 2020 2020 2020 7365 7269 616c 697a 6564        serialized
+0000c260: 5f62 6f64 793a 2074 7970 696e 672e 4f70  _body: typing.Op
+0000c270: 7469 6f6e 616c 5b74 7970 696e 672e 556e  tional[typing.Un
+0000c280: 696f 6e5b 7374 722c 2062 7974 6573 5d5d  ion[str, bytes]]
+0000c290: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000c2a0: 2062 6f64 793a 2074 7970 696e 672e 416e   body: typing.An
+0000c2b0: 7920 3d20 4e6f 6e65 2c0a 2020 2020 2020  y = None,.      
+0000c2c0: 2020 6669 656c 6473 3a20 7479 7069 6e67    fields: typing
+0000c2d0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
+0000c2e0: 2e54 7570 6c65 5b74 7970 696e 672e 5475  .Tuple[typing.Tu
+0000c2f0: 706c 655b 7374 722c 2073 7472 5d2c 202e  ple[str, str], .
+0000c300: 2e2e 5d5d 203d 204e 6f6e 652c 0a20 2020  ..]] = None,.   
+0000c310: 2020 2020 2061 7574 685f 7365 7474 696e       auth_settin
+0000c320: 6773 3a20 7479 7069 6e67 2e4f 7074 696f  gs: typing.Optio
+0000c330: 6e61 6c5b 7479 7069 6e67 2e4c 6973 745b  nal[typing.List[
+0000c340: 7374 725d 5d20 3d20 4e6f 6e65 2c0a 2020  str]] = None,.  
+0000c350: 2020 2020 2020 7374 7265 616d 3a20 626f        stream: bo
+0000c360: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0000c370: 2020 2020 7469 6d65 6f75 743a 2074 7970      timeout: typ
+0000c380: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0000c390: 696e 672e 556e 696f 6e5b 696e 742c 2074  ing.Union[int, t
+0000c3a0: 7970 696e 672e 5475 706c 655d 5d20 3d20  yping.Tuple]] = 
+0000c3b0: 4e6f 6e65 2c0a 2020 2020 2020 2020 686f  None,.        ho
+0000c3c0: 7374 3a20 7479 7069 6e67 2e4f 7074 696f  st: typing.Optio
+0000c3d0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000c3e0: 0a20 2020 2020 2020 2070 7265 6669 785f  .        prefix_
+0000c3f0: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+0000c400: 6f72 3a20 5072 6566 6978 5365 7061 7261  or: PrefixSepara
+0000c410: 746f 7249 7465 7261 746f 7220 3d20 4e6f  torIterator = No
+0000c420: 6e65 2c0a 2020 2020 2920 2d3e 2041 7379  ne,.    ) -> Asy
+0000c430: 6e63 5265 7370 6f6e 7365 5772 6170 7065  ncResponseWrappe
+0000c440: 723a 0a20 2020 2020 2020 2022 2222 4d61  r:.        """Ma
+0000c450: 6b65 7320 7468 6520 4854 5450 2072 6571  kes the HTTP req
+0000c460: 7565 7374 2028 7379 6e63 6872 6f6e 6f75  uest (synchronou
+0000c470: 7329 2061 6e64 2072 6574 7572 6e73 2064  s) and returns d
+0000c480: 6573 6572 6961 6c69 7a65 6420 6461 7461  eserialized data
+0000c490: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+0000c4a0: 6d20 7265 736f 7572 6365 5f70 6174 683a  m resource_path:
+0000c4b0: 2050 6174 6820 746f 206d 6574 686f 6420   Path to method 
+0000c4c0: 656e 6470 6f69 6e74 2e0a 2020 2020 2020  endpoint..      
+0000c4d0: 2020 3a70 6172 616d 206d 6574 686f 643a    :param method:
+0000c4e0: 204d 6574 686f 6420 746f 2063 616c 6c2e   Method to call.
+0000c4f0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000c500: 6865 6164 6572 733a 2048 6561 6465 7220  headers: Header 
+0000c510: 7061 7261 6d65 7465 7273 2074 6f20 6265  parameters to be
+0000c520: 0a20 2020 2020 2020 2020 2020 2070 6c61  .            pla
+0000c530: 6365 6420 696e 2074 6865 2072 6571 7565  ced in the reque
+0000c540: 7374 2068 6561 6465 722e 0a20 2020 2020  st header..     
+0000c550: 2020 203a 7061 7261 6d20 626f 6479 3a20     :param body: 
+0000c560: 5265 7175 6573 7420 626f 6479 2e0a 2020  Request body..  
+0000c570: 2020 2020 2020 3a70 6172 616d 2066 6965        :param fie
+0000c580: 6c64 733a 2052 6571 7565 7374 2070 6f73  lds: Request pos
+0000c590: 7420 666f 726d 2070 6172 616d 6574 6572  t form parameter
+0000c5a0: 732c 0a20 2020 2020 2020 2020 2020 2066  s,.            f
+0000c5b0: 6f72 2060 6170 706c 6963 6174 696f 6e2f  or `application/
+0000c5c0: 782d 7777 772d 666f 726d 2d75 726c 656e  x-www-form-urlen
+0000c5d0: 636f 6465 6460 2c20 606d 756c 7469 7061  coded`, `multipa
+0000c5e0: 7274 2f66 6f72 6d2d 6461 7461 602e 0a20  rt/form-data`.. 
+0000c5f0: 2020 2020 2020 203a 7061 7261 6d20 6175         :param au
+0000c600: 7468 5f73 6574 7469 6e67 733a 2041 7574  th_settings: Aut
+0000c610: 6820 5365 7474 696e 6773 206e 616d 6573  h Settings names
+0000c620: 2066 6f72 2074 6865 2072 6571 7565 7374   for the request
+0000c630: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+0000c640: 2073 7472 6561 6d3a 2069 6620 5472 7565   stream: if True
+0000c650: 2c20 7468 6520 7572 6c6c 6962 332e 4854  , the urllib3.HT
+0000c660: 5450 5265 7370 6f6e 7365 206f 626a 6563  TPResponse objec
+0000c670: 7420 7769 6c6c 0a20 2020 2020 2020 2020  t will.         
+0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c690: 2020 2020 2020 2020 6265 2072 6574 7572          be retur
+0000c6a0: 6e65 6420 7769 7468 6f75 7420 7265 6164  ned without read
+0000c6b0: 696e 672f 6465 636f 6469 6e67 2072 6573  ing/decoding res
+0000c6c0: 706f 6e73 650a 2020 2020 2020 2020 2020  ponse.          
+0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6e0: 2020 2020 2020 2064 6174 612e 2041 6c73         data. Als
+0000c6f0: 6f20 7768 656e 2054 7275 652c 2069 6620  o when True, if 
+0000c700: 7468 6520 6f70 656e 6170 6920 7370 6563  the openapi spec
+0000c710: 2064 6573 6372 6962 6573 2061 2066 696c   describes a fil
+0000c720: 6520 646f 776e 6c6f 6164 2c0a 2020 2020  e download,.    
+0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c740: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000c750: 2064 6174 6120 7769 6c6c 2062 6520 7772   data will be wr
+0000c760: 6974 7465 6e20 746f 2061 206c 6f63 616c  itten to a local
+0000c770: 2066 696c 6573 7973 746d 6520 6669 6c65   filesystme file
+0000c780: 2061 6e64 2074 6865 2042 696e 6172 7953   and the BinaryS
+0000c790: 6368 656d 610a 2020 2020 2020 2020 2020  chema.          
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 2020 2069 6e73 7461 6e63 6520         instance 
+0000c7c0: 7769 6c6c 2061 6c73 6f20 696e 6865 7269  will also inheri
+0000c7d0: 7420 6672 6f6d 2046 696c 6553 6368 656d  t from FileSchem
+0000c7e0: 6120 616e 6420 4669 6c65 494f 0a20 2020  a and FileIO.   
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c800: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0000c810: 6661 756c 7420 6973 2046 616c 7365 2e0a  fault is False..
+0000c820: 2020 2020 2020 2020 3a74 7970 6520 7374          :type st
+0000c830: 7265 616d 3a20 626f 6f6c 2c20 6f70 7469  ream: bool, opti
+0000c840: 6f6e 616c 0a20 2020 2020 2020 203a 7061  onal.        :pa
+0000c850: 7261 6d20 7469 6d65 6f75 743a 2074 696d  ram timeout: tim
+0000c860: 656f 7574 2073 6574 7469 6e67 2066 6f72  eout setting for
+0000c870: 2074 6869 7320 7265 7175 6573 742e 2049   this request. I
+0000c880: 6620 6f6e 650a 2020 2020 2020 2020 2020  f one.          
+0000c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8a0: 2020 2020 2020 206e 756d 6265 7220 7072         number pr
+0000c8b0: 6f76 6964 6564 2c20 6974 2077 696c 6c20  ovided, it will 
+0000c8c0: 6265 2074 6f74 616c 2072 6571 7565 7374  be total request
+0000c8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8f0: 2020 7469 6d65 6f75 742e 2049 7420 6361    timeout. It ca
+0000c900: 6e20 616c 736f 2062 6520 6120 7061 6972  n also be a pair
+0000c910: 2028 7475 706c 6529 206f 660a 2020 2020   (tuple) of.    
+0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c930: 2020 2020 2020 2020 2020 2020 2028 636f               (co
+0000c940: 6e6e 6563 7469 6f6e 2c20 7265 6164 2920  nnection, read) 
+0000c950: 7469 6d65 6f75 7473 2e0a 2020 2020 2020  timeouts..      
+0000c960: 2020 3a70 6172 616d 2068 6f73 743a 2061    :param host: a
+0000c970: 7069 2065 6e64 706f 696e 7420 686f 7374  pi endpoint host
+0000c980: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000c990: 3a20 7265 7370 6f6e 7365 0a20 2020 2020  : response.     
+0000c9a0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000c9b0: 6574 7572 6e20 6177 6169 7420 7365 6c66  eturn await self
+0000c9c0: 2e5f 5f61 7379 6e63 5f63 616c 6c5f 6170  .__async_call_ap
+0000c9d0: 6928 0a20 2020 2020 2020 2020 2020 2072  i(.            r
+0000c9e0: 6573 6f75 7263 655f 7061 7468 2c0a 2020  esource_path,.  
+0000c9f0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+0000ca00: 2c0a 2020 2020 2020 2020 2020 2020 6865  ,.            he
+0000ca10: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+0000ca20: 2020 2073 6572 6961 6c69 7a65 645f 626f     serialized_bo
+0000ca30: 6479 2c0a 2020 2020 2020 2020 2020 2020  dy,.            
+0000ca40: 626f 6479 2c0a 2020 2020 2020 2020 2020  body,.          
+0000ca50: 2020 6669 656c 6473 2c0a 2020 2020 2020    fields,.      
+0000ca60: 2020 2020 2020 6175 7468 5f73 6574 7469        auth_setti
+0000ca70: 6e67 732c 0a20 2020 2020 2020 2020 2020  ngs,.           
+0000ca80: 2073 7472 6561 6d2c 0a20 2020 2020 2020   stream,.       
+0000ca90: 2020 2020 2074 696d 656f 7574 2c0a 2020       timeout,.  
+0000caa0: 2020 2020 2020 2020 2020 686f 7374 2c0a            host,.
+0000cab0: 2020 2020 2020 2020 2020 2020 7072 6566              pref
+0000cac0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+0000cad0: 7261 746f 722c 0a20 2020 2020 2020 2029  rator,.        )
+0000cae0: 0a0a 2020 2020 6465 6620 6361 6c6c 5f61  ..    def call_a
+0000caf0: 7069 280a 2020 2020 2020 2020 7365 6c66  pi(.        self
+0000cb00: 2c0a 2020 2020 2020 2020 7265 736f 7572  ,.        resour
+0000cb10: 6365 5f70 6174 683a 2073 7472 2c0a 2020  ce_path: str,.  
+0000cb20: 2020 2020 2020 6d65 7468 6f64 3a20 7374        method: st
+0000cb30: 722c 0a20 2020 2020 2020 2068 6561 6465  r,.        heade
+0000cb40: 7273 3a20 7479 7069 6e67 2e4f 7074 696f  rs: typing.Optio
+0000cb50: 6e61 6c5b 4854 5450 4865 6164 6572 4469  nal[HTTPHeaderDi
+0000cb60: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
+0000cb70: 2020 2020 7365 7269 616c 697a 6564 5f62      serialized_b
+0000cb80: 6f64 793a 2074 7970 696e 672e 4f70 7469  ody: typing.Opti
+0000cb90: 6f6e 616c 5b74 7970 696e 672e 556e 696f  onal[typing.Unio
+0000cba0: 6e5b 7374 722c 2062 7974 6573 5d5d 203d  n[str, bytes]] =
+0000cbb0: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+0000cbc0: 6f64 793a 2074 7970 696e 672e 416e 7920  ody: typing.Any 
+0000cbd0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+0000cbe0: 6669 656c 6473 3a20 7479 7069 6e67 2e4f  fields: typing.O
+0000cbf0: 7074 696f 6e61 6c5b 7479 7069 6e67 2e54  ptional[typing.T
+0000cc00: 7570 6c65 5b74 7970 696e 672e 5475 706c  uple[typing.Tupl
+0000cc10: 655b 7374 722c 2073 7472 5d2c 202e 2e2e  e[str, str], ...
+0000cc20: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
+0000cc30: 2020 2061 7574 685f 7365 7474 696e 6773     auth_settings
+0000cc40: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000cc50: 6c5b 7479 7069 6e67 2e4c 6973 745b 7374  l[typing.List[st
+0000cc60: 725d 5d20 3d20 4e6f 6e65 2c0a 2020 2020  r]] = None,.    
+0000cc70: 2020 2020 7374 7265 616d 3a20 626f 6f6c      stream: bool
+0000cc80: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+0000cc90: 2020 7469 6d65 6f75 743a 2074 7970 696e    timeout: typin
+0000cca0: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+0000ccb0: 672e 556e 696f 6e5b 696e 742c 2074 7970  g.Union[int, typ
+0000ccc0: 696e 672e 5475 706c 655d 5d20 3d20 4e6f  ing.Tuple]] = No
+0000ccd0: 6e65 2c0a 2020 2020 2020 2020 686f 7374  ne,.        host
+0000cce0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+0000ccf0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
+0000cd00: 2020 2020 2020 2070 7265 6669 785f 7365         prefix_se
+0000cd10: 7061 7261 746f 725f 6974 6572 6174 6f72  parator_iterator
+0000cd20: 3a20 5072 6566 6978 5365 7061 7261 746f  : PrefixSeparato
+0000cd30: 7249 7465 7261 746f 7220 3d20 4e6f 6e65  rIterator = None
+0000cd40: 2c0a 2020 2020 2920 2d3e 2052 6573 706f  ,.    ) -> Respo
+0000cd50: 6e73 6557 7261 7070 6572 3a0a 2020 2020  nseWrapper:.    
+0000cd60: 2020 2020 2222 224d 616b 6573 2074 6865      """Makes the
+0000cd70: 2048 5454 5020 7265 7175 6573 7420 2873   HTTP request (s
+0000cd80: 796e 6368 726f 6e6f 7573 2920 616e 6420  ynchronous) and 
+0000cd90: 7265 7475 726e 7320 6465 7365 7269 616c  returns deserial
+0000cda0: 697a 6564 2064 6174 612e 0a0a 2020 2020  ized data...    
+0000cdb0: 2020 2020 3a70 6172 616d 2072 6573 6f75      :param resou
+0000cdc0: 7263 655f 7061 7468 3a20 5061 7468 2074  rce_path: Path t
+0000cdd0: 6f20 6d65 7468 6f64 2065 6e64 706f 696e  o method endpoin
+0000cde0: 742e 0a20 2020 2020 2020 203a 7061 7261  t..        :para
+0000cdf0: 6d20 6d65 7468 6f64 3a20 4d65 7468 6f64  m method: Method
+0000ce00: 2074 6f20 6361 6c6c 2e0a 2020 2020 2020   to call..      
+0000ce10: 2020 3a70 6172 616d 2068 6561 6465 7273    :param headers
+0000ce20: 3a20 4865 6164 6572 2070 6172 616d 6574  : Header paramet
+0000ce30: 6572 7320 746f 2062 650a 2020 2020 2020  ers to be.      
+0000ce40: 2020 2020 2020 706c 6163 6564 2069 6e20        placed in 
+0000ce50: 7468 6520 7265 7175 6573 7420 6865 6164  the request head
+0000ce60: 6572 2e0a 2020 2020 2020 2020 3a70 6172  er..        :par
+0000ce70: 616d 2062 6f64 793a 2052 6571 7565 7374  am body: Request
+0000ce80: 2062 6f64 792e 0a20 2020 2020 2020 203a   body..        :
+0000ce90: 7061 7261 6d20 6669 656c 6473 3a20 5265  param fields: Re
+0000cea0: 7175 6573 7420 706f 7374 2066 6f72 6d20  quest post form 
+0000ceb0: 7061 7261 6d65 7465 7273 2c0a 2020 2020  parameters,.    
+0000cec0: 2020 2020 2020 2020 666f 7220 6061 7070          for `app
+0000ced0: 6c69 6361 7469 6f6e 2f78 2d77 7777 2d66  lication/x-www-f
+0000cee0: 6f72 6d2d 7572 6c65 6e63 6f64 6564 602c  orm-urlencoded`,
+0000cef0: 2060 6d75 6c74 6970 6172 742f 666f 726d   `multipart/form
+0000cf00: 2d64 6174 6160 2e0a 2020 2020 2020 2020  -data`..        
+0000cf10: 3a70 6172 616d 2061 7574 685f 7365 7474  :param auth_sett
+0000cf20: 696e 6773 3a20 4175 7468 2053 6574 7469  ings: Auth Setti
+0000cf30: 6e67 7320 6e61 6d65 7320 666f 7220 7468  ngs names for th
+0000cf40: 6520 7265 7175 6573 742e 0a20 2020 2020  e request..     
+0000cf50: 2020 203a 7061 7261 6d20 7374 7265 616d     :param stream
+0000cf60: 3a20 6966 2054 7275 652c 2074 6865 2075  : if True, the u
+0000cf70: 726c 6c69 6233 2e48 5454 5052 6573 706f  rllib3.HTTPRespo
+0000cf80: 6e73 6520 6f62 6a65 6374 2077 696c 6c0a  nse object will.
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2062 6520 7265 7475 726e 6564 2077 6974   be returned wit
+0000cfc0: 686f 7574 2072 6561 6469 6e67 2f64 6563  hout reading/dec
+0000cfd0: 6f64 696e 6720 7265 7370 6f6e 7365 0a20  oding response. 
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d000: 6461 7461 2e20 416c 736f 2077 6865 6e20  data. Also when 
+0000d010: 5472 7565 2c20 6966 2074 6865 206f 7065  True, if the ope
+0000d020: 6e61 7069 2073 7065 6320 6465 7363 7269  napi spec descri
+0000d030: 6265 7320 6120 6669 6c65 2064 6f77 6e6c  bes a file downl
+0000d040: 6f61 642c 0a20 2020 2020 2020 2020 2020  oad,.           
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 7468 6520 6461 7461 2077        the data w
+0000d070: 696c 6c20 6265 2077 7269 7474 656e 2074  ill be written t
+0000d080: 6f20 6120 6c6f 6361 6c20 6669 6c65 7379  o a local filesy
+0000d090: 7374 6d65 2066 696c 6520 616e 6420 7468  stme file and th
+0000d0a0: 6520 4269 6e61 7279 5363 6865 6d61 0a20  e BinarySchema. 
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0d0: 696e 7374 616e 6365 2077 696c 6c20 616c  instance will al
+0000d0e0: 736f 2069 6e68 6572 6974 2066 726f 6d20  so inherit from 
+0000d0f0: 4669 6c65 5363 6865 6d61 2061 6e64 2046  FileSchema and F
+0000d100: 696c 6549 4f0a 2020 2020 2020 2020 2020  ileIO.          
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2020 2020 2020 2044 6566 6175 6c74 2069         Default i
+0000d130: 7320 4661 6c73 652e 0a20 2020 2020 2020  s False..       
+0000d140: 203a 7479 7065 2073 7472 6561 6d3a 2062   :type stream: b
+0000d150: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 2020  ool, optional.  
+0000d160: 2020 2020 2020 3a70 6172 616d 2074 696d        :param tim
+0000d170: 656f 7574 3a20 7469 6d65 6f75 7420 7365  eout: timeout se
+0000d180: 7474 696e 6720 666f 7220 7468 6973 2072  tting for this r
+0000d190: 6571 7565 7374 2e20 4966 206f 6e65 0a20  equest. If one. 
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1c0: 6e75 6d62 6572 2070 726f 7669 6465 642c  number provided,
+0000d1d0: 2069 7420 7769 6c6c 2062 6520 746f 7461   it will be tota
+0000d1e0: 6c20 7265 7175 6573 740a 2020 2020 2020  l request.      
+0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d200: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
+0000d210: 7574 2e20 4974 2063 616e 2061 6c73 6f20  ut. It can also 
+0000d220: 6265 2061 2070 6169 7220 2874 7570 6c65  be a pair (tuple
+0000d230: 2920 6f66 0a20 2020 2020 2020 2020 2020  ) of.           
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 2020 2863 6f6e 6e65 6374 696f        (connectio
+0000d260: 6e2c 2072 6561 6429 2074 696d 656f 7574  n, read) timeout
+0000d270: 732e 0a20 2020 2020 2020 203a 7061 7261  s..        :para
+0000d280: 6d20 686f 7374 3a20 6170 6920 656e 6470  m host: api endp
+0000d290: 6f69 6e74 2068 6f73 740a 2020 2020 2020  oint host.      
+0000d2a0: 2020 3a72 6574 7572 6e3a 2072 6573 706f    :return: respo
+0000d2b0: 6e73 650a 2020 2020 2020 2020 2222 220a  nse.        """.
+0000d2c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0000d2d0: 656c 662e 5f5f 6361 6c6c 5f61 7069 280a  elf.__call_api(.
+0000d2e0: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+0000d2f0: 7572 6365 5f70 6174 682c 0a20 2020 2020  urce_path,.     
+0000d300: 2020 2020 2020 206d 6574 686f 642c 0a20         method,. 
+0000d310: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+0000d320: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+0000d330: 7365 7269 616c 697a 6564 5f62 6f64 792c  serialized_body,
+0000d340: 0a20 2020 2020 2020 2020 2020 2062 6f64  .            bod
+0000d350: 792c 0a20 2020 2020 2020 2020 2020 2066  y,.            f
+0000d360: 6965 6c64 732c 0a20 2020 2020 2020 2020  ields,.         
+0000d370: 2020 2061 7574 685f 7365 7474 696e 6773     auth_settings
+0000d380: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+0000d390: 7265 616d 2c0a 2020 2020 2020 2020 2020  ream,.          
+0000d3a0: 2020 7469 6d65 6f75 742c 0a20 2020 2020    timeout,.     
+0000d3b0: 2020 2020 2020 2068 6f73 742c 0a20 2020         host,.   
+0000d3c0: 2020 2020 2020 2020 2070 7265 6669 785f           prefix_
+0000d3d0: 7365 7061 7261 746f 725f 6974 6572 6174  separator_iterat
+0000d3e0: 6f72 2c0a 2020 2020 2020 2020 290a 0a20  or,.        ).. 
+0000d3f0: 2020 2064 6566 2066 6965 6c64 735f 746f     def fields_to
+0000d400: 5f64 6963 7428 7365 6c66 2c20 6669 656c  _dict(self, fiel
+0000d410: 6473 3a20 7479 7069 6e67 2e4f 7074 696f  ds: typing.Optio
+0000d420: 6e61 6c5b 7479 7069 6e67 2e54 7570 6c65  nal[typing.Tuple
+0000d430: 5b74 7970 696e 672e 5475 706c 655b 7374  [typing.Tuple[st
+0000d440: 722c 2073 7472 5d2c 202e 2e2e 5d5d 293a  r, str], ...]]):
+0000d450: 0a20 2020 2020 2020 2022 2222 436f 6e76  .        """Conv
+0000d460: 6572 7473 2066 6965 6c64 7320 746f 2064  erts fields to d
+0000d470: 6963 742e 0a0a 2020 2020 2020 2020 3a70  ict...        :p
+0000d480: 6172 616d 2066 6965 6c64 733a 2066 6965  aram fields: fie
+0000d490: 6c64 730a 2020 2020 2020 2020 3a72 6574  lds.        :ret
+0000d4a0: 7572 6e3a 2064 6963 740a 2020 2020 2020  urn: dict.      
+0000d4b0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+0000d4c0: 2066 6965 6c64 7320 6973 204e 6f6e 653a   fields is None:
+0000d4d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d4e0: 7572 6e20 4e6f 6e65 0a20 2020 2020 2020  urn None.       
+0000d4f0: 2072 6574 7572 6e20 7b6b 3a20 7620 666f   return {k: v fo
+0000d500: 7220 6b2c 2076 2069 6e20 6669 656c 6473  r k, v in fields
+0000d510: 7d0a 0a20 2020 2061 7379 6e63 2064 6566  }..    async def
+0000d520: 2061 7379 6e63 5f72 6571 7565 7374 280a   async_request(.
+0000d530: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000d540: 2020 2020 2020 6d65 7468 6f64 3a20 7374        method: st
+0000d550: 722c 0a20 2020 2020 2020 2075 726c 3a20  r,.        url: 
+0000d560: 7374 722c 0a20 2020 2020 2020 2068 6561  str,.        hea
+0000d570: 6465 7273 3a20 7479 7069 6e67 2e4f 7074  ders: typing.Opt
+0000d580: 696f 6e61 6c5b 4854 5450 4865 6164 6572  ional[HTTPHeader
+0000d590: 4469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  Dict] = None,.  
+0000d5a0: 2020 2020 2020 6669 656c 6473 3a20 7479        fields: ty
+0000d5b0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000d5c0: 7069 6e67 2e54 7570 6c65 5b74 7970 696e  ping.Tuple[typin
+0000d5d0: 672e 5475 706c 655b 7374 722c 2073 7472  g.Tuple[str, str
+0000d5e0: 5d2c 202e 2e2e 5d5d 203d 204e 6f6e 652c  ], ...]] = None,
+0000d5f0: 0a20 2020 2020 2020 2062 6f64 793a 2074  .        body: t
+0000d600: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0000d610: 7970 696e 672e 556e 696f 6e5b 7374 722c  yping.Union[str,
+0000d620: 2062 7974 6573 5d5d 203d 204e 6f6e 652c   bytes]] = None,
+0000d630: 0a20 2020 2020 2020 2073 7472 6561 6d3a  .        stream:
+0000d640: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+0000d650: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
+0000d660: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+0000d670: 7479 7069 6e67 2e55 6e69 6f6e 5b69 6e74  typing.Union[int
+0000d680: 2c20 7479 7069 6e67 2e54 7570 6c65 5d5d  , typing.Tuple]]
+0000d690: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
+0000d6a0: 3e20 4173 796e 6352 6573 706f 6e73 6557  > AsyncResponseW
+0000d6b0: 7261 7070 6572 3a0a 2020 2020 2020 2020  rapper:.        
+0000d6c0: 6966 2062 6f64 7920 616e 6420 6669 656c  if body and fiel
+0000d6d0: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
+0000d6e0: 7261 6973 6520 4170 6956 616c 7565 4572  raise ApiValueEr
+0000d6f0: 726f 7228 2262 6f64 7920 7061 7261 6d65  ror("body parame
+0000d700: 7465 7220 6361 6e6e 6f74 2062 6520 7573  ter cannot be us
+0000d710: 6564 2077 6974 6820 6669 656c 6473 2070  ed with fields p
+0000d720: 6172 616d 6574 6572 2229 0a20 2020 2020  arameter").     
+0000d730: 2020 2064 6174 6120 3d20 4e6f 6e65 0a20     data = None. 
+0000d740: 2020 2020 2020 2069 6620 626f 6479 3a0a         if body:.
+0000d750: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000d760: 3d62 6f64 790a 2020 2020 2020 2020 6966  =body.        if
+0000d770: 2066 6965 6c64 733a 0a20 2020 2020 2020   fields:.       
+0000d780: 2020 2020 2064 6174 613d 7365 6c66 2e66       data=self.f
+0000d790: 6965 6c64 735f 746f 5f64 6963 7428 6669  ields_to_dict(fi
+0000d7a0: 656c 6473 290a 2020 2020 2020 2020 7365  elds).        se
+0000d7b0: 7373 696f 6e20 3d20 6169 6f68 7474 702e  ssion = aiohttp.
+0000d7c0: 436c 6965 6e74 5365 7373 696f 6e28 290a  ClientSession().
+0000d7d0: 2020 2020 2020 2020 7431 203d 2074 696d          t1 = tim
+0000d7e0: 652e 7469 6d65 2829 0a20 2020 2020 2020  e.time().       
+0000d7f0: 2069 6620 6d65 7468 6f64 203d 3d20 2247   if method == "G
+0000d800: 4554 223a 0a20 2020 2020 2020 2020 2020  ET":.           
+0000d810: 2073 6573 7369 6f6e 2e67 6574 2875 726c   session.get(url
+0000d820: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0000d830: 7370 6f6e 7365 203d 2061 7761 6974 2073  sponse = await s
+0000d840: 6573 7369 6f6e 2e67 6574 2875 726c 2c20  ession.get(url, 
+0000d850: 6865 6164 6572 733d 6865 6164 6572 7329  headers=headers)
+0000d860: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000d870: 7572 6e20 4173 796e 6352 6573 706f 6e73  urn AsyncRespons
+0000d880: 6557 7261 7070 6572 2872 6573 706f 6e73  eWrapper(respons
+0000d890: 652c 2074 696d 652e 7469 6d65 2829 202d  e, time.time() -
+0000d8a0: 2074 312c 2073 6573 7369 6f6e 290a 2020   t1, session).  
+0000d8b0: 2020 2020 2020 656c 6966 206d 6574 686f        elif metho
+0000d8c0: 6420 3d3d 2022 4845 4144 223a 0a20 2020  d == "HEAD":.   
+0000d8d0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+0000d8e0: 6520 3d20 6177 6169 7420 7365 7373 696f  e = await sessio
+0000d8f0: 6e2e 6865 6164 2875 726c 2c20 6865 6164  n.head(url, head
+0000d900: 6572 733d 6865 6164 6572 7329 0a20 2020  ers=headers).   
+0000d910: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d920: 4173 796e 6352 6573 706f 6e73 6557 7261  AsyncResponseWra
+0000d930: 7070 6572 2872 6573 706f 6e73 652c 2074  pper(response, t
+0000d940: 696d 652e 7469 6d65 2829 202d 2074 312c  ime.time() - t1,
+0000d950: 2073 6573 7369 6f6e 290a 2020 2020 2020   session).      
+0000d960: 2020 656c 6966 206d 6574 686f 6420 3d3d    elif method ==
+0000d970: 2022 4f50 5449 4f4e 5322 3a0a 2020 2020   "OPTIONS":.    
+0000d980: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0000d990: 203d 2061 7761 6974 2073 6573 7369 6f6e   = await session
+0000d9a0: 2e6f 7074 696f 6e73 2875 726c 2c20 6461  .options(url, da
+0000d9b0: 7461 3d64 6174 612c 2068 6561 6465 7273  ta=data, headers
+0000d9c0: 3d68 6561 6465 7273 290a 2020 2020 2020  =headers).      
+0000d9d0: 2020 2020 2020 7265 7475 726e 2041 7379        return Asy
+0000d9e0: 6e63 5265 7370 6f6e 7365 5772 6170 7065  ncResponseWrappe
+0000d9f0: 7228 7265 7370 6f6e 7365 2c20 7469 6d65  r(response, time
+0000da00: 2e74 696d 6528 2920 2d20 7431 2c20 7365  .time() - t1, se
+0000da10: 7373 696f 6e29 0a20 2020 2020 2020 2065  ssion).        e
+0000da20: 6c69 6620 6d65 7468 6f64 203d 3d20 2250  lif method == "P
+0000da30: 4f53 5422 3a0a 2020 2020 2020 2020 2020  OST":.          
+0000da40: 2020 7265 7370 6f6e 7365 203d 2061 7761    response = awa
+0000da50: 6974 2073 6573 7369 6f6e 2e70 6f73 7428  it session.post(
+0000da60: 7572 6c2c 2064 6174 613d 6461 7461 2c20  url, data=data, 
+0000da70: 6865 6164 6572 733d 6865 6164 6572 7329  headers=headers)
+0000da80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000da90: 7572 6e20 4173 796e 6352 6573 706f 6e73  urn AsyncRespons
+0000daa0: 6557 7261 7070 6572 2872 6573 706f 6e73  eWrapper(respons
+0000dab0: 652c 2074 696d 652e 7469 6d65 2829 202d  e, time.time() -
+0000dac0: 2074 312c 2073 6573 7369 6f6e 290a 2020   t1, session).  
+0000dad0: 2020 2020 2020 656c 6966 206d 6574 686f        elif metho
+0000dae0: 6420 3d3d 2022 5055 5422 3a0a 2020 2020  d == "PUT":.    
+0000daf0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+0000db00: 203d 2061 7761 6974 2073 6573 7369 6f6e   = await session
+0000db10: 2e70 7574 2875 726c 2c20 6461 7461 3d64  .put(url, data=d
+0000db20: 6174 612c 2068 6561 6465 7273 3d68 6561  ata, headers=hea
+0000db30: 6465 7273 290a 2020 2020 2020 2020 2020  ders).          
+0000db40: 2020 7265 7475 726e 2041 7379 6e63 5265    return AsyncRe
+0000db50: 7370 6f6e 7365 5772 6170 7065 7228 7265  sponseWrapper(re
+0000db60: 7370 6f6e 7365 2c20 7469 6d65 2e74 696d  sponse, time.tim
+0000db70: 6528 2920 2d20 7431 2c20 7365 7373 696f  e() - t1, sessio
+0000db80: 6e29 0a20 2020 2020 2020 2065 6c69 6620  n).        elif 
+0000db90: 6d65 7468 6f64 203d 3d20 2250 4154 4348  method == "PATCH
+0000dba0: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
+0000dbb0: 6573 706f 6e73 6520 3d20 6177 6169 7420  esponse = await 
+0000dbc0: 7365 7373 696f 6e2e 7061 7463 6828 7572  session.patch(ur
+0000dbd0: 6c2c 2064 6174 613d 6461 7461 2c20 6865  l, data=data, he
+0000dbe0: 6164 6572 733d 6865 6164 6572 7329 0a20  aders=headers). 
+0000dbf0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000dc00: 6e20 4173 796e 6352 6573 706f 6e73 6557  n AsyncResponseW
+0000dc10: 7261 7070 6572 2872 6573 706f 6e73 652c  rapper(response,
+0000dc20: 2074 696d 652e 7469 6d65 2829 202d 2074   time.time() - t
+0000dc30: 312c 2073 6573 7369 6f6e 290a 2020 2020  1, session).    
+0000dc40: 2020 2020 656c 6966 206d 6574 686f 6420      elif method 
+0000dc50: 3d3d 2022 4445 4c45 5445 223a 0a20 2020  == "DELETE":.   
+0000dc60: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+0000dc70: 6520 3d20 6177 6169 7420 7365 7373 696f  e = await sessio
+0000dc80: 6e2e 6465 6c65 7465 2875 726c 2c20 6461  n.delete(url, da
+0000dc90: 7461 3d64 6174 612c 2068 6561 6465 7273  ta=data, headers
+0000dca0: 3d68 6561 6465 7273 290a 2020 2020 2020  =headers).      
+0000dcb0: 2020 2020 2020 7265 7475 726e 2041 7379        return Asy
+0000dcc0: 6e63 5265 7370 6f6e 7365 5772 6170 7065  ncResponseWrappe
+0000dcd0: 7228 7265 7370 6f6e 7365 2c20 7469 6d65  r(response, time
+0000dce0: 2e74 696d 6528 2920 2d20 7431 2c20 7365  .time() - t1, se
+0000dcf0: 7373 696f 6e29 0a20 2020 2020 2020 2072  ssion).        r
+0000dd00: 6169 7365 2041 7069 5661 6c75 6545 7272  aise ApiValueErr
+0000dd10: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000dd20: 2268 7474 7020 6d65 7468 6f64 206d 7573  "http method mus
+0000dd30: 7420 6265 2060 4745 5460 2c20 6048 4541  t be `GET`, `HEA
+0000dd40: 4460 2c20 604f 5054 494f 4e53 602c 220a  D`, `OPTIONS`,".
+0000dd50: 2020 2020 2020 2020 2020 2020 2220 6050              " `P
+0000dd60: 4f53 5460 2c20 6050 4154 4348 602c 2060  OST`, `PATCH`, `
+0000dd70: 5055 5460 206f 7220 6044 454c 4554 4560  PUT` or `DELETE`
+0000dd80: 2e22 0a20 2020 2020 2020 2029 0a0a 2020  .".        )..  
+0000dd90: 2020 6465 6620 7265 7175 6573 7428 0a20    def request(. 
+0000dda0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000ddb0: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
+0000ddc0: 2c0a 2020 2020 2020 2020 7572 6c3a 2073  ,.        url: s
+0000ddd0: 7472 2c0a 2020 2020 2020 2020 6865 6164  tr,.        head
+0000dde0: 6572 733a 2074 7970 696e 672e 4f70 7469  ers: typing.Opti
+0000ddf0: 6f6e 616c 5b48 5454 5048 6561 6465 7244  onal[HTTPHeaderD
+0000de00: 6963 745d 203d 204e 6f6e 652c 0a20 2020  ict] = None,.   
+0000de10: 2020 2020 2066 6965 6c64 733a 2074 7970       fields: typ
+0000de20: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
+0000de30: 696e 672e 5475 706c 655b 7479 7069 6e67  ing.Tuple[typing
+0000de40: 2e54 7570 6c65 5b73 7472 2c20 7374 725d  .Tuple[str, str]
+0000de50: 2c20 2e2e 2e5d 5d20 3d20 4e6f 6e65 2c0a  , ...]] = None,.
+0000de60: 2020 2020 2020 2020 626f 6479 3a20 7479          body: ty
+0000de70: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+0000de80: 7069 6e67 2e55 6e69 6f6e 5b73 7472 2c20  ping.Union[str, 
+0000de90: 6279 7465 735d 5d20 3d20 4e6f 6e65 2c0a  bytes]] = None,.
+0000dea0: 2020 2020 2020 2020 7374 7265 616d 3a20          stream: 
+0000deb0: 626f 6f6c 203d 2046 616c 7365 2c0a 2020  bool = False,.  
+0000dec0: 2020 2020 2020 7469 6d65 6f75 743a 2074        timeout: t
+0000ded0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+0000dee0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+0000def0: 2074 7970 696e 672e 5475 706c 655d 5d20   typing.Tuple]] 
+0000df00: 3d20 4e6f 6e65 2c0a 2020 2020 2920 2d3e  = None,.    ) ->
+0000df10: 2052 6573 706f 6e73 6557 7261 7070 6572   ResponseWrapper
+0000df20: 3a0a 2020 2020 2020 2020 2222 224d 616b  :.        """Mak
+0000df30: 6573 2074 6865 2048 5454 5020 7265 7175  es the HTTP requ
+0000df40: 6573 7420 7573 696e 6720 5245 5354 436c  est using RESTCl
+0000df50: 6965 6e74 2e22 2222 0a20 2020 2020 2020  ient.""".       
+0000df60: 2069 6620 6d65 7468 6f64 203d 3d20 2247   if method == "G
+0000df70: 4554 223a 0a20 2020 2020 2020 2020 2020  ET":.           
+0000df80: 2072 6574 7572 6e20 7365 6c66 2e72 6573   return self.res
+0000df90: 745f 636c 6965 6e74 2e47 4554 2875 726c  t_client.GET(url
+0000dfa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfc0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
+0000dfd0: 3d73 7472 6561 6d2c 0a20 2020 2020 2020  =stream,.       
+0000dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e000: 2074 696d 656f 7574 3d74 696d 656f 7574   timeout=timeout
+0000e010: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e030: 2020 2020 2020 2020 2020 6865 6164 6572            header
+0000e040: 733d 6865 6164 6572 7329 0a20 2020 2020  s=headers).     
+0000e050: 2020 2065 6c69 6620 6d65 7468 6f64 203d     elif method =
+0000e060: 3d20 2248 4541 4422 3a0a 2020 2020 2020  = "HEAD":.      
+0000e070: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0000e080: 662e 7265 7374 5f63 6c69 656e 742e 4845  f.rest_client.HE
+0000e090: 4144 2875 726c 2c0a 2020 2020 2020 2020  AD(url,.        
+0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0c0: 2073 7472 6561 6d3d 7374 7265 616d 2c0a   stream=stream,.
+0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0f0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+0000e100: 3d74 696d 656f 7574 2c0a 2020 2020 2020  =timeout,.      
+0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e130: 2020 2068 6561 6465 7273 3d68 6561 6465     headers=heade
+0000e140: 7273 290a 2020 2020 2020 2020 656c 6966  rs).        elif
+0000e150: 206d 6574 686f 6420 3d3d 2022 4f50 5449   method == "OPTI
+0000e160: 4f4e 5322 3a0a 2020 2020 2020 2020 2020  ONS":.          
+0000e170: 2020 7265 7475 726e 2073 656c 662e 7265    return self.re
+0000e180: 7374 5f63 6c69 656e 742e 4f50 5449 4f4e  st_client.OPTION
+0000e190: 5328 7572 6c2c 0a20 2020 2020 2020 2020  S(url,.         
+0000e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1c0: 2020 2068 6561 6465 7273 3d68 6561 6465     headers=heade
+0000e1d0: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+0000e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e200: 6669 656c 6473 3d66 6965 6c64 732c 0a20  fields=fields,. 
+0000e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e230: 2020 2020 2020 2020 2020 2073 7472 6561             strea
+0000e240: 6d3d 7374 7265 616d 2c0a 2020 2020 2020  m=stream,.      
+0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e270: 2020 2020 2020 7469 6d65 6f75 743d 7469        timeout=ti
+0000e280: 6d65 6f75 742c 0a20 2020 2020 2020 2020  meout,.         
+0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2b0: 2020 2062 6f64 793d 626f 6479 290a 2020     body=body).  
+0000e2c0: 2020 2020 2020 656c 6966 206d 6574 686f        elif metho
+0000e2d0: 6420 3d3d 2022 504f 5354 223a 0a20 2020  d == "POST":.   
+0000e2e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000e2f0: 7365 6c66 2e72 6573 745f 636c 6965 6e74  self.rest_client
+0000e300: 2e50 4f53 5428 7572 6c2c 0a20 2020 2020  .POST(url,.     
+0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e330: 2020 2020 6865 6164 6572 733d 6865 6164      headers=head
+0000e340: 6572 732c 0a20 2020 2020 2020 2020 2020  ers,.           
 0000e350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e360: 6e61 6d65 3d6b 6579 2c0a 2020 2020 2020  name=key,.      
-0000e370: 2020 2020 2020 2020 2020 6461 7461 3d76            data=v
-0000e380: 616c 7565 2e72 6561 6428 292c 0a20 2020  alue.read(),.   
-0000e390: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-0000e3a0: 656e 616d 653d 6669 6c65 6e61 6d65 2c0a  ename=filename,.
-0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3c0: 6865 6164 6572 733d 7b27 436f 6e74 656e  headers={'Conten
-0000e3d0: 742d 5479 7065 273a 2067 7565 7373 5f63  t-Type': guess_c
-0000e3e0: 6f6e 7465 6e74 5f74 7970 6528 6669 6c65  ontent_type(file
-0000e3f0: 6e61 6d65 297d 0a20 2020 2020 2020 2020  name)}.         
-0000e400: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000e410: 2076 616c 7565 2e63 6c6f 7365 2829 0a20   value.close(). 
-0000e420: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e430: 6e20 7265 7175 6573 745f 6669 656c 640a  n request_field.
-0000e440: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e450: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e460: 2073 656c 662e 5f5f 6d75 6c74 6970 6172   self.__multipar
-0000e470: 745f 6a73 6f6e 5f69 7465 6d28 6b65 793d  t_json_item(key=
-0000e480: 6b65 792c 2076 616c 7565 3d76 616c 7565  key, value=value
-0000e490: 290a 0a20 2020 2064 6566 205f 5f73 6572  )..    def __ser
-0000e4a0: 6961 6c69 7a65 5f6d 756c 7469 7061 7274  ialize_multipart
-0000e4b0: 5f66 6f72 6d5f 6461 7461 280a 2020 2020  _form_data(.    
-0000e4c0: 2020 2020 7365 6c66 2c20 696e 5f64 6174      self, in_dat
-0000e4d0: 613a 2053 6368 656d 610a 2020 2020 2920  a: Schema.    ) 
-0000e4e0: 2d3e 2074 7970 696e 672e 4469 6374 5b73  -> typing.Dict[s
-0000e4f0: 7472 2c20 7479 7069 6e67 2e54 7570 6c65  tr, typing.Tuple
-0000e500: 5b52 6571 7565 7374 4669 656c 642c 202e  [RequestField, .
-0000e510: 2e2e 5d5d 3a0a 2020 2020 2020 2020 6966  ..]]:.        if
-0000e520: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0000e530: 696e 5f64 6174 612c 2066 726f 7a65 6e64  in_data, frozend
-0000e540: 6963 742e 6672 6f7a 656e 6469 6374 293a  ict.frozendict):
-0000e550: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0000e560: 7365 2056 616c 7565 4572 726f 7228 6627  se ValueError(f'
-0000e570: 556e 6162 6c65 2074 6f20 7365 7269 616c  Unable to serial
-0000e580: 697a 6520 7b69 6e5f 6461 7461 7d20 746f  ize {in_data} to
-0000e590: 206d 756c 7469 7061 7274 2f66 6f72 6d2d   multipart/form-
-0000e5a0: 6461 7461 2062 6563 6175 7365 2069 7420  data because it 
-0000e5b0: 6973 206e 6f74 2061 2064 6963 7420 6f66  is not a dict of
-0000e5c0: 2064 6174 6127 290a 2020 2020 2020 2020   data').        
-0000e5d0: 2222 220a 2020 2020 2020 2020 496e 2061  """.        In a
-0000e5e0: 206d 756c 7469 7061 7274 2f66 6f72 6d2d   multipart/form-
-0000e5f0: 6461 7461 2072 6571 7565 7374 2062 6f64  data request bod
-0000e600: 792c 2065 6163 6820 7363 6865 6d61 2070  y, each schema p
-0000e610: 726f 7065 7274 792c 206f 7220 6561 6368  roperty, or each
-0000e620: 2065 6c65 6d65 6e74 206f 6620 6120 7363   element of a sc
-0000e630: 6865 6d61 2061 7272 6179 2070 726f 7065  hema array prope
-0000e640: 7274 792c 0a20 2020 2020 2020 2074 616b  rty,.        tak
-0000e650: 6573 2061 2073 6563 7469 6f6e 2069 6e20  es a section in 
-0000e660: 7468 6520 7061 796c 6f61 6420 7769 7468  the payload with
-0000e670: 2061 6e20 696e 7465 726e 616c 2068 6561   an internal hea
-0000e680: 6465 7220 6173 2064 6566 696e 6564 2062  der as defined b
-0000e690: 7920 5246 4337 3537 382e 2054 6865 2073  y RFC7578. The s
-0000e6a0: 6572 6961 6c69 7a61 7469 6f6e 2073 7472  erialization str
-0000e6b0: 6174 6567 790a 2020 2020 2020 2020 666f  ategy.        fo
-0000e6c0: 7220 6561 6368 2070 726f 7065 7274 7920  r each property 
-0000e6d0: 6f66 2061 206d 756c 7469 7061 7274 2f66  of a multipart/f
-0000e6e0: 6f72 6d2d 6461 7461 2072 6571 7565 7374  orm-data request
-0000e6f0: 2062 6f64 7920 6361 6e20 6265 2073 7065   body can be spe
-0000e700: 6369 6669 6564 2069 6e20 616e 2061 7373  cified in an ass
-0000e710: 6f63 6961 7465 6420 456e 636f 6469 6e67  ociated Encoding
-0000e720: 204f 626a 6563 742e 0a0a 2020 2020 2020   Object...      
-0000e730: 2020 5768 656e 2070 6173 7369 6e67 2069    When passing i
-0000e740: 6e20 6d75 6c74 6970 6172 7420 7479 7065  n multipart type
-0000e750: 732c 2062 6f75 6e64 6172 6965 7320 4d41  s, boundaries MA
-0000e760: 5920 6265 2075 7365 6420 746f 2073 6570  Y be used to sep
-0000e770: 6172 6174 6520 7365 6374 696f 6e73 206f  arate sections o
-0000e780: 6620 7468 6520 636f 6e74 656e 7420 6265  f the content be
-0000e790: 696e 670a 2020 2020 2020 2020 7472 616e  ing.        tran
-0000e7a0: 7366 6572 7265 6420 e280 9320 7468 7573  sferred ... thus
-0000e7b0: 2c20 7468 6520 666f 6c6c 6f77 696e 6720  , the following 
-0000e7c0: 6465 6661 756c 7420 436f 6e74 656e 742d  default Content-
-0000e7d0: 5479 7065 7320 6172 6520 6465 6669 6e65  Types are define
-0000e7e0: 6420 666f 7220 6d75 6c74 6970 6172 743a  d for multipart:
-0000e7f0: 0a0a 2020 2020 2020 2020 4966 2074 6865  ..        If the
-0000e800: 2028 6f62 6a65 6374 2920 7072 6f70 6572   (object) proper
-0000e810: 7479 2069 7320 6120 7072 696d 6974 6976  ty is a primitiv
-0000e820: 652c 206f 7220 616e 2061 7272 6179 206f  e, or an array o
-0000e830: 6620 7072 696d 6974 6976 6520 7661 6c75  f primitive valu
-0000e840: 6573 2c20 7468 6520 6465 6661 756c 7420  es, the default 
-0000e850: 436f 6e74 656e 742d 5479 7065 2069 7320  Content-Type is 
-0000e860: 7465 7874 2f70 6c61 696e 0a20 2020 2020  text/plain.     
-0000e870: 2020 2049 6620 7468 6520 7072 6f70 6572     If the proper
-0000e880: 7479 2069 7320 636f 6d70 6c65 782c 206f  ty is complex, o
-0000e890: 7220 616e 2061 7272 6179 206f 6620 636f  r an array of co
-0000e8a0: 6d70 6c65 7820 7661 6c75 6573 2c20 7468  mplex values, th
-0000e8b0: 6520 6465 6661 756c 7420 436f 6e74 656e  e default Conten
-0000e8c0: 742d 5479 7065 2069 7320 6170 706c 6963  t-Type is applic
-0000e8d0: 6174 696f 6e2f 6a73 6f6e 0a20 2020 2020  ation/json.     
-0000e8e0: 2020 2020 2020 2051 7565 7374 696f 6e3a         Question:
-0000e8f0: 2068 6f77 2069 7320 7468 6520 6172 7261   how is the arra
-0000e900: 7920 6f66 2070 7269 6d69 7469 7665 7320  y of primitives 
-0000e910: 656e 636f 6465 643f 0a20 2020 2020 2020  encoded?.       
-0000e920: 2049 6620 7468 6520 7072 6f70 6572 7479   If the property
-0000e930: 2069 7320 6120 7479 7065 3a20 7374 7269   is a type: stri
-0000e940: 6e67 2077 6974 6820 6120 636f 6e74 656e  ng with a conten
-0000e950: 7445 6e63 6f64 696e 672c 2074 6865 2064  tEncoding, the d
-0000e960: 6566 6175 6c74 2043 6f6e 7465 6e74 2d54  efault Content-T
-0000e970: 7970 6520 6973 2061 7070 6c69 6361 7469  ype is applicati
-0000e980: 6f6e 2f6f 6374 6574 2d73 7472 6561 6d0a  on/octet-stream.
-0000e990: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000e9a0: 2020 2020 6669 656c 6473 3a20 7479 7069      fields: typi
-0000e9b0: 6e67 2e4c 6973 745b 5265 7175 6573 7446  ng.List[RequestF
-0000e9c0: 6965 6c64 5d20 3d20 5b5d 0a20 2020 2020  ield] = [].     
-0000e9d0: 2020 2066 6f72 206b 6579 2c20 7661 6c75     for key, valu
-0000e9e0: 6520 696e 2069 6e5f 6461 7461 2e69 7465  e in in_data.ite
-0000e9f0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000ea00: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-0000ea10: 7661 6c75 652c 2074 7570 6c65 293a 0a20  value, tuple):. 
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ea30: 6620 7661 6c75 653a 0a20 2020 2020 2020  f value:.       
-0000ea40: 2020 2020 2020 2020 2020 2020 2023 2076               # v
-0000ea50: 616c 7565 7320 7573 6520 6578 706c 6f64  alues use explod
-0000ea60: 6520 3d20 5472 7565 2c20 736f 2074 6865  e = True, so the
-0000ea70: 2063 6f64 6520 6d61 6b65 7320 6120 5265   code makes a Re
-0000ea80: 7175 6573 7446 6965 6c64 2066 6f72 2065  questField for e
-0000ea90: 6163 6820 6974 656d 2077 6974 6820 6e61  ach item with na
-0000eaa0: 6d65 3d6b 6579 0a20 2020 2020 2020 2020  me=key.         
-0000eab0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000eac0: 7465 6d20 696e 2076 616c 7565 3a0a 2020  tem in value:.  
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2020 2020 2020 7265 7175 6573 745f 6669        request_fi
-0000eaf0: 656c 6420 3d20 7365 6c66 2e5f 5f6d 756c  eld = self.__mul
-0000eb00: 7469 7061 7274 5f66 6f72 6d5f 6974 656d  tipart_form_item
-0000eb10: 286b 6579 3d6b 6579 2c20 7661 6c75 653d  (key=key, value=
-0000eb20: 6974 656d 290a 2020 2020 2020 2020 2020  item).          
-0000eb30: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-0000eb40: 656c 6473 2e61 7070 656e 6428 7265 7175  elds.append(requ
-0000eb50: 6573 745f 6669 656c 6429 0a20 2020 2020  est_field).     
-0000eb60: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000eb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eb80: 2020 2020 2023 2073 656e 6420 616e 2065       # send an e
-0000eb90: 6d70 7479 2061 7272 6179 2061 7320 6a73  mpty array as js
-0000eba0: 6f6e 2062 6563 6175 7365 2065 7870 6c6f  on because explo
-0000ebb0: 6469 6e67 2077 696c 6c20 6e6f 7420 7365  ding will not se
-0000ebc0: 6e64 2069 740a 2020 2020 2020 2020 2020  nd it.          
-0000ebd0: 2020 2020 2020 2020 2020 7265 7175 6573            reques
-0000ebe0: 745f 6669 656c 6420 3d20 7365 6c66 2e5f  t_field = self._
-0000ebf0: 5f6d 756c 7469 7061 7274 5f6a 736f 6e5f  _multipart_json_
-0000ec00: 6974 656d 286b 6579 3d6b 6579 2c20 7661  item(key=key, va
-0000ec10: 6c75 653d 7661 6c75 6529 0a20 2020 2020  lue=value).     
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ec30: 6965 6c64 732e 6170 7065 6e64 2872 6571  ields.append(req
-0000ec40: 7565 7374 5f66 6965 6c64 290a 2020 2020  uest_field).    
-0000ec50: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000ec70: 7175 6573 745f 6669 656c 6420 3d20 7365  quest_field = se
-0000ec80: 6c66 2e5f 5f6d 756c 7469 7061 7274 5f66  lf.__multipart_f
-0000ec90: 6f72 6d5f 6974 656d 286b 6579 3d6b 6579  orm_item(key=key
-0000eca0: 2c20 7661 6c75 653d 7661 6c75 6529 0a20  , value=value). 
-0000ecb0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ecc0: 6965 6c64 732e 6170 7065 6e64 2872 6571  ields.append(req
-0000ecd0: 7565 7374 5f66 6965 6c64 290a 0a20 2020  uest_field)..   
-0000ece0: 2020 2020 2023 2054 6869 7320 6973 206e       # This is n
-0000ecf0: 6563 6573 7361 7279 2074 6f20 6669 6c6c  ecessary to fill
-0000ed00: 2074 6865 2022 436f 6e74 656e 742d 4469   the "Content-Di
-0000ed10: 7370 6f73 6974 696f 6e22 2068 6561 6465  sposition" heade
-0000ed20: 7220 6e65 6564 6564 2066 6f72 206e 616d  r needed for nam
-0000ed30: 696e 6720 6669 656c 6473 2069 6e20 6d75  ing fields in mu
-0000ed40: 6c74 6970 6172 740a 2020 2020 2020 2020  ltipart.        
-0000ed50: 666f 7220 6669 656c 6420 696e 2066 6965  for field in fie
-0000ed60: 6c64 733a 0a20 2020 2020 2020 2020 2020  lds:.           
-0000ed70: 2066 6965 6c64 2e6d 616b 655f 6d75 6c74   field.make_mult
-0000ed80: 6970 6172 7428 636f 6e74 656e 745f 7479  ipart(content_ty
-0000ed90: 7065 3d66 6965 6c64 2e68 6561 6465 7273  pe=field.headers
-0000eda0: 5b22 436f 6e74 656e 742d 5479 7065 225d  ["Content-Type"]
-0000edb0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0000edc0: 2064 6963 7428 6669 656c 6473 3d74 7570   dict(fields=tup
-0000edd0: 6c65 2866 6965 6c64 7329 290a 0a20 2020  le(fields))..   
-0000ede0: 2064 6566 205f 5f73 6572 6961 6c69 7a65   def __serialize
-0000edf0: 5f61 7070 6c69 6361 7469 6f6e 5f6f 6374  _application_oct
-0000ee00: 6574 5f73 7472 6561 6d28 7365 6c66 2c20  et_stream(self, 
-0000ee10: 696e 5f64 6174 613a 2042 696e 6172 7953  in_data: BinaryS
-0000ee20: 6368 656d 6129 202d 3e20 7479 7069 6e67  chema) -> typing
-0000ee30: 2e44 6963 745b 7374 722c 2062 7974 6573  .Dict[str, bytes
-0000ee40: 5d3a 0a20 2020 2020 2020 2069 6620 6973  ]:.        if is
-0000ee50: 696e 7374 616e 6365 2869 6e5f 6461 7461  instance(in_data
-0000ee60: 2c20 6279 7465 7329 3a0a 2020 2020 2020  , bytes):.      
-0000ee70: 2020 2020 2020 7265 7475 726e 2064 6963        return dic
-0000ee80: 7428 626f 6479 3d69 6e5f 6461 7461 290a  t(body=in_data).
-0000ee90: 2020 2020 2020 2020 2320 4669 6c65 494f          # FileIO
-0000eea0: 2074 7970 650a 2020 2020 2020 2020 7265   type.        re
-0000eeb0: 7375 6c74 203d 2064 6963 7428 626f 6479  sult = dict(body
-0000eec0: 3d69 6e5f 6461 7461 2e72 6561 6428 2929  =in_data.read())
-0000eed0: 0a20 2020 2020 2020 2069 6e5f 6461 7461  .        in_data
-0000eee0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-0000eef0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0000ef00: 2020 2020 6465 6620 5f5f 7365 7269 616c      def __serial
-0000ef10: 697a 655f 6170 706c 6963 6174 696f 6e5f  ize_application_
-0000ef20: 785f 7777 775f 666f 726d 5f64 6174 6128  x_www_form_data(
-0000ef30: 0a20 2020 2020 2020 2073 656c 662c 2069  .        self, i
-0000ef40: 6e5f 6461 7461 3a20 7479 7069 6e67 2e41  n_data: typing.A
-0000ef50: 6e79 0a20 2020 2029 202d 3e20 5365 7269  ny.    ) -> Seri
-0000ef60: 616c 697a 6564 5265 7175 6573 7442 6f64  alizedRequestBod
-0000ef70: 793a 0a20 2020 2020 2020 2022 2222 0a20  y:.        """. 
-0000ef80: 2020 2020 2020 2050 4f53 5420 7375 626d         POST subm
-0000ef90: 6973 7369 6f6e 206f 6620 666f 726d 2064  ission of form d
-0000efa0: 6174 6120 696e 2062 6f64 790a 2020 2020  ata in body.    
-0000efb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000efc0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-0000efd0: 6528 696e 5f64 6174 612c 2066 726f 7a65  e(in_data, froze
-0000efe0: 6e64 6963 742e 6672 6f7a 656e 6469 6374  ndict.frozendict
-0000eff0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000f000: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000f010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f020: 2066 2755 6e61 626c 6520 746f 2073 6572   f'Unable to ser
-0000f030: 6961 6c69 7a65 207b 696e 5f64 6174 617d  ialize {in_data}
-0000f040: 2074 6f20 6170 706c 6963 6174 696f 6e2f   to application/
-0000f050: 782d 7777 772d 666f 726d 2d75 726c 656e  x-www-form-urlen
-0000f060: 636f 6465 6420 6265 6361 7573 6520 6974  coded because it
-0000f070: 2069 7320 6e6f 7420 6120 6469 6374 206f   is not a dict o
-0000f080: 6620 6461 7461 2729 0a20 2020 2020 2020  f data').       
-0000f090: 2063 6173 745f 696e 5f64 6174 6120 3d20   cast_in_data = 
-0000f0a0: 7365 6c66 2e5f 5f6a 736f 6e5f 656e 636f  self.__json_enco
-0000f0b0: 6465 722e 6465 6661 756c 7428 696e 5f64  der.default(in_d
-0000f0c0: 6174 6129 0a20 2020 2020 2020 2076 616c  ata).        val
-0000f0d0: 7565 203d 2073 656c 662e 5f73 6572 6961  ue = self._seria
-0000f0e0: 6c69 7a65 5f66 6f72 6d28 6361 7374 5f69  lize_form(cast_i
-0000f0f0: 6e5f 6461 7461 2c20 6e61 6d65 3d27 272c  n_data, name='',
-0000f100: 2065 7870 6c6f 6465 3d54 7275 652c 2070   explode=True, p
-0000f110: 6572 6365 6e74 5f65 6e63 6f64 653d 5472  ercent_encode=Tr
-0000f120: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
-0000f130: 726e 2064 6963 7428 626f 6479 3d76 616c  rn dict(body=val
-0000f140: 7565 290a 0a20 2020 2064 6566 2073 6572  ue)..    def ser
-0000f150: 6961 6c69 7a65 280a 2020 2020 2020 2020  ialize(.        
-0000f160: 7365 6c66 2c20 696e 5f64 6174 613a 2074  self, in_data: t
-0000f170: 7970 696e 672e 416e 792c 2063 6f6e 7465  yping.Any, conte
-0000f180: 6e74 5f74 7970 653a 2073 7472 0a20 2020  nt_type: str.   
-0000f190: 2029 202d 3e20 5365 7269 616c 697a 6564   ) -> Serialized
-0000f1a0: 5265 7175 6573 7442 6f64 793a 0a20 2020  RequestBody:.   
-0000f1b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f1c0: 2049 6620 6120 7374 7220 6973 2072 6574   If a str is ret
-0000f1d0: 7572 6e65 6420 7468 656e 2074 6865 2072  urned then the r
-0000f1e0: 6573 756c 7420 7769 6c6c 2062 6520 6173  esult will be as
-0000f1f0: 7369 676e 6564 2074 6f20 6461 7461 2077  signed to data w
-0000f200: 6865 6e20 6d61 6b69 6e67 2074 6865 2072  hen making the r
-0000f210: 6571 7565 7374 0a20 2020 2020 2020 2049  equest.        I
-0000f220: 6620 6120 7475 706c 6520 6973 2072 6574  f a tuple is ret
-0000f230: 7572 6e65 6420 7468 656e 2074 6865 2072  urned then the r
-0000f240: 6573 756c 7420 7769 6c6c 2062 6520 7573  esult will be us
-0000f250: 6564 2061 7320 6669 656c 6473 2069 6e70  ed as fields inp
-0000f260: 7574 2069 6e20 656e 636f 6465 5f6d 756c  ut in encode_mul
-0000f270: 7469 7061 7274 5f66 6f72 6d64 6174 610a  tipart_formdata.
-0000f280: 2020 2020 2020 2020 5265 7475 726e 2061          Return a
-0000f290: 2074 7570 6c65 206f 660a 0a20 2020 2020   tuple of..     
-0000f2a0: 2020 2054 6865 206b 6579 206f 6620 7468     The key of th
-0000f2b0: 6520 7265 7475 726e 2064 6963 7420 6973  e return dict is
-0000f2c0: 0a20 2020 2020 2020 202d 2062 6f64 7920  .        - body 
-0000f2d0: 666f 7220 6170 706c 6963 6174 696f 6e2f  for application/
-0000f2e0: 6a73 6f6e 0a20 2020 2020 2020 202d 2065  json.        - e
-0000f2f0: 6e63 6f64 655f 6d75 6c74 6970 6172 7420  ncode_multipart 
-0000f300: 616e 6420 6669 656c 6473 2066 6f72 206d  and fields for m
-0000f310: 756c 7469 7061 7274 2f66 6f72 6d2d 6461  ultipart/form-da
-0000f320: 7461 0a20 2020 2020 2020 2022 2222 0a20  ta.        """. 
-0000f330: 2020 2020 2020 206d 6564 6961 5f74 7970         media_typ
-0000f340: 6520 3d20 7365 6c66 2e63 6f6e 7465 6e74  e = self.content
-0000f350: 5b63 6f6e 7465 6e74 5f74 7970 655d 0a20  [content_type]. 
-0000f360: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0000f370: 616e 6365 2869 6e5f 6461 7461 2c20 6d65  ance(in_data, me
-0000f380: 6469 615f 7479 7065 2e73 6368 656d 6129  dia_type.schema)
-0000f390: 3a0a 2020 2020 2020 2020 2020 2020 6361  :.            ca
-0000f3a0: 7374 5f69 6e5f 6461 7461 203d 2069 6e5f  st_in_data = in_
-0000f3b0: 6461 7461 0a20 2020 2020 2020 2065 6c69  data.        eli
-0000f3c0: 6620 6973 696e 7374 616e 6365 2869 6e5f  f isinstance(in_
-0000f3d0: 6461 7461 2c20 2864 6963 742c 2066 726f  data, (dict, fro
-0000f3e0: 7a65 6e64 6963 742e 6672 6f7a 656e 6469  zendict.frozendi
-0000f3f0: 6374 2929 2061 6e64 2069 6e5f 6461 7461  ct)) and in_data
-0000f400: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0000f410: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000f420: 2020 2063 6173 745f 696e 5f64 6174 6120     cast_in_data 
-0000f430: 3d20 6d65 6469 615f 7479 7065 2e73 6368  = media_type.sch
-0000f440: 656d 6128 2a2a 696e 5f64 6174 6129 0a20  ema(**in_data). 
-0000f450: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0000f460: 7420 5479 7065 4572 726f 7220 6173 2065  t TypeError as e
-0000f470: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f480: 2020 7261 6973 6520 4d69 7373 696e 6752    raise MissingR
-0000f490: 6571 7569 7265 6450 6172 616d 6574 6572  equiredParameter
-0000f4a0: 7345 7272 6f72 2865 290a 2020 2020 2020  sError(e).      
-0000f4b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f4c0: 2020 2020 6361 7374 5f69 6e5f 6461 7461      cast_in_data
-0000f4d0: 203d 206d 6564 6961 5f74 7970 652e 7363   = media_type.sc
-0000f4e0: 6865 6d61 2869 6e5f 6461 7461 290a 2020  hema(in_data).  
-0000f4f0: 2020 2020 2020 2320 544f 444f 2063 6865        # TODO che
-0000f500: 636b 2066 6f72 2061 6e64 2075 7365 2065  ck for and use e
-0000f510: 6e63 6f64 696e 6720 6966 2069 7420 6578  ncoding if it ex
-0000f520: 6973 7473 0a20 2020 2020 2020 2023 2061  ists.        # a
-0000f530: 6e64 2063 6f6e 7465 6e74 5f74 7970 6520  nd content_type 
-0000f540: 6973 206d 756c 7469 7061 7274 206f 7220  is multipart or 
-0000f550: 6170 706c 6963 6174 696f 6e2f 782d 7777  application/x-ww
-0000f560: 772d 666f 726d 2d75 726c 656e 636f 6465  w-form-urlencode
-0000f570: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0000f580: 662e 5f63 6f6e 7465 6e74 5f74 7970 655f  f._content_type_
-0000f590: 6973 5f6a 736f 6e28 636f 6e74 656e 745f  is_json(content_
-0000f5a0: 7479 7065 293a 0a20 2020 2020 2020 2020  type):.         
-0000f5b0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0000f5c0: 5f73 6572 6961 6c69 7a65 5f6a 736f 6e28  _serialize_json(
-0000f5d0: 6361 7374 5f69 6e5f 6461 7461 290a 2020  cast_in_data).  
-0000f5e0: 2020 2020 2020 656c 6966 2063 6f6e 7465        elif conte
-0000f5f0: 6e74 5f74 7970 6520 3d3d 2027 7465 7874  nt_type == 'text
-0000f600: 2f70 6c61 696e 273a 0a20 2020 2020 2020  /plain':.       
-0000f610: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000f620: 2e5f 5f73 6572 6961 6c69 7a65 5f74 6578  .__serialize_tex
-0000f630: 745f 706c 6169 6e28 6361 7374 5f69 6e5f  t_plain(cast_in_
-0000f640: 6461 7461 290a 2020 2020 2020 2020 656c  data).        el
-0000f650: 6966 2063 6f6e 7465 6e74 5f74 7970 6520  if content_type 
-0000f660: 3d3d 2027 6d75 6c74 6970 6172 742f 666f  == 'multipart/fo
-0000f670: 726d 2d64 6174 6127 3a0a 2020 2020 2020  rm-data':.      
-0000f680: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000f690: 662e 5f5f 7365 7269 616c 697a 655f 6d75  f.__serialize_mu
-0000f6a0: 6c74 6970 6172 745f 666f 726d 5f64 6174  ltipart_form_dat
-0000f6b0: 6128 6361 7374 5f69 6e5f 6461 7461 290a  a(cast_in_data).
-0000f6c0: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
-0000f6d0: 7465 6e74 5f74 7970 6520 3d3d 2027 6170  tent_type == 'ap
-0000f6e0: 706c 6963 6174 696f 6e2f 782d 7777 772d  plication/x-www-
-0000f6f0: 666f 726d 2d75 726c 656e 636f 6465 6427  form-urlencoded'
-0000f700: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000f710: 7475 726e 2073 656c 662e 5f5f 7365 7269  turn self.__seri
-0000f720: 616c 697a 655f 6170 706c 6963 6174 696f  alize_applicatio
-0000f730: 6e5f 785f 7777 775f 666f 726d 5f64 6174  n_x_www_form_dat
-0000f740: 6128 6361 7374 5f69 6e5f 6461 7461 290a  a(cast_in_data).
-0000f750: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
-0000f760: 7465 6e74 5f74 7970 6520 3d3d 2027 6170  tent_type == 'ap
-0000f770: 706c 6963 6174 696f 6e2f 6f63 7465 742d  plication/octet-
-0000f780: 7374 7265 616d 273a 0a20 2020 2020 2020  stream':.       
-0000f790: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0000f7a0: 2e5f 5f73 6572 6961 6c69 7a65 5f61 7070  .__serialize_app
-0000f7b0: 6c69 6361 7469 6f6e 5f6f 6374 6574 5f73  lication_octet_s
-0000f7c0: 7472 6561 6d28 6361 7374 5f69 6e5f 6461  tream(cast_in_da
-0000f7d0: 7461 290a 2020 2020 2020 2020 7261 6973  ta).        rais
-0000f7e0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-0000f7f0: 4572 726f 7228 2753 6572 6961 6c69 7a61  Error('Serializa
-0000f800: 7469 6f6e 2068 6173 206e 6f74 2079 6574  tion has not yet
-0000f810: 2062 6565 6e20 696d 706c 656d 656e 7465   been implemente
-0000f820: 6420 666f 7220 7b7d 272e 666f 726d 6174  d for {}'.format
-0000f830: 2863 6f6e 7465 6e74 5f74 7970 6529 290a  (content_type)).
+0000e360: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000e370: 656c 6473 3d66 6965 6c64 732c 0a20 2020  elds=fields,.   
+0000e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3a0: 2020 2020 2020 7374 7265 616d 3d73 7472        stream=str
+0000e3b0: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
+0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+0000e3e0: 6d65 6f75 743d 7469 6d65 6f75 742c 0a20  meout=timeout,. 
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e410: 2020 2020 2020 2020 626f 6479 3d62 6f64          body=bod
+0000e420: 7929 0a20 2020 2020 2020 2065 6c69 6620  y).        elif 
+0000e430: 6d65 7468 6f64 203d 3d20 2250 5554 223a  method == "PUT":
+0000e440: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e450: 7572 6e20 7365 6c66 2e72 6573 745f 636c  urn self.rest_cl
+0000e460: 6965 6e74 2e50 5554 2875 726c 2c0a 2020  ient.PUT(url,.  
+0000e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e490: 2020 2020 2020 6865 6164 6572 733d 6865        headers=he
+0000e4a0: 6164 6572 732c 0a20 2020 2020 2020 2020  aders,.         
+0000e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e4d0: 6965 6c64 733d 6669 656c 6473 2c0a 2020  ields=fields,.  
+0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 2020 2020 7374 7265 616d 3d73 7472        stream=str
+0000e510: 6561 6d2c 0a20 2020 2020 2020 2020 2020  eam,.           
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+0000e540: 656f 7574 3d74 696d 656f 7574 2c0a 2020  eout=timeout,.  
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e570: 2020 2020 2020 626f 6479 3d62 6f64 7929        body=body)
+0000e580: 0a20 2020 2020 2020 2065 6c69 6620 6d65  .        elif me
+0000e590: 7468 6f64 203d 3d20 2250 4154 4348 223a  thod == "PATCH":
+0000e5a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000e5b0: 7572 6e20 7365 6c66 2e72 6573 745f 636c  urn self.rest_cl
+0000e5c0: 6965 6e74 2e50 4154 4348 2875 726c 2c0a  ient.PATCH(url,.
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5f0: 2020 2020 2020 2020 2020 6865 6164 6572            header
+0000e600: 733d 6865 6164 6572 732c 0a20 2020 2020  s=headers,.     
+0000e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e630: 2020 2020 2066 6965 6c64 733d 6669 656c       fields=fiel
+0000e640: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000e670: 7265 616d 3d73 7472 6561 6d2c 0a20 2020  ream=stream,.   
+0000e680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6a0: 2020 2020 2020 2074 696d 656f 7574 3d74         timeout=t
+0000e6b0: 696d 656f 7574 2c0a 2020 2020 2020 2020  imeout,.        
+0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 2020 626f 6479 3d62 6f64 7929 0a20 2020    body=body).   
+0000e6f0: 2020 2020 2065 6c69 6620 6d65 7468 6f64       elif method
+0000e700: 203d 3d20 2244 454c 4554 4522 3a0a 2020   == "DELETE":.  
+0000e710: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e720: 2073 656c 662e 7265 7374 5f63 6c69 656e   self.rest_clien
+0000e730: 742e 4445 4c45 5445 2875 726c 2c0a 2020  t.DELETE(url,.  
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e760: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0000e770: 3d68 6561 6465 7273 2c0a 2020 2020 2020  =headers,.      
+0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7a0: 2020 2020 2073 7472 6561 6d3d 7374 7265       stream=stre
+0000e7b0: 616d 2c0a 2020 2020 2020 2020 2020 2020  am,.            
+0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000e7e0: 696d 656f 7574 3d74 696d 656f 7574 2c0a  imeout=timeout,.
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 2020 2020 2020 2062 6f64 793d             body=
+0000e820: 626f 6479 290a 2020 2020 2020 2020 656c  body).        el
+0000e830: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000e840: 7261 6973 6520 4170 6956 616c 7565 4572  raise ApiValueEr
+0000e850: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+0000e860: 2020 2020 2022 6874 7470 206d 6574 686f       "http metho
+0000e870: 6420 6d75 7374 2062 6520 6047 4554 602c  d must be `GET`,
+0000e880: 2060 4845 4144 602c 2060 4f50 5449 4f4e   `HEAD`, `OPTION
+0000e890: 5360 2c22 0a20 2020 2020 2020 2020 2020  S`,".           
+0000e8a0: 2020 2020 2022 2060 504f 5354 602c 2060       " `POST`, `
+0000e8b0: 5041 5443 4860 2c20 6050 5554 6020 6f72  PATCH`, `PUT` or
+0000e8c0: 2060 4445 4c45 5445 602e 220a 2020 2020   `DELETE`.".    
+0000e8d0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000e8e0: 6566 2075 7064 6174 655f 7061 7261 6d73  ef update_params
+0000e8f0: 5f66 6f72 5f61 7574 6828 0a20 2020 2020  _for_auth(.     
+0000e900: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0000e910: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+0000e920: 2c0a 2020 2020 2020 2020 2020 2020 6175  ,.            au
+0000e930: 7468 5f73 6574 7469 6e67 732c 0a20 2020  th_settings,.   
+0000e940: 2020 2020 2020 2020 2072 6573 6f75 7263           resourc
+0000e950: 655f 7061 7468 2c0a 2020 2020 2020 2020  e_path,.        
+0000e960: 2020 2020 6d65 7468 6f64 2c0a 2020 2020      method,.    
+0000e970: 2020 2020 2020 2020 626f 6479 2c0a 2020          body,.  
+0000e980: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
+0000e990: 5f73 6570 6172 6174 6f72 5f69 7465 7261  _separator_itera
+0000e9a0: 746f 723a 2050 7265 6669 7853 6570 6172  tor: PrefixSepar
+0000e9b0: 6174 6f72 4974 6572 6174 6f72 203d 204e  atorIterator = N
+0000e9c0: 6f6e 650a 2020 2020 2020 2020 2920 2d3e  one.        ) ->
+0000e9d0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
+0000e9e0: 2255 7064 6174 6573 2068 6561 6465 7220  "Updates header 
+0000e9f0: 616e 6420 7175 6572 7920 7061 7261 6d73  and query params
+0000ea00: 2062 6173 6564 206f 6e20 6175 7468 656e   based on authen
+0000ea10: 7469 6361 7469 6f6e 2073 6574 7469 6e67  tication setting
+0000ea20: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+0000ea30: 6d20 6865 6164 6572 733a 2048 6561 6465  m headers: Heade
+0000ea40: 7220 7061 7261 6d65 7465 7273 2064 6963  r parameters dic
+0000ea50: 7420 746f 2062 6520 7570 6461 7465 642e  t to be updated.
+0000ea60: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000ea70: 6175 7468 5f73 6574 7469 6e67 733a 2041  auth_settings: A
+0000ea80: 7574 6865 6e74 6963 6174 696f 6e20 7365  uthentication se
+0000ea90: 7474 696e 6720 6964 656e 7469 6669 6572  tting identifier
+0000eaa0: 7320 6c69 7374 2e0a 2020 2020 2020 2020  s list..        
+0000eab0: 3a70 6172 616d 2072 6573 6f75 7263 655f  :param resource_
+0000eac0: 7061 7468 3a20 4120 7374 7269 6e67 2072  path: A string r
+0000ead0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
+0000eae0: 2074 6865 2048 5454 5020 7265 7175 6573   the HTTP reques
+0000eaf0: 7420 7265 736f 7572 6365 2070 6174 682e  t resource path.
+0000eb00: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000eb10: 6d65 7468 6f64 3a20 4120 7374 7269 6e67  method: A string
+0000eb20: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+0000eb30: 6f66 2074 6865 2048 5454 5020 7265 7175  of the HTTP requ
+0000eb40: 6573 7420 6d65 7468 6f64 2e0a 2020 2020  est method..    
+0000eb50: 2020 2020 3a70 6172 616d 2062 6f64 793a      :param body:
+0000eb60: 2041 206f 626a 6563 7420 7265 7072 6573   A object repres
+0000eb70: 656e 7469 6e67 2074 6865 2062 6f64 7920  enting the body 
+0000eb80: 6f66 2074 6865 2048 5454 5020 7265 7175  of the HTTP requ
+0000eb90: 6573 742e 0a20 2020 2020 2020 2020 2020  est..           
+0000eba0: 2054 6865 206f 626a 6563 7420 7479 7065   The object type
+0000ebb0: 2069 7320 7468 6520 7265 7475 726e 2076   is the return v
+0000ebc0: 616c 7565 206f 6620 5f65 6e63 6f64 6572  alue of _encoder
+0000ebd0: 2e64 6566 6175 6c74 2829 2e0a 2020 2020  .default()..    
+0000ebe0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000ebf0: 6966 206e 6f74 2061 7574 685f 7365 7474  if not auth_sett
+0000ec00: 696e 6773 3a0a 2020 2020 2020 2020 2020  ings:.          
+0000ec10: 2020 7265 7475 726e 2072 6573 6f75 7263    return resourc
+0000ec20: 655f 7061 7468 0a20 2020 2020 2020 2069  e_path.        i
+0000ec30: 6620 7072 6566 6978 5f73 6570 6172 6174  f prefix_separat
+0000ec40: 6f72 5f69 7465 7261 746f 7220 6973 204e  or_iterator is N
+0000ec50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000ec60: 2070 7265 6669 785f 7365 7061 7261 746f   prefix_separato
+0000ec70: 725f 6974 6572 6174 6f72 203d 2050 7265  r_iterator = Pre
+0000ec80: 6669 7853 6570 6172 6174 6f72 4974 6572  fixSeparatorIter
+0000ec90: 6174 6f72 2822 3f22 2c20 2226 2229 0a0a  ator("?", "&")..
+0000eca0: 2020 2020 2020 2020 666f 7220 6175 7468          for auth
+0000ecb0: 2069 6e20 6175 7468 5f73 6574 7469 6e67   in auth_setting
+0000ecc0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
+0000ecd0: 7574 685f 7365 7474 696e 6720 3d20 7365  uth_setting = se
+0000ece0: 6c66 2e63 6f6e 6669 6775 7261 7469 6f6e  lf.configuration
+0000ecf0: 2e61 7574 685f 7365 7474 696e 6773 2829  .auth_settings()
+0000ed00: 2e67 6574 2861 7574 6829 0a20 2020 2020  .get(auth).     
+0000ed10: 2020 2020 2020 2069 6620 6e6f 7420 6175         if not au
+0000ed20: 7468 5f73 6574 7469 6e67 3a0a 2020 2020  th_setting:.    
+0000ed30: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000ed40: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000ed50: 2069 6620 6175 7468 5f73 6574 7469 6e67   if auth_setting
+0000ed60: 5b27 696e 275d 203d 3d20 2763 6f6f 6b69  ['in'] == 'cooki
+0000ed70: 6527 3a0a 2020 2020 2020 2020 2020 2020  e':.            
+0000ed80: 2020 2020 6865 6164 6572 732e 6164 6428      headers.add(
+0000ed90: 2743 6f6f 6b69 6527 2c20 6175 7468 5f73  'Cookie', auth_s
+0000eda0: 6574 7469 6e67 5b27 7661 6c75 6527 5d29  etting['value'])
+0000edb0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000edc0: 6620 6175 7468 5f73 6574 7469 6e67 5b27  f auth_setting['
+0000edd0: 696e 275d 203d 3d20 2768 6561 6465 7227  in'] == 'header'
+0000ede0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000edf0: 2020 6966 2061 7574 685f 7365 7474 696e    if auth_settin
+0000ee00: 675b 2774 7970 6527 5d20 213d 2027 6874  g['type'] != 'ht
+0000ee10: 7470 2d73 6967 6e61 7475 7265 273a 0a20  tp-signature':. 
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee30: 2020 2068 6561 6465 7273 2e61 6464 2861     headers.add(a
+0000ee40: 7574 685f 7365 7474 696e 675b 276b 6579  uth_setting['key
+0000ee50: 275d 2c20 6175 7468 5f73 6574 7469 6e67  '], auth_setting
+0000ee60: 5b27 7661 6c75 6527 5d29 0a20 2020 2020  ['value']).     
+0000ee70: 2020 2020 2020 2065 6c69 6620 6175 7468         elif auth
+0000ee80: 5f73 6574 7469 6e67 5b27 696e 275d 203d  _setting['in'] =
+0000ee90: 3d20 2771 7565 7279 273a 0a20 2020 2020  = 'query':.     
+0000eea0: 2020 2020 2020 2020 2020 2022 2222 2054             """ T
+0000eeb0: 4f44 4f20 696d 706c 656d 656e 7420 6175  ODO implement au
+0000eec0: 7468 2069 6e20 7175 6572 790a 2020 2020  th in query.    
+0000eed0: 2020 2020 2020 2020 2020 2020 6e65 6564              need
+0000eee0: 2074 6f20 7061 7373 2069 6e20 7072 6566   to pass in pref
+0000eef0: 6978 5f73 6570 6172 6174 6f72 5f69 7465  ix_separator_ite
+0000ef00: 7261 746f 720a 2020 2020 2020 2020 2020  rator.          
+0000ef10: 2020 2020 2020 616e 6420 6e65 6564 2074        and need t
+0000ef20: 6f20 6f75 7470 7574 2072 6573 6f75 7263  o output resourc
+0000ef30: 655f 7061 7468 2077 6974 6820 7175 6572  e_path with quer
+0000ef40: 7920 7061 7261 6d73 2061 6464 6564 0a20  y params added. 
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ef60: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+0000ef70: 2020 2072 6573 6f75 7263 655f 7061 7468     resource_path
+0000ef80: 202b 3d20 5061 7261 6d65 7465 7253 6572   += ParameterSer
+0000ef90: 6961 6c69 7a65 7242 6173 652e 5f72 6566  ializerBase._ref
+0000efa0: 3635 3730 5f65 7870 616e 7369 6f6e 280a  6570_expansion(.
+0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efc0: 2020 2020 7661 7269 6162 6c65 5f6e 616d      variable_nam
+0000efd0: 653d 6175 7468 5f73 6574 7469 6e67 5b27  e=auth_setting['
+0000efe0: 6b65 7927 5d2c 0a20 2020 2020 2020 2020  key'],.         
+0000eff0: 2020 2020 2020 2020 2020 2069 6e5f 6461             in_da
+0000f000: 7461 3d61 7574 685f 7365 7474 696e 675b  ta=auth_setting[
+0000f010: 2776 616c 7565 275d 2c0a 2020 2020 2020  'value'],.      
+0000f020: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0000f030: 706c 6f64 653d 4661 6c73 652c 0a20 2020  plode=False,.   
+0000f040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f050: 2070 6572 6365 6e74 5f65 6e63 6f64 653d   percent_encode=
+0000f060: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+0000f070: 2020 2020 2020 2020 2020 2070 7265 6669             prefi
+0000f080: 785f 7365 7061 7261 746f 725f 6974 6572  x_separator_iter
+0000f090: 6174 6f72 3d70 7265 6669 785f 7365 7061  ator=prefix_sepa
+0000f0a0: 7261 746f 725f 6974 6572 6174 6f72 0a20  rator_iterator. 
+0000f0b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000f0c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000f0d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000f0e0: 2020 2072 6169 7365 2041 7069 5661 6c75     raise ApiValu
+0000f0f0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0000f100: 2020 2020 2020 2020 2020 2020 2741 7574              'Aut
+0000f110: 6865 6e74 6963 6174 696f 6e20 746f 6b65  hentication toke
+0000f120: 6e20 6d75 7374 2062 6520 696e 2060 7175  n must be in `qu
+0000f130: 6572 7960 206f 7220 6068 6561 6465 7260  ery` or `header`
+0000f140: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000f150: 2020 290a 2020 2020 2020 2020 7265 7475    ).        retu
+0000f160: 726e 2072 6573 6f75 7263 655f 7061 7468  rn resource_path
+0000f170: 0a0a 0a63 6c61 7373 2041 7069 3a0a 2020  ...class Api:.  
+0000f180: 2020 2222 224e 4f54 453a 0a20 2020 2054    """NOTE:.    T
+0000f190: 6869 7320 636c 6173 7320 6973 2061 7574  his class is aut
+0000f1a0: 6f20 6765 6e65 7261 7465 640a 2020 2020  o generated.    
+0000f1b0: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+0000f1c0: 6e69 745f 5f28 7365 6c66 2c20 6170 695f  nit__(self, api_
+0000f1d0: 636c 6965 6e74 3a20 7479 7069 6e67 2e4f  client: typing.O
+0000f1e0: 7074 696f 6e61 6c5b 4170 6943 6c69 656e  ptional[ApiClien
+0000f1f0: 745d 203d 204e 6f6e 6529 3a0a 2020 2020  t] = None):.    
+0000f200: 2020 2020 6966 2061 7069 5f63 6c69 656e      if api_clien
+0000f210: 7420 6973 204e 6f6e 653a 0a20 2020 2020  t is None:.     
+0000f220: 2020 2020 2020 2061 7069 5f63 6c69 656e         api_clien
+0000f230: 7420 3d20 4170 6943 6c69 656e 7428 290a  t = ApiClient().
+0000f240: 2020 2020 2020 2020 7365 6c66 2e61 7069          self.api
+0000f250: 5f63 6c69 656e 7420 3d20 6170 695f 636c  _client = api_cl
+0000f260: 6965 6e74 0a0a 2020 2020 4073 7461 7469  ient..    @stati
+0000f270: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+0000f280: 5f76 6572 6966 795f 7479 7065 645f 6469  _verify_typed_di
+0000f290: 6374 5f69 6e70 7574 735f 6f61 7067 2863  ct_inputs_oapg(c
+0000f2a0: 6c73 3a20 7479 7069 6e67 2e54 7970 655b  ls: typing.Type[
+0000f2b0: 7479 7069 6e67 5f65 7874 656e 7369 6f6e  typing_extension
+0000f2c0: 732e 5479 7065 6444 6963 745d 2c20 6461  s.TypedDict], da
+0000f2d0: 7461 3a20 7479 7069 6e67 2e44 6963 745b  ta: typing.Dict[
+0000f2e0: 7374 722c 2074 7970 696e 672e 416e 795d  str, typing.Any]
+0000f2f0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000f300: 2020 2020 2020 2045 6e73 7572 6573 2074         Ensures t
+0000f310: 6861 743a 0a20 2020 2020 2020 202d 2072  hat:.        - r
+0000f320: 6571 7569 7265 6420 6b65 7973 2061 7265  equired keys are
+0000f330: 2070 7265 7365 6e74 0a20 2020 2020 2020   present.       
+0000f340: 202d 2061 6464 6974 696f 6e61 6c20 7072   - additional pr
+0000f350: 6f70 6572 7469 6573 2061 7265 206e 6f74  operties are not
+0000f360: 2069 6e70 7574 0a20 2020 2020 2020 202d   input.        -
+0000f370: 2076 616c 7565 2073 746f 7265 6420 756e   value stored un
+0000f380: 6465 7220 7265 7175 6972 6564 206b 6579  der required key
+0000f390: 7320 646f 206e 6f74 2068 6176 6520 7468  s do not have th
+0000f3a0: 6520 7661 6c75 6520 756e 7365 740a 2020  e value unset.  
+0000f3b0: 2020 2020 2020 4e6f 7465 3a20 6465 7461        Note: deta
+0000f3c0: 696c 6564 2076 616c 7565 2063 6865 636b  iled value check
+0000f3d0: 696e 6720 6973 2064 6f6e 6520 696e 2073  ing is done in s
+0000f3e0: 6368 656d 6120 636c 6173 7365 730a 2020  chema classes.  
+0000f3f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f400: 2020 6d69 7373 696e 675f 7265 7175 6972    missing_requir
+0000f410: 6564 5f6b 6579 7320 3d20 5b5d 0a20 2020  ed_keys = [].   
+0000f420: 2020 2020 2072 6571 7569 7265 645f 6b65       required_ke
+0000f430: 7973 5f77 6974 685f 756e 7365 745f 7661  ys_with_unset_va
+0000f440: 6c75 6573 203d 205b 5d0a 2020 2020 2020  lues = [].      
+0000f450: 2020 666f 7220 7265 7175 6972 6564 5f6b    for required_k
+0000f460: 6579 2069 6e20 636c 732e 5f5f 7265 7175  ey in cls.__requ
+0000f470: 6972 6564 5f6b 6579 735f 5f3a 0a20 2020  ired_keys__:.   
+0000f480: 2020 2020 2020 2020 2069 6620 7265 7175           if requ
+0000f490: 6972 6564 5f6b 6579 206e 6f74 2069 6e20  ired_key not in 
+0000f4a0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+0000f4b0: 2020 2020 2020 6d69 7373 696e 675f 7265        missing_re
+0000f4c0: 7175 6972 6564 5f6b 6579 732e 6170 7065  quired_keys.appe
+0000f4d0: 6e64 2872 6571 7569 7265 645f 6b65 7929  nd(required_key)
+0000f4e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f4f0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+0000f500: 2020 2020 2020 7661 6c75 6520 3d20 6461        value = da
+0000f510: 7461 5b72 6571 7569 7265 645f 6b65 795d  ta[required_key]
+0000f520: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000f530: 7661 6c75 6520 6973 2075 6e73 6574 3a0a  value is unset:.
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f550: 7265 7175 6972 6564 5f6b 6579 735f 7769  required_keys_wi
+0000f560: 7468 5f75 6e73 6574 5f76 616c 7565 732e  th_unset_values.
+0000f570: 6170 7065 6e64 2872 6571 7569 7265 645f  append(required_
+0000f580: 6b65 7929 0a20 2020 2020 2020 2069 6620  key).        if 
+0000f590: 6d69 7373 696e 675f 7265 7175 6972 6564  missing_required
+0000f5a0: 5f6b 6579 733a 0a20 2020 2020 2020 2020  _keys:.         
+0000f5b0: 2020 2072 6169 7365 2041 7069 5479 7065     raise ApiType
+0000f5c0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000f5d0: 2020 2020 2020 2027 7b7d 206d 6973 7369         '{} missi
+0000f5e0: 6e67 207b 7d20 7265 7175 6972 6564 2061  ng {} required a
+0000f5f0: 7267 756d 656e 7473 3a20 7b7d 272e 666f  rguments: {}'.fo
+0000f600: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+0000f610: 2020 2020 2020 2020 2020 636c 732e 5f5f            cls.__
+0000f620: 6e61 6d65 5f5f 2c20 6c65 6e28 6d69 7373  name__, len(miss
+0000f630: 696e 675f 7265 7175 6972 6564 5f6b 6579  ing_required_key
+0000f640: 7329 2c20 6d69 7373 696e 675f 7265 7175  s), missing_requ
+0000f650: 6972 6564 5f6b 6579 730a 2020 2020 2020  ired_keys.      
+0000f660: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000f670: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f680: 2020 2020 6966 2072 6571 7569 7265 645f      if required_
+0000f690: 6b65 7973 5f77 6974 685f 756e 7365 745f  keys_with_unset_
+0000f6a0: 7661 6c75 6573 3a0a 2020 2020 2020 2020  values:.        
+0000f6b0: 2020 2020 7261 6973 6520 4170 6956 616c      raise ApiVal
+0000f6c0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+0000f6d0: 2020 2020 2020 2020 2027 7b7d 2063 6f6e           '{} con
+0000f6e0: 7461 696e 7320 696e 7661 6c69 6420 756e  tains invalid un
+0000f6f0: 7365 7420 7661 6c75 6573 2066 6f72 207b  set values for {
+0000f700: 7d20 7265 7175 6972 6564 206b 6579 733a  } required keys:
+0000f710: 207b 7d27 2e66 6f72 6d61 7428 0a20 2020   {}'.format(.   
+0000f720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f730: 2063 6c73 2e5f 5f6e 616d 655f 5f2c 206c   cls.__name__, l
+0000f740: 656e 2872 6571 7569 7265 645f 6b65 7973  en(required_keys
+0000f750: 5f77 6974 685f 756e 7365 745f 7661 6c75  _with_unset_valu
+0000f760: 6573 292c 2072 6571 7569 7265 645f 6b65  es), required_ke
+0000f770: 7973 5f77 6974 685f 756e 7365 745f 7661  ys_with_unset_va
+0000f780: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
+0000f790: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000f7a0: 2020 2029 0a0a 2020 2020 2020 2020 6469     )..        di
+0000f7b0: 7361 6c6c 6f77 6564 5f61 6464 6974 696f  sallowed_additio
+0000f7c0: 6e61 6c5f 6b65 7973 203d 205b 5d0a 2020  nal_keys = [].  
+0000f7d0: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+0000f7e0: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+0000f7f0: 2020 2069 6620 6b65 7920 696e 2063 6c73     if key in cls
+0000f800: 2e5f 5f72 6571 7569 7265 645f 6b65 7973  .__required_keys
+0000f810: 5f5f 206f 7220 6b65 7920 696e 2063 6c73  __ or key in cls
+0000f820: 2e5f 5f6f 7074 696f 6e61 6c5f 6b65 7973  .__optional_keys
+0000f830: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
+0000f840: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+0000f850: 2020 2020 2020 2020 2064 6973 616c 6c6f           disallo
+0000f860: 7765 645f 6164 6469 7469 6f6e 616c 5f6b  wed_additional_k
+0000f870: 6579 732e 6170 7065 6e64 286b 6579 290a  eys.append(key).
+0000f880: 2020 2020 2020 2020 6966 2064 6973 616c          if disal
+0000f890: 6c6f 7765 645f 6164 6469 7469 6f6e 616c  lowed_additional
+0000f8a0: 5f6b 6579 733a 0a20 2020 2020 2020 2020  _keys:.         
+0000f8b0: 2020 2072 6169 7365 2041 7069 5479 7065     raise ApiType
+0000f8c0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+0000f8d0: 2020 2020 2020 2027 7b7d 2067 6f74 207b         '{} got {
+0000f8e0: 7d20 756e 6578 7065 6374 6564 206b 6579  } unexpected key
+0000f8f0: 776f 7264 2061 7267 756d 656e 7473 3a20  word arguments: 
+0000f900: 7b7d 272e 666f 726d 6174 280a 2020 2020  {}'.format(.    
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f920: 636c 732e 5f5f 6e61 6d65 5f5f 2c20 6c65  cls.__name__, le
+0000f930: 6e28 6469 7361 6c6c 6f77 6564 5f61 6464  n(disallowed_add
+0000f940: 6974 696f 6e61 6c5f 6b65 7973 292c 2064  itional_keys), d
+0000f950: 6973 616c 6c6f 7765 645f 6164 6469 7469  isallowed_additi
+0000f960: 6f6e 616c 5f6b 6579 730a 2020 2020 2020  onal_keys.      
+0000f970: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f980: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+0000f990: 6566 205f 6765 745f 686f 7374 5f6f 6170  ef _get_host_oap
+0000f9a0: 6728 0a20 2020 2020 2020 2073 656c 662c  g(.        self,
+0000f9b0: 0a20 2020 2020 2020 206f 7065 7261 7469  .        operati
+0000f9c0: 6f6e 5f69 643a 2073 7472 2c0a 2020 2020  on_id: str,.    
+0000f9d0: 2020 2020 7365 7276 6572 733a 2074 7970      servers: typ
+0000f9e0: 696e 672e 5475 706c 655b 7479 7069 6e67  ing.Tuple[typing
+0000f9f0: 2e44 6963 745b 7374 722c 2073 7472 5d2c  .Dict[str, str],
+0000fa00: 202e 2e2e 5d20 3d20 7475 706c 6528 292c   ...] = tuple(),
+0000fa10: 0a20 2020 2020 2020 2068 6f73 745f 696e  .        host_in
+0000fa20: 6465 783a 2074 7970 696e 672e 4f70 7469  dex: typing.Opti
+0000fa30: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
+0000fa40: 0a20 2020 2029 202d 3e20 7479 7069 6e67  .    ) -> typing
+0000fa50: 2e4f 7074 696f 6e61 6c5b 7374 725d 3a0a  .Optional[str]:.
+0000fa60: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
+0000fa70: 6174 696f 6e20 3d20 7365 6c66 2e61 7069  ation = self.api
+0000fa80: 5f63 6c69 656e 742e 636f 6e66 6967 7572  _client.configur
+0000fa90: 6174 696f 6e0a 2020 2020 2020 2020 7472  ation.        tr
+0000faa0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
+0000fab0: 6620 686f 7374 5f69 6e64 6578 2069 7320  f host_index is 
+0000fac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000fad0: 2020 2020 2020 696e 6465 7820 3d20 636f        index = co
+0000fae0: 6e66 6967 7572 6174 696f 6e2e 7365 7276  nfiguration.serv
+0000faf0: 6572 5f6f 7065 7261 7469 6f6e 5f69 6e64  er_operation_ind
+0000fb00: 6578 2e67 6574 280a 2020 2020 2020 2020  ex.get(.        
+0000fb10: 2020 2020 2020 2020 2020 2020 6f70 6572              oper
+0000fb20: 6174 696f 6e5f 6964 2c20 636f 6e66 6967  ation_id, config
+0000fb30: 7572 6174 696f 6e2e 7365 7276 6572 5f69  uration.server_i
+0000fb40: 6e64 6578 0a20 2020 2020 2020 2020 2020  ndex.           
+0000fb50: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000fb60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000fb70: 2020 2020 2020 2020 2069 6e64 6578 203d           index =
+0000fb80: 2068 6f73 745f 696e 6465 780a 2020 2020   host_index.    
+0000fb90: 2020 2020 2020 2020 7365 7276 6572 5f76          server_v
+0000fba0: 6172 6961 626c 6573 203d 2063 6f6e 6669  ariables = confi
+0000fbb0: 6775 7261 7469 6f6e 2e73 6572 7665 725f  guration.server_
+0000fbc0: 6f70 6572 6174 696f 6e5f 7661 7269 6162  operation_variab
+0000fbd0: 6c65 732e 6765 7428 0a20 2020 2020 2020  les.get(.       
+0000fbe0: 2020 2020 2020 2020 206f 7065 7261 7469           operati
+0000fbf0: 6f6e 5f69 642c 2063 6f6e 6669 6775 7261  on_id, configura
+0000fc00: 7469 6f6e 2e73 6572 7665 725f 7661 7269  tion.server_vari
+0000fc10: 6162 6c65 730a 2020 2020 2020 2020 2020  ables.          
+0000fc20: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000fc30: 686f 7374 203d 2063 6f6e 6669 6775 7261  host = configura
+0000fc40: 7469 6f6e 2e67 6574 5f68 6f73 745f 6672  tion.get_host_fr
+0000fc50: 6f6d 5f73 6574 7469 6e67 7328 0a20 2020  om_settings(.   
+0000fc60: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000fc70: 6578 2c20 7661 7269 6162 6c65 733d 7365  ex, variables=se
+0000fc80: 7276 6572 5f76 6172 6961 626c 6573 2c20  rver_variables, 
+0000fc90: 7365 7276 6572 733d 7365 7276 6572 730a  servers=servers.
+0000fca0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000fcb0: 2020 2020 2020 6578 6365 7074 2049 6e64        except Ind
+0000fcc0: 6578 4572 726f 723a 0a20 2020 2020 2020  exError:.       
+0000fcd0: 2020 2020 2069 6620 7365 7276 6572 733a       if servers:
+0000fce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fcf0: 2072 6169 7365 2041 7069 5661 6c75 6545   raise ApiValueE
+0000fd00: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000fd10: 2020 2020 2020 2020 2020 2249 6e76 616c            "Inval
+0000fd20: 6964 2068 6f73 7420 696e 6465 782e 204d  id host index. M
+0000fd30: 7573 7420 6265 2030 203c 3d20 696e 6465  ust be 0 <= inde
+0000fd40: 7820 3c20 2573 2220 250a 2020 2020 2020  x < %s" %.      
+0000fd50: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000fd60: 6e28 7365 7276 6572 7329 0a20 2020 2020  n(servers).     
+0000fd70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000fd80: 2020 2020 2020 2020 2068 6f73 7420 3d20           host = 
+0000fd90: 4e6f 6e65 0a20 2020 2020 2020 2072 6574  None.        ret
+0000fda0: 7572 6e20 686f 7374 0a0a 0a63 6c61 7373  urn host...class
+0000fdb0: 2053 6572 6961 6c69 7a65 6452 6571 7565   SerializedReque
+0000fdc0: 7374 426f 6479 2874 7970 696e 675f 6578  stBody(typing_ex
+0000fdd0: 7465 6e73 696f 6e73 2e54 7970 6564 4469  tensions.TypedDi
+0000fde0: 6374 2c20 746f 7461 6c3d 4661 6c73 6529  ct, total=False)
+0000fdf0: 3a0a 2020 2020 626f 6479 3a20 7479 7069  :.    body: typi
+0000fe00: 6e67 2e55 6e69 6f6e 5b73 7472 2c20 6279  ng.Union[str, by
+0000fe10: 7465 735d 0a20 2020 2066 6965 6c64 733a  tes].    fields:
+0000fe20: 2074 7970 696e 672e 5475 706c 655b 7479   typing.Tuple[ty
+0000fe30: 7069 6e67 2e55 6e69 6f6e 5b52 6571 7565  ping.Union[Reque
+0000fe40: 7374 4669 656c 642c 2074 7970 696e 672e  stField, typing.
+0000fe50: 5475 706c 655b 7374 722c 2073 7472 5d5d  Tuple[str, str]]
+0000fe60: 2c20 2e2e 2e5d 0a0a 0a63 6c61 7373 2052  , ...]...class R
+0000fe70: 6571 7565 7374 426f 6479 2853 7479 6c65  equestBody(Style
+0000fe80: 466f 726d 5365 7269 616c 697a 6572 2c20  FormSerializer, 
+0000fe90: 4a53 4f4e 4465 7465 6374 6f72 293a 0a20  JSONDetector):. 
+0000fea0: 2020 2022 2222 0a20 2020 2041 2072 6571     """.    A req
+0000feb0: 7565 7374 2062 6f64 7920 7061 7261 6d65  uest body parame
+0000fec0: 7465 720a 2020 2020 636f 6e74 656e 743a  ter.    content:
+0000fed0: 2063 6f6e 7465 6e74 5f74 7970 6520 746f   content_type to
+0000fee0: 204d 6564 6961 5479 7065 2053 6368 656d   MediaType Schem
+0000fef0: 6120 696e 666f 0a20 2020 2022 2222 0a20  a info.    """. 
+0000ff00: 2020 205f 5f6a 736f 6e5f 656e 636f 6465     __json_encode
+0000ff10: 7220 3d20 4a53 4f4e 456e 636f 6465 7228  r = JSONEncoder(
+0000ff20: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
+0000ff30: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0000ff40: 662c 0a20 2020 2020 2020 2063 6f6e 7465  f,.        conte
+0000ff50: 6e74 3a20 7479 7069 6e67 2e44 6963 745b  nt: typing.Dict[
+0000ff60: 7374 722c 204d 6564 6961 5479 7065 5d2c  str, MediaType],
+0000ff70: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
+0000ff80: 643a 2062 6f6f 6c20 3d20 4661 6c73 652c  d: bool = False,
+0000ff90: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000ffa0: 7365 6c66 2e72 6571 7569 7265 6420 3d20  self.required = 
+0000ffb0: 7265 7175 6972 6564 0a20 2020 2020 2020  required.       
+0000ffc0: 2069 6620 6c65 6e28 636f 6e74 656e 7429   if len(content)
+0000ffd0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0000ffe0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000fff0: 726f 7228 2749 6e76 616c 6964 2076 616c  ror('Invalid val
+00010000: 7565 2066 6f72 2063 6f6e 7465 6e74 2c20  ue for content, 
+00010010: 7468 6520 636f 6e74 656e 7420 6469 6374  the content dict
+00010020: 206d 7573 7420 6861 7665 203e 3d20 3120   must have >= 1 
+00010030: 656e 7472 7927 290a 2020 2020 2020 2020  entry').        
+00010040: 7365 6c66 2e63 6f6e 7465 6e74 203d 2063  self.content = c
+00010050: 6f6e 7465 6e74 0a0a 2020 2020 6465 6620  ontent..    def 
+00010060: 5f5f 7365 7269 616c 697a 655f 6a73 6f6e  __serialize_json
+00010070: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00010080: 2020 2020 2020 2020 696e 5f64 6174 613a          in_data:
+00010090: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
+000100a0: 2920 2d3e 2074 7970 696e 672e 4469 6374  ) -> typing.Dict
+000100b0: 5b73 7472 2c20 6279 7465 735d 3a0a 2020  [str, bytes]:.  
+000100c0: 2020 2020 2020 696e 5f64 6174 6120 3d20        in_data = 
+000100d0: 7365 6c66 2e5f 5f6a 736f 6e5f 656e 636f  self.__json_enco
+000100e0: 6465 722e 6465 6661 756c 7428 696e 5f64  der.default(in_d
+000100f0: 6174 6129 0a20 2020 2020 2020 206a 736f  ata).        jso
+00010100: 6e5f 7374 7220 3d20 6a73 6f6e 2e64 756d  n_str = json.dum
+00010110: 7073 2869 6e5f 6461 7461 2c20 7365 7061  ps(in_data, sepa
+00010120: 7261 746f 7273 3d28 222c 222c 2022 3a22  rators=(",", ":"
+00010130: 292c 2065 6e73 7572 655f 6173 6369 693d  ), ensure_ascii=
+00010140: 4661 6c73 6529 2e65 6e63 6f64 6528 0a20  False).encode(. 
+00010150: 2020 2020 2020 2020 2020 2022 7574 662d             "utf-
+00010160: 3822 0a20 2020 2020 2020 2029 0a20 2020  8".        ).   
+00010170: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
+00010180: 2862 6f64 793d 6a73 6f6e 5f73 7472 290a  (body=json_str).
+00010190: 0a20 2020 2040 7374 6174 6963 6d65 7468  .    @staticmeth
+000101a0: 6f64 0a20 2020 2064 6566 205f 5f73 6572  od.    def __ser
+000101b0: 6961 6c69 7a65 5f74 6578 745f 706c 6169  ialize_text_plai
+000101c0: 6e28 696e 5f64 6174 613a 2074 7970 696e  n(in_data: typin
+000101d0: 672e 416e 7929 202d 3e20 7479 7069 6e67  g.Any) -> typing
+000101e0: 2e44 6963 745b 7374 722c 2073 7472 5d3a  .Dict[str, str]:
+000101f0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
+00010200: 7374 616e 6365 2869 6e5f 6461 7461 2c20  stance(in_data, 
+00010210: 6672 6f7a 656e 6469 6374 2e66 726f 7a65  frozendict.froze
+00010220: 6e64 6963 7429 3a0a 2020 2020 2020 2020  ndict):.        
+00010230: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00010240: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
+00010250: 7365 7269 616c 697a 6520 7479 7065 2066  serialize type f
+00010260: 726f 7a65 6e64 6963 742e 6672 6f7a 656e  rozendict.frozen
+00010270: 6469 6374 2074 6f20 7465 7874 2f70 6c61  dict to text/pla
+00010280: 696e 2729 0a20 2020 2020 2020 2065 6c69  in').        eli
+00010290: 6620 6973 696e 7374 616e 6365 2869 6e5f  f isinstance(in_
+000102a0: 6461 7461 2c20 7475 706c 6529 3a0a 2020  data, tuple):.  
+000102b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000102c0: 5661 6c75 6545 7272 6f72 2827 556e 6162  ValueError('Unab
+000102d0: 6c65 2074 6f20 7365 7269 616c 697a 6520  le to serialize 
+000102e0: 7479 7065 2074 7570 6c65 2074 6f20 7465  type tuple to te
+000102f0: 7874 2f70 6c61 696e 2729 0a20 2020 2020  xt/plain').     
+00010300: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00010310: 6365 2869 6e5f 6461 7461 2c20 4e6f 6e65  ce(in_data, None
+00010320: 436c 6173 7329 3a0a 2020 2020 2020 2020  Class):.        
+00010330: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00010340: 7272 6f72 2827 556e 6162 6c65 2074 6f20  rror('Unable to 
+00010350: 7365 7269 616c 697a 6520 7479 7065 204e  serialize type N
+00010360: 6f6e 6543 6c61 7373 2074 6f20 7465 7874  oneClass to text
+00010370: 2f70 6c61 696e 2729 0a20 2020 2020 2020  /plain').       
+00010380: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00010390: 2869 6e5f 6461 7461 2c20 426f 6f6c 436c  (in_data, BoolCl
+000103a0: 6173 7329 3a0a 2020 2020 2020 2020 2020  ass):.          
+000103b0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000103c0: 6f72 2827 556e 6162 6c65 2074 6f20 7365  or('Unable to se
+000103d0: 7269 616c 697a 6520 7479 7065 2042 6f6f  rialize type Boo
+000103e0: 6c43 6c61 7373 2074 6f20 7465 7874 2f70  lClass to text/p
+000103f0: 6c61 696e 2729 0a20 2020 2020 2020 2072  lain').        r
+00010400: 6574 7572 6e20 6469 6374 2862 6f64 793d  eturn dict(body=
+00010410: 7374 7228 696e 5f64 6174 6129 290a 0a20  str(in_data)).. 
+00010420: 2020 2064 6566 205f 5f6d 756c 7469 7061     def __multipa
+00010430: 7274 5f6a 736f 6e5f 6974 656d 2873 656c  rt_json_item(sel
+00010440: 662c 206b 6579 3a20 7374 722c 2076 616c  f, key: str, val
+00010450: 7565 3a20 5363 6865 6d61 2920 2d3e 2052  ue: Schema) -> R
+00010460: 6571 7565 7374 4669 656c 643a 0a20 2020  equestField:.   
+00010470: 2020 2020 206a 736f 6e5f 7661 6c75 6520       json_value 
+00010480: 3d20 7365 6c66 2e5f 5f6a 736f 6e5f 656e  = self.__json_en
+00010490: 636f 6465 722e 6465 6661 756c 7428 7661  coder.default(va
+000104a0: 6c75 6529 0a20 2020 2020 2020 2072 6574  lue).        ret
+000104b0: 7572 6e20 5265 7175 6573 7446 6965 6c64  urn RequestField
+000104c0: 286e 616d 653d 6b65 792c 2064 6174 613d  (name=key, data=
+000104d0: 6a73 6f6e 2e64 756d 7073 286a 736f 6e5f  json.dumps(json_
+000104e0: 7661 6c75 6529 2c20 6865 6164 6572 733d  value), headers=
+000104f0: 7b27 436f 6e74 656e 742d 5479 7065 273a  {'Content-Type':
+00010500: 2027 6170 706c 6963 6174 696f 6e2f 6a73   'application/js
+00010510: 6f6e 277d 290a 0a20 2020 2064 6566 205f  on'})..    def _
+00010520: 5f6d 756c 7469 7061 7274 5f66 6f72 6d5f  _multipart_form_
+00010530: 6974 656d 2873 656c 662c 206b 6579 3a20  item(self, key: 
+00010540: 7374 722c 2076 616c 7565 3a20 5363 6865  str, value: Sche
+00010550: 6d61 2920 2d3e 2052 6571 7565 7374 4669  ma) -> RequestFi
+00010560: 656c 643a 0a20 2020 2020 2020 2069 6620  eld:.        if 
+00010570: 6973 696e 7374 616e 6365 2876 616c 7565  isinstance(value
+00010580: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+00010590: 2020 2020 7265 7475 726e 2052 6571 7565      return Reque
+000105a0: 7374 4669 656c 6428 6e61 6d65 3d6b 6579  stField(name=key
+000105b0: 2c20 6461 7461 3d73 7472 2876 616c 7565  , data=str(value
+000105c0: 292c 2068 6561 6465 7273 3d7b 2743 6f6e  ), headers={'Con
+000105d0: 7465 6e74 2d54 7970 6527 3a20 2774 6578  tent-Type': 'tex
+000105e0: 742f 706c 6169 6e27 7d29 0a20 2020 2020  t/plain'}).     
+000105f0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00010600: 6365 2876 616c 7565 2c20 6279 7465 7329  ce(value, bytes)
+00010610: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00010620: 7475 726e 2052 6571 7565 7374 4669 656c  turn RequestFiel
+00010630: 6428 6e61 6d65 3d6b 6579 2c20 6461 7461  d(name=key, data
+00010640: 3d76 616c 7565 2c20 6865 6164 6572 733d  =value, headers=
+00010650: 7b27 436f 6e74 656e 742d 5479 7065 273a  {'Content-Type':
+00010660: 2027 6170 706c 6963 6174 696f 6e2f 6f63   'application/oc
+00010670: 7465 742d 7374 7265 616d 277d 290a 2020  tet-stream'}).  
+00010680: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+00010690: 7461 6e63 6528 7661 6c75 652c 2046 696c  tance(value, Fil
+000106a0: 6549 4f29 3a0a 2020 2020 2020 2020 2020  eIO):.          
+000106b0: 2020 6669 6c65 6e61 6d65 203d 206f 732e    filename = os.
+000106c0: 7061 7468 2e62 6173 656e 616d 6528 7661  path.basename(va
+000106d0: 6c75 652e 6e61 6d65 290a 2020 2020 2020  lue.name).      
+000106e0: 2020 2020 2020 7265 7175 6573 745f 6669        request_fi
+000106f0: 656c 6420 3d20 5265 7175 6573 7446 6965  eld = RequestFie
+00010700: 6c64 280a 2020 2020 2020 2020 2020 2020  ld(.            
+00010710: 2020 2020 6e61 6d65 3d6b 6579 2c0a 2020      name=key,.  
+00010720: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00010730: 7461 3d76 616c 7565 2e72 6561 6428 292c  ta=value.read(),
+00010740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010750: 2066 696c 656e 616d 653d 6669 6c65 6e61   filename=filena
+00010760: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+00010770: 2020 2020 6865 6164 6572 733d 7b27 436f      headers={'Co
+00010780: 6e74 656e 742d 5479 7065 273a 2067 7565  ntent-Type': gue
+00010790: 7373 5f63 6f6e 7465 6e74 5f74 7970 6528  ss_content_type(
+000107a0: 6669 6c65 6e61 6d65 297d 0a20 2020 2020  filename)}.     
+000107b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000107c0: 2020 2020 2076 616c 7565 2e63 6c6f 7365       value.close
+000107d0: 2829 0a20 2020 2020 2020 2020 2020 2072  ().            r
+000107e0: 6574 7572 6e20 7265 7175 6573 745f 6669  eturn request_fi
+000107f0: 656c 640a 2020 2020 2020 2020 656c 7365  eld.        else
+00010800: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00010810: 7475 726e 2073 656c 662e 5f5f 6d75 6c74  turn self.__mult
+00010820: 6970 6172 745f 6a73 6f6e 5f69 7465 6d28  ipart_json_item(
+00010830: 6b65 793d 6b65 792c 2076 616c 7565 3d76  key=key, value=v
+00010840: 616c 7565 290a 0a20 2020 2064 6566 205f  alue)..    def _
+00010850: 5f73 6572 6961 6c69 7a65 5f6d 756c 7469  _serialize_multi
+00010860: 7061 7274 5f66 6f72 6d5f 6461 7461 280a  part_form_data(.
+00010870: 2020 2020 2020 2020 7365 6c66 2c20 696e          self, in
+00010880: 5f64 6174 613a 2053 6368 656d 610a 2020  _data: Schema.  
+00010890: 2020 2920 2d3e 2074 7970 696e 672e 4469    ) -> typing.Di
+000108a0: 6374 5b73 7472 2c20 7479 7069 6e67 2e54  ct[str, typing.T
+000108b0: 7570 6c65 5b52 6571 7565 7374 4669 656c  uple[RequestFiel
+000108c0: 642c 202e 2e2e 5d5d 3a0a 2020 2020 2020  d, ...]]:.      
+000108d0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+000108e0: 6e63 6528 696e 5f64 6174 612c 2066 726f  nce(in_data, fro
+000108f0: 7a65 6e64 6963 742e 6672 6f7a 656e 6469  zendict.frozendi
+00010900: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+00010910: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00010920: 7228 6627 556e 6162 6c65 2074 6f20 7365  r(f'Unable to se
+00010930: 7269 616c 697a 6520 7b69 6e5f 6461 7461  rialize {in_data
+00010940: 7d20 746f 206d 756c 7469 7061 7274 2f66  } to multipart/f
+00010950: 6f72 6d2d 6461 7461 2062 6563 6175 7365  orm-data because
+00010960: 2069 7420 6973 206e 6f74 2061 2064 6963   it is not a dic
+00010970: 7420 6f66 2064 6174 6127 290a 2020 2020  t of data').    
+00010980: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010990: 496e 2061 206d 756c 7469 7061 7274 2f66  In a multipart/f
+000109a0: 6f72 6d2d 6461 7461 2072 6571 7565 7374  orm-data request
+000109b0: 2062 6f64 792c 2065 6163 6820 7363 6865   body, each sche
+000109c0: 6d61 2070 726f 7065 7274 792c 206f 7220  ma property, or 
+000109d0: 6561 6368 2065 6c65 6d65 6e74 206f 6620  each element of 
+000109e0: 6120 7363 6865 6d61 2061 7272 6179 2070  a schema array p
+000109f0: 726f 7065 7274 792c 0a20 2020 2020 2020  roperty,.       
+00010a00: 2074 616b 6573 2061 2073 6563 7469 6f6e   takes a section
+00010a10: 2069 6e20 7468 6520 7061 796c 6f61 6420   in the payload 
+00010a20: 7769 7468 2061 6e20 696e 7465 726e 616c  with an internal
+00010a30: 2068 6561 6465 7220 6173 2064 6566 696e   header as defin
+00010a40: 6564 2062 7920 5246 4337 3537 382e 2054  ed by RFC7578. T
+00010a50: 6865 2073 6572 6961 6c69 7a61 7469 6f6e  he serialization
+00010a60: 2073 7472 6174 6567 790a 2020 2020 2020   strategy.      
+00010a70: 2020 666f 7220 6561 6368 2070 726f 7065    for each prope
+00010a80: 7274 7920 6f66 2061 206d 756c 7469 7061  rty of a multipa
+00010a90: 7274 2f66 6f72 6d2d 6461 7461 2072 6571  rt/form-data req
+00010aa0: 7565 7374 2062 6f64 7920 6361 6e20 6265  uest body can be
+00010ab0: 2073 7065 6369 6669 6564 2069 6e20 616e   specified in an
+00010ac0: 2061 7373 6f63 6961 7465 6420 456e 636f   associated Enco
+00010ad0: 6469 6e67 204f 626a 6563 742e 0a0a 2020  ding Object...  
+00010ae0: 2020 2020 2020 5768 656e 2070 6173 7369        When passi
+00010af0: 6e67 2069 6e20 6d75 6c74 6970 6172 7420  ng in multipart 
+00010b00: 7479 7065 732c 2062 6f75 6e64 6172 6965  types, boundarie
+00010b10: 7320 4d41 5920 6265 2075 7365 6420 746f  s MAY be used to
+00010b20: 2073 6570 6172 6174 6520 7365 6374 696f   separate sectio
+00010b30: 6e73 206f 6620 7468 6520 636f 6e74 656e  ns of the conten
+00010b40: 7420 6265 696e 670a 2020 2020 2020 2020  t being.        
+00010b50: 7472 616e 7366 6572 7265 6420 e280 9320  transferred ... 
+00010b60: 7468 7573 2c20 7468 6520 666f 6c6c 6f77  thus, the follow
+00010b70: 696e 6720 6465 6661 756c 7420 436f 6e74  ing default Cont
+00010b80: 656e 742d 5479 7065 7320 6172 6520 6465  ent-Types are de
+00010b90: 6669 6e65 6420 666f 7220 6d75 6c74 6970  fined for multip
+00010ba0: 6172 743a 0a0a 2020 2020 2020 2020 4966  art:..        If
+00010bb0: 2074 6865 2028 6f62 6a65 6374 2920 7072   the (object) pr
+00010bc0: 6f70 6572 7479 2069 7320 6120 7072 696d  operty is a prim
+00010bd0: 6974 6976 652c 206f 7220 616e 2061 7272  itive, or an arr
+00010be0: 6179 206f 6620 7072 696d 6974 6976 6520  ay of primitive 
+00010bf0: 7661 6c75 6573 2c20 7468 6520 6465 6661  values, the defa
+00010c00: 756c 7420 436f 6e74 656e 742d 5479 7065  ult Content-Type
+00010c10: 2069 7320 7465 7874 2f70 6c61 696e 0a20   is text/plain. 
+00010c20: 2020 2020 2020 2049 6620 7468 6520 7072         If the pr
+00010c30: 6f70 6572 7479 2069 7320 636f 6d70 6c65  operty is comple
+00010c40: 782c 206f 7220 616e 2061 7272 6179 206f  x, or an array o
+00010c50: 6620 636f 6d70 6c65 7820 7661 6c75 6573  f complex values
+00010c60: 2c20 7468 6520 6465 6661 756c 7420 436f  , the default Co
+00010c70: 6e74 656e 742d 5479 7065 2069 7320 6170  ntent-Type is ap
+00010c80: 706c 6963 6174 696f 6e2f 6a73 6f6e 0a20  plication/json. 
+00010c90: 2020 2020 2020 2020 2020 2051 7565 7374             Quest
+00010ca0: 696f 6e3a 2068 6f77 2069 7320 7468 6520  ion: how is the 
+00010cb0: 6172 7261 7920 6f66 2070 7269 6d69 7469  array of primiti
+00010cc0: 7665 7320 656e 636f 6465 643f 0a20 2020  ves encoded?.   
+00010cd0: 2020 2020 2049 6620 7468 6520 7072 6f70       If the prop
+00010ce0: 6572 7479 2069 7320 6120 7479 7065 3a20  erty is a type: 
+00010cf0: 7374 7269 6e67 2077 6974 6820 6120 636f  string with a co
+00010d00: 6e74 656e 7445 6e63 6f64 696e 672c 2074  ntentEncoding, t
+00010d10: 6865 2064 6566 6175 6c74 2043 6f6e 7465  he default Conte
+00010d20: 6e74 2d54 7970 6520 6973 2061 7070 6c69  nt-Type is appli
+00010d30: 6361 7469 6f6e 2f6f 6374 6574 2d73 7472  cation/octet-str
+00010d40: 6561 6d0a 2020 2020 2020 2020 2222 220a  eam.        """.
+00010d50: 2020 2020 2020 2020 6669 656c 6473 3a20          fields: 
+00010d60: 7479 7069 6e67 2e4c 6973 745b 5265 7175  typing.List[Requ
+00010d70: 6573 7446 6965 6c64 5d20 3d20 5b5d 0a20  estField] = []. 
+00010d80: 2020 2020 2020 2066 6f72 206b 6579 2c20         for key, 
+00010d90: 7661 6c75 6520 696e 2069 6e5f 6461 7461  value in in_data
+00010da0: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00010db0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00010dc0: 6e63 6528 7661 6c75 652c 2074 7570 6c65  nce(value, tuple
+00010dd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010de0: 2020 2069 6620 7661 6c75 653a 0a20 2020     if value:.   
+00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e00: 2023 2076 616c 7565 7320 7573 6520 6578   # values use ex
+00010e10: 706c 6f64 6520 3d20 5472 7565 2c20 736f  plode = True, so
+00010e20: 2074 6865 2063 6f64 6520 6d61 6b65 7320   the code makes 
+00010e30: 6120 5265 7175 6573 7446 6965 6c64 2066  a RequestField f
+00010e40: 6f72 2065 6163 6820 6974 656d 2077 6974  or each item wit
+00010e50: 6820 6e61 6d65 3d6b 6579 0a20 2020 2020  h name=key.     
+00010e60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00010e70: 6f72 2069 7465 6d20 696e 2076 616c 7565  or item in value
+00010e80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010e90: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+00010ea0: 745f 6669 656c 6420 3d20 7365 6c66 2e5f  t_field = self._
+00010eb0: 5f6d 756c 7469 7061 7274 5f66 6f72 6d5f  _multipart_form_
+00010ec0: 6974 656d 286b 6579 3d6b 6579 2c20 7661  item(key=key, va
+00010ed0: 6c75 653d 6974 656d 290a 2020 2020 2020  lue=item).      
+00010ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ef0: 2020 6669 656c 6473 2e61 7070 656e 6428    fields.append(
+00010f00: 7265 7175 6573 745f 6669 656c 6429 0a20  request_field). 
+00010f10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00010f20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00010f30: 2020 2020 2020 2020 2023 2073 656e 6420           # send 
+00010f40: 616e 2065 6d70 7479 2061 7272 6179 2061  an empty array a
+00010f50: 7320 6a73 6f6e 2062 6563 6175 7365 2065  s json because e
+00010f60: 7870 6c6f 6469 6e67 2077 696c 6c20 6e6f  xploding will no
+00010f70: 7420 7365 6e64 2069 740a 2020 2020 2020  t send it.      
+00010f80: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00010f90: 7175 6573 745f 6669 656c 6420 3d20 7365  quest_field = se
+00010fa0: 6c66 2e5f 5f6d 756c 7469 7061 7274 5f6a  lf.__multipart_j
+00010fb0: 736f 6e5f 6974 656d 286b 6579 3d6b 6579  son_item(key=key
+00010fc0: 2c20 7661 6c75 653d 7661 6c75 6529 0a20  , value=value). 
+00010fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fe0: 2020 2066 6965 6c64 732e 6170 7065 6e64     fields.append
+00010ff0: 2872 6571 7565 7374 5f66 6965 6c64 290a  (request_field).
+00011000: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00011010: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011020: 2020 7265 7175 6573 745f 6669 656c 6420    request_field 
+00011030: 3d20 7365 6c66 2e5f 5f6d 756c 7469 7061  = self.__multipa
+00011040: 7274 5f66 6f72 6d5f 6974 656d 286b 6579  rt_form_item(key
+00011050: 3d6b 6579 2c20 7661 6c75 653d 7661 6c75  =key, value=valu
+00011060: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00011070: 2020 2066 6965 6c64 732e 6170 7065 6e64     fields.append
+00011080: 2872 6571 7565 7374 5f66 6965 6c64 290a  (request_field).
+00011090: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+000110a0: 6973 206e 6563 6573 7361 7279 2074 6f20  is necessary to 
+000110b0: 6669 6c6c 2074 6865 2022 436f 6e74 656e  fill the "Conten
+000110c0: 742d 4469 7370 6f73 6974 696f 6e22 2068  t-Disposition" h
+000110d0: 6561 6465 7220 6e65 6564 6564 2066 6f72  eader needed for
+000110e0: 206e 616d 696e 6720 6669 656c 6473 2069   naming fields i
+000110f0: 6e20 6d75 6c74 6970 6172 740a 2020 2020  n multipart.    
+00011100: 2020 2020 666f 7220 6669 656c 6420 696e      for field in
+00011110: 2066 6965 6c64 733a 0a20 2020 2020 2020   fields:.       
+00011120: 2020 2020 2066 6965 6c64 2e6d 616b 655f       field.make_
+00011130: 6d75 6c74 6970 6172 7428 636f 6e74 656e  multipart(conten
+00011140: 745f 7479 7065 3d66 6965 6c64 2e68 6561  t_type=field.hea
+00011150: 6465 7273 5b22 436f 6e74 656e 742d 5479  ders["Content-Ty
+00011160: 7065 225d 290a 2020 2020 2020 2020 7265  pe"]).        re
+00011170: 7475 726e 2064 6963 7428 6669 656c 6473  turn dict(fields
+00011180: 3d74 7570 6c65 2866 6965 6c64 7329 290a  =tuple(fields)).
+00011190: 0a20 2020 2064 6566 205f 5f73 6572 6961  .    def __seria
+000111a0: 6c69 7a65 5f61 7070 6c69 6361 7469 6f6e  lize_application
+000111b0: 5f6f 6374 6574 5f73 7472 6561 6d28 7365  _octet_stream(se
+000111c0: 6c66 2c20 696e 5f64 6174 613a 2042 696e  lf, in_data: Bin
+000111d0: 6172 7953 6368 656d 6129 202d 3e20 7479  arySchema) -> ty
+000111e0: 7069 6e67 2e44 6963 745b 7374 722c 2062  ping.Dict[str, b
+000111f0: 7974 6573 5d3a 0a20 2020 2020 2020 2069  ytes]:.        i
+00011200: 6620 6973 696e 7374 616e 6365 2869 6e5f  f isinstance(in_
+00011210: 6461 7461 2c20 6279 7465 7329 3a0a 2020  data, bytes):.  
+00011220: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011230: 2064 6963 7428 626f 6479 3d69 6e5f 6461   dict(body=in_da
+00011240: 7461 290a 2020 2020 2020 2020 2320 4669  ta).        # Fi
+00011250: 6c65 494f 2074 7970 650a 2020 2020 2020  leIO type.      
+00011260: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00011270: 626f 6479 3d69 6e5f 6461 7461 2e72 6561  body=in_data.rea
+00011280: 6428 2929 0a20 2020 2020 2020 2069 6e5f  d()).        in_
+00011290: 6461 7461 2e63 6c6f 7365 2829 0a20 2020  data.close().   
+000112a0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+000112b0: 6c74 0a0a 2020 2020 6465 6620 5f5f 7365  lt..    def __se
+000112c0: 7269 616c 697a 655f 6170 706c 6963 6174  rialize_applicat
+000112d0: 696f 6e5f 785f 7777 775f 666f 726d 5f64  ion_x_www_form_d
+000112e0: 6174 6128 0a20 2020 2020 2020 2073 656c  ata(.        sel
+000112f0: 662c 2069 6e5f 6461 7461 3a20 7479 7069  f, in_data: typi
+00011300: 6e67 2e41 6e79 0a20 2020 2029 202d 3e20  ng.Any.    ) -> 
+00011310: 5365 7269 616c 697a 6564 5265 7175 6573  SerializedReques
+00011320: 7442 6f64 793a 0a20 2020 2020 2020 2022  tBody:.        "
+00011330: 2222 0a20 2020 2020 2020 2050 4f53 5420  "".        POST 
+00011340: 7375 626d 6973 7369 6f6e 206f 6620 666f  submission of fo
+00011350: 726d 2064 6174 6120 696e 2062 6f64 790a  rm data in body.
+00011360: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011370: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
+00011380: 7461 6e63 6528 696e 5f64 6174 612c 2066  tance(in_data, f
+00011390: 726f 7a65 6e64 6963 742e 6672 6f7a 656e  rozendict.frozen
+000113a0: 6469 6374 293a 0a20 2020 2020 2020 2020  dict):.         
+000113b0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+000113c0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+000113d0: 2020 2020 2066 2755 6e61 626c 6520 746f       f'Unable to
+000113e0: 2073 6572 6961 6c69 7a65 207b 696e 5f64   serialize {in_d
+000113f0: 6174 617d 2074 6f20 6170 706c 6963 6174  ata} to applicat
+00011400: 696f 6e2f 782d 7777 772d 666f 726d 2d75  ion/x-www-form-u
+00011410: 726c 656e 636f 6465 6420 6265 6361 7573  rlencoded becaus
+00011420: 6520 6974 2069 7320 6e6f 7420 6120 6469  e it is not a di
+00011430: 6374 206f 6620 6461 7461 2729 0a20 2020  ct of data').   
+00011440: 2020 2020 2063 6173 745f 696e 5f64 6174       cast_in_dat
+00011450: 6120 3d20 7365 6c66 2e5f 5f6a 736f 6e5f  a = self.__json_
+00011460: 656e 636f 6465 722e 6465 6661 756c 7428  encoder.default(
+00011470: 696e 5f64 6174 6129 0a20 2020 2020 2020  in_data).       
+00011480: 2076 616c 7565 203d 2073 656c 662e 5f73   value = self._s
+00011490: 6572 6961 6c69 7a65 5f66 6f72 6d28 6361  erialize_form(ca
+000114a0: 7374 5f69 6e5f 6461 7461 2c20 6e61 6d65  st_in_data, name
+000114b0: 3d27 272c 2065 7870 6c6f 6465 3d54 7275  ='', explode=Tru
+000114c0: 652c 2070 6572 6365 6e74 5f65 6e63 6f64  e, percent_encod
+000114d0: 653d 5472 7565 290a 2020 2020 2020 2020  e=True).        
+000114e0: 7265 7475 726e 2064 6963 7428 626f 6479  return dict(body
+000114f0: 3d76 616c 7565 290a 0a20 2020 2064 6566  =value)..    def
+00011500: 2073 6572 6961 6c69 7a65 280a 2020 2020   serialize(.    
+00011510: 2020 2020 7365 6c66 2c20 696e 5f64 6174      self, in_dat
+00011520: 613a 2074 7970 696e 672e 416e 792c 2063  a: typing.Any, c
+00011530: 6f6e 7465 6e74 5f74 7970 653a 2073 7472  ontent_type: str
+00011540: 0a20 2020 2029 202d 3e20 5365 7269 616c  .    ) -> Serial
+00011550: 697a 6564 5265 7175 6573 7442 6f64 793a  izedRequestBody:
+00011560: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011570: 2020 2020 2049 6620 6120 7374 7220 6973       If a str is
+00011580: 2072 6574 7572 6e65 6420 7468 656e 2074   returned then t
+00011590: 6865 2072 6573 756c 7420 7769 6c6c 2062  he result will b
+000115a0: 6520 6173 7369 676e 6564 2074 6f20 6461  e assigned to da
+000115b0: 7461 2077 6865 6e20 6d61 6b69 6e67 2074  ta when making t
+000115c0: 6865 2072 6571 7565 7374 0a20 2020 2020  he request.     
+000115d0: 2020 2049 6620 6120 7475 706c 6520 6973     If a tuple is
+000115e0: 2072 6574 7572 6e65 6420 7468 656e 2074   returned then t
+000115f0: 6865 2072 6573 756c 7420 7769 6c6c 2062  he result will b
+00011600: 6520 7573 6564 2061 7320 6669 656c 6473  e used as fields
+00011610: 2069 6e70 7574 2069 6e20 656e 636f 6465   input in encode
+00011620: 5f6d 756c 7469 7061 7274 5f66 6f72 6d64  _multipart_formd
+00011630: 6174 610a 2020 2020 2020 2020 5265 7475  ata.        Retu
+00011640: 726e 2061 2074 7570 6c65 206f 660a 0a20  rn a tuple of.. 
+00011650: 2020 2020 2020 2054 6865 206b 6579 206f         The key o
+00011660: 6620 7468 6520 7265 7475 726e 2064 6963  f the return dic
+00011670: 7420 6973 0a20 2020 2020 2020 202d 2062  t is.        - b
+00011680: 6f64 7920 666f 7220 6170 706c 6963 6174  ody for applicat
+00011690: 696f 6e2f 6a73 6f6e 0a20 2020 2020 2020  ion/json.       
+000116a0: 202d 2065 6e63 6f64 655f 6d75 6c74 6970   - encode_multip
+000116b0: 6172 7420 616e 6420 6669 656c 6473 2066  art and fields f
+000116c0: 6f72 206d 756c 7469 7061 7274 2f66 6f72  or multipart/for
+000116d0: 6d2d 6461 7461 0a20 2020 2020 2020 2022  m-data.        "
+000116e0: 2222 0a20 2020 2020 2020 206d 6564 6961  "".        media
+000116f0: 5f74 7970 6520 3d20 7365 6c66 2e63 6f6e  _type = self.con
+00011700: 7465 6e74 5b63 6f6e 7465 6e74 5f74 7970  tent[content_typ
+00011710: 655d 0a20 2020 2020 2020 2069 6620 6973  e].        if is
+00011720: 696e 7374 616e 6365 2869 6e5f 6461 7461  instance(in_data
+00011730: 2c20 6d65 6469 615f 7479 7065 2e73 6368  , media_type.sch
+00011740: 656d 6129 3a0a 2020 2020 2020 2020 2020  ema):.          
+00011750: 2020 6361 7374 5f69 6e5f 6461 7461 203d    cast_in_data =
+00011760: 2069 6e5f 6461 7461 0a20 2020 2020 2020   in_data.       
+00011770: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00011780: 2869 6e5f 6461 7461 2c20 2864 6963 742c  (in_data, (dict,
+00011790: 2066 726f 7a65 6e64 6963 742e 6672 6f7a   frozendict.froz
+000117a0: 656e 6469 6374 2929 2061 6e64 2069 6e5f  endict)) and in_
+000117b0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
+000117c0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000117d0: 2020 2020 2020 2063 6173 745f 696e 5f64         cast_in_d
+000117e0: 6174 6120 3d20 6d65 6469 615f 7479 7065  ata = media_type
+000117f0: 2e73 6368 656d 6128 2a2a 696e 5f64 6174  .schema(**in_dat
+00011800: 6129 0a20 2020 2020 2020 2020 2020 2065  a).            e
+00011810: 7863 6570 7420 5479 7065 4572 726f 7220  xcept TypeError 
+00011820: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00011830: 2020 2020 2020 7261 6973 6520 4d69 7373        raise Miss
+00011840: 696e 6752 6571 7569 7265 6450 6172 616d  ingRequiredParam
+00011850: 6574 6572 7345 7272 6f72 2865 290a 2020  etersError(e).  
+00011860: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00011870: 2020 2020 2020 2020 6361 7374 5f69 6e5f          cast_in_
+00011880: 6461 7461 203d 206d 6564 6961 5f74 7970  data = media_typ
+00011890: 652e 7363 6865 6d61 2869 6e5f 6461 7461  e.schema(in_data
+000118a0: 290a 2020 2020 2020 2020 2320 544f 444f  ).        # TODO
+000118b0: 2063 6865 636b 2066 6f72 2061 6e64 2075   check for and u
+000118c0: 7365 2065 6e63 6f64 696e 6720 6966 2069  se encoding if i
+000118d0: 7420 6578 6973 7473 0a20 2020 2020 2020  t exists.       
+000118e0: 2023 2061 6e64 2063 6f6e 7465 6e74 5f74   # and content_t
+000118f0: 7970 6520 6973 206d 756c 7469 7061 7274  ype is multipart
+00011900: 206f 7220 6170 706c 6963 6174 696f 6e2f   or application/
+00011910: 782d 7777 772d 666f 726d 2d75 726c 656e  x-www-form-urlen
+00011920: 636f 6465 640a 2020 2020 2020 2020 6966  coded.        if
+00011930: 2073 656c 662e 5f63 6f6e 7465 6e74 5f74   self._content_t
+00011940: 7970 655f 6973 5f6a 736f 6e28 636f 6e74  ype_is_json(cont
+00011950: 656e 745f 7479 7065 293a 0a20 2020 2020  ent_type):.     
+00011960: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011970: 6c66 2e5f 5f73 6572 6961 6c69 7a65 5f6a  lf.__serialize_j
+00011980: 736f 6e28 6361 7374 5f69 6e5f 6461 7461  son(cast_in_data
+00011990: 290a 2020 2020 2020 2020 656c 6966 2063  ).        elif c
+000119a0: 6f6e 7465 6e74 5f74 7970 6520 3d3d 2027  ontent_type == '
+000119b0: 7465 7874 2f70 6c61 696e 273a 0a20 2020  text/plain':.   
+000119c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000119d0: 7365 6c66 2e5f 5f73 6572 6961 6c69 7a65  self.__serialize
+000119e0: 5f74 6578 745f 706c 6169 6e28 6361 7374  _text_plain(cast
+000119f0: 5f69 6e5f 6461 7461 290a 2020 2020 2020  _in_data).      
+00011a00: 2020 656c 6966 2063 6f6e 7465 6e74 5f74    elif content_t
+00011a10: 7970 6520 3d3d 2027 6d75 6c74 6970 6172  ype == 'multipar
+00011a20: 742f 666f 726d 2d64 6174 6127 3a0a 2020  t/form-data':.  
+00011a30: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011a40: 2073 656c 662e 5f5f 7365 7269 616c 697a   self.__serializ
+00011a50: 655f 6d75 6c74 6970 6172 745f 666f 726d  e_multipart_form
+00011a60: 5f64 6174 6128 6361 7374 5f69 6e5f 6461  _data(cast_in_da
+00011a70: 7461 290a 2020 2020 2020 2020 656c 6966  ta).        elif
+00011a80: 2063 6f6e 7465 6e74 5f74 7970 6520 3d3d   content_type ==
+00011a90: 2027 6170 706c 6963 6174 696f 6e2f 782d   'application/x-
+00011aa0: 7777 772d 666f 726d 2d75 726c 656e 636f  www-form-urlenco
+00011ab0: 6465 6427 3a0a 2020 2020 2020 2020 2020  ded':.          
+00011ac0: 2020 7265 7475 726e 2073 656c 662e 5f5f    return self.__
+00011ad0: 7365 7269 616c 697a 655f 6170 706c 6963  serialize_applic
+00011ae0: 6174 696f 6e5f 785f 7777 775f 666f 726d  ation_x_www_form
+00011af0: 5f64 6174 6128 6361 7374 5f69 6e5f 6461  _data(cast_in_da
+00011b00: 7461 290a 2020 2020 2020 2020 656c 6966  ta).        elif
+00011b10: 2063 6f6e 7465 6e74 5f74 7970 6520 3d3d   content_type ==
+00011b20: 2027 6170 706c 6963 6174 696f 6e2f 6f63   'application/oc
+00011b30: 7465 742d 7374 7265 616d 273a 0a20 2020  tet-stream':.   
+00011b40: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011b50: 7365 6c66 2e5f 5f73 6572 6961 6c69 7a65  self.__serialize
+00011b60: 5f61 7070 6c69 6361 7469 6f6e 5f6f 6374  _application_oct
+00011b70: 6574 5f73 7472 6561 6d28 6361 7374 5f69  et_stream(cast_i
+00011b80: 6e5f 6461 7461 290a 2020 2020 2020 2020  n_data).        
+00011b90: 7261 6973 6520 4e6f 7449 6d70 6c65 6d65  raise NotImpleme
+00011ba0: 6e74 6564 4572 726f 7228 2753 6572 6961  ntedError('Seria
+00011bb0: 6c69 7a61 7469 6f6e 2068 6173 206e 6f74  lization has not
+00011bc0: 2079 6574 2062 6565 6e20 696d 706c 656d   yet been implem
+00011bd0: 656e 7465 6420 666f 7220 7b7d 272e 666f  ented for {}'.fo
+00011be0: 726d 6174 2863 6f6e 7465 6e74 5f74 7970  rmat(content_typ
+00011bf0: 6529 290a                                e)).
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/path_to_api.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/apis/tags/kyc_api.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/apis/tags/kyc_api.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/client.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/client_custom.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,25 @@
     KYC & Onboarding
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
+import typing
+
 from decentro_in_kyc_client.configuration import Configuration
 from decentro_in_kyc_client.api_client import ApiClient
-from decentro_in_kyc_client.apis.tags.kyc_api import KYCApi
 
 
-class Decentro:
 
-    def __init__(self, configuration: Configuration = None, **kwargs):
+class ClientCustom:
+
+    def __init__(self, configuration: typing.Union[Configuration, None] = None, **kwargs):
         if (len(kwargs) > 0):
             configuration = Configuration(**kwargs)
         if (configuration is None):
             raise Exception("configuration is required")
         api_client = ApiClient(configuration)
-        self.kyc = KYCApi(api_client)
+        # customize here
+
+    # add custom methods here
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/configuration.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 4.3.0".\
+               "SDK Package Version: 4.4.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
@@ -506,17 +506,17 @@
     def host(self, value):
         """Fix base path."""
         self._base_path = check_url(value)
         self.server_index = None
         
 def check_url(url: str):
     parsed = urlparse(url)
-    if parsed.query is not '':
+    if parsed.query != '':
         raise InvalidHostConfigurationError(url, "query string is not allowed")
-    if parsed.fragment is not '':
+    if parsed.fragment != '':
         raise InvalidHostConfigurationError(url, "fragment is not allowed")
     if parsed.scheme not in ["http", "https"]:
         raise InvalidHostConfigurationError(url, 'scheme must be "http" or "https"'.format(parsed.scheme))
     if not validators.url(url):
         raise InvalidHostConfigurationError(url, "invalid url")
     if (url.endswith("/")):
         return url[:-1]
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
 
 import typing
-from decentro_in_kyc_client.api_response import ApiResponse
+from decentro_in_kyc_client.api_response import ApiResponse, AsyncApiResponse
 from decentro_in_kyc_client.exceptions_base import OpenApiException, ApiTypeError, ApiValueError, render_path
 
 class ClientConfigurationError(OpenApiException):
     def __init__(self, msg):
         super(ClientConfigurationError, self).__init__(msg)
 
 
@@ -54,20 +54,20 @@
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
 
-    def __init__(self, status=None, reason=None, api_response: ApiResponse = None):
+    def __init__(self, status=None, reason=None, api_response: typing.Optional[typing.Union[ApiResponse, AsyncApiResponse]] = None):
         if api_response:
             self.status = api_response.status
             self.reason = api_response.response.reason
             self.body = api_response.body
-            self.headers = api_response.response.getheaders()
+            self.headers = api_response.response.headers
             self.round_trip_time = api_response.round_trip_time
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
             self.round_trip_time = None
@@ -82,22 +82,45 @@
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
+class AnyOfValidationError(OpenApiException):
+    def __init__(self, error_list: typing.List[typing.Union[ApiTypeError, ApiValueError]]):
+        self.error_list = error_list
+        sub_msgs: typing.List[str] = []
+        for type_error in error_list:
+            sub_msgs.append(str(type_error))
+        num_validation_errors = len(self.error_list)
+        if num_validation_errors == 1:
+            super().__init__(sub_msgs[0])
+        else:
+            # create a string that says how many validation errors there were and
+            # prints each sub_msg out using a bulleted list of messages
+            msg = "{} validation error{} detected: \n".format(num_validation_errors, "s" if num_validation_errors > 1 else "")
+            for i, sub_msg in enumerate(sub_msgs):
+                msg += " {}. {}\n".format(i+1, sub_msg)
+            super().__init__(msg)
+
+
 class InvalidHostConfigurationError(ClientConfigurationError):
     def __init__(self, host: str, reason: str):
         self.host = host
         self.reason = reason
         super().__init__('Invalid host: "{}", {}'.format(self.host, self.reason))
 
 
-class MissingRequiredParametersError(TypeError):
+class MissingRequiredPropertiesError(ApiTypeError):
+    def __init__(self, msg: str):
+        super().__init__(msg)
+
+
+class MissingRequiredParametersError(ApiTypeError):
     def __init__(self, error: TypeError):
         self.error = error
         error_str = str(error)
         self.msg = error_str
         if "__new__()" in error_str:
             # parse error to reformat
             missing_parameters = error_str.split(":")[1].strip()
@@ -123,20 +146,26 @@
                              True if it is a key in a dict
                              False if our item is an item in a list
                              None if unset
         """
         self.validation_errors = validation_errors
         self.type_errors: typing.List[ApiTypeError] = []
         self.value_errors: typing.List[ApiValueError] = []
+        self.missing_required_properties_errors: typing.List[MissingRequiredPropertiesError] = []
         for error in validation_errors:
             if isinstance(error, ApiTypeError):
                 self.type_errors.append(error)
             elif isinstance(error, ApiValueError):
                 self.value_errors.append(error)
+            elif isinstance(error, MissingRequiredPropertiesError):
+                self.missing_required_properties_errors.append(error)
         sub_msgs: typing.List[str] = []
+        if len(self.missing_required_properties_errors) > 0:
+            for error in self.missing_required_properties_errors:
+                sub_msgs.append(str(error))
         if len(self.type_errors) > 0:
             for type_error in self.type_errors:
                 classes = ", ".join([cls.__name__ for cls in type_error.valid_classes])
                 msg = 'Got {}({}) for required type {} at {}'.format(
                     type(type_error.invalid_value).__name__, type_error.invalid_value, classes, render_path(type_error.path_to_item))
                 sub_msgs.append(msg)
         if len(self.value_errors) > 0:
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/exceptions_base.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_image_quality_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_image_quality_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_photocopy_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_photocopy_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/check_video_liveness_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/check_video_liveness_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/classify_document_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/classify_document_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/extract_text_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/extract_text_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_uid400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/mask_aadhaar_uid_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/match_face_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/match_face_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate400_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate_request.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/model/validate_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/model/validate_response.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/models/__init__.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/__init__.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_public_registry_validate/post.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,36 +12,41 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from decentro_in_kyc_client.api_response import AsyncGeneratorResponse
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
-from decentro_in_kyc_client.model.validate_response import ValidateResponse
-from decentro_in_kyc_client.model.validate400_response import Validate400Response
-from decentro_in_kyc_client.model.validate_request import ValidateRequest
+from decentro_in_kyc_client.model.validate_response import ValidateResponse as ValidateResponseSchema
+from decentro_in_kyc_client.model.validate400_response import Validate400Response as Validate400ResponseSchema
+from decentro_in_kyc_client.model.validate_request import ValidateRequest as ValidateRequestSchema
+
+from decentro_in_kyc_client.type.validate400_response import Validate400Response
+from decentro_in_kyc_client.type.validate_request import ValidateRequest
+from decentro_in_kyc_client.type.validate_response import ValidateResponse
 
 from . import path
 
 # body param
-SchemaForRequestBodyApplicationJson = ValidateRequest
+SchemaForRequestBodyApplicationJson = ValidateRequestSchema
 
 
 request_body_validate_request = api_client.RequestBody(
     content={
         'application/json': api_client.MediaType(
             schema=SchemaForRequestBodyApplicationJson),
     },
@@ -198,15 +203,15 @@
 )
 KongRequestIDSchema = schemas.StrSchema
 kong_request_id_parameter = api_client.HeaderParameter(
     name="Kong-Request-ID",
     style=api_client.ParameterStyle.SIMPLE,
     schema=KongRequestIDSchema,
 )
-SchemaFor200ResponseBodyApplicationJson = ValidateResponse
+SchemaFor200ResponseBodyApplicationJson = ValidateResponseSchema
 ResponseHeadersFor200 = typing_extensions.TypedDict(
     'ResponseHeadersFor200',
     {
         'Content-Length': ContentLengthSchema,
         'Connection': ConnectionSchema,
         'Date': DateSchema,
         'Server': ServerSchema,
@@ -233,21 +238,25 @@
         'Kong-Request-ID': KongRequestIDSchema,
     }
 )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
+    body: ValidateResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: ValidateResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
     headers=[
         content_length_parameter,
         connection_parameter,
@@ -272,26 +281,30 @@
         rate_limit_reset_parameter,
         x_rate_limit_remaining_minute_parameter,
         x_rate_limit_remaining_second_parameter,
         rate_limit_limit_parameter,
         kong_request_id_parameter,
     ]
 )
-SchemaFor400ResponseBodyApplicationJson = Validate400Response
+SchemaFor400ResponseBodyApplicationJson = Validate400ResponseSchema
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: Validate400Response
+
+
+@dataclass
+class ApiResponseFor400Async(api_client.AsyncApiResponse):
+    body: Validate400Response
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    response_cls_async=ApiResponseFor400Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
@@ -299,277 +312,331 @@
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _validate_oapg(
+
+    def _validate_mapped_args(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"] = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        body: typing.Optional[ValidateRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        id_number: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        dob: typing.Optional[str] = None,
+        name: typing.Optional[str] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        query_params = {}
+        header_params = {}
+        path_params = {}
+        cookie_params = {}
+        _body = {}
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
+        if document_type is not None:
+            _body["document_type"] = document_type
+        if id_number is not None:
+            _body["id_number"] = id_number
+        if dob is not None:
+            _body["dob"] = dob
+        if consent is not None:
+            _body["consent"] = consent
+        if consent_purpose is not None:
+            _body["consent_purpose"] = consent_purpose
+        if name is not None:
+            _body["name"] = name
+        args.body = body if body is not None else _body
+        args.query = query_params
+        args.header = header_params
+        args.path = path_params
+        args.cookie = cookie_params
+        return args
 
-    @typing.overload
-    def _validate_oapg(
+    async def _avalidate_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        Validate
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+    
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_validate_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
     def _validate_oapg(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _validate_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'application/json',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _validate_oapg(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json',
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
         Validate
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
-
+    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
         if body is schemas.unset:
             raise exceptions.ApiValueError(
                 'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
         serialized_data = request_body_validate_request.serialize(body, content_type)
         _headers.add('Content-Type', content_type)
         if 'fields' in serialized_data:
             _fields = serialized_data['fields']
         elif 'body' in serialized_data:
-            _body = serialized_data['body']
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
 class Validate(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def validate(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"] = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def validate(
+    async def avalidate(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[ValidateRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        id_number: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        dob: typing.Optional[str] = None,
+        name: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def validate(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._validate_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            document_type=document_type,
+            id_number=id_number,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            dob=dob,
+            name=name,
+        )
+        return await self._avalidate_oapg(
+            body=args.body,
+        )
+    
     def validate(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[ValidateRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        id_number: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        dob: typing.Optional[str] = None,
+        name: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def validate(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json',
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._validate_oapg(
+    ]:
+        args = self._validate_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            document_type=document_type,
+            id_number=id_number,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            dob=dob,
+            name=name,
+        )
+        return self._validate_oapg(
+            body=args.body,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: typing_extensions.Literal["application/json"] = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[ValidateRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        id_number: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        dob: typing.Optional[str] = None,
+        name: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._validate_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            document_type=document_type,
+            id_number=id_number,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            dob=dob,
+            name=name,
+        )
+        return await self._avalidate_oapg(
+            body=args.body,
+        )
+    
     def post(
         self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = ...,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[ValidateRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        id_number: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        dob: typing.Optional[str] = None,
+        name: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        body: typing.Union[SchemaForRequestBodyApplicationJson,],
-        content_type: str = 'application/json',
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._validate_oapg(
+    ]:
+        args = self._validate_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            document_type=document_type,
+            id_number=id_number,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            dob=dob,
+            name=name,
+        )
+        return self._validate_oapg(
+            body=args.body,
         )
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,197 +12,92 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from decentro_in_kyc_client.api_response import AsyncGeneratorResponse
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
-from decentro_in_kyc_client.model.extract_text400_response import ExtractText400Response
-from decentro_in_kyc_client.model.extract_text_response import ExtractTextResponse
-from decentro_in_kyc_client.model.extract_text_request import ExtractTextRequest
+from decentro_in_kyc_client.model.mask_aadhaar_request import MaskAadhaarRequest as MaskAadhaarRequestSchema
+from decentro_in_kyc_client.model.mask_aadhaar_uid_response import MaskAadhaarUidResponse as MaskAadhaarUidResponseSchema
+from decentro_in_kyc_client.model.mask_aadhaar_uid400_response import MaskAadhaarUid400Response as MaskAadhaarUid400ResponseSchema
+
+from decentro_in_kyc_client.type.mask_aadhaar_uid400_response import MaskAadhaarUid400Response
+from decentro_in_kyc_client.type.mask_aadhaar_request import MaskAadhaarRequest
+from decentro_in_kyc_client.type.mask_aadhaar_uid_response import MaskAadhaarUidResponse
 
 from . import path
 
 # body param
-SchemaForRequestBodyMultipartFormData = ExtractTextRequest
+SchemaForRequestBodyMultipartFormData = MaskAadhaarRequestSchema
 
 
-request_body_body = api_client.RequestBody(
+request_body_mask_aadhaar_request = api_client.RequestBody(
     content={
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
+    required=True,
 )
 _auth = [
     'client_id',
     'client_secret',
     'module_secret',
 ]
-ContentLengthSchema = schemas.IntSchema
-content_length_parameter = api_client.HeaderParameter(
-    name="Content-Length",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ContentLengthSchema,
-)
-ConnectionSchema = schemas.StrSchema
-connection_parameter = api_client.HeaderParameter(
-    name="Connection",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ConnectionSchema,
-)
-DateSchema = schemas.StrSchema
-date_parameter = api_client.HeaderParameter(
-    name="Date",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=DateSchema,
-)
-XDECENTROURNSchema = schemas.StrSchema
-x_decentro_urn_parameter = api_client.HeaderParameter(
-    name="X-DECENTRO-URN",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XDECENTROURNSchema,
-)
-ExpectCTSchema = schemas.StrSchema
-expect_ct_parameter = api_client.HeaderParameter(
-    name="Expect-CT",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ExpectCTSchema,
-)
-XPermittedCrossDomainPoliciesSchema = schemas.StrSchema
-x_permitted_cross_domain_policies_parameter = api_client.HeaderParameter(
-    name="X-Permitted-Cross-Domain-Policies",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XPermittedCrossDomainPoliciesSchema,
-)
-XFrameOptionsSchema = schemas.StrSchema
-x_frame_options_parameter = api_client.HeaderParameter(
-    name="X-Frame-Options",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XFrameOptionsSchema,
-)
-XXSSProtectionSchema = schemas.StrSchema
-x_xss_protection_parameter = api_client.HeaderParameter(
-    name="X-XSS-Protection",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XXSSProtectionSchema,
-)
-XContentTypeOptionsSchema = schemas.StrSchema
-x_content_type_options_parameter = api_client.HeaderParameter(
-    name="X-Content-Type-Options",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XContentTypeOptionsSchema,
-)
-ContentSecurityPolicySchema = schemas.StrSchema
-content_security_policy_parameter = api_client.HeaderParameter(
-    name="Content-Security-Policy",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ContentSecurityPolicySchema,
-)
-XContentSecurityPolicySchema = schemas.StrSchema
-x_content_security_policy_parameter = api_client.HeaderParameter(
-    name="X-Content-Security-Policy",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XContentSecurityPolicySchema,
-)
-StrictTransportSecuritySchema = schemas.StrSchema
-strict_transport_security_parameter = api_client.HeaderParameter(
-    name="Strict-Transport-Security",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=StrictTransportSecuritySchema,
-)
-ReferrerPolicySchema = schemas.StrSchema
-referrer_policy_parameter = api_client.HeaderParameter(
-    name="Referrer-Policy",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ReferrerPolicySchema,
-)
-VarySchema = schemas.StrSchema
-vary_parameter = api_client.HeaderParameter(
-    name="vary",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=VarySchema,
-)
-SchemaFor200ResponseBodyApplicationJson = ExtractTextResponse
-ResponseHeadersFor200 = typing_extensions.TypedDict(
-    'ResponseHeadersFor200',
-    {
-        'Content-Length': ContentLengthSchema,
-        'Connection': ConnectionSchema,
-        'Date': DateSchema,
-        'X-DECENTRO-URN': XDECENTROURNSchema,
-        'Expect-CT': ExpectCTSchema,
-        'X-Permitted-Cross-Domain-Policies': XPermittedCrossDomainPoliciesSchema,
-        'X-Frame-Options': XFrameOptionsSchema,
-        'X-XSS-Protection': XXSSProtectionSchema,
-        'X-Content-Type-Options': XContentTypeOptionsSchema,
-        'Content-Security-Policy': ContentSecurityPolicySchema,
-        'X-Content-Security-Policy': XContentSecurityPolicySchema,
-        'Strict-Transport-Security': StrictTransportSecuritySchema,
-        'Referrer-Policy': ReferrerPolicySchema,
-        'vary': VarySchema,
-    }
-)
+SchemaFor200ResponseBodyApplicationJson = MaskAadhaarUidResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
+    body: MaskAadhaarUidResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: MaskAadhaarUidResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
-    headers=[
-        content_length_parameter,
-        connection_parameter,
-        date_parameter,
-        x_decentro_urn_parameter,
-        expect_ct_parameter,
-        x_permitted_cross_domain_policies_parameter,
-        x_frame_options_parameter,
-        x_xss_protection_parameter,
-        x_content_type_options_parameter,
-        content_security_policy_parameter,
-        x_content_security_policy_parameter,
-        strict_transport_security_parameter,
-        referrer_policy_parameter,
-        vary_parameter,
-    ]
 )
-SchemaFor400ResponseBodyApplicationJson = ExtractText400Response
+SchemaFor400ResponseBodyApplicationJson = MaskAadhaarUid400ResponseSchema
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: MaskAadhaarUid400Response
+
+
+@dataclass
+class ApiResponseFor400Async(api_client.AsyncApiResponse):
+    body: MaskAadhaarUid400Response
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    response_cls_async=ApiResponseFor400Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
@@ -210,275 +105,309 @@
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _extract_text_oapg(
+
+    def _mask_aadhaar_uid_mapped_args(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        query_params = {}
+        header_params = {}
+        path_params = {}
+        cookie_params = {}
+        _body = {}
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
+        if consent is not None:
+            _body["consent"] = consent
+        if consent_purpose is not None:
+            _body["consent_purpose"] = consent_purpose
+        if image is not None:
+            _body["image"] = image
+        if image_url is not None:
+            _body["image_url"] = image_url
+        args.body = body if body is not None else _body
+        args.query = query_params
+        args.header = header_params
+        args.path = path_params
+        args.cookie = cookie_params
+        return args
 
-    @typing.overload
-    def _extract_text_oapg(
+    async def _amask_aadhaar_uid_oapg(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        Aadhaar Masking
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+    
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_mask_aadhaar_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _extract_text_oapg(
+    def _mask_aadhaar_uid_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _extract_text_oapg(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _extract_text_oapg(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
-        Scan &amp; Extract
+        Aadhaar Masking
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
-
+    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_mask_aadhaar_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class ExtractText(BaseApi):
+class MaskAadhaarUid(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def extract_text(
+    async def amask_aadhaar_uid(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def extract_text(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def extract_text(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def extract_text(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return await self._amask_aadhaar_uid_oapg(
+            body=args.body,
+        )
+    
+    def mask_aadhaar_uid(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def extract_text(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._extract_text_oapg(
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return self._mask_aadhaar_uid_oapg(
+            body=args.body,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
-        self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return await self._amask_aadhaar_uid_oapg(
+            body=args.body,
+        )
+    
     def post(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._extract_text_oapg(
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return self._mask_aadhaar_uid_oapg(
+            body=args.body,
         )
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_face_match/post.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,43 +12,49 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from decentro_in_kyc_client.api_response import AsyncGeneratorResponse
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
-from decentro_in_kyc_client.model.match_face_response import MatchFaceResponse
-from decentro_in_kyc_client.model.match_face400_response import MatchFace400Response
-from decentro_in_kyc_client.model.match_face_request import MatchFaceRequest
+from decentro_in_kyc_client.model.check_photocopy_response import CheckPhotocopyResponse as CheckPhotocopyResponseSchema
+from decentro_in_kyc_client.model.check_photocopy400_response import CheckPhotocopy400Response as CheckPhotocopy400ResponseSchema
+from decentro_in_kyc_client.model.check_photocopy_request import CheckPhotocopyRequest as CheckPhotocopyRequestSchema
+
+from decentro_in_kyc_client.type.check_photocopy400_response import CheckPhotocopy400Response
+from decentro_in_kyc_client.type.check_photocopy_request import CheckPhotocopyRequest
+from decentro_in_kyc_client.type.check_photocopy_response import CheckPhotocopyResponse
 
 from . import path
 
 # body param
-SchemaForRequestBodyMultipartFormData = MatchFaceRequest
+SchemaForRequestBodyMultipartFormData = CheckPhotocopyRequestSchema
 
 
-request_body_body = api_client.RequestBody(
+request_body_check_photocopy_request = api_client.RequestBody(
     content={
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
+    required=True,
 )
 _auth = [
     'client_id',
     'client_secret',
     'module_secret',
 ]
 ContentLengthSchema = schemas.IntSchema
@@ -131,15 +137,15 @@
 )
 VarySchema = schemas.StrSchema
 vary_parameter = api_client.HeaderParameter(
     name="vary",
     style=api_client.ParameterStyle.SIMPLE,
     schema=VarySchema,
 )
-SchemaFor200ResponseBodyApplicationJson = MatchFaceResponse
+SchemaFor200ResponseBodyApplicationJson = CheckPhotocopyResponseSchema
 ResponseHeadersFor200 = typing_extensions.TypedDict(
     'ResponseHeadersFor200',
     {
         'Content-Length': ContentLengthSchema,
         'Connection': ConnectionSchema,
         'Date': DateSchema,
         'X-DECENTRO-URN': XDECENTROURNSchema,
@@ -155,21 +161,25 @@
         'vary': VarySchema,
     }
 )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
+    body: CheckPhotocopyResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: CheckPhotocopyResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
     headers=[
         content_length_parameter,
         connection_parameter,
@@ -183,26 +193,30 @@
         content_security_policy_parameter,
         x_content_security_policy_parameter,
         strict_transport_security_parameter,
         referrer_policy_parameter,
         vary_parameter,
     ]
 )
-SchemaFor400ResponseBodyApplicationJson = MatchFace400Response
+SchemaFor400ResponseBodyApplicationJson = CheckPhotocopy400ResponseSchema
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: CheckPhotocopy400Response
+
+
+@dataclass
+class ApiResponseFor400Async(api_client.AsyncApiResponse):
+    body: CheckPhotocopy400Response
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    response_cls_async=ApiResponseFor400Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
@@ -210,275 +224,309 @@
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _match_face_oapg(
+
+    def _check_photocopy_mapped_args(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        body: typing.Optional[CheckPhotocopyRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        query_params = {}
+        header_params = {}
+        path_params = {}
+        cookie_params = {}
+        _body = {}
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
+        if consent is not None:
+            _body["consent"] = consent
+        if consent_purpose is not None:
+            _body["consent_purpose"] = consent_purpose
+        if image is not None:
+            _body["image"] = image
+        if image_url is not None:
+            _body["image_url"] = image_url
+        args.body = body if body is not None else _body
+        args.query = query_params
+        args.header = header_params
+        args.path = path_params
+        args.cookie = cookie_params
+        return args
 
-    @typing.overload
-    def _match_face_oapg(
+    async def _acheck_photocopy_oapg(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        Photocopy Check
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+    
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_check_photocopy_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _match_face_oapg(
+    def _check_photocopy_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _match_face_oapg(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _match_face_oapg(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
-        Face Match
+        Photocopy Check
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
-
+    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_check_photocopy_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class MatchFace(BaseApi):
+class CheckPhotocopy(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def match_face(
+    async def acheck_photocopy(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[CheckPhotocopyRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def match_face(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def match_face(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def match_face(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._check_photocopy_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return await self._acheck_photocopy_oapg(
+            body=args.body,
+        )
+    
+    def check_photocopy(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[CheckPhotocopyRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def match_face(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._match_face_oapg(
+    ]:
+        args = self._check_photocopy_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return self._check_photocopy_oapg(
+            body=args.body,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[CheckPhotocopyRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._check_photocopy_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return await self._acheck_photocopy_oapg(
+            body=args.body,
+        )
+    
     def post(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[CheckPhotocopyRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._match_face_oapg(
+    ]:
+        args = self._check_photocopy_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return self._check_photocopy_oapg(
+            body=args.body,
         )
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_image_quality/post.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/kyc_scan_extract_ocr/post.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,43 +12,49 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from decentro_in_kyc_client.api_response import AsyncGeneratorResponse
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
-from decentro_in_kyc_client.model.check_image_quality_request import CheckImageQualityRequest
-from decentro_in_kyc_client.model.check_image_quality400_response import CheckImageQuality400Response
-from decentro_in_kyc_client.model.check_image_quality_response import CheckImageQualityResponse
+from decentro_in_kyc_client.model.extract_text400_response import ExtractText400Response as ExtractText400ResponseSchema
+from decentro_in_kyc_client.model.extract_text_request import ExtractTextRequest as ExtractTextRequestSchema
+from decentro_in_kyc_client.model.extract_text_response import ExtractTextResponse as ExtractTextResponseSchema
+
+from decentro_in_kyc_client.type.extract_text400_response import ExtractText400Response
+from decentro_in_kyc_client.type.extract_text_response import ExtractTextResponse
+from decentro_in_kyc_client.type.extract_text_request import ExtractTextRequest
 
 from . import path
 
 # body param
-SchemaForRequestBodyMultipartFormData = CheckImageQualityRequest
+SchemaForRequestBodyMultipartFormData = ExtractTextRequestSchema
 
 
-request_body_body = api_client.RequestBody(
+request_body_extract_text_request = api_client.RequestBody(
     content={
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
+    required=True,
 )
 _auth = [
     'client_id',
     'client_secret',
     'module_secret',
 ]
 ContentLengthSchema = schemas.IntSchema
@@ -131,15 +137,15 @@
 )
 VarySchema = schemas.StrSchema
 vary_parameter = api_client.HeaderParameter(
     name="vary",
     style=api_client.ParameterStyle.SIMPLE,
     schema=VarySchema,
 )
-SchemaFor200ResponseBodyApplicationJson = CheckImageQualityResponse
+SchemaFor200ResponseBodyApplicationJson = ExtractTextResponseSchema
 ResponseHeadersFor200 = typing_extensions.TypedDict(
     'ResponseHeadersFor200',
     {
         'Content-Length': ContentLengthSchema,
         'Connection': ConnectionSchema,
         'Date': DateSchema,
         'X-DECENTRO-URN': XDECENTROURNSchema,
@@ -155,21 +161,25 @@
         'vary': VarySchema,
     }
 )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
+    body: ExtractTextResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: ExtractTextResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
     headers=[
         content_length_parameter,
         connection_parameter,
@@ -183,421 +193,384 @@
         content_security_policy_parameter,
         x_content_security_policy_parameter,
         strict_transport_security_parameter,
         referrer_policy_parameter,
         vary_parameter,
     ]
 )
-ContentLengthSchema = schemas.IntSchema
-content_length_parameter = api_client.HeaderParameter(
-    name="Content-Length",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ContentLengthSchema,
-)
-ConnectionSchema = schemas.StrSchema
-connection_parameter = api_client.HeaderParameter(
-    name="Connection",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ConnectionSchema,
-)
-DateSchema = schemas.StrSchema
-date_parameter = api_client.HeaderParameter(
-    name="Date",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=DateSchema,
-)
-XDECENTROURNSchema = schemas.StrSchema
-x_decentro_urn_parameter = api_client.HeaderParameter(
-    name="X-DECENTRO-URN",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XDECENTROURNSchema,
-)
-ExpectCTSchema = schemas.StrSchema
-expect_ct_parameter = api_client.HeaderParameter(
-    name="Expect-CT",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ExpectCTSchema,
-)
-XPermittedCrossDomainPoliciesSchema = schemas.StrSchema
-x_permitted_cross_domain_policies_parameter = api_client.HeaderParameter(
-    name="X-Permitted-Cross-Domain-Policies",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XPermittedCrossDomainPoliciesSchema,
-)
-XFrameOptionsSchema = schemas.StrSchema
-x_frame_options_parameter = api_client.HeaderParameter(
-    name="X-Frame-Options",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XFrameOptionsSchema,
-)
-XXSSProtectionSchema = schemas.StrSchema
-x_xss_protection_parameter = api_client.HeaderParameter(
-    name="X-XSS-Protection",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XXSSProtectionSchema,
-)
-XContentTypeOptionsSchema = schemas.StrSchema
-x_content_type_options_parameter = api_client.HeaderParameter(
-    name="X-Content-Type-Options",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XContentTypeOptionsSchema,
-)
-ContentSecurityPolicySchema = schemas.StrSchema
-content_security_policy_parameter = api_client.HeaderParameter(
-    name="Content-Security-Policy",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ContentSecurityPolicySchema,
-)
-XContentSecurityPolicySchema = schemas.StrSchema
-x_content_security_policy_parameter = api_client.HeaderParameter(
-    name="X-Content-Security-Policy",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=XContentSecurityPolicySchema,
-)
-StrictTransportSecuritySchema = schemas.StrSchema
-strict_transport_security_parameter = api_client.HeaderParameter(
-    name="Strict-Transport-Security",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=StrictTransportSecuritySchema,
-)
-ReferrerPolicySchema = schemas.StrSchema
-referrer_policy_parameter = api_client.HeaderParameter(
-    name="Referrer-Policy",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=ReferrerPolicySchema,
-)
-VarySchema = schemas.StrSchema
-vary_parameter = api_client.HeaderParameter(
-    name="vary",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=VarySchema,
-)
-SchemaFor400ResponseBodyApplicationJson = CheckImageQuality400Response
-ResponseHeadersFor400 = typing_extensions.TypedDict(
-    'ResponseHeadersFor400',
-    {
-        'Content-Length': ContentLengthSchema,
-        'Connection': ConnectionSchema,
-        'Date': DateSchema,
-        'X-DECENTRO-URN': XDECENTROURNSchema,
-        'Expect-CT': ExpectCTSchema,
-        'X-Permitted-Cross-Domain-Policies': XPermittedCrossDomainPoliciesSchema,
-        'X-Frame-Options': XFrameOptionsSchema,
-        'X-XSS-Protection': XXSSProtectionSchema,
-        'X-Content-Type-Options': XContentTypeOptionsSchema,
-        'Content-Security-Policy': ContentSecurityPolicySchema,
-        'X-Content-Security-Policy': XContentSecurityPolicySchema,
-        'Strict-Transport-Security': StrictTransportSecuritySchema,
-        'Referrer-Policy': ReferrerPolicySchema,
-        'vary': VarySchema,
-    }
-)
+SchemaFor400ResponseBodyApplicationJson = ExtractText400ResponseSchema
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: ExtractText400Response
+
+
+@dataclass
+class ApiResponseFor400Async(api_client.AsyncApiResponse):
+    body: ExtractText400Response
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    response_cls_async=ApiResponseFor400Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
-    headers=[
-        content_length_parameter,
-        connection_parameter,
-        date_parameter,
-        x_decentro_urn_parameter,
-        expect_ct_parameter,
-        x_permitted_cross_domain_policies_parameter,
-        x_frame_options_parameter,
-        x_xss_protection_parameter,
-        x_content_type_options_parameter,
-        content_security_policy_parameter,
-        x_content_security_policy_parameter,
-        strict_transport_security_parameter,
-        referrer_policy_parameter,
-        vary_parameter,
-    ]
 )
 _status_code_to_response = {
     '200': _response_for_200,
     '400': _response_for_400,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _check_image_quality_oapg(
+
+    def _extract_text_mapped_args(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        body: typing.Optional[ExtractTextRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        kyc_validate: typing.Optional[int] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
+        document_back: typing.Optional[typing.IO] = None,
+        document_back_url: typing.Optional[str] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        query_params = {}
+        header_params = {}
+        path_params = {}
+        cookie_params = {}
+        _body = {}
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
+        if document_type is not None:
+            _body["document_type"] = document_type
+        if consent is not None:
+            _body["consent"] = consent
+        if consent_purpose is not None:
+            _body["consent_purpose"] = consent_purpose
+        if kyc_validate is not None:
+            _body["kyc_validate"] = kyc_validate
+        if document is not None:
+            _body["document"] = document
+        if document_url is not None:
+            _body["document_url"] = document_url
+        if document_back is not None:
+            _body["document_back"] = document_back
+        if document_back_url is not None:
+            _body["document_back_url"] = document_back_url
+        args.body = body if body is not None else _body
+        args.query = query_params
+        args.header = header_params
+        args.path = path_params
+        args.cookie = cookie_params
+        return args
 
-    @typing.overload
-    def _check_image_quality_oapg(
+    async def _aextract_text_oapg(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        Scan &amp; Extract
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+    
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_extract_text_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _check_image_quality_oapg(
+    def _extract_text_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _check_image_quality_oapg(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _check_image_quality_oapg(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
-        Image Quality Check
+        Scan &amp; Extract
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
-
+    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_extract_text_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class CheckImageQuality(BaseApi):
+class ExtractText(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def check_image_quality(
+    async def aextract_text(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[ExtractTextRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        kyc_validate: typing.Optional[int] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
+        document_back: typing.Optional[typing.IO] = None,
+        document_back_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_image_quality(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def check_image_quality(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def check_image_quality(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._extract_text_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            kyc_validate=kyc_validate,
+            document=document,
+            document_url=document_url,
+            document_back=document_back,
+            document_back_url=document_back_url,
+        )
+        return await self._aextract_text_oapg(
+            body=args.body,
+        )
+    
+    def extract_text(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[ExtractTextRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        kyc_validate: typing.Optional[int] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
+        document_back: typing.Optional[typing.IO] = None,
+        document_back_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def check_image_quality(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_image_quality_oapg(
+    ]:
+        args = self._extract_text_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            kyc_validate=kyc_validate,
+            document=document,
+            document_url=document_url,
+            document_back=document_back,
+            document_back_url=document_back_url,
+        )
+        return self._extract_text_oapg(
+            body=args.body,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
-        self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[ExtractTextRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        kyc_validate: typing.Optional[int] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
+        document_back: typing.Optional[typing.IO] = None,
+        document_back_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._extract_text_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            kyc_validate=kyc_validate,
+            document=document,
+            document_url=document_url,
+            document_back=document_back,
+            document_back_url=document_back_url,
+        )
+        return await self._aextract_text_oapg(
+            body=args.body,
+        )
+    
     def post(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[ExtractTextRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[str] = None,
+        consent_purpose: typing.Optional[str] = None,
+        kyc_validate: typing.Optional[int] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
+        document_back: typing.Optional[typing.IO] = None,
+        document_back_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_image_quality_oapg(
+    ]:
+        args = self._extract_text_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            kyc_validate=kyc_validate,
+            document=document,
+            document_url=document_url,
+            document_back=document_back,
+            document_back_url=document_back_url,
+        )
+        return self._extract_text_oapg(
+            body=args.body,
         )
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_photocopy_check/post.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_document_classification/post.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,43 +12,49 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from decentro_in_kyc_client.api_response import AsyncGeneratorResponse
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
-from decentro_in_kyc_client.model.check_photocopy_response import CheckPhotocopyResponse
-from decentro_in_kyc_client.model.check_photocopy400_response import CheckPhotocopy400Response
-from decentro_in_kyc_client.model.check_photocopy_request import CheckPhotocopyRequest
+from decentro_in_kyc_client.model.classify_document400_response import ClassifyDocument400Response as ClassifyDocument400ResponseSchema
+from decentro_in_kyc_client.model.classify_document_request import ClassifyDocumentRequest as ClassifyDocumentRequestSchema
+from decentro_in_kyc_client.model.classify_document_response import ClassifyDocumentResponse as ClassifyDocumentResponseSchema
+
+from decentro_in_kyc_client.type.classify_document400_response import ClassifyDocument400Response
+from decentro_in_kyc_client.type.classify_document_request import ClassifyDocumentRequest
+from decentro_in_kyc_client.type.classify_document_response import ClassifyDocumentResponse
 
 from . import path
 
 # body param
-SchemaForRequestBodyMultipartFormData = CheckPhotocopyRequest
+SchemaForRequestBodyMultipartFormData = ClassifyDocumentRequestSchema
 
 
-request_body_body = api_client.RequestBody(
+request_body_classify_document_request = api_client.RequestBody(
     content={
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
+    required=True,
 )
 _auth = [
     'client_id',
     'client_secret',
     'module_secret',
 ]
 ContentLengthSchema = schemas.IntSchema
@@ -131,15 +137,15 @@
 )
 VarySchema = schemas.StrSchema
 vary_parameter = api_client.HeaderParameter(
     name="vary",
     style=api_client.ParameterStyle.SIMPLE,
     schema=VarySchema,
 )
-SchemaFor200ResponseBodyApplicationJson = CheckPhotocopyResponse
+SchemaFor200ResponseBodyApplicationJson = ClassifyDocumentResponseSchema
 ResponseHeadersFor200 = typing_extensions.TypedDict(
     'ResponseHeadersFor200',
     {
         'Content-Length': ContentLengthSchema,
         'Connection': ConnectionSchema,
         'Date': DateSchema,
         'X-DECENTRO-URN': XDECENTROURNSchema,
@@ -155,21 +161,25 @@
         'vary': VarySchema,
     }
 )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
+    body: ClassifyDocumentResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: ClassifyDocumentResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
     headers=[
         content_length_parameter,
         connection_parameter,
@@ -183,26 +193,30 @@
         content_security_policy_parameter,
         x_content_security_policy_parameter,
         strict_transport_security_parameter,
         referrer_policy_parameter,
         vary_parameter,
     ]
 )
-SchemaFor400ResponseBodyApplicationJson = CheckPhotocopy400Response
+SchemaFor400ResponseBodyApplicationJson = ClassifyDocument400ResponseSchema
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: ClassifyDocument400Response
+
+
+@dataclass
+class ApiResponseFor400Async(api_client.AsyncApiResponse):
+    body: ClassifyDocument400Response
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    response_cls_async=ApiResponseFor400Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
@@ -210,275 +224,320 @@
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _check_photocopy_oapg(
+
+    def _classify_document_mapped_args(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        body: typing.Optional[ClassifyDocumentRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        query_params = {}
+        header_params = {}
+        path_params = {}
+        cookie_params = {}
+        _body = {}
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
+        if document_type is not None:
+            _body["document_type"] = document_type
+        if consent is not None:
+            _body["consent"] = consent
+        if consent_purpose is not None:
+            _body["consent_purpose"] = consent_purpose
+        if document is not None:
+            _body["document"] = document
+        if document_url is not None:
+            _body["document_url"] = document_url
+        args.body = body if body is not None else _body
+        args.query = query_params
+        args.header = header_params
+        args.path = path_params
+        args.cookie = cookie_params
+        return args
 
-    @typing.overload
-    def _check_photocopy_oapg(
+    async def _aclassify_document_oapg(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        ID Classification
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+    
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_classify_document_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _check_photocopy_oapg(
+    def _classify_document_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _check_photocopy_oapg(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _check_photocopy_oapg(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
-        Photocopy Check
+        ID Classification
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
-
+    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_classify_document_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class CheckPhotocopy(BaseApi):
+class ClassifyDocument(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def check_photocopy(
+    async def aclassify_document(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[ClassifyDocumentRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_photocopy(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def check_photocopy(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def check_photocopy(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._classify_document_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            document=document,
+            document_url=document_url,
+        )
+        return await self._aclassify_document_oapg(
+            body=args.body,
+        )
+    
+    def classify_document(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[ClassifyDocumentRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def check_photocopy(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_photocopy_oapg(
+    ]:
+        args = self._classify_document_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            document=document,
+            document_url=document_url,
+        )
+        return self._classify_document_oapg(
+            body=args.body,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[ClassifyDocumentRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._classify_document_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            document=document,
+            document_url=document_url,
+        )
+        return await self._aclassify_document_oapg(
+            body=args.body,
+        )
+    
     def post(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[ClassifyDocumentRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        document_type: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        document: typing.Optional[typing.IO] = None,
+        document_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_photocopy_oapg(
+    ]:
+        args = self._classify_document_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            document_type=document_type,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            document=document,
+            document_url=document_url,
+        )
+        return self._classify_document_oapg(
+            body=args.body,
         )
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/paths/v2_kyc_forensics_video_liveness/post.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/paths/v2_kyc_identities_mask_aadhaar_uid/post.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -12,354 +12,391 @@
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 import json
 from urllib3._collections import HTTPHeaderDict
 
+from decentro_in_kyc_client.api_response import AsyncGeneratorResponse
 from decentro_in_kyc_client import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from decentro_in_kyc_client import schemas  # noqa: F401
 
-from decentro_in_kyc_client.model.check_video_liveness400_response import CheckVideoLiveness400Response
-from decentro_in_kyc_client.model.check_video_liveness_response import CheckVideoLivenessResponse
-from decentro_in_kyc_client.model.check_video_liveness_request import CheckVideoLivenessRequest
-
-from . import path
+from decentro_in_kyc_client.model.mask_aadhaar_request import MaskAadhaarRequest as MaskAadhaarRequestSchema
+from decentro_in_kyc_client.model.mask_aadhaar_uid_response import MaskAadhaarUidResponse as MaskAadhaarUidResponseSchema
+from decentro_in_kyc_client.model.mask_aadhaar_uid400_response import MaskAadhaarUid400Response as MaskAadhaarUid400ResponseSchema
+
+from decentro_in_kyc_client.type.mask_aadhaar_uid400_response import MaskAadhaarUid400Response
+from decentro_in_kyc_client.type.mask_aadhaar_request import MaskAadhaarRequest
+from decentro_in_kyc_client.type.mask_aadhaar_uid_response import MaskAadhaarUidResponse
 
 # body param
-SchemaForRequestBodyMultipartFormData = CheckVideoLivenessRequest
+SchemaForRequestBodyMultipartFormData = MaskAadhaarRequestSchema
 
 
-request_body_body = api_client.RequestBody(
+request_body_mask_aadhaar_request = api_client.RequestBody(
     content={
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
+    required=True,
 )
-_auth = [
-    'client_id',
-    'client_secret',
-    'module_secret',
-]
-SchemaFor200ResponseBodyApplicationJson = CheckVideoLivenessResponse
+SchemaFor200ResponseBodyApplicationJson = MaskAadhaarUidResponseSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
-    ]
+    body: MaskAadhaarUidResponse
+
+
+@dataclass
+class ApiResponseFor200Async(api_client.AsyncApiResponse):
+    body: MaskAadhaarUidResponse
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
+    response_cls_async=ApiResponseFor200Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = CheckVideoLiveness400Response
+SchemaFor400ResponseBodyApplicationJson = MaskAadhaarUid400ResponseSchema
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
-    body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
-    ]
+    body: MaskAadhaarUid400Response
+
+
+@dataclass
+class ApiResponseFor400Async(api_client.AsyncApiResponse):
+    body: MaskAadhaarUid400Response
 
 
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
+    response_cls_async=ApiResponseFor400Async,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '400': _response_for_400,
-}
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
-    @typing.overload
-    def _check_video_liveness_oapg(
+
+    def _mask_aadhaar_uid_mapped_args(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
+    ) -> api_client.MappedArgs:
+        args: api_client.MappedArgs = api_client.MappedArgs()
+        query_params = {}
+        header_params = {}
+        path_params = {}
+        cookie_params = {}
+        _body = {}
+        if reference_id is not None:
+            _body["reference_id"] = reference_id
+        if consent is not None:
+            _body["consent"] = consent
+        if consent_purpose is not None:
+            _body["consent_purpose"] = consent_purpose
+        if image is not None:
+            _body["image"] = image
+        if image_url is not None:
+            _body["image_url"] = image_url
+        args.body = body if body is not None else _body
+        args.query = query_params
+        args.header = header_params
+        args.path = path_params
+        args.cookie = cookie_params
+        return args
 
-    @typing.overload
-    def _check_video_liveness_oapg(
+    async def _amask_aadhaar_uid_oapg(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        """
+        Aadhaar Masking
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        used_path = path.value
+    
+        _headers = HTTPHeaderDict()
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add('Accept', accept_content_type)
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
+        _fields = None
+        _body = None
+        serialized_data = request_body_mask_aadhaar_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
+        response = await self.api_client.async_call_api(
+            resource_path=used_path,
+            method='post'.upper(),
+            headers=_headers,
+            fields=_fields,
+            serialized_body=_body,
+            body=body,
+            auth_settings=_auth,
+            timeout=timeout,
+        )
+        
+        if stream:
+            async def stream_iterator():
+                """
+                iterates over response.http_response.content and closes connection once iteration has finished
+                """
+                async for line in response.http_response.content:
+                    if line == b'\r\n':
+                        continue
+                    yield line
+                response.http_response.close()
+                await response.session.close()
+            return AsyncGeneratorResponse(
+                content=stream_iterator(),
+                headers=response.http_response.headers,
+                status=response.http_response.status,
+                response=response.http_response
+            )
+    
+        response_for_status = _status_code_to_response.get(str(response.http_response.status))
+        if response_for_status:
+            api_response = await response_for_status.deserialize_async(
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
+        else:
+            # If response data is JSON then deserialize for SDK consumer convenience
+            is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
+            api_response = api_client.ApiResponseWithoutDeserializationAsync(
+                body=await response.http_response.json() if is_json else await response.http_response.text(),
+                response=response.http_response,
+                round_trip_time=response.round_trip_time,
+                status=response.http_response.status,
+                headers=response.http_response.headers,
+            )
+    
+        if not 200 <= api_response.status <= 299:
+            raise exceptions.ApiException(api_response=api_response)
+    
+        # cleanup session / response
+        response.http_response.close()
+        await response.session.close()
+    
+        return api_response
 
-    @typing.overload
-    def _check_video_liveness_oapg(
+    def _mask_aadhaar_uid_oapg(
         self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
+        body: typing.Any = None,
+        skip_deserialization: bool = True,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def _check_video_liveness_oapg(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        content_type: str = 'multipart/form-data',
         stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _check_video_liveness_oapg(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
+    ]:
         """
-        Liveness Check
+        Aadhaar Masking
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         used_path = path.value
-
+    
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
-
+    
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_mask_aadhaar_request.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']    
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             serialized_body=_body,
             body=body,
             auth_settings=_auth,
-            stream=stream,
             timeout=timeout,
         )
-
+    
         response_for_status = _status_code_to_response.get(str(response.http_response.status))
         if response_for_status:
             api_response = response_for_status.deserialize(
-                                                   response,
-                                                   self.api_client.configuration,
-                                                   skip_deserialization=skip_deserialization
-                                               )
+                                                    response,
+                                                    self.api_client.configuration,
+                                                    skip_deserialization=skip_deserialization
+                                                )
         else:
             # If response data is JSON then deserialize for SDK consumer convenience
             is_json = api_client.JSONDetector._content_type_is_json(response.http_response.headers.get('Content-Type', ''))
             api_response = api_client.ApiResponseWithoutDeserialization(
                 body=json.loads(response.http_response.data) if is_json else response.http_response.data,
                 response=response.http_response,
                 round_trip_time=response.round_trip_time,
                 status=response.http_response.status,
                 headers=response.http_response.headers,
             )
-
+    
         if not 200 <= api_response.status <= 299:
             raise exceptions.ApiException(api_response=api_response)
-
+    
         return api_response
 
-
-class CheckVideoLiveness(BaseApi):
+class MaskAadhaarUid(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
-    @typing.overload
-    def check_video_liveness(
+    async def amask_aadhaar_uid(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def check_video_liveness(
-        self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def check_video_liveness(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
-    def check_video_liveness(
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return await self._amask_aadhaar_uid_oapg(
+            body=args.body,
+        )
+    
+    def mask_aadhaar_uid(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def check_video_liveness(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_video_liveness_oapg(
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return self._mask_aadhaar_uid_oapg(
+            body=args.body,
         )
-
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
-    @typing.overload
-    def post(
-        self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
-    ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-    @typing.overload
-    def post(
+    async def apost(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: typing_extensions.Literal[False] = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
-
-    @typing.overload
-    def post(
-        self,
-        skip_deserialization: typing_extensions.Literal[True],
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
-
-    @typing.overload
+        ApiResponseFor200Async,
+        api_client.ApiResponseWithoutDeserializationAsync,
+        AsyncGeneratorResponse,
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
+            body=body,
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return await self._amask_aadhaar_uid_oapg(
+            body=args.body,
+        )
+    
     def post(
         self,
-        content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = ...,
+        body: typing.Optional[MaskAadhaarRequest] = None,
+        reference_id: typing.Optional[str] = None,
+        consent: typing.Optional[bool] = None,
+        consent_purpose: typing.Optional[str] = None,
+        image: typing.Optional[typing.IO] = None,
+        image_url: typing.Optional[str] = None,
     ) -> typing.Union[
         ApiResponseFor200,
         api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def post(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
-        stream: bool = False,
-        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-        skip_deserialization: bool = True,
-    ):
-        return self._check_video_liveness_oapg(
+    ]:
+        args = self._mask_aadhaar_uid_mapped_args(
             body=body,
-            content_type=content_type,
-            accept_content_types=accept_content_types,
-            stream=stream,
-            timeout=timeout,
-            skip_deserialization=skip_deserialization
+            reference_id=reference_id,
+            consent=consent,
+            consent_purpose=consent_purpose,
+            image=image,
+            image_url=image_url,
+        )
+        return self._mask_aadhaar_uid_oapg(
+            body=args.body,
         )
-
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_after_hook.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/request_before_hook.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/rest.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,37 @@
 """
 
 
 import logging
 import ssl
 from urllib.parse import urlencode
 import typing
+import aiohttp
 
 import certifi
 import urllib3
 import time
 from urllib3._collections import HTTPHeaderDict
 
 from decentro_in_kyc_client.exceptions import ApiException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 class ResponseWrapper:
-    def __init__(self, http_response: urllib3.HTTPResponse, round_trip_time: int):
+    def __init__(self, http_response: urllib3.HTTPResponse, round_trip_time: float):
         self.http_response = http_response
         self.round_trip_time = round_trip_time
 
+class AsyncResponseWrapper:
+    def __init__(self, http_response: aiohttp.ClientResponse, round_trip_time: float, session: aiohttp.ClientSession):
+        self.http_response = http_response
+        self.round_trip_time = round_trip_time
+        self.session = session
+
 class RESTClientObject(object):
 
     def __init__(self, configuration, pools_size=4, maxsize=None):
         # urllib3.PoolManager will pass all kw parameters to connectionpool
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/poolmanager.py#L75
         # https://github.com/shazow/urllib3/blob/f9409436f83aeb79fbaf090181cd81b784f1b8ce/urllib3/connectionpool.py#L680
         # maxsize is the number of requests to host that are allowed in parallel
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/schemas.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from datetime import date, datetime, timedelta  # noqa: F401
 import functools
 import decimal
 import io
 import re
 import types
 import typing
+import typing_extensions
 import uuid
 
 from dateutil.parser.isoparser import isoparser, _takes_ascii
 import frozendict
 
 from decentro_in_kyc_client.exceptions_base import (
     ApiTypeError,
@@ -29,15 +30,18 @@
 )
 from decentro_in_kyc_client.configuration import (
     Configuration,
 )
 from decentro_in_kyc_client.exceptions import SchemaValidationError
 from decentro_in_kyc_client.exceptions import render_path
 from decentro_in_kyc_client.validation_metadata import ValidationMetadata
+from decentro_in_kyc_client.exceptions import AnyOfValidationError
+from decentro_in_kyc_client.exceptions import MissingRequiredPropertiesError
 
+Primitive: typing_extensions.TypeAlias = typing.Union[int, float, bool, str]
 
 class Unset(object):
     """
     An instance of this class is set as the default value for object type(dict) properties that are optional
     When a property has an unset value, that property will not be assigned in the dict
     """
     pass
@@ -170,17 +174,17 @@
     class properties:
         # to hold object properties
         pass
 
     additional_properties: typing.Optional[typing.Type['Schema']]
     max_properties: int
     min_properties: int
-    all_of: typing.List[typing.Type['Schema']]
-    one_of: typing.List[typing.Type['Schema']]
-    any_of: typing.List[typing.Type['Schema']]
+    all_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    one_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
+    any_of: typing.Callable[[], typing.List[typing.Type['Schema']]]
     not_schema: typing.Type['Schema']
     max_length: int
     min_length: int
     items: typing.Type['Schema']
 
 
 class Schema:
@@ -447,35 +451,35 @@
             kwargs (str, int/float/decimal.Decimal/str/list/tuple/dict/frozendict.frozendict/bool/None): dict values
             _configuration: contains the Configuration that enables json schema validation keywords
                 like minItems, minLength etc
 
         Note: double underscores are used here because pycharm thinks that these variables
         are instance properties if they are named normally :(
         """
-        __kwargs = cls.__remove_unsets(kwargs)
-        if not args and not __kwargs:
+        _kwargs = cls.__remove_unsets(kwargs)
+        if not args and not _kwargs:
             raise TypeError(
                 'No input given. args or kwargs must be given.'
             )
-        if not __kwargs and args and not isinstance(args[0], dict):
-            __arg = args[0]
+        if not _kwargs and args and not isinstance(args[0], dict):
+            _arg = args[0]
         else:
-            __arg = cls.__get_input_dict(*args, **__kwargs)
-        __from_server = False
-        __validated_path_to_schemas = {}
-        __arg = cast_to_allowed_types(
-            __arg, __from_server, __validated_path_to_schemas, schema=cls)
-        __validation_metadata = ValidationMetadata(
-            configuration=_configuration, from_server=__from_server, validated_path_to_schemas=__validated_path_to_schemas)
-        __path_to_schemas = cls.__get_new_cls(__arg, __validation_metadata)
-        __new_cls = __path_to_schemas[__validation_metadata.path_to_item]
-        return __new_cls._get_new_instance_without_conversion_oapg(
-            __arg,
-            __validation_metadata.path_to_item,
-            __path_to_schemas
+            _arg = cls.__get_input_dict(*args, **_kwargs)
+        _from_server = False
+        _validated_path_to_schemas = {}
+        _arg = cast_to_allowed_types(
+            _arg, _from_server, _validated_path_to_schemas, schema=cls)
+        _validation_metadata = ValidationMetadata(
+            configuration=_configuration, from_server=_from_server, validated_path_to_schemas=_validated_path_to_schemas)
+        _path_to_schemas = cls.__get_new_cls(_arg, _validation_metadata)
+        _new_cls = _path_to_schemas[_validation_metadata.path_to_item]
+        return _new_cls._get_new_instance_without_conversion_oapg(
+            _arg,
+            _validation_metadata.path_to_item,
+            _path_to_schemas
         )
 
     def __init__(
         self,
         *args: typing.Union[
             dict, frozendict.frozendict, list, tuple, decimal.Decimal, float, int, str, date, datetime, bool, None, 'Schema'],
         _configuration: typing.Optional[Configuration] = None,
@@ -518,14 +522,16 @@
     TupleMixin = tuple
     StrMixin = str
     DecimalMixin = decimal.Decimal
     BoolMixin = BoolClass
     BytesMixin = bytes
     FileMixin = FileIO
     # qty 2
+    class NumberMixin(decimal.Decimal, int):
+        pass
     class BinaryMixin(bytes, FileIO):
         pass
     class NoneFrozenDictMixin(NoneClass, frozendict.frozendict):
         pass
     class NoneTupleMixin(NoneClass, tuple):
         pass
     class NoneStrMixin(NoneClass, str):
@@ -662,14 +668,16 @@
     class BoolMixin:
         _types = {BoolClass}
     class BytesMixin:
         _types = {bytes}
     class FileMixin:
         _types = {FileIO}
     # qty 2
+    class NumberMixin:
+        _types = {decimal.Decimal, int}
     class BinaryMixin:
         _types = {bytes, FileIO}
     class NoneFrozenDictMixin:
         _types = {NoneClass, frozendict.frozendict}
     class NoneTupleMixin:
         _types = {NoneClass, tuple}
     class NoneStrMixin:
@@ -1435,15 +1443,15 @@
                     return discriminated_cls
         return None
 
 
 class DictBase(Discriminable, ValidatorBase):
 
     @classmethod
-    def __validate_arg_presence(cls, arg):
+    def __validate_arg_presence(cls, arg, validation_metadata: ValidationMetadata):
         """
         Ensures that:
         - all required arguments are passed in
         - the input variable names are valid
             - present in properties or
             - accepted because additionalProperties exists
         Exceptions will be raised if:
@@ -1472,19 +1480,20 @@
             elif additional_properties is not NotAnyTypeSchema:
                 continue
             else:
                 invalid_arguments.append(property_name)
         missing_required_arguments = list(required_property_names - seen_required_properties)
         if missing_required_arguments:
             missing_required_arguments.sort()
-            raise ApiTypeError(
-                "{} is missing {} required argument{}: {}".format(
+            raise MissingRequiredPropertiesError(
+                "{} is missing {} required propert{}{}: {}".format(
                     cls.__name__,
                     len(missing_required_arguments),
-                    "s" if len(missing_required_arguments) > 1 else "",
+                    "ies" if len(missing_required_arguments) > 1 else "y",
+                    " at '{}'".format('.'.join([str(i) for i in validation_metadata.path_to_item[1:]])) if len(validation_metadata.path_to_item) > 1 else "",
                     missing_required_arguments
                 )
             )
         if invalid_arguments:
             invalid_arguments.sort()
             raise ApiTypeError(
                 "{} was passed {} invalid argument{}: {}".format(
@@ -1540,15 +1549,15 @@
                 validated_path_to_schemas=validation_metadata.validated_path_to_schemas
             )
             if arg_validation_metadata.validation_ran_earlier(schema):
                 continue
             try:
                 other_path_to_schemas = schema._validate_oapg(value, validation_metadata=arg_validation_metadata)
                 update(path_to_schemas, other_path_to_schemas)
-            except (ApiTypeError, ApiValueError) as e:
+            except (ApiTypeError, ApiValueError, MissingRequiredPropertiesError) as e:
                 validation_errors.append(e)
         if len(validation_errors) > 0:
             raise SchemaValidationError(validation_errors)
         return path_to_schemas
 
     @classmethod
     def __check_dict_validations(
@@ -1600,15 +1609,15 @@
             ApiTypeError: when the input type is not in the list of allowed spec types
         """
         if isinstance(arg, frozendict.frozendict):
             cls.__check_dict_validations(arg, validation_metadata)
         _path_to_schemas = super()._validate_oapg(arg, validation_metadata=validation_metadata)
         if not isinstance(arg, frozendict.frozendict):
             return _path_to_schemas
-        cls.__validate_arg_presence(arg)
+        cls.__validate_arg_presence(arg, validation_metadata)
         other_path_to_schemas = cls.__validate_args(arg, validation_metadata=validation_metadata)
         update(_path_to_schemas, other_path_to_schemas)
         try:
             discriminator = cls.MetaOapg.discriminator()
         except AttributeError:
             return _path_to_schemas
         # discriminator exists
@@ -1848,33 +1857,32 @@
     def __get_anyof_classes(
         cls,
         arg,
         discriminated_cls,
         validation_metadata: ValidationMetadata
     ):
         anyof_classes = []
+        exceptions: typing.List[typing.Union[ApiTypeError, ApiValueError]] = []
         path_to_schemas = defaultdict(set)
         for anyof_cls in cls.MetaOapg.any_of():
             if validation_metadata.validation_ran_earlier(anyof_cls):
                 anyof_classes.append(anyof_cls)
                 continue
 
             try:
                 other_path_to_schemas = anyof_cls._validate_oapg(arg, validation_metadata=validation_metadata)
             except (ApiValueError, ApiTypeError) as ex:
                 if discriminated_cls is not None and anyof_cls is discriminated_cls:
                     raise ex
+                exceptions.append(ex)
                 continue
             anyof_classes.append(anyof_cls)
             update(path_to_schemas, other_path_to_schemas)
         if not anyof_classes:
-            raise ApiValueError(
-                "Invalid inputs given to generate an instance of {}. None "
-                "of the anyOf schemas matched the input data.".format(cls)
-            )
+            raise AnyOfValidationError(error_list=exceptions)
         return path_to_schemas
 
     @classmethod
     def _validate_oapg(
         cls,
         arg,
         validation_metadata: ValidationMetadata,
@@ -2021,16 +2029,15 @@
     def __new__(cls, arg: None, **kwargs: Configuration):
         return super().__new__(cls, arg, **kwargs)
 
 
 class NumberSchema(
     NumberBase,
     Schema,
-    IntMixin,
-    DecimalMixin
+    NumberMixin
 ):
     """
     This is used for type: number with no format
     Both integers AND floats are accepted
     """
 
     @classmethod
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/decentro_in_kyc_client/validation_metadata.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_request.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_photocopy_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,21 +6,29 @@
     KYC & Onboarding
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
-import unittest
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import decentro_in_kyc_client
-from decentro_in_kyc_client.model.check_photocopy_request import CheckPhotocopyRequest
-from decentro_in_kyc_client import configuration
 
+RequiredCheckPhotocopyRequest = TypedDict("RequiredCheckPhotocopyRequest", {
+    "reference_id": str,
 
-class TestCheckPhotocopyRequest(unittest.TestCase):
-    """CheckPhotocopyRequest unit test stubs"""
-    pass
+    "consent": bool,
+
+    "consent_purpose": str,
+    })
 
+OptionalCheckPhotocopyRequest = TypedDict("OptionalCheckPhotocopyRequest", {
+    "image": typing.IO,
 
-if __name__ == '__main__':
-    unittest.main()
+    "image_url": str,
+    }, total=False)
+
+class CheckPhotocopyRequest(RequiredCheckPhotocopyRequest, OptionalCheckPhotocopyRequest):
+    pass
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_check_photocopy_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/check_photocopy_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,21 +6,30 @@
     KYC & Onboarding
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
-import unittest
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import decentro_in_kyc_client
-from decentro_in_kyc_client.model.check_photocopy_response import CheckPhotocopyResponse
-from decentro_in_kyc_client import configuration
 
+RequiredCheckPhotocopyResponse = TypedDict("RequiredCheckPhotocopyResponse", {
+    })
 
-class TestCheckPhotocopyResponse(unittest.TestCase):
-    """CheckPhotocopyResponse unit test stubs"""
-    pass
+OptionalCheckPhotocopyResponse = TypedDict("OptionalCheckPhotocopyResponse", {
+    "data": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+
+    "decentroTxnId": str,
+
+    "message": str,
 
+    "responseCode": str,
 
-if __name__ == '__main__':
-    unittest.main()
+    "status": str,
+    }, total=False)
+
+class CheckPhotocopyResponse(RequiredCheckPhotocopyResponse, OptionalCheckPhotocopyResponse):
+    pass
```

### Comparing `decentro-in-kyc-python-sdk-4.3.0/test/test_models/test_classify_document400_response.py` & `decentro_in_kyc_python_sdk-4.4.0/decentro_in_kyc_client/type/classify_document_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,21 +6,30 @@
     KYC & Onboarding
 
     The version of the OpenAPI document: 1.0.0
     Contact: admin@decentro.tech
     Created by: https://decentro.tech
 """
 
-import unittest
+from datetime import datetime, date
+import typing
+from enum import Enum
+from typing_extensions import TypedDict, Literal
 
-import decentro_in_kyc_client
-from decentro_in_kyc_client.model.classify_document400_response import ClassifyDocument400Response
-from decentro_in_kyc_client import configuration
 
+RequiredClassifyDocumentResponse = TypedDict("RequiredClassifyDocumentResponse", {
+    })
 
-class TestClassifyDocument400Response(unittest.TestCase):
-    """ClassifyDocument400Response unit test stubs"""
-    pass
+OptionalClassifyDocumentResponse = TypedDict("OptionalClassifyDocumentResponse", {
+    "data": typing.Dict[str, typing.Union[bool, date, datetime, dict, float, int, list, str, None]],
+
+    "decentroTxnId": str,
+
+    "message": str,
 
+    "responseCode": str,
 
-if __name__ == '__main__':
-    unittest.main()
+    "status": str,
+    }, total=False)
+
+class ClassifyDocumentResponse(RequiredClassifyDocumentResponse, OptionalClassifyDocumentResponse):
+    pass
```

