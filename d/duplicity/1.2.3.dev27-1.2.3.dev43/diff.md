# Comparing `tmp/duplicity-1.2.3.dev27.tar.gz` & `tmp/duplicity-1.2.3.dev43.tar.gz`

## Comparing `duplicity-1.2.3.dev27.tar` & `duplicity-1.2.3.dev43.tar`

### file list

```diff
@@ -1,313 +1,314 @@
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/
--rw-r--r--   0 ken       (1000) ken       (1000)    92665 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/CHANGELOG.md
--rw-r--r--   0 ken       (1000) ken       (1000)      101 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/setup.cfg
--rw-r--r--   0 ken       (1000) ken       (1000)      651 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/pylintrc
--rw-r--r--   0 ken       (1000) ken       (1000)     1390 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/CONTRIBUTING.md
--rw-r--r--   0 ken       (1000) ken       (1000)     2814 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/tox.ini
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/bin/
--rwxr-xr-x   0 ken       (1000) ken       (1000)     5215 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/bin/duplicity
--rw-r--r--   0 ken       (1000) ken       (1000)     3108 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/bin/rdiffdir.1
--rw-r--r--   0 ken       (1000) ken       (1000)    97335 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/bin/duplicity.1
--rwxr-xr-x   0 ken       (1000) ken       (1000)     9127 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/bin/rdiffdir
--rw-r--r--   0 ken       (1000) ken       (1000)     1053 2023-03-08 15:58:27.000000 duplicity-1.2.3.dev27/requirements.txt
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/snap/
--rw-r--r--   0 ken       (1000) ken       (1000)     5723 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/snap/snapcraft.yaml
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/snap/local/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      186 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/snap/local/debug.sh
--rwxr-xr-x   0 ken       (1000) ken       (1000)      110 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/snap/local/launcher.sh
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/testing/
--rw-r--r--   0 ken       (1000) ken       (1000)   319661 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/testfiles.tar.gz
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/testing/unit/
--rw-r--r--   0 ken       (1000) ken       (1000)     8373 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_gpginterface.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11911 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_patchdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6777 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_dup_time.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12146 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_lazy.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5751 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_statistics.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14365 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_globmatch.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5848 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_manifest.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1027 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12014 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_collections.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2566 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_dup_temp.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6028 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_file_naming.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1287 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_tarfile.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13493 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_diffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2596 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_tempdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10376 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_backend_instance.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3877 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/testing/unit/test_path.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1546 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_util.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8686 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_gpg.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12081 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    67031 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/unit/test_selection.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/testing/overrides/
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/testing/overrides/bin/
--rwxr-xr-x   0 ken       (1000) ken       (1000)      226 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/bin/ncftpget
--rwxr-xr-x   0 ken       (1000) ken       (1000)      593 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/bin/lftp
--rwxr-xr-x   0 ken       (1000) ken       (1000)      226 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/bin/ncftpput
--rwxr-xr-x   0 ken       (1000) ken       (1000)      494 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/bin/hsi
--rwxr-xr-x   0 ken       (1000) ken       (1000)      487 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/bin/tahoe
--rwxr-xr-x   0 ken       (1000) ken       (1000)      628 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/bin/ncftpls
--rw-r--r--   0 ken       (1000) ken       (1000)      318 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/overrides/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5228 2023-02-21 16:03:23.000000 duplicity-1.2.3.dev27/testing/__init__.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)      878 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/run-tests
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/testing/functional/
--rw-r--r--   0 ken       (1000) ken       (1000)     2641 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_log.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9764 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/testing/functional/test_final.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1724 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_badupload.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3513 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_cleanup.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9513 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3514 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_replicate.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9126 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_verify.py
--rw-r--r--   0 ken       (1000) ken       (1000)    20273 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_restart.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3936 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/functional/test_rdiffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)   111376 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/testing/functional/test_selection.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)     3614 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/fix_unadorned_strings.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1083 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/conftest.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6236 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/test_code.py
--rwxr-xr-x   0 ken       (1000) ken       (1000)     2979 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/find_unadorned_strings.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/testing/gnupg/
--rw-r--r--   0 ken       (1000) ken       (1000)      145 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/gnupg/gpg-agent.conf
--rw-r--r--   0 ken       (1000) ken       (1000)     3567 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/gnupg/pubring.gpg
--rw-r--r--   0 ken       (1000) ken       (1000)     7549 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/gnupg/secring.gpg
--rw-r--r--   0 ken       (1000) ken       (1000)      425 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/gnupg/gpg.conf
--rw-r--r--   0 ken       (1000) ken       (1000)      255 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/gnupg/README
--rw-r--r--   0 ken       (1000) ken       (1000)     1440 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/testing/gnupg/trustdb.gpg
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity/
--rw-r--r--   0 ken       (1000) ken       (1000)    11648 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/dup_time.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity/backends/
--rw-r--r--   0 ken       (1000) ken       (1000)     3033 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/localbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16858 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/duplicity/backends/onedrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    17385 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/adbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8839 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/megav2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10572 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/swiftbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4474 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/rclonebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9459 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/duplicity/backends/b2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2645 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/tahoebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16496 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/gdrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13658 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/ssh_pexpect_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9393 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/gdocsbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8216 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/giobackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6895 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/megabackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13014 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/pydrivebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5620 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/azurebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1116 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    19552 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/idrivedbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15865 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/multibackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    20414 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/dpbxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7160 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/boxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1154 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/cfbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    20735 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/webdavbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10349 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/megav3backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2439 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/hubicbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10027 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/lftpbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6672 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/rsyncbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5710 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/ncftpbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     4824 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/mediafirebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1327 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/s3_boto_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2732 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/hsibackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9859 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/_boto_multi.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9178 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/par2backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    20341 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/ssh_paramiko_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12787 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/duplicity/backends/pcabackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     9999 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/s3_boto3_backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5693 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/jottacloudbackend.py
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity/backends/pyrax_identity/
--rw-r--r--   0 ken       (1000) ken       (1000)    10241 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/pyrax_identity/hubic.py
--rw-r--r--   0 ken       (1000) ken       (1000)      903 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/pyrax_identity/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10199 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/imapbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     3948 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/_cf_cloudfiles.py
--rw-r--r--   0 ken       (1000) ken       (1000)     5243 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/_cf_pyrax.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15676 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/_boto_single.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2579 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/README
--rw-r--r--   0 ken       (1000) ken       (1000)     2368 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/sxbackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     6630 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backends/slatebackend.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8735 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/dup_threading.py
--rw-r--r--   0 ken       (1000) ken       (1000)    68721 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/dup_main.py
--rw-r--r--   0 ken       (1000) ken       (1000)    27197 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/backend.py
--rw-r--r--   0 ken       (1000) ken       (1000)    11553 2023-03-12 17:52:34.000000 duplicity-1.2.3.dev27/duplicity/config.py
--rw-r--r--   0 ken       (1000) ken       (1000)     7714 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/globmatch.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1165 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/duplicity/__init__.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8762 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/librsync.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2789 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/errors.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10812 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/tempdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1303 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/tarfile.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13906 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/progress.py
--rw-r--r--   0 ken       (1000) ken       (1000)    17508 2023-03-07 18:50:39.000000 duplicity-1.2.3.dev27/duplicity/gpg.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2708 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/filechunkio.py
--rw-r--r--   0 ken       (1000) ken       (1000)    22629 2023-03-07 18:50:39.000000 duplicity-1.2.3.dev27/duplicity/patchdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)    18558 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/manifest.py
--rw-r--r--   0 ken       (1000) ken       (1000)    17200 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/file_naming.py
--rw-r--r--   0 ken       (1000) ken       (1000)    14510 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/_librsyncmodule.c
--rw-r--r--   0 ken       (1000) ken       (1000)    47632 2023-03-12 18:11:30.000000 duplicity-1.2.3.dev27/duplicity/dup_collections.py
--rw-r--r--   0 ken       (1000) ken       (1000)     2499 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/robust.py
--rw-r--r--   0 ken       (1000) ken       (1000)    58255 2023-03-12 19:33:36.000000 duplicity-1.2.3.dev27/duplicity/commandline.py
--rw-r--r--   0 ken       (1000) ken       (1000)    27140 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/diffdir.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1698 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/cached_ops.py
--rw-r--r--   0 ken       (1000) ken       (1000)    12804 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev27/duplicity/util.py
--rw-r--r--   0 ken       (1000) ken       (1000)     8286 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/dup_temp.py
--rw-r--r--   0 ken       (1000) ken       (1000)    10812 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/asyncscheduler.py
--rw-r--r--   0 ken       (1000) ken       (1000)    13348 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/statistics.py
--rw-r--r--   0 ken       (1000) ken       (1000)    15187 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/lazy.py
--rw-r--r--   0 ken       (1000) ken       (1000)    29244 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/path.py
--rw-r--r--   0 ken       (1000) ken       (1000)    29548 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/duplicity/selection.py
--rw-r--r--   0 ken       (1000) ken       (1000)    16103 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/log.py
--rw-r--r--   0 ken       (1000) ken       (1000)    23812 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/duplicity/gpginterface.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1284 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/README-LOG.md
--rw-rw-r--   0 ken       (1000) ken       (1000)     2715 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/PKG-INFO
--rw-r--r--   0 ken       (1000) ken       (1000)    18028 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/COPYING
--rw-r--r--   0 ken       (1000) ken       (1000)      164 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/crowdin.yml
--rw-r--r--   0 ken       (1000) ken       (1000)     3250 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/README-SNAP.md
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/
--rw-r--r--   0 ken       (1000) ken       (1000)    43314 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/fi_FI.po
--rw-r--r--   0 ken       (1000) ken       (1000)    62584 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ru_MD.po
--rw-r--r--   0 ken       (1000) ken       (1000)    57878 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/es_ES.po
--rw-r--r--   0 ken       (1000) ken       (1000)    54340 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/pt_BR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/uk_UA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32646 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/uk_UA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    44636 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/en_GB.po
--rw-r--r--   0 ken       (1000) ken       (1000)    52949 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/zh_CN.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43316 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/no_NO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/nl_NL/
--rw-rw-r--   0 ken       (1000) ken       (1000)      512 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/nl_NL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    54422 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/it_IT.po
--rw-r--r--   0 ken       (1000) ken       (1000)    58422 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/cs_CZ.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/hu_HU/
--rw-rw-r--   0 ken       (1000) ken       (1000)    25308 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/hu_HU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    59909 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/de_DE.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/es_ES/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33152 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/es_ES/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/zh_HK/
--rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/zh_HK/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43313 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/da_DK.po
--rw-r--r--   0 ken       (1000) ken       (1000)    55236 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/pl_PL.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43325 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/nl_SR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/vi_VN/
--rw-rw-r--   0 ken       (1000) ken       (1000)      510 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/vi_VN/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43314 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ca_ES.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/nl_BE/
--rw-rw-r--   0 ken       (1000) ken       (1000)      524 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/nl_BE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43735 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/el_GR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/it_IT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    25347 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/it_IT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43333 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/zh_HK.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ru_UA/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ru_UA/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/es_EM/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33161 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/es_EM/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43308 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ja_JP.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/pt_PT/
--rw-rw-r--   0 ken       (1000) ken       (1000)      520 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/pt_PT/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/zh_TW/
--rw-rw-r--   0 ken       (1000) ken       (1000)      522 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/zh_TW/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    59921 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/de_AT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/en_GB/
--rw-rw-r--   0 ken       (1000) ken       (1000)     3375 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/en_GB/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/cs_CZ/
--rw-rw-r--   0 ken       (1000) ken       (1000)    34670 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/cs_CZ/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/pl_PL/
--rw-rw-r--   0 ken       (1000) ken       (1000)    26950 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/pl_PL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43332 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/en_US.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/es_US/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33167 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/es_US/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/he_IL/
--rw-rw-r--   0 ken       (1000) ken       (1000)      964 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/he_IL/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43312 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/nl_NL.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ru_BY/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ru_BY/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/en_US/
--rw-rw-r--   0 ken       (1000) ken       (1000)      532 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/en_US/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ar_SA/
--rw-rw-r--   0 ken       (1000) ken       (1000)      598 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ar_SA/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/pt_BR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    24541 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/pt_BR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/tr_TR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     4256 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/tr_TR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/af_ZA/
--rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/af_ZA/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)     1184 2023-01-25 19:30:41.000000 duplicity-1.2.3.dev27/po/POTFILES.skip
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/nl_SR/
--rw-rw-r--   0 ken       (1000) ken       (1000)      525 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/nl_SR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ru_RU/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32865 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ru_RU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    62584 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ru_BY.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ca_ES/
--rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ca_ES/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43399 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/sr_SP.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43322 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/zh_TW.po
--rw-r--r--   0 ken       (1000) ken       (1000)    62584 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ru_UA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ko_KR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     7034 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ko_KR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43727 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/en_AU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/fi_FI/
--rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/fi_FI/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    62186 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/uk_UA.po
--rw-r--r--   0 ken       (1000) ken       (1000)     2285 2023-01-25 19:29:23.000000 duplicity-1.2.3.dev27/po/POTFILES.in
--rwxr-xr-x   0 ken       (1000) ken       (1000)      361 2023-01-13 18:29:53.000000 duplicity-1.2.3.dev27/po/update-pot
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/sr_SP/
--rw-rw-r--   0 ken       (1000) ken       (1000)      599 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/sr_SP/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/de_DE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    36226 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/de_DE/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/de_AT/
--rw-rw-r--   0 ken       (1000) ken       (1000)    36238 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/de_AT/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    62572 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ru_RU.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/sv_SE/
--rw-rw-r--   0 ken       (1000) ken       (1000)    24543 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/sv_SE/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    57344 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/fr_FR.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43320 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/pt_PT.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ro_RO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      559 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ro_RO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43398 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ar_SA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/el_GR/
--rw-rw-r--   0 ken       (1000) ken       (1000)     1574 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/el_GR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43549 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/he_IL.po
--rw-r--r--   0 ken       (1000) ken       (1000)    54689 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/hu_HU.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43324 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/nl_BE.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/en_AU/
--rw-rw-r--   0 ken       (1000) ken       (1000)     1412 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/en_AU/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43329 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/zh_MO.po
--rw-r--r--   0 ken       (1000) ken       (1000)    44655 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/tr_TR.po
--rw-r--r--   0 ken       (1000) ken       (1000)      276 2023-01-25 19:29:23.000000 duplicity-1.2.3.dev27/po/LINGUAS
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/da_DK/
--rw-rw-r--   0 ken       (1000) ken       (1000)      513 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/da_DK/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/zh_MO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      529 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/zh_MO/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/es_PR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33165 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/es_PR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/zh_SG/
--rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/zh_SG/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ja_JP/
--rw-rw-r--   0 ken       (1000) ken       (1000)      508 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ja_JP/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    57893 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/es_US.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/es_MX/
--rw-rw-r--   0 ken       (1000) ken       (1000)    33160 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/es_MX/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/ru_MD/
--rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/ru_MD/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43333 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/zh_SG.po
--rw-r--r--   0 ken       (1000) ken       (1000)    57886 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/es_MX.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/zh_CN/
--rw-rw-r--   0 ken       (1000) ken       (1000)    25656 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/zh_CN/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43330 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/en_PR.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43310 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/vi_VN.po
--rw-r--r--   0 ken       (1000) ken       (1000)    53746 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/sv_SE.po
--rw-r--r--   0 ken       (1000) ken       (1000)    57887 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/es_EM.po
--rw-r--r--   0 ken       (1000) ken       (1000)    43316 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/af_ZA.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/no_NO/
--rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/no_NO/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    57891 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/es_PR.po
--rw-r--r--   0 ken       (1000) ken       (1000)     1174 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/po/Makevars
--rw-r--r--   0 ken       (1000) ken       (1000)    46050 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ko_KR.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/en_PR/
--rw-rw-r--   0 ken       (1000) ken       (1000)      530 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/en_PR/duplicity.mo
--rw-r--r--   0 ken       (1000) ken       (1000)    43559 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/duplicity.pot
--rw-r--r--   0 ken       (1000) ken       (1000)    43359 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev27/po/ro_RO.po
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:28.000000 duplicity-1.2.3.dev27/po/fr_FR/
--rw-rw-r--   0 ken       (1000) ken       (1000)    29965 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/po/fr_FR/duplicity.mo
-drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity.egg-info/
--rw-rw-r--   0 ken       (1000) ken       (1000)       18 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity.egg-info/top_level.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)       17 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity.egg-info/requires.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)     2715 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity.egg-info/PKG-INFO
--rw-rw-r--   0 ken       (1000) ken       (1000)        1 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity.egg-info/dependency_links.txt
--rw-rw-r--   0 ken       (1000) ken       (1000)     7665 2023-03-13 12:27:27.000000 duplicity-1.2.3.dev27/duplicity.egg-info/SOURCES.txt
--rwxr-xr-x   0 ken       (1000) ken       (1000)    13544 2023-02-21 16:03:23.000000 duplicity-1.2.3.dev27/setup.py
--rw-r--r--   0 ken       (1000) ken       (1000)     1459 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/README.md
--rw-r--r--   0 ken       (1000) ken       (1000)     1357 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/README-REPO.md
--rw-r--r--   0 ken       (1000) ken       (1000)     5364 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev27/README-TESTING.md
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/
+-rw-r--r--   0 ken       (1000) ken       (1000)    95895 2023-03-16 18:49:20.000000 duplicity-1.2.3.dev43/CHANGELOG.md
+-rw-r--r--   0 ken       (1000) ken       (1000)      101 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/setup.cfg
+-rw-r--r--   0 ken       (1000) ken       (1000)      651 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/pylintrc
+-rw-r--r--   0 ken       (1000) ken       (1000)     1390 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/CONTRIBUTING.md
+-rw-r--r--   0 ken       (1000) ken       (1000)     2814 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev43/tox.ini
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/bin/
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     5215 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev43/bin/duplicity
+-rw-r--r--   0 ken       (1000) ken       (1000)     3108 2023-04-05 14:51:14.000000 duplicity-1.2.3.dev43/bin/rdiffdir.1
+-rw-r--r--   0 ken       (1000) ken       (1000)    98253 2023-04-05 14:51:14.000000 duplicity-1.2.3.dev43/bin/duplicity.1
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     9127 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/bin/rdiffdir
+-rw-r--r--   0 ken       (1000) ken       (1000)     1053 2023-04-05 14:50:34.000000 duplicity-1.2.3.dev43/requirements.txt
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/snap/
+-rw-r--r--   0 ken       (1000) ken       (1000)     5723 2023-04-05 14:51:14.000000 duplicity-1.2.3.dev43/snap/snapcraft.yaml
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/snap/local/
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      186 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/snap/local/debug.sh
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      110 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/snap/local/launcher.sh
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/testing/
+-rw-r--r--   0 ken       (1000) ken       (1000)   319661 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/testfiles.tar.gz
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/testing/unit/
+-rw-r--r--   0 ken       (1000) ken       (1000)     8373 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_gpginterface.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    11911 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_patchdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6777 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_dup_time.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12146 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_lazy.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5751 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_statistics.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    14365 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_globmatch.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5848 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_manifest.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1027 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12014 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_collections.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2566 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_dup_temp.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6028 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_file_naming.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1287 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_tarfile.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13493 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_diffdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2596 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_tempdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10376 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_backend_instance.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3877 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev43/testing/unit/test_path.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1546 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_util.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8686 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_gpg.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12435 2023-04-03 18:52:11.000000 duplicity-1.2.3.dev43/testing/unit/test_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    67031 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/unit/test_selection.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/testing/overrides/
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/testing/overrides/bin/
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      226 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/bin/ncftpget
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      593 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/bin/lftp
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      226 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/bin/ncftpput
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      494 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/bin/hsi
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      487 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/bin/tahoe
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      628 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/bin/ncftpls
+-rw-r--r--   0 ken       (1000) ken       (1000)      318 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/overrides/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5228 2023-04-05 14:50:34.000000 duplicity-1.2.3.dev43/testing/__init__.py
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      878 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/run-tests
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/testing/functional/
+-rw-r--r--   0 ken       (1000) ken       (1000)     2641 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_log.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9764 2023-04-05 14:50:34.000000 duplicity-1.2.3.dev43/testing/functional/test_final.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1724 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_badupload.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3513 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_cleanup.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9513 2023-04-05 14:50:34.000000 duplicity-1.2.3.dev43/testing/functional/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3514 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_replicate.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9126 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_verify.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    20273 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_restart.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3936 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/functional/test_rdiffdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)   111376 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/testing/functional/test_selection.py
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     3614 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/fix_unadorned_strings.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1083 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/conftest.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6236 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/test_code.py
+-rwxr-xr-x   0 ken       (1000) ken       (1000)     2979 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/find_unadorned_strings.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/testing/gnupg/
+-rw-r--r--   0 ken       (1000) ken       (1000)      145 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/gnupg/gpg-agent.conf
+-rw-r--r--   0 ken       (1000) ken       (1000)     3567 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/gnupg/pubring.gpg
+-rw-r--r--   0 ken       (1000) ken       (1000)     7549 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/gnupg/secring.gpg
+-rw-r--r--   0 ken       (1000) ken       (1000)      425 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/gnupg/gpg.conf
+-rw-r--r--   0 ken       (1000) ken       (1000)      255 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/gnupg/README
+-rw-r--r--   0 ken       (1000) ken       (1000)     1440 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/testing/gnupg/trustdb.gpg
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity/
+-rw-r--r--   0 ken       (1000) ken       (1000)    11648 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/dup_time.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity/backends/
+-rw-r--r--   0 ken       (1000) ken       (1000)     3033 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/localbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    16858 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev43/duplicity/backends/onedrivebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    17385 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/adbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8839 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/megav2backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10572 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/swiftbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     4474 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/rclonebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9599 2023-03-16 15:21:39.000000 duplicity-1.2.3.dev43/duplicity/backends/b2backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2645 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/tahoebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    16496 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/gdrivebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13658 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/ssh_pexpect_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9393 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/gdocsbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8216 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/giobackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6895 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/megabackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13014 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/pydrivebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5620 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/azurebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1116 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    19552 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/idrivedbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    15865 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/multibackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    20414 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/dpbxbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     7160 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/boxbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1154 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/cfbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    20735 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/webdavbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10349 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/megav3backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2439 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/hubicbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10027 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/lftpbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6672 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/rsyncbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5710 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/ncftpbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     4824 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/mediafirebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1327 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/s3_boto_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2732 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/hsibackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9859 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/_boto_multi.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9178 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/par2backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    20341 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/ssh_paramiko_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12787 2023-03-07 16:20:30.000000 duplicity-1.2.3.dev43/duplicity/backends/pcabackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     9999 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/s3_boto3_backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5693 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/jottacloudbackend.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity/backends/pyrax_identity/
+-rw-r--r--   0 ken       (1000) ken       (1000)    10241 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/pyrax_identity/hubic.py
+-rw-r--r--   0 ken       (1000) ken       (1000)      903 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/pyrax_identity/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10199 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/imapbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     3948 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/_cf_cloudfiles.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     5243 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/_cf_pyrax.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    15676 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/_boto_single.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2579 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/README
+-rw-r--r--   0 ken       (1000) ken       (1000)     2368 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backends/sxbackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12292 2023-04-03 18:52:11.000000 duplicity-1.2.3.dev43/duplicity/backends/xorrisobackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     6631 2023-03-15 14:35:48.000000 duplicity-1.2.3.dev43/duplicity/backends/slatebackend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8735 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/dup_threading.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    68721 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/dup_main.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    27197 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/backend.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    11553 2023-03-12 17:52:34.000000 duplicity-1.2.3.dev43/duplicity/config.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     7714 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/globmatch.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1165 2023-04-05 14:51:14.000000 duplicity-1.2.3.dev43/duplicity/__init__.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8762 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/librsync.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2789 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/errors.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10812 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/tempdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1303 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/tarfile.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13906 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/progress.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    17508 2023-03-07 18:50:39.000000 duplicity-1.2.3.dev43/duplicity/gpg.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2708 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/filechunkio.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    22629 2023-03-07 18:50:39.000000 duplicity-1.2.3.dev43/duplicity/patchdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    18558 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/manifest.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    17200 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/file_naming.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    14510 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/_librsyncmodule.c
+-rw-r--r--   0 ken       (1000) ken       (1000)    47632 2023-03-12 18:11:30.000000 duplicity-1.2.3.dev43/duplicity/dup_collections.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     2514 2023-03-24 17:54:59.000000 duplicity-1.2.3.dev43/duplicity/robust.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    58255 2023-03-12 19:33:36.000000 duplicity-1.2.3.dev43/duplicity/commandline.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    27140 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/diffdir.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1698 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/cached_ops.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    12804 2023-03-28 15:21:45.000000 duplicity-1.2.3.dev43/duplicity/util.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     8286 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/dup_temp.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    10812 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/asyncscheduler.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    13348 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/statistics.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    15187 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/lazy.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    29244 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/path.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    29548 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/duplicity/selection.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    16103 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/duplicity/log.py
+-rw-r--r--   0 ken       (1000) ken       (1000)    23813 2023-03-15 14:35:48.000000 duplicity-1.2.3.dev43/duplicity/gpginterface.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1284 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/README-LOG.md
+-rw-rw-r--   0 ken       (1000) ken       (1000)     2770 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/PKG-INFO
+-rw-r--r--   0 ken       (1000) ken       (1000)    18028 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/COPYING
+-rw-r--r--   0 ken       (1000) ken       (1000)      164 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/crowdin.yml
+-rw-r--r--   0 ken       (1000) ken       (1000)     3250 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/README-SNAP.md
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/
+-rw-r--r--   0 ken       (1000) ken       (1000)    43314 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/fi_FI.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    62584 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ru_MD.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    57878 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/es_ES.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    54340 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/pt_BR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/uk_UA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32646 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/uk_UA/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    44636 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/en_GB.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    52949 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/zh_CN.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43316 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/no_NO.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/nl_NL/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      512 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/nl_NL/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    54422 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/it_IT.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    58422 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/cs_CZ.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/hu_HU/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    25308 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/hu_HU/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    59909 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/de_DE.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_ES/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33152 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_ES/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_HK/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_HK/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43313 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/da_DK.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    55236 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/pl_PL.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43325 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/nl_SR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/vi_VN/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      510 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/vi_VN/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43314 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ca_ES.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/nl_BE/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      524 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/nl_BE/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43735 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/el_GR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/it_IT/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    25347 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/it_IT/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43333 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/zh_HK.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_UA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_UA/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_EM/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33161 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_EM/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43308 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ja_JP.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/pt_PT/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      520 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/pt_PT/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_TW/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      522 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_TW/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    59921 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/de_AT.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_GB/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     3375 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_GB/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/cs_CZ/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    34670 2023-04-05 14:51:12.000000 duplicity-1.2.3.dev43/po/cs_CZ/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/pl_PL/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    26950 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/pl_PL/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43332 2023-03-20 16:30:59.000000 duplicity-1.2.3.dev43/po/en_US.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_US/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33167 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_US/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/he_IL/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      964 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/he_IL/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43312 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/nl_NL.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_BY/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_BY/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_US/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      532 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_US/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ar_SA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      598 2023-04-05 14:51:12.000000 duplicity-1.2.3.dev43/po/ar_SA/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/pt_BR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    24541 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/pt_BR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/tr_TR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     4256 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/tr_TR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/af_ZA/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-04-05 14:51:12.000000 duplicity-1.2.3.dev43/po/af_ZA/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)     1184 2023-01-25 19:30:41.000000 duplicity-1.2.3.dev43/po/POTFILES.skip
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/nl_SR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      525 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/nl_SR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_RU/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32865 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_RU/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    62584 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ru_BY.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ca_ES/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-04-05 14:51:12.000000 duplicity-1.2.3.dev43/po/ca_ES/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43399 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/sr_SP.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43322 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/zh_TW.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    62584 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ru_UA.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ko_KR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     7034 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ko_KR/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43727 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/en_AU.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/fi_FI/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      514 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/fi_FI/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    62186 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/uk_UA.po
+-rw-r--r--   0 ken       (1000) ken       (1000)     2285 2023-01-25 19:29:23.000000 duplicity-1.2.3.dev43/po/POTFILES.in
+-rwxr-xr-x   0 ken       (1000) ken       (1000)      361 2023-01-13 18:29:53.000000 duplicity-1.2.3.dev43/po/update-pot
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/sr_SP/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      599 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/sr_SP/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/de_DE/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    36226 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/de_DE/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/de_AT/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    36238 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/de_AT/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    62572 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ru_RU.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/sv_SE/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    24543 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/sv_SE/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    57344 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/fr_FR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43320 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/pt_PT.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ro_RO/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      559 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ro_RO/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43398 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ar_SA.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/el_GR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1574 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/el_GR/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43549 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/he_IL.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    54689 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/hu_HU.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43324 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/nl_BE.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_AU/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1412 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_AU/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43329 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/zh_MO.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    44655 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/tr_TR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)      276 2023-01-25 19:29:23.000000 duplicity-1.2.3.dev43/po/LINGUAS
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/da_DK/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      513 2023-04-05 14:51:12.000000 duplicity-1.2.3.dev43/po/da_DK/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_MO/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      529 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_MO/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_PR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33165 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_PR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_SG/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      533 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_SG/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ja_JP/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      508 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ja_JP/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    57893 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/es_US.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_MX/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    33160 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/es_MX/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_MD/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    32877 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/ru_MD/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43333 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/zh_SG.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    57886 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/es_MX.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_CN/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    25656 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/zh_CN/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43330 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/en_PR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43310 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/vi_VN.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    53746 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/sv_SE.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    57887 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/es_EM.po
+-rw-r--r--   0 ken       (1000) ken       (1000)    43316 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/af_ZA.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/no_NO/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      516 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/no_NO/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    57891 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/es_PR.po
+-rw-r--r--   0 ken       (1000) ken       (1000)     1174 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/po/Makevars
+-rw-r--r--   0 ken       (1000) ken       (1000)    46050 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ko_KR.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_PR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)      530 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/en_PR/duplicity.mo
+-rw-r--r--   0 ken       (1000) ken       (1000)    43559 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/duplicity.pot
+-rw-r--r--   0 ken       (1000) ken       (1000)    43359 2023-02-06 15:48:19.000000 duplicity-1.2.3.dev43/po/ro_RO.po
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/fr_FR/
+-rw-rw-r--   0 ken       (1000) ken       (1000)    29965 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/po/fr_FR/duplicity.mo
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity.egg-info/
+-rw-rw-r--   0 ken       (1000) ken       (1000)       18 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity.egg-info/top_level.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)       17 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity.egg-info/requires.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)     2770 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity.egg-info/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1000)        1 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity.egg-info/dependency_links.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)     7689 2023-04-05 14:51:13.000000 duplicity-1.2.3.dev43/duplicity.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ken       (1000) ken       (1000)    13544 2023-02-21 16:03:23.000000 duplicity-1.2.3.dev43/setup.py
+-rw-r--r--   0 ken       (1000) ken       (1000)     1514 2023-03-21 18:05:37.000000 duplicity-1.2.3.dev43/README.md
+-rw-r--r--   0 ken       (1000) ken       (1000)     1357 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/README-REPO.md
+-rw-r--r--   0 ken       (1000) ken       (1000)     5364 2022-12-27 19:32:15.000000 duplicity-1.2.3.dev43/README-TESTING.md
```

### Comparing `duplicity-1.2.3.dev27/CHANGELOG.md` & `duplicity-1.2.3.dev43/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,123 @@
+## (unreleased)
+
+### New
+
+* Onedrive for Business Support. [Tobias Simetsreiter]
+
+### Changes
+
+* Fix spelling errors. [Barak A. Pearlmutter]
+
+* Chg:pkg:  Cleanup.  Add 'unsquashfs -l' test from @ede. [Kenneth Loafman]
+
+* Update Makefile 'make clean' list. [Kenneth Loafman]
+
+* Fix run website ci call after pushes/releases. [ede]
+
+  [skip_tests]
+
+* Update version for Launchpad. [Kenneth Loafman]
+
+### Fix
+
+* Fixes #701 - unable to resume full backup to B2. [Kenneth Loafman]
+
+  Now tries .name and .uc_name before failing.
+
+* Fixes #698 - backups without GPG decryption key. [Kenneth Loafman]
+
+  Added option --no-check-remote to skip checking the   remote manifest.
+  The default is to check.
+
+* Fixes #698 - backups without GPG decryption key. [Kenneth Loafman]
+
+  Added option --no-check-remote to skip checking the   remote manifest.
+  The default is to check.
+
+* Fixes #686 - PCA backend does not unseal volumes. [Kenneth Loafman]
+
+  Patch supplied by Bertrand Marc, user @bmarc.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Skip test\_path::test\_compare on non-native. [Kenneth Loafman]
+
+  Skip on GitLab and Launchpad build systems.   Works fine on Linux and
+  macOS.
+
+* Revert to medieval string formatting. [Kenneth Loafman]
+
+* Revert to medieval string formatting. [Kenneth Loafman]
+
+* Revert to medieval string formatting. [Kenneth Loafman]
+
+* Revert to medieval string formatting. [Kenneth Loafman]
+
+* Remove dependency scanner. [Kenneth Loafman]
+
+* Fix PEP8 and todo issues. [Kenneth Loafman]
+
+* Misc fixes to testing/build environ. [Kenneth Loafman]
+
+  start_debugger now supports multiprocess debug.   restore
+  testing.unit.test_path.test_compare
+
+* Encoding errors when logging.  Fixes #693. [Kenneth Loafman]
+
+  Use os.fsdecode/os.fsencode when in py3.
+
+* Onedrive may hang indefinitely.  Fixes #695. [Kenneth Loafman]
+
+### Other
+
+* Fix typo. [ede]
+
+* Try to fix. [ede]
+
+  Executing "step_script" stage of the job script   00:00   Using docker
+  image sha256:3148ec916ea71d90f1beae623b3c5eb4a2db5a585db3178d9619bc2fe
+  b8f5f49 for curlimages/curl:latest with digest curlimages/curl@sha256:
+  f7f265d5c64eb4463a43a99b6bf773f9e61a50aaa7cefaf564f43e42549a01dd ...
+  /bin/sh: eval: line 136: apt-get: not found
+
+
 ## rel.1.2.2 (2023-01-26)
 
 ### Changes
 
 * \_runtest\_dir on Darwin may use TMPDIR for testing. [Kenneth Loafman]
 
 * Update duplicity.pot. [Kenneth Loafman]
```

### Comparing `duplicity-1.2.3.dev27/pylintrc` & `duplicity-1.2.3.dev43/pylintrc`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/CONTRIBUTING.md` & `duplicity-1.2.3.dev43/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/tox.ini` & `duplicity-1.2.3.dev43/tox.ini`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/bin/duplicity` & `duplicity-1.2.3.dev43/bin/duplicity`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/bin/rdiffdir.1` & `duplicity-1.2.3.dev43/bin/rdiffdir.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH RDIFFDIR 1 "March 13, 2023" "Version 1.2.3.dev27" "User Manuals" \"  -*- nroff -*-
+.TH RDIFFDIR 1 "April 05, 2023" "Version 1.2.3.dev43" "User Manuals" \"  -*- nroff -*-
 .\" disable justification (adjust text to left margin only)
 .\" command line examples stay readable through that
 .ad l
 .\" disable hyphenation
 .nh
 
 .SH NAME
```

### Comparing `duplicity-1.2.3.dev27/bin/duplicity.1` & `duplicity-1.2.3.dev43/bin/duplicity.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH DUPLICITY 1 "March 13, 2023" "Version 1.2.3.dev27" "User Manuals" \"  -*- nroff -*-
+.TH DUPLICITY 1 "April 05, 2023" "Version 1.2.3.dev43" "User Manuals" \"  -*- nroff -*-
 .\" disable justification (adjust text to left margin only)
 .\" command line examples stay readable through that
 .ad l
 .\" disable hyphenation
 .nh
 
 .SH NAME
@@ -150,15 +150,15 @@
 If a backup is in order and old signatures can be found duplicity automatically
 performs an incremental backup.
 .PP
 .B NOTE:
 The following explanations explain some but
 .B not
 all options that can be used in connection with that action command.
-Consult the OPTIONS section for more detailed informations.
+Consult the OPTIONS section for more detailed information.
 
 .TP
 .BI "full " "<folder> <url>"
 Perform a full backup. A new backup chain is started even if
 signatures are available for an incremental backup.
 
 .TP
@@ -179,15 +179,15 @@
 unless the --compare-data option is used (see below).
 .br
 The
 .I --file-to-restore
 option restricts verify to that file or folder.
 The
 .I --time
-option allows to select a backup to verify.
+option allows one to select a backup to verify.
 The
 .I --compare-data
 option enables data comparison (see below).
 
 .TP
 .BI "collection-status " "[--file-changed <relpath>] [--show-changes-in-set <index>] <url>"
 Summarize the status of the backup repository by printing the chains
@@ -366,15 +366,15 @@
 .BI "--azure-max-connections"
 Specify the number of maximum connections to transfer one blob to Azure
 blob size exceeds 64MB. The default values is 2.
 
 .TP
 .BI "--backend-retry-delay " number
 Specifies the number of seconds that duplicity waits after an error has
-occured before attempting to repeat the operation.
+occurred before attempting to repeat the operation.
 
 .TP
 .BI "--cf-backend " backend
 Allows the explicit selection of a cloudfiles backend. Defaults to
 .BR pyrax .
 Alternatively you might choose
 .BR cloudfiles .
@@ -1316,29 +1316,29 @@
 
 .TP
 .B TMPDIR, TEMP, TMP
 In decreasing order of importance, specifies the directory to use for
 temporary files (inherited from Python's tempfile module).
 Eventually the option
 .BI --tempdir
-supercedes any of these.
+supersedes any of these.
 .TP
 .B FTP_PASSWORD
 Supported by most backends which are password capable. More secure than
 setting it in the backend url (which might be readable in the operating
 systems process listing to other users on the same machine).
 .TP
 .B PASSPHRASE
 This passphrase is passed to GnuPG. If this is not set, the user will be
 prompted for the passphrase.
 .TP
 .B SIGN_PASSPHRASE
 The passphrase to be used for
 .BR --sign-key .
-If ommitted
+If omitted
 .B and
 sign key is also one of the keys to encrypt against
 .B PASSPHRASE
 will be reused instead.
 Otherwise, if passphrase is needed but not set the user will be prompted for it.
 
 Other environment variables may be used to configure specific backends.
@@ -1467,15 +1467,15 @@
 .B boto
 backend. default is boto3+s3://
 
 See
 .B "A NOTE ON GOOGLE CLOUD STORAGE"
 about
 .B needed
-endpoint option and env vars for authentification.
+endpoint option and env vars for authentication.
 .RE
 
 .TP
 .B "Google Docs"
 .RS
 gdocs://user[:password]@other.host/some_dir
 
@@ -1681,14 +1681,25 @@
 .RS
 webdav[s]://user[:password]@other.host[:port]/some_dir
 
 .B alternatively
 try lftp+webdav[s]://
 .RE
 
+.TP
+.B "Optical media (ISO9660 CD/DVD/Bluray using xorriso)"
+.RS
+xorriso:///dev/byOpticalDrive[:/path/to/directory/on/iso]
+xorriso:///path/to/image.iso[:/path/to/directory/on/iso]
+
+
+See also
+.B "A NOTE ON THE XORRISO BACKEND"
+.RE
+
 .SH TIME FORMATS
 duplicity uses time strings in two places.  Firstly, many of the files
 duplicity creates will have the time in their filenames in the w3
 datetime format as described in a w3 note at
 http://www.w3.org/TR/NOTE-datetime.  Basically they look like
 "2001-07-15T04:09:38-07:00", which means what it looks like.  The
 "-07:00" section means the time zone is 7 hours behind UTC.
@@ -1901,15 +1912,15 @@
 options, should the directory portion of the path (/usr/bin) contain any
 uppercase characters.
 
 If the pattern starts with "ignorecase:" (case insensitive), then
 this prefix will be removed and any character in the string can be
 replaced with an upper- or lowercase version of itself. This prefix is a
 legacy feature supported for shell globbing selection conditions only,
-but for backward compatability reasons is otherwise considered part of
+but for backward compatibility reasons is otherwise considered part of
 the pattern itself (use
 .B --filter-ignorecase
 instead).
 
 Remember that you may need to quote patterns when typing them
 into a shell, so the shell does not interpret the globbing patterns
 or whitespace characters before duplicity sees them.
@@ -2149,15 +2160,15 @@
 backend does not currently support initiating restores
 from the glacier storage class.  When restoring a backup from
 glacier or glacier deep archive, the backup files must first be
 restored out of band.  There are multiple options when restoring
 backups from cold storage, which vary in both cost and speed.
 See Amazon's documentation for details.
 
-Both backends use environment variables for authentification:
+Both backends use environment variables for authentication:
 .br
 .RS
 .BR AWS_ACCESS_KEY_ID " (required),"
 .br
 .BR AWS_SECRET_ACCESS_KEY " (required)"
 .br
 or
@@ -2184,15 +2195,15 @@
 legacy
 .BR "boto backend" " example backup command line:"
 
 .RS
 AWS_ACCESS_KEY_ID=<key_id> AWS_SECRET_ACCESS_KEY=<access_key> duplicity /some/path boto+s3://[host:port]/bucket/subfolder
 .RE
 
-.RB "The url host setting is optional and allows to define a custom endpoint host. you may add " "--s3-european-buckets"
+.RB "The url host setting is optional and allows one to define a custom endpoint host. you may add " "--s3-european-buckets"
 and other s3 options documented above if needed.
 
 
 .SH A NOTE ON AZURE ACCESS
 The Azure backend requires the Microsoft Azure Storage Blobs client library
 for Python to be installed on the system.
 See
@@ -2236,15 +2247,15 @@
 .BR REQUIREMENTS .
 
 It uses the environment variable
 .BR BOX_CONFIG_PATH " (optional)."
 This string contains the path to box custom app's config.json. Either this environment variable or
 the
 .BR config
-query parameter in the url need to be specified, if both are specified, query paramter takes precedence.
+query parameter in the url need to be specified, if both are specified, query parameter takes precedence.
 
 .SS Create a Box custom app
 In order to use box backend, user need to create a box custom app in the box developer console (https://app.box.com/developers/console).
 
 After create a new custom app, please make sure it is configured as follow:
 
 .RS
@@ -2275,15 +2286,15 @@
 Object Storage protocol.  Users wishing to use Duplicity with Rackspace
 Cloud Files should migrate to the new Pyrax plugin to ensure support.
 
 The backend requires python-cloudfiles to be installed on the system.
 See
 .BR REQUIREMENTS .
 
-It uses three environment variables for authentification:
+It uses three environment variables for authentication:
 .BR CLOUDFILES_USERNAME " (required),"
 .BR CLOUDFILES_APIKEY " (required),"
 .BR CLOUDFILES_AUTHURL " (optional)"
 
 If
 .B CLOUDFILES_AUTHURL
 is unspecified it will default to the value
@@ -2602,15 +2613,15 @@
 
 The destination folder will be created for you if it does not exist.
 
 .SH A NOTE ON MULTI BACKEND
 The multi backend allows duplicity to combine the storage available in
 more than one backend store (e.g., you can store across a google drive
 account and a onedrive account to get effectively the combined storage
-available in both).  The URL path specifies a JSON formated config
+available in both).  The URL path specifies a JSON formatted config
 file containing a list of the backends it will use. The URL may also
 specify "query" parameters to configure overall behavior.
 Each element of the list must have a "url" element, and may also contain
 an optional "description" and an optional "env" list of environment
 variables used to configure that backend.
 .SS Query Parameters
 Query parameters come after the file URL in standard HTTP format
@@ -2740,25 +2751,25 @@
 .I percent.
 
 .SH A NOTE ON PCA ACCESS
 PCA is a long-term data archival solution by OVH. It runs a slightly modified
 version of Openstack Swift introducing latency in the data retrieval process.
 It is a good pick for a
 .BR "multi backend "
-configuration where receiving volumes while an other backend is used to store
+configuration where receiving volumes while another backend is used to store
 manifests and signatures.
 
 .br
 The backend requires python-switclient to be installed on the system.
 python-keystoneclient is also needed to interact with OpenStack's Keystone
 Identity service.
 See
 .BR REQUIREMENTS .
 
-It uses following environment variables for authentification:
+It uses following environment variables for authentication:
 .BR PCA_USERNAME " (required),"
 .BR PCA_PASSWORD " (required),"
 .BR PCA_AUTHURL " (required),"
 .BR PCA_USERID " (optional),"
 .BR PCA_TENANTID " (optional, but either the tenant name or tenant id must be supplied)"
 .BR PCA_REGIONNAME " (optional),"
 .BR PCA_TENANTNAME " (optional, but either the tenant name or tenant id must be supplied)"
@@ -2790,15 +2801,15 @@
 
 Download the .p12 key file of the account and convert it to the .pem format:
 .br
 openssl pkcs12 -in XXX.p12  -nodes -nocerts > pydriveprivatekey.pem
 
 The content of .pem file should be passed to
 .BR GOOGLE_DRIVE_ACCOUNT_KEY
-environment variable for authentification.
+environment variable for authentication.
 
 The email address of the account will be used as part of URL. See
 .B URL FORMAT
 above.
 
 The alternative is to use a regular account. To do this, start as above,
 but when creating a new Client ID, select "Installed application" of
@@ -2911,15 +2922,15 @@
 .br
 paramiko & pexpect support
 .BR --use-scp ,
 .BR --ssh-askpass " and"
 .BR --ssh-options "."
 Only the
 .B pexpect
-backend allows to define
+backend allows one to define
 .BR --scp-command " and"
 .BR --sftp-command .
 .PP
 .BR "SSH paramiko backend " "(default)"
 is a complete reimplementation of ssh protocols natively in python. Advantages
 are speed and maintainability. Minor disadvantage is that extra packages are
 needed as listed in
@@ -2990,27 +3001,27 @@
 Duplicity searches it there in the same order and will fail if it can't find it.
 You can however specify the option
 .BI --ssl-cacert-file " <file>"
 to point duplicity to a copy in a different location.
 .PP
 Finally there is the
 .BI --ssl-no-check-certificate
-option to disable certificate verification alltogether, in case some ssl library
+option to disable certificate verification altogether, in case some ssl library
 is missing or verification is not wanted. Use it with care, as even with self signed
 servers manually providing the private ca certificate is definitely the safer option.
 
 .SH A NOTE ON SWIFT (OPENSTACK OBJECT STORAGE) ACCESS
 Swift is the OpenStack Object Storage service.
 .br
 The backend requires python-switclient to be installed on the system.
 python-keystoneclient is also needed to use OpenStack's Keystone Identity service.
 See
 .BR REQUIREMENTS .
 
-It uses following environment variables for authentification:
+It uses following environment variables for authentication:
 
 .RS
 .BR SWIFT_USERNAME " (required),"
 .br
 .BR SWIFT_PASSWORD " (required),"
 .br
 .BR SWIFT_AUTHURL " (required),"
@@ -3051,14 +3062,29 @@
 .B empty
 passphrase.
 .PP
 3. The used
 .BI PASSPHRASE
 for symmetric encryption and the passphrase of the signing key are identical.
 
+.SH A NOTE ON THE XORRISO BACKEND
+
+This backend uses the xorriso tool to append backups to optical media or ISO9660 images.
+
+Use the following environment variables for more settings:
+.RS
+. BR XORRISO_PATH ", set an alternative path to the xorriso executable"
+. br
+. BR XORRISO_WRITE_SPEED ", specify the speed for writing to the optical disc. One of [min, max]"
+. br
+. BR XORRISO_ASSERT_VOLID ", specify the required volume ID of the ISO. Aborts when the actual volume ID is different."
+. br
+. BR XORRISO_ARGS ", for expert use only. Pass arbitrary arguments to xorriso. Example: XORRISO_ARGS='-md5 all'"
+.RE
+
 .SH KNOWN ISSUES / BUGS
 Hard links currently unsupported (they will be treated as non-linked
 regular files).
 
 Bad signatures will be treated as empty instead of logging appropriate
 error message.
 
@@ -3256,14 +3282,18 @@
 .B Python kerberos module
 for kerberos authentication
 - https://github.com/02strich/pykerberos
 .TP
 .BR "MediaFire backend"
 .B MediaFire Python Open SDK
 - https://pypi.python.org/pypi/mediafire/
+.TP
+.BR "xorriso backend"
+.B xorriso
+- https://www.gnu.org/software/xorriso/
 
 .SH AUTHOR
 .TP
 .BR "Original Author" " - Ben Escoto <bescoto@stanford.edu>"
 .TP
 .BR "Current Maintainer" " - Kenneth Loafman <kenneth@loafman.com>"
 .TP
```

### Comparing `duplicity-1.2.3.dev27/bin/rdiffdir` & `duplicity-1.2.3.dev43/bin/rdiffdir`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/requirements.txt` & `duplicity-1.2.3.dev43/requirements.txt`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/snap/snapcraft.yaml` & `duplicity-1.2.3.dev43/snap/snapcraft.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: duplicity
-version: 1.2.3.dev27
+version: 1.2.3.dev43
 license: GPL-2.0
 summary: Efficient, encrypted backup to local or remote hosts
 description: |
   Duplicity backs directories by producing encrypted tar-format volumes and uploading
   them to a remote or local file server. Because duplicity uses librsync, the incremental
   archives are space efficient and only record the parts of files that have changed since
   the last backup. Because duplicity uses GnuPG to encrypt and/or sign these archives,
```

### Comparing `duplicity-1.2.3.dev27/testing/testfiles.tar.gz` & `duplicity-1.2.3.dev43/testing/testfiles.tar.gz`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_gpginterface.py` & `duplicity-1.2.3.dev43/testing/unit/test_gpginterface.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_patchdir.py` & `duplicity-1.2.3.dev43/testing/unit/test_patchdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_dup_time.py` & `duplicity-1.2.3.dev43/testing/unit/test_dup_time.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_lazy.py` & `duplicity-1.2.3.dev43/testing/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_statistics.py` & `duplicity-1.2.3.dev43/testing/unit/test_statistics.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_globmatch.py` & `duplicity-1.2.3.dev43/testing/unit/test_globmatch.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_manifest.py` & `duplicity-1.2.3.dev43/testing/unit/test_manifest.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/__init__.py` & `duplicity-1.2.3.dev43/testing/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_collections.py` & `duplicity-1.2.3.dev43/testing/unit/test_collections.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_dup_temp.py` & `duplicity-1.2.3.dev43/testing/unit/test_dup_temp.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_file_naming.py` & `duplicity-1.2.3.dev43/testing/unit/test_file_naming.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_tarfile.py` & `duplicity-1.2.3.dev43/testing/unit/test_tarfile.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_diffdir.py` & `duplicity-1.2.3.dev43/testing/unit/test_diffdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_tempdir.py` & `duplicity-1.2.3.dev43/testing/unit/test_tempdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_backend_instance.py` & `duplicity-1.2.3.dev43/testing/unit/test_backend_instance.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_path.py` & `duplicity-1.2.3.dev43/testing/unit/test_path.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_util.py` & `duplicity-1.2.3.dev43/testing/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_gpg.py` & `duplicity-1.2.3.dev43/testing/unit/test_gpg.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_backend.py` & `duplicity-1.2.3.dev43/testing/unit/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,22 @@
         assert pu.username == u"foo@bar.com", pu.username
         assert pu.password is None, pu.password
         assert pu.port is None, pu.port
 
         pu = duplicity.backend.ParsedUrl(u"scheme://username:passwor@127.0.0.1:22/path/path")
         assert pu.strip_auth() == u"scheme://127.0.0.1:22/path/path"
 
+        pu = duplicity.backend.ParsedUrl(u"xorriso:///dev/sr0")
+        assert pu.scheme == u"xorriso", pu.scheme
+        assert pu.path == u"///dev/sr0", pu.path
+
+        pu = duplicity.backend.ParsedUrl(u"xorriso:///dev/sr0:/path/on/iso")
+        assert pu.scheme == u"xorriso", pu.scheme
+        assert pu.path == u"///dev/sr0:/path/on/iso", pu.path
+
     def test_errors(self):
         u"""Test various url errors"""
         self.assertRaises(InvalidBackendURL, duplicity.backend.ParsedUrl,
                           u"file:path")  # no relative paths for non-netloc schemes
         self.assertRaises(UnsupportedBackendScheme, duplicity.backend.get_backend,
                           u"ssh://foo@bar:pass@example.com/home")
```

### Comparing `duplicity-1.2.3.dev27/testing/unit/test_selection.py` & `duplicity-1.2.3.dev43/testing/unit/test_selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/overrides/bin/lftp` & `duplicity-1.2.3.dev43/testing/overrides/bin/lftp`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/overrides/bin/ncftpls` & `duplicity-1.2.3.dev43/testing/overrides/bin/ncftpls`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/__init__.py` & `duplicity-1.2.3.dev43/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/run-tests` & `duplicity-1.2.3.dev43/testing/run-tests`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_log.py` & `duplicity-1.2.3.dev43/testing/functional/test_log.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_final.py` & `duplicity-1.2.3.dev43/testing/functional/test_final.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_badupload.py` & `duplicity-1.2.3.dev43/testing/functional/test_badupload.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_cleanup.py` & `duplicity-1.2.3.dev43/testing/functional/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/__init__.py` & `duplicity-1.2.3.dev43/testing/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_replicate.py` & `duplicity-1.2.3.dev43/testing/functional/test_replicate.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_verify.py` & `duplicity-1.2.3.dev43/testing/functional/test_verify.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_restart.py` & `duplicity-1.2.3.dev43/testing/functional/test_restart.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_rdiffdir.py` & `duplicity-1.2.3.dev43/testing/functional/test_rdiffdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/functional/test_selection.py` & `duplicity-1.2.3.dev43/testing/functional/test_selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/fix_unadorned_strings.py` & `duplicity-1.2.3.dev43/testing/fix_unadorned_strings.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/conftest.py` & `duplicity-1.2.3.dev43/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/test_code.py` & `duplicity-1.2.3.dev43/testing/test_code.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/find_unadorned_strings.py` & `duplicity-1.2.3.dev43/testing/find_unadorned_strings.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/gnupg/pubring.gpg` & `duplicity-1.2.3.dev43/testing/gnupg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/gnupg/secring.gpg` & `duplicity-1.2.3.dev43/testing/gnupg/secring.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/testing/gnupg/trustdb.gpg` & `duplicity-1.2.3.dev43/testing/gnupg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/dup_time.py` & `duplicity-1.2.3.dev43/duplicity/dup_time.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/localbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/localbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/onedrivebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/onedrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/adbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/adbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/megav2backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/megav2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/swiftbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/swiftbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/rclonebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/rclonebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/b2backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/b2backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,20 @@
                                     util.fsdecode(local_path.name)),
                 log.INFO)
         if self.v_num < [1, 11, 0]:
             self.bucket.download_file_by_name(quote_plus(self.path + util.fsdecode(remote_filename), u'/'),
                                               DownloadDestLocalFile(local_path.name))
         else:
             df = self.bucket.download_file_by_name(quote_plus(self.path + util.fsdecode(remote_filename), u'/'))
-            df.save_to(util.fsdecode(local_path.name))
+            try:
+                # b2sdk >= 1.19.0
+                df.save_to(local_path.uc_name)
+            except:
+                # b2sdk < 1.19.0
+                df.save_to(local_path.name)
 
     def _put(self, source_path, remote_filename):
         u"""
         Copy source_path to remote_filename
         """
         log.Log(u"Put: %s -> %s" % (util.fsdecode(source_path.name),
                                     self.path + util.fsdecode(remote_filename)),
```

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/tahoebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/tahoebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/gdrivebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/gdrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/ssh_pexpect_backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/ssh_pexpect_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/gdocsbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/gdocsbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/giobackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/giobackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/megabackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/megabackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/pydrivebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/pydrivebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/azurebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/azurebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/__init__.py` & `duplicity-1.2.3.dev43/duplicity/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/idrivedbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/idrivedbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/multibackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/multibackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/dpbxbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/dpbxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/boxbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/boxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/cfbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/cfbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/webdavbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/webdavbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/megav3backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/megav3backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/hubicbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/hubicbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/lftpbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/lftpbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/rsyncbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/rsyncbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/ncftpbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/ncftpbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/mediafirebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/mediafirebackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/s3_boto_backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/s3_boto_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/hsibackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/hsibackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/_boto_multi.py` & `duplicity-1.2.3.dev43/duplicity/backends/_boto_multi.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/par2backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/par2backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/ssh_paramiko_backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/ssh_paramiko_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/pcabackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/pcabackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/s3_boto3_backend.py` & `duplicity-1.2.3.dev43/duplicity/backends/s3_boto3_backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/jottacloudbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/jottacloudbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/pyrax_identity/hubic.py` & `duplicity-1.2.3.dev43/duplicity/backends/pyrax_identity/hubic.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/pyrax_identity/__init__.py` & `duplicity-1.2.3.dev43/duplicity/backends/pyrax_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/imapbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/imapbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/_cf_cloudfiles.py` & `duplicity-1.2.3.dev43/duplicity/backends/_cf_cloudfiles.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/_cf_pyrax.py` & `duplicity-1.2.3.dev43/duplicity/backends/_cf_pyrax.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/_boto_single.py` & `duplicity-1.2.3.dev43/duplicity/backends/_boto_single.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/README` & `duplicity-1.2.3.dev43/duplicity/backends/README`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/sxbackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/sxbackend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backends/slatebackend.py` & `duplicity-1.2.3.dev43/duplicity/backends/slatebackend.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         response = requests.post(
             url=u'https://uploads.slate.host/api/public/' + self.slate_id,
             files=files,
             headers=headers)
         log.Debug(u"response handled")
 
         if not response.ok:
-            raise BackendException(u"An error occured whilst attempting to upload a file: %s" % (response))
+            raise BackendException(u"An error occurred whilst attempting to upload a file: %s" % (response))
         else:
             log.Debug(u"File successfully uploaded to slate with id:" + self.slate_id)
 
         if str(src).endswith(u"difftar.gpg"):
             os.remove(str(src))
 
     def _list(self):
```

### Comparing `duplicity-1.2.3.dev27/duplicity/dup_threading.py` & `duplicity-1.2.3.dev43/duplicity/dup_threading.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/dup_main.py` & `duplicity-1.2.3.dev43/duplicity/dup_main.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/backend.py` & `duplicity-1.2.3.dev43/duplicity/backend.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/config.py` & `duplicity-1.2.3.dev43/duplicity/config.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/globmatch.py` & `duplicity-1.2.3.dev43/duplicity/globmatch.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/__init__.py` & `duplicity-1.2.3.dev43/duplicity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 # You should have received a copy of the GNU General Public License
 # along with duplicity; if not, write to the Free Software Foundation,
 # Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307 USA
 
 import sys
 import gettext
 
-__version__ = u'1.2.3.dev27'
+__version__ = u'1.2.3.dev43'
 
 if sys.version_info.major >= 3:
     gettext.install(u'duplicity', names=[u'ngettext'])
 else:
     gettext.install(u'duplicity', names=[u'ngettext'], unicode=True)  # pylint: disable=unexpected-keyword-arg
```

### Comparing `duplicity-1.2.3.dev27/duplicity/librsync.py` & `duplicity-1.2.3.dev43/duplicity/librsync.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/errors.py` & `duplicity-1.2.3.dev43/duplicity/errors.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/tempdir.py` & `duplicity-1.2.3.dev43/duplicity/tempdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/tarfile.py` & `duplicity-1.2.3.dev43/duplicity/tarfile.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/progress.py` & `duplicity-1.2.3.dev43/duplicity/progress.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/gpg.py` & `duplicity-1.2.3.dev43/duplicity/gpg.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/filechunkio.py` & `duplicity-1.2.3.dev43/duplicity/filechunkio.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/patchdir.py` & `duplicity-1.2.3.dev43/duplicity/patchdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/manifest.py` & `duplicity-1.2.3.dev43/duplicity/manifest.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/file_naming.py` & `duplicity-1.2.3.dev43/duplicity/file_naming.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/_librsyncmodule.c` & `duplicity-1.2.3.dev43/duplicity/_librsyncmodule.c`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/dup_collections.py` & `duplicity-1.2.3.dev43/duplicity/dup_collections.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/robust.py` & `duplicity-1.2.3.dev43/duplicity/robust.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     #    TracebackArchive.add()
     except (IOError, EnvironmentError, librsync.librsyncError, path.PathException) as exc:
         if (not isinstance(exc, EnvironmentError) or
             hasattr(exc, u"errno") and
             errno.errorcode[exc.errno] in
             [u'EPERM', u'ENOENT', u'EACCES', u'EBUSY', u'EEXIST',
              u'ENOTDIR', u'ENAMETOOLONG', u'EINTR', u'ENOTEMPTY',
-             u'EIO', u'ETXTBSY', u'ESRCH', u'EINVAL']):
+             u'EIO', u'ETXTBSY', u'ESRCH', u'EINVAL', u'EOPNOTSUPP']):
             # Log.exception()
             if error_handler:
                 return error_handler(exc, *args)
         else:
             # Log.exception(1, 2)
             raise
```

### Comparing `duplicity-1.2.3.dev27/duplicity/commandline.py` & `duplicity-1.2.3.dev43/duplicity/commandline.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/diffdir.py` & `duplicity-1.2.3.dev43/duplicity/diffdir.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/cached_ops.py` & `duplicity-1.2.3.dev43/duplicity/cached_ops.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/util.py` & `duplicity-1.2.3.dev43/duplicity/util.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/dup_temp.py` & `duplicity-1.2.3.dev43/duplicity/dup_temp.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/asyncscheduler.py` & `duplicity-1.2.3.dev43/duplicity/asyncscheduler.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/statistics.py` & `duplicity-1.2.3.dev43/duplicity/statistics.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/lazy.py` & `duplicity-1.2.3.dev43/duplicity/lazy.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/path.py` & `duplicity-1.2.3.dev43/duplicity/path.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/selection.py` & `duplicity-1.2.3.dev43/duplicity/selection.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/log.py` & `duplicity-1.2.3.dev43/duplicity/log.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity/gpginterface.py` & `duplicity-1.2.3.dev43/duplicity/gpginterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 >>>
 >>> # ...and see it's the same as what we orignally encrypted
 >>> assert decrypted_plaintext == plaintext, \
           "GnuPG decrypted output does not match original input"
 >>>
 >>>
 >>> ##################################################
->>> # Now let's trying using run()'s attach_fhs paramter
+>>> # Now let's trying using run()'s attach_fhs parameter
 >>>
 >>> # we're assuming we're running on a unix...
 >>> infp = open('/etc/manpaths', 'rb')
 >>>
 >>> p1 = gnupg.run(['--symmetric'], create_fhs=['stdout'],
 ...                                 attach_fhs={'stdin': infp})
 >>>
```

### Comparing `duplicity-1.2.3.dev27/README-LOG.md` & `duplicity-1.2.3.dev43/README-LOG.md`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/PKG-INFO` & `duplicity-1.2.3.dev43/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplicity
-Version: 1.2.3.dev27
+Version: 1.2.3.dev43
 Summary: Encrypted backup using rsync algorithm
 Home-page: http://duplicity.us
 Author: Ben Escoto <ben@emrose.org>
 Author-email: ben@emrose.org
 Maintainer: Kenneth Loafman <kenneth@loafman.com>
 Maintainer-email: kenneth@loafman.com
 Platform: any
@@ -80,20 +80,22 @@
 if you're using python3
 
 # DEVELOPMENT
 
 For more information on downloading duplicity's source code from the
 code repository and developing for duplicity, see README-REPO.
 
+For source docs: http://duplicity.readthedocs.io/
+
 # HELP
 
 For more information see the duplicity web site at:
 
   http://duplicity.us
 
-  or
+  or at:
 
   http://duplicity.gitlab.io
 
 or post to the mailing list at
 
   https://lists.nongnu.org/mailman/listinfo/duplicity-talk
```

### Comparing `duplicity-1.2.3.dev27/COPYING` & `duplicity-1.2.3.dev43/COPYING`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/README-SNAP.md` & `duplicity-1.2.3.dev43/README-SNAP.md`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/fi_FI.po` & `duplicity-1.2.3.dev43/po/fi_FI.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_MD.po` & `duplicity-1.2.3.dev43/po/ru_MD.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_ES.po` & `duplicity-1.2.3.dev43/po/es_ES.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/pt_BR.po` & `duplicity-1.2.3.dev43/po/pt_BR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/uk_UA/duplicity.mo` & `duplicity-1.2.3.dev43/po/uk_UA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_GB.po` & `duplicity-1.2.3.dev43/po/en_GB.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_CN.po` & `duplicity-1.2.3.dev43/po/zh_CN.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/no_NO.po` & `duplicity-1.2.3.dev43/po/no_NO.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/nl_NL/duplicity.mo` & `duplicity-1.2.3.dev43/po/nl_NL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/it_IT.po` & `duplicity-1.2.3.dev43/po/it_IT.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/cs_CZ.po` & `duplicity-1.2.3.dev43/po/cs_CZ.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/hu_HU/duplicity.mo` & `duplicity-1.2.3.dev43/po/hu_HU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/de_DE.po` & `duplicity-1.2.3.dev43/po/de_DE.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_ES/duplicity.mo` & `duplicity-1.2.3.dev43/po/es_ES/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_HK/duplicity.mo` & `duplicity-1.2.3.dev43/po/zh_HK/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/da_DK.po` & `duplicity-1.2.3.dev43/po/da_DK.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/pl_PL.po` & `duplicity-1.2.3.dev43/po/pl_PL.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/nl_SR.po` & `duplicity-1.2.3.dev43/po/nl_SR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ca_ES.po` & `duplicity-1.2.3.dev43/po/ca_ES.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/nl_BE/duplicity.mo` & `duplicity-1.2.3.dev43/po/nl_BE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/el_GR.po` & `duplicity-1.2.3.dev43/po/el_GR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/it_IT/duplicity.mo` & `duplicity-1.2.3.dev43/po/it_IT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_HK.po` & `duplicity-1.2.3.dev43/po/zh_HK.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_UA/duplicity.mo` & `duplicity-1.2.3.dev43/po/ru_UA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_EM/duplicity.mo` & `duplicity-1.2.3.dev43/po/es_EM/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ja_JP.po` & `duplicity-1.2.3.dev43/po/ja_JP.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/pt_PT/duplicity.mo` & `duplicity-1.2.3.dev43/po/pt_PT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_TW/duplicity.mo` & `duplicity-1.2.3.dev43/po/zh_TW/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/de_AT.po` & `duplicity-1.2.3.dev43/po/de_AT.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_GB/duplicity.mo` & `duplicity-1.2.3.dev43/po/en_GB/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/cs_CZ/duplicity.mo` & `duplicity-1.2.3.dev43/po/cs_CZ/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/pl_PL/duplicity.mo` & `duplicity-1.2.3.dev43/po/pl_PL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_US.po` & `duplicity-1.2.3.dev43/po/en_US.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: duplicity\n"
 "Report-Msgid-Bugs-To: Kenneth Loafman <kenneth@loafman.com>\n"
 "POT-Creation-Date: 2023-01-25 13:29-0600\n"
-"PO-Revision-Date: 2023-01-25 19:48\n"
+"PO-Revision-Date: 2023-03-20 15:04\n"
 "Last-Translator: \n"
 "Language-Team: English, United States\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
```

### Comparing `duplicity-1.2.3.dev27/po/es_US/duplicity.mo` & `duplicity-1.2.3.dev43/po/es_US/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/he_IL/duplicity.mo` & `duplicity-1.2.3.dev43/po/he_IL/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/nl_NL.po` & `duplicity-1.2.3.dev43/po/nl_NL.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_BY/duplicity.mo` & `duplicity-1.2.3.dev43/po/ru_BY/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_US/duplicity.mo` & `duplicity-1.2.3.dev43/po/en_US/duplicity.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: duplicity*

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 00000030: 0000 0000 0000 0000 0050 726f 6a65 6374  .........Project
 00000040: 2d49 642d 5665 7273 696f 6e3a 2064 7570  -Id-Version: dup
 00000050: 6c69 6369 7479 0a52 6570 6f72 742d 4d73  licity.Report-Ms
 00000060: 6769 642d 4275 6773 2d54 6f3a 204b 656e  gid-Bugs-To: Ken
 00000070: 6e65 7468 204c 6f61 666d 616e 203c 6b65  neth Loafman <ke
 00000080: 6e6e 6574 6840 6c6f 6166 6d61 6e2e 636f  nneth@loafman.co
 00000090: 6d3e 0a50 4f2d 5265 7669 7369 6f6e 2d44  m>.PO-Revision-D
-000000a0: 6174 653a 2032 3032 332d 3031 2d32 3520  ate: 2023-01-25 
-000000b0: 3139 3a34 380a 4c61 7374 2d54 7261 6e73  19:48.Last-Trans
+000000a0: 6174 653a 2032 3032 332d 3033 2d32 3020  ate: 2023-03-20 
+000000b0: 3135 3a30 340a 4c61 7374 2d54 7261 6e73  15:04.Last-Trans
 000000c0: 6c61 746f 723a 200a 4c61 6e67 7561 6765  lator: .Language
 000000d0: 2d54 6561 6d3a 2045 6e67 6c69 7368 2c20  -Team: English, 
 000000e0: 556e 6974 6564 2053 7461 7465 730a 4c61  United States.La
 000000f0: 6e67 7561 6765 3a20 656e 5f55 530a 4d49  nguage: en_US.MI
 00000100: 4d45 2d56 6572 7369 6f6e 3a20 312e 300a  ME-Version: 1.0.
 00000110: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 00000120: 7874 2f70 6c61 696e 3b20 6368 6172 7365  xt/plain; charse
```

### Comparing `duplicity-1.2.3.dev27/po/ar_SA/duplicity.mo` & `duplicity-1.2.3.dev43/po/ar_SA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/pt_BR/duplicity.mo` & `duplicity-1.2.3.dev43/po/pt_BR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/tr_TR/duplicity.mo` & `duplicity-1.2.3.dev43/po/tr_TR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/af_ZA/duplicity.mo` & `duplicity-1.2.3.dev43/po/af_ZA/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/POTFILES.skip` & `duplicity-1.2.3.dev43/po/POTFILES.skip`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/nl_SR/duplicity.mo` & `duplicity-1.2.3.dev43/po/nl_SR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_RU/duplicity.mo` & `duplicity-1.2.3.dev43/po/ru_RU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_BY.po` & `duplicity-1.2.3.dev43/po/ru_BY.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ca_ES/duplicity.mo` & `duplicity-1.2.3.dev43/po/ca_ES/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/sr_SP.po` & `duplicity-1.2.3.dev43/po/sr_SP.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_TW.po` & `duplicity-1.2.3.dev43/po/zh_TW.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_UA.po` & `duplicity-1.2.3.dev43/po/ru_UA.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ko_KR/duplicity.mo` & `duplicity-1.2.3.dev43/po/ko_KR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_AU.po` & `duplicity-1.2.3.dev43/po/en_AU.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/fi_FI/duplicity.mo` & `duplicity-1.2.3.dev43/po/fi_FI/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/uk_UA.po` & `duplicity-1.2.3.dev43/po/uk_UA.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/POTFILES.in` & `duplicity-1.2.3.dev43/po/POTFILES.in`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/sr_SP/duplicity.mo` & `duplicity-1.2.3.dev43/po/sr_SP/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/de_DE/duplicity.mo` & `duplicity-1.2.3.dev43/po/de_DE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/de_AT/duplicity.mo` & `duplicity-1.2.3.dev43/po/de_AT/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_RU.po` & `duplicity-1.2.3.dev43/po/ru_RU.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/sv_SE/duplicity.mo` & `duplicity-1.2.3.dev43/po/sv_SE/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/fr_FR.po` & `duplicity-1.2.3.dev43/po/fr_FR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/pt_PT.po` & `duplicity-1.2.3.dev43/po/pt_PT.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ro_RO/duplicity.mo` & `duplicity-1.2.3.dev43/po/ro_RO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ar_SA.po` & `duplicity-1.2.3.dev43/po/ar_SA.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/el_GR/duplicity.mo` & `duplicity-1.2.3.dev43/po/el_GR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/he_IL.po` & `duplicity-1.2.3.dev43/po/he_IL.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/hu_HU.po` & `duplicity-1.2.3.dev43/po/hu_HU.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/nl_BE.po` & `duplicity-1.2.3.dev43/po/nl_BE.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_AU/duplicity.mo` & `duplicity-1.2.3.dev43/po/en_AU/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_MO.po` & `duplicity-1.2.3.dev43/po/zh_MO.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/tr_TR.po` & `duplicity-1.2.3.dev43/po/tr_TR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/da_DK/duplicity.mo` & `duplicity-1.2.3.dev43/po/da_DK/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_MO/duplicity.mo` & `duplicity-1.2.3.dev43/po/zh_MO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_PR/duplicity.mo` & `duplicity-1.2.3.dev43/po/es_PR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_SG/duplicity.mo` & `duplicity-1.2.3.dev43/po/zh_SG/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_US.po` & `duplicity-1.2.3.dev43/po/es_US.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_MX/duplicity.mo` & `duplicity-1.2.3.dev43/po/es_MX/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ru_MD/duplicity.mo` & `duplicity-1.2.3.dev43/po/ru_MD/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_SG.po` & `duplicity-1.2.3.dev43/po/zh_SG.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_MX.po` & `duplicity-1.2.3.dev43/po/es_MX.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/zh_CN/duplicity.mo` & `duplicity-1.2.3.dev43/po/zh_CN/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_PR.po` & `duplicity-1.2.3.dev43/po/en_PR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/vi_VN.po` & `duplicity-1.2.3.dev43/po/vi_VN.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/sv_SE.po` & `duplicity-1.2.3.dev43/po/sv_SE.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_EM.po` & `duplicity-1.2.3.dev43/po/es_EM.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/af_ZA.po` & `duplicity-1.2.3.dev43/po/af_ZA.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/no_NO/duplicity.mo` & `duplicity-1.2.3.dev43/po/no_NO/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/es_PR.po` & `duplicity-1.2.3.dev43/po/es_PR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/Makevars` & `duplicity-1.2.3.dev43/po/Makevars`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ko_KR.po` & `duplicity-1.2.3.dev43/po/ko_KR.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/en_PR/duplicity.mo` & `duplicity-1.2.3.dev43/po/en_PR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/duplicity.pot` & `duplicity-1.2.3.dev43/po/duplicity.pot`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/ro_RO.po` & `duplicity-1.2.3.dev43/po/ro_RO.po`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/po/fr_FR/duplicity.mo` & `duplicity-1.2.3.dev43/po/fr_FR/duplicity.mo`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/duplicity.egg-info/PKG-INFO` & `duplicity-1.2.3.dev43/duplicity.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplicity
-Version: 1.2.3.dev27
+Version: 1.2.3.dev43
 Summary: Encrypted backup using rsync algorithm
 Home-page: http://duplicity.us
 Author: Ben Escoto <ben@emrose.org>
 Author-email: ben@emrose.org
 Maintainer: Kenneth Loafman <kenneth@loafman.com>
 Maintainer-email: kenneth@loafman.com
 Platform: any
@@ -80,20 +80,22 @@
 if you're using python3
 
 # DEVELOPMENT
 
 For more information on downloading duplicity's source code from the
 code repository and developing for duplicity, see README-REPO.
 
+For source docs: http://duplicity.readthedocs.io/
+
 # HELP
 
 For more information see the duplicity web site at:
 
   http://duplicity.us
 
-  or
+  or at:
 
   http://duplicity.gitlab.io
 
 or post to the mailing list at
 
   https://lists.nongnu.org/mailman/listinfo/duplicity-talk
```

### Comparing `duplicity-1.2.3.dev27/duplicity.egg-info/SOURCES.txt` & `duplicity-1.2.3.dev43/duplicity.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 bin/rdiffdir.1
 debian/changelog
 debian/compat
 debian/control
 debian/copyright
 debian/rules
 debian/source/format
-docs/Makefile
+docs/README.md
 docs/conf.py
 docs/index.rst
-docs/make.bat
 docs/modules.rst
 duplicity/__init__.py
 duplicity/_librsyncmodule.c
 duplicity/asyncscheduler.py
 duplicity/backend.py
 duplicity/cached_ops.py
 duplicity/commandline.py
@@ -108,14 +107,15 @@
 duplicity/backends/slatebackend.py
 duplicity/backends/ssh_paramiko_backend.py
 duplicity/backends/ssh_pexpect_backend.py
 duplicity/backends/swiftbackend.py
 duplicity/backends/sxbackend.py
 duplicity/backends/tahoebackend.py
 duplicity/backends/webdavbackend.py
+duplicity/backends/xorrisobackend.py
 duplicity/backends/pyrax_identity/__init__.py
 duplicity/backends/pyrax_identity/hubic.py
 po/LINGUAS
 po/Makevars
 po/POTFILES.in
 po/POTFILES.skip
 po/af_ZA.po
```

### Comparing `duplicity-1.2.3.dev27/setup.py` & `duplicity-1.2.3.dev43/setup.py`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/README.md` & `duplicity-1.2.3.dev43/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,20 +49,22 @@
 if you're using python3
 
 # DEVELOPMENT
 
 For more information on downloading duplicity's source code from the
 code repository and developing for duplicity, see README-REPO.
 
+For source docs: http://duplicity.readthedocs.io/
+
 # HELP
 
 For more information see the duplicity web site at:
 
   http://duplicity.us
 
-  or
+  or at:
 
   http://duplicity.gitlab.io
 
 or post to the mailing list at
 
   https://lists.nongnu.org/mailman/listinfo/duplicity-talk
```

### Comparing `duplicity-1.2.3.dev27/README-REPO.md` & `duplicity-1.2.3.dev43/README-REPO.md`

 * *Files identical despite different names*

### Comparing `duplicity-1.2.3.dev27/README-TESTING.md` & `duplicity-1.2.3.dev43/README-TESTING.md`

 * *Files identical despite different names*

