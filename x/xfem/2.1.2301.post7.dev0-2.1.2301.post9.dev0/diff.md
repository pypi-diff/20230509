# Comparing `tmp/xfem-2.1.2301.post7.dev0.tar.gz` & `tmp/xfem-2.1.2301.post9.dev0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfem-2.1.2301.post7.dev0.tar", last modified: Tue May  9 12:58:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

