# Comparing `tmp/aa_memberaudit-2.8.0.tar.gz` & `tmp/aa_memberaudit-2.8.1.tar.gz`

## Comparing `aa_memberaudit-2.8.0.tar` & `aa_memberaudit-2.8.1.tar`

### file list

```diff
@@ -1,234 +1,234 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/__init__.py
--rw-r--r--   0        0        0    23256 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/admin.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/app_settings.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/apps.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/auth_hooks.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/checks.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/constants.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/decorators.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/forms.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/helpers.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/providers.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/signals.py
--rw-r--r--   0        0        0   881821 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/swagger.json
--rw-r--r--   0        0        0    40138 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tasks.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/__init__.py
--rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/data_exporters.py
--rw-r--r--   0        0        0    19266 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/eft_parser.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/fittings.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/skill_plans.py
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/skills.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/core/xml_converter.py
--rw-r--r--   0        0        0    40962 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/django.pot
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41012 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    41009 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41009 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41081 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41069 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41007 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41019 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26859 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    54511 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41002 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/__init__.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_data_export.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_load_eve.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_stats.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_update_characters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/__init__.py
--rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/character.py
--rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/general.py
--rw-r--r--   0        0        0    48513 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/managers/sections.py
--rw-r--r--   0        0        0    65995 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0003_add_notify_permission.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0004_character_is_disabled.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0005_add_fw_stats.py
--rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0006_add_localizations.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/0007_add_localization_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/migrations/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/__init__.py
--rw-r--r--   0        0        0    54096 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/character.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/constants.py
--rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/general.py
--rw-r--r--   0        0        0    40017 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/models/sections.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/admin.css
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_finder.css
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.css
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/data_export.css
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.css
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.min.css
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.css
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.min.css
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.css
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/reports.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/charisma.png
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/eve-prism.png
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/evelogo.png
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/evesearch.png
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/intelligence.png
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/memory.png
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/perception.png
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/willpower.png
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/zkillboard.png
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/base.html
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_finder.html
--rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_viewer.html
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/data_export.html
--rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/launcher.html
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/reports.html
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/menu.html
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templatetags/__init__.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/templatetags/memberaudit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/__init__.py
--rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_admin.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_checks.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_commands.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_decorators.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_factories.py
--rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_forms.py
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_helpers.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_integration.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_signals.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_tasks.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/test_templatetags.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/__init__.py
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_core_xml_converter.py
--rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_data_exporters.py
--rw-r--r--   0        0        0    22356 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_eft_parser.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_fittings.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_skill_plans.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/core/test_skills.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/__init__.py
--rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/test_character.py
--rw-r--r--   0        0        0    41576 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/test_general.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/managers/test_sections.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/__init__.py
--rw-r--r--   0        0        0    36061 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_1.py
--rw-r--r--   0        0        0    35834 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_2.py
--rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_3.py
--rw-r--r--   0        0        0    28275 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_4.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_5.py
--rw-r--r--   0        0        0    10448 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_general.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/test_sections.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/models/utils.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/__init__.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/entities.json
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0    40192 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_testdata.json
--rw-r--r--   0        0        0  1159197 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/factories.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_character.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_doctrines.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_entities.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_locations.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/profiler_toolbox.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/__init__.py
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_admin.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_finder.py
--rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_1.py
--rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_2.py
--rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_characters.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_data_export.py
--rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tests/views/test_reports.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tools/drop_tables.sql
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/tools/total_size.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/__init__.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/_common.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/admin.py
--rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/character_finder.py
--rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/character_viewer_1.py
--rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/character_viewer_2.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/characters.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/data_export.py
--rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/memberaudit/views/reports.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/LICENSE
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/README.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/__init__.py
+-rw-r--r--   0        0        0    23180 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/admin.py
+-rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/apps.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/checks.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/constants.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/forms.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/helpers.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/providers.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/signals.py
+-rw-r--r--   0        0        0   881821 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/swagger.json
+-rw-r--r--   0        0        0    40138 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tasks.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11673 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19266 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0    40902 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40961 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    40949 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40949 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41027 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41015 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40956 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40968 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26859 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41186 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40942 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13012 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    48513 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/managers/sections.py
+-rw-r--r--   0        0        0    65995 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    54096 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/models/character.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    15409 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/models/general.py
+-rw-r--r--   0        0        0    40017 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/models/sections.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0    14036 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12708 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    22356 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    41576 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/managers/test_sections.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0    36061 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_1.py
+-rw-r--r--   0        0        0    35834 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_2.py
+-rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_3.py
+-rw-r--r--   0        0        0    28275 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_4.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_5.py
+-rw-r--r--   0        0        0    10448 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/test_sections.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/models/utils.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    40192 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1159197 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    12618 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    22475 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16230 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12529 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    22528 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13100 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/memberaudit/views/reports.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/LICENSE
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/README.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7470 2020-02-02 00:00:00.000000 aa_memberaudit-2.8.1/PKG-INFO
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/admin.py` & `aa_memberaudit-2.8.1/memberaudit/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,18 +354,16 @@
             for obj in queryset:
                 tasks.delete_character.apply_async(
                     kwargs={"character_pk": obj.pk},
                     priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
                 )  # type: ignore
             self.message_user(
                 request,
-                _(
-                    "Started deleting %d character(s). "
-                    "This can take a minute." % queryset.count()
-                ),
+                _("Started deleting %d character(s). This can take a minute.")
+                % queryset.count(),
             )
             return redirect(request.get_full_path())
         return render(
             request,
             "admin/memberaudit/character/confirm_character_deletion.html",
             {
                 "title": _("Are you sure you want to delete these characters?"),
@@ -376,27 +374,27 @@
     @admin.display(description=_("Update selected characters from EVE server"))
     def update_characters(self, request, queryset):
         for obj in queryset:
             tasks.update_character.apply_async(
                 kwargs={"character_pk": obj.pk, "force_update": True},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )  # type: ignore
-            self.message_user(request, _("Started updating character %s." % obj))
+            self.message_user(request, _("Started updating character %s.") % obj)
 
     @admin.display(
         description=_("Update assets for selected characters from EVE server")
     )
     def update_assets(self, request, queryset):
         for obj in queryset:
             tasks.update_character_assets.apply_async(
                 kwargs={"character_pk": obj.pk, "force_update": True},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )  # type: ignore
             self.message_user(
-                request, _("Started updating assets for character %s." % obj)
+                request, _("Started updating assets for character %s.") % obj
             )
 
     @admin.display(
         description=(
             _(
                 "Update %s for selected characters from EVE server"
                 % {
@@ -412,29 +410,24 @@
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )  # type: ignore
             self.message_user(
                 request,
-                _(
-                    "Started updating %s for character %s."
-                    % (Character.UpdateSection.display_name(section), obj)
-                ),
+                _("Started updating section %(section)s for character %(character)s.")
+                % {
+                    "section": Character.UpdateSection.display_name(section),
+                    "character": obj,
+                },
             )
 
     @admin.display(
-        description=(
-            _(
-                "Update %s for selected characters from EVE server"
-                % Character.UpdateSection.display_name(
-                    Character.UpdateSection.ONLINE_STATUS
-                )
-            )
-        )
+        description=_("Update %s for selected characters from EVE server")
+        % Character.UpdateSection.display_name(Character.UpdateSection.ONLINE_STATUS)
     )
     def update_online_status(self, request, queryset):
         section = Character.UpdateSection.ONLINE_STATUS
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
@@ -450,21 +443,21 @@
                 ),
             )
 
     @admin.display(description=_("Enable selected characters"))
     def enable_characters(self, request, queryset):
         pks = list(queryset.values_list("pk", flat=True))
         queryset.filter(pk__in=pks).update(is_disabled=False)
-        self.message_user(request, _("Enabled %d characters." % len(pks)))
+        self.message_user(request, _("Enabled %d characters.") % len(pks))
 
     @admin.display(description=_("Disable selected characters"))
     def disable_characters(self, request, queryset):
         pks = list(queryset.values_list("pk", flat=True))
         queryset.filter(pk__in=pks).update(is_disabled=True)
-        self.message_user(request, _("Disabled %d characters." % len(pks)))
+        self.message_user(request, _("Disabled %d characters.") % len(pks))
 
     inlines = (SyncStatusAdminInline,)
 
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
@@ -565,15 +558,15 @@
                         row
                         and row.get("DELETE") is False
                         and not row.get("required_level")
                         and not row.get("recommended_level")
                     ):
                         eve_type = row.get("eve_type")
                         raise ValidationError(
-                            _("Skill '%s' must have a level." % eve_type.name)
+                            _("Skill '%s' must have a level.") % eve_type.name
                         )
 
 
 class SkillSetSkillAdminInline(MinValidatedInlineMixIn, admin.TabularInline):
     model = SkillSetSkill
     verbose_name = "skill"
     verbose_name_plural = "skills"
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/app_settings.py` & `aa_memberaudit-2.8.1/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/auth_hooks.py` & `aa_memberaudit-2.8.1/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/checks.py` & `aa_memberaudit-2.8.1/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/constants.py` & `aa_memberaudit-2.8.1/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/decorators.py` & `aa_memberaudit-2.8.1/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/forms.py` & `aa_memberaudit-2.8.1/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/helpers.py` & `aa_memberaudit-2.8.1/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/swagger.json` & `aa_memberaudit-2.8.1/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tasks.py` & `aa_memberaudit-2.8.1/memberaudit/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/urls.py` & `aa_memberaudit-2.8.1/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.8.1/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.8.1/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/core/fittings.py` & `aa_memberaudit-2.8.1/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.8.1/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/core/skills.py` & `aa_memberaudit-2.8.1/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.8.1/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/django.pot` & `aa_memberaudit-2.8.1/memberaudit/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,148 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -1628,34 +1628,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1685,18 +1680,18 @@
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,149 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: German (https://app.transifex.com/kalkoken-apps/teams/107978/"
-"de/)\n"
-"Language: de\n"
+"Language-Team: French (France) (https://app.transifex.com/kalkoken-apps/teams/107978/fr_FR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: fr_FR\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -296,15 +295,16 @@
 msgstr ""
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:284
 msgid "is active"
 msgstr ""
 
 #: models/general.py:285
@@ -370,15 +370,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr ""
@@ -752,15 +753,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -1605,15 +1607,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1629,34 +1632,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1675,29 +1673,29 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,149 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
+"PO-Revision-Date: 2020-12-07 21:40+0000\n"
+"Language-Team: German (https://app.transifex.com/kalkoken-apps/teams/107978/de/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -296,15 +295,16 @@
 msgstr ""
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:284
 msgid "is active"
 msgstr ""
 
 #: models/general.py:285
@@ -370,15 +370,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr ""
@@ -752,15 +753,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -1605,15 +1607,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1629,34 +1632,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1675,29 +1673,29 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,149 +4,149 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -1629,34 +1629,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1686,18 +1681,18 @@
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/fr_FR/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,150 +4,149 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
-"PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: French (France) (https://app.transifex.com/kalkoken-apps/"
-"teams/107978/fr_FR/)\n"
-"Language: fr_FR\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
-"1000000 == 0 ? 1 : 2;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -1630,34 +1629,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1687,18 +1681,18 @@
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/it_IT/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,150 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: Italian (Italy) (https://app.transifex.com/kalkoken-apps/"
-"teams/107978/it_IT/)\n"
-"Language: it_IT\n"
+"Language-Team: Italian (Italy) (https://app.transifex.com/kalkoken-apps/teams/107978/it_IT/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
-"1 : 2;\n"
+"Language: it_IT\n"
+"Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? 1 : 2;\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -297,15 +295,16 @@
 msgstr ""
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:284
 msgid "is active"
 msgstr ""
 
 #: models/general.py:285
@@ -371,15 +370,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr ""
@@ -753,15 +753,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -1606,15 +1607,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1630,34 +1632,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1676,29 +1673,29 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/ja/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,149 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: Japanese (https://app.transifex.com/kalkoken-apps/"
-"teams/107978/ja/)\n"
-"Language: ja\n"
+"Language-Team: Japanese (https://app.transifex.com/kalkoken-apps/teams/107978/ja/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ja\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -296,15 +295,16 @@
 msgstr ""
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:284
 msgid "is active"
 msgstr ""
 
 #: models/general.py:285
@@ -370,15 +370,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr ""
@@ -752,15 +753,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -1605,15 +1607,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1629,34 +1632,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1675,29 +1673,29 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/ko_KR/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,149 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: Korean (Korea) (https://app.transifex.com/kalkoken-apps/"
-"teams/107978/ko_KR/)\n"
-"Language: ko_KR\n"
+"Language-Team: Korean (Korea) (https://app.transifex.com/kalkoken-apps/teams/107978/ko_KR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Language: ko_KR\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -296,15 +295,16 @@
 msgstr ""
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:284
 msgid "is active"
 msgstr ""
 
 #: models/general.py:285
@@ -370,15 +370,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr ""
@@ -752,15 +753,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -1605,15 +1607,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1629,34 +1632,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1675,29 +1673,29 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/ru/LC_MESSAGES/django.mo` & `aa_memberaudit-2.8.1/memberaudit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files 16% similar despite different names*

```diff
@@ -2,163 +2,155 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 # Translators:
 # Николай Постников, 2023
 # Тимур Шихалиев, 2023
-# Erik Kalkoken <erik.kalkoken@gmail.com>, 2023
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Last-Translator: Erik Kalkoken <erik.kalkoken@gmail.com>, 2023\n"
-"Language-Team: Russian (https://app.transifex.com/kalkoken-apps/teams/107978/"
-"ru/)\n"
-"Language: ru\n"
+"Last-Translator: Тимур Шихалиев, 2023\n"
+"Language-Team: Russian (https://app.transifex.com/kalkoken-apps/teams/107978/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Language: ru\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr "Ограничено состояниями"
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr "статус обновления"
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr "состояние"
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr "Нет главного"
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr "персонажа"
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr "включено"
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr "главный"
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr "организация"
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr "создано"
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr "последнее обновление"
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr "Удалить выбранных персонажей"
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr "Началось удаление %d персонажа(ей). Это может занять минуту."
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr "Вы уверены, что хотите удалить этих персонажей?"
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr "Обновить выбранных персонажей с сервера EVE"
 
-#: admin.py:384
-#, fuzzy, python-format
-#| msgid "Started updating character: %s. "
+#: admin.py:381
+#, python-format
 msgid "Started updating character %s."
 msgstr "Началось обновление персонажа %s."
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr "Обновить имущество выбранных персонажей с сервера EVE"
 
-#: admin.py:396
-#, fuzzy, python-format
-#| msgid "Started updating assets for character: %s."
+#: admin.py:393
+#, python-format
 msgid "Started updating assets for character %s."
-msgstr " Началось обновление имущества персонажа %s."
+msgstr "Началось обновление имущества для персонажа %s."
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr "Обновление %s для выбранных персонажей с сервера EVE"
 
-#: admin.py:421
-#, fuzzy, python-format
-#| msgid "Started updating %s for character: %s."
-msgid "Started updating %s for character %s."
-msgstr "Началось обновление %s для персонажа: %s. "
+#: admin.py:417
+#, python-format
+msgid "Started updating section %(section)s for character %(character)s."
+msgstr "Началось обновление раздела %(section)sдля персонажа %(character)s. "
 
-#: admin.py:446
-#, fuzzy, python-format
-#| msgid "Started updating assets for character: %s."
+#: admin.py:438
+#, python-format
 msgid "Started updating %(section)s for character %(character)s."
-msgstr " Началось обновление имущества персонажа %s."
+msgstr "Началось обновление %(section)s для персонажа %(character)s."
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr "Активировать выбранных персонажей."
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr "Активировано %d персонажей."
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr "Деактивировать выбранных персонажей"
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr "Деактивировано %d персонажей."
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr "название"
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr "звездная система"
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr "тип"
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr "группа"
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr "обновлено"
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr "Навык должен иметь уровень '%s'."
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr "Просмотр пилотов"
@@ -280,70 +272,61 @@
 msgstr "выключено"
 
 #: models/character.py:169
 msgid "mailing lists"
 msgstr "списки рассылок"
 
 #: models/character.py:177
-#, fuzzy
-#| msgid "character"
 msgid "characters"
-msgstr "персонажа"
+msgstr "персонажи"
 
 #: models/character.py:1294 models/character.py:1295
-#, fuzzy
-#| msgid "update status"
 msgid "character update status"
-msgstr "статус обновления"
+msgstr "статус обновления персонажа"
 
 #: models/general.py:116
 msgid "compliance group designation"
-msgstr ""
+msgstr "обозначение группы соблюдения"
 
 #: models/general.py:117
 msgid "compliance group designations"
-msgstr ""
+msgstr "обозначения группы соблюдения"
 
 #: models/general.py:186
-#, fuzzy
-#| msgid "location"
 msgid "locations"
-msgstr "местонахождение"
+msgstr "местонахождения"
 
 #: models/general.py:269 models/general.py:309
 msgid "description"
 msgstr "описание"
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr "является доктриной"
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr "Включить корректное отображение группы набора навыков в отчетах"
 
 #: models/general.py:284
 msgid "is active"
 msgstr "активен"
 
 #: models/general.py:285
 msgid "Whether this skill set group is in active use"
 msgstr "Активна ли группа набора навыков"
 
 #: models/general.py:290
-#, fuzzy
-#| msgid "Skill Set Group"
 msgid "skill set group"
-msgstr "Группа наборов навыков"
+msgstr "группа наборов навыков"
 
 #: models/general.py:291
-#, fuzzy
-#| msgid "Skill Set Group"
 msgid "skill set groups"
-msgstr "Группа наборов навыков"
+msgstr "группы наборов навыков"
 
 #: models/general.py:298
 msgid "Doctrine: "
 msgstr "Формат:"
 
 #: models/general.py:317
 msgid "ship type"
@@ -366,18 +349,16 @@
 "Non visible skill sets are not shown to users on their character sheet and "
 "used for audit purposes only."
 msgstr ""
 "Невидимые наборы навыков не отображаются на карточках персонажей и "
 "используются для аудита"
 
 #: models/general.py:339
-#, fuzzy
-#| msgid "skill sets"
 msgid "skill set"
-msgstr "наборы навыков"
+msgstr "набор навыков"
 
 #: models/general.py:358 models/general.py:385
 msgid "skill"
 msgstr "навык"
 
 #: models/general.py:367
 msgid "required level"
@@ -398,15 +379,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr "Персонаж"
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr "Корпорация"
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr "Список адресатов"
@@ -780,15 +762,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr "Основной"
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr "Статус"
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -903,25 +886,29 @@
 
 #: templates/memberaudit/data_export.html:45
 #, python-format
 msgid ""
 "Export files contain the complete data of all %(amount_of_characters)s "
 "characters known to Member Audit."
 msgstr ""
+"Файлы экспорта содержат полную информацию по %(amount_of_characters)s "
+"персонажам известных Member Audit."
 
 #: templates/memberaudit/data_export.html:46
 msgid "They are in CSV format and zipped."
-msgstr ""
+msgstr "Они в формате CSV и упакованы в zip-архив."
 
 #: templates/memberaudit/data_export.html:47
 #, python-format
 msgid ""
 "Existing export files are updated after %(minutes_until_next_update)s "
 "minutes."
 msgstr ""
+"Существующие файлы экспорта будут обновлены через "
+"%(minutes_until_next_update)s минут."
 
 #: templates/memberaudit/launcher.html:20
 msgid "Register Character"
 msgstr "Зарегистрировать персонажа"
 
 #: templates/memberaudit/launcher.html:29
 msgid "Register"
@@ -1633,15 +1620,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr "Зарегистрированный?"
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr "Соответствует?"
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr "Всего персонажей"
 
@@ -1657,36 +1645,29 @@
 msgid "Groups"
 msgstr "Группы"
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr "[Разгруппированный]"
 
-#: views/admin.py:37
+#: views/admin.py:35 views/admin.py:68
 #, python-format
-msgid "A skill set with the name %s already exists."
-msgstr "Набор навыков с именем %s уже существует."
-
-#: views/admin.py:51 views/admin.py:89
-#, fuzzy, python-format
-#| msgid "Skill Set <b>%s</b> has been created"
 msgid "Skill Set %s has been created"
-msgstr "Набор навыков 1%s1 был создан"
+msgstr "Набор навыков %s создан"
 
-#: views/admin.py:53 views/admin.py:91
-#, fuzzy, python-format
-#| msgid "Skill Set <b>%s</b> has been updated"
+#: views/admin.py:37 views/admin.py:70
+#, python-format
 msgid "Skill Set %s has been updated"
-msgstr "Набор навыков 1%s1 был обновлен"
+msgstr "Набор навыков %s обновлен"
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr "Создать набор навыков из подгонки"
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr "Создать набор навыков из плана"
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr "Вы не владеете этим персонажем"
 
@@ -1705,76 +1686,36 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr "Продать"
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 "был зарегистрирован. Обратите внимание, что все данные по персонажу станут "
 "доступными к просмотру через минуту."
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr "%s: персонаж был убран!"
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
-msgstr "%s убрал персонажа '%s'"
+msgid "%(user)s has removed character %(character)s"
+msgstr "%(user)s удалил персонажа %(character)s"
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr "Убрал персонажа %sпо запросу."
 
 #: views/data_export.py:53
-#, fuzzy, python-format
-#| msgid ""
-#| "Data export for topic <strong>%s</strong> has been started. This can take "
-#| "a couple of minutes. You will get a notification once it is completed."
+#, python-format
 msgid ""
 "Data export for topic %s has been started. This can take a couple of "
 "minutes. You will get a notification once it is completed."
 msgstr ""
-"Топик экспорта данных для <strong>%s</strong>запущен. Это займет несколько "
-"минут. По окончанию экспорта, вы получите уведомление."
-
-#, python-format
-#~ msgid "Started updating %s for character: %s. "
-#~ msgstr "Началось обновление %s для персонажа: %s. "
-
-#~ msgid "Character<br>Name"
-#~ msgstr "Имя персонажа"
-
-#~ msgid "Character<br>Organization"
-#~ msgstr "Организация персонажа"
-
-#~ msgid "Main<br>Name"
-#~ msgstr "Основное Имя"
-
-#~ msgid "Main<br>Organization"
-#~ msgstr "Основная Организация"
-
-#~ msgid "Main<br>State"
-#~ msgstr "Основной Статус"
-
-#, python-format
-#~ msgid ""
-#~ "\n"
-#~ "                    Export files contain the complete data of all "
-#~ "<strong>%(amount_of_characters)s</strong>\n"
-#~ "                    characters known to Member Audit. They are in CSV "
-#~ "format and zipped.\n"
-#~ "                    Existing export files can updated after "
-#~ "%(minutes_until_next_update)s minutes.\n"
-#~ "                "
-#~ msgstr ""
-#~ "\n"
-#~ "Экспортируемые файлы содержат все данные для %(amount_of_characters)s "
-#~ "известных \"Просмотру персонажей\". Файлы в CSV формате и "
-#~ "заархивированы.\n"
-#~ "Существующие файлы могут быть обновлены через "
-#~ "%(minutes_until_next_update)s минут."
+"Топик экспорта данных для %s запущен. Это займет несколько минут. По "
+"окончанию экспорта, вы получите уведомление."
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.mo` & `aa_memberaudit-2.8.1/memberaudit/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/uk/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,152 +4,148 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: 2020-12-07 21:40+0000\n"
-"Language-Team: Ukrainian (https://app.transifex.com/kalkoken-apps/"
-"teams/107978/uk/)\n"
-"Language: uk\n"
+"Language-Team: Ukrainian (https://app.transifex.com/kalkoken-apps/teams/107978/uk/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
-"11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
-"100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
-"(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
+"Language: uk\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != 11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % 100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || (n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -299,15 +295,16 @@
 msgstr ""
 
 #: models/general.py:276
 msgid "is doctrine"
 msgstr ""
 
 #: models/general.py:278
-msgid "This enables a skill set group to show up correctly in doctrine reports"
+msgid ""
+"This enables a skill set group to show up correctly in doctrine reports"
 msgstr ""
 
 #: models/general.py:284
 msgid "is active"
 msgstr ""
 
 #: models/general.py:285
@@ -373,15 +370,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:13
 msgid "Character"
 msgstr ""
 
 #: models/general.py:435
 #: templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html:6
 #: templates/memberaudit/partials/character_viewer/tabs/loyalty.html:8
-#: templates/memberaudit/reports.html:80 templates/memberaudit/reports.html:145
+#: templates/memberaudit/reports.html:80
+#: templates/memberaudit/reports.html:145
 #: templates/memberaudit/reports.html:219
 msgid "Corporation"
 msgstr ""
 
 #: models/general.py:436
 msgid "Mailing List"
 msgstr ""
@@ -755,15 +753,16 @@
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:10
 msgid "Main"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:22
 #: templates/memberaudit/partials/reports/tabs/skill_sets.html:11
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:9
-#: templates/memberaudit/reports.html:70 templates/memberaudit/reports.html:209
+#: templates/memberaudit/reports.html:70
+#: templates/memberaudit/reports.html:209
 msgid "State"
 msgstr ""
 
 #: templates/memberaudit/character_finder.html:31
 #: templates/memberaudit/launcher.html:42
 #: templates/memberaudit/launcher.html:126
 #: templates/memberaudit/partials/character_viewer/sidebar_character.html:10
@@ -1608,15 +1607,16 @@
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:11
 #: templates/memberaudit/reports.html:85
 msgid "Registered?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:12
-#: templates/memberaudit/reports.html:90 templates/memberaudit/reports.html:150
+#: templates/memberaudit/reports.html:90
+#: templates/memberaudit/reports.html:150
 msgid "Compliant?"
 msgstr ""
 
 #: templates/memberaudit/partials/reports/tabs/user_compliance.html:13
 msgid "Total Chars"
 msgstr ""
 
@@ -1632,34 +1632,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1678,29 +1673,29 @@
 
 #: views/character_viewer_2.py:616
 msgid "Sell"
 msgstr ""
 
 #: views/characters.py:119
 msgid ""
-"has been registered. Note that it can take a minute until all character data "
-"is visible."
+"has been registered. Note that it can take a minute until all character data"
+" is visible."
 msgstr ""
 
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_memberaudit-2.8.1/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,149 +4,149 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-25 20:21+0200\n"
+"POT-Creation-Date: 2023-05-08 22:21+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: admin.py:73
+#: admin.py:75
 msgid "Restricted to states"
 msgstr ""
 
-#: admin.py:134 admin.py:312
+#: admin.py:136 admin.py:311
 msgid "update status"
 msgstr ""
 
-#: admin.py:160 admin.py:289
+#: admin.py:162 admin.py:291
 msgid "state"
 msgstr ""
 
-#: admin.py:186
+#: admin.py:188
 msgid "No main"
 msgstr ""
 
-#: admin.py:268 models/character.py:176
+#: admin.py:270 models/character.py:176
 msgid "character"
 msgstr ""
 
-#: admin.py:272
+#: admin.py:274
 msgid "enabled"
 msgstr ""
 
-#: admin.py:278
+#: admin.py:280
 msgid "main"
 msgstr ""
 
-#: admin.py:299
+#: admin.py:301
 msgid "organization"
 msgstr ""
 
-#: admin.py:324
+#: admin.py:323
 msgid "created"
 msgstr ""
 
-#: admin.py:328
+#: admin.py:327
 msgid "last update"
 msgstr ""
 
-#: admin.py:352
+#: admin.py:351
 msgid "Delete selected characters"
 msgstr ""
 
-#: admin.py:363
+#: admin.py:361
 #, python-format
 msgid "Started deleting %d character(s). This can take a minute."
 msgstr ""
 
-#: admin.py:372
+#: admin.py:369
 msgid "Are you sure you want to delete these characters?"
 msgstr ""
 
-#: admin.py:377
+#: admin.py:374
 msgid "Update selected characters from EVE server"
 msgstr ""
 
-#: admin.py:384
+#: admin.py:381
 #, python-format
 msgid "Started updating character %s."
 msgstr ""
 
-#: admin.py:387
+#: admin.py:384
 msgid "Update assets for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:396
+#: admin.py:393
 #, python-format
 msgid "Started updating assets for character %s."
 msgstr ""
 
-#: admin.py:402 admin.py:429
+#: admin.py:399 admin.py:425
 #, python-format
 msgid "Update %s for selected characters from EVE server"
 msgstr ""
 
-#: admin.py:421
+#: admin.py:417
 #, python-format
-msgid "Started updating %s for character %s."
+msgid "Started updating section %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:446
+#: admin.py:438
 #, python-format
 msgid "Started updating %(section)s for character %(character)s."
 msgstr ""
 
-#: admin.py:454
+#: admin.py:446
 msgid "Enable selected characters"
 msgstr ""
 
-#: admin.py:458
+#: admin.py:450
 #, python-format
 msgid "Enabled %d characters."
 msgstr ""
 
-#: admin.py:460
+#: admin.py:452
 msgid "Disable selected characters"
 msgstr ""
 
-#: admin.py:464
+#: admin.py:456
 #, python-format
 msgid "Disabled %d characters."
 msgstr ""
 
-#: admin.py:496 models/general.py:267 models/general.py:307
+#: admin.py:488 models/general.py:267 models/general.py:307
 msgid "name"
 msgstr ""
 
-#: admin.py:500
+#: admin.py:492
 msgid "solar system"
 msgstr ""
 
-#: admin.py:504
+#: admin.py:496
 msgid "type"
 msgstr ""
 
-#: admin.py:508
+#: admin.py:500
 msgid "group"
 msgstr ""
 
-#: admin.py:512
+#: admin.py:504
 msgid "updated at"
 msgstr ""
 
-#: admin.py:573
+#: admin.py:565
 #, python-format
 msgid "Skill '%s' must have a level."
 msgstr ""
 
 #: app_settings.py:8
 msgid "Member Audit"
 msgstr ""
@@ -1629,34 +1629,29 @@
 msgid "Groups"
 msgstr ""
 
 #: views/_common.py:12
 msgid "[Ungrouped]"
 msgstr ""
 
-#: views/admin.py:37
-#, python-format
-msgid "A skill set with the name %s already exists."
-msgstr ""
-
-#: views/admin.py:51 views/admin.py:89
+#: views/admin.py:35 views/admin.py:68
 #, python-format
 msgid "Skill Set %s has been created"
 msgstr ""
 
-#: views/admin.py:53 views/admin.py:91
+#: views/admin.py:37 views/admin.py:70
 #, python-format
 msgid "Skill Set %s has been updated"
 msgstr ""
 
-#: views/admin.py:67
+#: views/admin.py:46
 msgid "Create skill set from fitting"
 msgstr ""
 
-#: views/admin.py:105
+#: views/admin.py:79
 msgid "Create skill set from skill plan"
 msgstr ""
 
 #: views/character_viewer_1.py:186
 msgid "You do not own this character"
 msgstr ""
 
@@ -1686,18 +1681,18 @@
 #: views/characters.py:148
 #, python-format
 msgid "%s: Character has been removed!"
 msgstr ""
 
 #: views/characters.py:149
 #, python-format
-msgid "%s has removed character '%s'"
+msgid "%(user)s has removed character %(character)s"
 msgstr ""
 
-#: views/characters.py:156
+#: views/characters.py:159
 #, python-format
 msgid "Removed character %s as requested."
 msgstr ""
 
 #: views/data_export.py:53
 #, python-format
 msgid ""
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.8.1/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/managers/character.py` & `aa_memberaudit-2.8.1/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/managers/general.py` & `aa_memberaudit-2.8.1/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/managers/sections.py` & `aa_memberaudit-2.8.1/memberaudit/managers/sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/migrations/0007_add_localization_2.py` & `aa_memberaudit-2.8.1/memberaudit/migrations/0007_add_localization_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/models/__init__.py` & `aa_memberaudit-2.8.1/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/models/character.py` & `aa_memberaudit-2.8.1/memberaudit/models/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/models/general.py` & `aa_memberaudit-2.8.1/memberaudit/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/models/sections.py` & `aa_memberaudit-2.8.1/memberaudit/models/sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.8.1/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.8.1/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.8.1/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.8.1/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.8.1/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/utils.py` & `aa_memberaudit-2.8.1/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.8.1/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.8.1/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.8.1/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.8.1/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.8.1/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.8.1/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.8.1/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.8.1/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/managers/test_sections.py` & `aa_memberaudit-2.8.1/memberaudit/tests/managers/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_1.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_2.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_3.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_4.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_4.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_character_5.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_character_5.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/test_sections.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/models/utils.py` & `aa_memberaudit-2.8.1/memberaudit/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.8.1/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_characters.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         self.assertTrue(mock_tasks.update_compliance_groups_for_user.apply_async.called)
         self.assertTrue(mock_messages.success.called)
 
         expected_removal_notification_title = (
             "Member Audit: Character has been removed!"
         )
         expected_removal_notification_message = (
-            "Bruce Wayne has removed character 'Bruce Wayne'"
+            "Bruce Wayne has removed character Bruce Wayne"
         )
         latest_auditor_notification = auditor.notification_set.order_by("-pk")[0]
         self.assertEqual(
             latest_auditor_notification.title, expected_removal_notification_title
         )
         self.assertEqual(
             latest_auditor_notification.message, expected_removal_notification_message
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.8.1/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.8.1/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/_common.py` & `aa_memberaudit-2.8.1/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/admin.py` & `aa_memberaudit-2.8.1/memberaudit/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/character_finder.py` & `aa_memberaudit-2.8.1/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.8.1/memberaudit/views/character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.8.1/memberaudit/views/character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/characters.py` & `aa_memberaudit-2.8.1/memberaudit/views/characters.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,19 @@
         character_name = character.eve_character.character_name
 
         # Notify that character has been dropped
         permission_to_notify = Permission.objects.select_related("content_type").get(
             content_type__app_label=Character._meta.app_label,
             codename="notified_on_character_removal",
         )
-        title = _("%s: Character has been removed!" % __title__)
-        message = _("%s has removed character '%s'" % (request.user, character_name))
+        title = _("%s: Character has been removed!") % __title__
+        message = _("%(user)s has removed character %(character)s") % {
+            "user": request.user,
+            "character": character_name,
+        }
         for to_notify in users_with_permission(permission_to_notify):
             if character.user_has_scope(to_notify):
                 notify(user=to_notify, title=title, message=message, level="INFO")
 
         character.delete()
         messages.success(
             request, _("Removed character %s as requested.") % character_name
```

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/data_export.py` & `aa_memberaudit-2.8.1/memberaudit/views/data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/memberaudit/views/reports.py` & `aa_memberaudit-2.8.1/memberaudit/views/reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/LICENSE` & `aa_memberaudit-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/README.md` & `aa_memberaudit-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/pyproject.toml` & `aa_memberaudit-2.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.8.0/PKG-INFO` & `aa_memberaudit-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.8.0
+Version: 2.8.1
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-memberaudit
 Project-URL: Documentation, https://aa-memberaudit.readthedocs.io/en/latest/
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-memberaudit
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-memberaudit/-/issues
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Peter Pfeufer <develop@ppfeufer.de>, Rebecca Murphy <rebecca@rcmurphy.me>
```

