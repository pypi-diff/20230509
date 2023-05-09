# Comparing `tmp/hexwatershed-0.1.9.tar.gz` & `tmp/hexwatershed-0.2.4-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexwatershed-0.1.9.tar", last modified: Tue May  3 16:34:06 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

