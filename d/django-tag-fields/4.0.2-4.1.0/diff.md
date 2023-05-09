# Comparing `tmp/django-tag-fields-4.0.2.tar.gz` & `tmp/django-tag-fields-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tag-fields-4.0.2.tar", last modified: Sat May  6 09:16:09 2023, max compression
+gzip compressed data, was "django-tag-fields-4.1.0.tar", last modified: Tue May  9 01:29:05 2023, max compression
```

## Comparing `django-tag-fields-4.0.2.tar` & `django-tag-fields-4.1.0.tar`

### file list

```diff
@@ -1,117 +1,112 @@
--rw-r--r--   0        0        0      235 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.coveragerc
--rw-r--r--   0        0        0     1983 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/.git-commit-template.txt
--rw-r--r--   0        0        0      907 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      136 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/chore.md
--rw-r--r--   0        0        0      424 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/documentation-request.md
--rw-r--r--   0        0        0      619 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      841 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/semantic.yaml
--rw-r--r--   0        0        0      923 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1503 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1198 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.gitignore
--rw-r--r--   0        0        0     1389 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      751 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/AUTHORS
--rw-r--r--   0        0        0    13299 2023-05-06 09:16:04.401654 django-tag-fields-4.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    13597 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/CHANGELOG.rst
--rw-r--r--   0        0        0     5488 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5382 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1574 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/LICENSE
--rw-r--r--   0        0        0      205 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/MANIFEST.in
--rw-r--r--   0        0        0     2739 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/README.rst
--rw-r--r--   0        0        0      853 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/codecov.yml
--rw-r--r--   0        0        0     1525 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/admin.rst
--rw-r--r--   0        0        0     4396 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/api.rst
--rw-r--r--   0        0        0       29 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/changelog.rst
--rw-r--r--   0        0        0      471 2023-05-06 09:16:04.417654 django-tag-fields-4.0.2/docs/conf.py
--rw-r--r--   0        0        0       33 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/contributing.rst
--rw-r--r--   0        0        0     8990 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/custom_tagging.rst
--rw-r--r--   0        0        0     2251 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/external_apps.rst
--rw-r--r--   0        0        0     1040 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/faq.rst
--rw-r--r--   0        0        0     2378 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/forms.rst
--rw-r--r--   0        0        0     1902 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/getting_started.rst
--rw-r--r--   0        0        0      705 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/index.rst
--rw-r--r--   0        0        0      810 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/docs/serializers.rst
--rw-r--r--   0        0        0     1854 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/pyproject.toml
--rw-r--r--   0        0        0       33 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/requirements/docs.txt
--rw-r--r--   0        0        0       36 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/requirements/test.txt
--rw-r--r--   0        0        0       38 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/setup.py
--rw-r--r--   0        0        0      259 2023-05-06 09:16:04.421654 django-tag-fields-4.0.2/tag_fields/__init__.py
--rw-r--r--   0        0        0      382 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/admin.py
--rw-r--r--   0        0        0      253 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/apps.py
--rw-r--r--   0        0        0     1442 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/forms.py
--rw-r--r--   0        0        0     1299 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2206 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1042 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2005 2023-05-06 09:16:03.481648 django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1033 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1941 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1068 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1839 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      991 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2188 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1738 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1131 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1873 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1058 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2021 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1203 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2162 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1047 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1928 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1105 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2073 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      828 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1955 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      945 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1904 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1142 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1908 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      993 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1947 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      933 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1739 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1045 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1897 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1870 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2544 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1051 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2014 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1211 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2144 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      992 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1982 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    30372 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/managers.py
--rw-r--r--   0        0        0     2694 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0001_initial.py
--rw-r--r--   0        0        0      280 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0002_auto_20150616_2121.py
--rw-r--r--   0        0        0      374 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0003_taggeditem_add_unique_index.py
--rw-r--r--   0        0        0     1232 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py
--rw-r--r--   0        0        0      502 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/0005_auto_20220424_2025.py
--rw-r--r--   0        0        0        0 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/migrations/__init__.py
--rw-r--r--   0        0        0     7778 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/models.py
--rw-r--r--   0        0        0     4417 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/serializers.py
--rw-r--r--   0        0        0     4476 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/utils.py
--rw-r--r--   0        0        0     1583 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tag_fields/views.py
--rw-r--r--   0        0        0        0 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/__init__.py
--rw-r--r--   0        0        0       89 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/admin.py
--rw-r--r--   0        0        0      168 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/custom_parser.py
--rw-r--r--   0        0        0      834 2023-05-06 09:16:03.485648 django-tag-fields-4.0.2/tests/forms.py
--rw-r--r--   0        0        0    39683 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0001_initial.py
--rw-r--r--   0        0        0     3529 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0002_auto_20200214_1129.py
--rw-r--r--   0        0        0     3015 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0003_auto_20210310_0918.py
--rw-r--r--   0        0        0     4440 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0004_auto_20210619_0826.py
--rw-r--r--   0        0        0     1025 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/0005_auto_20210713_2301.py
--rw-r--r--   0        0        0        0 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/migrations/__init__.py
--rw-r--r--   0        0        0    10311 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/models.py
--rw-r--r--   0        0        0      323 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/serializers.py
--rw-r--r--   0        0        0     1333 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/settings.py
--rw-r--r--   0        0        0      124 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/templates/tests/food_tag_list.html
--rw-r--r--   0        0        0     1394 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_admin.py
--rw-r--r--   0        0        0     1857 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_forms.py
--rw-r--r--   0        0        0     2359 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_models.py
--rw-r--r--   0        0        0     3366 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_serializers.py
--rw-r--r--   0        0        0      984 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/test_utils.py
--rw-r--r--   0        0        0    54035 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/tests.py
--rw-r--r--   0        0        0      294 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/urls.py
--rw-r--r--   0        0        0      182 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tests/views.py
--rw-r--r--   0        0        0     1174 2023-05-06 09:16:03.489647 django-tag-fields-4.0.2/tox.ini
--rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 django-tag-fields-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0      235 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.coveragerc
+-rw-r--r--   0        0        0     1983 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/.git-commit-template.txt
+-rw-r--r--   0        0        0      907 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      136 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/ISSUE_TEMPLATE/chore.md
+-rw-r--r--   0        0        0      424 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/ISSUE_TEMPLATE/documentation-request.md
+-rw-r--r--   0        0        0      619 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      841 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/semantic.yaml
+-rw-r--r--   0        0        0      923 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1503 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1209 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.gitignore
+-rw-r--r--   0        0        0     1389 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      413 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      751 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/AUTHORS
+-rw-r--r--   0        0        0    14292 2023-05-09 01:29:00.500080 django-tag-fields-4.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5488 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5382 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1596 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/LICENSE
+-rw-r--r--   0        0        0      205 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     2739 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/README.rst
+-rw-r--r--   0        0        0    13597 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/_OLD_CHANGELOG.rst
+-rw-r--r--   0        0        0      853 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/codecov.yml
+-rw-r--r--   0        0        0      638 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/docs/make.bat
+-rw-r--r--   0        0        0     1528 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/docs/source/admin.rst
+-rw-r--r--   0        0        0     4405 2023-05-09 01:28:59.692024 django-tag-fields-4.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0       53 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     2602 2023-05-09 01:29:00.516081 django-tag-fields-4.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0       38 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0     9001 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/custom_tagging.rst
+-rw-r--r--   0        0        0     2251 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/external_apps.rst
+-rw-r--r--   0        0        0     1040 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/faq.rst
+-rw-r--r--   0        0        0     2379 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/forms.rst
+-rw-r--r--   0        0        0     1904 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      955 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      811 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/docs/source/serializers.rst
+-rw-r--r--   0        0        0     1861 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/requirements/docs.txt
+-rw-r--r--   0        0        0       36 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/requirements/test.txt
+-rw-r--r--   0        0        0       38 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/setup.py
+-rw-r--r--   0        0        0      259 2023-05-09 01:29:00.516081 django-tag-fields-4.1.0/tag_fields/__init__.py
+-rw-r--r--   0        0        0      398 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/admin.py
+-rw-r--r--   0        0        0      253 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/apps.py
+-rw-r--r--   0        0        0     1442 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/forms.py
+-rw-r--r--   0        0        0     1299 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2206 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1042 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2005 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1033 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1941 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1068 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1839 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      991 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2188 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1738 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1131 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1873 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1058 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2021 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1203 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2162 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1047 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1928 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1105 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2073 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      828 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1955 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      945 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1904 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1142 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1908 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      993 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1947 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      933 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1739 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1045 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1897 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1870 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2544 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1051 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2014 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1211 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2144 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      992 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1982 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    31051 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/managers.py
+-rw-r--r--   0        0        0     1843 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/migrations/__init__.py
+-rw-r--r--   0        0        0     8002 2023-05-09 01:28:59.696025 django-tag-fields-4.1.0/tag_fields/models.py
+-rw-r--r--   0        0        0     4417 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tag_fields/serializers.py
+-rw-r--r--   0        0        0     4476 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tag_fields/utils.py
+-rw-r--r--   0        0        0     1599 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tag_fields/views.py
+-rw-r--r--   0        0        0        0 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       89 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/admin.py
+-rw-r--r--   0        0        0      168 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/custom_parser.py
+-rw-r--r--   0        0        0      834 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/forms.py
+-rw-r--r--   0        0        0    29102 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/migrations/__init__.py
+-rw-r--r--   0        0        0    10360 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/models.py
+-rw-r--r--   0        0        0      323 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/serializers.py
+-rw-r--r--   0        0        0     1333 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/settings.py
+-rw-r--r--   0        0        0      124 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/templates/tests/food_tag_list.html
+-rw-r--r--   0        0        0     1394 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/test_admin.py
+-rw-r--r--   0        0        0     1907 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/test_forms.py
+-rw-r--r--   0        0        0     2359 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/test_models.py
+-rw-r--r--   0        0        0     3366 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/test_serializers.py
+-rw-r--r--   0        0        0      984 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0    54134 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/tests.py
+-rw-r--r--   0        0        0      294 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/urls.py
+-rw-r--r--   0        0        0      182 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tests/views.py
+-rw-r--r--   0        0        0     1174 2023-05-09 01:28:59.700025 django-tag-fields-4.1.0/tox.ini
+-rw-r--r--   0        0        0     4065 1970-01-01 00:00:00.000000 django-tag-fields-4.1.0/PKG-INFO
```

### Comparing `django-tag-fields-4.0.2/.github/.git-commit-template.txt` & `django-tag-fields-4.1.0/.github/.git-commit-template.txt`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/bug-report.md` & `django-tag-fields-4.1.0/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/.github/ISSUE_TEMPLATE/feature-request.md` & `django-tag-fields-4.1.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/.github/semantic.yaml` & `django-tag-fields-4.1.0/.github/semantic.yaml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/.github/workflows/release.yml` & `django-tag-fields-4.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/.github/workflows/test.yml` & `django-tag-fields-4.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/.gitignore` & `django-tag-fields-4.1.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/html/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `django-tag-fields-4.0.2/.pre-commit-config.yaml` & `django-tag-fields-4.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/AUTHORS` & `django-tag-fields-4.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/CHANGELOG.md` & `django-tag-fields-4.1.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 # Changelog
 
 ## (Unreleased)
 
 <!--next-version-placeholder-->
 
+## v4.1.0 (2023-05-09)
+### Feature
+* **tags:** Rename models ready for adding fields #66 ([`a21fec8`](https://github.com/imAsparky/django-tag-fields/commit/a21fec833f4745682228260e8f77886c0b8ddfd3))
+
+### Fix
+* **ver:** Update conf.py location in sem_ver #68 ([`14ff854`](https://github.com/imAsparky/django-tag-fields/commit/14ff8549930c0c46a5ed097f92d61a36f5f281ed))
+
+### Documentation
+* **models:** Update model names #66 ([`de364b4`](https://github.com/imAsparky/django-tag-fields/commit/de364b48ecf9afe09279b2c9d74f9f3fd7004c09))
+* **structure:** Update to standard Sphinx #63 ([`f03086a`](https://github.com/imAsparky/django-tag-fields/commit/f03086acd78a8ad5d0af36dfb122e09444865ab0))
+* **config:** Add readthedocs and extra deps #63 ([`94e4374`](https://github.com/imAsparky/django-tag-fields/commit/94e437496323dd5545d9ccd1f6b768fd653e9db5))
+* **deps:** Update docutils #61 ([`c5a4ed3`](https://github.com/imAsparky/django-tag-fields/commit/c5a4ed3802cd421d2dab2d22a4fe814fb6305acd))
+
 ## v4.0.2 (2023-05-06)
 ### Fix
 * **settings:** Update Constant names #59 ([`c2a9b3a`](https://github.com/imAsparky/django-tag-fields/commit/c2a9b3ab5047023464ff4a032f2eafce68c7d06b))
 
 ### Documentation
 * **settings:** Update Constant names #59 ([`1395043`](https://github.com/imAsparky/django-tag-fields/commit/13950430a4300365259f5e99c560f70c29069fca))
 * **manager:** Add docstrings to select areas #57 ([`d524d44`](https://github.com/imAsparky/django-tag-fields/commit/d524d44ba99f4214ba05080903997593d6c6849f))
```

### Comparing `django-tag-fields-4.0.2/CHANGELOG.rst` & `django-tag-fields-4.1.0/_OLD_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/CODE_OF_CONDUCT.md` & `django-tag-fields-4.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/CONTRIBUTING.rst` & `django-tag-fields-4.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/LICENSE` & `django-tag-fields-4.1.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     1. Redistributions of source code must retain the above copyright notice,
        this list of conditions and the following disclaimer.
 
     2. Redistributions in binary form must reproduce the above copyright
        notice, this list of conditions and the following disclaimer in the
        documentation and/or other materials provided with the distribution.
 
-    3. Neither the name of django-taggit nor the names of its contributors
-       may be used to endorse or promote products derived from this software
-       without specific prior written permission.
+    3. Neither the names of django-taggit or django-tag-fields nor the names of
+       its contributors may be used to endorse or promote products derived from
+       this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
 ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
```

### Comparing `django-tag-fields-4.0.2/README.rst` & `django-tag-fields-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/codecov.yml` & `django-tag-fields-4.1.0/codecov.yml`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/docs/admin.rst` & `django-tag-fields-4.1.0/docs/source/admin.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Using tags in the admin
 =======================
 
-By default if you have a :class:`TaggableManager` on your model it will show up
+By default if you have a :class:`ModelTagsManager` on your model it will show up
 in the admin, just as it will in any other form.
 
 If you are specifying :attr:`ModelAdmin.fieldsets
 <django.contrib.admin.ModelAdmin.fieldsets>`, include the name of the
-:class:`TaggableManager` as a field::
+:class:`ModelTagsManager` as a field::
 
     fieldsets = (
         (None, {'fields': ('tags',)}),
     )
 
 Including tags in ``ModelAdmin.list_display``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 One important thing to note is that you *cannot* include a
-:class:`TaggableManager` in :attr:`ModelAdmin.list_display
+:class:`ModelTagsManager` in :attr:`ModelAdmin.list_display
 <django.contrib.admin.ModelAdmin.list_display>`. If you do you'll see an
 exception that looks like::
 
     AttributeError: '_TaggableManager' object has no attribute 'name'
 
 This is for the same reason that you cannot include a
 :class:`~django.db.models.ManyToManyField`: it would result in an unreasonable
```

### Comparing `django-tag-fields-4.0.2/docs/api.rst` & `django-tag-fields-4.1.0/docs/source/api.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 The API
 =======
 
-After you've got your ``TaggableManager`` added to your model you can start
+After you've got your ``ModelTagsManager`` added to your model you can start
 playing around with the API.
 
-.. class:: TaggableManager([verbose_name="Tags", help_text="A comma-separated list of tags.", through=None, blank=False])
+.. class:: ModelTagsManager([verbose_name="Tags", help_text="A comma-separated list of tags.", through=None, blank=False])
 
     :param verbose_name: The verbose_name for this field.
     :param help_text: The help_text to be used in forms (including the admin).
     :param through: The through model, see :doc:`custom_tagging` for more
         information.
     :param blank: Controls whether this field is required.
 
@@ -81,27 +81,27 @@
 
             >>> apple.tags.slugs()
             ["green-and-juicy", "red"]
 
     .. hint::
 
        You can subclass ``_TaggableManager`` (note the underscore) to add
-       methods or functionality. ``TaggableManager`` takes an optional
+       methods or functionality. ``ModelTagsManager`` takes an optional
        manager keyword argument for your custom class, like this::
 
           class Food(models.Model):
               # ... fields here
-              tags = TaggableManager(manager=_CustomTaggableManager)
+              tags = ModelTagsManager(manager=_CustomTaggableManager)
 
 Filtering
 ~~~~~~~~~
 
 To find all of a model with a specific tags you can filter, using the normal
 Django ORM API.  For example if you had a ``Food`` model, whose
-``TaggableManager`` was named ``tags``, you could find all the delicious fruit
+``ModelTagsManager`` was named ``tags``, you could find all the ``delicious`` fruit
 like so::
 
     >>> Food.objects.filter(tags__name__in=["delicious"])
     [<Food: apple>, <Food: pear>, <Food: plum>]
 
 
 If you're filtering on multiple tags, it's very common to get duplicate
```

### Comparing `django-tag-fields-4.0.2/docs/custom_tagging.rst` & `django-tag-fields-4.1.0/docs/source/custom_tagging.rst`

 * *Files 10% similar despite different names*

```diff
@@ -35,31 +35,31 @@
 Custom ForeignKeys
 ~~~~~~~~~~~~~~~~~~
 
 Your intermediary model must be a subclass of
 ``tag_fields.models.TaggedItemThroughBase`` with a foreign key to your content
 model named ``content_object``.
 
-Pass this intermediary model as the ``through`` argument to ``TaggableManager``:
+Pass this intermediary model as the ``through`` argument to ``ModelTagsManager``:
 
   .. code-block:: python
 
     from django.db import models
 
-    from tag_fields.managers import TaggableManager
+    from tag_fields.managers import ModelTagsManager
     from tag_fields.models import TaggedItemThroughBase
 
 
     class TaggedFood(TaggedItemThroughBase):
         content_object = models.ForeignKey('Food', on_delete=models.CASCADE)
 
     class Food(models.Model):
         # ... fields here
 
-        tags = TaggableManager(through=TaggedFood)
+        tags = ModelTagsManager(through=TaggedFood)
 
 
 Once this is done, the API works the same as for GFK-tagged models.
 
 Custom GenericForeignKeys
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -70,42 +70,42 @@
 
 For example, if your primary key is a string:
 
   .. code-block:: python
 
     from django.db import models
 
-    from tag_fields.managers import TaggableManager
+    from tag_fields.managers import ModelTagsManager
     from tag_fields.models import (
                                    GenericFKTaggedItemThroughBase,
                                    TaggedItemThroughBase,
                                   )
 
     class GenericStringTaggedItem(GenericFKTaggedItemThroughBase, TaggedItemThroughBase):
         object_id = models.CharField(max_length=50, verbose_name=_('Object id'), db_index=True)
 
     class Food(models.Model):
         food_id = models.CharField(primary_key=True)
         # ... fields here
 
-        tags = TaggableManager(through=GenericStringTaggedItem)
+        tags = ModelTagsManager(through=GenericStringTaggedItem)
 
 UUIDFKTaggedItemThroughBase
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A common use case of a non-integer primary key is the UUID primary key.
 ``django-tag-fields`` provides a base class ``UUIDFKTaggedItemThroughBase`` ready
 to use with models using a UUID primary key:
 
   .. code-block:: python
 
     from django.db import models
     from django.utils.translation import gettext_lazy as _
 
-    from tag_fields.managers import TaggableManager
+    from tag_fields.managers import ModelTagsManager
     from tag_fields.models import (
                                    UUIDFKTaggedItemThroughBase,
                                    TaggedItemThroughBase,
                                   )
 
     class UUIDTaggedItem(UUIDFKTaggedItemThroughBase, TaggedItemThroughBase):
         # If you only inherit UUIDFKTaggedItemThroughBase, you need to define
@@ -116,32 +116,32 @@
             verbose_name = _("Tag")
             verbose_name_plural = _("Tags")
 
     class Food(models.Model):
         id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
         # ... fields here
 
-        tags = TaggableManager(through=UUIDTaggedItem)
+        tags = ModelTagsManager(through=UUIDTaggedItem)
 
 Custom tag
 ~~~~~~~~~~
 
 When providing a custom ``Tag`` model, it should be a ``ForeignKey`` to your
 tag model named ``"tag"``. If your custom ``Tag`` model has extra parameters
 you want to initialize during setup, you can pass it along via the
-``tag_kwargs`` parameter of ``TaggableManager.add``.
+``tag_kwargs`` parameter of ``ModelTagsManager.add``.
 
 For example, ``my_food.tags.add("tag_name1", "tag_name2", tag_kwargs={"my_field":3})``:
 
 .. code-block:: python
 
     from django.db import models
     from django.utils.translation import gettext_lazy as _
 
-    from tag_fields.managers import TaggableManager
+    from tag_fields.managers import ModelTagsManager
     from tag_fields.models import TagBase, GenericFKTaggedItemThroughBase
 
 
     class MyCustomTag(TagBase):
         # ... fields here
 
         class Meta:
@@ -164,21 +164,21 @@
             related_name="%(app_label)s_%(class)s_items",
         )
 
 
     class Food(models.Model):
         # ... fields here
 
-        tags = TaggableManager(through=TaggedWhatever)
+        tags = ModelTagsManager(through=TaggedWhatever)
 
 
     class Drink(models.Model):
         # ... fields here
 
-        tags = TaggableManager(through=TaggedWhatever)
+        tags = ModelTagsManager(through=TaggedWhatever)
 
 
 .. class:: TagBase
 
     .. method:: slugify(tag, i=None)
 
       The ``tag-fields`` feature uses the :func:`django.utils.text.slugify`
```

### Comparing `django-tag-fields-4.0.2/docs/external_apps.rst` & `django-tag-fields-4.1.0/docs/source/external_apps.rst`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/docs/faq.rst` & `django-tag-fields-4.1.0/docs/source/faq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Frequently Asked Questions
 ==========================
 
 1. How can I get all my tags?
 -----------------------------
 
 To start using tags, you can access the pre-built ``Tag`` model
-in ``tag_fields.models``.
-
-However, if you have a custom model derived
-from ``ThroughTableBase``you will need to query that instead.
-
-For the standard setup, use ``Tag.objects.all()`` to retrieve all the
+in ``tag_fields.models``.  However, if you have a custom model derived from ``ThroughTableBase``you will need to query that instead.  For the standard setup, use ``Tag.objects.all()`` to retrieve all the
 available tags.
 
 
 
 2. How can I use this with factory_boy?
 ---------------------------------------
```

### Comparing `django-tag-fields-4.0.2/docs/forms.rst` & `django-tag-fields-4.1.0/docs/source/forms.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. _tags-in-forms:
 
 Tags in forms
 =============
 
-The ``TaggableManager`` will show up automatically as a field in a
+The ``ModelTagsManager`` will show up automatically as a field in a
 ``ModelForm`` or in the admin. Tags input via the form field are parsed
 as follows:
 
 * If the input doesn't contain any commas or double quotes, it is simply
   treated as a space-delimited list of tag names.
 
 * If the input does contain either of these characters:
```

### Comparing `django-tag-fields-4.0.2/docs/getting_started.rst` & `django-tag-fields-4.1.0/docs/source/getting_started.rst`

 * *Files 13% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 And then, to any model you want tagged, do the following.
 
 .. code-block:: python
 
     from django.db import models
 
-    from tag_fields.managers import TaggableManager
+    from tag_fields.managers import ModelTagsManager
 
     class Food(models.Model):
         # ... fields here
 
-        tags = TaggableManager()
+        tags = ModelTagsManager()
 
 
 .. tip::
 
     To make ``django-tag-fields`` search for existing tags in a
     case-insensitive way, you need to modify the ``TAGS_CASE_INSENSITIVE``
     setting.
```

### Comparing `django-tag-fields-4.0.2/docs/serializers.rst` & `django-tag-fields-4.1.0/docs/source/serializers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Usage With Django Rest Framework
 ================================
 
-To add tags into a ``TaggableManager()`` using ``django-tag-fields``, the usual
+To add tags into a ``ModelTagsManager()`` using ``django-tag-fields``, the usual
 ``Serializer`` from Django REST Framework cannot be used.
 
 Attempting to save the tags into a list using ``DRF Serializer`` will cause
 an exception.
 
 To enable the acceptance of tags via a REST API call, you need to add the
 following to the ``Serializer``.
```

### Comparing `django-tag-fields-4.0.2/pyproject.toml` & `django-tag-fields-4.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 [tool.semantic_release]
 branch = "main"
 build_command = 'python -m pip install flit && flit build'
 changelog_file = "CHANGELOG.md"
 commit_subject = ":memo: build(version): Bump to version - {version}."
-version_variable = "docs/conf.py:__version__,tag_fields/__init__.py:__version__"
+version_variable = "docs/source/conf.py:__version__,tag_fields/__init__.py:__version__"
 
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 # tests = ["B201", "B301"]
 # skips = ["B101", "B601"]
```

### Comparing `django-tag-fields-4.0.2/tag_fields/forms.py` & `django-tag-fields-4.1.0/tag_fields/forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/ar/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/cs/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/da/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/de/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/el/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/en/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/eo/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/es/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/fa/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/fi/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/fr/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/he/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/it/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/ja/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/nb/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/nl/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/pt_BR/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/ru/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/tr/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/uk/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-tag-fields-4.1.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po` & `django-tag-fields-4.1.0/tag_fields/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/managers.py` & `django-tag-fields-4.1.0/tag_fields/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from django.utils.text import capfirst
 from django.utils.translation import gettext_lazy as _
 
 from tag_fields.forms import TagField
 from tag_fields.models import (
     GenericFKTaggedItemThroughBase,
     UUIDFKTaggedItemThroughBase,
-    TaggedItem,
+    ModelTagIntFk,
 )
 from tag_fields.utils import require_instance_manager
 
 
 class ExtraJoinRestriction:
     """
     An extra restriction used for contenttype restriction in joins.
@@ -85,39 +85,44 @@
 
     Paramaters
     ==========
 
     :param through: The name of the django through table
     :type through: str
 
-    :param model: The namen of the model for the Taggable manager
+    :param model: The name of the model for the Taggable manager
     :type model: str
 
     :param instance: Instance for the Taggable manager
     :type instance: class:`models.Model`
 
     :param prefetch_cache_name: todo
     :type prefetch_cache_name: todo
 
     :param ordering: todo
     :type ordering: todo
 
+    :param field_name: Default ``tags``.  Provide a custom field name for the
+        model tag field name.
+    :type field_name: str, optional
+
     .. todo::
         Very old todo here.
 
         Investigate whether we can use a RelatedManager instead of all this
         stuff to take advantage of all the Django goodness
     """
 
     def __init__(
         self,
         through,
         model,
         instance,
         prefetch_cache_name,
+        field_name=None,
         ordering=None,
     ):
         super().__init__()
         self.through = through
         self.model = model
         self.instance = instance
         self.prefetch_cache_name = prefetch_cache_name
@@ -520,15 +525,15 @@
         for result in qs:
             obj = items[tuple(result[k] for k in lookup_keys)]
             obj.similar_tags = result["n"]
             results.append(obj)
         return results
 
 
-class TaggableManager(RelatedField):
+class ModelTagsManager(RelatedField):
     """
     Manager for handling the actions required on Tags.
 
     Paramaters
     ==========
 
     :param blank: Default: False Determines if the field is required
@@ -572,17 +577,18 @@
         verbose_name=_("Tags"),
         help_text=_("A comma-separated list of tags."),
         through=None,
         blank=False,
         related_name=None,
         to=None,
         ordering=None,
+        field_name=None,
         manager=_TaggableManager,
     ):
-        self.through = through or TaggedItem
+        self.through = through or ModelTagIntFk
 
         rel = ManyToManyRel(
             self, to, related_name=related_name, through=self.through
         )
 
         super().__init__(
             verbose_name=verbose_name,
@@ -593,14 +599,19 @@
             rel=rel,
         )
 
         self.ordering = ordering
         self.swappable = False
         self.manager = manager
 
+        if field_name:
+            self.field_name = field_name
+        else:
+            self.field_name = "tags"
+
     def __get__(self, instance, model):
         """
         Check the instance has a primary key.
 
         :raises ValueError: "%s objects need to have a primary key value "
                 "before you can access their tags." % model.__name__
 
@@ -681,29 +692,38 @@
             else:
                 self.post_through_setup(cls)
 
     def get_internal_type(self):
         return "ManyToManyField"
 
     def post_through_setup(self, cls):
+        """
+        Checks the tag through table, and if duplicates raises an error.
+
+        :raises ValueError: "You can't have two TaggableManagers with the
+            same through model."
+        """
+        print(f"\nMANAGER FIELD NAME {self.field_name}")
         self.use_gfk = self.through is None or issubclass(
             self.through, GenericFKTaggedItemThroughBase
         )
 
         if not self.remote_field.model:
             self.remote_field.model = self.through._meta.get_field(
                 "tag"
             ).remote_field.model
 
         if self.use_gfk:
+            print(f"\nMANAGER USING GFK {self.through}")
             tagged_items = GenericRelation(self.through)
             tagged_items.contribute_to_class(cls, "tagged_items")
 
         for rel in cls._meta.local_many_to_many:
-            if rel == self or not isinstance(rel, TaggableManager):
+            print(f"\nMANAGER REL {rel}")
+            if rel == self or not isinstance(rel, ModelTagsManager):
                 continue
             if rel.through == self.through:
                 raise ValueError(
                     "You can't have two TaggableManagers with the"
                     " same through model."
                 )
```

### Comparing `django-tag-fields-4.0.2/tag_fields/migrations/0004_alter_taggeditem_content_type_alter_taggeditem_tag.py` & `django-tag-fields-4.1.0/tag_fields/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,43 @@
-# This migration has no effect in practice. It exists to stop
-# Django from autodetecting migrations in tag_fields when users
-# update to Django 4.0.
-# See https://docs.djangoproject.com/en/stable/releases/4.0/#migrations-autodetector-changes
-import django.db.models.deletion
+# Generated by Django 4.2 on 2023-05-08 19:18
+
 from django.db import migrations, models
+import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
+    initial = True
+
     dependencies = [
-        ("contenttypes", "0002_remove_content_type_name"),
-        ("tag_fields", "0003_taggeditem_add_unique_index"),
+        ('contenttypes', '0002_remove_content_type_name'),
     ]
 
     operations = [
-        migrations.AlterField(
-            model_name="taggeditem",
-            name="content_type",
-            field=models.ForeignKey(
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="%(app_label)s_%(class)s_tagged_items",
-                to="contenttypes.contenttype",
-                verbose_name="content type",
-            ),
+        migrations.CreateModel(
+            name='ModelTag',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=100, unique=True, verbose_name='name')),
+                ('slug', models.SlugField(allow_unicode=True, max_length=100, unique=True, verbose_name='slug')),
+            ],
+            options={
+                'verbose_name': 'Model Tag',
+                'verbose_name_plural': 'Model Tags',
+            },
         ),
-        migrations.AlterField(
-            model_name="taggeditem",
-            name="tag",
-            field=models.ForeignKey(
-                on_delete=django.db.models.deletion.CASCADE,
-                related_name="%(app_label)s_%(class)s_items",
-                to="tag_fields.tag",
-            ),
+        migrations.CreateModel(
+            name='ModelTagIntFk',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('object_id', models.IntegerField(db_index=True, verbose_name='object ID')),
+                ('content_type', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='%(app_label)s_%(class)s_tagged_items', to='contenttypes.contenttype', verbose_name='content type')),
+                ('tag', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='%(app_label)s_%(class)s_items', to='tag_fields.modeltag')),
+            ],
+            options={
+                'verbose_name': 'Model Tag IntFk',
+                'verbose_name_plural': 'Model Tags IntFk',
+                'unique_together': {('content_type', 'object_id', 'tag')},
+                'index_together': {('content_type', 'object_id')},
+            },
         ),
     ]
```

### Comparing `django-tag-fields-4.0.2/tag_fields/models.py` & `django-tag-fields-4.1.0/tag_fields/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     from unidecode import unidecode
 except ImportError:
 
     def unidecode(tag):
         return tag
 
 
+# Tags base models ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 class TagBase(models.Model):
     """Abstract Base class for the tags."""
 
     class Meta:
         abstract = True
 
     name = models.CharField(
@@ -84,35 +85,37 @@
         else:
             slug = slugify(tag, allow_unicode=True)
         if i is not None:
             slug += "_%d" % i
         return slug
 
 
-class Tag(TagBase):
+# Tag models ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+class ModelTag(TagBase):
     """Model tag for use with your own model.
 
     This is a model level tag, i.e. there can only be one per model.
 
+    taggit class name was Tag
     """
 
     class Meta:
-        verbose_name = _("tag")
-        verbose_name_plural = _("tags")
+        verbose_name = _("Model Tag")
+        verbose_name_plural = _("Model Tags")
         app_label = "tag_fields"
 
 
+# Through table base models ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 class ThroughTableBase(models.Model):
-    """Base class for a model ``tags`` through table.
+    """Base class for a models ``tags`` through table.
 
     Abstract Base Class: ``through table`` for all ``through table``
     sub classes.
 
     taggit class name was ItemBase
-
     """
 
     class Meta:
         abstract = True
 
     def __str__(self):
         return gettext("%(object)s tagged with %(tag)s") % {
@@ -148,36 +151,33 @@
 
 class TaggedItemThroughBase(ThroughTableBase):
     """Sub class of ``ThroughTableBase``
 
     Base class: ``through table`` for a ``Tagged Item`` model.
 
     taggit class name was TaggedItemBase
-
     """
 
     class Meta:
         abstract = True
 
     tag = models.ForeignKey(
-        Tag,
+        ModelTag,
         related_name="%(app_label)s_%(class)s_items",
         on_delete=models.CASCADE,
     )
 
 
 class GenericFKTaggedItemThroughBase(ThroughTableBase):
     """Abstract subclass of ``ThroughTableBase`` using a ``GenericForeignKey``.
 
     Base class: ``through table`` for a ``Tagged Item`` model using an
     ``GenericForeignKey``.
 
     taggit class name was CommonGenericTaggedItemBase
-
-
     """
 
     class Meta:
         abstract = True
 
     content_type = models.ForeignKey(
         ContentType,
@@ -213,15 +213,14 @@
     """Abstract subclass of ``GenericFKTaggedItemThroughBase`` with
      ``Integer Foreign Key``.
 
     Base class: ``through table`` for a ``Tagged Item`` model using an
     ``integer`` primary key.
 
     taggit class name was GenericTaggedItemBase
-
     """
 
     class Meta:
         abstract = True
 
     object_id = models.IntegerField(verbose_name=_("object ID"), db_index=True)
 
@@ -230,36 +229,30 @@
     """Abstract subclass of CommonGenericTaggedItemBase with a
       ```UUID Foreign Key``.
 
     Base class: ``through table`` for a ``Tagged Item`` model using an ``UUID``
     primary key.
 
     taggit class name was GenericUUIDTaggedItemBase
-
     """
 
     class Meta:
         abstract = True
 
     object_id = models.UUIDField(verbose_name=_("object ID"), db_index=True)
 
 
-class TaggedItem(IntegerFKTaggedItemThroughBase, TaggedItemThroughBase):
+# Through tables ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+class ModelTagIntFk(IntegerFKTaggedItemThroughBase, TaggedItemThroughBase):
     """Tagged Item Through Table using Integer Foreign Key.
 
     Allows custom Tag models. Tagged models use a ``Integer`` primary key.
 
     taggit class name was TaggedItem
-
-    .. note::
-
-        Changing this class name breaks the tests. Some checks made to see what
-        was causing the error but it requires more time.
-
     """
 
     class Meta:
-        verbose_name = _("tagged item")
-        verbose_name_plural = _("tagged items")
+        verbose_name = _("Model Tag IntFk")
+        verbose_name_plural = _("Model Tags IntFk")
         app_label = "tag_fields"
         index_together = [["content_type", "object_id"]]
         unique_together = [["content_type", "object_id", "tag"]]
```

### Comparing `django-tag-fields-4.0.2/tag_fields/serializers.py` & `django-tag-fields-4.1.0/tag_fields/serializers.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/utils.py` & `django-tag-fields-4.1.0/tag_fields/utils.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tag_fields/views.py` & `django-tag-fields-4.1.0/tag_fields/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import get_object_or_404
 from django.views.generic.list import ListView
 
-from tag_fields.models import Tag, TaggedItem
+from tag_fields.models import ModelTag, ModelTagIntFk
 
 
 def tagged_object_list(request, slug, queryset, **kwargs):
     if callable(queryset):
         queryset = queryset()
     kwargs["slug"] = slug
     tag_list_view = type(
@@ -18,21 +18,21 @@
 
 
 class TagListMixin:
     tag_suffix = "_tag"
 
     def dispatch(self, request, *args, **kwargs):
         slug = kwargs.pop("slug")
-        self.tag = get_object_or_404(Tag, slug=slug)
+        self.tag = get_object_or_404(ModelTag, slug=slug)
         return super().dispatch(request, *args, **kwargs)
 
     def get_queryset(self, **kwargs):
         qs = super().get_queryset(**kwargs)
         return qs.filter(
-            pk__in=TaggedItem.objects.filter(
+            pk__in=ModelTagIntFk.objects.filter(
                 tag=self.tag,
                 content_type=ContentType.objects.get_for_model(qs.model),
             ).values_list("object_id", flat=True)
         )
 
     def get_template_names(self):
         if self.tag_suffix:
```

### Comparing `django-tag-fields-4.0.2/tests/forms.py` & `django-tag-fields-4.1.0/tests/forms.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tests/models.py` & `django-tag-fields-4.1.0/tests/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import uuid
 
 from django.db import models
 
-from tag_fields.managers import TaggableManager
+from tag_fields.managers import ModelTagsManager
 from tag_fields.models import (
     GenericFKTaggedItemThroughBase,
     IntegerFKTaggedItemThroughBase,
     UUIDFKTaggedItemThroughBase,
     ThroughTableBase,
-    Tag,
+    ModelTag,
     TagBase,
-    TaggedItem,
+    ModelTagIntFk,
     TaggedItemThroughBase,
 )
 
 
 # base test model
 class TestModel(models.Model):
-    tags = TaggableManager()
+    tags = ModelTagsManager()
 
 
 # Ensure that two TaggableManagers with custom through model are allowed.
 class Through1(TaggedItemThroughBase):
     content_object = models.ForeignKey(
         "MultipleTags", on_delete=models.CASCADE
     )
@@ -30,44 +30,44 @@
 class Through2(TaggedItemThroughBase):
     content_object = models.ForeignKey(
         "MultipleTags", on_delete=models.CASCADE
     )
 
 
 class MultipleTags(models.Model):
-    tags1 = TaggableManager(through=Through1, related_name="tags1")
-    tags2 = TaggableManager(through=Through2, related_name="tags2")
+    tags1 = ModelTagsManager(through=Through1, related_name="tags1")
+    tags2 = ModelTagsManager(through=Through2, related_name="tags2")
 
 
 # Ensure that two TaggableManagers with GFK via different through
 # models are allowed.
 class ThroughGFK(IntegerFKTaggedItemThroughBase):
     tag = models.ForeignKey(
-        Tag, related_name="tagged_items", on_delete=models.CASCADE
+        ModelTag, related_name="tagged_items", on_delete=models.CASCADE
     )
 
 
 class MultipleTagsGFK(models.Model):
-    tags1 = TaggableManager(related_name="tagsgfk1")
-    tags2 = TaggableManager(through=ThroughGFK, related_name="tagsgfk2")
+    tags1 = ModelTagsManager(related_name="tagsgfk1")
+    tags2 = ModelTagsManager(through=ThroughGFK, related_name="tagsgfk2")
 
 
 class BlankTagModel(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(blank=True)
+    tags = ModelTagsManager(blank=True)
 
     def __str__(self):
         return self.name
 
 
 class Food(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager()
+    tags = ModelTagsManager()
 
     def __str__(self):
         return self.name
 
 
 class BaseFood(models.Model):
     name = models.CharField(max_length=50)
@@ -84,24 +84,24 @@
     )
 
     class Meta:
         unique_together = [["content_object", "tag"]]
 
 
 class MultiInheritanceFood(BaseFood):
-    tags = TaggableManager(through=MultiInheritanceLazyResolutionFoodTag)
+    tags = ModelTagsManager(through=MultiInheritanceLazyResolutionFoodTag)
 
     def __str__(self):
         return self.name
 
 
 class Pet(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager()
+    tags = ModelTagsManager()
 
     def __str__(self):
         return self.name
 
 
 class HousePet(Pet):
     trained = models.BooleanField(default=False)
@@ -120,24 +120,24 @@
 class TaggedPet(TaggedItemThroughBase):
     content_object = models.ForeignKey("DirectPet", on_delete=models.CASCADE)
 
 
 class DirectFood(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through="TaggedFood")
+    tags = ModelTagsManager(through="TaggedFood")
 
     def __str__(self):
         return self.name
 
 
 class DirectPet(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through=TaggedPet)
+    tags = ModelTagsManager(through=TaggedPet)
 
     def __str__(self):
         return self.name
 
 
 class DirectHousePet(DirectPet):
     trained = models.BooleanField(default=False)
@@ -176,24 +176,24 @@
     created_by = models.CharField(max_length=50)
     created_dt = models.DateTimeField(auto_now_add=True)
 
 
 class DirectTrackedFood(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through=TaggedTrackedFood)
+    tags = ModelTagsManager(through=TaggedTrackedFood)
 
     def __str__(self):
         return self.name
 
 
 class DirectTrackedPet(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through=TaggedTrackedPet)
+    tags = ModelTagsManager(through=TaggedTrackedPet)
 
     def __str__(self):
         return self.name
 
 
 class DirectTrackedHousePet(DirectTrackedPet):
     trained = models.BooleanField(default=False)
@@ -218,24 +218,24 @@
 
     class Meta:
         unique_together = [["content_object", "tag"]]
 
 
 class DirectCustomPKFood(models.Model):
     name = models.CharField(max_length=50, primary_key=True)
-    tags = TaggableManager(through=TaggedCustomPKFood)
+    tags = ModelTagsManager(through=TaggedCustomPKFood)
 
     def __str__(self):
         return self.name
 
 
 class DirectCustomPKPet(models.Model):
     name = models.CharField(max_length=50, primary_key=True)
 
-    tags = TaggableManager(through=TaggedCustomPKPet)
+    tags = ModelTagsManager(through=TaggedCustomPKPet)
 
     def __str__(self):
         return self.name
 
 
 class DirectCustomPKHousePet(DirectCustomPKPet):
     trained = models.BooleanField(default=False)
@@ -250,24 +250,24 @@
     class Meta:
         unique_together = [["object_id", "tag"]]
 
 
 class CustomPKFood(models.Model):
     name = models.CharField(max_length=50, primary_key=True)
 
-    tags = TaggableManager(through=TaggedCustomPK)
+    tags = ModelTagsManager(through=TaggedCustomPK)
 
     def __str__(self):
         return self.name
 
 
 class CustomPKPet(models.Model):
     name = models.CharField(max_length=50, primary_key=True)
 
-    tags = TaggableManager(through=TaggedCustomPK)
+    tags = ModelTagsManager(through=TaggedCustomPK)
 
     def __str__(self):
         return self.name
 
 
 class CustomPKHousePet(CustomPKPet):
     trained = models.BooleanField(default=False)
@@ -289,35 +289,35 @@
     class Meta:
         unique_together = [["content_type", "object_id", "tag"]]
 
 
 class OfficialFood(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through=OfficialThroughModel)
+    tags = ModelTagsManager(through=OfficialThroughModel)
 
     def __str__(self):
         return self.name
 
 
 class OfficialPet(models.Model):
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through=OfficialThroughModel)
+    tags = ModelTagsManager(through=OfficialThroughModel)
 
     def __str__(self):
         return self.name
 
 
 class OfficialHousePet(OfficialPet):
     trained = models.BooleanField(default=False)
 
 
 class Media(models.Model):
-    tags = TaggableManager()
+    tags = ModelTagsManager()
 
     class Meta:
         abstract = True
 
 
 class Photo(Media):
     pass
@@ -328,61 +328,61 @@
 
 
 class ProxyPhoto(Photo):
     class Meta:
         proxy = True
 
 
-class ArticleTag(Tag):
+class ArticleTag(ModelTag):
     class Meta:
         proxy = True
 
     def slugify(self, tag, i=None):
         slug = "category-%s" % tag.lower()
 
         if i is not None:
             slug += "-%d" % i
         return slug
 
 
-class ArticleTaggedItem(TaggedItem):
+class ArticleTaggedItem(ModelTagIntFk):
     class Meta:
         proxy = True
 
     @classmethod
     def tag_model(self):
         return ArticleTag
 
 
 class Article(models.Model):
     title = models.CharField(max_length=100)
 
-    tags = TaggableManager(through=ArticleTaggedItem)
+    tags = ModelTagsManager(through=ArticleTaggedItem)
 
 
 class CustomManager(models.Model):
     class Foo:
         def __init__(*args, **kwargs):
             pass
 
-    tags = TaggableManager(manager=Foo)
+    tags = ModelTagsManager(manager=Foo)
 
 
 class Parent(models.Model):
-    tags = TaggableManager()
+    tags = ModelTagsManager()
 
 
 class Child(Parent):
     pass
 
 
 class UUIDFood(models.Model):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     name = models.CharField(max_length=50)
-    tags = TaggableManager(through="UUIDTaggedItem")
+    tags = ModelTagsManager(through="UUIDTaggedItem")
 
     created_at = models.DateTimeField(auto_now_add=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
@@ -391,15 +391,15 @@
         ordering = ["created_at"]
 
 
 class UUIDPet(models.Model):
     id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
     name = models.CharField(max_length=50)
 
-    tags = TaggableManager(through="UUIDTaggedItem")
+    tags = ModelTagsManager(through="UUIDTaggedItem")
     created_at = models.DateTimeField(auto_now_add=True)
 
     def __str__(self):
         return self.name
 
     class Meta:
         # With a UUIDField pk, objects are not always ordered by creation time.
@@ -428,12 +428,12 @@
 
 # Exists to verify system check failure.
 # tests.Name.tags: (fields.E303) Reverse query name for 'Name.tags' clashes
 # with field name 'Tag.name'.
 # 	HINT: Rename field 'Tag.name', or add/change a related_name argument to
 # the definition for field 'Name.tags'.
 class Name(models.Model):
-    tags = TaggableManager(related_name="a_unique_related_name")
+    tags = ModelTagsManager(related_name="a_unique_related_name")
 
 
 class OrderedModel(models.Model):
-    tags = TaggableManager(ordering=["name"])
+    tags = ModelTagsManager(ordering=["name"])
```

### Comparing `django-tag-fields-4.0.2/tests/settings.py` & `django-tag-fields-4.1.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tests/test_admin.py` & `django-tag-fields-4.1.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tests/test_forms.py` & `django-tag-fields-4.1.0/tests/test_forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django import forms
 from django.test import TestCase
 from django.test.utils import override_settings
 
 from tag_fields.forms import TagField
-from tag_fields.models import Tag
+from tag_fields.models import ModelTag
 
 
 def _test_parse_tags(tagstring):
     if "," in tagstring:
         return tagstring.split(",")
     else:
         raise ValueError()
@@ -37,24 +37,27 @@
         self.assertTrue(form.is_valid())
         self.assertFalse(form.has_changed())
 
     def test_should_return_True_if_form_has_changed(self):
         class TestForm(forms.Form):
             tag = TagField()
 
-        form = TestForm(initial={"tag": [Tag(name="a")]}, data={"tag": ["b"]})
+        form = TestForm(
+            initial={"tag": [ModelTag(name="a")]}, data={"tag": ["b"]}
+        )
 
         self.assertTrue(form.has_changed())
 
     def test_should_return_False_if_form_has_not_changed(self):
         class TestForm(forms.Form):
             tag = TagField()
 
         form = TestForm(
-            initial={"tag": [Tag(name="foo-bar")]}, data={"tag": ["foo-bar"]}
+            initial={"tag": [ModelTag(name="foo-bar")]},
+            data={"tag": ["foo-bar"]},
         )
 
         self.assertFalse(form.has_changed())
 
     def test_should_return_False_if_not_provided(self):
         class TestForm(forms.Form):
             tag = TagField()
```

### Comparing `django-tag-fields-4.0.2/tests/test_models.py` & `django-tag-fields-4.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tests/test_serializers.py` & `django-tag-fields-4.1.0/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tests/test_utils.py` & `django-tag-fields-4.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/tests/tests.py` & `django-tag-fields-4.1.0/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from django.core import serializers
 from django.core.exceptions import ValidationError
 from django.core.management import call_command
 from django.db import IntegrityError, connection, models
 from django.test import RequestFactory, SimpleTestCase, TestCase
 from django.test.utils import override_settings
 
-from tag_fields.managers import TaggableManager, _TaggableManager
-from tag_fields.models import Tag, TaggedItem
+from tag_fields.managers import ModelTagsManager, _TaggableManager
+from tag_fields.models import ModelTag, ModelTagIntFk
 from tag_fields.utils import edit_string_for_tags, parse_tags
 from tag_fields.views import tagged_object_list
 
 from .forms import (
     BlankTagForm,
     CustomPKFoodForm,
     DirectCustomPKFoodForm,
@@ -75,15 +75,15 @@
             got.sort()
             tags.sort()
         self.assertEqual(got, tags)
 
 
 class TagModelTestCase(BaseTaggingTestCase):
     food_model = Food
-    tag_model = Tag
+    tag_model = ModelTag
 
     def test_unique_slug(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("Red", "red")
 
     def test_update(self):
         special = self.tag_model.objects.create(name="special")
@@ -142,25 +142,25 @@
         self.assertEqual(apple.tags.count(), 4)
         self.assertEqual(apple.tags.filter(official=True).count(), 2)
         self.assertEqual(apple.tags.filter(official=False).count(), 2)
 
 
 class TagModelDirectTestCase(TagModelTestCase):
     food_model = DirectFood
-    tag_model = Tag
+    tag_model = ModelTag
 
 
 class TagModelDirectCustomPKTestCase(TagModelTestCase):
     food_model = DirectCustomPKFood
-    tag_model = Tag
+    tag_model = ModelTag
 
 
 class TagModelCustomPKTestCase(TagModelTestCase):
     food_model = CustomPKFood
-    tag_model = Tag
+    tag_model = ModelTag
 
 
 class TagModelOfficialTestCase(TagModelTestCase):
     food_model = OfficialFood
     tag_model = OfficialTag
 
 
@@ -170,16 +170,16 @@
 
 
 class TaggableManagerTestCase(BaseTaggingTestCase):
     food_model = Food
     multi_inheritance_food_model = MultiInheritanceFood
     pet_model = Pet
     housepet_model = HousePet
-    taggeditem_model = TaggedItem
-    tag_model = Tag
+    taggeditem_model = ModelTagIntFk
+    tag_model = ModelTag
 
     def setUp(self):
         super().setUp()
         ContentType.objects.clear_cache()
 
     def test_add_tag(self):
         apple = self.food_model.objects.create(name="apple")
@@ -788,15 +788,15 @@
             }
             self.assertEqual(
                 foods, {"orange": {"2", "4"}, "apple": {"1", "2"}}
             )
 
     def test_internal_type_is_manytomany(self):
         self.assertEqual(
-            TaggableManager().get_internal_type(), "ManyToManyField"
+            ModelTagsManager().get_internal_type(), "ManyToManyField"
         )
 
     def test_prefetch_no_extra_join(self):
         apple = self.food_model.objects.create(name="apple")
         apple.tags.add("1", "2")
         with self.assertNumQueries(2):
             list(self.food_model.objects.prefetch_related("tags").all())
@@ -1095,27 +1095,27 @@
             self.assertFormRenders(
                 f,
                 """<tr><th><label for="id_name">Name:</label></th><td><input id="id_name" type="text" name="name" value="apple" maxlength="50" %(required)s /></td></tr>
     <tr><th><label for="id_tags">Tags:</label></th><td><input type="text" name="tags" value="&quot;has space&quot;, &quot;has,comma&quot;, delicious, green, red, yummy" id="id_tags" %(required)s /><br />%(help_start)sA comma-separated list of tags.%(help_stop)s</td></tr>""",
             )
 
     def test_formfield(self):
-        tm = TaggableManager(
+        tm = ModelTagsManager(
             verbose_name="categories",
             help_text="Add some categories",
             blank=True,
         )
         ff = tm.formfield()
         self.assertEqual(ff.label, "Categories")
         self.assertEqual(ff.help_text, "Add some categories")
         self.assertEqual(ff.required, False)
 
         self.assertEqual(ff.clean(""), [])
 
-        tm = TaggableManager()
+        tm = ModelTagsManager()
         ff = tm.formfield()
         self.assertRaises(ValidationError, ff.clean, "")
 
     def test_form_changed_data(self):
         # new food, blank tag
         pear = self.food_model()
         request = {"name": "pear", "tags": ""}
@@ -1297,17 +1297,17 @@
         self.assertEqual(parse_tags('",",",",",",","'), [","])
         self.assertEqual(
             parse_tags('a-one "a-two" and "a-three'),
             ["a-one", "a-three", "a-two", "and"],
         )
 
     def test_recreation_of_tag_list_string_representations(self):
-        plain = Tag(name="plain")
-        spaces = Tag(name="spa ces")
-        comma = Tag(name="com,ma")
+        plain = ModelTag(name="plain")
+        spaces = ModelTag(name="spa ces")
+        comma = ModelTag(name="com,ma")
         self.assertEqual(edit_string_for_tags([plain]), "plain")
         self.assertEqual(
             edit_string_for_tags([plain, spaces]), '"spa ces", plain'
         )
         self.assertEqual(
             edit_string_for_tags([plain, spaces, comma]),
             '"com,ma", "spa ces", plain',
@@ -1331,26 +1331,28 @@
             ["Cued Speech", "dictionary"],
         )
 
     @override_settings(
         TAGS_GET_STRING_FROM_TAGS="tests.custom_parser.comma_joiner"
     )
     def test_custom_comma_joiner(self):
-        a = Tag(name="Cued Speech")
-        b = Tag(name="transliterator")
+        a = ModelTag(name="Cued Speech")
+        b = ModelTag(name="transliterator")
         self.assertEqual(
             edit_string_for_tags([a, b]), "Cued Speech, transliterator"
         )
 
 
 class DeconstructTestCase(SimpleTestCase):
     def test_deconstruct_kwargs_kept(self):
-        instance = TaggableManager(through=OfficialThroughModel, to="dummy.To")
+        instance = ModelTagsManager(
+            through=OfficialThroughModel, to="dummy.To"
+        )
         name, path, args, kwargs = instance.deconstruct()
-        new_instance = TaggableManager(*args, **kwargs)
+        new_instance = ModelTagsManager(*args, **kwargs)
         self.assertEqual(
             "tests.OfficialThroughModel", new_instance.remote_field.through
         )
         self.assertEqual("dummy.To", new_instance.remote_field.model)
 
 
 class InheritedPrefetchTests(TestCase):
@@ -1401,21 +1403,21 @@
         self.assertNotIn(self.strawberry, response.context_data["object_list"])
 
 
 class RelatedNameTests(TestCase):
     def test_default_related_name(self):
         food = Food.objects.create(name="apple")
         food.tags.add("green")
-        tag = Tag.objects.get(food=food.pk)
+        tag = ModelTag.objects.get(food=food.pk)
         self.assertEqual(tag.name, "green")
 
     def test_custom_related_name(self):
         name = Name.objects.create()
         name.tags.add("foo")
-        tag = Tag.objects.get(a_unique_related_name=name.pk)
+        tag = ModelTag.objects.get(a_unique_related_name=name.pk)
         self.assertEqual(tag.name, "foo")
 
 
 class OrderedTagsTest(TestCase):
     def test_added_tags_are_returned_ordered(self):
         obj = OrderedModel.objects.create()
         obj.tags.add("green", "red", "orange", "yellow", "blue")
```

### Comparing `django-tag-fields-4.0.2/tox.ini` & `django-tag-fields-4.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `django-tag-fields-4.0.2/PKG-INFO` & `django-tag-fields-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tag-fields
-Version: 4.0.2
+Version: 4.1.0
 Summary: Add field tags to a Django project
 Keywords: Django,django,django tagging
 Author-email: Alex Gaynor <alex.gaynor@gmail.com>
 Maintainer-email: Mark Sevelj <mark.sevelj@dunwright.com.au>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 1 - Planning
```

