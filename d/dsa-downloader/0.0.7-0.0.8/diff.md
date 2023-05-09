# Comparing `tmp/dsa-downloader-0.0.7.tar.gz` & `tmp/dsa_downloader-0.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dsa-downloader-0.0.7.tar", last modified: Wed Sep 14 12:15:45 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

