# Comparing `tmp/r2diaphora-0.2.3.tar.gz` & `tmp/r2diaphora-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2diaphora-0.2.3.tar", last modified: Thu Apr 20 08:23:23 2023, max compression
+gzip compressed data, was "r2diaphora-0.2.4.tar", last modified: Tue May  9 10:57:25 2023, max compression
```

## Comparing `r2diaphora-0.2.3.tar` & `r2diaphora-0.2.4.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.644130 r2diaphora-0.2.3/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/LICENSE
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/MANIFEST.in
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-04-20 08:23:23.644130 r2diaphora-0.2.3/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/README.md
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.620134 r2diaphora-0.2.3/r2diaphora/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/__init__.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94431 2023-04-19 14:00:56.000000 r2diaphora-0.2.3/r2diaphora/diaphora.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/diaphora_heuristics.py
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)    41453 2023-04-19 15:08:18.000000 r2diaphora-0.2.3/r2diaphora/diaphora_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/difflibparser.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/html_diff.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.620134 r2diaphora-0.2.3/r2diaphora/idaapi/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/idaapi/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    22772 2023-03-23 12:48:30.000000 r2diaphora-0.2.3/r2diaphora/idaapi/idaapi_to_r2.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/idaapi/instructions.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.620134 r2diaphora-0.2.3/r2diaphora/jkutils/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/jkutils/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/jkutils/factor.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-03-22 16:06:47.000000 r2diaphora-0.2.3/r2diaphora/jkutils/graph_hashes.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/jkutils/kfuzzy.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.620134 r2diaphora-0.2.3/r2diaphora/others/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/others/__init__.py
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/others/tarjan_sort.py
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.616135 r2diaphora-0.2.3/r2diaphora/pycparser/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/X11/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      311 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     1111 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/_ansi.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     5734 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     5040 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/_syslist.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/aio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/alloca.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/ar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/argz.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/arpa/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/asm-generic/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/assert.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/complex.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/cpio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/ctype.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/dirent.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/dlfcn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/emmintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/endian.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/envz.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/errno.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/fastmath.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/fcntl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/features.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/fenv.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/float.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/fnmatch.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/ftw.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/getopt.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/glob.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/grp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/iconv.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/ieeefp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/immintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/inttypes.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/iso646.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/langinfo.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/libgen.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/libintl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/limits.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/linux/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/linux/socket.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/linux/version.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/locale.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/malloc.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/math.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/monetary.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/mqueue.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/ndbm.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/net/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/net/if.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/netdb.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/netinet/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/netinet/in.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/newlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/nl_types.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.636131 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/openssl/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/openssl/err.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/paths.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/poll.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/process.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/pthread.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/pwd.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/reent.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/regdef.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/regex.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sched.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/search.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/semaphore.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/setjmp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/signal.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/smmintrin.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/spawn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdarg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdatomic.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdbool.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stddef.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdint.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdlib.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/string.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/strings.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/stropts.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.640130 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/mman.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/msg.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/poll.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/resource.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/select.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/sem.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/shm.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/socket.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/stat.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/time.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/times.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/types.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/uio.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/un.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/sys/wait.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/syslog.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/tar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/termios.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/tgmath.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/threads.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/time.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/trace.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/ulimit.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/unctrl.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/unistd.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/utime.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/utmp.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/utmpx.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/wchar.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/wctype.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/wordexp.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.640130 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/xcb/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      514 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/zlib.h
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.616135 r2diaphora-0.2.3/r2diaphora/signatures/
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.644130 r2diaphora-0.2.3/r2diaphora/signatures/flirt/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    32585 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_arm.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    44648 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_mips.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    42356 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_ppc.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    32757 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_sh4.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    31653 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_x86-64.sig
--rw-rw-r--   0 fdd       (1000) fdd       (1000)    53445 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_x86.sig
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.620134 r2diaphora-0.2.3/r2diaphora.egg-info/
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-04-20 08:23:23.000000 r2diaphora-0.2.3/r2diaphora.egg-info/PKG-INFO
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     7329 2023-04-20 08:23:23.000000 r2diaphora-0.2.3/r2diaphora.egg-info/SOURCES.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-04-20 08:23:23.000000 r2diaphora-0.2.3/r2diaphora.egg-info/dependency_links.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       59 2023-04-20 08:23:23.000000 r2diaphora-0.2.3/r2diaphora.egg-info/entry_points.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)      128 2023-04-20 08:23:23.000000 r2diaphora-0.2.3/r2diaphora.egg-info/requires.txt
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-04-20 08:23:23.000000 r2diaphora-0.2.3/r2diaphora.egg-info/top_level.txt
-drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-04-20 08:23:23.644130 r2diaphora-0.2.3/scripts/
--rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/scripts/r2diaphora-bulk
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-01-25 09:51:26.000000 r2diaphora-0.2.3/scripts/r2diaphora-db
--rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-04-20 08:23:23.644130 r2diaphora-0.2.3/setup.cfg
--rw-rw-r--   0 fdd       (1000) fdd       (1000)     2069 2023-04-19 15:10:07.000000 r2diaphora-0.2.3/setup.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.287975 r2diaphora-0.2.4/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    34523 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/LICENSE
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       82 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/MANIFEST.in
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-09 10:57:25.287975 r2diaphora-0.2.4/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2425 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/README.md
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.263983 r2diaphora-0.2.4/r2diaphora/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      404 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/__init__.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    94431 2023-04-19 14:00:56.000000 r2diaphora-0.2.4/r2diaphora/diaphora.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    57599 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/diaphora_heuristics.py
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)    41632 2023-05-09 10:51:41.000000 r2diaphora-0.2.4/r2diaphora/diaphora_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     4604 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/difflibparser.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    13283 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/html_diff.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.263983 r2diaphora-0.2.4/r2diaphora/idaapi/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/idaapi/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    22800 2023-05-09 09:05:20.000000 r2diaphora-0.2.4/r2diaphora/idaapi/idaapi_to_r2.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    77880 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/idaapi/instructions.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.267982 r2diaphora-0.2.4/r2diaphora/jkutils/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/jkutils/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6336 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/jkutils/factor.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     6037 2023-03-22 16:06:47.000000 r2diaphora-0.2.4/r2diaphora/jkutils/graph_hashes.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    10023 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/jkutils/kfuzzy.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.267982 r2diaphora-0.2.4/r2diaphora/others/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        0 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/others/__init__.py
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2807 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/others/tarjan_sort.py
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.255986 r2diaphora-0.2.4/r2diaphora/pycparser/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/X11/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/X11/Intrinsic.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      118 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/X11/Xlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      311 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_defines.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     1111 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/_ansi.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     5734 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/_fake_defines.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     5040 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/_syslist.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/aio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/alloca.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/ar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/argz.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/arpa/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/arpa/inet.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/asm-generic/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/asm-generic/int-ll64.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/assert.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/complex.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/cpio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/ctype.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/dirent.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/dlfcn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/emmintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/endian.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/envz.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/errno.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/fastmath.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/fcntl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/features.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/fenv.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/float.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/fmtmsg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/fnmatch.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/ftw.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/getopt.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/glob.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/grp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/iconv.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/ieeefp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/immintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/inttypes.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/iso646.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/langinfo.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/libgen.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/libintl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/limits.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/linux/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/linux/socket.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/linux/version.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/locale.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/malloc.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/math.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/mir_toolkit/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/mir_toolkit/client_types.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/monetary.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/mqueue.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/ndbm.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.279978 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/net/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/net/if.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/netdb.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.283976 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/netinet/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/netinet/in.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/netinet/tcp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/newlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/nl_types.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.283976 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/openssl/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/openssl/err.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/openssl/evp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/openssl/hmac.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/openssl/ssl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/openssl/x509v3.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/paths.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/poll.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/process.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/pthread.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/pwd.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/reent.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/regdef.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/regex.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sched.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/search.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/semaphore.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/setjmp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/signal.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/smmintrin.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/spawn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdarg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdatomic.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdbool.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stddef.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdint.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdlib.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stdnoreturn.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/string.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/strings.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/stropts.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.283976 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/ioctl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/ipc.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/mman.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/msg.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/poll.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/resource.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/select.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/sem.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/shm.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/socket.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/stat.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/statvfs.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/sysctl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/time.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/times.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/types.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/uio.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/un.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/utsname.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/sys/wait.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/syslog.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/tar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/termios.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/tgmath.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/threads.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/time.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/trace.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/ulimit.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/unctrl.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/unistd.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/utime.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/utmp.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/utmpx.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/wchar.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/wctype.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/wordexp.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.287975 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/xcb/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       55 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/xcb/xcb.h
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      514 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/zlib.h
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.259984 r2diaphora-0.2.4/r2diaphora/signatures/
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.287975 r2diaphora-0.2.4/r2diaphora/signatures/flirt/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    32585 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_arm.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    44648 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_mips.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    42356 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_ppc.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    32757 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_sh4.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    31653 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_x86-64.sig
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)    53445 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_x86.sig
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.263983 r2diaphora-0.2.4/r2diaphora.egg-info/
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      455 2023-05-09 10:57:25.000000 r2diaphora-0.2.4/r2diaphora.egg-info/PKG-INFO
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     7329 2023-05-09 10:57:25.000000 r2diaphora-0.2.4/r2diaphora.egg-info/SOURCES.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)        1 2023-05-09 10:57:25.000000 r2diaphora-0.2.4/r2diaphora.egg-info/dependency_links.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       59 2023-05-09 10:57:25.000000 r2diaphora-0.2.4/r2diaphora.egg-info/entry_points.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)      128 2023-05-09 10:57:25.000000 r2diaphora-0.2.4/r2diaphora.egg-info/requires.txt
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       11 2023-05-09 10:57:25.000000 r2diaphora-0.2.4/r2diaphora.egg-info/top_level.txt
+drwxrwxr-x   0 fdd       (1000) fdd       (1000)        0 2023-05-09 10:57:25.287975 r2diaphora-0.2.4/scripts/
+-rwxrwxr-x   0 fdd       (1000) fdd       (1000)      802 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/scripts/r2diaphora-bulk
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2231 2023-01-25 09:51:26.000000 r2diaphora-0.2.4/scripts/r2diaphora-db
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)       79 2023-05-09 10:57:25.287975 r2diaphora-0.2.4/setup.cfg
+-rw-rw-r--   0 fdd       (1000) fdd       (1000)     2069 2023-05-09 10:52:51.000000 r2diaphora-0.2.4/setup.py
```

### Comparing `r2diaphora-0.2.3/LICENSE` & `r2diaphora-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/README.md` & `r2diaphora-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/diaphora.py` & `r2diaphora-0.2.4/r2diaphora/diaphora.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/diaphora_heuristics.py` & `r2diaphora-0.2.4/r2diaphora/diaphora_heuristics.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/diaphora_r2.py` & `r2diaphora-0.2.4/r2diaphora/diaphora_r2.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,18 @@
         ret = None
 
         try:
             ret = self.read_function(f)
         except TimeoutError:
             log.warning("Timeout while reading function at 0x%s", f)
         except Exception:
-            log.exception("Exception while trying to read %s", f)
+            log.exception(
+                "Exception while trying to read function at 0x%x in sample %s",
+                f, log_exec_r2_cmdj("ij").get("core", {}).get("file", "PATH ERROR")
+            )
         finally:
             # Unregister the signal so it won't be triggered
             # if the timeout is not reached.
             signal.signal(signal.SIGALRM, signal.SIG_IGN)
         return ret
 
     # Most important function
@@ -661,15 +664,16 @@
         try:
             keys.remove(f - image_base)
         except Exception:
             pass
         keys.insert(0, f - image_base)
         for key in keys:
             try:
-                asm.extend(assembly[key])
+                if key in assembly:
+                    asm.extend(assembly[key])
             except Exception:
                 log.exception("Failed to build assembly corpus for function %s", f)
 
         return "\n".join(asm)
 
     def get_switches_info_for_fn(self, function_ea):
         switches = []
```

### Comparing `r2diaphora-0.2.3/r2diaphora/difflibparser.py` & `r2diaphora-0.2.4/r2diaphora/difflibparser.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/html_diff.py` & `r2diaphora-0.2.4/r2diaphora/html_diff.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/idaapi/idaapi_to_r2.py` & `r2diaphora-0.2.4/r2diaphora/idaapi/idaapi_to_r2.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,14 +642,15 @@
         res[flag["offset"]] = flag["name"]
     return res
 
 #-----------------------------------------------------------------------
 def r2_open(input_path, ident_libs = False):
     global r2
     r2 = r2pipe.open(f"ccall://{input_path}", flags=["-2", "-q"])
+    r2.cmd("e log.level=0")
     r2.use_cache = True
     r2.cmd("aaaa")
     #r2.cmd("aac")
 
     # perform analysis
     r2.cmd("e asm.flags=false")
     r2.cmd("e asm.bytes=false")
```

### Comparing `r2diaphora-0.2.3/r2diaphora/idaapi/instructions.py` & `r2diaphora-0.2.4/r2diaphora/idaapi/instructions.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/jkutils/factor.py` & `r2diaphora-0.2.4/r2diaphora/jkutils/factor.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/jkutils/graph_hashes.py` & `r2diaphora-0.2.4/r2diaphora/jkutils/graph_hashes.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/jkutils/kfuzzy.py` & `r2diaphora-0.2.4/r2diaphora/jkutils/kfuzzy.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/others/tarjan_sort.py` & `r2diaphora-0.2.4/r2diaphora/others/tarjan_sort.py`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h` & `r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/X11/_X11_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/_fake_defines.h` & `r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/_fake_defines.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h` & `r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/pycparser/fake_libc_include/zlib.h` & `r2diaphora-0.2.4/r2diaphora/pycparser/fake_libc_include/zlib.h`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_arm.sig` & `r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_arm.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_mips.sig` & `r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_mips.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_ppc.sig` & `r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_ppc.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_sh4.sig` & `r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_sh4.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_x86-64.sig` & `r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_x86-64.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora/signatures/flirt/uclibc_x86.sig` & `r2diaphora-0.2.4/r2diaphora/signatures/flirt/uclibc_x86.sig`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/r2diaphora.egg-info/SOURCES.txt` & `r2diaphora-0.2.4/r2diaphora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/scripts/r2diaphora-bulk` & `r2diaphora-0.2.4/scripts/r2diaphora-bulk`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/scripts/r2diaphora-db` & `r2diaphora-0.2.4/scripts/r2diaphora-db`

 * *Files identical despite different names*

### Comparing `r2diaphora-0.2.3/setup.py` & `r2diaphora-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             shutil.copy2(
                 f,
                 os.path.join(os.path.expanduser("~"), ".r2diaphora", "signatures", "flirt")
             )
 
 setup(
     name="r2diaphora",
-    version="0.2.3",
+    version="0.2.4",
     description="radare2 port of diaphora",
     url="https://github.com/FernandoDoming/r2diaphora",
     author="Fernando Domínguez",
     author_email="fernando.dom.del@gmail.com",
     license="GNU GPL v3",
     packages=[
         "r2diaphora",
```

