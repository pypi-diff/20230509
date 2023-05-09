# Comparing `tmp/pystacker-1.2.8.tar.gz` & `tmp/pystacker-1.2.9-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystacker-1.2.8.tar", last modified: Wed May  3 15:23:54 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

