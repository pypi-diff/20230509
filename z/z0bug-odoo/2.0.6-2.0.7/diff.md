# Comparing `tmp/z0bug_odoo-2.0.6.tar.gz` & `tmp/z0bug_odoo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z0bug_odoo-2.0.6.tar", last modified: Thu Feb 23 08:32:59 2023, max compression
+gzip compressed data, was "dist/z0bug_odoo-2.0.7.tar", last modified: Tue May  9 16:04:15 2023, max compression
```

## Comparing `z0bug_odoo-2.0.6.tar` & `z0bug_odoo-2.0.7.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5923 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/asset_category.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6015 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_mode.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17914 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_21.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7818 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/date_range.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11354 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/res_partner.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5958 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_9.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12377 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_12.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.partner_mycompany.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    28222 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_2.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_method.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8641 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/res_country_state.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5736 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_term.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    26659 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_5.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/italy_profile_account.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5649 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_fiscal_position_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6034 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_term_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/decimal_precision.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5304 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/asset_asset.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6297 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/miscellaneous.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    21273 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_4.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6230 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_move_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9845 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_24.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6256 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_10.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5320 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/res_bank.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8169 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_5.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20091 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_6.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20415 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_10.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5183 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/date_range_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_3.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    23271 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_11.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    36713 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_account.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_18.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/res_partner_bank.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5806 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/purchase_order.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5098 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_fiscal_year.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    13357 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_26.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10816 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_19.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    40384 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/base.partner_admin.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5008 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/res_company.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    49021 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_6.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_14.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5548 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/product_supplierinfo.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6862 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_4.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/modules.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5485 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/withholding_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7139 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_journal.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_22.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7885 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/purchase_order_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    37268 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_8.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5063 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/stock_inventory.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5185 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/withholding_tax_rate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14221 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_16.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_15.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5681 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/asset_category_depreciation_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5797 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_16.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15336 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_1.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14581 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_1.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_15.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5420 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_rc_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10897 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_17.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5159 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_banking_mandate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4987 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9709 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_invoice_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8011 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/sale_order_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14993 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_3.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5289 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/dichiarazione_intento.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5496 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/res_currency_rate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7931 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_11.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6090 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_13.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_invoice.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5573 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_move.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7118 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_20.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9911 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_13.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12143 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_7.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10429 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_12.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7695 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_8.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5119 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_rc_type_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_14.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9180 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/product_product.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_7.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8985 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/product_template.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12852 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_2.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6097 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/sale_order.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5212 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/stock_inventory_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6561 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/data/account_fiscal_position.xlsx
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2311 2023-02-23 08:30:28.000000 z0bug_odoo-2.0.6/z0bug_odoo/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6398 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4491 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/z0bug_odoo_lib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/testenv/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)   106343 2023-02-22 20:24:56.000000 z0bug_odoo-2.0.6/z0bug_odoo/testenv/testenv.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       46 2022-12-21 12:44:21.000000 z0bug_odoo-2.0.6/z0bug_odoo/testenv/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    12824 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/test_common.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14660 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/run_pylint.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/openerp/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       68 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/openerp/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      174 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/README.md
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/pudb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/pdb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/pylint_deprecated_modules/ipdb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1515 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/git_run.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3601 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/get_test_dependencies.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2084 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/test_pylint
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8580 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/getaddons.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3134 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_test_dependencies
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6412 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/odoo_connection.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3551 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/apis.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2598 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/test_flake8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3827 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_run_tests
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_tnlbot.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7550 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/clone_oca_dependencies
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    28554 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/test_server.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      775 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      117 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3247 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_makepot
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      263 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      120 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_run_flake8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      833 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_helpers.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      780 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/z0bug_odoo/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-07 16:23:41.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       66 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6100 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/z0bug_odoo.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/setup.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2311 2023-02-21 04:57:54.000000 z0bug_odoo-2.0.6/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    98016 2023-02-23 08:32:59.000000 z0bug_odoo-2.0.6/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5923 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6015 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_mode.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17914 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_21.png
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     8512 2023-03-31 16:47:10.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/date_range.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11354 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5958 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_9.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12377 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_12.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.partner_mycompany.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    28222 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_2.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_method.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8641 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_country_state.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5736 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    26659 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_5.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/italy_profile_account.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5649 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6034 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/decimal_precision.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5304 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/asset_asset.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6297 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/miscellaneous.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    21273 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_4.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6230 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_move_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9845 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_24.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6256 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_10.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5320 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_bank.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8169 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_5.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20091 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_6.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20415 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_10.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5183 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/date_range_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_3.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    23271 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_11.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    36713 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_account.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_18.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner_bank.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5806 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5098 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_year.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    13357 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_26.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10816 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_19.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    40384 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/base.partner_admin.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5008 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_company.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    49021 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_6.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_14.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5548 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/product_supplierinfo.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6862 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_4.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/modules.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5485 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7139 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_journal.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_22.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7885 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    37268 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_8.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5063 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5185 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax_rate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14221 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_16.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_15.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5681 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category_depreciation_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5797 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_16.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15336 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_1.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14581 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_1.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_15.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5420 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10897 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_17.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5159 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_banking_mandate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4987 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9709 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8011 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14993 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_3.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5289 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5496 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/res_currency_rate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7931 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_11.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6090 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_13.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5573 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_move.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7118 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_20.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9911 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_13.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12143 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_7.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10429 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_12.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7695 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_8.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5119 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_14.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9180 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/product_product.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_7.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8985 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/product_template.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12852 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_2.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6097 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5212 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6561 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position.xlsx
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2311 2023-05-01 09:23:43.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-01 08:26:51.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4491 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/z0bug_odoo_lib.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/testenv/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   113219 2023-04-26 13:59:11.000000 z0bug_odoo-2.0.7/z0bug_odoo/testenv/testenv.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       46 2022-12-21 12:44:21.000000 z0bug_odoo-2.0.7/z0bug_odoo/testenv/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    12824 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/test_common.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14660 2023-04-15 07:25:23.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/run_pylint.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       68 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/openerp/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      174 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/README.md
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/pudb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/pdb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/pylint_deprecated_modules/ipdb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1515 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/git_run.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3601 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/get_test_dependencies.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2084 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/test_pylint
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8580 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/getaddons.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3134 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_test_dependencies
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6412 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/odoo_connection.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3551 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/apis.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2598 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/test_flake8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3843 2023-04-30 14:00:33.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_run_tests
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1863 2023-04-15 07:25:46.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_tnlbot.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7550 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/clone_oca_dependencies
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    28570 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/test_server.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      775 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      117 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3247 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_makepot
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      263 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      120 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_run_flake8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      833 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_helpers.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      780 2023-04-15 07:28:59.000000 z0bug_odoo-2.0.7/z0bug_odoo/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-07 16:23:41.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       66 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6100 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       44 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/z0bug_odoo.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-05-04 12:56:37.000000 z0bug_odoo-2.0.7/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-09 16:04:15.000000 z0bug_odoo-2.0.7/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    98395 2023-05-09 16:04:14.000000 z0bug_odoo-2.0.7/README.rst
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/asset_category.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_mode.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_mode.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_21.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_21.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/res_partner.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_9.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_9.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_12.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_12.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.partner_mycompany.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.partner_mycompany.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_2.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_2.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_method.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_method.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/res_country_state.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/res_country_state.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_term.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_5.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_5.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/italy_profile_account.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/italy_profile_account.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_fiscal_position_tax.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_payment_term_line.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_payment_term_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/decimal_precision.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/decimal_precision.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/asset_asset.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/asset_asset.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/miscellaneous.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/miscellaneous.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_4.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_4.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_tax.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_move_line.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_move_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_24.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_24.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_10.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_10.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/res_bank.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/res_bank.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_5.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_5.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_6.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_6.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_10.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_10.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/date_range_type.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/date_range_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_3.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_3.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_11.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_11.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_account.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_account.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_18.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_18.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/res_partner_bank.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/res_partner_bank.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/purchase_order.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_fiscal_year.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_year.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_26.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_26.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_19.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_19.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/base.partner_admin.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/base.partner_admin.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/res_company.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/res_company.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_6.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_6.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_14.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_14.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/product_supplierinfo.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/product_supplierinfo.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_4.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_4.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/modules.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/modules.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/withholding_tax.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_journal.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_journal.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_22.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_22.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/purchase_order_line.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/purchase_order_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_8.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_8.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/stock_inventory.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/withholding_tax_rate.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/withholding_tax_rate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_16.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_16.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_15.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_15.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/asset_category_depreciation_type.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/asset_category_depreciation_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_16.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_16.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_1.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_1.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_1.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_1.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_15.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_15.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_rc_type.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_17.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_17.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_banking_mandate.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_banking_mandate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_invoice_line.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/sale_order_line.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_3.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_3.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/dichiarazione_intento.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/dichiarazione_intento.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/res_currency_rate.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/res_currency_rate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_11.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_11.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_13.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_13.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_invoice.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_move.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_move.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_20.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_20.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_13.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_13.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_7.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_7.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_12.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_12.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_8.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_8.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_rc_type_tax.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_rc_type_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.res_partner_14.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.res_partner_14.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/product_product.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/product_product.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_7.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_7.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/product_template.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/product_template.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/z0bug.product_template_2.png` & `z0bug_odoo-2.0.7/z0bug_odoo/data/z0bug.product_template_2.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/sale_order.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/sale_order.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/stock_inventory_line.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/stock_inventory_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/data/account_fiscal_position.xlsx` & `z0bug_odoo-2.0.7/z0bug_odoo/data/account_fiscal_position.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/scripts/setup.info` & `z0bug_odoo-2.0.7/z0bug_odoo/scripts/setup.info`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0bug_odoo',
-    version='2.0.6',
+    version='2.0.7',
     description='Odoo testing framework',
     long_description="""
 Zeroincombenze(R) continuous testing framework for Odoo modules.
 
 Make avaiable test functions indipendent by Odoo version.
 """,
     classifiers=[
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/scripts/main.py` & `z0bug_odoo-2.0.7/z0bug_odoo/scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# template 20
+# template 21
 """
 Python supplemental features
 ----------------------------
 
 python_plus adds various features to python 2 and python 3 programs.
 It is designed to be used as integration of pypi future to help to port
 your code from Python 2 to Python 3 and still have it run on Python 2.
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -104,20 +104,28 @@
                             else:
                                 fd.write(help_text)
                         if verbose:
                             print("$ gzip -c %s > %s" % (full_fn, tgt_fn))
                         continue
                     if lib_path:
                         tgt_fn = os.path.join(lib_path, base)
-                        try:
-                            shutil.copy(full_fn, tgt_fn)
-                            if verbose:
-                                print("$ cp %s %s" % (full_fn, tgt_fn))
-                        except shutil.SameFileError:
-                            pass
+                        if sys.version_info[0] == 3:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except shutil.SameFileError:
+                                pass
+                        else:
+                            try:
+                                shutil.copy(full_fn, tgt_fn)
+                                if verbose:
+                                    print("$ cp %s %s" % (full_fn, tgt_fn))
+                            except BaseException:
+                                pass
                     # TODO> compatibility mode
                     tgt_fn = os.path.join(bin_path, base)
                     if os.path.isfile(tgt_fn):
                         os.unlink(tgt_fn)
                     if not os.path.exists(tgt_fn):
                         if verbose:
                             print("$ ln -s %s %s" % (full_fn, tgt_fn))
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/z0bug_odoo_lib.py` & `z0bug_odoo-2.0.7/z0bug_odoo/z0bug_odoo_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 from openpyxl import load_workbook
 
 
 from python_plus import unicodes
 
-__version__ = "2.0.6"
+__version__ = "2.0.7"
 
 
 class Z0bugOdoo(object):
     def __init__(self, release=None):
         try:
             import odoo.release as release
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/testenv/testenv.py` & `z0bug_odoo-2.0.7/z0bug_odoo/testenv/testenv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Test Environment v2.0.6
+"""Test Environment v2.0.7.1
 
 Copy this file in tests directory of your module.
 Please copy the documentation testenv.rst file too in your module.
 The __init__.py must import testenv.
 Your python test file should have to contain some following example lines:
 
 ::
@@ -92,22 +92,30 @@
 
 import os
 
 from future.utils import PY2, PY3
 from past.builtins import basestring, long
 
 from datetime import datetime, date
+import re
 import json
 import logging
 import base64
 import inspect
 
+from odoo import api
 from odoo.tools.safe_eval import safe_eval
 from odoo.modules.module import get_module_resource
-
+try:
+    import odoo.release as release
+except ImportError:
+    try:
+        import openerp.release as release
+    except ImportError:
+        release = None
 import python_plus
 from z0bug_odoo.test_common import SingleTransactionCase
 from z0bug_odoo import z0bug_odoo_lib
 
 # from clodoo import transodoo
 
 _logger = logging.getLogger(__name__)
@@ -151,29 +159,30 @@
 # Please, do not change fields order
 KEY_CANDIDATE = (
     "acc_number",
     "code_prefix",
     "default_code",
     "sequence",
     "login",
-    "description",
+    # "description",
     "depreciation_type_id",
     "number",
     "move_name",
     "partner_id",
     "product_id",
     "product_tmpl_id",
     "tax_src_id",
     "tax_dest_id",
     "code",
     "name",
 )
 KEY_OF_RESOURCE = {
     "res.users": "login",
     "account.tax": "description",
+    "account.rc.type.tax": "purchase_tax_id",
 }
 REC_KEY_NAME = {"id", "code", "name"}
 if PY3:  # pragma: no cover
     text_type = unicode = str
     bytestr_type = bytes
 elif PY2:  # pragma: no cover
     # unicode exist only for python2
@@ -185,28 +194,30 @@
     return hasattr(obj, "__iter__")
 
 
 class MainTest(SingleTransactionCase):
 
     def setUp(self):
         super(MainTest, self).setUp()
+        self.odoo_major_version = release.version_info[0] if release else 0
         self.debug_level = 0
         self.PYCODESET = "utf-8"
         self._logger = _logger
         self.setup_data_list = {}
         self.setup_data = {}
         self.setup_xrefs = {}
         self.struct = {}
         self.skeys = {}
         self.parent_name = {}
         self.parent_resource = {}
         self.childs_name = {}
         self.childs_resource = {}
         self.uninstallable_modules = []
         self.convey_record = {}
+        self.assert_counter = 0
         for item in self.__module__.split("."):
             if item not in ("odoo", "openerp", "addons"):
                 self.module = self.env["ir.module.module"].search(
                     [("name", "=", item)]
                 )[0]
                 if self.module:
                     break
@@ -222,14 +233,18 @@
         #     except ImportError:
         #         try:
         #             import openerp.release as release
         #             self.odoo_version = "%" % release.version_info[0]
         #         except ImportError:
         #             self.odoo_version = "16"
 
+    def tearDown(self):
+        super(MainTest, self).tearDown()
+        self._logger.info("🏆🥇 %d tests SUCCESSFULLY completed" % self.assert_counter)
+
     # ---------------------------------------
     # --  Unicode encode/decode functions  --
     # ---------------------------------------
     def u(self, s):  # pragma: no cover
         if isinstance(s, bytestr_type):
             if PY3:
                 return s.decode(self.PYCODESET)
@@ -250,15 +265,15 @@
 
     # ---------------------------
     # -- log/tracing functions --
     # ---------------------------
     def dict_2_print(self, values):  # pragma: no cover
         def to_str(obj):
             x = str(obj)
-            return x if (hasattr(obj, "len") and len(x) < 120) else "[...]"
+            return x if (hasattr(obj, "len") and len(x) < 150) else "[...]"
 
         if isinstance(values, dict):
             return json.dumps(values, default=to_str, indent=4)
         return values
 
     def log_lvl_3(self, mesg, strict=None):  # pragma: no cover
         if (self.debug_level >= 3 and not strict) or self.debug_level == 3:
@@ -288,14 +303,86 @@
             if ctr > 0:
                 break
 
     def raise_error(self, mesg):  # pragma: no cover
         self._logger.info("🛑 " + mesg)
         raise ValueError(mesg)
 
+    # ----------------------------------
+    # --  Counted assertion functions --
+    # ----------------------------------
+
+    def assertFalse(self, expr, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertFalse(expr, msg=msg)
+
+    def assertTrue(self, expr, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertTrue(expr, msg=msg)
+
+    def assertRaises(self, expected_exception, *args, **kwargs):     # pragma: no cover
+        self.assert_counter += 1
+        return super(MainTest, self).assertRaises(expected_exception, *args, **kwargs)
+
+    def assertEqual(self, first, second, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertEqual(first, second, msg=msg)
+
+    def assertNotEqual(self, first, second, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertNotEqual(first, second, msg=msg)
+
+    def assertIn(self, member, container, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertIn(member, container, msg=msg)
+
+    def assertNotIn(self, member, container, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertNotIn(member, container, msg=msg)
+
+    def assertIs(self, expr1, expr2, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertIs(expr1, expr2, msg=msg)
+
+    def assertIsNot(self, expr1, expr2, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertIsNot(expr1, expr2, msg=msg)
+
+    def assertLess(self, a, b, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertLess(a, b, msg=msg)
+
+    def assertLessEqual(self, a, b, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertLessEqual(a, b, msg=msg)
+
+    def assertGreater(self, a, b, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertGreater(a, b, msg=msg)
+
+    def assertGreaterEqual(self, a, b, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertGreaterEqual(a, b, msg=msg)
+
+    def assertIsNone(self, obj, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertIsNone(obj, msg=msg)
+
+    def assertIsNotNone(self, obj, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertIsNotNone(obj, msg=msg)
+
+    def assertIsInstance(self, obj, cls, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertIsInstance(obj, cls, msg=msg)
+
+    def assertNotIsInstance(self, obj, cls, msg=None):
+        self.assert_counter += 1
+        return super(MainTest, self).assertNotIsInstance(obj, cls, msg=msg)
+
     # ----------------------------
     # --  Conveyance functions  --
     # ----------------------------
     # def translate(self, resource, source, ttype=None, fld_name=False):
     #     if self.decl_version == self.odoo_version:
     #         return source
     #     return transodoo.translate_from_to(
@@ -342,14 +429,15 @@
         self._logger.info("⚠ xref '%s' -> '%s'" % (xref, conveyed_xref))
         ir_resource = "ir.model.data"
         if ir_resource not in self.convey_record:
             self.convey_record[ir_resource] = {}
         self.convey_record[ir_resource][xref] = conveyed_xref
         self._move_conveyed_xref(resource, xref, conveyed_xref, group=group)
 
+    @api.model
     def _get_conveyed_value(self, resource, field, value, fmt=None):
         if (
             resource in self.convey_record
             and field == "all"
             and field in self.convey_record[resource]
             and isinstance(value, dict)
             and hasattr(self, self.convey_record[resource][field])
@@ -383,14 +471,15 @@
                 ("state", "=", "installed"),
             ]
         ):
             self._add_conveyance(
                 "account.payment.term.line", "all", "_cvt_account_payment_term_line"
             )
 
+    @api.model
     def _cvt_account_payment_term_line(self, values):
         if values.get("months"):
             values["days"] = values["months"] * 30
             values["months"] = ""
             if values.get("option") in (
                 "fix_day_following_month",
                 "after_invoice_month",
@@ -418,50 +507,58 @@
                         " 🌍 parent_resource[%s] = %s"
                         % (resource, self.parent_resource[resource])
                     )
                     self.log_lvl_2(" 🌍 parent_name[%s] = %s" % (resource, field))
                     break
 
     def _search4childs(self, resource, childs_resource=None):
+        def _relation_prio(resource):
+            return childs_resource.index(resource)
+
         childs_resource = childs_resource or []
         if not childs_resource:
             if resource == "product.template":
                 childs_resource = ["product.product"]
             else:
-                for suffix in (".line", ".rate", ".state"):
+                for suffix in (".line", ".rate", ".state", ".tax"):
                     childs_resource.append(resource + suffix)
         if not isinstance(childs_resource, (list, tuple)):
             childs_resource = [childs_resource]  # pragma: no cover
         if resource not in self.childs_resource:
             for field in self.struct[resource].keys():
                 if self.struct[resource][field].get("relation", "/") in childs_resource:
-                    if resource not in self.childs_name or len(field) < len(
-                        self.childs_name[resource]
+                    candidate = self.struct[resource][field]["relation"]
+                    if (
+                        resource not in self.childs_name
+                        or _relation_prio(candidate) < _relation_prio(
+                            self.childs_resource[resource])
+                        or (_relation_prio(candidate) == _relation_prio(
+                            self.childs_resource[resource])
+                            and len(field) < len(self.childs_name[resource]))
                     ):
                         self.childs_name[resource] = field
-                        self.childs_resource[resource] = self.struct[resource][field][
-                            "relation"
-                        ]
+                        self.childs_resource[resource] = candidate
                         self.log_lvl_2(
                             " 🌍 childs_resource[%s] = %s"
                             % (resource, self.childs_resource[resource])
                         )
                         self.log_lvl_2(" 🌍 childs_name[%s] = %s" % (resource, field))
 
+    @api.model
     def _add_child_records(self, resource, xref, values, group=None):
         if resource not in self.childs_name:
             return values
         field = self.childs_name[resource]
         if values.get(field):
             return values
         values[field] = []
         childs_resource = self.childs_resource[resource]
         for child_xref in self.get_resource_data_list(childs_resource, group=group):
             if child_xref.startswith(xref):
-                record = self.resource_bind(
+                record = self.resource_browse(
                     child_xref,
                     raise_if_not_found=False,
                     resource=childs_resource,
                     group=group,
                 )
                 if record:
                     values[field].append((1, record.id, child_xref))
@@ -469,40 +566,42 @@
                     values[field].append((0, 0, child_xref))
         return values
 
     # --------------------------------
     # --  Data structure functions  --
     # --------------------------------
 
+    @api.model
     def _is_xref(self, xref):
         return (
             isinstance(xref, basestring)
-            and "." in xref
-            and " " not in xref
-            and len(xref.split(".")) == 2
+            and re.match(r"[\w]+\.[\w][^\s]+$", xref)
         )
 
+    @api.model
     def _unpack_xref(self, xref):
         # This is a 3 level external reference for header/detail relationship
         ln = xref.split("_")
         # Actual external reference for parent record
         xref = "_".join(ln[:-1])
         # Key to search for child record
         ln = ln[-1]
         if ln.isdigit():
-            ln = int(ln)
-            if not ln:                                               # pragma: no cover
-                return xref, False  # pragma: no cove
+            ln = int(ln) or False
+        elif isinstance(ln, basestring) and self._is_xref(ln):
+            ln = self._get_xref_id(self._get_model_of_xref(xref), xref=ln, fmt="id")
         return xref, ln
 
+    @api.model
     def _is_transient(self, resource):
         if isinstance(resource, basestring):
             return self.env[resource]._transient                     # pragma: no cover
         return resource._transient
 
+    @api.model
     def _add_xref(self, xref, xid, resource):
         """Add external reference ID that will be used in next tests.
         If xref exist, result ID will be upgraded"""
         module, name = xref.split(".", 1)
         if module == "external":
             return False
         ir_model = self.env["ir.model.data"]
@@ -514,21 +613,22 @@
         }
         xrefs = ir_model.search([("module", "=", module), ("name", "=", name)])
         if not xrefs:
             return ir_model.create(values)
         xrefs[0].write(values)  # pragma: no cover
         return xrefs[0]  # pragma: no cover
 
+    @api.model
     def _get_xref_id(self, resource, xref, fmt=None, group=None):
         res = xref
         if xref.isdigit() or (xref.startswith("-") and xref[1:].isdigit()):
             res = int(xref)
         elif self._is_xref(xref):
             if fmt:
-                res = self.resource_bind(
+                res = self.resource_browse(
                     xref,
                     raise_if_not_found=False,
                     resource=resource,
                     group=group,
                 )
                 if not res and not self.get_resource_data(resource, xref):
                     self._logger.info("⚠ External reference %s not found" % xref)
@@ -538,14 +638,15 @@
                 res = self.env.ref(
                     self._get_conveyed_value(resource, None, xref),
                     raise_if_not_found=False,
                 )
             res = res.id if res else False if fmt else xref
         return res
 
+    @api.model
     def _get_model_of_xref(self, xref):
         resource = name = ln = None
         if xref in self.setup_xrefs:
             group, resource = self.setup_xrefs[xref]
         if not resource:
             name, ln = self._unpack_xref(xref)
             if ln and name in self.setup_xrefs:
@@ -558,14 +659,15 @@
                 resource, res_id = self.env['ir.model.data'].xmlid_to_res_model_res_id(
                     name, raise_if_not_found=False)
                 resource = self.childs_resource.get(resource, resource)
             if resource:
                 self.setup_xrefs[xref] = (None, resource)
         return resource
 
+    @api.model
     def _get_depending_xref(self, resource, xref):
         resource_child = xref_child = field_child = field_parent = False
         if resource == "product.template":
             xref_child = xref.replace("_template", "_product")
             if xref_child == xref:
                 xref_child = xref.replace("template_", "product_")  # pragma: no cover
             if xref_child == xref:
@@ -630,14 +732,15 @@
                         break
 
     # ---------------------------------------------
     # --  Type <char> / <text> / base functions  --
     # ---------------------------------------------
     # Return unicode even on python2
 
+    @api.model
     def _cast_field(self, resource, field, value, fmt=None, group=None):
         ftype = self.struct[resource][field]["type"]
         if ftype not in ("text", "binary", "html"):
             value = self._get_conveyed_value(resource, field, value, fmt=fmt)
         if value is None or (
             isinstance(value, basestring)
             and (value in ("None", r"\N") or field == "id")
@@ -652,48 +755,54 @@
             value = self.default_company().id
         else:
             method = "_cast_field_%s" % ftype
             method = method if hasattr(self, method) else "_cast_field_base"
             value = getattr(self, method)(resource, field, value, fmt=fmt, group=group)
         return value
 
+    @api.model
     def _convert_field_to_write(self, record, field):
         value = record[field]
         if value is not None and value is not False:
             method = "_convert_%s_to_write" % record._fields[field].type
             method = method if hasattr(self, method) else "_convert_base_to_write"
             value = getattr(self, method)(record, field, value)
         return value
 
+    @api.model
     def _cast_field_base(self, resource, field, value, fmt=None, group=None):
         return value
 
+    @api.model
     def _upgrade_field_base(self, record, field, value):
         return value
 
+    @api.model
     def _convert_base_to_write(self, record, field, value):
         return value
 
     # ----------------------------------
     # --  Type <selection> functions  --
     # ----------------------------------
     # Return unicode even on python2
 
+    @api.model
     def _cast_field_selection(self, resource, field, value, fmt=None, group=None):
         if fmt and resource == "res.partner" and field == "lang":
             if not self.env["res.lang"].search([("code", "=", value)]):
                 self._logger.info("⚠ Invalid value %s" % value)
                 value = None
         return value
 
     # --------------------------------
     # --  Type <boolean> functions  --
     # --------------------------------
     # Return boolean
 
+    @api.model
     def _cast_field_boolean(self, resource, field, value, fmt=None, group=None):
         if isinstance(value, basestring):
             if value.isdigit():
                 value = int(value)
             elif (
                 not value
                 or value.lower().startswith("f")
@@ -705,43 +814,47 @@
         return value
 
     # --------------------------------
     # --  Type <integer> functions  --
     # --------------------------------
     # Return integer and/or long on python2
 
+    @api.model
     def _cast_field_integer(self, resource, field, value, fmt=None, group=None):
         if value and isinstance(value, basestring):
             value = int(value)
         return value
 
     # ------------------------------
     # --  Type <float> functions  --
     # ------------------------------
     # Return float
 
+    @api.model
     def _cast_field_float(self, resource, field, value, fmt=None, group=None):
         if value and isinstance(value, basestring):
             value = eval(value)
         return value
 
     # ---------------------------------
     # --  Type <monetary> functions  --
     # ---------------------------------
     # Return float
 
+    @api.model
     def _cast_field_monetary(self, resource, field, value, fmt=None, group=None):
         return self._cast_field_float(resource, field, value, fmt=fmt, group=group)
 
     # ---------------------------------
     # --  Type <datetime> functions  --
     # ---------------------------------
     # Return datetime (cast / upgrade)
     # Return datetime (convert Odoo 11+) or string (convert Odoo 10-)
 
+    @api.model
     def _cvt_to_datetime(self, value):
         if isinstance(value, date):
             if isinstance(value, datetime):
                 value = datetime(value.year,
                                  value.month,
                                  value.day,
                                  value.hour,
@@ -751,56 +864,62 @@
                 value = datetime(value.year, value.month, value.day, 0, 0, 0)
         elif isinstance(value, basestring):
             if len(value) <= 10:
                 value += " 00:00:00"
             value = datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
         return value
 
+    @api.model
     def _cast_field_datetime(self, resource, field, value, fmt=None, group=None):
         if isinstance(value, (list, tuple)) and fmt:
             value = self._cvt_to_datetime(self.compute_date(value[0], refdate=value[1]))
         else:
             value = self._cvt_to_datetime(self.compute_date(value))
         if PY2 and isinstance(value, datetime) and fmt == "cmd":     # pragma: no cover
             value = datetime.strftime(value, "%Y-%m-%d %H:%M:%S")
         return value
 
+    @api.model
     def _convert_datetime_to_write(self, record, field, value):
         return self._cvt_to_datetime(value)
 
     # -----------------------------
     # --  Type <date> functions  --
     # -----------------------------
     # Return date (cast / upgrade)
     # Return date (convert Odoo 11+) or string (convert Odoo 10-)
 
+    @api.model
     def _cvt_to_date(self, value):
         if isinstance(value, datetime):
             value = value.date()
         elif isinstance(value, basestring):
             value = datetime.strptime(value[:10], "%Y-%m-%d").date()
         return value
 
+    @api.model
     def _cast_field_date(self, resource, field, value, fmt=None, group=None):
         if isinstance(value, (list, tuple)) and fmt:
             value = self._cvt_to_date(self.compute_date(value[0], refdate=value[1]))
         else:
             value = self._cvt_to_date(self.compute_date(value))
         if PY2 and isinstance(value, date) and fmt == "cmd":         # pragma: no cover
             value = datetime.strftime(value, "%Y-%m-%d")
         return value
 
+    @api.model
     def _convert_date_to_write(self, record, field, value):
         return self._cvt_to_date(value)
 
     # -------------------------------
     # --  Type <binary> functions  --
     # -------------------------------
     # Return base64 (binary data) or string (filename with len<=64)
 
+    @api.model
     def _get_binary_filename(self, xref, bin_types=None):
         binary_root = get_module_resource(self.module.name, "tests", "data")
         if not bin_types:
             binary_file = os.path.join(binary_root, xref)
             if os.path.isfile(binary_file):
                 return binary_file
         bin_types = bin_types or ["png", "jpg", "xml"]
@@ -808,88 +927,98 @@
             bin_types = [bin_types]  # pragma: no cover
         for btype in bin_types:
             binary_file = os.path.join(binary_root, "%s.%s" % (xref, btype))
             if os.path.isfile(binary_file):
                 return binary_file
         return False  # pragma: no cover
 
+    @api.model
     def _get_binary_contents(self, value):
         if (
             not isinstance(value, basestring)
             or (PY3 and isinstance(value, bytes))
             or len(value) > 64
         ):
             return value
         bin_file = self._get_binary_filename(value)
         if bin_file:
             with open(bin_file, "rb") as fd:
                 bin_contents = python_plus._b(fd.read())
             return base64.b64encode(bin_contents)
         return False  # pragma: no cover
 
+    @api.model
     def _cast_field_binary(self, resource, field, value, fmt=None, group=None):
         bin_contents = self._get_binary_contents(value)
         if bin_contents:
             value = bin_contents
         else:
             value = None
         return value
 
     # ---------------------------------
     # --  Type <many2one> functions  --
     # ---------------------------------
     # Return int (fmt), string (for xref before bind)
 
+    @api.model
     def _cast_field_many2one(self, resource, field, value, fmt=None, group=None):
         if isinstance(value, basestring):
             value = self._get_xref_id(
                 self.struct[resource][field].get("relation", resource),
                 value,
                 fmt=fmt,
                 group=group,
             )
         elif (
             fmt in ("cmd", "py", "id")
             and not isinstance(value, (int, long))
             and is_iterable(value)
             and "id" in value
         ):
-            value = value.id
+            # Odoo 14.0 NewId requires origin
+            value = value.id if isinstance(value.id, (int, long)) else value.id.origin
         return value if value else None
 
+    @api.model
     def _convert_many2one_to_write(self, record, field, value):
-        return value.id if value else None
+        if not value:
+            return None
+        # Odoo 14.0 NewId requires origin
+        return value.id if isinstance(value.id, (int, long)) else value.id.origin
 
     # -----------------------------------------------
     # --  Type <one2many> / <many2many> functions  --
     # -----------------------------------------------
     # Return [*] (fmt), string (for xref before bind)
 
+    @api.model
     def _value2dict(self, resource, value, fmt=None, group=None):
         if isinstance(value, dict):
             return self.cast_types(resource, value, fmt=fmt)
         elif isinstance(value, basestring):
             return self.cast_types(
                 resource,
                 self.get_resource_data(resource, value, group=group),
                 fmt=fmt,
                 group=group,
             )
         return value                                                 # pragma: no cover
 
+    @api.model
     def _cast_2many(self, resource, field, value, fmt=None, group=None):
         """ "One2many and many2many may have more representations:
         * External reference (str) -> 1 value or None
         * list() or list (str)
         * - [0, 0, values (dict)]           # CREATE record and link
         * - [1, ID (int), values (dict)]    # UPDATE linked record
         * - [2, ID (int)]                   # DELETE linked record by ID
         * - [3, ID (int)]                   # UNLINK record ID (do not delete record)
         * - [4, ID (int)]                   # LINK record by ID
-        * - [5, x]                          # CLEAR unlink all record IDs
+        * - [5, x] or [5]                   # CLEAR unlink all record IDs
         * - [6, x, IDs (list)]              # SET link record IDs
         * - External reference (str) -> 1 value or None
         """
 
         def value2list(value):
             if isinstance(value, basestring):
                 value = [x for x in value.split(",")]
@@ -990,47 +1119,54 @@
                     res |= self.env[resource].browse(id)
         else:
             res = False
             if fmt:
                 self._logger.info("⚠ No *2many value for %s.%s" % (resource, value))
         return res
 
+    @api.model
     def _cast_field_one2many(self, resource, field, value, fmt=None, group=None):
         value = self._cast_2many(
             self.struct[resource][field]["relation"],
             field,
             value,
             fmt=fmt,
             group=group,
         )
         if not value:
             value = None
         return value
 
+    @api.model
     def _cast_field_many2many(self, resource, field, value, fmt=None, group=None):
         return self._cast_2many(
             self.struct[resource][field]["relation"],
             field,
             value,
             fmt=fmt,
             group=group
         )
 
+    @api.model
     def _convert_one2many_to_write(self, record, field, value):
         if value:
-            return [(6, 0, [x.id for x in value])]
+            return [(6, 0, [
+                x.id if isinstance(x.id, (int, long)) else x.id.origin
+                for x in value])]
         return False
 
+    @api.model
     def _convert_many2many_to_write(self, record, field, value):
         return self._convert_one2many_to_write(record, field, value)
 
     # -------------------------------------
     # --  ir.model / resource functions  --
     # -------------------------------------
 
+    @api.model
     def cast_types(self, resource, values, fmt=None, group=None):
         """Convert resource fields in appropriate type, based on Odoo type.
         The parameter fmt declares the purpose of casting: 'cmd' means convert to Odoo
         API format and 'py' means convert to native python format.
         When no format is required (fmt=None), some conversion may be not applicable:
         * many2one field will be leave unchanged if invalid xref is issued
         * 2many field me will be leave unchanged if one or more invalid xref is issued
@@ -1050,14 +1186,19 @@
             - "py": writable data to store directly in object
             - "id": like 'cmd' but does not add prefixes for Odoo API
             group (str): used to manager group data; default is "base"
 
         Returns:
             Dictionary values
         """
+        if not isinstance(values, dict):
+            self.raise_error(
+                "Invalid dict %s for %s!"
+                % (values, resource)  # pragma: no cover
+            )
         if values:
             self._load_field_struct(resource)
             values = self._get_conveyed_value(resource, "all", values, fmt=fmt)
             for field in [x for x in list(values.keys())]:
                 if field not in self.struct[resource]:
                     del values[field]
                     self.log_lvl_2(
@@ -1074,14 +1215,15 @@
                     continue
                 values[field] = value
             if not values:  # pragma: no cover
                 self.log_lvl_2(" 🕶️ %s.cast_type() = {}" % resource)
 
         return values
 
+    @api.model
     def _convert_to_write(self, record, new=None, orig=None):
         values = {}
         for field in list(record._fields.keys()):
             if (
                 field in BLACKLIST_COLUMNS
                 or record._fields[field].readonly
             ):
@@ -1093,41 +1235,44 @@
                 if new or (orig and value == self._convert_field_to_write(orig, field)):
                     continue
                 values[field] = value
             elif not orig or value != self._convert_field_to_write(orig, field):
                 values[field] = value
         return values
 
+    @api.model
     def _upgrade_record(self, record, values, default={}):
         for field in list(values.keys()):
             if field in SUPERMAGIC_COLUMNS:  # pragma: no cover
                 continue
             method = "_upgrade_field_%s" % record._fields[field].type
             method = method if hasattr(self, method) else "_upgrade_field_base"
             value = getattr(self, method)(record, field, values[field])
             if not value and default.get(field):
                 value = getattr(self, method)(record, field, default[field])
             if value is not None:
                 setattr(record, field, value)
         return record
 
+    @api.model
     def _purge_values(self, values, timed=None):
         for field in BITTER_COLUMNS:
             if field in values:
                 del values[field]
         if timed:  # pragma: no cover
             for field in LOG_ACCESS_COLUMNS:
                 if field in values:
                     del values[field]
         return values
 
     # --------------------------------------
     # --  Wizard/Form internal functions  --
     # --------------------------------------
 
+    @api.model
     def _ctx_active_ids(self, records, ctx={}):
         if records:
             if is_iterable(records):
                 ctx["active_ids"] = [x.id for x in records]
                 if len(records) == 1:
                     ctx["active_id"] = records[0].id
                 else:
@@ -1138,65 +1283,97 @@
 
     def _finalize_ctx_act_windows(self, records, act_windows, ctx={}):
         if isinstance(act_windows.get("context"), basestring):
             _ctx = self.env["ir.actions.actions"]._get_eval_context()
             _ctx.update(self._ctx_active_ids(records, ctx))
             _ctx.update(safe_eval(act_windows["context"], _ctx))
             act_windows["context"] = _ctx
-            if isinstance(records, (int, long)) != act_windows["multi"]:
+            if (
+                self.odoo_major_version < 13
+                and isinstance(records, (int, long)) != act_windows["multi"]
+            ):
                 self._logger.info("⚠ act_windows['multi'] does not match # of records!")
         elif "context" not in act_windows:
             act_windows["context"] = {}
 
+    @api.model
     def _create_object(self, resource, default={}, origin=None, ctx={}):
-        if ctx:
-            record = self.env[resource].with_context(ctx).new(values=default)
-        else:
-            record = self.env[resource].new(values=default)
-        if origin:
-            record._origin = origin
+        if self.odoo_major_version < 13:
+            if ctx:
+                record = self.env[resource].with_context(ctx).new(values=default)
+            else:
+                record = self.env[resource].new(values=default)
+            if origin:
+                record._origin = origin
+            else:
+                record._origin = self.env[resource].with_context(ctx)
         else:
-            record._origin = self.env[resource].with_context(ctx)
+            if ctx:
+                record = self.env[resource].with_context(ctx).new(
+                    values=default,
+                    origin=origin or self.env[resource].with_context(ctx))
+            else:
+                record = self.env[resource].new(
+                    values=default,
+                    origin=origin or self.env[resource].with_context(ctx))
         if hasattr(record, "default_get"):
             self._upgrade_record(
                 record, record.default_get(record.fields_get_keys()), default
             )
         for field in record._onchange_methods.values():
             for method in field:
                 method(record)
         return record
 
-    def _exec_action(self, record, action, default={}, web_changes=[], ctx={}):
+    @api.model
+    def for_xml_id(self, module, name):
+        if self.odoo_major_version < 13:
+            return self.env["ir.actions.act_window"].for_xml_id(module, name)
+        else:
+            record = self.env.ref("%s.%s" % (module, name))
+            return record.read()[0]
+
+    @api.model
+    def _set_origin(self, record, ctx={}):
         resource_model = self._get_model_from_records(record)
         origin = self.env[resource_model]
-        if self._is_transient(origin) and action in ("save", "create", "discard"):
-            self.raise_error(
-                "Invalid action %s for %s!"
-                % (action, resource_model)  # pragma: no cover
+        if is_iterable(record) and len(record) == 1:
+            origin = self._create_object(
+                resource_model,
+                default=self._convert_to_write(record[0], new=True),
+                origin=origin,
+                ctx=ctx,
             )
+        return origin
+
+    @api.model
+    def _exec_action(self, record, action, default={}, web_changes=[], origin=None,
+                     ctx={}):
+        resource_model = self._get_model_from_records(record)
+        origin = origin or self.env[resource_model]
         if isinstance(record, basestring):
             record = self._create_object(
                 resource_model,
                 default=self.cast_types(resource_model, default or {}, fmt="cmd"),
                 origin=origin,
                 ctx=ctx,
             )
         elif is_iterable(record):
             if not self._is_transient(origin):
                 if not isinstance(record, (list, tuple)):
                     _ctx = self.env["ir.actions.actions"]._get_eval_context()
                     _ctx.update(self._ctx_active_ids(record, ctx))
                     record = record.with_context(_ctx)
-                if len(record) == 1:
-                    origin = self._create_object(
-                        resource_model,
-                        default=self._convert_to_write(record[0], new=True),
-                        ctx=ctx,
-                    )
-                    record._origin = origin
+                if not origin or origin._name != resource_model:
+                    origin = self._set_origin(record, ctx=ctx)
+        if self._is_transient(origin) and action in ("save", "create", "discard"):
+            self.raise_error(
+                "Invalid action %s for %s!"
+                % (action, resource_model)  # pragma: no cover
+            )
         self._load_field_struct(resource_model)
         for args in web_changes:
             self._wiz_edit(
                 record,
                 resource_model,
                 args[0],
                 args[1],
@@ -1218,29 +1395,31 @@
             # Weird bug: this is a workaround!!!
             if action == "action_invoice_draft" and record.state != "draft":
                 record.state = "draft"
             elif action == "action_invoice_open" and record.state != "open":
                 record.state = "open"
         elif self._is_xref(action):
             module, name = action.split(".", 1)
-            act_windows = self.env["ir.actions.act_window"].for_xml_id(module, name)
+            act_windows = self.for_xml_id(module, name)
             self.log_lvl_2("🐜  act_windows(%s)" % action)
             self._finalize_ctx_act_windows(record, act_windows)
         else:  # pragma: no cover
             self.raise_error(
                 "Invalid action %s for %s!"
                 % (action, resource_model)  # pragma: no cover
             )
         return act_windows
 
+    @api.model
     def _get_model_from_act_windows(self, act_windows):
         return act_windows.get(
             "model_name", act_windows.get("res_model", act_windows.get("model"))
         )
 
+    @api.model
     def _get_src_model_from_act_windows(self, act_windows):
         model_name = act_windows.get(
             "src_model",
             act_windows.get(
                 "binding_model_id", self._get_model_from_act_windows(act_windows)
             ),
         )
@@ -1248,25 +1427,27 @@
             model_name = None
             value = "%s,%d" % (act_windows["type"], act_windows["id"])
             records = self.env["ir.values"].search([("value", "=", value)])
             if len(records) == 1:
                 model_name = records[0].model
         return model_name
 
+    @api.model
     def _get_model_from_records(self, records):
         if not records:  # pragma: no cover
             resource_model = None
         elif isinstance(records, basestring):
             resource_model = records
         elif isinstance(records, (list, tuple)):
             resource_model = records[0]._name
         else:
             resource_model = records._name
         return resource_model
 
+    @api.model
     def _wiz_launch(self, act_windows, records=None, default=None, ctx={}):
         """Start a wizard from a windows action.
 
         This function simulates the wizard or action server starting web interface.
         It creates the wizard record with default values.
         It is useful to test:
             * view names
@@ -1367,14 +1548,15 @@
         # Save wizard for furthermore use
         act_windows["_wizard_"] = wizard
         if act_windows.get("view_id"):
             # This code is just executed to test valid view structure
             self.env["ir.ui.view"].browse(act_windows["view_id"])  # pragma: no cover
         return act_windows
 
+    @api.model
     def _wiz_launch_by_act_name(
         self,
         module,
         action_name,
         records=None,
         default=None,
         ctx={},
@@ -1402,24 +1584,25 @@
             module (str): module name with wizard to test
             action_name (str): action name
             records (obj): objects supplied for action server
 
         Returns:
             Same of <wizard_start>
         """
-        act_model = "ir.actions.act_window"
+        # act_model = "ir.actions.act_window"
         module = self.module.name if module == "." else module
-        act_windows = self.env[act_model].for_xml_id(module, action_name)
+        act_windows = self.for_xml_id(module, action_name)
         return self._wiz_launch(
             act_windows,
             default=default,
             ctx=ctx,
             records=records,
         )
 
+    @api.model
     def _wiz_edit(self, wizard, resource, field, value, onchange=None):
         """Simulate view editing on a field.
 
         Assign value to field, then engage all onchange functions on current field and
         on all updated fields.
         Finally, run onchange function issued by caller.
         Internal function of <wizard_execution>
@@ -1453,14 +1636,15 @@
                     user_act = True
                     for method in wizard._onchange_methods[field]:
                         method(wizard)
                 cur_vals[field] = getattr(wizard, field)
         if onchange:  # pragma: no cover
             getattr(wizard, onchange)()
 
+    @api.model
     def _wiz_execution(
         self,
         act_windows,
         button_name=None,
         web_changes=[],
         button_ctx={},
     ):
@@ -1562,14 +1746,15 @@
                     parent[field_child] = []
                 if xref not in parent[field_child]:
                     parent[field_child].append(xref)
         if name not in self.setup_data_list[group]:
             self.setup_data_list[group].append(name)
         self.setup_xrefs[xref] = (group, resource)
 
+    @api.model
     def default_company(self):
         return self.env.user.company_id
 
     def compute_date(self, date, refdate=None):
         """Compute date
 
         Args:
@@ -1577,15 +1762,24 @@
             refdate (date or string): reference date
 
         Returns:
             ISO format string with result date
         """
         return python_plus.compute_date(self.u(date), refdate=self.u(refdate))
 
+    @api.model
     def resource_bind(self, xref, raise_if_not_found=True, resource=None, group=None):
+        self.log_lvl_1("resource_bind() is deprecated: please use resource_browse()")
+        return self.resource_browse(xref=xref,
+                                    raise_if_not_found=raise_if_not_found,
+                                    resource=resource,
+                                    group=group)
+
+    @api.model
+    def resource_browse(self, xref, raise_if_not_found=True, resource=None, group=None):
         """Bind record by xref or searching it or browsing it.
         This function returns a record using issued parameters. It works in follow ways:
 
         * With valid xref it work exactly like self.env.ref()
         * If xref is an integer it works exactly like self.browse()
         * I xref is invalid, xref is used to search record
             * xref is searched in stored data
@@ -1601,15 +1795,15 @@
         Returns:
             obj: the Odoo model record
 
         Raises:
             ValueError: if invalid parameters issued
         """
         self.log_stack()
-        self.log_lvl_3("🐞%s.resource_bind(%s)" % (resource, xref))
+        self.log_lvl_3("🐞%s.resource_browse(%s)" % (resource, xref))
         # Search for Odoo standard external reference
         record = None
         if isinstance(xref, (int, long)):
             if not resource:  # pragma: no cover
                 self.raise_error("No model issued for binding")
                 return False
             record = self.env[resource].browse(xref)
@@ -1642,15 +1836,15 @@
         key_field = self.skeys[resource][0]
         parent_name = self.parent_name.get(resource)
         if parent_name and self.parent_resource[resource] in self.childs_resource:
             name, x = self._unpack_xref(name)
             if not x:                                                # pragma: no cover
                 return False
             domain = [(key_field, "=", x)]
-            x = self.resource_bind(
+            x = self.resource_browse(
                 "%s.%s" % (module, name),
                 resource=self.parent_resource[resource],
                 raise_if_not_found=False,
                 group=group,
             )
             if not x:                                                # pragma: no cover
                 return False
@@ -1669,14 +1863,15 @@
         record = self.env[resource].search(domain)
         if len(record) == 1:
             return self.env[resource].browse(record[0].id)
         if raise_if_not_found:
             self.raise_error("External ID %s not found" % xref)  # pragma: no cover
         return False
 
+    @api.model
     def resource_create(self, resource, values=None, xref=None, group=None):
         """Create a test record and set external ID to next tests.
         This function works as standard Odoo create() with follow improvements:
 
         * It can create external reference too
         * It can use stored data if no values supplied
 
@@ -1727,14 +1922,15 @@
                 values_child = {k: v for (k, v) in values.items()}
                 values_child[field_parent] = res.id
                 self.store_resource_data(
                     resource_child, xref_child, values_child, group=group
                 )
         return res
 
+    @api.model
     def resource_write(
         self, resource, xref=None, values=None, raise_if_not_found=True, group=None
     ):
         """Update a test record.
         This function works as standard Odoo write() with follow improvements:
 
         * If resource is a record, xref is ignored (it should be None)
@@ -1755,15 +1951,15 @@
         Raises:
             ValueError: if invalid parameters issued
         """
         self.log_stack()
         if resource is None or isinstance(resource, basestring):
             if not xref and not values:                              # pragma: no cover
                 self.raise_error("%s.write() without values and xref" % resource)
-            record = self.resource_bind(
+            record = self.resource_browse(
                 xref,
                 resource=resource,
                 raise_if_not_found=raise_if_not_found,
                 group=group,
             )
         else:
             record = resource
@@ -1782,14 +1978,15 @@
             )
             if resource.startswith("account.move"):
                 record.with_context(check_move_validity=False).write(values)
             else:
                 record.write(values)
         return record
 
+    @api.model
     def resource_make(self, resource, xref, values=None, group=None):
         """Create or write a test record.
         This function is a hook to resource_write() or resource_create().
         """
         self.log_stack()
         self.log_lvl_3(
             "🐞%s.resource_make(%s,xref=%s)"
@@ -1869,14 +2066,15 @@
         for resource in message["TEST_SETUP_LIST"]:
             self.log_lvl_1(" 🐜 declare_all_data(%s,group=%s)" % (resource, group))
             item = "TEST_%s" % resource.upper().replace(".", "_")
             self.declare_resource_data(
                 resource, message[item], group=group, merge=merge
             )
 
+    @api.model
     def get_resource_data(self, resource, xref, group=None):
         """Get declared resource data; may be used to test compare.
 
         Args:
             resource (str): Odoo model name or name assigned, i.e. "res.partner"
             xref (str): external reference
             group (str): if supplied select specific group data; default is "base"
@@ -1892,14 +2090,15 @@
             group in self.setup_data
             and resource in self.setup_data[group]
             and xref in self.setup_data[group][resource]
         ):
             return self.setup_data[group][resource][xref]
         return {}  # pragma: no cover
 
+    @api.model
     def get_resource_data_list(self, resource, group=None):
         """Get declared resource data list.
 
         Args:
             resource (str): Odoo model name or name assigned, i.e. "res.partner"
             group (str): if supplied select specific group data; default is "base"
 
@@ -1907,14 +2106,15 @@
             list of data
         """
         group = group or "base"
         if group in self.setup_data and resource in self.setup_data[group]:
             return list(self.setup_data[group][resource].keys())
         return []  # pragma: no cover
 
+    @api.model
     def get_resource_list(self, group=None):
         """Get declared resource list.
 
         Args:
             group (str): if supplied select specific group data; default is "base"
         """
         group = group or "base"
@@ -1953,14 +2153,15 @@
                 "overwrite": overwrite,
             }
             self.env["base.language.install"].create(vals).lang_install()
         if force_translation:
             vals = {"lang": iso}
             self.env["base.update.translations"].create(vals).act_update()
 
+    @api.model
     def setup_company(
         self,
         company,
         xref=None,
         partner_xref=None,
         recv_xref=None,
         pay_xref=None,
@@ -2074,39 +2275,41 @@
             locale (str): install locale module with CoA; i.e l10n_it
             group (str): if supplied select specific group data; default is "base"
 
         Returns:
             None
         """
         self._logger.info(
-            "🎺🎺🎺 Starting test v2.0.6 (debug_level=%s)" % (self.debug_level)
+            "🎺🎺🎺 Starting test v2.0.7.1 (debug_level=%s)" % (self.debug_level)
         )
         self._logger.info(
             "🎺🎺 Testing module: %s (%s)"
             % (self.module.name, self.module.installed_version)
         )
         self.log_stack()
         if locale:  # pragma: no cover
             self.set_locale(locale)
         if lang:  # pragma: no cover
             self.install_language(lang)
         self._convert_test_data(group=group)
         for resource in self.get_resource_list(group=group):
             for xref in self.get_resource_data_list(resource, group=group):
                 self.resource_make(resource, xref, group=group)
-        self.env["account.journal"].search([("update_posted", "!=", True)]).write(
-            {"update_posted": True}
-        )
+        if self.odoo_major_version < 13:
+            self.env["account.journal"].search([("update_posted", "!=", True)]).write(
+                {"update_posted": True}
+            )
 
     ############################################
     #                                          #
     #     WIZARD/FORM ENVIRONMENT TEST API     #
     #                                          #
     ############################################
 
+    @api.model
     def resource_edit(self, resource, default={}, web_changes=[], actions=[], ctx={}):
         """Server-side web form editing.
         Ordinary Odoo test use the primitive create() and write() functions to manage
         test data. These methods create an update records, but they do not properly
         reflect the behaviour of user editing form with GUI interface.
 
         This function simulates the client-side form editing in the server-side.
@@ -2167,24 +2370,29 @@
                 resource,
                 self.dict_2_print(default),
                 self.dict_2_print(web_changes),
                 actions,
                 self.dict_2_print(ctx),
             )
         )
+        origin = self._set_origin(resource, ctx=ctx)
         for action in actions:
             result = self._exec_action(
-                resource, action, default=default, web_changes=web_changes, ctx=ctx
+                resource, action,
+                default=default, web_changes=web_changes, origin=origin, ctx=ctx
             )
             # Web changes executed, clear them, same for default
             web_changes = []
             default = {}
-            resource = result
+            if hasattr(result, "_name"):
+                # action returned recordset
+                resource = result
         return result
 
+    @api.model
     def field_download(self, record, field):
         """Execute the data download from a binary field.
 
         Args:
             record (obj): record object
             field (str): field name to download
 
@@ -2192,14 +2400,15 @@
             binary obj downloaded from field
         """
         self.log_stack()
         if field not in record:  # pragma: no cover
             raise ValueError("Field %s not found in %s" % (field, record._name))
         return base64.b64decode(getattr(record, field))
 
+    @api.model
     def resource_download(
         self,
         module=None,
         action_name=None,
         act_windows=None,
         records=None,
         default=None,
@@ -2258,20 +2467,22 @@
         res_model = self._get_model_from_act_windows(act_windows)
         if field not in self.env[res_model]:
             self.raise_error("Field %s not found in %s" % (field, res_model))
         return base64.b64decode(
             getattr(self.env[res_model].browse(act_windows["res_id"]), field)
         )
 
+    @api.model
     def is_action(self, act_windows):
         return isinstance(act_windows, dict) and act_windows.get("type") in (
             "ir.actions.act_window",
             "ir.actions.client",
         )
 
+    @api.model
     def wizard(
         self,
         module=None,
         action_name=None,
         act_windows=None,
         records=None,
         default=None,
@@ -2350,14 +2561,15 @@
         return self._wiz_execution(
             act_windows,
             button_name=button_name,
             web_changes=web_changes,
             button_ctx=button_ctx,
         )
 
+    @api.model
     def get_records_from_act_windows(self, act_windows):
         """Get records from a windows message.
 
         Args:
             act_windows (dict): Odoo windows action returned by a wizard
 
         Returns:
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/test_common.py` & `z0bug_odoo-2.0.7/z0bug_odoo/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     else:
         import odoo.tests.common as test_common
         from odoo.modules.module import get_module_resource  # noqa: F401
 else:
     print('No Odoo environment found!')
     sys.exit(0)
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 class Z0bugBaseCase(test_common.BaseCase):
     def pool_env(self, model):
         """Return model pool_environment"""
         if int(release.major_version.split('.')[0]) < 8:
             return self.registry(model)
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/run_pylint.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/run_pylint.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/git_run.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/git_run.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/get_test_dependencies.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/get_test_dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from test_server import get_test_dependencies
 except ImportError:
     from .getaddons import (get_dependencies, get_dependents, get_modules,
                             get_modules_info)
     from .test_server import get_test_dependencies
 
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 def get_module_list(paths):
     res = []
     for path in paths.split(','):
         r = get_modules(os.path.expanduser(path))
         for m in r:
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/test_pylint` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/test_pylint`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/getaddons.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/getaddons.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from git_run import GitRun
 except ImportError:
     try:
         from .git_run import GitRun
     except ImportError:
         from git_run import GitRun
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 
 
 def is_module(path):
     """return False if the path doesn't contain an odoo module, and the full
     path to the module manifest otherwise"""
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_test_dependencies` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_test_dependencies`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/odoo_connection.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/apis.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/apis.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/test_flake8` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/test_flake8`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 import sys
 
 from getaddons import get_modules
 
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 def get_build_dir():
     odoo_version = os.environ.get("VERSION")
     travis_base_dir = os.environ.get("TRAVIS_BUILD_DIR", "../..")
     tested_version = ''
     for ldir in ('./server/openerp', './openerp', './odoo'):
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_run_tests` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_run_tests`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 # import subprocess
 # import shutil
 import sys
 from distutils.spawn import find_executable
 from travis_helpers import success_msg, fail_msg
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 def main(test_list):
     """
     Loop through each test and run them, add display results at the end
 
     If the test has a .py extension, import as a list and call main function
@@ -74,15 +74,15 @@
     # makepot using the test database, which will be faster
     must_run_makepot = (
         (os.environ.get('MAKEPOT') == '1' or
          os.environ.get('TRANSIFEX') == '1') and
         not tests_enabled and
         is_oca_project and
         os.environ.get('TRAVIS_BRANCH')
-        in ('8.0', '9.0', '10.0', '11.0', '12.0', '13.0', '14.0') and
+        in ('8.0', '9.0', '10.0', '11.0', '12.0', '13.0', '14.0', '15.0', '16.0') and
         not is_pull_request and
         os.environ.get('GITHUB_USER') and
         os.environ.get('GITHUB_EMAIL') and
         os.environ.get('GITHUB_TOKEN')
     )
     must_run_tnlbot = (
         os.environ.get('ODOO_TNLBOT') == '1' and
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_tnlbot.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_tnlbot.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/clone_oca_dependencies` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/clone_oca_dependencies`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os.path as osp
 import subprocess
 import logging
 from travis_helpers import print_flush
 from z0lib import z0lib
 
 _logger = logging.getLogger()
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 
 def create_deps():
     return {
         'reqfilenames': [],
         'processed': set(),
     }
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/test_server.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                             get_modules, get_modules_info)
     from .travis_helpers import fail_msg, print_flush, success_msg
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 
 LDIR = ('server/openerp', 'odoo/odoo', 'openerp', 'odoo')
 
 
 def has_test_errors(fname, dbname, odoo_version, check_loaded=True):
     """
     Check a list of log lines for test errors.
@@ -174,14 +174,15 @@
             ldir = os.path.join(travis_base_dir, ldir)
             if os.path.isdir(ldir) and os.path.isfile('%s/release.py' % ldir):
                 lpath = ldir
                 break
         return lpath
 
     VERSIONS = (
+        '16.0',
         '15.0',
         '14.0',
         '13.0',
         '12.0',
         '11.0',
         '10.0',
         '9.0',
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_makepot` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_makepot`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/travis/travis_helpers.py` & `z0bug_odoo-2.0.7/z0bug_odoo/travis/travis_helpers.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo/__init__.py` & `z0bug_odoo-2.0.7/z0bug_odoo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 except ImportError:
     try:
         import openerp.release as release
         from . import test_common
     except ImportError:
         release = ''
 
-__version__ = '2.0.6'
+__version__ = '2.0.7'
 if eval(os.environ.get('TRAVIS_DEBUG_MODE', '0')) > 2:
     print('DEBUG: z0bug_odoo %s' % __version__)
     print('DEBUG: z0bug_odoo.sys.path=%s' % sys.path)
     if release:
         print('DEBUG: Odoo version detected: %s' % release.version)
     else:
         print('DEBUG: No Odoo environment found!')
```

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo.egg-info/SOURCES.txt` & `z0bug_odoo-2.0.7/z0bug_odoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.6/z0bug_odoo.egg-info/PKG-INFO` & `z0bug_odoo-2.0.7/z0bug_odoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: z0bug-odoo
-Version: 2.0.6
+Version: 2.0.7
 Summary: Odoo testing framework
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `z0bug_odoo-2.0.6/setup.py` & `z0bug_odoo-2.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='z0bug_odoo',
-    version='2.0.6',
+    version='2.0.7',
     description='Odoo testing framework',
     long_description="""
 Zeroincombenze(R) continuous testing framework for Odoo modules.
 
 Make avaiable test functions indipendent by Odoo version.
 """,
     classifiers=[
@@ -28,16 +28,15 @@
     project_urls={
         'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
         'Source': 'https://github.com/zeroincombenze/tools',
     },
     author='Antonio Maria Vigliotti',
     author_email='antoniomaria.vigliotti@gmail.com',
     license='Affero GPL',
-    # install_requires=['future', 'python-magic', 'clodoo', 'zerobug', 'gitPython'],
-    install_requires=['future', 'python-magic', 'zerobug', 'gitPython'],
+    install_requires=['future', 'python-magic', 'zerobug', 'gitPython', 'Click'],
     packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
     package_data={
         '': [
             'scripts/setup.info',
             'data/*',
             'travis/cfg/*',
             'travis/pylint_deprecated_modules/*',
```

### Comparing `z0bug_odoo-2.0.6/PKG-INFO` & `z0bug_odoo-2.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: z0bug_odoo
-Version: 2.0.6
+Version: 2.0.7
 Summary: Odoo testing framework
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `z0bug_odoo-2.0.6/README.rst` & `z0bug_odoo-2.0.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 ================
-z0bug_odoo 2.0.6
+z0bug_odoo 2.0.7
 ================
 
 
 
 |Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
@@ -1839,14 +1839,27 @@
     ./install_tools.sh -Ud
     source /opt/odoo/devel/activate_tools
 
 
 History
 -------
 
+2.0.7.1 (2023-04-26)
+~~~~~~~~~~~~~~~~~~~~
+
+* [FIX] TestEnv: multiple actione on the same records
+
+2.0.7 (2023-04-08)
+~~~~~~~~~~~~~~~~~~
+
+* [NEW] TestEnv: assertion counter
+* [IMP] TestEnv: is_xref recognizes dot name, i.e "zobug.external.10"
+* [IMP] TestEnv: the field <description> is not mode key (only acount.tax)
+* [IMP] TestEnv: 3th level xref may be a many2one field type
+
 2.0.6 (2023-02-20)
 ~~~~~~~~~~~~~~~~~~
 
 * [FIX] TestEnv: _get_xref_id recognize any group
 * [FIX] TestEnv: datetime field more precise (always with time)
 * [FIX] TestEnv: resource_make / resource_write fall in crash if repeated on headr/detail models
 * [NEW] TestEnv: 2many fields accepts more xref values
@@ -1935,15 +1948,15 @@
 
 
 
 |
 
 This module is part of tools project.
 
-Last Update / Ultimo aggiornamento: 2023-02-23
+Last Update / Ultimo aggiornamento: 2023-05-01
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
 .. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
     :target: https://travis-ci.com/zeroincombenze/tools
     :alt: github.com
```

