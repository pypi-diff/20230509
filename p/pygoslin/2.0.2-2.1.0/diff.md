# Comparing `tmp/pygoslin-2.0.2.tar.gz` & `tmp/pygoslin-2.1.0-py3.8.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygoslin-2.0.2.tar", last modified: Thu Jun 23 12:07:09 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

