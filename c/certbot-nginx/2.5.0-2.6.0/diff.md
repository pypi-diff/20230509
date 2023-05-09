# Comparing `tmp/certbot-nginx-2.5.0.tar.gz` & `tmp/certbot_nginx-2.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/certbot-nginx-2.5.0.tar", last modified: Tue Apr  4 15:07:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

