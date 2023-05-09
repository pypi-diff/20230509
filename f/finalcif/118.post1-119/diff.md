# Comparing `tmp/finalcif-118.post1.tar.gz` & `tmp/finalcif-119.tar.gz`

## Comparing `finalcif-118.post1.tar` & `finalcif-119.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/app_path.py
--rw-r--r--   0        0        0    91866 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/appwindow.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/finalcif_start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/all_cif_dicts.py
--rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/atoms.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cif_dict_foo.py
--rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cif_file_io.py
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cif_order.py
--rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/core_dict.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/hkl.py
--rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/modulation_dict.py
--rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/powder_dict.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/reference.py
--rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/restraints_dict.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/text.py
--rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/twin_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/checkcif/__init__.py
--rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/checkcif/checkcif.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/__init__.py
--rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/deposit.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/deposit_check.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/deposition_list.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/doi.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/upload.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/cif/cod/website_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/__init__.py
--rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/bruker_data.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/bruker_frame.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/ccdc_mail.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/data.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/p4p_reader.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/sadabs.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/saint.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/shelx_lst.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/datafiles/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/displaymol/__init__.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/displaymol/sdm.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/displaymol/vtk_molecule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/equip_property/__init__.py
--rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/equip_property/author_loop_templates.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/equip_property/equipment.py
--rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/equip_property/properties.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/equip_property/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/__init__.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/combobox.py
--rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/custom_classes.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/dialogs.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/equipmenttable.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/file_editor.py
--rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/finalcif_gui_ui.py
--rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/finalcif_gui_ui.ui
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/loop_creator.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/loop_creator_ui.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/loop_creator_ui.ui
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/loops.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/mainstackwidget.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/mixins.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/new_key_dialog.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/new_key_dialog_ui.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/new_key_dialog_ui.ui
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/plaintextedit.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/playground.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/propertytable.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/text_templates_ui.py
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/text_templates_ui.ui
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/text_value_editor.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/gui/vrf_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/__init__.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/finalcif.png
--rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/finalcif2.ico
--rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/finalcif2.png
--rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/multitable.ico
--rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/multitable.png
--rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/icon/multitable.xcf
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/archive_report.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/mtools.py
--rw-r--r--   0        0        0    18359 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/references.py
--rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/report_text.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/symm.py
--rw-r--r--   0        0        0    38145 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/tables.py
--rw-r--r--   0        0        0    26583 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/templated_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/gui/__init__.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/gui/mainwindow.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/report/gui/mainwindow.ui
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/template/__init__.py
--rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/template/mathml2omml.xsl
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/template/template1.docx
--rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/template/template_text.docx
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/template/template_without_text.docx
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/template/templates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/__init__.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/download.py
--rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/dsrmath.py
--rw-r--r--   0        0        0    32789 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/misc.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/options.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/platon.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/pupdate.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/settings.py
--rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/shred.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/space_groups.py
--rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/spgr_format.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/statusbar.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-118.post1/finalcif/tools/sumformula.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-118.post1/.gitignore
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-118.post1/LICENSE
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 finalcif-118.post1/README.md
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 finalcif-118.post1/pyproject.toml
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 finalcif-118.post1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-119/finalcif/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-119/finalcif/app_path.py
+-rw-r--r--   0        0        0    91866 2020-02-02 00:00:00.000000 finalcif-119/finalcif/appwindow.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 finalcif-119/finalcif/finalcif_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/all_cif_dicts.py
+-rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/atoms.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cif_dict_foo.py
+-rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cif_file_io.py
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cif_order.py
+-rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/core_dict.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/hkl.py
+-rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/modulation_dict.py
+-rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/powder_dict.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/reference.py
+-rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/restraints_dict.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/text.py
+-rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/twin_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/checkcif/__init__.py
+-rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/checkcif/checkcif.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/__init__.py
+-rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/deposit.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/deposit_check.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/deposition_list.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/doi.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/upload.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-119/finalcif/cif/cod/website_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/__init__.py
+-rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/bruker_data.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/bruker_frame.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/ccdc_mail.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/data.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/p4p_reader.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/sadabs.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/saint.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/shelx_lst.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-119/finalcif/datafiles/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/__init__.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/sdm.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-119/finalcif/displaymol/vtk_molecule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/__init__.py
+-rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/author_loop_templates.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/equipment.py
+-rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/properties.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-119/finalcif/equip_property/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/__init__.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/combobox.py
+-rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/custom_classes.py
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/dialogs.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/equipmenttable.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/file_editor.py
+-rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/finalcif_gui_ui.py
+-rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/finalcif_gui_ui.ui
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loop_creator.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loop_creator_ui.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loop_creator_ui.ui
+-rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/loops.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/mainstackwidget.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/mixins.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/new_key_dialog.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/new_key_dialog_ui.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/new_key_dialog_ui.ui
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/plaintextedit.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/playground.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/propertytable.py
+-rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/text_templates_ui.py
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/text_templates_ui.ui
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/text_value_editor.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-119/finalcif/gui/vrf_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/__init__.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/finalcif.png
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/finalcif2.ico
+-rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/finalcif2.png
+-rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/multitable.ico
+-rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/multitable.png
+-rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-119/finalcif/icon/multitable.xcf
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/archive_report.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/mtools.py
+-rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/references.py
+-rw-r--r--   0        0        0    22298 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/report_text.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/symm.py
+-rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/tables.py
+-rw-r--r--   0        0        0    26776 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/templated_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/gui/__init__.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/gui/mainwindow.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-119/finalcif/report/gui/mainwindow.ui
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/__init__.py
+-rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/mathml2omml.xsl
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/template1.docx
+-rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/template_text.docx
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/template_without_text.docx
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-119/finalcif/template/templates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/__init__.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/download.py
+-rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/dsrmath.py
+-rw-r--r--   0        0        0    32789 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/misc.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/options.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/platon.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/pupdate.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/settings.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/shred.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/space_groups.py
+-rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/spgr_format.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/statusbar.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-119/finalcif/tools/sumformula.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-119/.gitignore
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-119/LICENSE
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-119/README.md
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 finalcif-119/pyproject.toml
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 finalcif-119/PKG-INFO
```

### Comparing `finalcif-118.post1/finalcif/app_path.py` & `finalcif-119/finalcif/app_path.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/appwindow.py` & `finalcif-119/finalcif/appwindow.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/finalcif_start.py` & `finalcif-119/finalcif/finalcif_start.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/all_cif_dicts.py` & `finalcif-119/finalcif/cif/all_cif_dicts.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/atoms.py` & `finalcif-119/finalcif/cif/atoms.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cif_dict_foo.py` & `finalcif-119/finalcif/cif/cif_dict_foo.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cif_file_io.py` & `finalcif-119/finalcif/cif/cif_file_io.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cif_order.py` & `finalcif-119/finalcif/cif/cif_order.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/core_dict.py` & `finalcif-119/finalcif/cif/core_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/hkl.py` & `finalcif-119/finalcif/cif/hkl.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/modulation_dict.py` & `finalcif-119/finalcif/cif/modulation_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/powder_dict.py` & `finalcif-119/finalcif/cif/powder_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/reference.py` & `finalcif-119/finalcif/cif/reference.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/restraints_dict.py` & `finalcif-119/finalcif/cif/restraints_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/text.py` & `finalcif-119/finalcif/cif/text.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/twin_dict.py` & `finalcif-119/finalcif/cif/twin_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/checkcif/checkcif.py` & `finalcif-119/finalcif/cif/checkcif/checkcif.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cod/deposit.py` & `finalcif-119/finalcif/cif/cod/deposit.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cod/deposit_check.py` & `finalcif-119/finalcif/cif/cod/deposit_check.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cod/deposition_list.py` & `finalcif-119/finalcif/cif/cod/deposition_list.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cod/doi.py` & `finalcif-119/finalcif/cif/cod/doi.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cod/upload.py` & `finalcif-119/finalcif/cif/cod/upload.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/cif/cod/website_parser.py` & `finalcif-119/finalcif/cif/cod/website_parser.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/bruker_data.py` & `finalcif-119/finalcif/datafiles/bruker_data.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/bruker_frame.py` & `finalcif-119/finalcif/datafiles/bruker_frame.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/ccdc_mail.py` & `finalcif-119/finalcif/datafiles/ccdc_mail.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/data.py` & `finalcif-119/finalcif/datafiles/data.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/p4p_reader.py` & `finalcif-119/finalcif/datafiles/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/sadabs.py` & `finalcif-119/finalcif/datafiles/sadabs.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/saint.py` & `finalcif-119/finalcif/datafiles/saint.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/shelx_lst.py` & `finalcif-119/finalcif/datafiles/shelx_lst.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/datafiles/utils.py` & `finalcif-119/finalcif/datafiles/utils.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/displaymol/molecule2D.py` & `finalcif-119/finalcif/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/displaymol/sdm.py` & `finalcif-119/finalcif/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/displaymol/vtk_molecule.py` & `finalcif-119/finalcif/displaymol/vtk_molecule.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/equip_property/author_loop_templates.py` & `finalcif-119/finalcif/equip_property/author_loop_templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/equip_property/equipment.py` & `finalcif-119/finalcif/equip_property/equipment.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/equip_property/properties.py` & `finalcif-119/finalcif/equip_property/properties.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/equip_property/tools.py` & `finalcif-119/finalcif/equip_property/tools.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/combobox.py` & `finalcif-119/finalcif/gui/combobox.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/custom_classes.py` & `finalcif-119/finalcif/gui/custom_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/dialogs.py` & `finalcif-119/finalcif/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/equipmenttable.py` & `finalcif-119/finalcif/gui/equipmenttable.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/file_editor.py` & `finalcif-119/finalcif/gui/file_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/finalcif_gui_ui.py` & `finalcif-119/finalcif/gui/finalcif_gui_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/finalcif_gui_ui.ui` & `finalcif-119/finalcif/gui/finalcif_gui_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/loop_creator.py` & `finalcif-119/finalcif/gui/loop_creator.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/loop_creator_ui.py` & `finalcif-119/finalcif/gui/loop_creator_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/loop_creator_ui.ui` & `finalcif-119/finalcif/gui/loop_creator_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/loops.py` & `finalcif-119/finalcif/gui/loops.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/mainstackwidget.py` & `finalcif-119/finalcif/gui/mainstackwidget.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/mixins.py` & `finalcif-119/finalcif/gui/mixins.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/new_key_dialog.py` & `finalcif-119/finalcif/gui/new_key_dialog.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/new_key_dialog_ui.py` & `finalcif-119/finalcif/gui/new_key_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/new_key_dialog_ui.ui` & `finalcif-119/finalcif/gui/new_key_dialog_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/plaintextedit.py` & `finalcif-119/finalcif/gui/plaintextedit.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/playground.py` & `finalcif-119/finalcif/gui/playground.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/propertytable.py` & `finalcif-119/finalcif/gui/propertytable.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/text_templates_ui.py` & `finalcif-119/finalcif/gui/text_templates_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/text_templates_ui.ui` & `finalcif-119/finalcif/gui/text_templates_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/text_value_editor.py` & `finalcif-119/finalcif/gui/text_value_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/gui/vrf_classes.py` & `finalcif-119/finalcif/gui/vrf_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/icon/finalcif.png` & `finalcif-119/finalcif/icon/finalcif.png`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/icon/finalcif2.ico` & `finalcif-119/finalcif/icon/finalcif2.ico`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/icon/finalcif2.png` & `finalcif-119/finalcif/icon/finalcif2.png`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/icon/multitable.ico` & `finalcif-119/finalcif/icon/multitable.ico`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/icon/multitable.png` & `finalcif-119/finalcif/icon/multitable.png`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/icon/multitable.xcf` & `finalcif-119/finalcif/icon/multitable.xcf`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/report/archive_report.py` & `finalcif-119/finalcif/report/archive_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/report/mtools.py` & `finalcif-119/finalcif/report/mtools.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/report/references.py` & `finalcif-119/finalcif/report/references.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,24 +50,24 @@
     At the end of the document, a numbered list of references can be generated with self.make_make_literature_list().
     """
 
     def __init__(self, paragraph: Paragraph):
         self.paragraph = paragraph
         self._references = list()
 
-    def append(self, ref: Union[List, Tuple]) -> None:
+    def append(self, ref: Union[List['ReferenceFormatter'], Tuple['ReferenceFormatter'], 'ReferenceFormatter']) -> None:
         """Adds a superscript list of reference numbers in brackets to the document."""
         if isinstance(ref, (list, tuple)):
             if not ref:
                 return None
             self._append_list(ref)
         else:
             if ref not in self._references:
                 self._references.append(ref)
-            self.paragraph.add_run('[{}]'.format(self._references.index(ref) + 1)).font.superscript = True
+            self.paragraph.add_run(f'[{self._references.index(ref) + 1}]').font.superscript = True
         # better not here:
         # self.paragraph.add_run(' ')
 
     def _append_list(self, reflist: List) -> None:
         reflst_long = []
         self.paragraph.add_run('[').font.superscript = True
         reflist = [x for x in reflist if x]
@@ -100,30 +100,30 @@
             with suppress(IndexError):
                 nextnext = int(stringlist[n + 2])
             # a sequence starts:
             if nextnext == val + 2 and not start:
                 start = val
             # in a sequence and next value is not +1 -> squence ends with val:
             if start and nextval != val + 1:
-                folg.append('{}-{}'.format(start, val))
+                folg.append(f'{start}-{val}')
                 start = 0
                 continue
             # everything outside a sequence:
             if not start:
                 folg.append(val)
         return ','.join([str(x) for x in folg])
 
     def make_literature_list(self, document):
         if len(self._references) < 10:
             template = 'references_ni'
         else:
             template = 'references'
         for num, ref in enumerate(self._references, 1):
             paragraph_reflist = document.add_paragraph('', template)
-            paragraph_reflist.add_run('[{}] \t'.format(str(num)))
+            paragraph_reflist.add_run(f'[{str(num)}] \t')
             ref.add_reference(paragraph_reflist)
             # paragraph_reflist.add_run('\n')
 
 
 class ReferenceFormatter():
     def __init__(self):
         self.authors = ''
@@ -286,14 +286,15 @@
         self.authors = ('F. Kleemiss, O. V. Dolomanov, M. Bodensteiner, N. Peyerimhoff, L. Midgley, L. J. Bourhis, '
                         'A. Genoni, L. A. Malaspina, D. Jayatilaka, J. L. Spencer, F. White, B. Grundkotter-Stock, '
                         'S. Steinhauer, D. Lentz, H. Puschmann, S. Grabowsky')
         self.journal = 'Chem. Sci.'
         self.year = '2021'
         self.volume = '12'
         self.pages = '1675–1692'
+        self.title = 'Accurate crystal structures and chemical properties from NoSpherA2'
 
 
 class SAINTReference(ReferenceFormatter):
     def __init__(self, name: str, version: str):
         """
         >>> SAINTReference('SAINT', 'V7.68a')
         Bruker, SAINT, V7.68a, Bruker AXS Inc., Madison, Wisconsin, USA.
@@ -528,18 +529,18 @@
 
 class CrysalisProReference(ReferenceFormatter):
     """
     >>> CrysalisProReference(version='1.171.40.68a', year='2019')
     Crysalispro, 1.171.40.68a, 2019, Rigaku OD.
     """
 
-    def __init__(self, version: str, year: str):
+    def __init__(self, version: str, year: str, pages: str = 'Rigaku OD'):
         super().__init__()
         self.authors = 'Crysalispro'
         self.journal = version
         self.year = year
-        self.pages = 'Rigaku OD'
+        self.pages = pages
 
 
 if __name__ == '__main__':
-    r = ReferenceList.get_sequence([1, 2, 3, 4])
+    r = ReferenceList.get_sequence([1, 2, 3, 6])
     print(r)
```

### Comparing `finalcif-118.post1/finalcif/report/report_text.py` & `finalcif-119/finalcif/report/report_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 from builtins import str
-from typing import Union, List
+from typing import Union, List, Tuple
 
 import gemmi
 from docx import Document
 from docx.text.paragraph import Paragraph
 from docx.text.run import Run
 from lxml import etree
 from shelxfile.atoms.atoms import Atom as SHXAtom
 
 from finalcif.app_path import application_path
 from finalcif.cif.cif_file_io import CifContainer
 from finalcif.cif.text import retranslate_delimiter, string_to_utf8
 from finalcif.report.references import DummyReference, SAINTReference, SORTAVReference, ReferenceList, CCDCReference, \
     SHELXLReference, SHELXTReference, SHELXSReference, FinalCifReference, ShelXleReference, Olex2Reference, \
-    SHELXDReference, SadabsTwinabsReference, CrysalisProReference, Nosphera2Reference, XDSReference
-from finalcif.tools.misc import protected_space, angstrom, zero_width_space, remove_line_endings
+    SHELXDReference, SadabsTwinabsReference, CrysalisProReference, Nosphera2Reference, XDSReference, DSRReference2015, \
+    DSRReference2018
+from finalcif.tools.misc import protected_space, angstrom, zero_width_space, remove_line_endings, flatten
 
 
 def math_to_word(eq: str) -> str:
     """Transform a sympy equation to be printed in word document."""
     tree = etree.fromstring(eq)
     xslt = etree.parse(os.path.join(application_path, 'template/mathml2omml.xsl'))
     transform = etree.XSLT(xslt)
@@ -84,27 +85,28 @@
         if not temperature:
             temperature = '[No _diffrn_ambient_temperature given]'
         shape = gstr(self.cif['_exptl_crystal_description'])
         if not shape:
             shape = '[No _exptl_crystal_description given]'
         colour = gstr(self.cif['_exptl_crystal_colour'])
         crystal_mount = gstr(self.cif['_diffrn_measurement_specimen_support'])
-        #adhesive = gstr(self.cif['_diffrn_measurement_specimen_adhesive'])
-        #if not adhesive:
+        # adhesive = gstr(self.cif['_diffrn_measurement_specimen_adhesive'])
+        # if not adhesive:
         #    adhesive = '[No _diffrn_measurement_specimen_adhesive given]'
         if not crystal_mount:
             crystal_mount = '[No _diffrn_measurement_specimen_support given]'
         method = 'shock-cooled '
         try:
             if float(temperature.split('(')[0]) > 200:
                 method = ''
         except ValueError:
             method = ''
-        txt_crystal = (f"A {colour}{', ' if colour else ''}{shape} shaped crystal of {self.cif.block.name} was mounted on a "
-                       f"{crystal_mount} with perfluoroether oil. ")
+        txt_crystal = (
+            f"A {colour}{', ' if colour else ''}{shape} shaped crystal of {self.cif.block.name} was mounted on a "
+            f"{crystal_mount} with perfluoroether oil. ")
         txt_data = (f"Data were collected from a {method}single crystal at {temperature}{protected_space}K ")
         paragraph.add_run(retranslate_delimiter(txt_crystal))
         Crystallization(cif, paragraph)
         paragraph.add_run(retranslate_delimiter(txt_data))
 
 
 class MachineType():
@@ -178,55 +180,64 @@
         if 'XDS' in integration:
             data_reduct_ref = XDSReference()
             integration_prog = 'XDS'
         if 'CrysAlisPro'.lower() in integration.lower():
             data_reduct_ref, absorpt_ref, integration_prog = self.add_crysalispro_reference(integration)
         absdetails = cif['_exptl_absorpt_process_details'].replace('-', ' ')
         if 'SADABS' in absdetails.upper() or 'TWINABS' in absdetails.upper():
-            #if len(absdetails.split()) > 1:
+            # if len(absdetails.split()) > 1:
             #    version = absdetails.split()[1]
-            #else:
+            # else:
             #    version = 'unknown version'
             if 'SADABS' in absdetails:
                 scale_prog = 'SADABS'
             else:
                 scale_prog = 'TWINABS'
             # absorpt_ref = SAINTReference(scale_prog, version)
             absorpt_ref = SadabsTwinabsReference()
         if 'SORTAV' in absdetails.upper():
             scale_prog = 'SORTAV'
             absorpt_ref = SORTAVReference()
         if 'crysalis' in abs_details.lower():
             scale_prog = 'SCALE3 ABSPACK'
-        sentence = 'All data were integrated with {} and {} {} absorption correction using {} was applied.'
-        txt = sentence.format(integration_prog,
-                              get_inf_article(abstype),
-                              abstype,
-                              scale_prog)
+        txt = (f'All data were integrated with {integration_prog} and {get_inf_article(abstype)} '
+               f'{abstype} absorption correction using {scale_prog} was applied.')
         paragraph.add_run(retranslate_delimiter(txt))
         ref.append([data_reduct_ref, absorpt_ref])
 
     def add_saint_reference(self, integration):
         saintversion = 'unknown version'
         if len(integration.split()) > 1:
             saintversion = integration.split()[1]
         integration_prog = 'SAINT'
         data_reduct_ref = SAINTReference('SAINT', saintversion)
         return data_reduct_ref, integration_prog
 
-    def add_crysalispro_reference(self, integration):
+    def add_crysalispro_reference(self, integration: str) -> Tuple[CrysalisProReference, CrysalisProReference, str]:
+        """
+        CrysAlisPro, Agilent Technologies,Version 1.171.37.31h (release 21-03-2014 CrysAlis171 .NET)
+            (compiled Mar 21 2014,18:13:45)
+        CrysAlisPro 1.171.42.58a (Rigaku OD, 2022)
+        """
         year = 'unknown version'
-        if len(integration.split()) > 3:
-            year = integration.split()[4][:-1]
         version = 'unknown year'
-        if len(integration.split()) >= 1:
+        pages = 'Rigaku OD'
+        length = len(integration.split())
+        if 3 < length <= 5:
+            year = integration.split()[4][:-1]
             version = integration.split()[1][:-1]
+        elif length > 8 and 'agilent' in integration.lower():
+            pages = 'Agilent Technologies'
+            year = integration.split()[5]
+            if '-' in year:
+                year = year.split('-')[-1]
+            version = integration.split()[3]
         integration_prog = 'Crysalispro'
-        data_reduct_ref = CrysalisProReference(version=version, year=year)
-        absorpt_ref = CrysalisProReference(version=version, year=year)
+        data_reduct_ref = CrysalisProReference(version=version, year=year, pages=pages)
+        absorpt_ref = CrysalisProReference(version=version, year=year, pages=pages)
         return data_reduct_ref, absorpt_ref, integration_prog
 
 
 class SolveRefine():
     def __init__(self, cif: CifContainer, paragraph: Paragraph, ref: ReferenceList):
         self.cif = cif
         refineref = DummyReference()
@@ -240,81 +251,84 @@
         if 'SHELXD' in solution_prog.upper():
             solveref = SHELXDReference()
         refined = gstr(self.cif['_computing_structure_refinement']) or '??'
         if refined.upper().startswith(('SHELXL', 'XL')):
             refineref = SHELXLReference()
         if 'OLEX' in refined.upper():
             refineref = Olex2Reference()
-        if 'NOSPHERA2' in solution_prog.upper() or 'NOSPHERA2' in self.cif['_refine_special_details'].upper():
-            refineref = Nosphera2Reference()
+        if 'NOSPHERA2' in solution_prog.upper() or 'NOSPHERA2' in self.cif['_refine_special_details'].upper() \
+                or 'NOSPHERA2' in self.cif['_olex2_refine_details'].upper():
+            refineref = [Olex2Reference(), Nosphera2Reference()]
         refine_coef = gstr(self.cif['_refine_ls_structure_factor_coef'])
-        sentence = r"The structure was solved by {} methods using {} and refined by full-matrix " \
-                   "least-squares methods against "
-        txt = sentence.format(solution_method.strip('\n\r'), solution_prog.split()[0])
+        newline = '\n\r'
+        txt = (f"The structure was solved by {solution_method.strip(newline)} methods using "
+               f"{solution_prog.split()[0]} and refined by full-matrix least-squares methods against ")
         paragraph.add_run(retranslate_delimiter(txt))
         paragraph.add_run('F').font.italic = True
         if refine_coef.lower() == 'fsqd':
             paragraph.add_run('2').font.superscript = True
-        paragraph.add_run(' by {}'.format(refined.split()[0]))
+        paragraph.add_run(f' by {refined.split()[0]}')
         shelxle = None
         if 'shelxle' in refined.lower() or 'shelxle' in self.cif['_computing_molecular_graphics'].lower():
             paragraph.add_run(' using ShelXle')
             shelxle = ShelXleReference()
         paragraph.add_run('.')
-        ref.append([solveref, refineref, shelxle])
+        ref.append(flatten([solveref, refineref, shelxle]))
 
 
 class Atoms():
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
         """
         Text for non-hydrogen atoms.
         """
         self.cif = cif
-        n_isotropic = self.number_of_isotropic_atoms()
+        self.n_isotropic = self.number_of_isotropic_atoms(without_h=True)
+        self.n_isotropic_with_h = self.number_of_isotropic_atoms(without_h=False)
         number = 'All'
         parameter_type = 'anisotropic'
-        if 0 < n_isotropic < self.cif.natoms(without_h=True):
-            number = f'Some atoms ({n_isotropic}) were refined using isotropic displacement parameters.' \
-                     ' All other'
-        if n_isotropic > 0 and n_isotropic > self.cif.natoms(without_h=True):
-            number = f'Most atoms ({n_isotropic}) were refined using isotropic displacement parameters.' \
-                     ' All other'
-        if n_isotropic == self.cif.natoms(without_h=True):
+        if 0 < self.n_isotropic < self.cif.natoms(without_h=True):
+            number = (f'Some atoms ({self.n_isotropic}) were refined using isotropic displacement parameters. '
+                      f'All other')
+        if self.n_isotropic > 0 and self.n_isotropic > self.cif.natoms(without_h=True):
+            number = (f'Most atoms ({self.n_isotropic}) were refined using isotropic displacement parameters. '
+                      f'All other')
+        if self.n_isotropic == self.cif.natoms(without_h=True):
             number = 'All'
             parameter_type = 'isotropic'
-        # TODO: test how many hydrogen atoms have ueq < -1.0 -> constrained or free refinement
-        #                                                       of hydrogen displacement params
-        # TODO: detect riding model of hydrogen atoms -> res file?
-        sentence1 = f"{number} non-hydrogen atoms were refined with {parameter_type} displacement parameters. "
+        non_h = 'non-hydrogen '
+        sentence1 = (f"{number} {non_h if self.n_isotropic_with_h > 0 else ''}atoms were refined with {parameter_type} "
+                     f"displacement parameters. ")
         paragraph.add_run(sentence1)
 
-    def number_of_isotropic_atoms(self) -> Union[float, int]:
+    def number_of_isotropic_atoms(self, without_h: bool = True) -> Union[float, int]:
         isotropic_count = 0
         for site in self.cif.atomic_struct.sites:
-            if self.atom_is_isotropic_and_not_hydrogen(site):
+            if self.atom_is_isotropic(site, without_h):
                 isotropic_count += 1
         return isotropic_count
 
     @staticmethod
-    def atom_is_isotropic_and_not_hydrogen(site):
-        return not site.aniso.nonzero() and not site.element.is_hydrogen
-
+    def atom_is_isotropic(site, without_h: bool):
+        if without_h:
+            return not site.aniso.nonzero() and not site.element.is_hydrogen
+        else:
+            return not site.aniso.nonzero()
 
 class Hydrogens():
     def __init__(self, cif: CifContainer, paragraph: Paragraph):
         """
         The hydrogen atoms were refined isotropically on calculated positions using
         a riding model with their Uiso values constrained to 1.5 times the Ueq of
         their pivot atoms for terminal sp3 carbon atoms and 1.2 times for all other
         carbon atoms.
         """
         self.cif = cif
         hatoms: List[SHXAtom] = [x for x in self.cif.shx.atoms.all_atoms if x.is_hydrogen]
         n_hatoms = len(hatoms)
-        n_anisotropic_h = len([x for x in hatoms if sum(x.uvals[1:]) > 0.0001])
+        n_anisotropic_h = len([x for x in hatoms if sum([abs(y) for y in x.uvals[1:]]) > 0.0001])
         n_constr_h = len([x for x in hatoms if x.uvals[0] < -1.0])
         riding_atoms = [x for x in hatoms if x.afix]
         pivot_atoms = self.get_hydrogen_pivot_atoms(riding_atoms)
         n_riding = len(riding_atoms)
         n_non_riding = len(hatoms) - n_riding
 
         atom_type = "carbon"
@@ -432,27 +446,28 @@
         paragraph.add_run(sentence1)
         ref.append(CCDCReference())
         SpaceChar(paragraph).regular()
         paragraph.add_run(sentence2)
 
 
 class FinalCifreport():
-    def __init__(self, paragraph: Paragraph, ref: ReferenceList):
+    def __init__(self, paragraph: Paragraph):
         sentence = "This report and the CIF file were generated using FinalCif."
         paragraph.add_run(sentence)
-        ref.append(FinalCifReference())
 
 
 class RefinementDetails():
     def __init__(self, cif: CifContainer, document: Document):
         ph = document.add_paragraph(style='Heading 2')
         ph.add_run(text=fr"Refinement details for {cif.block.name}")
         p = document.add_paragraph()
         p.style = document.styles['fliesstext']
         text = ' '.join(cif['_refine_special_details'].splitlines(keepends=False))
+        if cif['_olex2_refine_details']:
+            text += ' '.join(cif['_olex2_refine_details'].splitlines(keepends=False))
         # Replacing semicolon, because it can damage the CIF:
         text = text.replace(';', '.')
         p.add_run(string_to_utf8(text).strip())
 
 
 def get_inf_article(next_word: str) -> str:
     if not next_word:
@@ -464,7 +479,36 @@
 def format_radiation(radiation_type: str) -> list:
     radtype = list(radiation_type.partition("K"))
     if len(radtype) > 2:
         radtype[2] = retranslate_delimiter(radtype[2])
         return radtype
     else:
         return radtype
+
+
+def make_report_text(cif, document: Document) -> ReferenceList:
+    paragr = document.add_paragraph()
+    paragr.style = document.styles['fliesstext']
+    ref = ReferenceList(paragr)
+    # -- The main text:
+    paragr.add_run('The following text is only a suggestion: ').font.bold = True
+    CrstalSelection(cif, paragr)
+    MachineType(cif, paragr)
+    DataReduct(cif, paragr, ref)
+    SpaceChar(paragr).regular()
+    SolveRefine(cif, paragr, ref)
+    SpaceChar(paragr).regular()
+    if cif.hydrogen_atoms_present:
+        a = Atoms(cif, paragr)
+        if a.n_isotropic_with_h != 0 and (a.n_isotropic_with_h > a.n_isotropic):
+            Hydrogens(cif, paragr)
+            SpaceChar(paragr).regular()
+    if cif.disorder_present:
+        d = Disorder(cif, paragr)
+        if d.dsr_sentence:
+            ref.append([DSRReference2015(), DSRReference2018()])
+            SpaceChar(paragr).regular()
+    CCDC(cif, paragr, ref)
+    SpaceChar(paragr).regular()
+    FinalCifreport(paragr)
+    ref.append(FinalCifReference())
+    return ref
```

### Comparing `finalcif-118.post1/finalcif/report/symm.py` & `finalcif-119/finalcif/report/symm.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/report/tables.py` & `finalcif-119/finalcif/report/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 from docx.shared import Cm, Length, Pt
 from docx.table import Table, _Cell
 from docx.text.paragraph import Paragraph
 
 from finalcif.app_path import application_path
 from finalcif.cif.cif_file_io import CifContainer
 from finalcif.report.mtools import cif_keywords_list, format_space_group
-from finalcif.report.references import ReferenceList, DSRReference2018, DSRReference2015
-from finalcif.report.report_text import CCDC, CrstalSelection, DataReduct, Disorder, Hydrogens, \
-    MachineType, \
-    SolveRefine, format_radiation, FinalCifreport, SpaceChar, RefinementDetails, Atoms
+from finalcif.report.references import ReferenceList
+from finalcif.report.report_text import format_radiation, RefinementDetails, make_report_text
 from finalcif.report.templated_report import BondsAndAngles, TorsionAngles, HydrogenBonds
 from finalcif.tools.misc import protected_space, angstrom, bequal, sigma_sm, halbgeviert, degree_sign, ellipsis_mid, \
     less_or_equal, \
     timessym, lambdasym, this_or_quest, isnumeric, minus_sign, theta_symbol, grouper, open_file, pi_symbol, \
     ellipsis_char, medium_math_space
 from finalcif.tools.options import Options
 from finalcif.tools.settings import FinalCifSettings
@@ -98,15 +96,17 @@
         tab0_head = fr"Table {table_num}. Crystal data and structure refinement for {cif.block.name}"
         p.add_run(text=tab0_head)
     table_num = add_residuals_table(document, cif, table_num)
     p = document.add_paragraph()
     p.add_run().add_break(WD_BREAK.PAGE)
     if options.report_text:
         make_columns_section(document, columns='1')
-    if cif['_refine_special_details'] and cif['_refine_special_details'] != '?' and options.report_text:
+    if ((cif['_refine_special_details'] or cif['_olex2_refine_details']) and
+            (cif['_refine_special_details'] != '?') or
+            (cif['_olex2_refine_details'] != '?') and options.report_text):
         RefinementDetails(cif, document)
     table_num = add_coords_table(document, cif, table_num)
     if options.report_adp and len(tuple(cif.displacement_parameters())) > 0:
         table_num = add_adp_table(document, cif, table_num)
 
     if cif.symmops:
         if len(list(cif.bonds())) + len(list(cif.angles())) > 0:
@@ -148,41 +148,14 @@
     try:
         width = float(options.picture_width)
     except ValueError:
         width = 7.0
     pic.add_run().add_picture(str(picfile), width=Cm(width))
 
 
-def make_report_text(cif, document: Document) -> ReferenceList:
-    paragr = document.add_paragraph()
-    paragr.style = document.styles['fliesstext']
-    ref = ReferenceList(paragr)
-    # -- The main text:
-    paragr.add_run('The following text is only a suggestion: ').font.bold = True
-    CrstalSelection(cif, paragr)
-    MachineType(cif, paragr)
-    DataReduct(cif, paragr, ref)
-    SpaceChar(paragr).regular()
-    SolveRefine(cif, paragr, ref)
-    SpaceChar(paragr).regular()
-    if cif.hydrogen_atoms_present:
-        Atoms(cif, paragr)
-        Hydrogens(cif, paragr)
-        SpaceChar(paragr).regular()
-    if cif.disorder_present:
-        d = Disorder(cif, paragr)
-        if d.dsr_sentence:
-            ref.append([DSRReference2015(), DSRReference2018()])
-            SpaceChar(paragr).regular()
-    CCDC(cif, paragr, ref)
-    SpaceChar(paragr).regular()
-    FinalCifreport(paragr, ref)
-    return ref
-
-
 def create_document() -> Document:
     """
     Creates the report docx document.
 
     :return: The document instance.
     """
     try:
@@ -506,15 +479,15 @@
     col1_cells = coords_table.columns[1].cells
     col2_cells = coords_table.columns[2].cells
     col3_cells = coords_table.columns[3].cells
     col4_cells = coords_table.columns[4].cells
     rowidx = 1
     for at in atoms:
         c0, c1, c2, c3, c4 = col0_cells[rowidx], col1_cells[rowidx], col2_cells[rowidx], \
-                             col3_cells[rowidx], col4_cells[rowidx]
+            col3_cells[rowidx], col4_cells[rowidx]
         rowidx += 1
         c0.text = at[0]  # label
         c1.text = (str(at[2]))  # x
         c2.text = (str(at[3]))  # y
         c3.text = (str(at[4]))  # z
         c4.text = (str(at[7]))  # ueq
     p = document.add_paragraph()
@@ -711,15 +684,15 @@
     col1_cells = hydrogen_table.columns[1].cells
     col2_cells = hydrogen_table.columns[2].cells
     col3_cells = hydrogen_table.columns[3].cells
     col4_cells = hydrogen_table.columns[4].cells
     rowidx = 1
     for h in data.hydrogen_bonds_as_str:
         c0, c1, c2, c3, c4 = col0_cells[rowidx], col1_cells[rowidx], \
-                             col2_cells[rowidx], col3_cells[rowidx], col4_cells[rowidx]
+            col2_cells[rowidx], col3_cells[rowidx], col4_cells[rowidx]
         rowidx += 1
         c0.text = h.get('atoms')
         c0.paragraphs[0].add_run(h.get('symm')).font.superscript = True
         c1.text = h.get('dist_dh')
         c2.text = h.get('dist_ha')
         c3.text = h.get('dist_da')
         c4.text = h.get('angle_dha')
@@ -868,15 +841,15 @@
 if __name__ == '__main__':
     output_filename = 'tables.docx'
     import time
 
     settings = FinalCifSettings()
     options = Options(None, settings)
 
-    #make_report_from(options, CifContainer('test-data/hydrogen/some_riding_some_isotropic.cif'),
+    # make_report_from(options, CifContainer('test-data/hydrogen/some_riding_some_isotropic.cif'),
     #                 output_filename='test.docx')
     make_report_from(options, CifContainer('test-data/DK_Zucker2_0m.cif'), output_filename='test.docx')
     # make_report_from(options, CifContainer(r'C:\Users\daniel.kratzert\Downloads\hydrogen_bond_types\1218_31_7_0m.cif'), output_filename='test.docx')
     # make_report_from(options, CifContainer(r'C:\Users\daniel.kratzert\Downloads\rqt_c1_0m_sq_complete.cif'), output_filename='test.docx')
 
     # make_multi_tables(CifContainer('test-data/1000007-multi-finalcif.cif'))
     open_file(Path('test.docx'))
```

### Comparing `finalcif-118.post1/finalcif/report/templated_report.py` & `finalcif-119/finalcif/report/templated_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import re
 from collections import namedtuple
 from math import sin, radians
 from pathlib import Path
-from typing import List, Dict
+from typing import List, Dict, Union
 
 import jinja2
 from docx.enum.text import WD_PARAGRAPH_ALIGNMENT
 from docx.shared import Cm
 from docx.text.paragraph import Paragraph
 from docxtpl import DocxTemplate, RichText, InlineImage, Subdoc
 
@@ -53,15 +53,15 @@
         symms = {}
         for at1, at2, dist, symm2 in self.cif.bonds(without_h):
             dist = dist.replace('-', minus_sign)
             if symm2 in ('.', '?'):
                 symm2 = None
             num = symmsearch(self.cif, newsymms, num, symm2, symms)
             # Atom1 - Atom2:
-            a = '{}{}{}'.format(at1, halbgeviert, at2)
+            a = f'{at1}{halbgeviert}{at2}'
             symm = '#' + str(symms[symm2]) if symm2 else ''
             atoms = RichText(a)
             atoms.add(symm, superscript=True)
             bonds.append({'atoms': atoms, 'dist': dist})
             self.bonds_as_string.append({'atoms': a, 'symm': symm, 'dist': dist})
         self._symmlist.update(newsymms)
         return bonds
@@ -82,15 +82,15 @@
             num = symmsearch(self.cif, newsymms, num, symm2, symms)
             symm1_str = '#' + str(symms[symm1]) if symm1 else ''
             symm2_str = '#' + str(symms[symm2]) if symm2 else ''
             angle_val = ang.angle_val.replace('-', minus_sign)
             # atom1 symm1_str a symm2_str
             atoms = RichText(ang.label1)
             atoms.add(symm1_str, superscript=True)
-            a = '{}{}{}{}'.format(halbgeviert, ang.label2, halbgeviert, ang.label3)
+            a = f'{halbgeviert}{ang.label2}{halbgeviert}{ang.label3}'
             atoms.add(a, superscript=False)
             atoms.add(symm2_str, superscript=True)
             angles_list.append({'atoms': atoms, 'angle': angle_val})
             self.angles_as_string.append({'atom1': ang.label1,
                                           'atom2': a,
                                           'symm1': symm1_str,
                                           'symm2': symm2_str,
@@ -201,22 +201,25 @@
                                'dist_da': h.dist_da, 'angle_dha': h.angle_dha})
             self.hydrogen_bonds_as_str.append({'atoms'  : a, 'dist_dh': h.dist_dh, 'dist_ha': h.dist_ha,
                                                'dist_da': h.dist_da, 'angle_dha': h.angle_dha, 'symm': symmval})
         self._symmlist = newsymms
         return atoms_list
 
 
-def get_card(cif: CifContainer, symm: str) -> List[str]:
+def get_card(cif: CifContainer, symm: str) -> Union[List[str], None]:
     """
     Returns a symmetry card from the _space_group_symop_operation_xyz or _symmetry_equiv_pos_as_xyz list.
     :param cif: the cif file object
     :param symm: the symmetry number
     :return: ['x', ' y', ' z'] etc
     """
-    card = cif.symmops[int(symm.split('_')[0]) - 1].split(',')
+    try:
+        card = cif.symmops[int(symm.split('_')[0]) - 1].split(',')
+    except IndexError:
+        return None
     return card
 
 
 def get_symminfo(newsymms: dict) -> str:
     """
     Adds text about the symmetry generators used in order to add symmetry generated atoms.
     """
@@ -224,25 +227,29 @@
     nitems = len(newsymms)
     n = 0
     for key, value in newsymms.items():
         sep = ';'
         if n == nitems:
             sep = ''
         n += 1
-        line += "#{}: {}{}   ".format(key, value, sep)
+        line += f"#{key}: {value}{sep}   "
     if newsymms:
         return line
     else:
         return ''
 
 
 def symmsearch(cif: CifContainer, newsymms, num, symm, symms_list) -> int:
     if symm and symm not in symms_list.keys():
         symms_list[symm] = num
-        s = SymmetryElement(get_card(cif, symm))
+        card = get_card(cif, symm)
+        if card is None:
+            num += 1
+            return num
+        s = SymmetryElement(card)
         s.translate(symm)
         newsymms[num] = s.toShelxl()
         num += 1
     return num
 
 
 class TemplatedReport():
@@ -290,15 +297,15 @@
         spgr_word = math_to_word(spgrxml)
         # I have to create a subdocument in order to add the xml:
         sd = tpl_doc.new_subdoc()
         p: Paragraph = sd.add_paragraph()
         p.alignment = WD_PARAGRAPH_ALIGNMENT.LEFT
         p._element.append(spgr_word)
         try:
-            p.add_run(' ({})'.format(cif.spgr_number))
+            p.add_run(f' ({cif.spgr_number})')
         except AttributeError:
             pass
         return sd
 
     @staticmethod
     def get_from_to_theta_range(cif: CifContainer) -> str:
         theta_min = cif['_diffrn_reflns_theta_min']
@@ -439,15 +446,16 @@
 
     def refinement_prog(self, cif: CifContainer) -> str:
         refined = gstr(cif['_computing_structure_refinement']) or '??'
         if 'SHELXL' in refined.upper() or 'XL' in refined.upper():
             self.literature['refinement'] = SHELXLReference()
         if 'OLEX' in refined.upper():
             self.literature['refinement'] = Olex2Reference()
-        if 'NOSPHERA2' in refined.upper() or 'NOSPHERA2' in cif['_refine_special_details'].upper():
+        if ('NOSPHERA2' in refined.upper() or 'NOSPHERA2' in cif['_refine_special_details'].upper() or
+                'NOSPHERAT2' in cif['_olex2_refine_details'].upper()):
             self.literature['refinement'] = Nosphera2Reference()
         return refined.split()[0]
 
     def get_atomic_coordinates(self, cif: CifContainer):
         for at in cif.atoms(without_h=False):
             yield {'label': at.label,
                    'type' : at.type,
```

### Comparing `finalcif-118.post1/finalcif/report/gui/mainwindow.py` & `finalcif-119/finalcif/report/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/report/gui/mainwindow.ui` & `finalcif-119/finalcif/report/gui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/template/mathml2omml.xsl` & `finalcif-119/finalcif/template/mathml2omml.xsl`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/template/template1.docx` & `finalcif-119/finalcif/template/template1.docx`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/template/template_text.docx` & `finalcif-119/finalcif/template/template_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/template/template_without_text.docx` & `finalcif-119/finalcif/template/template_without_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/template/templates.py` & `finalcif-119/finalcif/template/templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/download.py` & `finalcif-119/finalcif/tools/download.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/dsrmath.py` & `finalcif-119/finalcif/tools/dsrmath.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/misc.py` & `finalcif-119/finalcif/tools/misc.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/options.py` & `finalcif-119/finalcif/tools/options.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/platon.py` & `finalcif-119/finalcif/tools/platon.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/pupdate.py` & `finalcif-119/finalcif/tools/pupdate.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/settings.py` & `finalcif-119/finalcif/tools/settings.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/shred.py` & `finalcif-119/finalcif/tools/shred.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/space_groups.py` & `finalcif-119/finalcif/tools/space_groups.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/spgr_format.py` & `finalcif-119/finalcif/tools/spgr_format.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/statusbar.py` & `finalcif-119/finalcif/tools/statusbar.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/finalcif/tools/sumformula.py` & `finalcif-119/finalcif/tools/sumformula.py`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/.gitignore` & `finalcif-119/.gitignore`

 * *Files identical despite different names*

### Comparing `finalcif-118.post1/README.md` & `finalcif-119/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ![Lates Release](https://img.shields.io/github/v/tag/dkratzert/FinalCif?label=Release)
 [![Unit Tests](https://github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml)
 ![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+[![PyPI package](https://repology.org/badge/version-for-repo/pypi/python:finalcif.svg)](https://repology.org/project/python:finalcif/versions)
 <a href="https://repology.org/project/finalcif/versions">
     <img src="https://repology.org/badge/vertical-allrepos/finalcif.svg" alt="Packaging status" align="right">
 </a>
 
 
 # FinalCif
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
 ![Lates Release](https://img.shields.io/github/v/tag/dkratzert/
 FinalCif?label=Release) [![Unit Tests](https://github.com/dkratzert/FinalCif/
 actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://
 github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml) !
-[Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+[Contributions](https://img.shields.io/badge/contributions-welcome-blue) [!
+[PyPI package](https://repology.org/badge/version-for-repo/pypi/python:
+finalcif.svg)](https://repology.org/project/python:finalcif/versions)
 [Packaging_status] # FinalCif FinalCif helps you to get a complete [CIF](https:
 //www.iucr.org/resources/cif) file from a single-xrystal X-ray diffraction
 experiment. See here [https://dkratzert.de/finalcif.html](https://dkratzert.de/
 finalcif.html) for details. For tables from multiple CIF files, you may want to
 use the program [multitable](https://github.com/dkratzert/multitable). **Report
 templates** You only need them if you want to make report tables that differ
 from the default ones. - [A template with everything in](https://github.com/
```

### Comparing `finalcif-118.post1/pyproject.toml` & `finalcif-119/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "finalcif"
-version = "118.post1"
+version = "119"
 authors = [
     { name = "Daniel Kratzert", email = "dkratzert@gmx.de" },
 ]
 description = "CIF file editor"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `finalcif-118.post1/PKG-INFO` & `finalcif-119/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalcif
-Version: 118.post1
+Version: 119
 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/FinalCif/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -36,14 +36,15 @@
 Requires-Dist: urllib3
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 ![Lates Release](https://img.shields.io/github/v/tag/dkratzert/FinalCif?label=Release)
 [![Unit Tests](https://github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml)
 ![Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+[![PyPI package](https://repology.org/badge/version-for-repo/pypi/python:finalcif.svg)](https://repology.org/project/python:finalcif/versions)
 <a href="https://repology.org/project/finalcif/versions">
     <img src="https://repology.org/badge/vertical-allrepos/finalcif.svg" alt="Packaging status" align="right">
 </a>
 
 
 # FinalCif
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: finalcif Version: 118.post1 Summary: CIF file
-editor Project-URL: Homepage, https://dkratzert.de/finalcif.html Project-URL:
-Bug Tracker, https://github.com/dkratzert/FinalCif/issues Author-email: Daniel
+Metadata-Version: 2.1 Name: finalcif Version: 119 Summary: CIF file editor
+Project-URL: Homepage, https://dkratzert.de/finalcif.html Project-URL: Bug
+Tracker, https://github.com/dkratzert/FinalCif/issues Author-email: Daniel
 Kratzert
 gmx.de> License-File: LICENSE Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-Python: >=3.9
 Requires-Dist: altgraph Requires-Dist: certifi Requires-Dist: chardet Requires-
 Dist: crossrefapi Requires-Dist: docxtpl Requires-Dist: future Requires-Dist:
@@ -14,15 +14,17 @@
 python-docx~=0.8 Requires-Dist: pywin32-ctypes~=0.2 Requires-Dist: qtawesome
 Requires-Dist: qtpy Requires-Dist: requests Requires-Dist: shelxfile Requires-
 Dist: urllib3 Requires-Dist: wheel Description-Content-Type: text/markdown !
 [Lates Release](https://img.shields.io/github/v/tag/dkratzert/
 FinalCif?label=Release) [![Unit Tests](https://github.com/dkratzert/FinalCif/
 actions/workflows/python-app_windows.yml/badge.svg?branch=master)](https://
 github.com/dkratzert/FinalCif/actions/workflows/python-app_windows.yml) !
-[Contributions](https://img.shields.io/badge/contributions-welcome-blue)
+[Contributions](https://img.shields.io/badge/contributions-welcome-blue) [!
+[PyPI package](https://repology.org/badge/version-for-repo/pypi/python:
+finalcif.svg)](https://repology.org/project/python:finalcif/versions)
 [Packaging_status] # FinalCif FinalCif helps you to get a complete [CIF](https:
 //www.iucr.org/resources/cif) file from a single-xrystal X-ray diffraction
 experiment. See here [https://dkratzert.de/finalcif.html](https://dkratzert.de/
 finalcif.html) for details. For tables from multiple CIF files, you may want to
 use the program [multitable](https://github.com/dkratzert/multitable). **Report
 templates** You only need them if you want to make report tables that differ
 from the default ones. - [A template with everything in](https://github.com/
```

