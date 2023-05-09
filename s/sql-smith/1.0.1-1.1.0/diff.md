# Comparing `tmp/sql-smith-1.0.1.tar.gz` & `tmp/sql_smith-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql-smith-1.0.1.tar", last modified: Tue Dec 20 21:04:16 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

