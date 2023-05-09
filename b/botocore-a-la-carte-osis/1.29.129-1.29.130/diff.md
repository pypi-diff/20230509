# Comparing `tmp/botocore-a-la-carte-osis-1.29.129.tar.gz` & `tmp/botocore_a_la_carte_osis-1.29.130-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.129.tar", last modified: Sat May  6 01:11:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

