# Comparing `tmp/mse_cli-0.12.0.tar.gz` & `tmp/mse_cli-0.9.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli-0.12.0.tar", last modified: Tue May  9 09:14:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

