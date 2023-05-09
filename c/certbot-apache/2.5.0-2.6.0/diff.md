# Comparing `tmp/certbot-apache-2.5.0.tar.gz` & `tmp/certbot-apache-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-apache-2.5.0.tar", last modified: Tue Apr  4 15:07:04 2023, max compression
+gzip compressed data, was "certbot-apache-2.6.0.tar", last modified: Tue May  9 19:44:42 2023, max compression
```

## Comparing `certbot-apache-2.5.0.tar` & `certbot-apache-2.6.0.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/
--rw-r--r--   0 bmw        (501) staff       (20)    10786 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/LICENSE.txt
--rw-r--r--   0 bmw        (501) staff       (20)      306 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/MANIFEST.in
--rw-r--r--   0 bmw        (501) staff       (20)     1171 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)       26 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/README.rst
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/
--rw-r--r--   0 bmw        (501) staff       (20)       29 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/__init__.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/
--rw-r--r--   0 bmw        (501) staff       (20)       29 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)     7369 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/apache_util.py
--rw-r--r--   0 bmw        (501) staff       (20)     8072 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/apacheparser.py
--rw-r--r--   0 bmw        (501) staff       (20)     5893 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/assertions.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/augeas_lens/
--rw-r--r--   0 bmw        (501) staff       (20)     7528 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/augeas_lens/httpd.aug
--rw-r--r--   0 bmw        (501) staff       (20)    21112 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/augeasparser.py
--rw-r--r--   0 bmw        (501) staff       (20)   112791 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/configurator.py
--rw-r--r--   0 bmw        (501) staff       (20)     3442 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/constants.py
--rw-r--r--   0 bmw        (501) staff       (20)     4576 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/display_ops.py
--rw-r--r--   0 bmw        (501) staff       (20)    14986 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/dualparser.py
--rw-r--r--   0 bmw        (501) staff       (20)     2870 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/entrypoint.py
--rw-r--r--   0 bmw        (501) staff       (20)     8415 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/http_01.py
--rw-r--r--   0 bmw        (501) staff       (20)    22825 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/interfaces.py
--rw-r--r--   0 bmw        (501) staff       (20)     9299 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/obj.py
--rw-r--r--   0 bmw        (501) staff       (20)      676 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_arch.py
--rw-r--r--   0 bmw        (501) staff       (20)     4700 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_centos.py
--rw-r--r--   0 bmw        (501) staff       (20)      604 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_darwin.py
--rw-r--r--   0 bmw        (501) staff       (20)     5285 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_debian.py
--rw-r--r--   0 bmw        (501) staff       (20)     3460 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_fedora.py
--rw-r--r--   0 bmw        (501) staff       (20)     2427 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_gentoo.py
--rw-r--r--   0 bmw        (501) staff       (20)      670 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_suse.py
--rw-r--r--   0 bmw        (501) staff       (20)      681 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/override_void.py
--rw-r--r--   0 bmw        (501) staff       (20)    36804 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/parser.py
--rw-r--r--   0 bmw        (501) staff       (20)     5823 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/parsernode_util.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/
--rw-r--r--   0 bmw        (501) staff       (20)       27 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/__init__.py
--rw-r--r--   0 bmw        (501) staff       (20)    12943 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/augeasnode_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     8892 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/autohsts_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    10972 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/centos_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     4408 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/complex_parsing_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     2816 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/configurator_reverter_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    77783 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/configurator_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     9283 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/debian_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     3748 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/display_ops_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    24089 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/dualnode_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     1718 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/entrypoint_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     8161 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/fedora_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     5590 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/gentoo_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     9189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/http_01_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     5165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/obj_test.py
--rw-r--r--   0 bmw        (501) staff       (20)    16692 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/parser_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     1625 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/parsernode_configurator_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     3554 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/parsernode_test.py
--rw-r--r--   0 bmw        (501) staff       (20)     3275 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/parsernode_util_test.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/
--rw-r--r--   0 bmw        (501) staff       (20)    11753 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf
--rw-r--r--   0 bmw        (501) staff       (20)    13077 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/
--rw-r--r--   0 bmw        (501) staff       (20)      366 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/README
--rw-r--r--   0 bmw        (501) staff       (20)     2926 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf
--rw-r--r--   0 bmw        (501) staff       (20)      213 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/centos.example.com.conf
--rw-r--r--   0 bmw        (501) staff       (20)     9295 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1252 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf
--rw-r--r--   0 bmw        (501) staff       (20)      824 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/
--rw-r--r--   0 bmw        (501) staff       (20)     3739 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf
--rw-r--r--   0 bmw        (501) staff       (20)      139 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-dav.conf
--rw-r--r--   0 bmw        (501) staff       (20)       41 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-lua.conf
--rw-r--r--   0 bmw        (501) staff       (20)      742 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf
--rw-r--r--   0 bmw        (501) staff       (20)      957 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf
--rw-r--r--   0 bmw        (501) staff       (20)       41 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)       88 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-systemd.conf
--rw-r--r--   0 bmw        (501) staff       (20)      451 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/01-cgi.conf
--rw-r--r--   0 bmw        (501) staff       (20)       51 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sites
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/
--rw-r--r--   0 bmw        (501) staff       (20)      890 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/
--rw-r--r--   0 bmw        (501) staff       (20)     1078 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      267 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/dummy.conf
--rw-r--r--   0 bmw        (501) staff       (20)       26 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_fnmatch.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1234 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/
--rw-r--r--   0 bmw        (501) staff       (20)     6533 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/
--rw-r--r--   0 bmw        (501) staff       (20)       46 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/bad_conf_file.conf
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/other-vhosts-access-log.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf
--rw-r--r--   0 bmw        (501) staff       (20)      455 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/serve-cgi-bin.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf
--rw-r--r--   0 bmw        (501) staff       (20)      455 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
--rw-r--r--   0 bmw        (501) staff       (20)      982 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/
--rw-r--r--   0 bmw        (501) staff       (20)      165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/authz_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)       93 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav.load
--rw-r--r--   0 bmw        (501) staff       (20)     2372 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf
--rw-r--r--   0 bmw        (501) staff       (20)      203 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)       66 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/rewrite.load
--rw-r--r--   0 bmw        (501) staff       (20)     3405 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)       97 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.load
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/authz_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)       93 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav.load
--rw-r--r--   0 bmw        (501) staff       (20)     2372 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf
--rw-r--r--   0 bmw        (501) staff       (20)      203 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)      320 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/ports.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/
--rw-r--r--   0 bmw        (501) staff       (20)      282 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/another_wildcard.conf
--rw-r--r--   0 bmw        (501) staff       (20)      266 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/old-and-default.conf
--rw-r--r--   0 bmw        (501) staff       (20)      322 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/wildcard.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      282 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/another_wildcard.conf
--rw-r--r--   0 bmw        (501) staff       (20)      266 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/old-and-default.conf
--rw-r--r--   0 bmw        (501) staff       (20)      322 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/wildcard.conf
--rw-r--r--   0 bmw        (501) staff       (20)      153 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/sites
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/
--rw-r--r--   0 bmw        (501) staff       (20)     6536 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/other-vhosts-access-log.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1014 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf
--rw-r--r--   0 bmw        (501) staff       (20)      455 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/serve-cgi-bin.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/other-vhosts-access-log.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1014 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf
--rw-r--r--   0 bmw        (501) staff       (20)      455 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/serve-cgi-bin.conf
--rw-r--r--   0 bmw        (501) staff       (20)      981 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/
--rw-r--r--   0 bmw        (501) staff       (20)     3405 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)       97 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.load
--rw-r--r--   0 bmw        (501) staff       (20)      397 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/ports.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/
--rw-r--r--   0 bmw        (501) staff       (20)      295 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/000-default.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1140 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      295 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/000-default.conf
--rw-r--r--   0 bmw        (501) staff       (20)       47 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/sites
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/
--rw-r--r--   0 bmw        (501) staff       (20)     6533 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf
--rw-r--r--   0 bmw        (501) staff       (20)      982 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars
--rw-r--r--   0 bmw        (501) staff       (20)      320 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/ports.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/
--rw-r--r--   0 bmw        (501) staff       (20)      474 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/default.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1280 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      474 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/default.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1280 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/
--rw-r--r--   0 bmw        (501) staff       (20)     6749 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/
--rw-r--r--   0 bmw        (501) staff       (20)       46 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/bad_conf_file.conf
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/other-vhosts-access-log.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf
--rw-r--r--   0 bmw        (501) staff       (20)      455 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/serve-cgi-bin.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf
--rw-r--r--   0 bmw        (501) staff       (20)      455 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
--rw-r--r--   0 bmw        (501) staff       (20)      982 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/
--rw-r--r--   0 bmw        (501) staff       (20)      165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/authz_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)       93 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav.load
--rw-r--r--   0 bmw        (501) staff       (20)     2372 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf
--rw-r--r--   0 bmw        (501) staff       (20)      203 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)       66 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/rewrite.load
--rw-r--r--   0 bmw        (501) staff       (20)     3405 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)       97 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.load
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      165 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/authz_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)       93 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav.load
--rw-r--r--   0 bmw        (501) staff       (20)     2372 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf
--rw-r--r--   0 bmw        (501) staff       (20)      203 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.load
--rw-r--r--   0 bmw        (501) staff       (20)      320 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/ports.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/
--rw-r--r--   0 bmw        (501) staff       (20)      266 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/000-default.conf
--rw-r--r--   0 bmw        (501) staff       (20)      941 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1112 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1201 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)      228 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttp.conf
--rw-r--r--   0 bmw        (501) staff       (20)      378 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttps.conf
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/empty.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1157 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf
--rw-r--r--   0 bmw        (501) staff       (20)      377 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/mod_macro-example.conf
--rw-r--r--   0 bmw        (501) staff       (20)       90 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/no-directives.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1568 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)      289 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/wildcard.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/
--rw-r--r--   0 bmw        (501) staff       (20)      266 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/000-default.conf
--rw-r--r--   0 bmw        (501) staff       (20)      941 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1112 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1201 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)      228 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttp.conf
--rw-r--r--   0 bmw        (501) staff       (20)      378 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttps.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1157 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf
--rw-r--r--   0 bmw        (501) staff       (20)      377 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/mod_macro-example.conf
--rw-r--r--   0 bmw        (501) staff       (20)      222 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/non-symlink.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1568 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)      289 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/wildcard.conf
--rw-r--r--   0 bmw        (501) staff       (20)      153 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/sites
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/
--rw-r--r--   0 bmw        (501) staff       (20)     6303 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf
--rw-r--r--   0 bmw        (501) staff       (20)    13077 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/
--rw-r--r--   0 bmw        (501) staff       (20)     5308 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf
--rw-r--r--   0 bmw        (501) staff       (20)     2520 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf
--rw-r--r--   0 bmw        (501) staff       (20)     5041 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf
--rw-r--r--   0 bmw        (501) staff       (20)     2883 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf
--rw-r--r--   0 bmw        (501) staff       (20)      225 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_info.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1518 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1707 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf
--rw-r--r--   0 bmw        (501) staff       (20)      458 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_status.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1015 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf
--rw-r--r--   0 bmw        (501) staff       (20)     2959 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf
--rw-r--r--   0 bmw        (501) staff       (20)      206 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/10_mod_mem_cache.conf
--rw-r--r--   0 bmw        (501) staff       (20)     2652 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf
--rw-r--r--   0 bmw        (501) staff       (20)      189 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/41_mod_http2.conf
--rw-r--r--   0 bmw        (501) staff       (20)      758 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf
--rw-r--r--   0 bmw        (501) staff       (20)      406 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/46_mod_ldap.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/
--rw-r--r--   0 bmw        (501) staff       (20)     8596 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf
--rw-r--r--   0 bmw        (501) staff       (20)     1462 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf
--rw-r--r--   0 bmw        (501) staff       (20)     2804 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include
--rw-r--r--   0 bmw        (501) staff       (20)      213 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/gentoo.example.com.conf
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/
--rw-r--r--   0 bmw        (501) staff       (20)     3136 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2
--rw-r--r--   0 bmw        (501) staff       (20)      141 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/sites
--rw-r--r--   0 bmw        (501) staff       (20)    10802 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tests/util.py
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache/_internal/tls_configs/
--rw-r--r--   0 bmw        (501) staff       (20)     1005 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf
--rw-r--r--   0 bmw        (501) staff       (20)      977 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf
--rw-r--r--   0 bmw        (501) staff       (20)        0 2023-04-04 15:06:41.000000 certbot-apache-2.5.0/certbot_apache/py.typed
-drwxr-xr-x   0 bmw        (501) staff       (20)        0 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/
--rw-r--r--   0 bmw        (501) staff       (20)     1171 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/PKG-INFO
--rw-r--r--   0 bmw        (501) staff       (20)    16809 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/SOURCES.txt
--rw-r--r--   0 bmw        (501) staff       (20)        1 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/dependency_links.txt
--rw-r--r--   0 bmw        (501) staff       (20)       74 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/entry_points.txt
--rw-r--r--   0 bmw        (501) staff       (20)      102 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/requires.txt
--rw-r--r--   0 bmw        (501) staff       (20)       15 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/certbot_apache.egg-info/top_level.txt
--rw-r--r--   0 bmw        (501) staff       (20)       38 2023-04-04 15:07:04.000000 certbot-apache-2.5.0/setup.cfg
--rw-r--r--   0 bmw        (501) staff       (20)     1930 2023-04-04 15:06:42.000000 certbot-apache-2.5.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      306 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/MANIFEST.in
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1171 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       26 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.695332 certbot-apache-2.6.0/certbot_apache/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       29 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.699331 certbot-apache-2.6.0/certbot_apache/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       29 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7369 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/apache_util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8072 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/apacheparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5893 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/assertions.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.699331 certbot-apache-2.6.0/certbot_apache/_internal/augeas_lens/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7528 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/augeas_lens/httpd.aug
+-rw-rw-r--   0 erica     (1001) erica     (1001)    21112 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/augeasparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)   112791 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/configurator.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3442 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/constants.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4576 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/display_ops.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14986 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/dualparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2870 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/entrypoint.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8415 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/http_01.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22825 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/interfaces.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9299 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/obj.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      676 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_arch.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4700 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_centos.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      604 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_darwin.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5285 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_debian.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3460 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_fedora.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2427 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_gentoo.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      670 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_suse.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      681 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/override_void.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    36804 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/parser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5823 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/parsernode_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.699331 certbot-apache-2.6.0/certbot_apache/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       27 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12943 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/augeasnode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8939 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/autohsts_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10972 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/centos_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4408 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/complex_parsing_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2816 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/configurator_reverter_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    77783 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/configurator_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9283 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/debian_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3748 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/display_ops_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    24089 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/dualnode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1718 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/entrypoint_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8161 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/fedora_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5590 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/gentoo_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/http_01_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/obj_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    16692 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/parser_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1625 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/parsernode_configurator_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3554 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/parsernode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3275 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/parsernode_util_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.695332 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.691333 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.699331 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.691333 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.699331 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11753 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13077 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.699331 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      366 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/README
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2926 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      213 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/centos.example.com.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9295 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1252 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      824 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3739 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      139 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-dav.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       41 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-lua.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      742 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      957 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       41 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       88 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-systemd.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      451 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/01-cgi.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       51 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      890 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1078 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      267 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/dummy.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       26 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_fnmatch.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1234 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.695332 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6533 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/bad_conf_file.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/serve-cgi-bin.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      982 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       66 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/rewrite.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3405 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.load
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)      320 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      282 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/another_wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/old-and-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      322 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/wildcard.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      282 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/another_wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/old-and-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      322 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      153 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6536 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1014 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/serve-cgi-bin.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1014 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/serve-cgi-bin.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      981 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3405 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)      397 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      295 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1140 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.703330 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      295 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       47 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.695332 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6533 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      982 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars
+-rw-rw-r--   0 erica     (1001) erica     (1001)      320 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      474 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1280 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      474 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1280 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6749 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/bad_conf_file.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/serve-cgi-bin.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      982 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       66 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/rewrite.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3405 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.load
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)      320 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.707329 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      941 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1112 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1201 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      228 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttp.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      378 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttps.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/empty.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1157 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      377 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/mod_macro-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       90 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/no-directives.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1568 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      289 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/wildcard.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      941 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1112 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1201 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      228 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttp.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      378 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttps.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1157 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      377 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/mod_macro-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      222 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/non-symlink.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1568 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      289 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      153 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.695332 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6303 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13077 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5308 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2520 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5041 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2883 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      225 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_info.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1518 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1707 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      458 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_status.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1015 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2959 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      206 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/10_mod_mem_cache.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2652 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/41_mod_http2.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      758 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      406 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/46_mod_ldap.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8596 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1462 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2804 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include
+-rw-rw-r--   0 erica     (1001) erica     (1001)      213 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/gentoo.example.com.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3136 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2
+-rw-rw-r--   0 erica     (1001) erica     (1001)      141 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/sites
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10802 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tests/util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/certbot_apache/_internal/tls_configs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1005 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      977 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:36.000000 certbot-apache-2.6.0/certbot_apache/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2023-05-09 19:44:42.695332 certbot-apache-2.6.0/certbot_apache.egg-info/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1171 2023-05-09 19:44:42.000000 certbot-apache-2.6.0/certbot_apache.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)    16809 2023-05-09 19:44:42.000000 certbot-apache-2.6.0/certbot_apache.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2023-05-09 19:44:42.000000 certbot-apache-2.6.0/certbot_apache.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       74 2023-05-09 19:44:42.000000 certbot-apache-2.6.0/certbot_apache.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      102 2023-05-09 19:44:42.000000 certbot-apache-2.6.0/certbot_apache.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       15 2023-05-09 19:44:42.000000 certbot-apache-2.6.0/certbot_apache.egg-info/top_level.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2023-05-09 19:44:42.711327 certbot-apache-2.6.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1930 2023-05-09 19:44:37.000000 certbot-apache-2.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `certbot-apache-2.5.0/LICENSE.txt` & `certbot-apache-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/PKG-INFO` & `certbot-apache-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-apache
-Version: 2.5.0
+Version: 2.6.0
 Summary: Apache plugin for Certbot
 Home-page: https://github.com/letsencrypt/letsencrypt
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/apache_util.py` & `certbot-apache-2.6.0/certbot_apache/_internal/apache_util.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/apacheparser.py` & `certbot-apache-2.6.0/certbot_apache/_internal/apacheparser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/assertions.py` & `certbot-apache-2.6.0/certbot_apache/_internal/assertions.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/augeas_lens/httpd.aug` & `certbot-apache-2.6.0/certbot_apache/_internal/augeas_lens/httpd.aug`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/augeasparser.py` & `certbot-apache-2.6.0/certbot_apache/_internal/augeasparser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/configurator.py` & `certbot-apache-2.6.0/certbot_apache/_internal/configurator.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/constants.py` & `certbot-apache-2.6.0/certbot_apache/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/display_ops.py` & `certbot-apache-2.6.0/certbot_apache/_internal/display_ops.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/dualparser.py` & `certbot-apache-2.6.0/certbot_apache/_internal/dualparser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/entrypoint.py` & `certbot-apache-2.6.0/certbot_apache/_internal/entrypoint.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/http_01.py` & `certbot-apache-2.6.0/certbot_apache/_internal/http_01.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/interfaces.py` & `certbot-apache-2.6.0/certbot_apache/_internal/interfaces.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/obj.py` & `certbot-apache-2.6.0/certbot_apache/_internal/obj.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_arch.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_arch.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_centos.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_centos.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_darwin.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_darwin.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_debian.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_debian.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_fedora.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_fedora.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_gentoo.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_gentoo.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_suse.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_suse.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/override_void.py` & `certbot-apache-2.6.0/certbot_apache/_internal/override_void.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/parser.py` & `certbot-apache-2.6.0/certbot_apache/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/parsernode_util.py` & `certbot-apache-2.6.0/certbot_apache/_internal/parsernode_util.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/augeasnode_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/augeasnode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/autohsts_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/autohsts_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,19 +124,19 @@
                           maxage.format(constants.AUTOHSTS_STEPS[-1])
         # Make permanent
         self.config.deploy_autohsts(mock_lineage)
         assert self.get_autohsts_value(self.vh_truth[7].path) == \
                           max_val
 
     def test_autohsts_update_noop(self):
-        with mock.patch("time.time") as mock_time:
+        with mock.patch("certbot_apache._internal.configurator.time") as mock_time_module:
             # Time mock is used to make sure that the execution does not
             # continue when no autohsts entries exist in pluginstorage
             self.config.update_autohsts(mock.MagicMock())
-            assert mock_time.called is False
+            assert not mock_time_module.time.called
 
     def test_autohsts_make_permanent_noop(self):
         self.config.storage.put = mock.MagicMock()
         self.config.deploy_autohsts(mock.MagicMock())
         # Make sure that the execution does not continue when no entries in store
         assert self.config.storage.put.called is False
```

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/centos_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/centos_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/complex_parsing_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/complex_parsing_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/configurator_reverter_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/configurator_reverter_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/configurator_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/debian_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/debian_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/display_ops_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/display_ops_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/dualnode_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/dualnode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/entrypoint_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/entrypoint_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/fedora_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/fedora_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/gentoo_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/gentoo_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/http_01_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/http_01_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/obj_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/obj_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/parser_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/parser_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/parsernode_configurator_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/parsernode_configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/parsernode_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/parsernode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/parsernode_util_test.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/parsernode_util_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tests/util.py` & `certbot-apache-2.6.0/certbot_apache/_internal/tests/util.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf` & `certbot-apache-2.6.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/certbot_apache.egg-info/PKG-INFO` & `certbot-apache-2.6.0/certbot_apache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-apache
-Version: 2.5.0
+Version: 2.6.0
 Summary: Apache plugin for Certbot
 Home-page: https://github.com/letsencrypt/letsencrypt
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-apache-2.5.0/certbot_apache.egg-info/SOURCES.txt` & `certbot-apache-2.6.0/certbot_apache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.5.0/setup.py` & `certbot-apache-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.5.0'
+version = '2.6.0'
 
 install_requires = [
     # We specify the minimum acme and certbot version as the current plugin
     # version for simplicity. See
     # https://github.com/certbot/certbot/issues/8761 for more info.
     f'acme>={version}',
     f'certbot>={version}',
```

