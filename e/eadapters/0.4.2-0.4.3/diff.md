# Comparing `tmp/eadapters-0.4.2.tar.gz` & `tmp/eadapters-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eadapters-0.4.2.tar", last modified: Wed May  3 19:25:26 2023, max compression
+gzip compressed data, was "dist/eadapters-0.4.3.tar", last modified: Tue May  9 19:36:55 2023, max compression
```

## Comparing `eadapters-0.4.2.tar` & `eadapters-0.4.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-03 19:25:26.000000 eadapters-0.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2800 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1032 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 19:25:21.000000 eadapters-0.4.2/src/eadapters.egg-info/not-zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters/
--rw-r--r--   0 root         (0) root         (0)    10178 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/base.py
--rw-r--r--   0 root         (0) root         (0)    19541 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/budy_a.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters/models/
--rw-r--r--   0 root         (0) root         (0)     1525 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/address.py
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 19:25:26.000000 eadapters-0.4.2/src/eadapters/models/budy/
--rw-r--r--   0 root         (0) root         (0)      548 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_address.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_subscription.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_brand.py
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_season.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_voucher.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_category.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_city.py
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_shipping_option.py
--rw-r--r--   0 root         (0) root         (0)     1392 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_product.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_wishlist.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_payment_method.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_bag_line.py
--rw-r--r--   0 root         (0) root         (0)      621 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_store.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_payment.py
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_collection.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_order_line.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_return.py
--rw-r--r--   0 root         (0) root         (0)     4144 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_common.py
--rw-r--r--   0 root         (0) root         (0)     4335 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_account.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_color.py
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_merchant.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_country.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_section.py
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_referral.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_state.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_bag.py
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_card_payment_method.py
--rw-r--r--   0 root         (0) root         (0)      187 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_wishlist_line.py
--rw-r--r--   0 root         (0) root         (0)     3791 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_order.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_group.py
--rw-r--r--   0 root         (0) root         (0)      161 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/budy/bd_credit.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/base.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/graphic.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/card_payment_method.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/wishlist_line.py
--rw-r--r--   0 root         (0) root         (0)      109 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/season.py
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/voucher.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/bag_line.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/group.py
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/store.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/order.py
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/country.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/category.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/currency.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/merchant.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/collection.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/credit_card.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/shipping_option.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/credit.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/account.py
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/payment.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/_return.py
--rw-r--r--   0 root         (0) root         (0)     2877 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/product.py
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/state.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/city.py
--rw-r--r--   0 root         (0) root         (0)      333 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/payment_method.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/bag.py
--rw-r--r--   0 root         (0) root         (0)      343 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/wishlist.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/section.py
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/brand.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/order_line.py
--rw-r--r--   0 root         (0) root         (0)      108 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/models/referral.py
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2754 2023-05-03 19:25:18.000000 eadapters-0.4.2/src/eadapters/factory.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-05-03 19:25:18.000000 eadapters-0.4.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-03 19:25:18.000000 eadapters-0.4.2/README.md
--rw-r--r--   0 root         (0) root         (0)     1032 2023-05-03 19:25:26.000000 eadapters-0.4.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:36:55.000000 eadapters-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-09 19:36:55.000000 eadapters-0.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 19:36:50.000000 eadapters-0.4.3/src/eadapters.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters/
+-rw-r--r--   0 root         (0) root         (0)    10178 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/base.py
+-rw-r--r--   0 root         (0) root         (0)    19541 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/budy_a.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters/models/
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/address.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 19:36:55.000000 eadapters-0.4.3/src/eadapters/models/budy/
+-rw-r--r--   0 root         (0) root         (0)      548 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_address.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_subscription.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_brand.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_season.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_voucher.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_category.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_city.py
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_shipping_option.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_product.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_wishlist.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_bag_line.py
+-rw-r--r--   0 root         (0) root         (0)      621 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_store.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_payment.py
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_collection.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_order_line.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_return.py
+-rw-r--r--   0 root         (0) root         (0)     4144 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_common.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_account.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_color.py
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_merchant.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_country.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_section.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_referral.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_state.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_bag.py
+-rw-r--r--   0 root         (0) root         (0)      154 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_card_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      187 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_wishlist_line.py
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_order.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_group.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/budy/bd_credit.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/graphic.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/card_payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/wishlist_line.py
+-rw-r--r--   0 root         (0) root         (0)      109 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/season.py
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/voucher.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/bag_line.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/group.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/store.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/order.py
+-rw-r--r--   0 root         (0) root         (0)      439 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/country.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/category.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/merchant.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/collection.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/credit_card.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/shipping_option.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/credit.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/account.py
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/payment.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/_return.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/product.py
+-rw-r--r--   0 root         (0) root         (0)      105 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/state.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/city.py
+-rw-r--r--   0 root         (0) root         (0)      333 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/payment_method.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/bag.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/wishlist.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/section.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/brand.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/order_line.py
+-rw-r--r--   0 root         (0) root         (0)      108 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/models/referral.py
+-rw-r--r--   0 root         (0) root         (0)      229 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2754 2023-05-09 19:36:47.000000 eadapters-0.4.3/src/eadapters/factory.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-05-09 19:36:47.000000 eadapters-0.4.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-09 19:36:47.000000 eadapters-0.4.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-05-09 19:36:55.000000 eadapters-0.4.3/PKG-INFO
```

### Comparing `eadapters-0.4.2/src/eadapters.egg-info/SOURCES.txt` & `eadapters-0.4.3/src/eadapters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters.egg-info/PKG-INFO` & `eadapters-0.4.3/src/eadapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: eadapters
-Version: 0.4.2
+Version: 0.4.3
 Summary: E-Commerce Adapters
 Home-page: http://eadapters.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: e-commerce adapters logic
```

### Comparing `eadapters-0.4.2/src/eadapters/base.py` & `eadapters-0.4.3/src/eadapters/base.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/budy_a.py` & `eadapters-0.4.3/src/eadapters/budy_a.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/address.py` & `eadapters-0.4.3/src/eadapters/models/address.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_address.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_address.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_product.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_product.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_bag_line.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_bag_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_store.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_store.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_order_line.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_order_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_common.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_common.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_account.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_account.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_country.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_country.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/__init__.py` & `eadapters-0.4.3/src/eadapters/models/budy/__init__.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_bag.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_bag.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/budy/bd_order.py` & `eadapters-0.4.3/src/eadapters/models/budy/bd_order.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import appier
 
+from . import bd_store
 from . import bd_common
 from . import bd_address
 from . import bd_voucher
 from . import bd_order_line
 
 from .. import order
 
@@ -17,19 +18,21 @@
     @classmethod
     def wrap(cls, models, build = True, handler = None, **kwargs):
         def handler(model):
             lines = model.get("lines", [])
             vouchers = model.get("vouchers", [])
             shipping_address = model.get("shipping_address", {})
             billing_address = model.get("billing_address", {})
+            store = model.get("store", {})
             model.update(
                 lines = bd_order_line.BDOrderLine.wrap(lines),
                 vouchers = bd_voucher.BDVoucher.wrap(vouchers),
                 shipping_address = bd_address.BDAddress.wrap(shipping_address) if shipping_address else None,
-                billing_address = bd_address.BDAddress.wrap(billing_address) if billing_address else None
+                billing_address = bd_address.BDAddress.wrap(billing_address) if billing_address else None,
+                store = bd_store.BDStore.wrap(store) if store else None
             )
 
         return super(BDOrder, cls).wrap(
             models,
             build = build,
             handler = handler,
             **kwargs
```

### Comparing `eadapters-0.4.2/src/eadapters/models/base.py` & `eadapters-0.4.3/src/eadapters/models/base.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/graphic.py` & `eadapters-0.4.3/src/eadapters/models/graphic.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/bag_line.py` & `eadapters-0.4.3/src/eadapters/models/bag_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/order.py` & `eadapters-0.4.3/src/eadapters/models/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,21 @@
     vouchers = appier.field(
         type = appier.references(
             "EVoucher",
             name = "id"
         )
     )
 
+    store = appier.field(
+        type = appier.reference(
+            "EStore",
+            name = "id"
+        )
+    )
+
     @classmethod
     def _build(cls, model, map):
         super(EOrder, cls)._build(model, map)
 
         date = model["date"]
         if date: date = datetime.datetime.utcfromtimestamp(date)
         model["date_s"] = date.strftime("%Y-%m-%d") if date else None
```

### Comparing `eadapters-0.4.2/src/eadapters/models/credit_card.py` & `eadapters-0.4.3/src/eadapters/models/credit_card.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/account.py` & `eadapters-0.4.3/src/eadapters/models/account.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/__init__.py` & `eadapters-0.4.3/src/eadapters/models/__init__.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/product.py` & `eadapters-0.4.3/src/eadapters/models/product.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/models/order_line.py` & `eadapters-0.4.3/src/eadapters/models/order_line.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/src/eadapters/factory.py` & `eadapters-0.4.3/src/eadapters/factory.py`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/setup.py` & `eadapters-0.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
     name = "eadapters",
-    version = "0.4.2",
+    version = "0.4.3",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "E-Commerce Adapters",
     license = "Apache License, Version 2.0",
     keywords = "e-commerce adapters logic",
     url = "http://eadapters.hive.pt",
     zip_safe = False,
```

### Comparing `eadapters-0.4.2/README.md` & `eadapters-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `eadapters-0.4.2/PKG-INFO` & `eadapters-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: eadapters
-Version: 0.4.2
+Version: 0.4.3
 Summary: E-Commerce Adapters
 Home-page: http://eadapters.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: e-commerce adapters logic
```

