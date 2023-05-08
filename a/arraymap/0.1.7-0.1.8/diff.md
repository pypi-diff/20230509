# Comparing `tmp/arraymap-0.1.7.tar.gz` & `tmp/arraymap-0.1.8-cp37-cp37m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraymap-0.1.7.tar", last modified: Wed May  3 17:15:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

