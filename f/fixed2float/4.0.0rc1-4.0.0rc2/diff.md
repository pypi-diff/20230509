# Comparing `tmp/fixed2float-4.0.0_rc1.tar.gz` & `tmp/fixed2float-4.0.0_rc2-cp37-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

