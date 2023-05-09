# Comparing `tmp/django-wm-4.0.1.dev4.tar.gz` & `tmp/django-wm-4.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-wm-4.0.1.dev4.tar", last modified: Wed Dec 21 22:20:59 2022, max compression
+gzip compressed data, was "django-wm-4.1.0.dev0.tar", last modified: Tue May  9 17:16:22 2023, max compression
```

## Comparing `django-wm-4.0.1.dev4.tar` & `django-wm-4.1.0.dev0.tar`

### file list

```diff
@@ -1,127 +1,133 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.227443 django-wm-4.0.1.dev4/
--rwxrw-r-x   0 michael   (1000) michael   (1000)    35149 2022-01-27 11:41:47.000000 django-wm-4.0.1.dev4/LICENSE
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2902 2022-12-21 22:20:59.227567 django-wm-4.0.1.dev4/PKG-INFO
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2085 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.175727 django-wm-4.0.1.dev4/django_wm.egg-info/
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2902 2022-12-21 22:20:59.000000 django-wm-4.0.1.dev4/django_wm.egg-info/PKG-INFO
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3675 2022-12-21 22:20:59.000000 django-wm-4.0.1.dev4/django_wm.egg-info/SOURCES.txt
--rwxrw-r-x   0 michael   (1000) michael   (1000)        1 2022-12-21 22:20:59.000000 django-wm-4.0.1.dev4/django_wm.egg-info/dependency_links.txt
--rwxrw-r-x   0 michael   (1000) michael   (1000)      111 2022-12-21 22:20:59.000000 django-wm-4.0.1.dev4/django_wm.egg-info/requires.txt
--rwxrw-r-x   0 michael   (1000) michael   (1000)        9 2022-12-21 22:20:59.000000 django-wm-4.0.1.dev4/django_wm.egg-info/top_level.txt
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.180944 django-wm-4.0.1.dev4/mentions/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       78 2022-12-21 22:20:27.000000 django-wm-4.0.1.dev4/mentions/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3493 2022-10-25 18:47:15.000000 django-wm-4.0.1.dev4/mentions/admin.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)       91 2022-11-16 17:49:32.000000 django-wm-4.0.1.dev4/mentions/apps.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      583 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/config.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      288 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/contract.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2222 2022-12-21 19:08:23.000000 django-wm-4.0.1.dev4/mentions/exceptions.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.181950 django-wm-4.0.1.dev4/mentions/forms/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       52 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/forms/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      224 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/forms/submit_webmention.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.184591 django-wm-4.0.1.dev4/mentions/helpers/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/helpers/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2032 2022-12-21 21:58:13.000000 django-wm-4.0.1.dev4/mentions/helpers/resolution.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.185163 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.188382 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      160 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2096 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/proxy.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3484 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/resolution.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     7078 2022-12-21 22:18:09.000000 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/urls.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      635 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/util.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      849 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/types.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5883 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/urls.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      788 2022-11-30 17:25:42.000000 django-wm-4.0.1.dev4/mentions/helpers/util.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.188937 django-wm-4.0.1.dev4/mentions/management/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.0.1.dev4/mentions/management/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.190548 django-wm-4.0.1.dev4/mentions/management/commands/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.0.1.dev4/mentions/management/commands/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1763 2022-12-21 19:08:23.000000 django-wm-4.0.1.dev4/mentions/management/commands/mentions_reverify.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1073 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/management/commands/pending_mentions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      296 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/microformats.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.191586 django-wm-4.0.1.dev4/mentions/middleware/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       65 2022-10-26 15:53:11.000000 django-wm-4.0.1.dev4/mentions/middleware/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      739 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/middleware/webmention_head_middleware.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.198785 django-wm-4.0.1.dev4/mentions/migrations/
--rwxrw-r-x   0 michael   (1000) michael   (1000)     8690 2022-02-03 11:01:16.000000 django-wm-4.0.1.dev4/mentions/migrations/0001_initial.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1626 2022-10-27 12:03:01.000000 django-wm-4.0.1.dev4/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      664 2022-03-26 13:17:25.000000 django-wm-4.0.1.dev4/mentions/migrations/0003_alter_simplemention_published_and_more.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1349 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3250 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0005_rebuild_pending_models_with_constraints.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2853 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1076 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0007_dashboardpermissionproxy.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      361 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0008_alter_webmention_options.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      471 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0009_alter_outgoingwebmentionstatus_options.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      781 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      539 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)    16916 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/migrations/0012_alter_hcard_options_and_more.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-01-27 11:41:47.000000 django-wm-4.0.1.dev4/mentions/migrations/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.202555 django-wm-4.0.1.dev4/mentions/models/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      271 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/models/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      291 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/models/base.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2993 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/models/hcard.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.204900 django-wm-4.0.1.dev4/mentions/models/mixins/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/models/mixins/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     4541 2022-11-28 11:32:39.000000 django-wm-4.0.1.dev4/mentions/models/mixins/mentionable.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3372 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/models/mixins/quotable.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2879 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/models/mixins/retryable.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2522 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/models/outgoing_status.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2169 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/models/pending.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.206043 django-wm-4.0.1.dev4/mentions/models/proxy/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/models/proxy/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      386 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/models/proxy/permissions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      649 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/models/simple_mention.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1677 2022-12-14 18:33:44.000000 django-wm-4.0.1.dev4/mentions/models/webmention.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     7145 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/options.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      956 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/permissions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5028 2022-12-21 21:49:36.000000 django-wm-4.0.1.dev4/mentions/resolution.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.207594 django-wm-4.0.1.dev4/mentions/tasks/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      178 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/tasks/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1333 2022-10-12 15:23:17.000000 django-wm-4.0.1.dev4/mentions/tasks/celeryproxy.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.211171 django-wm-4.0.1.dev4/mentions/tasks/incoming/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       49 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1138 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/local.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.213293 django-wm-4.0.1.dev4/mentions/tasks/incoming/parsing/
--rwxrw-r-x   0 michael   (1000) michael   (1000)       90 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/parsing/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3496 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/parsing/hcard.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      981 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/parsing/post_type.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     4288 2022-12-21 19:08:23.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/process.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     3023 2022-12-21 18:41:03.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/remote.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2557 2022-12-21 19:08:23.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/reverify.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      848 2022-12-21 19:08:23.000000 django-wm-4.0.1.dev4/mentions/tasks/incoming/status.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.215963 django-wm-4.0.1.dev4/mentions/tasks/outgoing/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      125 2022-10-06 19:42:52.000000 django-wm-4.0.1.dev4/mentions/tasks/outgoing/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2483 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/tasks/outgoing/local.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.217338 django-wm-4.0.1.dev4/mentions/tasks/outgoing/parsing/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      159 2022-10-06 19:42:52.000000 django-wm-4.0.1.dev4/mentions/tasks/outgoing/parsing/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1893 2022-10-06 19:42:52.000000 django-wm-4.0.1.dev4/mentions/tasks/outgoing/parsing/webmention_endpoint.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2351 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/tasks/outgoing/process.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5224 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/tasks/outgoing/remote.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     5707 2022-10-25 18:47:15.000000 django-wm-4.0.1.dev4/mentions/tasks/scheduling.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.170581 django-wm-4.0.1.dev4/mentions/templates/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.219208 django-wm-4.0.1.dev4/mentions/templates/mentions/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      261 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/templates/mentions/webmention-accepted.html
--rwxrw-r-x   0 michael   (1000) michael   (1000)     8071 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/templates/mentions/webmention-dashboard.html
--rwxrw-r-x   0 michael   (1000) michael   (1000)      585 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/templates/mentions/webmention-submit-manual.html
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.221305 django-wm-4.0.1.dev4/mentions/templatetags/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-03 11:01:16.000000 django-wm-4.0.1.dev4/mentions/templatetags/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1766 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/templatetags/webmention_dashboard.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      332 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/mentions/templatetags/webmention_endpoint.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1317 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/templatetags/webmentions.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      942 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/urls.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.223376 django-wm-4.0.1.dev4/mentions/util/
--rwxrw-r-x   0 michael   (1000) michael   (1000)      166 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/util/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      547 2022-10-06 19:42:52.000000 django-wm-4.0.1.dev4/mentions/util/html.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      559 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/util/requests.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      934 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/util/url.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-12-21 22:20:59.227000 django-wm-4.0.1.dev4/mentions/views/
--rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/__init__.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      409 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/contract.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1338 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/dashboard.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     2355 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/retrieve.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1810 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/serialize.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1804 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/submit.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      486 2022-11-25 16:03:29.000000 django-wm-4.0.1.dev4/mentions/views/view_names.py
--rwxrw-r-x   0 michael   (1000) michael   (1000)      112 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/pyproject.toml
--rwxrw-r-x   0 michael   (1000) michael   (1000)     1077 2022-12-21 22:20:59.228308 django-wm-4.0.1.dev4/setup.cfg
--rwxrw-r-x   0 michael   (1000) michael   (1000)       69 2022-09-29 19:47:26.000000 django-wm-4.0.1.dev4/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.496719 django-wm-4.1.0.dev0/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)    35149 2022-01-27 11:41:47.000000 django-wm-4.1.0.dev0/LICENSE
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2926 2023-05-09 17:16:22.496848 django-wm-4.1.0.dev0/PKG-INFO
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2085 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.415917 django-wm-4.1.0.dev0/django_wm.egg-info/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2926 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/PKG-INFO
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3884 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/SOURCES.txt
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        1 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/dependency_links.txt
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/requires.txt
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        9 2023-05-09 17:16:22.000000 django-wm-4.1.0.dev0/django_wm.egg-info/top_level.txt
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.423068 django-wm-4.1.0.dev0/mentions/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       78 2023-05-08 10:58:46.000000 django-wm-4.1.0.dev0/mentions/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     4091 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/admin.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       91 2022-11-16 17:49:32.000000 django-wm-4.1.0.dev0/mentions/apps.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      583 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/config.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      295 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/context_processors.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      365 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/contract.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2222 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/exceptions.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.425026 django-wm-4.1.0.dev0/mentions/forms/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       52 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/forms/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      224 2023-05-07 14:24:34.000000 django-wm-4.1.0.dev0/mentions/forms/submit_webmention.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.431152 django-wm-4.1.0.dev0/mentions/helpers/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/helpers/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1819 2022-12-22 15:35:08.000000 django-wm-4.1.0.dev0/mentions/helpers/resolution.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.432066 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.436609 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      160 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2096 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/proxy.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3484 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/resolution.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     6964 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/urls.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      635 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/util.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      849 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/types.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5883 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/urls.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      788 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/helpers/util.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.437240 django-wm-4.1.0.dev0/mentions/management/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.1.0.dev0/mentions/management/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.440226 django-wm-4.1.0.dev0/mentions/management/commands/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-05 17:15:41.000000 django-wm-4.1.0.dev0/mentions/management/commands/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1030 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/management/commands/mentions_pending.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2124 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/management/commands/mentions_reverify.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      143 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/management/commands/pending_mentions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      296 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/microformats.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.441361 django-wm-4.1.0.dev0/mentions/middleware/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       65 2022-10-26 15:53:11.000000 django-wm-4.1.0.dev0/mentions/middleware/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      739 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/middleware/webmention_head_middleware.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.455308 django-wm-4.1.0.dev0/mentions/migrations/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     8690 2022-02-03 11:01:16.000000 django-wm-4.1.0.dev0/mentions/migrations/0001_initial.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1626 2022-10-27 12:03:01.000000 django-wm-4.1.0.dev0/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      664 2022-03-26 13:17:25.000000 django-wm-4.1.0.dev0/mentions/migrations/0003_alter_simplemention_published_and_more.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1349 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3250 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0005_rebuild_pending_models_with_constraints.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2853 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1076 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0007_dashboardpermissionproxy.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      361 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0008_alter_webmention_options.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      471 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0009_alter_outgoingwebmentionstatus_options.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      781 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      539 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)    16916 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/migrations/0012_alter_hcard_options_and_more.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      430 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/migrations/0013_webmention_has_been_read.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-01-27 11:41:47.000000 django-wm-4.1.0.dev0/mentions/migrations/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.461822 django-wm-4.1.0.dev0/mentions/models/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      271 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      291 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/base.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2993 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/hcard.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.463030 django-wm-4.1.0.dev0/mentions/models/managers/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/models/managers/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      984 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/models/managers/webmention.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.466191 django-wm-4.1.0.dev0/mentions/models/mixins/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      137 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/mixins/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     4541 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/models/mixins/mentionable.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3372 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/mixins/quotable.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2879 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/mixins/retryable.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2522 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/outgoing_status.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2169 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/models/pending.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.467615 django-wm-4.1.0.dev0/mentions/models/proxy/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       50 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/proxy/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      386 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/proxy/permissions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      649 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/models/simple_mention.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1880 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/models/webmention.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     6958 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/options.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1178 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/permissions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5118 2023-05-09 16:46:26.000000 django-wm-4.1.0.dev0/mentions/resolution.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.469782 django-wm-4.1.0.dev0/mentions/tasks/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      178 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/tasks/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1333 2022-10-12 15:23:17.000000 django-wm-4.1.0.dev0/mentions/tasks/celeryproxy.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.475664 django-wm-4.1.0.dev0/mentions/tasks/incoming/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       49 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1138 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/local.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.478332 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       90 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3496 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/hcard.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      981 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/post_type.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     4288 2023-05-07 14:23:52.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/process.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     3023 2023-05-07 14:24:22.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/remote.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2557 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/reverify.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      848 2023-05-07 13:24:39.000000 django-wm-4.1.0.dev0/mentions/tasks/incoming/status.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.481712 django-wm-4.1.0.dev0/mentions/tasks/outgoing/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      125 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2483 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/local.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.483137 django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      159 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1893 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/webmention_endpoint.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2351 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/process.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5224 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/tasks/outgoing/remote.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     5707 2023-05-07 14:24:27.000000 django-wm-4.1.0.dev0/mentions/tasks/scheduling.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.410485 django-wm-4.1.0.dev0/mentions/templates/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.485443 django-wm-4.1.0.dev0/mentions/templates/mentions/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      261 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-accepted.html
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     8130 2023-05-09 16:46:35.000000 django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-dashboard.html
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      585 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-submit-manual.html
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.488167 django-wm-4.1.0.dev0/mentions/templatetags/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-02-03 11:01:16.000000 django-wm-4.1.0.dev0/mentions/templatetags/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1766 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/templatetags/webmention_dashboard.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      332 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/mentions/templatetags/webmention_endpoint.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1317 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/templatetags/webmentions.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      942 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/urls.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.490590 django-wm-4.1.0.dev0/mentions/util/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      166 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/util/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      547 2022-10-06 19:42:52.000000 django-wm-4.1.0.dev0/mentions/util/html.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      559 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/util/requests.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      934 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/util/url.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-05-09 17:16:22.496248 django-wm-4.1.0.dev0/mentions/views/
+-rwxrw-r-x   0 michael   (1000) michael   (1000)        0 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/__init__.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      409 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/contract.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1338 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/dashboard.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     2355 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/retrieve.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1810 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/serialize.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1804 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/submit.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      486 2022-11-25 16:03:29.000000 django-wm-4.1.0.dev0/mentions/views/view_names.py
+-rwxrw-r-x   0 michael   (1000) michael   (1000)      112 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/pyproject.toml
+-rwxrw-r-x   0 michael   (1000) michael   (1000)     1104 2023-05-09 17:16:22.497443 django-wm-4.1.0.dev0/setup.cfg
+-rwxrw-r-x   0 michael   (1000) michael   (1000)       69 2022-09-29 19:47:26.000000 django-wm-4.1.0.dev0/setup.py
```

### Comparing `django-wm-4.0.1.dev4/LICENSE` & `django-wm-4.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/PKG-INFO` & `django-wm-4.1.0.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: django-wm
-Version: 4.0.1.dev4
-Summary: Webmention support for Django.
-Home-page: https://beatonma.org/webmentions_tester/
-Author: Michael Beaton
-Author-email: michael@beatonma.org
-License: GPLv3
-Project-URL: Source, https://github.com/beatonma/django-wm
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: celery
-Provides-Extra: test
-License-File: LICENSE
-
 # `django-wm`
 
 [![Tests](https://github.com/beatonma/django-wm/actions/workflows/runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/actions/workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/django-wm.svg)](https://badge.fury.io/py/django-wm)
 
 `django-wm` lets you add [Webmention](https://indieweb.org/Webmention) functionality to your Django project with minimal setup.
```

#### html2text {}

```diff
@@ -1,37 +1,26 @@
-Metadata-Version: 2.1 Name: django-wm Version: 4.0.1.dev4 Summary: Webmention
-support for Django. Home-page: https://beatonma.org/webmentions_tester/ Author:
-Michael Beaton Author-email: michael@beatonma.org License: GPLv3 Project-URL:
-Source, https://github.com/beatonma/django-wm Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
-:: GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: celery
-Provides-Extra: test License-File: LICENSE # `django-wm` [![Tests](https://
-github.com/beatonma/django-wm/actions/workflows/runtests.yml/badge.svg)](https:
-//github.com/beatonma/django-wm/actions/workflows/runtests.yml) [![pypi
-package](https://badge.fury.io/py/django-wm.svg)](https://badge.fury.io/py/
-django-wm) `django-wm` lets you add [Webmention](https://indieweb.org/
-Webmention) functionality to your Django project with minimal setup. ###
-Upgrading Please check the [upgrade guide](https://github.com/beatonma/django-
-wm/wiki/Upgrading) for any breaking changes before upgrading. See the
-[changelog](./CHANGELOG.md) for full details. ### Getting started [Setup
-instructions](https://github.com/beatonma/django-wm/wiki/Guide_Getting-
-started). [Code for an example project](./sample-project). All done? You can
-use the [testing tool](https://beatonma.org/webmentions_tester/) to make sure
-it works. ### Features - Endpoints: - `/webmention`: Receives incoming
-Webmentions from other sites. - `/webmention/get`: Used to retrieve Webmentions
-for a page on your site. e.g. `/webmention/get?url=/my-article` will return any
-received Webmentions that target `/my-article` on your site. ```json5 // /
-webmention/get?url=/my-article { "target_url": "https://my-site.org/my-
-article", "mentions": [ { "hcard": { "name": "Jane Bloggs", "avatar": "https://
-gravatar.com/janebloggs", "homepage": "https://jane-bloggs-example.org" },
-"quote": null, "source_url": "https://jane-bloggs-example.org/some-article",
-"published": "2020-01-17T21:45:24.542Z", "type": "webmention" } ] } ``` -
-`WebmentionHeadMiddleware` adds your `/webmention` endpoint to the headers of
-your pages so that it can be discovered by other sites. - `{%
-webmentions_endpoint %}` template tag to include your `/webmention` endpoint to
-your Django templates
+# `django-wm` [![Tests](https://github.com/beatonma/django-wm/actions/
+workflows/runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/
+actions/workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/
+django-wm.svg)](https://badge.fury.io/py/django-wm) `django-wm` lets you add
+[Webmention](https://indieweb.org/Webmention) functionality to your Django
+project with minimal setup. ### Upgrading Please check the [upgrade guide]
+(https://github.com/beatonma/django-wm/wiki/Upgrading) for any breaking changes
+before upgrading. See the [changelog](./CHANGELOG.md) for full details. ###
+Getting started [Setup instructions](https://github.com/beatonma/django-wm/
+wiki/Guide_Getting-started). [Code for an example project](./sample-project).
+All done? You can use the [testing tool](https://beatonma.org/
+webmentions_tester/) to make sure it works. ### Features - Endpoints: - `/
+webmention`: Receives incoming Webmentions from other sites. - `/webmention/
+get`: Used to retrieve Webmentions for a page on your site. e.g. `/webmention/
+get?url=/my-article` will return any received Webmentions that target `/my-
+article` on your site. ```json5 // /webmention/get?url=/my-article
+{ "target_url": "https://my-site.org/my-article", "mentions": [ { "hcard":
+{ "name": "Jane Bloggs", "avatar": "https://gravatar.com/janebloggs",
+"homepage": "https://jane-bloggs-example.org" }, "quote": null, "source_url":
+"https://jane-bloggs-example.org/some-article", "published": "2020-01-17T21:45:
+24.542Z", "type": "webmention" } ] } ``` - `WebmentionHeadMiddleware` adds your
+`/webmention` endpoint to the headers of your pages so that it can be
+discovered by other sites. - `{% webmentions_endpoint %}` template tag to
+include your `/webmention` endpoint to your Django templates
 HTML element. - `MentionableMixin` enables automatic submission of Webmentions
 to other sites when you mention them in your content.
```

### Comparing `django-wm-4.0.1.dev4/README.md` & `django-wm-4.1.0.dev0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: django-wm
+Version: 4.1.0.dev0
+Summary: Webmention support for Django.
+Home-page: https://beatonma.org/webmentions_tester/
+Author: Michael Beaton
+Author-email: michael@beatonma.org
+License: GPLv3
+Project-URL: Source, https://github.com/beatonma/django-wm
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: celery
+Provides-Extra: test
+Provides-Extra: wagtail
+License-File: LICENSE
+
 # `django-wm`
 
 [![Tests](https://github.com/beatonma/django-wm/actions/workflows/runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/actions/workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/django-wm.svg)](https://badge.fury.io/py/django-wm)
 
 `django-wm` lets you add [Webmention](https://indieweb.org/Webmention) functionality to your Django project with minimal setup.
```

#### html2text {}

```diff
@@ -1,11 +1,22 @@
-# `django-wm` [![Tests](https://github.com/beatonma/django-wm/actions/
-workflows/runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/
-actions/workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/
-django-wm.svg)](https://badge.fury.io/py/django-wm) `django-wm` lets you add
+Metadata-Version: 2.1 Name: django-wm Version: 4.1.0.dev0 Summary: Webmention
+support for Django. Home-page: https://beatonma.org/webmentions_tester/ Author:
+Michael Beaton Author-email: michael@beatonma.org License: GPLv3 Project-URL:
+Source, https://github.com/beatonma/django-wm Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: celery
+Provides-Extra: test Provides-Extra: wagtail License-File: LICENSE # `django-
+wm` [![Tests](https://github.com/beatonma/django-wm/actions/workflows/
+runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/actions/
+workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/django-
+wm.svg)](https://badge.fury.io/py/django-wm) `django-wm` lets you add
 [Webmention](https://indieweb.org/Webmention) functionality to your Django
 project with minimal setup. ### Upgrading Please check the [upgrade guide]
 (https://github.com/beatonma/django-wm/wiki/Upgrading) for any breaking changes
 before upgrading. See the [changelog](./CHANGELOG.md) for full details. ###
 Getting started [Setup instructions](https://github.com/beatonma/django-wm/
 wiki/Guide_Getting-started). [Code for an example project](./sample-project).
 All done? You can use the [testing tool](https://beatonma.org/
```

### Comparing `django-wm-4.0.1.dev4/django_wm.egg-info/PKG-INFO` & `django-wm-4.1.0.dev0/django_wm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-wm
-Version: 4.0.1.dev4
+Version: 4.1.0.dev0
 Summary: Webmention support for Django.
 Home-page: https://beatonma.org/webmentions_tester/
 Author: Michael Beaton
 Author-email: michael@beatonma.org
 License: GPLv3
 Project-URL: Source, https://github.com/beatonma/django-wm
 Classifier: Framework :: Django
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: celery
 Provides-Extra: test
+Provides-Extra: wagtail
 License-File: LICENSE
 
 # `django-wm`
 
 [![Tests](https://github.com/beatonma/django-wm/actions/workflows/runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/actions/workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/django-wm.svg)](https://badge.fury.io/py/django-wm)
 
 `django-wm` lets you add [Webmention](https://indieweb.org/Webmention) functionality to your Django project with minimal setup.
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-Metadata-Version: 2.1 Name: django-wm Version: 4.0.1.dev4 Summary: Webmention
+Metadata-Version: 2.1 Name: django-wm Version: 4.1.0.dev0 Summary: Webmention
 support for Django. Home-page: https://beatonma.org/webmentions_tester/ Author:
 Michael Beaton Author-email: michael@beatonma.org License: GPLv3 Project-URL:
 Source, https://github.com/beatonma/django-wm Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra: celery
-Provides-Extra: test License-File: LICENSE # `django-wm` [![Tests](https://
-github.com/beatonma/django-wm/actions/workflows/runtests.yml/badge.svg)](https:
-//github.com/beatonma/django-wm/actions/workflows/runtests.yml) [![pypi
-package](https://badge.fury.io/py/django-wm.svg)](https://badge.fury.io/py/
-django-wm) `django-wm` lets you add [Webmention](https://indieweb.org/
-Webmention) functionality to your Django project with minimal setup. ###
-Upgrading Please check the [upgrade guide](https://github.com/beatonma/django-
-wm/wiki/Upgrading) for any breaking changes before upgrading. See the
-[changelog](./CHANGELOG.md) for full details. ### Getting started [Setup
-instructions](https://github.com/beatonma/django-wm/wiki/Guide_Getting-
-started). [Code for an example project](./sample-project). All done? You can
-use the [testing tool](https://beatonma.org/webmentions_tester/) to make sure
-it works. ### Features - Endpoints: - `/webmention`: Receives incoming
-Webmentions from other sites. - `/webmention/get`: Used to retrieve Webmentions
-for a page on your site. e.g. `/webmention/get?url=/my-article` will return any
-received Webmentions that target `/my-article` on your site. ```json5 // /
-webmention/get?url=/my-article { "target_url": "https://my-site.org/my-
-article", "mentions": [ { "hcard": { "name": "Jane Bloggs", "avatar": "https://
-gravatar.com/janebloggs", "homepage": "https://jane-bloggs-example.org" },
-"quote": null, "source_url": "https://jane-bloggs-example.org/some-article",
-"published": "2020-01-17T21:45:24.542Z", "type": "webmention" } ] } ``` -
-`WebmentionHeadMiddleware` adds your `/webmention` endpoint to the headers of
-your pages so that it can be discovered by other sites. - `{%
-webmentions_endpoint %}` template tag to include your `/webmention` endpoint to
-your Django templates
+Provides-Extra: test Provides-Extra: wagtail License-File: LICENSE # `django-
+wm` [![Tests](https://github.com/beatonma/django-wm/actions/workflows/
+runtests.yml/badge.svg)](https://github.com/beatonma/django-wm/actions/
+workflows/runtests.yml) [![pypi package](https://badge.fury.io/py/django-
+wm.svg)](https://badge.fury.io/py/django-wm) `django-wm` lets you add
+[Webmention](https://indieweb.org/Webmention) functionality to your Django
+project with minimal setup. ### Upgrading Please check the [upgrade guide]
+(https://github.com/beatonma/django-wm/wiki/Upgrading) for any breaking changes
+before upgrading. See the [changelog](./CHANGELOG.md) for full details. ###
+Getting started [Setup instructions](https://github.com/beatonma/django-wm/
+wiki/Guide_Getting-started). [Code for an example project](./sample-project).
+All done? You can use the [testing tool](https://beatonma.org/
+webmentions_tester/) to make sure it works. ### Features - Endpoints: - `/
+webmention`: Receives incoming Webmentions from other sites. - `/webmention/
+get`: Used to retrieve Webmentions for a page on your site. e.g. `/webmention/
+get?url=/my-article` will return any received Webmentions that target `/my-
+article` on your site. ```json5 // /webmention/get?url=/my-article
+{ "target_url": "https://my-site.org/my-article", "mentions": [ { "hcard":
+{ "name": "Jane Bloggs", "avatar": "https://gravatar.com/janebloggs",
+"homepage": "https://jane-bloggs-example.org" }, "quote": null, "source_url":
+"https://jane-bloggs-example.org/some-article", "published": "2020-01-17T21:45:
+24.542Z", "type": "webmention" } ] } ``` - `WebmentionHeadMiddleware` adds your
+`/webmention` endpoint to the headers of your pages so that it can be
+discovered by other sites. - `{% webmentions_endpoint %}` template tag to
+include your `/webmention` endpoint to your Django templates
 HTML element. - `MentionableMixin` enables automatic submission of Webmentions
 to other sites when you mention them in your content.
```

### Comparing `django-wm-4.0.1.dev4/django_wm.egg-info/SOURCES.txt` & `django-wm-4.1.0.dev0/django_wm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 django_wm.egg-info/dependency_links.txt
 django_wm.egg-info/requires.txt
 django_wm.egg-info/top_level.txt
 mentions/__init__.py
 mentions/admin.py
 mentions/apps.py
 mentions/config.py
+mentions/context_processors.py
 mentions/contract.py
 mentions/exceptions.py
 mentions/microformats.py
 mentions/options.py
 mentions/permissions.py
 mentions/resolution.py
 mentions/urls.py
@@ -30,14 +31,15 @@
 mentions/helpers/thirdparty/wagtail/__init__.py
 mentions/helpers/thirdparty/wagtail/proxy.py
 mentions/helpers/thirdparty/wagtail/resolution.py
 mentions/helpers/thirdparty/wagtail/urls.py
 mentions/helpers/thirdparty/wagtail/util.py
 mentions/management/__init__.py
 mentions/management/commands/__init__.py
+mentions/management/commands/mentions_pending.py
 mentions/management/commands/mentions_reverify.py
 mentions/management/commands/pending_mentions.py
 mentions/middleware/__init__.py
 mentions/middleware/webmention_head_middleware.py
 mentions/migrations/0001_initial.py
 mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py
 mentions/migrations/0003_alter_simplemention_published_and_more.py
@@ -46,22 +48,25 @@
 mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py
 mentions/migrations/0007_dashboardpermissionproxy.py
 mentions/migrations/0008_alter_webmention_options.py
 mentions/migrations/0009_alter_outgoingwebmentionstatus_options.py
 mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py
 mentions/migrations/0011_alter_pendingoutgoingcontent_text.py
 mentions/migrations/0012_alter_hcard_options_and_more.py
+mentions/migrations/0013_webmention_has_been_read.py
 mentions/migrations/__init__.py
 mentions/models/__init__.py
 mentions/models/base.py
 mentions/models/hcard.py
 mentions/models/outgoing_status.py
 mentions/models/pending.py
 mentions/models/simple_mention.py
 mentions/models/webmention.py
+mentions/models/managers/__init__.py
+mentions/models/managers/webmention.py
 mentions/models/mixins/__init__.py
 mentions/models/mixins/mentionable.py
 mentions/models/mixins/quotable.py
 mentions/models/mixins/retryable.py
 mentions/models/proxy/__init__.py
 mentions/models/proxy/permissions.py
 mentions/tasks/__init__.py
```

### Comparing `django-wm-4.0.1.dev4/mentions/admin.py` & `django-wm-4.1.0.dev0/mentions/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,30 +5,41 @@
     HCard,
     OutgoingWebmentionStatus,
     PendingIncomingWebmention,
     PendingOutgoingContent,
     SimpleMention,
     Webmention,
 )
+from mentions.models.managers.webmention import WebmentionQuerySet
 
 RETRYABLEMIXIN_FIELDS = [
     "is_awaiting_retry",
     "last_retry_attempt",
     "retry_attempt_count",
 ]
 
 
 @admin.action(permissions=["change"])
-def approve_webmention(modeladmin, request, queryset):
-    queryset.update(approved=True)
+def mark_webmention_approved(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_approved()
 
 
 @admin.action(permissions=["change"])
-def disapprove_webmention(modeladmin, request, queryset):
-    queryset.update(approved=False)
+def mark_webmention_unapproved(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_unapproved()
+
+
+@admin.action(permissions=["change"])
+def mark_webmention_read(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_read()
+
+
+@admin.action(permissions=["change"])
+def mark_webmention_unread(modeladmin, request, queryset: WebmentionQuerySet):
+    queryset.mark_as_unread()
 
 
 class BaseAdmin(admin.ModelAdmin):
     save_on_top = True
 
 
 @admin.register(SimpleMention)
@@ -50,33 +61,37 @@
     date_hierarchy = "published"
 
 
 class WebmentionModelForm(forms.ModelForm):
     class Meta:
         model = Webmention
         widgets = {
+            "quote": forms.Textarea(attrs={"rows": 3}),
             "notes": forms.Textarea(attrs={"rows": 3}),
         }
         fields = "__all__"
 
 
 @admin.register(Webmention)
 class WebmentionAdmin(QuotableAdmin):
     form = WebmentionModelForm
     readonly_fields = QuotableAdmin.readonly_fields + [
         "content_type",
         "object_id",
     ]
     actions = [
-        approve_webmention,
-        disapprove_webmention,
+        mark_webmention_approved,
+        mark_webmention_unapproved,
+        mark_webmention_read,
+        mark_webmention_unread,
     ]
     list_display = [
         "source_url",
         "target_url",
+        "has_been_read",
         "published",
         "validated",
         "approved",
         "target_object",
     ]
     fieldsets = (
         (
@@ -103,14 +118,15 @@
             },
         ),
         (
             "Metadata",
             {
                 "fields": (
                     "published",
+                    "has_been_read",
                     "approved",
                     "validated",
                     "notes",
                 ),
             },
         ),
     )
```

### Comparing `django-wm-4.0.1.dev4/mentions/config.py` & `django-wm-4.1.0.dev0/mentions/config.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/exceptions.py` & `django-wm-4.1.0.dev0/mentions/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/resolution.py` & `django-wm-4.1.0.dev0/mentions/helpers/resolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from typing import Dict, Optional, Sequence, Set, Tuple, Type
 
 from mentions import contract
 from mentions.helpers.types import (
     MentionableImpl,
     ModelFilter,
     ModelFilterMap,
@@ -12,17 +11,14 @@
 __all__ = [
     "get_model_for_url_by_helper",
 ]
 
 TypeSet = Set[Tuple[UrlKwarg, ModelFilter]]
 
 
-log = logging.getLogger(__name__)
-
-
 def get_model_for_url_by_helper(
     model_class: Type[MentionableImpl],
     urlpattern_args: Sequence,
     urlpattern_kwargs: Dict,
 ) -> Optional[MentionableImpl]:
     """Resolve a model instance from urlpattern kwargs, as configured by
     `mentions_path` or `mentions_re_path` helper functions.
@@ -34,17 +30,14 @@
 
     Returns:
         An instance of `model_class`.
 
     Raises:
         KeyError: If the given urlpattern_kwargs does not contain helper values.
     """
-    log.warning(
-        f"get_model_for_url_by_helper(model_class={model_class}, urlpattern_args={urlpattern_args} urlpattern_kwargs={urlpattern_kwargs})"
-    )
 
     model_filter_map: ModelFilterMap = urlpattern_kwargs.pop(
         contract.URLPATTERNS_MODEL_FILTER_MAP
     )
 
     mapping = unpack_model_filter_map(model_filter_map)
     query = {value: urlpattern_kwargs[key] for key, value in mapping}
```

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/proxy.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/proxy.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/resolution.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/resolution.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/urls.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,18 +75,14 @@
 
         if autopage:
             view_func = autopage_page_resolver(model_class, lookup, view_func)
 
         view_func = annotate_viewfunc(view_func, model_class, lookup)
         path = wagtail_path(view_func, *args, **kwargs)
 
-        log.warning(
-            f"pattern: {pattern} | model_class: {model_class} | lookup: {lookup}"
-        )
-
         return path
 
     return decorator
 
 
 def mentions_wagtail_path(
     pattern: str,
```

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/thirdparty/wagtail/util.py` & `django-wm-4.1.0.dev0/mentions/helpers/thirdparty/wagtail/util.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/types.py` & `django-wm-4.1.0.dev0/mentions/helpers/types.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/urls.py` & `django-wm-4.1.0.dev0/mentions/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/helpers/util.py` & `django-wm-4.1.0.dev0/mentions/helpers/util.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/management/commands/pending_mentions.py` & `django-wm-4.1.0.dev0/mentions/management/commands/mentions_pending.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-import logging
-
 from django.core.management import BaseCommand
 
 from mentions.tasks.scheduling import handle_pending_webmentions
 
 PENDING_TYPE_ALL = "all"
 PENDING_TYPE_INCOMING = "incoming"
 PENDING_TYPE_OUTGOING = "outgoing"
 
 
-log = logging.getLogger(__name__)
-
-
 class Command(BaseCommand):
     def add_arguments(self, parser):
         parser.add_argument(
             "pending_type",
             choices=[PENDING_TYPE_ALL, PENDING_TYPE_INCOMING, PENDING_TYPE_OUTGOING],
             default=PENDING_TYPE_ALL,
             nargs="?",
@@ -26,10 +21,10 @@
         incoming = pending_type == PENDING_TYPE_INCOMING
         outgoing = pending_type == PENDING_TYPE_OUTGOING
 
         if pending_type == PENDING_TYPE_ALL:
             incoming = True
             outgoing = True
 
-        log.info(f"Checking for pending webmentions [{pending_type}]...")
+        self.stdout.write(f"Checking for pending webmentions [{pending_type}]...")
 
         handle_pending_webmentions(incoming=incoming, outgoing=outgoing)
```

### Comparing `django-wm-4.0.1.dev4/mentions/middleware/webmention_head_middleware.py` & `django-wm-4.1.0.dev0/mentions/middleware/webmention_head_middleware.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0001_initial.py` & `django-wm-4.1.0.dev0/mentions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py` & `django-wm-4.1.0.dev0/mentions/migrations/0002_pendingincomingwebmention_pendingoutgoingcontent.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0003_alter_simplemention_published_and_more.py` & `django-wm-4.1.0.dev0/mentions/migrations/0003_alter_simplemention_published_and_more.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py` & `django-wm-4.1.0.dev0/mentions/migrations/0004_simplemention_post_type_webmention_post_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0005_rebuild_pending_models_with_constraints.py` & `django-wm-4.1.0.dev0/mentions/migrations/0005_rebuild_pending_models_with_constraints.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py` & `django-wm-4.1.0.dev0/mentions/migrations/0006_add_retryablemixin_pendingincomingwebmention_outgoingwebmentionstatus.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0007_dashboardpermissionproxy.py` & `django-wm-4.1.0.dev0/mentions/migrations/0007_dashboardpermissionproxy.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py` & `django-wm-4.1.0.dev0/mentions/migrations/0010_alter_hcard_avatar_alter_hcard_name.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py` & `django-wm-4.1.0.dev0/mentions/migrations/0011_alter_pendingoutgoingcontent_text.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/migrations/0012_alter_hcard_options_and_more.py` & `django-wm-4.1.0.dev0/mentions/migrations/0012_alter_hcard_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/hcard.py` & `django-wm-4.1.0.dev0/mentions/models/hcard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/mixins/mentionable.py` & `django-wm-4.1.0.dev0/mentions/models/mixins/mentionable.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/mixins/quotable.py` & `django-wm-4.1.0.dev0/mentions/models/mixins/quotable.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/mixins/retryable.py` & `django-wm-4.1.0.dev0/mentions/models/mixins/retryable.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/outgoing_status.py` & `django-wm-4.1.0.dev0/mentions/models/outgoing_status.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/pending.py` & `django-wm-4.1.0.dev0/mentions/models/pending.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/simple_mention.py` & `django-wm-4.1.0.dev0/mentions/models/simple_mention.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/models/webmention.py` & `django-wm-4.1.0.dev0/mentions/models/webmention.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from mentions import options
 from mentions.models.base import MentionsBaseModel
+from mentions.models.managers.webmention import WebmentionQuerySet
 from mentions.models.mixins import QuotableMixin
 
 __all__ = [
     "Webmention",
 ]
 
 
 def _approve_default():
     return options.auto_approve()
 
 
 class Webmention(QuotableMixin, MentionsBaseModel):
     """An incoming webmention that is received by your server."""
 
+    objects = WebmentionQuerySet.as_manager()
+
     sent_by = models.URLField(
         _("sent by"),
         blank=True,
         help_text=_("Source address of the HTTP request that sent this webmention."),
     )
 
     approved = models.BooleanField(
@@ -32,14 +35,18 @@
         _("validated"),
         default=False,
         help_text=_(
             "True if both source and target have been validated, "
             "confirmed to exist, and source really does link to target."
         ),
     )
+    has_been_read = models.BooleanField(
+        _("Read"),
+        default=False,
+    )
 
     notes = models.CharField(
         _("notes"),
         max_length=1024,
         blank=True,
         help_text=_(
             "A description of any errors encountered when building this Webmention."
```

### Comparing `django-wm-4.0.1.dev4/mentions/options.py` & `django-wm-4.1.0.dev0/mentions/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,15 @@
 
 
 def url_scheme() -> str:
     """Return settings.WEBMENTIONS_URL_SCHEME.
 
     This defaults to `https` which is hopefully what your server is using.
     It's handy to be able to choose when debugging stuff though."""
-    scheme = _get_attr(SETTING_URL_SCHEME)
-    if not settings.DEBUG and scheme != "https":
-        log.warning(
-            f"settings.{SETTING_URL_SCHEME} should not be `http` when in production!"
-        )
-
-    return scheme
+    return _get_attr(SETTING_URL_SCHEME)
 
 
 def use_celery() -> bool:
     """Return settings.WEBMENTIONS_USE_CELERY, or True if not set.
 
     This setting enables/disables the use of `celery` for running tasks.
     If disabled, user must run these tasks using `manage.py pending_mentions` management command."""
```

### Comparing `django-wm-4.0.1.dev4/mentions/permissions.py` & `django-wm-4.1.0.dev0/mentions/permissions.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from django.contrib.auth.models import Permission
 from django.utils.translation import gettext_lazy as _
 
 from mentions.apps import MentionsConfig
 
 __all__ = [
+    "can_change_webmention",
     "can_view_dashboard",
 ]
 
 
 @dataclass
 class MentionsPermission:
     codename: str
@@ -35,7 +36,13 @@
         return self.fqn()
 
 
 can_view_dashboard = MentionsPermission(
     "view_webmention_dashboard",
     _("Can view the webmention dashboard/status page."),
 )
+
+
+# The following permissions are created automatically by Django.
+can_change_webmention = MentionsPermission(
+    "change_webmention", _("Default 'change' permission for Webmention model.")
+)
```

### Comparing `django-wm-4.0.1.dev4/mentions/resolution.py` & `django-wm-4.1.0.dev0/mentions/resolution.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             # Wagtail is not installed
             pass
 
         except Http404:
             raise TargetDoesNotExist(f"Could not resolve a wagtail page for url {url}")
 
         except KeyError:
-            log.warning(
+            log.debug(
                 f"Wagtail match is not mentionable: {url_path} | args={match.args} | kwargs={match.kwargs}"
             )
 
         raise NoModelForUrlPath()
 
     try:
         model_class: Type[MentionableMixin] = apps.get_model(model_name)
@@ -131,39 +131,41 @@
     except ObjectDoesNotExist:
         raise TargetDoesNotExist(
             f"Cannot find instance of model `{model_class}` with kwargs=`{urlpattern_kwargs}`"
         )
 
 
 def get_mentions_for_url(url: str) -> List[QuotableMixin]:
+    if "://" not in url:
+        url = config.build_url(url)
+
     try:
         obj = get_model_for_url(url)
         return obj.get_mentions()
 
     except NoModelForUrlPath:
         pass
 
-    if "://" not in url:
-        url = config.build_url(url)
-
     return get_public_mentions(target_url=url)
 
 
 def get_mentions_for_view(request: HttpRequest) -> List[QuotableMixin]:
     return get_mentions_for_url(request.build_absolute_uri())
 
 
 def get_mentions_for_object(obj: MentionableMixin) -> List[QuotableMixin]:
     ctype = ContentType.objects.get_for_model(obj.__class__)
 
     return get_public_mentions(content_type=ctype, object_id=obj.id)
 
 
-def get_public_mentions(**filter) -> List[QuotableMixin]:
-    webmentions = Webmention.objects.filter(
-        **filter,
-        approved=True,
-        validated=True,
+def get_public_mentions(**filter_kwargs) -> List[QuotableMixin]:
+    webmentions = Webmention.objects.filter_public().filter(**filter_kwargs)
+    simple_mentions = SimpleMention.objects.filter(**filter_kwargs)
+
+    return list(
+        sorted(
+            list(webmentions) + list(simple_mentions),
+            key=lambda x: x.created_at,
+            reverse=True,
+        )
     )
-    simple_mentions = SimpleMention.objects.filter(**filter)
-
-    return list(webmentions) + list(simple_mentions)
```

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/celeryproxy.py` & `django-wm-4.1.0.dev0/mentions/tasks/celeryproxy.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/local.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/local.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/parsing/hcard.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/hcard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/parsing/post_type.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/parsing/post_type.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/process.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/process.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/remote.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/remote.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/reverify.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/reverify.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/incoming/status.py` & `django-wm-4.1.0.dev0/mentions/tasks/incoming/status.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/outgoing/local.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/local.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/outgoing/parsing/webmention_endpoint.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/parsing/webmention_endpoint.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/outgoing/process.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/process.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/outgoing/remote.py` & `django-wm-4.1.0.dev0/mentions/tasks/outgoing/remote.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/tasks/scheduling.py` & `django-wm-4.1.0.dev0/mentions/tasks/scheduling.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/templates/mentions/webmention-dashboard.html` & `django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-dashboard.html`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,20 @@
         .item:nth-child(odd) {
             background-color: #d4d4d4;
         }
         .item:nth-child(even) {
             background-color: #e4e4e4;
         }
 
+        .icon {
+            font-size: large;
+            margin: 0 .5ch;
+            cursor: default;
+        }
+
         .item-summary {
             display: flex;
             flex-direction: row;
             justify-content: space-between;
             align-items: center;
             padding: 1ch .5ch;
         }
@@ -75,20 +81,14 @@
             cursor: default;
             color: #cc3344;
         }
 
         .end {
             font-size: smaller;
         }
-
-        .icon {
-            font-size: large;
-            margin: 0 .5ch;
-            cursor: default;
-        }
     </style>
 </head>
 
 <body>
   <h1>Webmentions Dashboard</h1>
 
   <div id="dashboard_overview">
@@ -226,19 +226,21 @@
   <script type="application/javascript">
     const params = new URLSearchParams(window.location.search);
     const defaultExpanded = params.has("expanded");
 
     document.querySelectorAll(".item").forEach(item => {
         // Click on received webmention summary to show more detail.
         if (item.querySelector(".item-detail")) {
-            item.dataset.expanded = defaultExpanded;
+            item.dataset.expanded = `${defaultExpanded}`;
 
             const summary = item.querySelector(".item-summary");
             summary.addEventListener("click", () => {
                 const isExpanded = item.dataset.expanded === "true";
-                item.dataset.expanded = !isExpanded;
+                item.dataset.expanded = `${!isExpanded}`;
             });
         }
     });
+
+    setTimeout(() => location.reload(), 10_000)
   </script>
 </body>
 </html>
```

### Comparing `django-wm-4.0.1.dev4/mentions/templates/mentions/webmention-submit-manual.html` & `django-wm-4.1.0.dev0/mentions/templates/mentions/webmention-submit-manual.html`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/templatetags/webmention_dashboard.py` & `django-wm-4.1.0.dev0/mentions/templatetags/webmention_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/templatetags/webmentions.py` & `django-wm-4.1.0.dev0/mentions/templatetags/webmentions.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/urls.py` & `django-wm-4.1.0.dev0/mentions/urls.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/util/html.py` & `django-wm-4.1.0.dev0/mentions/util/html.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/util/requests.py` & `django-wm-4.1.0.dev0/mentions/util/requests.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/util/url.py` & `django-wm-4.1.0.dev0/mentions/util/url.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/views/dashboard.py` & `django-wm-4.1.0.dev0/mentions/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/views/retrieve.py` & `django-wm-4.1.0.dev0/mentions/views/retrieve.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/views/serialize.py` & `django-wm-4.1.0.dev0/mentions/views/serialize.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/mentions/views/submit.py` & `django-wm-4.1.0.dev0/mentions/views/submit.py`

 * *Files identical despite different names*

### Comparing `django-wm-4.0.1.dev4/setup.cfg` & `django-wm-4.1.0.dev0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -36,12 +36,13 @@
 exclude = tests*
 
 [options.extras_require]
 celery = celery >= 5.2.2
 test = 
 	pytest
 	pytest-django
+wagtail = wagtail >= 3.0.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

