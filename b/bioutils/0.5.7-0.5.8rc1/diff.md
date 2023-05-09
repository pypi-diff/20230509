# Comparing `tmp/bioutils-0.5.7.tar.gz` & `tmp/bioutils-0.5.8rc1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioutils-0.5.7.tar", last modified: Fri Jul  8 14:32:40 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

