# Comparing `tmp/loristrck-1.5.2.tar.gz` & `tmp/loristrck-1.5.4-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loristrck-1.5.2.tar", last modified: Thu Mar  9 18:58:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

