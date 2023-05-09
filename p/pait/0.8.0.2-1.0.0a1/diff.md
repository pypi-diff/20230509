# Comparing `tmp/pait-0.8.0.2.tar.gz` & `tmp/pait-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pait-0.8.0.2.tar", max compression
+gzip compressed data, was "pait-1.0.0a1.tar", max compression
```

## Comparing `pait-0.8.0.2.tar` & `pait-1.0.0a1.tar`

### file list

```diff
@@ -1,119 +1,184 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.800410 pait-0.8.0.2/LICENSE
--rw-r--r--   0        0        0     2878 2022-09-03 13:07:44.164092 pait-0.8.0.2/README.md
--rw-r--r--   0        0        0       24 2022-06-17 09:35:54.073471 pait-0.8.0.2/pait/__init__.py
--rw-r--r--   0        0        0        0 2022-01-21 03:47:13.390885 pait-0.8.0.2/pait/api_doc/__init__.py
--rw-r--r--   0        0        0       61 2021-12-05 05:37:12.197993 pait-0.8.0.2/pait/api_doc/__main__.py
--rw-r--r--   0        0        0    16007 2022-05-18 12:23:14.673480 pait-0.8.0.2/pait/api_doc/base_parse.py
--rw-r--r--   0        0        0     2261 2022-03-28 14:19:11.993656 pait-0.8.0.2/pait/api_doc/cli.py
--rw-r--r--   0        0        0      171 2022-10-25 03:45:47.819366 pait-0.8.0.2/pait/api_doc/html/__init__.py
--rw-r--r--   0        0        0     1042 2022-10-25 03:45:48.663393 pait-0.8.0.2/pait/api_doc/html/elements.py
--rw-r--r--   0        0        0     1196 2022-10-25 03:54:12.168725 pait-0.8.0.2/pait/api_doc/html/rapidoc.py
--rw-r--r--   0        0        0     1021 2022-06-18 16:09:46.202387 pait-0.8.0.2/pait/api_doc/html/redoc.py
--rw-r--r--   0        0        0     1285 2022-06-18 16:09:46.214388 pait-0.8.0.2/pait/api_doc/html/swagger.py
--rw-r--r--   0        0        0     9189 2022-04-25 15:44:24.324298 pait-0.8.0.2/pait/api_doc/markdown.py
--rw-r--r--   0        0        0    20476 2022-10-25 06:53:20.848145 pait-0.8.0.2/pait/api_doc/open_api.py
--rw-r--r--   0        0        0     5573 2022-05-10 14:30:28.760700 pait-0.8.0.2/pait/app/__init__.py
--rw-r--r--   0        0        0      562 2021-12-05 05:37:12.193994 pait-0.8.0.2/pait/app/auto_load_app.py
--rw-r--r--   0        0        0       97 2022-09-26 15:00:24.161625 pait-0.8.0.2/pait/app/base/__init__.py
--rw-r--r--   0        0        0     3725 2022-09-27 05:42:31.421889 pait-0.8.0.2/pait/app/base/app_helper.py
--rw-r--r--   0        0        0     9907 2022-10-25 08:14:43.243841 pait-0.8.0.2/pait/app/base/doc_route.py
--rw-r--r--   0        0        0    10862 2022-08-23 17:28:06.451157 pait-0.8.0.2/pait/app/base/grpc_route.py
--rw-r--r--   0        0        0    13014 2022-06-24 06:24:28.733022 pait-0.8.0.2/pait/app/base/test_helper.py
--rw-r--r--   0        0        0      610 2022-05-22 10:37:51.559801 pait-0.8.0.2/pait/app/base/util.py
--rw-r--r--   0        0        0      202 2022-05-22 09:15:45.861444 pait-0.8.0.2/pait/app/flask/__init__.py
--rw-r--r--   0        0        0     2061 2022-09-27 02:53:58.432686 pait-0.8.0.2/pait/app/flask/_app_helper.py
--rw-r--r--   0        0        0     1516 2022-10-25 07:47:00.286517 pait-0.8.0.2/pait/app/flask/_doc_route.py
--rw-r--r--   0        0        0     3706 2022-05-01 06:16:19.719474 pait-0.8.0.2/pait/app/flask/_load_app.py
--rw-r--r--   0        0        0      269 2022-01-10 09:58:31.982457 pait-0.8.0.2/pait/app/flask/_pait.py
--rw-r--r--   0        0        0     1905 2022-02-11 01:59:50.264282 pait-0.8.0.2/pait/app/flask/_test_helper.py
--rw-r--r--   0        0        0     1150 2022-08-23 17:28:05.371403 pait-0.8.0.2/pait/app/flask/grpc_route.py
--rw-r--r--   0        0        0      322 2022-03-28 14:19:11.993656 pait-0.8.0.2/pait/app/flask/plugin/__init__.py
--rw-r--r--   0        0        0      117 2022-01-15 15:01:59.773113 pait-0.8.0.2/pait/app/flask/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0       94 2022-04-26 15:15:35.767434 pait-0.8.0.2/pait/app/flask/plugin/cache_resonse.py
--rw-r--r--   0        0        0       95 2022-01-10 09:58:31.982457 pait-0.8.0.2/pait/app/flask/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1576 2022-01-18 08:49:09.550123 pait-0.8.0.2/pait/app/flask/plugin/mock_response.py
--rw-r--r--   0        0        0      202 2022-05-22 09:15:45.881445 pait-0.8.0.2/pait/app/sanic/__init__.py
--rw-r--r--   0        0        0     2232 2022-09-27 02:52:23.831830 pait-0.8.0.2/pait/app/sanic/_app_helper.py
--rw-r--r--   0        0        0     1607 2022-10-25 07:47:00.298517 pait-0.8.0.2/pait/app/sanic/_doc_route.py
--rw-r--r--   0        0        0     3950 2022-05-01 06:16:19.719474 pait-0.8.0.2/pait/app/sanic/_load_app.py
--rw-r--r--   0        0        0      374 2022-01-10 09:58:31.982457 pait-0.8.0.2/pait/app/sanic/_pait.py
--rw-r--r--   0        0        0     2177 2022-02-11 01:59:50.264282 pait-0.8.0.2/pait/app/sanic/_test_helper.py
--rw-r--r--   0        0        0     1128 2022-08-23 17:28:05.343410 pait-0.8.0.2/pait/app/sanic/grpc_route.py
--rw-r--r--   0        0        0      362 2022-03-28 14:19:11.993656 pait-0.8.0.2/pait/app/sanic/plugin/__init__.py
--rw-r--r--   0        0        0      601 2022-05-20 05:50:27.380488 pait-0.8.0.2/pait/app/sanic/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     1239 2022-05-20 06:05:34.037378 pait-0.8.0.2/pait/app/sanic/plugin/base.py
--rw-r--r--   0        0        0       94 2022-04-26 15:15:35.783434 pait-0.8.0.2/pait/app/sanic/plugin/cache_resonse.py
--rw-r--r--   0        0        0      530 2022-04-24 09:27:10.492493 pait-0.8.0.2/pait/app/sanic/plugin/check_json_resp.py
--rw-r--r--   0        0        0     2289 2022-04-24 08:42:32.960455 pait-0.8.0.2/pait/app/sanic/plugin/mock_response.py
--rw-r--r--   0        0        0      206 2022-05-22 09:15:45.881445 pait-0.8.0.2/pait/app/starlette/__init__.py
--rw-r--r--   0        0        0     3079 2022-09-27 02:53:58.448686 pait-0.8.0.2/pait/app/starlette/_app_helper.py
--rw-r--r--   0        0        0     2310 2022-10-25 07:55:58.154116 pait-0.8.0.2/pait/app/starlette/_doc_route.py
--rw-r--r--   0        0        0     4050 2022-05-01 06:16:19.723473 pait-0.8.0.2/pait/app/starlette/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.986457 pait-0.8.0.2/pait/app/starlette/_pait.py
--rw-r--r--   0        0        0     1935 2022-03-16 02:33:41.341890 pait-0.8.0.2/pait/app/starlette/_test_helper.py
--rw-r--r--   0        0        0     1282 2022-08-23 17:28:05.351408 pait-0.8.0.2/pait/app/starlette/grpc_route.py
--rw-r--r--   0        0        0      549 2022-04-24 07:40:23.411088 pait-0.8.0.2/pait/app/starlette/plugin/__init__.py
--rw-r--r--   0        0        0      739 2022-05-20 05:50:27.376488 pait-0.8.0.2/pait/app/starlette/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0      846 2022-05-20 04:35:53.759104 pait-0.8.0.2/pait/app/starlette/plugin/base.py
--rw-r--r--   0        0        0       94 2022-04-26 15:15:35.795434 pait-0.8.0.2/pait/app/starlette/plugin/cache_resonse.py
--rw-r--r--   0        0        0      675 2022-04-24 08:43:51.780740 pait-0.8.0.2/pait/app/starlette/plugin/check_json_resp.py
--rw-r--r--   0        0        0     4011 2022-04-24 09:41:49.805889 pait-0.8.0.2/pait/app/starlette/plugin/mock_response.py
--rw-r--r--   0        0        0      204 2022-05-22 09:15:45.861444 pait-0.8.0.2/pait/app/tornado/__init__.py
--rw-r--r--   0        0        0     2938 2022-09-27 02:53:58.440686 pait-0.8.0.2/pait/app/tornado/_app_helper.py
--rw-r--r--   0        0        0     3979 2022-10-25 08:00:15.346346 pait-0.8.0.2/pait/app/tornado/_doc_route.py
--rw-r--r--   0        0        0     2473 2022-05-01 06:16:19.723473 pait-0.8.0.2/pait/app/tornado/_load_app.py
--rw-r--r--   0        0        0      291 2022-01-10 09:58:31.986457 pait-0.8.0.2/pait/app/tornado/_pait.py
--rw-r--r--   0        0        0     4669 2022-02-11 01:59:50.264282 pait-0.8.0.2/pait/app/tornado/_test_helper.py
--rw-r--r--   0        0        0     2802 2022-08-23 17:28:05.415393 pait-0.8.0.2/pait/app/tornado/grpc_route.py
--rw-r--r--   0        0        0      366 2022-03-28 14:19:11.993656 pait-0.8.0.2/pait/app/tornado/plugin/__init__.py
--rw-r--r--   0        0        0      706 2022-05-20 05:50:27.484500 pait-0.8.0.2/pait/app/tornado/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     1002 2022-05-20 05:45:53.177191 pait-0.8.0.2/pait/app/tornado/plugin/base.py
--rw-r--r--   0        0        0     1329 2022-05-20 07:37:02.050010 pait-0.8.0.2/pait/app/tornado/plugin/cache_resonse.py
--rw-r--r--   0        0        0      672 2022-04-24 08:56:17.487671 pait-0.8.0.2/pait/app/tornado/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1784 2022-04-24 08:56:17.495671 pait-0.8.0.2/pait/app/tornado/plugin/mock_response.py
--rw-r--r--   0        0        0    16704 2022-09-28 06:29:21.991399 pait-0.8.0.2/pait/core.py
--rw-r--r--   0        0        0     1847 2021-12-30 03:38:52.475392 pait-0.8.0.2/pait/data.py
--rw-r--r--   0        0        0      688 2022-02-08 08:17:48.934446 pait-0.8.0.2/pait/exceptions.py
--rw-r--r--   0        0        0        0 2022-04-03 14:03:33.877350 pait-0.8.0.2/pait/extra/__init__.py
--rw-r--r--   0        0        0     7056 2022-09-06 07:25:10.427425 pait-0.8.0.2/pait/extra/config.py
--rw-r--r--   0        0        0      633 2022-04-06 08:54:19.783930 pait-0.8.0.2/pait/extra/status.py
--rw-r--r--   0        0        0      675 2022-09-27 06:49:29.899567 pait-0.8.0.2/pait/extra/util.py
--rw-r--r--   0        0        0     6634 2022-09-26 11:20:16.734071 pait-0.8.0.2/pait/field.py
--rw-r--r--   0        0        0     1286 2022-05-06 10:28:35.168403 pait-0.8.0.2/pait/g.py
--rw-r--r--   0        0        0     2925 2022-08-22 16:03:49.562401 pait-0.8.0.2/pait/http/api.proto
--rw-r--r--   0        0        0     4037 2022-08-22 16:03:49.562401 pait-0.8.0.2/pait/http/api_pb2.py
--rw-r--r--   0        0        0     8998 2022-08-22 16:03:49.562401 pait-0.8.0.2/pait/http/api_pb2.pyi
--rw-r--r--   0        0        0      146 2022-08-22 16:03:49.562401 pait-0.8.0.2/pait/http/api_pb2_grpc.py
--rw-r--r--   0        0        0       76 2022-08-22 16:03:49.562401 pait-0.8.0.2/pait/http/api_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2021-12-05 05:37:12.197993 pait-0.8.0.2/pait/model/__init__.py
--rw-r--r--   0        0        0     3883 2022-05-22 10:38:07.796589 pait-0.8.0.2/pait/model/config.py
--rw-r--r--   0        0        0     8291 2022-09-06 02:17:16.345167 pait-0.8.0.2/pait/model/core.py
--rw-r--r--   0        0        0     4199 2022-04-05 17:13:32.264529 pait-0.8.0.2/pait/model/links.py
--rw-r--r--   0        0        0     3107 2022-05-19 16:49:24.692635 pait-0.8.0.2/pait/model/response.py
--rw-r--r--   0        0        0      634 2022-04-05 17:03:51.158572 pait-0.8.0.2/pait/model/status.py
--rw-r--r--   0        0        0      526 2022-01-18 09:59:32.559247 pait-0.8.0.2/pait/model/tag.py
--rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.271191 pait-0.8.0.2/pait/model/template.py
--rw-r--r--   0        0        0    23770 2022-09-28 06:27:17.942919 pait-0.8.0.2/pait/param_handle.py
--rw-r--r--   0        0        0       32 2022-01-10 09:58:31.986457 pait-0.8.0.2/pait/plugin/__init__.py
--rw-r--r--   0        0        0     1232 2022-04-24 09:41:50.837895 pait-0.8.0.2/pait/plugin/at_most_one_of.py
--rw-r--r--   0        0        0     2129 2022-09-27 06:13:28.810618 pait-0.8.0.2/pait/plugin/auto_complete_json_resp.py
--rw-r--r--   0        0        0     3633 2022-09-28 06:28:36.927220 pait-0.8.0.2/pait/plugin/base.py
--rw-r--r--   0        0        0     2951 2022-09-28 06:28:36.915220 pait-0.8.0.2/pait/plugin/base_mock_response.py
--rw-r--r--   0        0        0     7724 2022-09-27 06:49:29.883567 pait-0.8.0.2/pait/plugin/cache_response.py
--rw-r--r--   0        0        0     2934 2022-09-28 06:28:36.895219 pait-0.8.0.2/pait/plugin/check_json_resp.py
--rw-r--r--   0        0        0     1367 2022-04-24 09:41:50.829895 pait-0.8.0.2/pait/plugin/required.py
--rw-r--r--   0        0        0      951 2022-05-22 10:37:51.771695 pait-0.8.0.2/pait/types.py
--rw-r--r--   0        0        0      597 2022-04-10 08:13:10.254884 pait-0.8.0.2/pait/util/__init__.py
--rw-r--r--   0        0        0     1769 2022-09-27 03:59:44.670659 pait-0.8.0.2/pait/util/_func_sig.py
--rw-r--r--   0        0        0     2513 2022-05-04 14:32:32.360048 pait-0.8.0.2/pait/util/_gen_tip.py
--rw-r--r--   0        0        0     4217 2022-04-14 06:46:25.199015 pait-0.8.0.2/pait/util/_i18n.py
--rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.203313 pait-0.8.0.2/pait/util/_lazy_property.py
--rw-r--r--   0        0        0     5054 2022-12-01 08:34:12.221728 pait-0.8.0.2/pait/util/_pydantic_util.py
--rw-r--r--   0        0        0     2729 2022-04-10 04:10:51.045552 pait-0.8.0.2/pait/util/_types.py
--rw-r--r--   0        0        0    12408 2022-08-25 03:29:58.918023 pait-0.8.0.2/pait/util/_util.py
--rw-r--r--   0        0        0        0 2022-05-01 06:16:19.723473 pait-0.8.0.2/pait/util/grpc_inspect/__init__.py
--rw-r--r--   0        0        0     7483 2022-08-24 02:28:24.934173 pait-0.8.0.2/pait/util/grpc_inspect/stub.py
--rw-r--r--   0        0        0      367 2022-05-06 07:15:56.863507 pait-0.8.0.2/pait/util/grpc_inspect/types.py
--rw-r--r--   0        0        0     2509 2022-12-01 08:34:17.501201 pait-0.8.0.2/pyproject.toml
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 pait-0.8.0.2/setup.py
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 pait-0.8.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 pait-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     4608 2023-03-21 10:06:14.408062 pait-1.0.0a1/README.md
+-rw-r--r--   0        0        0       37 2023-04-12 08:54:18.124162 pait-1.0.0a1/pait/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-09 17:42:05.966242 pait-1.0.0a1/pait/__version__.py
+-rw-r--r--   0        0        0      199 2023-04-15 07:27:03.886801 pait-1.0.0a1/pait/app/__init__.py
+-rw-r--r--   0        0        0     5448 2023-04-15 07:29:45.835731 pait-1.0.0a1/pait/app/any/__init__.py
+-rw-r--r--   0        0        0      535 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/__init__.py
+-rw-r--r--   0        0        0      460 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0      425 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/cache_response.py
+-rw-r--r--   0        0        0      405 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/check_json_resp.py
+-rw-r--r--   0        0        0      373 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/mock_response.py
+-rw-r--r--   0        0        0      424 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/any/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-17 11:47:59.744123 pait-1.0.0a1/pait/app/any/security/__init__.py
+-rw-r--r--   0        0        0      342 2023-02-08 03:58:49.610123 pait-1.0.0a1/pait/app/any/security/api_key.py
+-rw-r--r--   0        0        0      653 2023-02-10 15:24:31.281635 pait-1.0.0a1/pait/app/any/security/http.py
+-rw-r--r--   0        0        0      660 2023-02-08 03:43:07.655826 pait-1.0.0a1/pait/app/any/security/oauth2.py
+-rw-r--r--   0        0        0     1328 2023-01-18 19:31:20.014191 pait-1.0.0a1/pait/app/any/util.py
+-rw-r--r--   0        0        0      562 2023-02-15 10:04:32.538762 pait-1.0.0a1/pait/app/auto_load_app.py
+-rw-r--r--   0        0        0      121 2023-01-09 15:13:50.000000 pait-1.0.0a1/pait/app/base/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/base/adapter/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/base/adapter/request.py
+-rw-r--r--   0        0        0     1806 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/app/base/app_helper.py
+-rw-r--r--   0        0        0     8578 2023-04-12 08:47:20.207805 pait-1.0.0a1/pait/app/base/doc_route.py
+-rw-r--r--   0        0        0        0 2023-02-10 10:23:08.836059 pait-1.0.0a1/pait/app/base/security/__init__.py
+-rw-r--r--   0        0        0     1762 2023-03-28 15:33:21.719126 pait-1.0.0a1/pait/app/base/security/api_key.py
+-rw-r--r--   0        0        0      587 2023-02-10 03:32:05.848598 pait-1.0.0a1/pait/app/base/security/base.py
+-rw-r--r--   0        0        0     7379 2023-03-31 07:37:07.804728 pait-1.0.0a1/pait/app/base/security/http.py
+-rw-r--r--   0        0        0     4010 2023-04-12 08:47:20.183805 pait-1.0.0a1/pait/app/base/security/oauth2.py
+-rw-r--r--   0        0        0      794 2023-02-10 15:22:20.692947 pait-1.0.0a1/pait/app/base/security/util.py
+-rw-r--r--   0        0        0      649 2023-04-12 08:26:12.386264 pait-1.0.0a1/pait/app/base/simple_route.py
+-rw-r--r--   0        0        0    13748 2023-04-18 03:25:53.893314 pait-1.0.0a1/pait/app/base/test_helper.py
+-rw-r--r--   0        0        0      319 2023-04-15 07:12:04.318861 pait-1.0.0a1/pait/app/flask/__init__.py
+-rw-r--r--   0        0        0      719 2023-03-21 10:06:14.408062 pait-1.0.0a1/pait/app/flask/_app_helper.py
+-rw-r--r--   0        0        0      394 2023-03-21 10:06:14.408062 pait-1.0.0a1/pait/app/flask/_attribute.py
+-rw-r--r--   0        0        0      792 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/flask/_exception.py
+-rw-r--r--   0        0        0     3495 2023-04-12 08:26:12.398264 pait-1.0.0a1/pait/app/flask/_load_app.py
+-rw-r--r--   0        0        0      269 2022-01-10 09:58:31.000000 pait-1.0.0a1/pait/app/flask/_pait.py
+-rw-r--r--   0        0        0     1775 2023-04-15 07:12:11.062879 pait-1.0.0a1/pait/app/flask/_simple_route.py
+-rw-r--r--   0        0        0     1900 2023-04-12 08:23:56.321748 pait-1.0.0a1/pait/app/flask/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/flask/adapter/__init__.py
+-rw-r--r--   0        0        0     1689 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/flask/adapter/request.py
+-rw-r--r--   0        0        0     1070 2023-04-19 15:03:14.295510 pait-1.0.0a1/pait/app/flask/adapter/response.py
+-rw-r--r--   0        0        0      784 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/__init__.py
+-rw-r--r--   0        0        0      117 2023-02-06 11:24:42.996357 pait-1.0.0a1/pait/app/flask/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0       94 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/cache_response.py
+-rw-r--r--   0        0        0      556 2023-04-19 16:11:36.294732 pait-1.0.0a1/pait/app/flask/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1180 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/flask/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a1/pait/app/flask/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/flask/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/flask/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/flask/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-04-15 06:40:17.664067 pait-1.0.0a1/pait/app/flask/security/util.py
+-rw-r--r--   0        0        0      319 2023-04-15 07:12:04.418861 pait-1.0.0a1/pait/app/sanic/__init__.py
+-rw-r--r--   0        0        0      938 2023-03-21 10:06:14.408062 pait-1.0.0a1/pait/app/sanic/_app_helper.py
+-rw-r--r--   0        0        0      403 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/sanic/_attribute.py
+-rw-r--r--   0        0        0      319 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/sanic/_exception.py
+-rw-r--r--   0        0        0     3773 2023-04-12 08:23:56.217747 pait-1.0.0a1/pait/app/sanic/_load_app.py
+-rw-r--r--   0        0        0      374 2023-05-09 02:55:20.341357 pait-1.0.0a1/pait/app/sanic/_pait.py
+-rw-r--r--   0        0        0     1749 2023-04-15 07:12:11.082880 pait-1.0.0a1/pait/app/sanic/_simple_route.py
+-rw-r--r--   0        0        0     2172 2023-04-12 08:26:12.346264 pait-1.0.0a1/pait/app/sanic/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/sanic/adapter/__init__.py
+-rw-r--r--   0        0        0     2067 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/app/sanic/adapter/request.py
+-rw-r--r--   0        0        0     1102 2023-04-19 15:03:14.279509 pait-1.0.0a1/pait/app/sanic/adapter/response.py
+-rw-r--r--   0        0        0      716 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0       94 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/cache_response.py
+-rw-r--r--   0        0        0      934 2023-04-19 16:11:36.354731 pait-1.0.0a1/pait/app/sanic/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1432 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/mock_response.py
+-rw-r--r--   0        0        0      746 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/sanic/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a1/pait/app/sanic/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/sanic/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/sanic/security/http.py
+-rw-r--r--   0        0        0      566 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/sanic/security/oauth2.py
+-rw-r--r--   0        0        0      321 2023-04-15 06:38:51.947005 pait-1.0.0a1/pait/app/sanic/security/util.py
+-rw-r--r--   0        0        0      323 2023-04-15 07:12:04.374861 pait-1.0.0a1/pait/app/starlette/__init__.py
+-rw-r--r--   0        0        0      651 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/starlette/_app_helper.py
+-rw-r--r--   0        0        0      430 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/starlette/_attribute.py
+-rw-r--r--   0        0        0      319 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/starlette/_exception.py
+-rw-r--r--   0        0        0     3877 2023-04-12 08:26:12.314264 pait-1.0.0a1/pait/app/starlette/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a1/pait/app/starlette/_pait.py
+-rw-r--r--   0        0        0      996 2023-04-15 08:13:17.515420 pait-1.0.0a1/pait/app/starlette/_simple_route.py
+-rw-r--r--   0        0        0     1930 2023-04-12 08:26:12.430264 pait-1.0.0a1/pait/app/starlette/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/starlette/adapter/__init__.py
+-rw-r--r--   0        0        0     2718 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/starlette/adapter/request.py
+-rw-r--r--   0        0        0     1065 2023-04-19 15:03:14.267508 pait-1.0.0a1/pait/app/starlette/adapter/response.py
+-rw-r--r--   0        0        0      800 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/__init__.py
+-rw-r--r--   0        0        0      711 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0       94 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/cache_response.py
+-rw-r--r--   0        0        0      785 2023-04-19 16:11:35.998735 pait-1.0.0a1/pait/app/starlette/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1626 2023-02-16 07:49:53.639890 pait-1.0.0a1/pait/app/starlette/plugin/mock_response.py
+-rw-r--r--   0        0        0      702 2023-02-07 03:41:51.356781 pait-1.0.0a1/pait/app/starlette/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-01-09 09:37:04.000000 pait-1.0.0a1/pait/app/starlette/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/starlette/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/starlette/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/starlette/security/oauth2.py
+-rw-r--r--   0        0        0      325 2023-04-15 06:40:17.664067 pait-1.0.0a1/pait/app/starlette/security/util.py
+-rw-r--r--   0        0        0      321 2023-04-15 07:12:04.378861 pait-1.0.0a1/pait/app/tornado/__init__.py
+-rw-r--r--   0        0        0     1002 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/tornado/_app_helper.py
+-rw-r--r--   0        0        0      424 2023-03-21 10:06:14.412062 pait-1.0.0a1/pait/app/tornado/_attribute.py
+-rw-r--r--   0        0        0      298 2023-04-15 06:34:05.735149 pait-1.0.0a1/pait/app/tornado/_exception.py
+-rw-r--r--   0        0        0     2499 2023-04-12 08:23:56.301748 pait-1.0.0a1/pait/app/tornado/_load_app.py
+-rw-r--r--   0        0        0      291 2022-01-10 09:58:31.000000 pait-1.0.0a1/pait/app/tornado/_pait.py
+-rw-r--r--   0        0        0     2839 2023-04-15 07:36:59.865873 pait-1.0.0a1/pait/app/tornado/_simple_route.py
+-rw-r--r--   0        0        0     4664 2023-04-12 08:26:12.382264 pait-1.0.0a1/pait/app/tornado/_test_helper.py
+-rw-r--r--   0        0        0        0 2023-01-16 03:28:14.800891 pait-1.0.0a1/pait/app/tornado/adapter/__init__.py
+-rw-r--r--   0        0        0     2244 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/app/tornado/adapter/request.py
+-rw-r--r--   0        0        0     1130 2023-04-19 15:03:14.287509 pait-1.0.0a1/pait/app/tornado/adapter/response.py
+-rw-r--r--   0        0        0      792 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/__init__.py
+-rw-r--r--   0        0        0      574 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     1329 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/cache_response.py
+-rw-r--r--   0        0        0     1211 2023-04-19 16:11:36.402730 pait-1.0.0a1/pait/app/tornado/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     1237 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/mock_response.py
+-rw-r--r--   0        0        0     1247 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/app/tornado/plugin/unified_response.py
+-rw-r--r--   0        0        0        0 2023-02-03 19:54:29.188502 pait-1.0.0a1/pait/app/tornado/security/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/tornado/security/api_key.py
+-rw-r--r--   0        0        0      392 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/tornado/security/http.py
+-rw-r--r--   0        0        0      522 2023-04-15 06:37:25.447043 pait-1.0.0a1/pait/app/tornado/security/oauth2.py
+-rw-r--r--   0        0        0      323 2023-04-15 06:39:33.671398 pait-1.0.0a1/pait/app/tornado/security/util.py
+-rw-r--r--   0        0        0    18340 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/core.py
+-rw-r--r--   0        0        0     1645 2023-04-12 08:23:56.325748 pait-1.0.0a1/pait/data.py
+-rw-r--r--   0        0        0      688 2023-01-11 17:12:40.000000 pait-1.0.0a1/pait/exceptions.py
+-rw-r--r--   0        0        0        0 2022-04-03 14:03:33.000000 pait-1.0.0a1/pait/extra/__init__.py
+-rw-r--r--   0        0        0     7452 2023-04-12 08:47:20.055805 pait-1.0.0a1/pait/extra/config.py
+-rw-r--r--   0        0        0      637 2023-04-12 08:47:20.219805 pait-1.0.0a1/pait/extra/util.py
+-rw-r--r--   0        0        0    11023 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/field.py
+-rw-r--r--   0        0        0     1261 2023-04-12 08:47:20.207805 pait-1.0.0a1/pait/g.py
+-rw-r--r--   0        0        0      508 2023-04-12 08:47:20.799805 pait-1.0.0a1/pait/grpc/__init__.py
+-rw-r--r--   0        0        0     4623 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/base_gateway.py
+-rw-r--r--   0        0        0      511 2023-04-12 08:47:20.099805 pait-1.0.0a1/pait/grpc/desc_template.py
+-rw-r--r--   0        0        0    13407 2023-04-12 08:47:20.103805 pait-1.0.0a1/pait/grpc/gateway.py
+-rw-r--r--   0        0        0    10237 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/inspect.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/plugin/__init__.py
+-rw-r--r--   0        0        0       31 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/plugin/__main__.py
+-rw-r--r--   0        0        0     1762 2023-03-31 09:09:09.660127 pait-1.0.0a1/pait/grpc/plugin/code_gen.py
+-rw-r--r--   0        0        0     1322 2023-04-12 08:13:18.843706 pait-1.0.0a1/pait/grpc/plugin/config.py
+-rw-r--r--   0        0        0    20548 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/plugin/field_desc_proto_to_route_code.py
+-rw-r--r--   0        0        0     3248 2023-04-19 16:23:47.347674 pait-1.0.0a1/pait/grpc/plugin/gateway.py
+-rwxr-xr-x   0        0        0      266 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/plugin/main.py
+-rw-r--r--   0        0        0     1120 2023-04-19 16:29:34.584057 pait-1.0.0a1/pait/grpc/plugin/model.py
+-rw-r--r--   0        0        0        0 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/proto/__init__.py
+-rw-r--r--   0        0        0     4193 2023-04-10 06:13:16.195059 pait-1.0.0a1/pait/grpc/proto/api.proto
+-rw-r--r--   0        0        0     5030 2023-04-11 03:13:43.474993 pait-1.0.0a1/pait/grpc/proto/api_pb2.py
+-rw-r--r--   0        0        0    11716 2023-04-11 03:13:43.894994 pait-1.0.0a1/pait/grpc/proto/api_pb2.pyi
+-rw-r--r--   0        0        0      146 2023-04-11 03:13:45.778998 pait-1.0.0a1/pait/grpc/proto/api_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-04-10 09:17:38.116710 pait-1.0.0a1/pait/grpc/proto/api_pb2_grpc.pyi
+-rw-r--r--   0        0        0      436 2023-03-24 09:24:42.276250 pait-1.0.0a1/pait/grpc/types.py
+-rw-r--r--   0        0        0     4915 2023-05-09 17:31:34.510840 pait-1.0.0a1/pait/grpc/util.py
+-rw-r--r--   0        0        0      559 2023-04-12 08:23:56.233748 pait-1.0.0a1/pait/model/__init__.py
+-rw-r--r--   0        0        0     3305 2023-04-13 18:01:44.819386 pait-1.0.0a1/pait/model/config.py
+-rw-r--r--   0        0        0     1606 2023-04-12 08:47:20.947805 pait-1.0.0a1/pait/model/context.py
+-rw-r--r--   0        0        0     9670 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/model/core.py
+-rw-r--r--   0        0        0     6051 2023-04-12 16:05:40.728961 pait-1.0.0a1/pait/model/response.py
+-rw-r--r--   0        0        0      700 2023-04-17 06:04:21.361298 pait-1.0.0a1/pait/model/status.py
+-rw-r--r--   0        0        0     1400 2023-04-12 08:47:22.147805 pait-1.0.0a1/pait/model/tag.py
+-rw-r--r--   0        0        0     1166 2022-09-26 15:06:36.000000 pait-1.0.0a1/pait/model/template.py
+-rw-r--r--   0        0        0        0 2022-01-21 03:47:13.000000 pait-1.0.0a1/pait/openapi/__init__.py
+-rw-r--r--   0        0        0    10110 2023-04-15 08:16:39.307851 pait-1.0.0a1/pait/openapi/doc_route.py
+-rw-r--r--   0        0        0    12360 2023-04-08 08:28:39.674480 pait-1.0.0a1/pait/openapi/openapi.py
+-rw-r--r--   0        0        0      105 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/param_handle/__init__.py
+-rw-r--r--   0        0        0     6362 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/param_handle/_async.py
+-rw-r--r--   0        0        0     5305 2023-05-09 17:31:47.728377 pait-1.0.0a1/pait/param_handle/_sync.py
+-rw-r--r--   0        0        0    12308 2023-05-09 17:31:47.732377 pait-1.0.0a1/pait/param_handle/base.py
+-rw-r--r--   0        0        0       87 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/plugin/__init__.py
+-rw-r--r--   0        0        0     2298 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/plugin/at_most_one_of.py
+-rw-r--r--   0        0        0     2599 2023-04-18 03:27:33.637660 pait-1.0.0a1/pait/plugin/auto_complete_json_resp.py
+-rw-r--r--   0        0        0     3592 2023-04-19 15:26:48.912272 pait-1.0.0a1/pait/plugin/base.py
+-rw-r--r--   0        0        0     8794 2023-03-31 07:37:07.804728 pait-1.0.0a1/pait/plugin/cache_response.py
+-rw-r--r--   0        0        0     2228 2023-04-19 16:14:57.640339 pait-1.0.0a1/pait/plugin/check_json_resp.py
+-rw-r--r--   0        0        0     5105 2023-04-18 03:25:53.869314 pait-1.0.0a1/pait/plugin/mock_response.py
+-rw-r--r--   0        0        0     3312 2023-02-07 03:41:51.360782 pait-1.0.0a1/pait/plugin/required.py
+-rw-r--r--   0        0        0     2109 2023-04-18 03:25:53.877313 pait-1.0.0a1/pait/plugin/unified_response.py
+-rw-r--r--   0        0        0     1161 2023-02-08 11:47:07.069892 pait-1.0.0a1/pait/types.py
+-rw-r--r--   0        0        0      524 2023-02-14 09:33:41.434168 pait-1.0.0a1/pait/util/__init__.py
+-rw-r--r--   0        0        0     1979 2023-02-08 14:21:51.755841 pait-1.0.0a1/pait/util/_func_sig.py
+-rw-r--r--   0        0        0     2607 2023-01-12 10:30:13.000000 pait-1.0.0a1/pait/util/_gen_tip.py
+-rw-r--r--   0        0        0     1907 2022-04-10 08:10:06.000000 pait-1.0.0a1/pait/util/_lazy_property.py
+-rw-r--r--   0        0        0      957 2023-04-10 07:15:56.924352 pait-1.0.0a1/pait/util/_pydantic_util.py
+-rw-r--r--   0        0        0     4211 2023-04-15 06:41:46.425281 pait-1.0.0a1/pait/util/_types.py
+-rw-r--r--   0        0        0    13475 2023-04-26 06:56:27.310437 pait-1.0.0a1/pait/util/_util.py
+-rw-r--r--   0        0        0      869 2023-04-13 18:01:45.039386 pait-1.0.0a1/pait/util/encoder.py
+-rw-r--r--   0        0        0     3561 2023-05-09 17:42:05.962242 pait-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 pait-1.0.0a1/setup.py
+-rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 pait-1.0.0a1/PKG-INFO
```

### Comparing `pait-0.8.0.2/LICENSE` & `pait-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pait-0.8.0.2/pait/app/__init__.py` & `pait-1.0.0a1/pait/app/any/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,110 @@
 from dataclasses import MISSING
 from importlib import import_module
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Type
 
-from pydantic import BaseConfig
+from pydantic import BaseConfig, BaseModel
+from typing_extensions import NoReturn
 
-from pait.core import PluginManager, TagT
-from pait.model.status import PaitStatus
-
-from ..model.core import PaitCoreModel  # type: ignore
-from ..model.response import PaitBaseResponseModel  # type: ignore
-from .auto_load_app import auto_load_app_class  # type: ignore
-from .base.util import sniffing
+from pait.app.any.util import base_call_func, sniffing
+from pait.app.auto_load_app import auto_load_app_class
+from pait.app.base.simple_route import SimpleRoute
+from pait.field import BaseField
+from pait.model import BaseResponseModel, PaitCoreModel, PaitStatus, Tag
+from pait.plugin.base import PluginManager, PostPluginProtocol, PrePluginProtocol
 
 if TYPE_CHECKING:
+    from pait.openapi.openapi import OpenAPI
     from pait.param_handle import BaseParamHandler
 
+
+_NotFoundFrameworkException = RuntimeError(
+    "The web framework to use cannot be found automatically, please specify it manually"
+)
+
+
+class Empty(object):
+    def __int__(self) -> NoReturn:
+        raise _NotFoundFrameworkException
+
+    def __setattr__(self, key: Any, value: Any) -> NoReturn:
+        raise _NotFoundFrameworkException
+
+    def __getattr__(self, item: Any) -> NoReturn:
+        raise _NotFoundFrameworkException
+
+    def __call__(self, *args: Any, **kwargs: Any) -> NoReturn:
+        raise _NotFoundFrameworkException
+
+
 try:
     load_class_app: Any = auto_load_app_class()
     pait_app_path: str = "pait.app." + load_class_app.__name__.lower()
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
-        from pait.app.base.doc_route import AddDocRoute as _AddDocRoute
-        from pait.app.base.grpc_route import GrpcGatewayRoute as _GrpcGatewayRoute
         from pait.core import Pait as _Pait
 
     Pait: "_Pait" = getattr(import_module(pait_app_path), "Pait")
-    AddDocRoute: "_AddDocRoute" = getattr(import_module(pait_app_path), "AddDocRoute")
-    GrpcGatewayRoute: "_GrpcGatewayRoute" = getattr(import_module(pait_app_path + ".grpc_route"), "GrpcGatewayRoute")
+    http_exception = getattr(import_module(pait_app_path), "http_exception")
 except RuntimeError:  # pragma: no cover
     # Automatic loading of classes, loading failure when the user can not use
+    load_class_app = Empty()
+    Pait = Empty()  # type: ignore
     pait_app_path = ""  # pragma: no cover
+    http_exception = Empty()  # type: ignore
 
 
-def _import_func_from_app(app: Any, fun_name: str) -> Callable:
-    app_name: str = sniffing(app)
-    return getattr(import_module(f"pait.app.{app_name}"), fun_name)
-
-
-def _base_call_func(app: Any, fun_name: str, *args: Any, **kwargs: Any) -> Any:
-    return _import_func_from_app(app, fun_name)(*args, **kwargs)
-
-
-def load_app(app: Any, project_name: str = "") -> Dict[str, PaitCoreModel]:
+def load_app(app: Any, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`
     Note:This is an implicit method
     """
-    return _base_call_func(app, "load_app", app, project_name=project_name)
-
-
-def add_doc_route(
-    app: Any,
-    scheme: Optional[str] = None,
-    open_json_url_only_path: bool = False,
-    prefix: str = "",
-    pin_code: str = "",
-    title: str = "",
-    open_api_tag_list: Optional[List[Dict[str, Any]]] = None,
-    project_name: str = "",
-) -> None:
-    return _base_call_func(
-        app,
-        "add_doc_route",
-        scheme=scheme,
-        open_json_url_only_path=open_json_url_only_path,
-        prefix=prefix,
-        pin_code=pin_code,
-        title=title,
-        open_api_tag_list=open_api_tag_list,
-        project_name=project_name,
-    )
+    return base_call_func("load_app", app, app=app, auto_load_route=auto_load_route)
 
 
 def pait(
     pydantic_model_config: Optional[Type[BaseConfig]] = None,
+    pydantic_basemodel: Optional[Type[BaseModel]] = None,
+    default_field_class: Optional[Type[BaseField]] = None,
     # param check
     pre_depend_list: Optional[List[Callable]] = None,
     append_pre_depend_list: Optional[List[Callable]] = None,
     # doc
     author: Optional[Tuple[str, ...]] = None,
     append_author: Optional[Tuple[str, ...]] = None,
     desc: Optional[str] = None,
     summary: Optional[str] = None,
     name: Optional[str] = None,
     status: Optional[PaitStatus] = None,
     group: Optional[str] = None,
-    tag: Optional[Tuple[TagT, ...]] = None,
-    append_tag: Optional[Tuple[str, ...]] = None,
-    response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
-    append_response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
-    plugin_list: Optional[List[PluginManager]] = None,
-    append_plugin_list: Optional[List[PluginManager]] = None,
+    tag: Optional[Tuple[Tag, ...]] = None,
+    append_tag: Optional[Tuple[Tag, ...]] = None,
+    response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
+    append_response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
+    # plugin
+    plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+    append_plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+    post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
+    append_post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
     param_handler_plugin: Optional[Type["BaseParamHandler"]] = None,
     feature_code: str = "",
+    **kwargs: Any,
 ) -> Callable:
     """provide parameter checks and type conversions for each routing function/cbv class
     Note:This is an implicit method
     """
     if not pait_app_path:
         raise RuntimeError("Auto load app fail")  # pragma: no cover
     _pait: Optional[Callable] = getattr(import_module(pait_app_path), "pait")
     if not _pait:
         raise NotImplementedError(f"Pait not support:{load_class_app}")
     return _pait(
+        pydantic_basemodel=pydantic_basemodel,
         pydantic_model_config=pydantic_model_config,
+        default_field_class=default_field_class,
         pre_depend_list=pre_depend_list,
         append_pre_depend_list=append_pre_depend_list,
         author=author,
         append_author=append_author,
         desc=desc,
         summary=summary,
         name=name,
@@ -115,46 +112,31 @@
         group=group,
         tag=tag,
         append_tag=append_tag,
         response_model_list=response_model_list,
         append_response_model_list=append_response_model_list,
         plugin_list=plugin_list,
         append_plugin_list=append_plugin_list,
+        post_plugin_list=post_plugin_list,
+        append_post_plugin_list=append_post_plugin_list,
         param_handler_plugin=param_handler_plugin,
         feature_code=feature_code,
+        **kwargs,
     )
 
 
 def set_app_attribute(app: Any, key: str, value: Any) -> None:
-    app_name: str = sniffing(app)
-    if app_name == "flask":
-        app.config[key] = value
-        from flask import g
-
-        def _before_request() -> None:
-            setattr(g, key, value)
-
-        app.before_request(_before_request)
-    elif app_name == "sanic":
-        setattr(app.ctx, key, value)
-    elif app_name == "starlette":
-        setattr(app.state, key, value)
-    elif app_name == "tornado":
-        app.settings[key] = value
-
-
-def get_app_attribute(app: Any, key: str) -> Any:
-    app_name: str = sniffing(app)
-    if app_name == "flask":
-        value: Any = app.config.get(key, MISSING)
-        if value is not MISSING:
-            return value
-
-        from flask import g
-
-        return getattr(g, key)
-    elif app_name == "starlette":
-        return getattr(app.state, key)
-    elif app_name == "sanic":
-        return getattr(app.ctx, key)
-    elif app_name == "tornado":
-        return app.settings[key]
+    base_call_func("set_app_attribute", app, key, value, app=app)
+
+
+def get_app_attribute(app: Any, key: str, default_value: Any = MISSING) -> Any:
+    return base_call_func("get_app_attribute", app, key, default_value, app=app)
+
+
+def add_simple_route(app: Any, simple_route: "SimpleRoute") -> None:
+    base_call_func("add_simple_route", app, simple_route, app=app)
+
+
+def add_multi_simple_route(
+    app: Any, *simple_route_list: "SimpleRoute", prefix: str = "/", title: str = "", **kwargs: Any
+) -> None:
+    base_call_func("add_multi_simple_route", app, *simple_route_list, app=app, prefix=prefix, title=title, **kwargs)
```

### Comparing `pait-0.8.0.2/pait/app/auto_load_app.py` & `pait-1.0.0a1/pait/app/auto_load_app.py`

 * *Files identical despite different names*

### Comparing `pait-0.8.0.2/pait/app/base/doc_route.py` & `pait-1.0.0a1/pait/app/base/doc_route.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,86 +1,79 @@
 import json
 import logging
 from enum import Enum
 from typing import Any, Callable, Dict, Generic, List, Optional, Type, TypeVar
 from urllib.parse import urlencode
-from warnings import warn
 
-from pydantic import BaseModel
+from any_api.openapi import web_ui
+from pydantic import BaseModel, Field
 
-from pait.api_doc.html import get_elements_html as _get_elements_html
-from pait.api_doc.html import get_rapidoc_html as _get_rapidoc_html
-from pait.api_doc.html import get_rapipdf_html as _get_rapipdf_html
-from pait.api_doc.html import get_redoc_html as _get_redoc_html
-from pait.api_doc.html import get_swagger_ui_html as _get_swagger_ui_html
-from pait.api_doc.open_api import PaitOpenAPI
 from pait.core import Pait, PluginManager
 from pait.field import Depends, Path, Query
 from pait.g import config, pait_context
-from pait.model.core import PaitCoreModel
-from pait.model.response import PaitHtmlResponseModel, PaitJsonResponseModel
-from pait.model.status import PaitStatus
-from pait.model.tag import Tag
-from pait.model.template import TemplateContext
+from pait.model import HtmlResponseModel, JsonResponseModel, PaitCoreModel, PaitStatus, Tag, TemplateContext
+from pait.openapi.openapi import InfoModel, OpenAPI, ServerModel
 
 logger: logging.Logger = logging.getLogger(__name__)
-__all__ = ["DocHtmlRespModel", "OpenAPIRespModel", "AddDocRoute", "default_doc_fn_dict"]
+__all__ = [
+    "DocHtmlRespModel",
+    "OpenAPIRespModel",
+    "AddDocRoute",
+    "default_doc_fn_dict",
+    "OpenAPI",
+    "InfoModel",
+    "ServerModel",
+]
+
+
+class DocHtmlRespModel(HtmlResponseModel):
+    class HeaderModel(BaseModel):
+        x_example_type: str = Field(default="html", alias="X-Example-Type")
 
-
-class DocHtmlRespModel(PaitHtmlResponseModel):
-    header: dict = {"X-Example-Type": "html"}
+    header: BaseModel = HeaderModel
     description: str = "doc html response"
 
 
-class OpenAPIRespModel(PaitJsonResponseModel):
+class OpenAPIRespModel(JsonResponseModel):
     class OpenAPIResponseModel(BaseModel):
         pass
 
     description: str = "open api json response"
     # TODO replace to openapi response model
     response_data: dict = {}  # type: ignore
 
 
 APP_T = TypeVar("APP_T")
-ResponseT = TypeVar("ResponseT")
 
 
-default_doc_fn_dict: Dict[str, Callable] = {
-    "redoc": _get_redoc_html,
-    "swagger": _get_swagger_ui_html,
-    "rapidoc": _get_rapidoc_html,
-    "rapipdf": _get_rapipdf_html,
-    "elements": _get_elements_html,
-}
+default_doc_fn_dict: Dict[str, Callable] = {key.split("_")[1]: getattr(web_ui, key) for key in web_ui.__all__}
 
 
 class DocEnum(str, Enum):
     pass
 
 
-class AddDocRoute(Generic[APP_T, ResponseT]):
+class AddDocRoute(Generic[APP_T]):
     not_found_exc: Exception
-    html_response: staticmethod
-    json_response: staticmethod
     pait_class: Type[Pait]
     load_app: staticmethod
 
     def __init__(
         self,
+        app: APP_T,
         scheme: Optional[str] = None,
         openapi_json_url_only_path: bool = False,
         prefix: str = "",
         pin_code: str = "",
         title: str = "",
-        open_api_tag_list: Optional[List[Dict[str, Any]]] = None,
-        project_name: str = "",
         doc_fn_dict: Optional[Dict[str, Callable]] = None,
-        app: APP_T = None,
+        openapi: Optional[Type[OpenAPI]] = None,
     ):
         """
+        :param app: The app instance to which the doc route is bound
         :param scheme: The scheme of the specified url, if the value is empty,
             it will be automatically selected according to the request
 
             Note: If the deployment is HTTP and the site configured by Nginx is HTTPS,
                 then need to force the specified scheme to be HTTPS
         :param openapi_json_url_only_path: If True, openapi json url does not include HTTP scheme, hostname and port
             Example:
@@ -89,56 +82,42 @@
         :param prefix: Doc route path prefix
         :param pin_code: If pin_code is set, the pin code parameter needs to be added when requesting doc route
             Example:
                 pin_code: None, url `http://127.0.0.1:8080/api/path`
                 pin_code: 6666, url `http://127.0.0.1:8080/api/path?pin-code=6666`
         :param title: Doc route group name,
             the title of multiple doc routes registered for the same app instance must be different
-        :param open_api_tag_list: Doc route group open api tag
-        :param project_name: see `pait.app.{web framework}._load_app.load_app`
+        :param openapi: OpenAPI class
         :param doc_fn_dict: doc ui dict, default `pait.app.base.doc_route.default_doc_fn_dict`
-        :param app: The app instance to which the doc route is bound
         """
         if pin_code:
             logging.info(f"doc route start pin code:{pin_code}")
         self.scheme: Optional[str] = scheme
         self.openapi_json_url_only_path: bool = openapi_json_url_only_path
         self.prefix: str = prefix or "/"
         self.pin_code: str = pin_code
         self.title: str = title or "Pait Doc"
-        self.open_api_tag_list: Optional[List[Dict[str, Any]]] = open_api_tag_list
-        self.project_name: str = project_name
+        self.openapi: Type[OpenAPI] = openapi or OpenAPI
         self._is_gen: bool = False
         self._doc_fn_dict: Dict[str, Callable] = doc_fn_dict or default_doc_fn_dict
         self._doc_pait: Pait = self.pait_class(
             author=config.author or ("so1n",),
             status=config.status or PaitStatus.release,
             tag=(Tag("pait_doc", desc="pait default doc route"),),
             group="pait_doc",
         )
-
-        if app:
-            self._is_gen = True
-            self._gen_route(app)
+        self.gen_route(app)
 
     def _get_request_pin_code(
         self,
         r_pin_code: str = Query.i("", alias="pin-code"),
-        old_r_pin_code: str = Query.i(
-            "",
-            alias="pin_code",
-            description="This parameter is used for legacy functionality and will be deprecated later",
-        ),
     ) -> Optional[str]:
-        if self.pin_code:
-            if old_r_pin_code != "":
-                warn("Param `pin_code` will be deprecated, please use `pin-code`")
-            if r_pin_code != self.pin_code and old_r_pin_code != self.pin_code:
-                raise self.not_found_exc
-        return r_pin_code or old_r_pin_code
+        if self.pin_code and r_pin_code != self.pin_code:
+            raise self.not_found_exc
+        return r_pin_code
 
     @staticmethod
     def _get_request_template_map(extra_key: bool = False) -> Callable:
         def _get_request_template_map(
             url_dict: Dict[str, Any] = Query.i(
                 default_factory=dict,
                 raw_return=True,
@@ -157,22 +136,22 @@
         return _get_request_template_map
 
     def _gen_url_fn(self) -> Callable:
         def _get_openapi_json_url(
             r_pin_code: str = Depends.i(self._get_request_pin_code),
             url_dict: Dict[str, Any] = Depends.i(self._get_request_template_map()),
         ) -> str:
-            re = pait_context.get().app_helper.request_extend()
+            re = pait_context.get().app_helper.request.request_extend()
             _scheme: str = self.scheme or re.scheme
             if self.openapi_json_url_only_path:
                 openapi_json_url: str = f"{'/'.join(re.path.split('/')[:-1])}/openapi.json"
             else:
                 openapi_json_url = f"{_scheme}://{re.hostname}{'/'.join(re.path.split('/')[:-1])}/openapi.json"
             if r_pin_code:
-                url_dict["pin_code"] = r_pin_code
+                url_dict["pin-code"] = r_pin_code
             openapi_json_url += "?" + urlencode(url_dict)
             return openapi_json_url
 
         return _get_openapi_json_url
 
     @staticmethod
     def _get_doc_pait(
@@ -201,43 +180,41 @@
             pre_depend_list=[self._get_request_pin_code],
             response_model_list=[DocHtmlRespModel],
             feature_code=self.title,
         )
         def _doc_route(
             route_path: dynamic_enum_class = Path.i(description="doc ui html"),  # type: ignore
             url: str = Depends.i(self._gen_url_fn()),
-        ) -> ResponseT:
+        ) -> str:
             get_doc_route: Callable = self._doc_fn_dict[route_path.value]  # type: ignore
-            return self.html_response(get_doc_route(url, title=self.title))
+            return get_doc_route(url, title=self.title)
 
         _doc_route.__name__ = self.title + "doc_route"
         _doc_route.__qualname__ = _doc_route.__qualname__.replace("._doc_route", "." + _doc_route.__name__)
         return _doc_route
 
     def _get_openapi_route(self, app: APP_T) -> Callable:
         @self._doc_pait(
             pre_depend_list=[self._get_request_pin_code],
             response_model_list=[OpenAPIRespModel],
             feature_code=self.title,
         )
         def _openapi_route(
             url_dict: Dict[str, Any] = Depends.i(self._get_request_template_map(extra_key=True)),
-        ) -> ResponseT:
-            re = pait_context.get().app_helper.request_extend()
+        ) -> dict:
+            re = pait_context.get().app_helper.request.request_extend()
             _scheme: str = self.scheme or re.scheme
-            pait_dict: Dict[str, PaitCoreModel] = self.load_app(app, project_name=self.project_name)
+            pait_dict: Dict[str, PaitCoreModel] = self.load_app(app)
             with TemplateContext(url_dict):
-                pait_openapi: PaitOpenAPI = PaitOpenAPI(
+                pait_openapi: OpenAPI = OpenAPI(
                     pait_dict,
-                    title=self.title,
-                    open_api_server_list=[{"url": f"{_scheme}://{re.hostname}", "description": ""}],
-                    open_api_tag_list=self.open_api_tag_list,
+                    openapi_info_model=InfoModel(title=self.title),
+                    server_model_list=[ServerModel(url=f"{_scheme}://{re.hostname}")],
                 )
-                response: ResponseT = self.json_response(json.loads(pait_openapi.content))
-            return response
+                return json.loads(pait_openapi.content())
 
         return _openapi_route
 
     def gen_route(self, app: APP_T) -> None:
         """Will remove on version 1.0"""
         if self._is_gen:
             raise RuntimeError("Doc route has been generated")
```

### Comparing `pait-0.8.0.2/pait/app/base/test_helper.py` & `pait-1.0.0a1/pait/app/base/test_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,60 @@
 import copy
 import difflib
-from typing import Any, Callable, Dict, Generic, List, Mapping, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, Dict, Generic, List, Mapping, Optional, Type, TypeVar
 from urllib.parse import urlencode
 
 from pydantic import BaseModel, ValidationError
 
 from pait.model import response
-from pait.model.core import PaitCoreModel
 from pait.util import gen_example_dict_from_schema, gen_example_value_from_python, get_pait_response_model
 
+if TYPE_CHECKING:
+    from pait.model import PaitCoreModel
+
 RESP_T = TypeVar("RESP_T")
 
 
+class CheckResponseException(Exception):
+    def __init__(
+        self,
+        status_code: Optional[int] = None,
+        media_type: Optional[str] = None,
+        headers: Optional[Mapping] = None,
+        resp: Any = None,
+        func: Optional[Callable] = None,
+        message: Optional[str] = None,
+    ):
+        self.status_code: Optional[int] = status_code
+        self.media_type: Optional[str] = media_type
+        self.headers: Optional[Mapping] = headers
+        self.resp: Any = resp
+        self.func: Optional[Callable] = func
+        self.message: Optional[str] = message
+        super().__init__(self.message)
+
+
 class BaseTestHelper(Generic[RESP_T]):
     client: Any
 
     def __init__(
         self,
         client: Any,
         func: Callable,
-        pait_dict: Optional[Dict[str, PaitCoreModel]] = None,
+        pait_dict: Optional[Dict[str, "PaitCoreModel"]] = None,
         body_dict: Optional[dict] = None,
         cookie_dict: Optional[dict] = None,
         file_dict: Optional[dict] = None,
         form_dict: Optional[dict] = None,
         header_dict: Optional[dict] = None,
         path_dict: Optional[dict] = None,
         query_dict: Optional[dict] = None,
         strict_inspection_check_json_content: bool = True,
-        find_coro_response_model: bool = False,
-        target_pait_response_class: Optional[Type["response.PaitBaseResponseModel"]] = None,
+        find_response_model: bool = False,
+        target_pait_response_class: Optional[Type["response.BaseResponseModel"]] = None,
     ):
         """
         :param client:  test client
         :param func:  route handle decorated by pait
         :param pait_dict:  pait core data
         :param body_dict:  request body param
         :param cookie_dict:  request cookie param
@@ -47,18 +68,18 @@
         if not pait_id:
             raise RuntimeError(f"Can not found pait id from {func}")
 
         self.client: Any = client
         self.func: Callable = func
         # pait dict handle
         if pait_dict:
-            self.pait_dict: Dict[str, PaitCoreModel] = pait_dict
+            self.pait_dict: Dict[str, "PaitCoreModel"] = pait_dict
         else:
             self.pait_dict = self._gen_pait_dict()
-        self.pait_core_model: PaitCoreModel = self.pait_dict[pait_id]
+        self.pait_core_model: "PaitCoreModel" = self.pait_dict[pait_id]
 
         self.body_dict: Optional[dict] = body_dict
         self.cookie_dict: Optional[dict] = cookie_dict
         self.file_dict: Optional[dict] = file_dict
         self.form_dict: Optional[dict] = form_dict
         self.header_dict: dict = header_dict or {}
         self.path_dict: Optional[dict] = path_dict
@@ -82,23 +103,23 @@
 
         # add query path by path
         if self.query_dict:
             self.path = self.path + "?" + urlencode(self.query_dict, True)
         if not self.path.startswith("/"):
             self.path = "/" + self.path
 
-        self.find_coro_response_model: bool = find_coro_response_model
-        self.target_pait_response_class: Optional[Type["response.PaitBaseResponseModel"]] = target_pait_response_class
+        self.find_response_model: bool = find_response_model
+        self.target_pait_response_class: Optional[Type["response.BaseResponseModel"]] = target_pait_response_class
         self._app_init_field()
 
     def _app_init_field(self) -> None:
         """init request param by application framework"""
         raise NotImplementedError()
 
-    def _gen_pait_dict(self) -> Dict[str, PaitCoreModel]:
+    def _gen_pait_dict(self) -> Dict[str, "PaitCoreModel"]:
         """load pait dict"""
         raise NotImplementedError()
 
     @staticmethod
     def _get_status_code(resp: RESP_T) -> int:
         """get response status code"""
         raise NotImplementedError()
@@ -155,25 +176,24 @@
             raise RuntimeError(f"Can not found key from model, key:{' -> '.join(parent_key_list or '')}")
 
     def _assert_response(self, resp: RESP_T) -> None:
         """Whether the structure of the check response is correct"""
         if not self.pait_core_model.response_model_list:
             return
 
-        real_response_model: Optional[Type[response.PaitBaseResponseModel]] = None
+        real_response_model: Optional[Type[response.BaseResponseModel]] = None
         max_quick_ratio: float = 0.0
-        model_check_msg_dict: Dict[Type[response.PaitBaseResponseModel], List[str]] = {}
-        response_model_list: List[Type[response.PaitBaseResponseModel]] = (
+        model_check_msg_dict: Dict[Type[response.BaseResponseModel], List[str]] = {}
+        response_model_list: List[Type[response.BaseResponseModel]] = (
             self.pait_core_model.response_model_list
-            if not self.find_coro_response_model
+            if not self.find_response_model
             else [
                 get_pait_response_model(
                     self.pait_core_model.response_model_list,
                     target_pait_response_class=self.target_pait_response_class,
-                    find_core_response_model=self.find_coro_response_model,
                 )
             ]
         )
         for response_model in response_model_list:
             error_msg_list: List[str] = []
             status_code: int = self._get_status_code(resp)
             content_type: str = self._get_content_type(resp)
@@ -188,24 +208,29 @@
                 error_msg_list.append(
                     "check media type error."
                     f"Get the response with a media type of {content_type}, "
                     f"but the response_model specifies a media type of {response_model.media_type}"
                 )
 
             resp_header: Mapping = self._get_headers(resp)
-            for key, _ in response_model.header.items():
+            for key, _ in response_model.get_header_example_dict().items():
                 if key not in resp_header:
                     error_msg_list.append(
                         f"check header error. Can not found header:{key} in {str(resp_header).strip()}"
                     )
 
             # check content
-            if issubclass(response_model, response.PaitJsonResponseModel):
+            if issubclass(response_model, response.JsonResponseModel):
                 response_data_model: Type[BaseModel] = response_model.response_data
-                resp_dict: Optional[dict] = self._get_json(resp)
+                resp_dict: Optional[dict] = None
+                try:
+                    resp_dict = self._get_json(resp)
+                except Exception:
+                    pass
+
                 if not resp_dict:
                     continue
                 response_data_default_dict: dict = gen_example_dict_from_schema(response_data_model.schema())
                 ratio: float = difflib.SequenceMatcher(
                     None,
                     str(gen_example_value_from_python(resp_dict)),
                     str(response_data_default_dict),
@@ -219,57 +244,59 @@
                     if self.strict_inspection_check_json_content and not self._check_diff_resp_dict(
                         resp_dict, response_data_default_dict
                     ):
                         error_msg_list.append("check json structure error")
                 except (ValidationError, RuntimeError) as e:
                     error_msg_list.append(f"check json content error, exec: {e}")
 
-            elif issubclass(response_model, response.PaitHtmlResponseModel) or issubclass(
-                response_model, response.PaitTextResponseModel
+            elif issubclass(response_model, response.HtmlResponseModel) or issubclass(
+                response_model, response.TextResponseModel
             ):
                 real_response_model = response_model
                 if not isinstance(self._get_text(resp), type(response_model.response_data)):
                     error_msg_list.append("check text content type error")  # pragma: no cover
-            elif issubclass(response_model, response.PaitFileResponseModel):
+            elif issubclass(response_model, response.FileResponseModel):
                 real_response_model = response_model
                 if not isinstance(self._get_bytes(resp), type(response_model.response_data)):
                     error_msg_list.append("check bytes content type error")  # pragma: no cover
             else:
                 raise TypeError(f"Pait not support response model:{response_model}")
             if not error_msg_list:
                 return
             else:
                 model_check_msg_dict[response_model] = error_msg_list
-        response_dict: dict = {
-            "status_code": self._get_status_code(resp),
-            "media_type": self._get_content_type(resp),
-            "headers": self._get_headers(resp),
-            "obj": resp,
-        }
         if real_response_model in model_check_msg_dict:
             error_str: str = "\n    ".join(model_check_msg_dict[real_response_model])
-            raise RuntimeError(
-                f"Check {self.func} Response Error.\n"
-                " maybe error result: \n"
-                f"    {error_str}\n\n"
-                f" by response model:{real_response_model}\n"
-                f" response info: {response_dict}"
+            raise CheckResponseException(
+                status_code=self._get_status_code(resp),
+                media_type=self._get_content_type(resp),
+                headers=self._get_headers(resp),
+                resp=resp,
+                func=self.func,
+                message=(
+                    " maybe error result: \n" f"    {error_str}\n\n" f" by response model:{real_response_model}\n"
+                ),
             )
+
         error_str = ""
         for k, v in model_check_msg_dict.items():
             error_str += str(k)
             error_str += ":\n"
             error_str += "    \n".join(v)
-
-        raise RuntimeError(
-            f"Check {self.func} Response Error. \n"
-            f"response error result:{error_str} \n"
-            f"total response model:{self.pait_core_model.response_model_list}. \n"
-            f"response info: {response_dict} "
-        )  # pragma: no cover
+        raise CheckResponseException(
+            status_code=self._get_status_code(resp),
+            media_type=self._get_content_type(resp),
+            headers=self._get_headers(resp),
+            resp=resp,
+            func=self.func,
+            message=(
+                f"response error result:{error_str} \n"
+                f"by response model list:{self.pait_core_model.response_model_list}. \n"
+            ),
+        )
 
     def _replace_path(self, path_str: str) -> Optional[str]:
         raise NotImplementedError()
 
     def _real_request(self, method: str) -> RESP_T:
         """Whether the structure of the check response is correct"""
         raise NotImplementedError()
```

### Comparing `pait-0.8.0.2/pait/app/flask/_app_helper.py` & `pait-1.0.0a1/pait/app/flask/adapter/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,61 @@
-from dataclasses import MISSING
 from typing import Any, Dict, List, Mapping
 
-from flask import Request, g, request
-from flask.views import View
+from flask import Request as FlaskRequest
+from flask import request as _request
 from werkzeug.datastructures import EnvironHeaders, ImmutableMultiDict
 
-from pait.app.base import BaseAppHelper, BaseRequestExtend
+from pait.app.base.adapter.request import BaseRequest, BaseRequestExtend
 from pait.util import LazyProperty
 
-__all__ = ["AppHelper", "RequestExtend"]
 
-
-class RequestExtend(BaseRequestExtend[Request]):
+class RequestExtend(BaseRequestExtend[FlaskRequest]):
     @property
     def scheme(self) -> str:
-        return request.scheme
+        return _request.scheme
 
     @property
     def path(self) -> str:
-        return request.path
+        return _request.path
 
     @property
     def hostname(self) -> str:
-        return request.host
-
+        return _request.host
 
-class AppHelper(BaseAppHelper[Request, RequestExtend]):
 
-    RequestType = Request
+class Request(BaseRequest[FlaskRequest, RequestExtend]):
+    RequestType = FlaskRequest
     FormType = ImmutableMultiDict
-    FileType = Request.files
+    FileType = FlaskRequest.files
     HeaderType = EnvironHeaders
-    CbvType = (View,)
-    app_name = "flask"
-
-    def __init__(self, args: List[Any], kwargs: Mapping[str, Any]):
-        super().__init__(args, kwargs)
-
-        self.request = request
-
-    def get_attributes(self, key: str, default: Any = MISSING) -> Any:
-        if default is MISSING:
-            return getattr(g, key)
-        return getattr(g, key, default)
 
     def request_extend(self) -> RequestExtend:
         return RequestExtend(self.request)
 
     def body(self) -> dict:
-        return request.json
+        return _request.json
 
     def cookie(self) -> dict:
-        return request.cookies
+        return _request.cookies
 
-    def file(self) -> Request.files:  # type: ignore
-        return request.files
+    def file(self) -> FlaskRequest.files:  # type: ignore
+        return _request.files
 
-    def form(self) -> Request.form:  # type: ignore
-        return request.form
+    def form(self) -> FlaskRequest.form:  # type: ignore
+        return _request.form
 
     def header(self) -> EnvironHeaders:
-        return request.headers
+        return _request.headers
 
     def path(self) -> Mapping[str, Any]:
         return self.request_kwargs
 
     def query(self) -> Dict[str, Any]:
-        return request.args
+        return _request.args
 
     @LazyProperty()
     def multiform(self) -> Dict[str, List[Any]]:
-        return {key: request.form.getlist(key) for key, _ in request.form.items()}
+        return {key: _request.form.getlist(key) for key, _ in _request.form.items()}
 
     @LazyProperty()
     def multiquery(self) -> Dict[str, List[Any]]:
-        return {key: request.args.getlist(key) for key, _ in request.args.items()}
+        return {key: _request.args.getlist(key) for key, _ in _request.args.items()}
```

### Comparing `pait-0.8.0.2/pait/app/flask/_load_app.py` & `pait-1.0.0a1/pait/app/flask/_load_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import logging
 from typing import Callable, Dict, Set
 
 from flask import Flask
 from flask.views import MethodView
 
 from pait.g import pait_data
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._app_helper import AppHelper
 
 __all__ = ["load_app"]
 
 
-def load_app(app: Flask, project_name: str = "", auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
+def load_app(app: Flask, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`"""
     _pait_data: Dict[str, PaitCoreModel] = {}
-    if not project_name:
-        project_name = app.import_name.split(".")[0]
     for route in app.url_map.iter_rules():
         path: str = route.rule
         method_set: Set[str] = route.methods
         route_name: str = route.endpoint
         endpoint: Callable = app.view_functions[route_name]
         pait_id: str = getattr(endpoint, "_pait_id", "")
         # replace path <xxx> to {xxx}
@@ -48,39 +46,35 @@
             if not view_class_endpoint or not issubclass(view_class_endpoint, MethodView):
                 if auto_load_route:
                     from pait.app.flask import pait
 
                     endpoint = pait()(endpoint)
                     pait_id = getattr(endpoint, "_pait_id")
                     app.view_functions[route_name] = endpoint
-                    pait_data.add_route_info(
-                        AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name, project_name
-                    )
+                    pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name)
                 else:
                     logging.warning(
                         f"loan path:{path} fail, endpoint:{endpoint} not `view_class` attributes"
                     )  # pragma: no cover
                 continue
             for method in view_class_endpoint.methods:
                 method = method.lower()
                 method_set = {method}
-                endpoint = getattr(view_class_endpoint, method, None)
-                if not endpoint:
+                cbv_endpoint = getattr(view_class_endpoint, method, None)
+                if not cbv_endpoint:
                     continue
-                pait_id = getattr(endpoint, "_pait_id", None)
+                pait_id = getattr(cbv_endpoint, "_pait_id", "")
                 if not pait_id:
                     from pait.app.flask import pait
 
-                    endpoint = pait()(endpoint)
+                    endpoint = pait()(cbv_endpoint)
                     pait_id = getattr(endpoint, "_pait_id")
                     setattr(view_class_endpoint, method, endpoint)
 
                 pait_data.add_route_info(
-                    AppHelper.app_name, pait_id, path, openapi_path, method_set, f"{route_name}.{method}", project_name
+                    AppHelper.app_name, pait_id, path, openapi_path, method_set, f"{route_name}.{method}"
                 )
                 _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
         else:
-            pait_data.add_route_info(
-                AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name, project_name
-            )
+            pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name)
         _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
     return _pait_data
```

### Comparing `pait-0.8.0.2/pait/app/flask/_test_helper.py` & `pait-1.0.0a1/pait/app/flask/_test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Mapping, Optional
 
 from flask import Response
 from flask.testing import FlaskClient
 
 from pait.app.base import BaseTestHelper
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._load_app import load_app
 
 __all__ = ["FlaskTestHelper", "TestHelper"]
 
 
 class TestHelper(BaseTestHelper[Response]):
```

### Comparing `pait-0.8.0.2/pait/app/sanic/_app_helper.py` & `pait-1.0.0a1/pait/app/tornado/adapter/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,72 @@
-from dataclasses import MISSING
+import json
 from typing import Any, Dict, List, Mapping
 
-from sanic.headers import HeaderIterable
-from sanic.request import File, Request, RequestParameters
-from sanic.views import CompositionView, HTTPMethodView
-from sanic_testing.testing import SanicTestClient, TestingResponse  # type: ignore
+from tornado.httputil import HTTPHeaders, HTTPServerRequest
 
-from pait.app.base import BaseAppHelper, BaseRequestExtend
+from pait.app.base.adapter.request import BaseRequest, BaseRequestExtend
 from pait.util import LazyProperty
 
-__all__ = ["AppHelper", "RequestExtend"]
 
-
-class RequestExtend(BaseRequestExtend[Request]):
+class RequestExtend(BaseRequestExtend[HTTPServerRequest]):
     @property
     def scheme(self) -> str:
-        return self.request.scheme
+        return self.request.protocol
 
     @property
     def path(self) -> str:
         return self.request.path
 
     @property
     def hostname(self) -> str:
         return self.request.host
 
 
-class AppHelper(BaseAppHelper[Request, RequestExtend]):
-    RequestType = Request
-    FormType = RequestParameters
-    FileType = File
-    HeaderType = HeaderIterable
-    CbvType = (HTTPMethodView, CompositionView)
-    app_name = "sanic"
-
-    def get_attributes(self, key: str, default: Any = MISSING) -> Any:
-        if default is MISSING:
-            return getattr(self.request.app.ctx, key)
-        return getattr(self.request.app.ctx, key, default)
+class Request(BaseRequest[HTTPServerRequest, RequestExtend]):
+    RequestType = HTTPServerRequest
+    FormType = dict
+    FileType = dict
+    HeaderType = dict
 
     def request_extend(self) -> RequestExtend:
         return RequestExtend(self.request)
 
+    @LazyProperty()
     def body(self) -> dict:
-        return self.request.json
+        return json.loads(self.request.body.decode())
 
+    @LazyProperty()
     def cookie(self) -> dict:
-        return self.request.cookies
+        return {i.key: i.value for i in self.request.cookies.values()}
 
-    def file(self) -> Dict[str, File]:
-        return {key: value[0] for key, value in self.request.files.items()}
+    @LazyProperty()
+    def file(self) -> dict:
+        return {item["filename"]: item for item in self.request.files["file"]}
 
+    @LazyProperty()
     def form(self) -> dict:
-        return {key: value[0] for key, value in self.request.form.items()}
+        if self.request.arguments:
+            form_dict: dict = {key: value[0].decode() for key, value in self.request.arguments.items()}
+        else:
+            form_dict = json.loads(self.request.body.decode())  # pragma: no cover
+        return form_dict
 
-    def header(self) -> HeaderIterable:
+    def header(self) -> HTTPHeaders:
         return self.request.headers
 
     def path(self) -> Mapping[str, Any]:
         return self.request_kwargs
 
     @LazyProperty()
     def query(self) -> dict:
-        return {key: value[0] for key, value in self.request.args.items()}
+        return {key: value[0].decode() for key, value in self.request.query_arguments.items()}
 
     @LazyProperty()
     def multiform(self) -> Dict[str, List[Any]]:
-        return {key: self.request.form.getlist(key) for key, _ in self.request.form.items()}
+        if self.request.arguments:
+            return {key: [i.decode() for i in value] for key, value in self.request.arguments.items()}
+        else:
+            return {key: [value] for key, value in json.loads(self.request.body.decode()).items()}  # pragma: no cover
 
     @LazyProperty()
     def multiquery(self) -> Dict[str, Any]:
-        return {key: self.request.args.getlist(key) for key, _ in self.request.args.items()}
+        return {key: [i.decode() for i in value] for key, value in self.request.query_arguments.items()}
```

### Comparing `pait-0.8.0.2/pait/app/sanic/_load_app.py` & `pait-1.0.0a1/pait/app/sanic/_load_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 import logging
 from typing import Callable, Dict, Optional, Set, Type
 
 from sanic.app import Sanic
 from sanic_testing.testing import SanicTestClient, TestingResponse  # type: ignore
 
 from pait.g import pait_data
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._app_helper import AppHelper
 
 __all__ = ["load_app"]
 
 
-def load_app(app: Sanic, project_name: str = "", auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
+def load_app(app: Sanic, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`"""
-    if not project_name:
-        project_name = app.name
     _pait_data: Dict[str, PaitCoreModel] = {}
     for route in app.router.routes:
-        if "static" in route.name:
-            continue
-
         route_name: str = route.name
         method_set: Set[str] = route.methods
         path: str = route.path
         openapi_path: str = path
         handler: Callable = route.handler
 
         # replace path <xxx> to {xxx}
@@ -41,15 +36,15 @@
                 new_path_list.append(real_sub_path)
             openapi_path = "/".join(new_path_list)
         if not openapi_path.startswith("/"):
             openapi_path = "/" + openapi_path
         for method in method_set:
             view_class: Optional[Type] = getattr(handler, "view_class", None)
             if view_class:
-                real_handler: Callable = getattr(view_class, method.lower(), None)
+                real_handler: Optional[Callable] = getattr(view_class, method.lower(), None)
             else:
                 real_handler = handler
             if not real_handler:
                 logging.warning(f"{route_name} can not found handle")  # pragma: no cover
                 continue
             pait_id: str = getattr(real_handler, "_pait_id", "")
             if not pait_id:
@@ -63,17 +58,15 @@
                         setattr(view_class, method.lower(), real_handler)
                     else:
                         route.handler = real_handler
                 else:
                     logging.warning(f"{route_name} can not found pait id")  # pragma: no cover
                     continue
 
-            pait_data.add_route_info(
-                AppHelper.app_name, pait_id, path, openapi_path, {method}, route_name, project_name
-            )
+            pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, {method}, route_name)
             _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
 
         # old version
         # for path, handler_dict in route.handlers.items():
         #     for method, handler_list in handler_dict.items():
         #         for handler in handler_list:
         #             view_class: Optional[Type] = getattr(handler, "view_class", None)
```

### Comparing `pait-0.8.0.2/pait/app/sanic/_test_helper.py` & `pait-1.0.0a1/pait/app/sanic/_test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, Mapping, Optional
 
 from sanic_testing.testing import SanicTestClient, TestingResponse  # type: ignore
 
 from pait.app.base import BaseTestHelper
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._load_app import load_app
 
 __all__ = ["SanicTestHelper", "TestHelper"]
 
 
 class TestHelper(BaseTestHelper[TestingResponse]):
```

### Comparing `pait-0.8.0.2/pait/app/sanic/plugin/auto_complete_json_resp.py` & `pait-1.0.0a1/pait/app/sanic/plugin/auto_complete_json_resp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Any
 
 from pait.plugin.auto_complete_json_resp import AutoCompleteJsonRespPlugin as _AutoCompleteJsonRespPlugin
+from pait.plugin.base import PluginContext
 
-from .base import JsonProtocol
+from .unified_response import UnifiedResponsePluginProtocol
 
-__all__ = ["AsyncAutoCompleteJsonRespPlugin", "AutoCompleteJsonRespPlugin"]
+__all__ = ["AutoCompleteJsonRespPlugin"]
 
 
-class AutoCompleteJsonRespPlugin(JsonProtocol, _AutoCompleteJsonRespPlugin):
-    async def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        response: Any = await super(AutoCompleteJsonRespPlugin, self).__call__(*args, **kwargs)
-        return self.gen_response(response)
+class AutoCompleteJsonRespPlugin(UnifiedResponsePluginProtocol, _AutoCompleteJsonRespPlugin):
+    def _sync_call(self, context: PluginContext) -> Any:
+        response: Any = super()._sync_call(context)
+        return self._gen_response(response, context)
 
-
-class AsyncAutoCompleteJsonRespPlugin(AutoCompleteJsonRespPlugin):
-    """"""
+    async def _async_call(self, context: PluginContext) -> Any:
+        response: Any = await super()._async_call(context)
+        return self._gen_response(response, context)
```

### Comparing `pait-0.8.0.2/pait/app/sanic/plugin/mock_response.py` & `pait-1.0.0a1/pait/app/sanic/plugin/mock_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-from typing import Any, AsyncContextManager
+from typing import Any
 
 import aiofiles  # type: ignore
 from sanic import response as sanic_response
-from sanic.response import json as resp_json
 from sanic_testing.testing import SanicTestClient, TestingResponse  # type: ignore
 
-from pait.model import response
-from pait.plugin.base_mock_response import BaseAsyncMockPlugin
+from pait.app.sanic.adapter.response import gen_response, set_info_to_response
+from pait.plugin.mock_response import MockPluginProtocol
 
 
-class MockPlugin(BaseAsyncMockPlugin):
-    def mock_response(self) -> Any:
-        async def make_mock_response() -> sanic_response.BaseHTTPResponse:
-            if issubclass(self.pait_response_model, response.PaitJsonResponseModel):
-                resp: sanic_response.BaseHTTPResponse = resp_json(self.pait_response_model.get_example_value())
-            elif issubclass(self.pait_response_model, response.PaitTextResponseModel) or issubclass(
-                self.pait_response_model, response.PaitHtmlResponseModel
-            ):
-                resp = sanic_response.text(
-                    self.pait_response_model.get_example_value(), content_type=self.pait_response_model.media_type
-                )
-            elif issubclass(self.pait_response_model, response.PaitFileResponseModel):
-                named_temporary_file: AsyncContextManager = aiofiles.tempfile.NamedTemporaryFile()  # type: ignore
-                f: Any = await named_temporary_file.__aenter__()
-                await f.write(self.pait_response_model.get_example_value())
-                await f.seek(0)
-                resp = await sanic_response.file_stream(f.name, mime_type=self.pait_response_model.media_type)
-
-                raw_streaming_fn = resp.streaming_fn
-
-                async def _streaming_fn(_response: sanic_response.BaseHTTPResponse) -> None:
-                    await raw_streaming_fn(_response)
-                    await named_temporary_file.__aexit__(None, None, None)
-
-                resp.streaming_fn = _streaming_fn
-            else:
-                raise NotImplementedError(f"make_mock_response not support {self.pait_response_model}")
-            resp.status = self.pait_response_model.status_code[0]
-            if self.pait_response_model.header:
-                resp.headers.update(self.pait_response_model.header)
-            return resp
+class MockPlugin(MockPluginProtocol[sanic_response.BaseHTTPResponse]):
+    def get_response(self) -> sanic_response.BaseHTTPResponse:
+        return gen_response(
+            self.pait_response_model.get_example_value(example_column_name=self.example_column_name),
+            self.pait_response_model,
+        )
 
-        return make_mock_response()
+    async def async_get_file_response(self, temporary_file: Any, f: Any) -> sanic_response.BaseHTTPResponse:
+        await f.write(self.pait_response_model.get_example_value(example_column_name=self.example_column_name))
+        await f.seek(0)
+        resp = await sanic_response.file_stream(f.name, mime_type=self.pait_response_model.media_type)
 
+        raw_streaming_fn = resp.streaming_fn
 
-class AsyncMockPlugin(MockPlugin):
-    """"""
+        async def _streaming_fn(_response: sanic_response.BaseHTTPResponse) -> None:
+            await raw_streaming_fn(_response)
+            await temporary_file.__aexit__(None, None, None)
+
+        resp.streaming_fn = _streaming_fn
+        return resp
+
+    def set_info_to_response(self, resp: sanic_response.BaseHTTPResponse) -> None:
+        set_info_to_response(resp, self.pait_response_model)
```

### Comparing `pait-0.8.0.2/pait/app/starlette/_app_helper.py` & `pait-1.0.0a1/pait/app/starlette/adapter/request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from dataclasses import MISSING
 from typing import Any, Coroutine, Dict, List, Mapping, Optional
 
 from starlette.datastructures import FormData, Headers, UploadFile
-from starlette.endpoints import HTTPEndpoint
-from starlette.requests import Request
+from starlette.requests import Request as _Request
 
-from pait.app.base import BaseAppHelper, BaseRequestExtend
+from pait.app.base.adapter.request import BaseRequest, BaseRequestExtend
 from pait.util import LazyProperty
 
-__all__ = ["AppHelper", "RequestExtend"]
 
-
-class RequestExtend(BaseRequestExtend[Request]):
+class RequestExtend(BaseRequestExtend[_Request]):
     @property
     def scheme(self) -> str:
         return self.request.url.scheme
 
     @property
     def path(self) -> str:
         return self.request.url.path
@@ -23,32 +19,24 @@
     @property
     def hostname(self) -> str:
         if self.request.url.port:
             return f"{self.request.url.hostname}:{self.request.url.port}"
         return self.request.url.hostname
 
 
-class AppHelper(BaseAppHelper[Request, RequestExtend]):
-    RequestType = Request
+class Request(BaseRequest[_Request, RequestExtend]):
+    RequestType = _Request
     FormType = FormData
     FileType = UploadFile
     HeaderType = Headers
-    CbvType = (HTTPEndpoint,)
-    app_name = "starlette"
 
-    def __init__(self, args: List[Any], kwargs: Mapping[str, Any]):
-        super().__init__(args, kwargs)
+    def __init__(self, request: _Request, args: List[Any], kwargs: Mapping[str, Any]):
+        super().__init__(request, args, kwargs)
         self._form: Optional[FormData] = None
 
-    def get_attributes(self, key: str, default: Any = MISSING) -> Any:
-        if default is MISSING:
-            return getattr(self.request.app.state, key)
-        else:
-            return getattr(self.request.app.state, key, default)
-
     def request_extend(self) -> RequestExtend:
         return RequestExtend(self.request)
 
     def body(self) -> Coroutine[Any, Any, dict]:
         return self.request.json()
 
     def cookie(self) -> dict:
```

### Comparing `pait-0.8.0.2/pait/app/starlette/_load_app.py` & `pait-1.0.0a1/pait/app/starlette/_load_app.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 from typing import Callable, Dict, Optional, Type, Union
 
 from starlette import routing
 from starlette.applications import Starlette
 from starlette.endpoints import HTTPEndpoint
 
 from pait.g import pait_data
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 from pait.util import http_method_tuple
 
 from ._app_helper import AppHelper
 
 __all__ = ["load_app"]
 
 
 def _load_route(
     *,
     route: routing.Route,
     _pait_data: Dict[str, PaitCoreModel],
-    project_name: str,
     prefix_path: Optional[str] = None,
     auto_load_route: bool = False,
 ) -> None:
     path: str = route.path
     if prefix_path:
         path = prefix_path + path
     openapi_path: str = path
@@ -34,33 +33,32 @@
     pait_id: str = getattr(route.endpoint, "_pait_id", "")
     if not pait_id and inspect.isclass(endpoint) and issubclass(endpoint, HTTPEndpoint):  # type: ignore
         for method in http_method_tuple:
             method_endpoint = getattr(endpoint, method, None)
             if not method_endpoint:
                 continue
             method_set = {method}
-            pait_id = getattr(method_endpoint, "_pait_id", None)
+            pait_id = getattr(method_endpoint, "_pait_id", "")
             if not pait_id:
                 if not auto_load_route:
                     logging.warning(f"{route_name}.{method} can not found pait id")  # pragma: no cover
                 from pait.app.starlette import pait
 
                 method_endpoint = pait()(method_endpoint)
-                pait_id = getattr(method_endpoint, "_pait_id", None)
+                pait_id = getattr(method_endpoint, "_pait_id", "")
                 setattr(endpoint, method, method_endpoint)
 
             pait_data.add_route_info(
-                AppHelper.app_name, pait_id, path, openapi_path, method_set, f"{route_name}.{method}", project_name
+                AppHelper.app_name, pait_id, path, openapi_path, method_set, f"{route_name}.{method}"
             )
             _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
     elif pait_id:
-        pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name, project_name)
+        pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name)
         _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
     elif auto_load_route:
-
         from pait.app.starlette import pait
 
         endpoint = pait()(endpoint)
         pait_id = getattr(endpoint, "_pait_id", "")
 
         route.endpoint = endpoint
         endpoint_handler = endpoint
@@ -69,32 +67,31 @@
         if inspect.isfunction(endpoint_handler) or inspect.ismethod(endpoint_handler):
             # Endpoint is function or method. Treat it as `func(request) -> response`.
             route.app = routing.request_response(endpoint)
         else:
             # Endpoint is a class. Treat it as ASGI.
             route.app = endpoint
 
-        pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name, project_name)
+        pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, method_set, route_name)
         _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
     else:
         logging.warning(f"{route_name} can not found pait id")  # pragma: no cover
 
 
-def load_app(app: Starlette, project_name: str = "", auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
+def load_app(app: Starlette, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`"""
     _pait_data: Dict[str, PaitCoreModel] = {}
     for route in app.routes:
         if isinstance(route, routing.Route):
-            _load_route(route=route, _pait_data=_pait_data, project_name=project_name, auto_load_route=auto_load_route)
+            _load_route(route=route, _pait_data=_pait_data, auto_load_route=auto_load_route)
         elif isinstance(route, routing.Mount):
             for sub_route in route.routes:
                 _load_route(
                     route=sub_route,  # type: ignore
                     _pait_data=_pait_data,
-                    project_name=project_name,
                     prefix_path=route.path,
                     auto_load_route=auto_load_route,
                 )
         else:
             logging.info(f"load_app func not support route:{route.__class__}")
 
     return _pait_data
```

### Comparing `pait-0.8.0.2/pait/app/starlette/_test_helper.py` & `pait-1.0.0a1/pait/app/starlette/_test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Mapping, Optional
 
 from requests import Response as _Response  # type: ignore
 from starlette.testclient import TestClient
 
 from pait.app.base import BaseTestHelper
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._load_app import load_app
 
 __all__ = ["StarletteTestHelper", "TestHelper"]
 
 
 class TestHelper(BaseTestHelper[_Response]):
```

### Comparing `pait-0.8.0.2/pait/app/starlette/plugin/auto_complete_json_resp.py` & `pait-1.0.0a1/pait/app/starlette/plugin/auto_complete_json_resp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Any
 
 from pait.plugin.auto_complete_json_resp import AutoCompleteJsonRespPlugin as _AutoCompleteJsonRespPlugin
+from pait.plugin.base import PluginContext
 
-from .base import JsonProtocol
+from .unified_response import UnifiedResponsePluginProtocol
 
-__all__ = ["AutoCompleteJsonRespPlugin", "AsyncAutoCompleteJsonRespPlugin"]
+__all__ = ["AutoCompleteJsonRespPlugin"]
 
 
-class AutoCompleteJsonRespPlugin(JsonProtocol, _AutoCompleteJsonRespPlugin):
-    def _sync_call(self, *args: Any, **kwargs: Any) -> Any:
-        response: Any = super()._sync_call(*args, **kwargs)
-        return self.gen_response(response)
+class AutoCompleteJsonRespPlugin(UnifiedResponsePluginProtocol, _AutoCompleteJsonRespPlugin):
+    def _sync_call(self, context: PluginContext) -> Any:
+        response: Any = super()._sync_call(context)
+        return self._gen_response(response, context)
 
-    async def _async_call(self, *args: Any, **kwargs: Any) -> Any:
-        response: Any = await super()._async_call(*args, **kwargs)
-        return self.gen_response(response)
-
-
-class AsyncAutoCompleteJsonRespPlugin(AutoCompleteJsonRespPlugin):
-    """"""
+    async def _async_call(self, context: PluginContext) -> Any:
+        response: Any = await super()._async_call(context)
+        return self._gen_response(response, context)
```

### Comparing `pait-0.8.0.2/pait/app/tornado/_load_app.py` & `pait-1.0.0a1/pait/app/tornado/_load_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 from typing import Callable, Dict, Optional
 
-from tornado.web import Application
+from tornado.web import Application, RequestHandler
 
 from pait.g import pait_data
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._app_helper import AppHelper
 
 __all__ = ["load_app"]
 
 
-def load_app(app: Application, project_name: str = "", auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
+def load_app(app: Application, auto_load_route: bool = False) -> Dict[str, PaitCoreModel]:
     """Read data from the route that has been registered to `pait`"""
     _pait_data: Dict[str, PaitCoreModel] = {}
     for rule in app.wildcard_router.rules:
         path: str = rule.matcher.regex.pattern  # type: ignore
         openapi_path: str = path
         # replace path regex to {xxx}
         if "<" in openapi_path and ">" in openapi_path:
@@ -37,23 +37,23 @@
         if openapi_path.endswith("$"):
             openapi_path = openapi_path[:-1]
         base_name: str = rule.target.__name__
         for method in ["get", "post", "head", "options", "delete", "put", "trace", "patch"]:
             handler: Optional[Callable] = getattr(rule.target, method, None)
             if not handler:
                 continue
+            if handler is RequestHandler._unimplemented_method:
+                continue
             route_name: str = f"{base_name}.{method}"
             pait_id: str = getattr(handler, "_pait_id", "")
             if not pait_id:
                 if auto_load_route:
                     from pait.app.tornado import pait
 
                     handler = pait()(handler)
-                    pait_id = getattr(handler, "_pait_id", None)
+                    pait_id = getattr(handler, "_pait_id")
                     setattr(rule.target, method, handler)
                 else:
                     logging.warning(f"{route_name} can not found pait id")  # pragma: no cover
-            pait_data.add_route_info(
-                AppHelper.app_name, pait_id, path, openapi_path, {method}, route_name, project_name
-            )
+            pait_data.add_route_info(AppHelper.app_name, pait_id, path, openapi_path, {method}, route_name)
             _pait_data[pait_id] = pait_data.get_pait_data(AppHelper.app_name, pait_id)
     return _pait_data
```

### Comparing `pait-0.8.0.2/pait/app/tornado/_test_helper.py` & `pait-1.0.0a1/pait/app/tornado/_test_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from io import BytesIO
 from typing import Dict, Mapping, Optional, Tuple
 
 from tornado.testing import AsyncHTTPTestCase, HTTPResponse
 
 from pait.app.base import BaseTestHelper
-from pait.model.core import PaitCoreModel
+from pait.model import PaitCoreModel
 
 from ._load_app import load_app
 
 __all__ = ["TornadoTestHelper", "TestHelper"]
 
 
 class TestHelper(BaseTestHelper[HTTPResponse]):
```

### Comparing `pait-0.8.0.2/pait/app/tornado/plugin/auto_complete_json_resp.py` & `pait-1.0.0a1/pait/app/tornado/plugin/auto_complete_json_resp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from typing import Any
 
-from tornado.web import RequestHandler
-
 from pait.plugin.auto_complete_json_resp import AutoCompleteJsonRespPlugin as _AutoCompleteJsonRespPlugin
+from pait.plugin.base import PluginContext
 
-from .base import JsonProtocol
-
-__all__ = ["AsyncAutoCompleteJsonRespPlugin", "AutoCompleteJsonRespPlugin"]
-
+from .unified_response import UnifiedResponsePluginProtocol
 
-class AutoCompleteJsonRespPlugin(JsonProtocol, _AutoCompleteJsonRespPlugin):
-    async def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        response: Any = await super(AutoCompleteJsonRespPlugin, self).__call__(*args, **kwargs)
-        tornado_handle: RequestHandler = args[0]
-        return self.gen_response(tornado_handle, response)
+__all__ = ["AutoCompleteJsonRespPlugin"]
 
 
-class AsyncAutoCompleteJsonRespPlugin(AutoCompleteJsonRespPlugin):
-    """"""
+class AutoCompleteJsonRespPlugin(UnifiedResponsePluginProtocol, _AutoCompleteJsonRespPlugin):
+    async def __call__(self, context: PluginContext) -> Any:
+        response: Any = await super(AutoCompleteJsonRespPlugin, self).__call__(context)
+        return self._gen_response(response, context)
```

### Comparing `pait-0.8.0.2/pait/app/tornado/plugin/cache_resonse.py` & `pait-1.0.0a1/pait/app/tornado/plugin/cache_response.py`

 * *Files identical despite different names*

### Comparing `pait-0.8.0.2/pait/app/tornado/plugin/mock_response.py` & `pait-1.0.0a1/pait/app/tornado/plugin/mock_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 from typing import Any
 
 import aiofiles  # type: ignore
 from tornado.web import RequestHandler
 
-from pait.model import response
-from pait.plugin.base_mock_response import BaseMockPlugin
+from pait.app.tornado.adapter.response import gen_response, set_info_to_response
+from pait.plugin.base import PluginContext
+from pait.plugin.mock_response import MockPluginProtocol
 
 
-class MockPlugin(BaseMockPlugin):
+class MockPlugin(MockPluginProtocol[None]):
     tornado_handle: RequestHandler
 
-    def mock_response(self) -> Any:
-        async def make_mock_response() -> Any:
-            self.tornado_handle.set_status(self.pait_response_model.status_code[0])
-            for key, value in self.pait_response_model.header.items():
-                self.tornado_handle.set_header(key, value)
-            self.tornado_handle.set_header("Content-Type", self.pait_response_model.media_type)
-            if issubclass(self.pait_response_model, response.PaitJsonResponseModel):
-                self.tornado_handle.write(self.pait_response_model.get_example_value())
-            elif issubclass(self.pait_response_model, response.PaitTextResponseModel) or issubclass(
-                self.pait_response_model, response.PaitHtmlResponseModel
-            ):
-                self.tornado_handle.write(self.pait_response_model.get_example_value())
-            elif issubclass(self.pait_response_model, response.PaitFileResponseModel):
-                async with aiofiles.tempfile.NamedTemporaryFile() as f:  # type: ignore
-                    await f.write(self.pait_response_model.get_example_value())
-                    await f.seek(0)
-                    async for line in f:
-                        self.tornado_handle.write(line)
-            else:
-                raise NotImplementedError()
-
-        return make_mock_response()
-
-    async def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        self.tornado_handle = args[0]
-        await super().__call__(args, kwargs)
-
-
-class AsyncMockPlugin(MockPlugin):
-    """"""
+    def get_response(self) -> None:
+        return gen_response(
+            self.pait_response_model.get_example_value(example_column_name=self.example_column_name),
+            self.pait_response_model,
+            self.tornado_handle,
+        )
+
+    def set_info_to_response(self, resp: None) -> None:
+        set_info_to_response(self.tornado_handle, self.pait_response_model)
+
+    async def async_get_file_response(self, temporary_file: Any, f: Any) -> None:
+        await f.write(self.pait_response_model.get_example_value(example_column_name=self.example_column_name))
+        await f.seek(0)
+        async for line in f:
+            self.tornado_handle.write(line)
+        await temporary_file.__aexit__(None, None, None)
+
+    async def __call__(self, context: PluginContext) -> Any:
+        self.tornado_handle = context.args[0]
+        await super().__call__(context)
```

### Comparing `pait-0.8.0.2/pait/core.py` & `pait-1.0.0a1/pait/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 import inspect
-import logging
 from functools import wraps
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, TypeVar
 
-from pydantic import BaseConfig
+from pydantic import BaseConfig, BaseModel
 
 from pait.app.base import BaseAppHelper
 from pait.extra.util import sync_config_data_to_pait_core_model
+from pait.field import BaseField
 from pait.g import config, pait_context, pait_data
-from pait.model.core import ContextModel, PaitCoreModel
-from pait.model.response import PaitBaseResponseModel
-from pait.model.status import PaitStatus
-from pait.model.tag import Tag
-from pait.plugin.base import PluginManager, PluginProtocol
+from pait.model import BaseResponseModel, ContextModel, PaitCoreModel, PaitStatus, Tag
+from pait.param_handle import AsyncParamHandler, ParamHandler
+from pait.plugin.base import PluginManager, PluginProtocol, PostPluginProtocol, PrePluginProtocol
 from pait.util import get_func_sig
 
 if TYPE_CHECKING:
     from param_handle import BaseParamHandler
 _AppendT = TypeVar("_AppendT", list, tuple)
 _PaitT = TypeVar("_PaitT", bound="Pait")
 _PluginT = TypeVar("_PluginT", bound="PluginProtocol")
-TagT = Union[str, Tag]
 
 
 class Pait(object):
     app_helper_class: "Type[BaseAppHelper]"
+    param_handler_plugin_class: Type[ParamHandler] = ParamHandler
+    async_param_handler_plugin_class: Type[AsyncParamHandler] = AsyncParamHandler
 
     def __init__(
-        self,
+        self: "_PaitT",
         pydantic_model_config: Optional[Type[BaseConfig]] = None,
+        pydantic_basemodel: Optional[Type[BaseModel]] = None,
+        default_field_class: Optional[Type[BaseField]] = None,
         # param check
         pre_depend_list: Optional[List[Callable]] = None,
         # doc
         author: Optional[Tuple[str, ...]] = None,
         desc: Optional[str] = None,
         summary: Optional[str] = None,
         name: Optional[str] = None,
         status: Optional[PaitStatus] = None,
         group: Optional[str] = None,
-        tag: Optional[Tuple[TagT, ...]] = None,
-        response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
+        tag: Optional[Tuple[Tag, ...]] = None,
+        response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
         # plugin
-        plugin_list: Optional[List[PluginManager]] = None,
-        post_plugin_list: Optional[List[PluginManager]] = None,
+        plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+        post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
         param_handler_plugin: Optional[Type["BaseParamHandler"]] = None,
+        **kwargs: Any,
     ):
         """
         :param pydantic_model_config: pydantic.BaseConfig
+        :param pydantic_basemodel: pydantic.BaseModel
+        :param default_field_class: pait.field.BaseField
         :param pre_depend_list:  List of depend functions to execute before route functions
         :param author:  The author who wrote this routing function
         :param desc:  Description of the routing function
         :param summary:  Introduction to Routing Functions
         :param name:  The name of the routing function, defaults to the function name
         :param status:  The state of the routing function
         :param group:  The group to which the routing function belongs
@@ -71,68 +75,85 @@
         if not isinstance(self.app_helper_class, type):
             raise TypeError(f"{self.app_helper_class} must be class")
         if not issubclass(self.app_helper_class, BaseAppHelper):
             raise TypeError(f"{self.app_helper_class} must sub from {BaseAppHelper.__class__.__name__}")
 
         # Note: pydantic not check field.default value when config.validate_all = False
         # See issue: https://github.com/samuelcolvin/pydantic/issues/1280
-        self._pydantic_model_config: Type[BaseConfig] = pydantic_model_config or BaseConfig
+        self._pydantic_model_config: Optional[Type[BaseConfig]] = pydantic_model_config
+        self._pydantic_basemodel: Optional[Type[BaseModel]] = pydantic_basemodel
+        self._default_field_class: Optional[Type[BaseField]] = default_field_class
         # param check
         self._pre_depend_list: Optional[List[Callable]] = pre_depend_list
         # doc
         self._author: Optional[Tuple[str, ...]] = author
         self._desc: Optional[str] = desc
         self._summary: Optional[str] = summary
         self._name: Optional[str] = name
         self._status: Optional[PaitStatus] = status
         self._group: Optional[str] = group
-        self._tag: Optional[Tuple[TagT, ...]] = tag
-        self._response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = response_model_list
+        self._tag: Optional[Tuple[Tag, ...]] = tag
+        self._response_model_list: Optional[List[Type[BaseResponseModel]]] = response_model_list
         # plugin
-        self._plugin_list: Optional[List[PluginManager]] = plugin_list
-        self._post_plugin_list: Optional[List[PluginManager]] = post_plugin_list
+        self._plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = plugin_list
+        self._post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = post_plugin_list
         self._param_handler_plugin: Optional[Type["BaseParamHandler"]] = param_handler_plugin
+        self.extra: dict = kwargs
 
     @staticmethod
     def _append_data(
+        key: str,
         target_container: Optional[_AppendT],
         append_container: Optional[_AppendT],
         self_container: Optional[_AppendT],
     ) -> Optional[_AppendT]:
+        if target_container and append_container:
+            raise KeyError(f"{key} and append_{key} cannot be used together")
         if append_container:
             return (self_container or append_container.__class__()) + append_container
+        elif target_container is None:
+            return self_container
         else:
-            return target_container or self_container
+            return target_container
+
+    @property
+    def response_model_list(self) -> List[Type[BaseResponseModel]]:
+        return self._response_model_list or []
 
     def create_sub_pait(
-        self: _PaitT,
+        self: "_PaitT",
         pydantic_model_config: Optional[Type[BaseConfig]] = None,
+        pydantic_basemodel: Optional[Type[BaseModel]] = None,
+        default_field_class: Optional[Type[BaseField]] = None,
         # param check
         pre_depend_list: Optional[List[Callable]] = None,
         append_pre_depend_list: Optional[List[Callable]] = None,
         # doc
         author: Optional[Tuple[str, ...]] = None,
         append_author: Optional[Tuple[str, ...]] = None,
         desc: Optional[str] = None,
         summary: Optional[str] = None,
         name: Optional[str] = None,
         status: Optional[PaitStatus] = None,
         group: Optional[str] = None,
-        tag: Optional[Tuple[TagT, ...]] = None,
-        append_tag: Optional[Tuple[TagT, ...]] = None,
-        response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
-        append_response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
-        plugin_list: Optional[List[PluginManager]] = None,
-        append_plugin_list: Optional[List[PluginManager]] = None,
-        post_plugin_list: Optional[List[PluginManager]] = None,
-        append_post_plugin_list: Optional[List[PluginManager]] = None,
+        tag: Optional[Tuple[Tag, ...]] = None,
+        append_tag: Optional[Tuple[Tag, ...]] = None,
+        response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
+        append_response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
+        plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+        append_plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+        post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
+        append_post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
         param_handler_plugin: Optional[Type["BaseParamHandler"]] = None,
+        **kwargs: Any,
     ) -> _PaitT:
         """
         :param pydantic_model_config: pydantic.BaseConfig
+        :param pydantic_basemodel: pydantic.BaseModel
+        :param default_field_class: pait.field.BaseField
         :param pre_depend_list:  List of depend functions to execute before route functions(
             Do not use the pre depend value specified when Pait is initialized)
         :param append_pre_depend_list: Append some author when creating child Pait
         :param author:  The author who wrote this routing function(
             Do not use the author value specified when Pait is initialized)
         :param append_author: Append some author when creating child Pait
         :param desc:  Description of the routing function
@@ -151,91 +172,93 @@
         :param append_plugin_list: Append some pre plugin when creating child Pait
         :param post_plugin_list: post plugin list for routing functions(
             Do not use the post plugin value specified when Pait is initialized)
         :param append_post_plugin_list:  Append some post plugin when creating child Pait
         :param param_handler_plugin: The param handler plugin of the routing function,
          the default is pait.param_handler.x
         """
-        pre_depend_list = self._append_data(pre_depend_list, append_pre_depend_list, self._pre_depend_list)
-        author = self._append_data(author, append_author, self._author)
-        tag = self._append_data(tag, append_tag, self._tag)
+        pre_depend_list = self._append_data(
+            "pre_depend_list", pre_depend_list, append_pre_depend_list, self._pre_depend_list
+        )
+        author = self._append_data("author", author, append_author, self._author)
+        tag = self._append_data("tag", tag, append_tag, self._tag)
         response_model_list = self._append_data(
-            response_model_list, append_response_model_list, self._response_model_list
+            "response_model_list", response_model_list, append_response_model_list, self._response_model_list
+        )
+        plugin_list = self._append_data("plugin_list", plugin_list, append_plugin_list, self._plugin_list)
+        post_plugin_list = self._append_data(
+            "post_plugin_list", post_plugin_list, append_post_plugin_list, self._post_plugin_list
         )
-        plugin_list = self._append_data(plugin_list, append_plugin_list, self._plugin_list)
-        post_plugin_list = self._append_data(post_plugin_list, append_post_plugin_list, self._post_plugin_list)
 
         return self.__class__(
             pydantic_model_config=pydantic_model_config or self._pydantic_model_config,
+            pydantic_basemodel=pydantic_basemodel or self._pydantic_basemodel,
+            default_field_class=default_field_class or self._default_field_class,
             desc=desc or self._desc,
             summary=summary or self._summary,
             name=name or self._name,
             status=status or self._status,
             pre_depend_list=pre_depend_list,
             author=author,
             group=group,
             tag=tag,
             response_model_list=response_model_list,
             plugin_list=plugin_list,
             post_plugin_list=post_plugin_list,
             param_handler_plugin=param_handler_plugin or self._param_handler_plugin,
+            **(kwargs or self.extra),
         )
 
     @staticmethod
-    def _plugin_manager_handler(
-        pait_core_model: PaitCoreModel,
-        args: Any,
-        kwargs: Any,
-    ) -> List[_PluginT]:
-        plugin_instance_list: List[_PluginT] = []
-
-        pre_plugin: Callable = pait_core_model.func
-        for plugin_manager in pait_core_model.plugin_list:
-            plugin_instance: _PluginT = plugin_manager.get_plugin()
-            plugin_instance.__post_init__(pait_core_model, args, kwargs)
-            plugin_instance.call_next = pre_plugin  # type: ignore
-            pre_plugin = plugin_instance
-            plugin_instance_list.append(plugin_instance)
-        plugin_instance_list.reverse()
-        return plugin_instance_list
-
-    @staticmethod
-    def init_context(pait_core_model: "PaitCoreModel", args: Any, kwargs: Any) -> None:
+    def init_context(pait_core_model: "PaitCoreModel", args: Any, kwargs: Any) -> ContextModel:
         """Inject App Helper into context"""
         app_helper: BaseAppHelper = pait_core_model.app_helper_class(args, kwargs)
-        pait_context.set(ContextModel(cbv_instance=app_helper.cbv_instance, app_helper=app_helper))
+        context: ContextModel = ContextModel(
+            cbv_instance=app_helper.cbv_instance,
+            app_helper=app_helper,
+            pait_core_model=pait_core_model,
+            args=args,
+            kwargs=kwargs,
+        )
+        pait_context.set(context)
+        return context
 
     def __call__(
-        self,
+        self: "_PaitT",
         pydantic_model_config: Optional[Type[BaseConfig]] = None,
+        pydantic_basemodel: Optional[Type[BaseModel]] = None,
+        default_field_class: Optional[Type[BaseField]] = None,
         # param check
         pre_depend_list: Optional[List[Callable]] = None,
         append_pre_depend_list: Optional[List[Callable]] = None,
         # doc
         author: Optional[Tuple[str, ...]] = None,
         append_author: Optional[Tuple[str, ...]] = None,
         desc: Optional[str] = None,
         summary: Optional[str] = None,
         name: Optional[str] = None,
         status: Optional[PaitStatus] = None,
         group: Optional[str] = None,
-        tag: Optional[Tuple[TagT, ...]] = None,
-        append_tag: Optional[Tuple[TagT, ...]] = None,
-        response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
-        append_response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
+        tag: Optional[Tuple[Tag, ...]] = None,
+        append_tag: Optional[Tuple[Tag, ...]] = None,
+        response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
+        append_response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
         # plugin
-        plugin_list: Optional[List[PluginManager]] = None,
-        append_plugin_list: Optional[List[PluginManager]] = None,
-        post_plugin_list: Optional[List[PluginManager]] = None,
-        append_post_plugin_list: Optional[List[PluginManager]] = None,
+        plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+        append_plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+        post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
+        append_post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
         param_handler_plugin: Optional[Type["BaseParamHandler"]] = None,
         feature_code: str = "",
+        **kwargs: Any,
     ) -> Callable:
         """
         :param pydantic_model_config: pydantic.BaseConfig
+        :param pydantic_basemodel: pydantic.BaseModel
+        :param default_field_class: pait.field.BaseField
         :param pre_depend_list:  List of depend functions to execute before route functions
         :param author:  The author who wrote this routing function
         :param desc:  Description of the routing function
         :param summary:  Introduction to Routing Functions
         :param name:  The name of the routing function, defaults to the function name
         :param status:  The state of the routing function
         :param group:  The group to which the routing function belongs
@@ -256,79 +279,79 @@
         :param feature_code: Specify the prefix of the pait id corresponding to the generated routing function.
             Usually, the pait_id is equal to md5(func), but during dynamic generation,
             there may be multiple different routing functions generated by the same func.
             In this case, different feature_code is needed to generate different pait_id(feature_code + md5(func))
         """
         app_name: str = self.app_helper_class.app_name
         pydantic_model_config = pydantic_model_config or self._pydantic_model_config
+        pydantic_basemodel = pydantic_basemodel or self._pydantic_basemodel
         desc = desc or self._desc
         summary = summary or self._summary
         name = name or self._name
         group = group or self._group
 
-        pre_depend_list = self._append_data(pre_depend_list, append_pre_depend_list, self._pre_depend_list)
-        author = self._append_data(author, append_author, self._author)
-        tag = self._append_data(tag, append_tag, self._tag)
+        pre_depend_list = self._append_data(
+            "pre_depend_list", pre_depend_list, append_pre_depend_list, self._pre_depend_list
+        )
+        author = self._append_data("author", author, append_author, self._author)
+        tag = self._append_data("tag", tag, append_tag, self._tag)
         response_model_list = self._append_data(
-            response_model_list, append_response_model_list, self._response_model_list
+            "response_model_list", response_model_list, append_response_model_list, self._response_model_list
+        )
+        plugin_list = self._append_data("plugin_list", plugin_list, append_plugin_list, self._plugin_list)
+        post_plugin_list = self._append_data(
+            "post_plugin_list", post_plugin_list, append_post_plugin_list, self._post_plugin_list
         )
-        plugin_list = self._append_data(plugin_list, append_plugin_list, self._plugin_list)
-        post_plugin_list = self._append_data(post_plugin_list, append_post_plugin_list, self._post_plugin_list)
-
-        ###############
-        # tag handler #
-        ###############
-        new_tag: List[str] = []
-        if tag:
-            for _tag in tag:
-                if isinstance(_tag, Tag):
-                    _tag = _tag.name
-                else:
-                    logging.warning(
-                        "In later versions tag only supports Tag class, and does not support str type"
-                    )  # pragma: no cover
-                new_tag.append(_tag)
 
         def wrapper(func: Callable) -> Callable:
             # Pre-parsing function signatures
             get_func_sig(func)
+
+            # load param handler plugin
+            _param_handler_plugin = param_handler_plugin or self._param_handler_plugin
+            if _param_handler_plugin is None:
+                if inspect.iscoroutinefunction(func):
+                    _param_handler_plugin = self.async_param_handler_plugin_class
+                else:
+                    _param_handler_plugin = self.param_handler_plugin_class
             # gen pait core model and register to pait data
             pait_core_model: PaitCoreModel = PaitCoreModel(
+                func,
+                self.app_helper_class,
                 author=author,
-                app_helper_class=self.app_helper_class,
                 desc=desc,
                 summary=summary,
-                func=func,
                 func_name=name,
                 status=status,
                 group=group,
-                tag=tuple(new_tag),
+                tag=tag,
                 response_model_list=response_model_list,
                 pre_depend_list=pre_depend_list,
                 pydantic_model_config=pydantic_model_config,
+                pydantic_basemodel=pydantic_basemodel,
                 plugin_list=plugin_list,
                 post_plugin_list=post_plugin_list,
-                param_handler_plugin=param_handler_plugin or self._param_handler_plugin,
+                param_handler_plugin=_param_handler_plugin,
                 feature_code=feature_code,
+                default_field_class=default_field_class or self._default_field_class,
+                **(kwargs or self.extra),
             )
             sync_config_data_to_pait_core_model(config, pait_core_model)
             pait_data.register(app_name, pait_core_model)
             if inspect.iscoroutinefunction(func):
 
                 @wraps(func)
                 async def dispatch(*args: Any, **kwargs: Any) -> Callable:
-                    self.init_context(pait_core_model, args, kwargs)
-                    invoke: PluginProtocol = self._plugin_manager_handler(pait_core_model, args, kwargs)[0]
-                    return await invoke(*args, **kwargs)
+                    context: ContextModel = self.init_context(pait_core_model, args, kwargs)
+                    return await pait_core_model.main_plugin(context)
 
                 return dispatch
             else:
 
                 @wraps(func)
                 def dispatch(*args: Any, **kwargs: Any) -> Callable:
-                    self.init_context(pait_core_model, args, kwargs)
-                    invoke: PluginProtocol = self._plugin_manager_handler(pait_core_model, args, kwargs)[0]
-                    return invoke(*args, **kwargs)
+                    context = self.init_context(pait_core_model, args, kwargs)
+                    return pait_core_model.main_plugin(context)
 
                 return dispatch
 
         return wrapper
```

### Comparing `pait-0.8.0.2/pait/data.py` & `pait-1.0.0a1/pait/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from types import CodeType
 from typing import TYPE_CHECKING, Dict, Set
 
 if TYPE_CHECKING:
-    from pait.model.core import PaitCoreModel
+    from pait.model import PaitCoreModel
 
 
 class PaitData(object):
     def __init__(self) -> None:
         self.pait_id_dict: Dict[str, Dict[str, "PaitCoreModel"]] = {}
 
     def register(self, app_name: str, pait_info_model: "PaitCoreModel") -> None:
@@ -25,26 +25,22 @@
         self,
         app_name: str,
         pait_id: str,
         path: str,
         openapi_path: str,
         method_set: Set[str],
         route_name: str,
-        project_name: str,
     ) -> None:
         """Route handle information supplemented by load_app"""
         if pait_id in self.pait_id_dict[app_name]:
             model: "PaitCoreModel" = self.pait_id_dict[app_name][pait_id]
             model.path = path
             model.openapi_path = openapi_path
             model.method_list = sorted(list(method_set or set()), reverse=True)
             model.operation_id = route_name
             func_code: CodeType = model.func.__code__  # type: ignore
-            if project_name:
-                model.func_path = project_name + f"{project_name}".join(func_code.co_filename.split(project_name)[1:])
-            else:
-                model.func_path = func_code.co_filename
+            model.func_path = func_code.co_filename
         else:
             logging.warning(f"load path:{path} fail, pait id:{pait_id}")
 
     def __bool__(self) -> bool:
         return bool(self.pait_id_dict)
```

### Comparing `pait-0.8.0.2/pait/exceptions.py` & `pait-1.0.0a1/pait/exceptions.py`

 * *Files identical despite different names*

### Comparing `pait-0.8.0.2/pait/extra/config.py` & `pait-1.0.0a1/pait/extra/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import re
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, Set, Tuple, Type
 
 from pydantic import BaseConfig, BaseModel
 
-from pait.model.response import PaitBaseResponseModel
-from pait.plugin.base import PluginManager
+from pait.model.response import BaseResponseModel
+from pait.plugin.base import PluginManager, PrePluginProtocol
 from pait.types import Literal
 from pait.util import http_method_tuple
 
 if TYPE_CHECKING:
-    from pait.model.config import APPLY_FN
-    from pait.model.core import PaitCoreModel
+    from pait.model import APPLY_FN, PaitCoreModel
     from pait.param_handle import BaseParamHandler
 
 
 __all__ = [
     "apply_multi_plugin",
     "apply_extra_openapi_model",
     "apply_response_model",
@@ -113,15 +112,15 @@
         if _is_match(pait_core_model, match_rule):
             pait_core_model.extra_openapi_model_list = [extra_openapi_model]
 
     return _apply
 
 
 def apply_response_model(
-    response_model_list: List[Type[PaitBaseResponseModel]], match_rule: Optional["MatchRule"] = None
+    response_model_list: List[Type[BaseResponseModel]], match_rule: Optional["MatchRule"] = None
 ) -> "APPLY_FN":
     """
     Add a default response structure for routing handles
     """
     for response_model in response_model_list:
         if response_model.is_core:
             raise ValueError(f"{response_model} is core response model can not set to default_response_model_list")
@@ -141,14 +140,26 @@
     def _apply(pait_core_model: "PaitCoreModel") -> None:
         if _is_match(pait_core_model, match_rule):
             pait_core_model.pydantic_model_config = pydantic_model_config
 
     return _apply
 
 
+def apply_default_pydantic_basemodel(
+    pydantic_basemodel: Type[BaseModel], match_rule: Optional["MatchRule"] = None
+) -> "APPLY_FN":
+    """pait route gen pydantic model default pydantic base model"""
+
+    def _apply(pait_core_model: "PaitCoreModel") -> None:
+        if _is_match(pait_core_model, match_rule):
+            pait_core_model.pydantic_basemodel = pydantic_basemodel
+
+    return _apply
+
+
 def apply_block_http_method_set(
     block_http_method_set: Set[str], match_rule: Optional["MatchRule"] = None
 ) -> "APPLY_FN":
     """
     Under normal circumstances, pait.load_app can obtain the http method of the routing handle.
      However, some application frameworks such as flask will automatically add optional http methods
      to the handle, which is great, but you may not want to use them in pait, and pait will not
@@ -171,15 +182,15 @@
 ) -> "APPLY_FN":
     def _apply(pait_core_model: "PaitCoreModel") -> None:
         if _is_match(pait_core_model, match_rule):
             pre_plugin_manager_list: List[PluginManager] = []
             post_plugin_manager_list: List[PluginManager] = []
             for plugin_manager_fn in plugin_manager_fn_list:
                 plugin_manager: PluginManager = plugin_manager_fn()
-                if plugin_manager.plugin_class.is_pre_core:
+                if issubclass(plugin_manager.plugin_class, PrePluginProtocol):
                     pre_plugin_manager_list.append(plugin_manager)
                 else:
                     post_plugin_manager_list.append(plugin_manager)
             pait_core_model.add_plugin(pre_plugin_manager_list, post_plugin_manager_list)
 
     return _apply
```

### Comparing `pait-0.8.0.2/pait/extra/util.py` & `pait-1.0.0a1/pait/extra/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
-    from pait.model.config import Config
-    from pait.model.core import PaitCoreModel
+    from pait.model import Config, PaitCoreModel
 
 
 __all__ = ["sync_config_data_to_pait_core_model"]
 
 
 def sync_config_data_to_pait_core_model(config: "Config", pait_core_model: "PaitCoreModel", **kwargs: Any) -> None:
     """Synchronize the config data to the corresponding pait core model"""
```

### Comparing `pait-0.8.0.2/pait/g.py` & `pait-1.0.0a1/pait/g.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from contextvars import ContextVar
 from typing import TYPE_CHECKING, Any
 
 from pait.data import PaitData
 from pait.extra.util import sync_config_data_to_pait_core_model
-from pait.model import tag
-from pait.model.config import Config
+from pait.model import Config, tag
 
 if TYPE_CHECKING:
-    from pait.model.core import ContextModel
+    from pait.model.context import ContextModel
 
 __all__ = ["config", "pait_data", "pait_context"]
 
 pait_context: ContextVar["ContextModel"] = ContextVar("pait_context")
 # In order to reduce the intrusion of pait to the application framework,
 # pait conducts data interaction through PaitData and Config
 pait_data: PaitData = PaitData()
 config: Config = Config()
 
-# pait_data and config cannot refer to each other within the module
+# pait_data and config cannot refer to each other within the module,
 # By replacing the init_config function, the user can change the pait_data data when calling config.init_config
 _real_config_init_config_method = config.init_config
 
 
 def _after_config_init(*args: Any, **kwargs: Any) -> None:
     _real_config_init_config_method(*args, **kwargs)
     for app_name, real_pait_id_dict in pait_data.pait_id_dict.items():
```

### Comparing `pait-0.8.0.2/pait/http/api_pb2.pyi` & `pait-1.0.0a1/pait/grpc/proto/api_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,17 @@
     RESPONSE_BODY_FIELD_NUMBER: builtins.int
     ADDITIONAL_BINDINGS_FIELD_NUMBER: builtins.int
     GROUP_FIELD_NUMBER: builtins.int
     TAG_FIELD_NUMBER: builtins.int
     SUMMARY_FIELD_NUMBER: builtins.int
     DESC_FIELD_NUMBER: builtins.int
     NOT_ENABLE_FIELD_NUMBER: builtins.int
+    AUTHOR_FIELD_NUMBER: builtins.int
+    REQUEST_MESSAGE_FIELD_NUMBER: builtins.int
+    RESPONSE_MESSAGE_FIELD_NUMBER: builtins.int
     @property
     def get(self) -> global___HttpMethod:
         """Maps to HTTP GET. Used for listing and getting information about
         resources.
         """
         pass
     @property
@@ -61,53 +64,68 @@
         """
         pass
     @property
     def any(self) -> global___HttpMethod:
         """Automatically generated by gRPC Gateway"""
         pass
     body: typing.Text
-    """The name of the request field whose value is mapped to the HTTP request
-    body, or `*` for mapping all request fields not captured by the path
-    pattern to the HTTP body, or omitted for not having any HTTP request body.
-
-    NOTE: the referred field must be present at the top-level of the request
-    message type.
+    """Note: Pait Not support
+    // The name of the request field whose value is mapped to the HTTP request
+    // body, or `*` for mapping all request fields not captured by the path
+    // pattern to the HTTP body, or omitted for not having any HTTP request body.
+    //
+    // NOTE: the referred field must be present at the top-level of the request
+    // message type.
     """
 
     response_body: typing.Text
-    """Optional. The name of the response field whose value is mapped to the HTTP
-    response body. When omitted, the entire response message will be used
-    as the HTTP response body.
-
-    NOTE: The referred field must be present at the top-level of the response
-    message type.
+    """Note: Pait Not support
+    // Optional. The name of the response field whose value is mapped to the HTTP
+    // response body. When omitted, the entire response message will be used
+    // as the HTTP response body.
+    //
+    // NOTE: The referred field must be present at the top-level of the response
+    // message type.
     """
+
     @property
     def additional_bindings(
         self,
     ) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApiRule]:
         """Additional HTTP bindings for the selector. Nested bindings must
         not contain an `additional_bindings` field themselves (that is,
         the nesting may only be one level deep).
         """
         pass
     group: typing.Text
     """the group to which the method belongs"""
+
     @property
     def tag(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Tag]:
         """The tag corresponding to this method and the description of the tag"""
         pass
     summary: typing.Text
     """a summary of the method"""
 
     desc: typing.Text
     """documentation for the use of this method"""
 
     not_enable: builtins.bool
     """whether to map the method"""
+
+    @property
+    def author(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text]:
+        """Write the author of the API"""
+        pass
+    @property
+    def request_message(self) -> global___BuildMessage:
+        """Specifies how to build a new Message"""
+        pass
+    @property
+    def response_message(self) -> global___BuildMessage: ...
     def __init__(
         self,
         *,
         get: typing.Optional[global___HttpMethod] = ...,
         put: typing.Optional[global___HttpMethod] = ...,
         post: typing.Optional[global___HttpMethod] = ...,
         delete: typing.Optional[global___HttpMethod] = ...,
@@ -118,14 +136,17 @@
         response_body: typing.Text = ...,
         additional_bindings: typing.Optional[typing.Iterable[global___ApiRule]] = ...,
         group: typing.Text = ...,
         tag: typing.Optional[typing.Iterable[global___Tag]] = ...,
         summary: typing.Text = ...,
         desc: typing.Text = ...,
         not_enable: builtins.bool = ...,
+        author: typing.Optional[typing.Iterable[typing.Text]] = ...,
+        request_message: typing.Optional[global___BuildMessage] = ...,
+        response_message: typing.Optional[global___BuildMessage] = ...,
     ) -> None: ...
     def HasField(
         self,
         field_name: typing_extensions.Literal[
             "any",
             b"any",
             "custom",
@@ -138,23 +159,29 @@
             b"http_method",
             "patch",
             b"patch",
             "post",
             b"post",
             "put",
             b"put",
+            "request_message",
+            b"request_message",
+            "response_message",
+            b"response_message",
         ],
     ) -> builtins.bool: ...
     def ClearField(
         self,
         field_name: typing_extensions.Literal[
             "additional_bindings",
             b"additional_bindings",
             "any",
             b"any",
+            "author",
+            b"author",
             "body",
             b"body",
             "custom",
             b"custom",
             "delete",
             b"delete",
             "desc",
@@ -169,16 +196,20 @@
             b"not_enable",
             "patch",
             b"patch",
             "post",
             b"post",
             "put",
             b"put",
+            "request_message",
+            b"request_message",
             "response_body",
             b"response_body",
+            "response_message",
+            b"response_message",
             "summary",
             b"summary",
             "tag",
             b"tag",
         ],
     ) -> None: ...
     def WhichOneof(
@@ -236,14 +267,15 @@
     """The specified http url, if empty, it will be generated by gRPC Gateway
     example: /api/user/create
              /api/user/delete
     """
 
     default: builtins.bool
     """If the value is True, the url is the url corresponding to the rpc method"""
+
     def __init__(
         self,
         *,
         url: typing.Text = ...,
         default: builtins.bool = ...,
     ) -> None: ...
     def HasField(
@@ -254,12 +286,62 @@
     ) -> None: ...
     def WhichOneof(
         self, oneof_group: typing_extensions.Literal["http_url", b"http_url"]
     ) -> typing.Optional[typing_extensions.Literal["url", "default"]]: ...
 
 global___HttpMethod = HttpMethod
 
+class BuildMessage(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    EXCLUDE_COLUMN_NAME_FIELD_NUMBER: builtins.int
+    NESTED_FIELD_NUMBER: builtins.int
+    exclude_column_name: typing.Text
+    """Which fields (name) in Message are not used.(A comma-separated string,e.g. "a,b" -> ["a", "b"])
+    Which nested field of Message to use
+     Example:
+       nested = "/sub/subfield"
+       real message = SubSubMessage
+    """
+
+    nested: typing.Text
+    """   message GetMessageRequest {
+         message SubSubMessage {
+           string subfield = 1;
+         }
+         message SubMessage {
+           SubSubMessage subfield = 1;
+         }
+         string message_id = 1;
+         int64 revision = 2;
+         SubMessage sub = 3;
+       }
+    """
+
+    def __init__(
+        self,
+        *,
+        exclude_column_name: typing.Text = ...,
+        nested: typing.Text = ...,
+    ) -> None: ...
+    def HasField(
+        self,
+        field_name: typing_extensions.Literal[
+            "action", b"action", "exclude_column_name", b"exclude_column_name", "nested", b"nested"
+        ],
+    ) -> builtins.bool: ...
+    def ClearField(
+        self,
+        field_name: typing_extensions.Literal[
+            "action", b"action", "exclude_column_name", b"exclude_column_name", "nested", b"nested"
+        ],
+    ) -> None: ...
+    def WhichOneof(
+        self, oneof_group: typing_extensions.Literal["action", b"action"]
+    ) -> typing.Optional[typing_extensions.Literal["exclude_column_name", "nested"]]: ...
+
+global___BuildMessage = BuildMessage
+
 HTTP_FIELD_NUMBER: builtins.int
 http: google.protobuf.internal.extension_dict._ExtensionFieldDescriptor[
     google.protobuf.descriptor_pb2.MethodOptions, global___ApiRule
 ]
 """design like google.api.http"""
```

### Comparing `pait-0.8.0.2/pait/model/config.py` & `pait-1.0.0a1/pait/model/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from json import JSONEncoder
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Tuple, Type
 
 from pydantic import BaseConfig
 
-from pait.model.response import PaitBaseResponseModel
+from pait.model.response import BaseResponseModel
 from pait.model.status import PaitStatus
-from pait.util import CustomJSONEncoder, I18nTypedDict, change_local
-from pait.util import i18n_config_dict as pait_i18n_config_dict
-from pait.util import i18n_local as pait_i18n_local
 from pait.util import json_type_default_value_dict as pait_json_type_default_value_dict
 from pait.util import python_type_default_value_dict as pait_python_type_default_value_dict
+from pait.util.encoder import CustomJSONEncoder
 
 if TYPE_CHECKING:
     from pait.model.core import PaitCoreModel
 
 APPLY_FN = Callable[["PaitCoreModel"], None]
 
 
@@ -27,19 +25,18 @@
 
     __initialized: bool = False
 
     def __init__(self) -> None:
         self.author: Tuple[str, ...] = ("",)
         self.status: PaitStatus = PaitStatus.undefined
         self.block_http_method_set: Set[str] = set()
-        self.default_response_model_list: List[Type[PaitBaseResponseModel]] = []
+        self.default_response_model_list: List[Type[BaseResponseModel]] = []
         self.json_encoder: Type[JSONEncoder] = CustomJSONEncoder
         self.default_pydantic_model_config: Type[BaseConfig] = BaseConfig
         self.tag_dict: Dict[str, str] = {}
-        self.i18n_local: str = pait_i18n_local
         self.apply_func_list: List[APPLY_FN] = []
 
     def __setattr__(self, key: Any, value: Any) -> None:
         if not self.__initialized:
             super().__setattr__(key, value)
         else:
             raise RuntimeError("Can not set new value in runtime")
@@ -47,26 +44,22 @@
     def init_config(
         self,
         author: Optional[Tuple[str, ...]] = None,
         status: Optional[PaitStatus] = None,
         json_type_default_value_dict: Optional[Dict[str, Any]] = None,
         python_type_default_value_dict: Optional[Dict[type, Any]] = None,
         json_encoder: Optional[Type[JSONEncoder]] = None,
-        i18n_local: str = pait_i18n_local,
-        i18n_config_dict: Optional[Dict[str, I18nTypedDict]] = None,
         apply_func_list: Optional[List[APPLY_FN]] = None,
     ) -> None:
         """
         :param author:  Only @pait(author=None) will be called to change the configuration
         :param status:  Only @pait(status=None) will be called to change the configuration
         :param json_type_default_value_dict: Configure default values for each json type
         :param python_type_default_value_dict: Configure default values for each python type
         :param json_encoder: Define certain types of serialization rules
-        :param i18n_local: Select the default i18 language
-        :param i18n_config_dict: Update i18n-related configuration
         :param apply_func_list: List of functions for application configuration
         :return:
         """
         if self.__initialized:
             raise RuntimeError("Can not set new value in runtime")
         if author:
             self.author = author
@@ -75,18 +68,14 @@
 
         if json_type_default_value_dict:
             pait_json_type_default_value_dict.update(json_type_default_value_dict)
         if python_type_default_value_dict:
             pait_python_type_default_value_dict.update(python_type_default_value_dict)
         if json_encoder:
             self.json_encoder = json_encoder
-        if i18n_local:
-            change_local(i18n_local)
-        if i18n_config_dict:
-            pait_i18n_config_dict.update(i18n_config_dict)
         if apply_func_list:
             self.apply_func_list = apply_func_list
         self.__initialized = True
 
     @property
     def initialized(self) -> bool:
         """Judge whether it has been initialized, it can only be initialized once per run"""
```

### Comparing `pait-0.8.0.2/pait/model/core.py` & `pait-1.0.0a1/pait/model/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,141 @@
-import inspect
+import copy
 import logging
-from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, Set, Tuple, Type
 
 from pydantic import BaseConfig, BaseModel
 
-from pait.model.response import PaitBaseResponseModel, PaitResponseModel
+from pait.model.response import BaseResponseModel, PaitResponseModel
 from pait.model.status import PaitStatus
-from pait.param_handle import AsyncParamHandler, BaseParamHandler, ParamHandler
-from pait.plugin import PluginManager
-from pait.util import ignore_pre_check
+from pait.model.tag import Tag
+from pait.param_handle import BaseParamHandler
+from pait.plugin import PluginManager, PluginProtocol, PostPluginProtocol, PrePluginProtocol
+from pait.util import gen_tip_exc, ignore_pre_check
 
 if TYPE_CHECKING:
     from pait.app.base import BaseAppHelper
+    from pait.field import BaseField
 
-from pait.extra.config import MatchKeyLiteral, MatchRule
 
-__all__ = ["PaitCoreModel", "ContextModel", "MatchRule", "MatchKeyLiteral"]
+__all__ = ["PaitCoreModel", "get_core_model"]
+ChangeNotifyType = Callable[["PaitCoreModel", str, Any], None]
 
 
-@dataclass
-class ContextModel(object):
-    cbv_instance: Optional[Any]
-    app_helper: "BaseAppHelper"
+def get_core_model(route: Callable) -> "PaitCoreModel":
+    core_model: Optional["PaitCoreModel"] = getattr(route, "pait_core_model", None)
+    if not core_model:
+        raise TypeError(f"Routing function: {route} has not been wrapped by pait")
+    return core_model
 
 
 class PaitCoreModel(object):
     _param_handler_plugin: PluginManager["BaseParamHandler"]
+    _main_plugin: PluginProtocol
 
     def __init__(
         self,
         func: Callable,
         app_helper_class: "Type[BaseAppHelper]",
+        param_handler_plugin: Type[BaseParamHandler],
         pre_depend_list: Optional[List[Callable]] = None,
         path: Optional[str] = None,
         openapi_path: Optional[str] = None,
         method_set: Optional[Set[str]] = None,
         operation_id: Optional[str] = None,
         func_name: Optional[str] = None,
         author: Optional[Tuple[str, ...]] = None,
         summary: Optional[str] = None,
         desc: Optional[str] = None,
         status: Optional[PaitStatus] = None,
         group: Optional[str] = None,
-        tag: Optional[Tuple[str, ...]] = None,
-        response_model_list: Optional[List[Type[PaitBaseResponseModel]]] = None,
+        tag: Optional[Tuple[Tag, ...]] = None,
+        response_model_list: Optional[List[Type[BaseResponseModel]]] = None,
         pydantic_model_config: Optional[Type[BaseConfig]] = None,
-        plugin_list: Optional[List[PluginManager]] = None,
-        post_plugin_list: Optional[List[PluginManager]] = None,
-        param_handler_plugin: Optional[Type[BaseParamHandler]] = None,
+        pydantic_basemodel: Optional[Type[BaseModel]] = None,
+        default_field_class: Optional[Type["BaseField"]] = None,
+        plugin_list: Optional[List[PluginManager[PrePluginProtocol]]] = None,
+        post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]] = None,
         feature_code: str = "",
+        **kwargs: Any,
     ):
         # pait
         self.app_helper_class: "Type[BaseAppHelper]" = app_helper_class
+        self.default_field_class: Optional[Type["BaseField"]] = default_field_class
         self.func: Callable = func  # route func
         # self.qualname: str = func.__qualname__.split(".<locals>", 1)[0].rsplit(".", 1)[0]
         self.pait_id: str = f"{func.__qualname__}_{self.func_md5}"
         # Some functions have the same md5 as the name and need to be distinguished by the feature code
         if feature_code:
             self.pait_id = f"{feature_code}_{self.pait_id}"
         setattr(func, "_pait_id", self.pait_id)
         setattr(func, "pait_core_model", self)
         self.pre_depend_list: List[Callable] = pre_depend_list or []
         self.func_path: str = ""
         self.block_http_method_set: Set[str] = set()
-        self.pydantic_model_config: Type[BaseConfig] = pydantic_model_config or BaseConfig
+        self.pydantic_model_config: Optional[Type[BaseConfig]] = pydantic_model_config
+        self.pydantic_basemodel: Optional[Type[BaseModel]] = pydantic_basemodel
+        self.extra: dict = kwargs
 
         # api doc
         self.path: str = path or ""  # request url path
         self.openapi_path: str = openapi_path or ""
         self._method_list: List[str] = sorted(list(method_set or set()))  # request method set
         self.func_name: str = func_name or func.__name__
         self.operation_id: str = operation_id or self.func_name  # route name
         self.author: Optional[Tuple[str, ...]] = author  # The main developer of this func
         self.summary: str = summary or ""
         self.desc: str = desc or func.__doc__ or ""  # desc of this func
         self.status: PaitStatus = status or PaitStatus.undefined
         self.group: str = group or "root"  # Which group this interface belongs to
-        self.tag: Tuple[str, ...] = tag or ("default",)  # Interface tag
+        self.tag: Tuple[Tag, ...] = tag or (Tag(name="default"),)  # Interface tag
         self._extra_openapi_model_list: List[Type[BaseModel]] = []
-
-        self._response_model_list: List[Type[PaitBaseResponseModel]] = []
+        self._response_model_list: List[Type[BaseResponseModel]] = []
         if response_model_list:
             self.add_response_model_list(response_model_list)
 
         # pait plugin
         self._plugin_list: List[PluginManager] = []
         self._post_plugin_list: List[PluginManager] = []
-        self._plugin_manager_list: List[PluginManager] = []
-
         self.param_handler_plugin = param_handler_plugin  # type: ignore
         self.add_plugin(plugin_list, post_plugin_list)
 
+        # change notify
+        self._change_notify_list: List[ChangeNotifyType] = []
+
+    def add_change_notify(self, callback: ChangeNotifyType) -> None:
+        self._change_notify_list.append(callback)
+
+    def remove_change_notify(self, callback: ChangeNotifyType) -> None:
+        self._change_notify_list.remove(callback)
+
+    def __setattr__(self, key: str, value: Any) -> None:
+        if key.startswith("_"):
+            return super().__setattr__(key, value)
+
+        change_notify_list: List[ChangeNotifyType] = self.__dict__.get("_change_notify_list", [])
+        if change_notify_list:
+            for callback in self._change_notify_list:
+                callback(self, key, value)
+        return super().__setattr__(key, value)
+
     @property
     def param_handler_plugin(self) -> Type[BaseParamHandler]:
         return self._param_handler_plugin.plugin_class
 
     @param_handler_plugin.setter
-    def param_handler_plugin(self, param_handler_plugin: Optional[Type[BaseParamHandler]]) -> None:
-        if param_handler_plugin:
-            self._param_handler_plugin = PluginManager(param_handler_plugin)
-        elif inspect.iscoroutinefunction(self.func):
-            self._param_handler_plugin = PluginManager(AsyncParamHandler)
-        else:
-            self._param_handler_plugin = PluginManager(ParamHandler)
-        if not ignore_pre_check:
-            self._param_handler_plugin.pre_check_hook(self)
-        self._param_handler_plugin.pre_load_hook(self)
-        if not self._plugin_manager_list:
-            self.add_plugin([], [])
+    def param_handler_plugin(self, param_handler_plugin: Type[BaseParamHandler]) -> None:
+        self._param_handler_plugin = PluginManager(param_handler_plugin)
+
+        try:
+            if not ignore_pre_check:
+                self._param_handler_plugin.pre_check_hook(self)
+            self._param_handler_plugin.pre_load_hook(self)
+        except Exception as e:
+            raise gen_tip_exc(self.func, RuntimeError(f"set param plugin error: {e}")) from e
+        self.add_plugin([], [])
 
     @property
     def func_md5(self) -> str:
         from hashlib import md5
 
         h = md5()
         h.update(self.func.__code__.co_code)  # type: ignore
@@ -125,68 +148,73 @@
         return sorted(list(_temp_set))
 
     @method_list.setter
     def method_list(self, method_list: List[str]) -> None:
         self._method_list = list(set(self._method_list) | set(method_list))
 
     @property
-    def response_model_list(self) -> List[Type[PaitBaseResponseModel]]:
+    def openapi_method_list(self) -> List[str]:
+        return [i.lower() for i in self.method_list]
+
+    @property
+    def response_model_list(self) -> List[Type[BaseResponseModel]]:
         return self._response_model_list
 
-    def add_response_model_list(self, response_model_list: List[Type[PaitBaseResponseModel]]) -> None:
+    def add_response_model_list(self, response_model_list: List[Type[BaseResponseModel]]) -> None:
         for response_model in response_model_list:
             if response_model in self._response_model_list:
                 continue
             if issubclass(response_model, PaitResponseModel):
                 logging.warning(
-                    f"Please replace {self.operation_id}'s response model {response_model}"
-                    f" with {PaitBaseResponseModel}"
+                    f"Please replace {self.operation_id}'s response model {response_model}" f" with {BaseResponseModel}"
                 )
             self._response_model_list.append(response_model)
 
     @property
     def extra_openapi_model_list(self) -> List[Type[BaseModel]]:
         return self._extra_openapi_model_list
 
     @extra_openapi_model_list.setter
     def extra_openapi_model_list(self, item: List[Type[BaseModel]]) -> None:
         self._extra_openapi_model_list.extend(item)
 
     @property
-    def plugin_list(self) -> List[PluginManager]:
-        return self._plugin_manager_list
+    def main_plugin(self) -> PluginProtocol:
+        return self._main_plugin
+
+    def build_plugin_stack(self) -> None:
+        plugin_manager_list: List[PluginManager] = (
+            [i for i in self._plugin_list] + [self._param_handler_plugin] + [i for i in self._post_plugin_list]
+        )
+        self._main_plugin = self.func  # type: ignore
+        for plugin_manager in reversed(plugin_manager_list):
+            self._main_plugin = plugin_manager.get_plugin(self._main_plugin, self)
 
     def add_plugin(
-        self, plugin_list: Optional[List[PluginManager]], post_plugin_list: Optional[List[PluginManager]]
+        self,
+        plugin_list: Optional[List[PluginManager[PrePluginProtocol]]],
+        post_plugin_list: Optional[List[PluginManager[PostPluginProtocol]]],
     ) -> None:
-        raw_plugin_list: List[PluginManager] = self._plugin_list
-        raw_post_plugin_list: List[PluginManager] = self._post_plugin_list
+        raw_plugin_list: List[PluginManager] = copy.deepcopy(self._plugin_list)
+        raw_post_plugin_list: List[PluginManager] = copy.deepcopy(self._post_plugin_list)
         try:
             for plugin_manager in plugin_list or []:
-                if not plugin_manager.plugin_class.is_pre_core:
+                if issubclass(plugin_manager.plugin_class, PostPluginProtocol):
                     raise ValueError(f"{plugin_manager.plugin_class} is post plugin")
                 if not ignore_pre_check:
                     plugin_manager.pre_check_hook(self)
                 plugin_manager.pre_load_hook(self)
                 self._plugin_list.append(plugin_manager)
 
-            for plugin_manager in post_plugin_list or []:
-                if plugin_manager.plugin_class.is_pre_core:
-                    raise ValueError(f"{plugin_manager.plugin_class} is pre plugin")
+            for post_plugin_manager in post_plugin_list or []:
+                if issubclass(post_plugin_manager.plugin_class, PrePluginProtocol):
+                    raise ValueError(f"{post_plugin_manager.plugin_class} is pre plugin")
                 if not ignore_pre_check:
-                    plugin_manager.pre_check_hook(self)
-                plugin_manager.pre_load_hook(self)
-                self._post_plugin_list.append(plugin_manager)
+                    post_plugin_manager.pre_check_hook(self)
+                post_plugin_manager.pre_load_hook(self)
+                self._post_plugin_list.append(post_plugin_manager)
         except Exception as e:
             self._plugin_list = raw_plugin_list
             self._post_plugin_list = raw_post_plugin_list
-            raise e
+            raise gen_tip_exc(self.func, RuntimeError(f"{self.func} add plugin error")) from e
         else:
-            # In future version, it may be possible to switch plugins at runtime
-            plugin_manager_list: List[PluginManager] = (
-                [i for i in self._plugin_list] + [self._param_handler_plugin] + [i for i in self._post_plugin_list]
-            )
-            # copy.deepcopy(
-            #     self._plugin_list + [self._param_handler_plugin] + self._post_plugin_list
-            # )
-            plugin_manager_list.reverse()
-            self._plugin_manager_list = plugin_manager_list
+            self.build_plugin_stack()
```

### Comparing `pait-0.8.0.2/pait/model/response.py` & `pait-1.0.0a1/pait/plugin/auto_complete_json_resp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,100 +1,60 @@
 import copy
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, Type
 
-from pydantic import BaseModel
-
-from pait.util import gen_example_dict_from_pydantic_base_model
-
-__all__ = [
-    "PaitResponseModel",
-    "PaitBaseResponseModel",
-    "PaitHtmlResponseModel",
-    "PaitJsonResponseModel",
-    "PaitFileResponseModel",
-    "PaitTextResponseModel",
-]
-
-
-class PaitBaseResponseModel(object):
-    """response model https://swagger.io/docs/specification/describing-responses/"""
-
-    # Used for mock response and response checking to determine if the response model is the core response model
-    is_core: bool = False
-
-    # response data
-    response_data: Union[Type[BaseModel], str, bytes]
-    # response media type
-    media_type: str = "*/*"
-
-    # response name
-    name: Optional[str] = None
-    # response description
-    description: Optional[str] = None
-    # response header
-    header: dict = {}
-    # response status code
-    status_code: Tuple[int] = (200,)
-
-    # The value of this response in openapi.schema
-    # if value is empty, pait will auto gen response model and set to openapi.schema
-    openapi_schema: Optional[dict] = None
-
-    # links model
-    links_schema_dict: Dict[str, dict] = {}
-
-    @classmethod
-    def is_base_model_response_data(cls) -> bool:
-        return isinstance(cls.response_data, type) and issubclass(cls.response_data, BaseModel)
-
-    @classmethod
-    def get_example_value(cls, **extra: Any) -> Any:
-        return cls.response_data
-
-    @classmethod
-    def register_link_schema(cls, link_schema: dict) -> None:
-        cls.links_schema_dict.update(link_schema)
-
-
-class PaitJsonResponseModel(PaitBaseResponseModel):
-    response_data: Type[BaseModel]
-    media_type: str = "application/json"
+from pait.model.response import BaseResponseModel, JsonResponseModel
+from pait.plugin.base import PluginContext, PrePluginProtocol
+from pait.util import get_pait_response_model
+
+if TYPE_CHECKING:
+    from pait.model.core import PaitCoreModel
+
+
+class AutoCompleteJsonRespPlugin(PrePluginProtocol):
+    default_response_dict: dict
+
+    def _merge(self, source_dict: dict, target_dict: dict) -> None:
+        for key, value in source_dict.items():
+            if isinstance(value, dict) and key in target_dict:
+                self._merge(value, target_dict[key])
+            elif value and isinstance(value, list) and key in target_dict:
+                raw_value = value.pop()
+                for item in target_dict[key]:
+                    new_value = copy.deepcopy(raw_value)
+                    self._merge(new_value, item)
+                    value.append(new_value)
+            else:
+                source_dict[key] = target_dict.get(key, value)
+
+    def merge(self, response_dict: dict) -> dict:
+        default_response_dict: dict = copy.deepcopy(self.default_response_dict)
+        self._merge(default_response_dict, response_dict)
+        return default_response_dict
 
     @classmethod
-    def get_example_value(cls, **extra: Any) -> dict:
-        return gen_example_dict_from_pydantic_base_model(cls.response_data)
+    def pre_check_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> None:
+        super().pre_check_hook(pait_core_model, kwargs)
+        if "default_response_dict" in kwargs:
+            raise RuntimeError("Please use response_model_list param")
 
     @classmethod
-    def get_default_dict(cls, **extra: Any) -> dict:
-        default_dict: dict = getattr(cls.response_data, "PaitJsonResponseModel_default_dict", {})
-        if not default_dict:
-            default_dict = gen_example_dict_from_pydantic_base_model(cls.response_data, use_example_value=False)
-            setattr(cls.response_data, "PaitJsonResponseModel_default_dict", default_dict)
-        return copy.deepcopy(default_dict)
-
-
-class PaitResponseModel(PaitJsonResponseModel):
-    """
-    PaitJsonResponseModel alias
-    Compatible versions below 0.7
-    """
-
-
-class PaitTextResponseModel(PaitBaseResponseModel):
-    response_data: str = "pait example data"
-    media_type: str = "text/plain"
-
-    openapi_schema: dict = {"type": "string", "example": response_data}
-
-
-class PaitHtmlResponseModel(PaitBaseResponseModel):
-    response_data: str = "<h1>Pait example html</h1>"
-    media_type: str = "text/html"
-
-    openapi_schema: dict = {"type": "string", "example": response_data}
-
-
-class PaitFileResponseModel(PaitBaseResponseModel):
-    response_data: bytes = b"pait example bytes"
-    media_type: str = "application/octet-stream"
-
-    openapi_schema: dict = {"type": "string", "format": "binary"}
+    def pre_load_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> Dict:
+        kwargs = super().pre_load_hook(pait_core_model, kwargs)
+        pait_response_model: Type[BaseResponseModel] = get_pait_response_model(pait_core_model.response_model_list)
+        if not issubclass(pait_response_model, JsonResponseModel):
+            raise ValueError(f"pait_response_model must `{JsonResponseModel.__name__}` not {pait_response_model}")
+        kwargs["default_response_dict"] = pait_response_model.get_default_dict()
+        return kwargs
+
+    def _sync_call(self, context: PluginContext) -> Any:
+        response_dict: dict = super().__call__(context)
+        return self.merge(response_dict)
+
+    async def _async_call(self, context: PluginContext) -> Any:
+        response_dict: dict = await super().__call__(context)
+        return self.merge(response_dict)
+
+    def __call__(self, context: PluginContext) -> Any:
+        if self._is_async_func:
+            return self._async_call(context)
+        else:
+            return self._sync_call(context)
```

### Comparing `pait-0.8.0.2/pait/model/template.py` & `pait-1.0.0a1/pait/model/template.py`

 * *Files identical despite different names*

### Comparing `pait-0.8.0.2/pait/plugin/auto_complete_json_resp.py` & `pait-1.0.0a1/pait/plugin/unified_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,51 @@
-from typing import TYPE_CHECKING, Any, Dict, Type
+from abc import ABCMeta
+from typing import Any, Dict, Optional, Type
 
-from pydantic import BaseModel
-
-from pait.model.response import PaitBaseResponseModel, PaitJsonResponseModel
-from pait.plugin.base import PluginProtocol
+from pait.model.core import PaitCoreModel
+from pait.model.response import BaseResponseModel, FileResponseModel
+from pait.plugin.base import PluginContext, PrePluginProtocol
 from pait.util import get_pait_response_model
 
-if TYPE_CHECKING:
-    from pait.model.core import PaitCoreModel
-
-
-class AutoCompleteJsonRespPlugin(PluginProtocol):
-    """According to the response object, automatically fill in the missing value of json"""
 
-    response_data_model: Type[BaseModel]
+class UnifiedResponsePluginProtocol(PrePluginProtocol):
+    response_model_class: Type[BaseResponseModel]
 
-    def merge(self, response_dict: dict) -> dict:
-        return self.response_data_model(**response_dict).dict()
-
-    @classmethod
-    def pre_check_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> None:
-        super().pre_check_hook(pait_core_model, kwargs)
-        if "pait_response_model" in kwargs:
-            raise RuntimeError("Please use response_model_list param")
+    def _gen_response(self, return_value: Any, context: PluginContext) -> Any:
+        raise NotImplementedError
 
     @classmethod
     def pre_load_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> Dict:
         kwargs = super().pre_load_hook(pait_core_model, kwargs)
-        pait_response_model: Type[PaitBaseResponseModel] = get_pait_response_model(
-            pait_core_model.response_model_list, find_core_response_model=True
-        )
-        if not issubclass(pait_response_model, PaitJsonResponseModel):
-            raise ValueError(f"pait_response_model must {PaitJsonResponseModel} not {pait_response_model}")
-        kwargs["response_data_model"] = pait_response_model.response_data
+        if pait_core_model.response_model_list:
+            pait_response: Type[BaseResponseModel] = get_pait_response_model(
+                pait_core_model.response_model_list,
+                target_pait_response_class=kwargs.pop("target_pait_response_class", False),
+            )
+            if issubclass(pait_response, FileResponseModel):
+                raise ValueError(f"Not Support {FileResponseModel.__name__}")
+            kwargs["response_model_class"] = pait_response
+        else:
+            raise ValueError(
+                f"The response model list cannot be empty, please add a response model to"
+                f" {pait_core_model.func.__qualname__}"
+            )
         return kwargs
 
-    def _sync_call(self, *args: Any, **kwargs: Any) -> Any:
-        response_dict = self.call_next(*args, **kwargs)
-        return self.merge(response_dict)
-
-    async def _async_call(self, *args: Any, **kwargs: Any) -> Any:
-        response_dict: dict = await self.call_next(*args, **kwargs)
-        return self.merge(response_dict)
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        if self._is_async_func:
-            return self._async_call(*args, **kwargs)
-        else:
-            return self._sync_call(*args, **kwargs)
+class UnifiedResponsePlugin(UnifiedResponsePluginProtocol, metaclass=ABCMeta):
+    status_code: int
+    headers: Optional[dict]
+    media_type: Optional[str]
 
+    def __call__(self, context: PluginContext) -> Any:
+        if self._is_async_func:
+            return self._async_call(context)
+        return self._sync_call(context)
 
-class AsyncAutoCompleteJsonRespPlugin(AutoCompleteJsonRespPlugin):
-    """"""
+    def _sync_call(self, context: PluginContext) -> Any:
+        response: Any = super(UnifiedResponsePlugin, self).__call__(context)
+        return self._gen_response(response, context)
+
+    async def _async_call(self, context: PluginContext) -> Any:
+        response: Any = await super(UnifiedResponsePlugin, self).__call__(context)
+        return self._gen_response(response, context)
```

### Comparing `pait-0.8.0.2/pait/plugin/base.py` & `pait-1.0.0a1/pait/plugin/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,94 @@
 import inspect
 import logging
-from typing import TYPE_CHECKING, Any, Dict, Generic, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, Dict, Generic, Type, TypeVar, Union
 
 if TYPE_CHECKING:
     from pait.model.core import PaitCoreModel
 
+from pait.model.context import ContextModel as PluginContext
+
 _PluginT = TypeVar("_PluginT", bound="PluginProtocol")
+_NextPluginT = Union[_PluginT, Callable]
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class PluginProtocol(object):
-    # Indicates whether the plugin is a pre plugin or a post plugin, by default it is a pre plugin
-    is_pre_core: bool = True
-
-    pait_core_model: "PaitCoreModel"
-    args: list
-    kwargs: dict
-
-    _is_async_func: bool
-
-    def __init__(self: "_PluginT", **kwargs: Any) -> None:
+    def __init__(self, next_plugin: _NextPluginT, pait_core_model: "PaitCoreModel", **kwargs: Any) -> None:
         """Direct init calls are not supported,
         so there is no need to write clearly in init what parameters are needed
         """
+        self.next_plugin: _NextPluginT = next_plugin
+        self.pait_core_model: "PaitCoreModel" = pait_core_model
+        self._is_async_func: bool = inspect.iscoroutinefunction(pait_core_model.func)
         if kwargs:
             for k, v in kwargs.items():
                 if getattr(self, k, None) is not None:
                     continue
                 setattr(self, k, v)
+        self.__post_init__(**kwargs)
+
+    def __post_init__(self, **kwargs: Any) -> None:
+        pass
 
     @classmethod
     def pre_check_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> None:
         """The hook that runs the check at startup. If the value of env's PAIT_IGNORE_PRE_CHECK is True,
-        it will not be executed."""
-        class_name: str = cls.__class__.__name__
-        if class_name.startswith("Async"):
-            logger.warning(
-                f"Please use {class_name.replace('Async', '')}, {class_name} will remove on version 1.0"
-            )  # pragma: no cover
+        it will not be executed.
+
+        Note:
+            Failure to execute this stage will cause the plugin to fail to load, but will not affect the use of routes
+        """
 
     @classmethod
     def pre_load_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> Dict:
-        """Hook for initialization processing"""
-        kwargs["_is_async_func"] = inspect.iscoroutinefunction(pait_core_model.func)
-        return kwargs  # pragma: no cover
+        """Hook for initialization processing, the plugin has not been initialized at this time
 
-    def __post_init__(self, pait_core_model: "PaitCoreModel", args: tuple, kwargs: dict) -> None:
-        self.pait_core_model = pait_core_model
-        self.args = list(args) or []
-        self.kwargs = kwargs or {}
+        Note:
+            Failure to execute this stage will cause the plugin to fail to load, but will not affect the use of routes
+        """
+        return kwargs  # pragma: no cover
 
     @classmethod
     def build(cls, **kwargs: Any) -> "PluginManager[_PluginT]":
         """Factory function for generating plugins"""
         return PluginManager(cls, **kwargs)  # type: ignore
 
-    def call_next(self, *args: Any, **kwargs: Any) -> Any:
-        """Call the method of the next plugin, this method does not support being inherited and modified"""
-        raise RuntimeError("Failed to load Plugin, please check the list of plugins")  # pragma: no cover
-
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        """The entry function called by the plugin.
-        If it is a pre plugin, args and kwargs are the parameters for the corresponding web framework to call the
-         route.
-        If it is a post plugin, args and kwargs are the parameters filled in by the developer to write the routing
-         function.
-        """
-        return self.call_next(*args, **kwargs)  # pragma: no cover
+    def __call__(self, context: PluginContext) -> Any:
+        """The entry function called by the plugin."""
+        if isinstance(self.next_plugin, PluginProtocol):
+            return self.next_plugin(context)
+        else:
+            return self.next_plugin(*context.args, **context.kwargs)
+
+
+class PrePluginProtocol(PluginProtocol):
+    """Pre Plugin"""
+
+
+class PostPluginProtocol(PluginProtocol):
+    """Post Plugin"""
 
 
 class PluginManager(Generic[_PluginT]):
-    """A proxy for the Pait plugin, Ensure plugins referenced by each route function are isolated"""
+    """
+    A proxy for the Pait plugin, Ensure plugins referenced by each route function are isolated
+
+    Note: The plug-in will expose the build method to the user,
+        and the user does not need to call it directly `PluginManager`
+    """
 
     def __init__(self, plugin_class: Type[_PluginT], **kwargs: Any):
         self.plugin_class: Type[_PluginT] = plugin_class
         self._kwargs: Any = kwargs
 
     def pre_check_hook(self, pait_core_model: "PaitCoreModel") -> None:
         self.plugin_class.pre_check_hook(pait_core_model, self._kwargs)
 
     def pre_load_hook(self, pait_core_model: "PaitCoreModel") -> None:
         self._kwargs = self.plugin_class.pre_load_hook(pait_core_model, self._kwargs)
 
-    def get_plugin(self) -> _PluginT:
-        return self.plugin_class(**self._kwargs)
+    def get_plugin(self, next_plugin: _NextPluginT, pait_core_model: "PaitCoreModel") -> _PluginT:
+        return self.plugin_class(next_plugin, pait_core_model, **self._kwargs)
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.plugin_class.__name__}>"
```

### Comparing `pait-0.8.0.2/pait/plugin/base_mock_response.py` & `pait-1.0.0a1/pait/plugin/check_json_resp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,55 @@
-from abc import ABC
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Type
+from typing import TYPE_CHECKING, Any, Callable, Dict, Type
 
-from pait.model.response import PaitBaseResponseModel
-from pait.plugin.base import PluginManager, PluginProtocol
+from pait.model.response import BaseResponseModel, JsonResponseModel
+from pait.plugin.base import PluginContext, PrePluginProtocol
 from pait.util import get_pait_response_model
 
 if TYPE_CHECKING:
     from pait.model.core import PaitCoreModel
 
 
-class MockPluginProtocol(PluginProtocol):
-    """Automatically return a json response with sample values based on the response object
-    Note: the code logic of the routing function will not be executed
-    """
+class CheckJsonRespPlugin(PrePluginProtocol):
+    """Check if the json response result is legal"""
 
-    pait_response_model: Type[PaitBaseResponseModel]
+    check_resp_fn: Callable[[Any, PluginContext], None]
+
+    @staticmethod
+    def get_json(response_data: Any, context: PluginContext) -> dict:
+        raise NotImplementedError()
 
     @classmethod
     def pre_check_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> None:
         super().pre_check_hook(pait_core_model, kwargs)
-        if not pait_core_model.response_model_list:
-            raise RuntimeError(f"{pait_core_model.func} can not found response model")
-        if "pait_response_model" in kwargs:
+        if "check_resp_fn" in kwargs:
             raise RuntimeError("Please use response_model_list param")
 
     @classmethod
     def pre_load_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> Dict:
         kwargs = super().pre_load_hook(pait_core_model, kwargs)
-        pait_response: Optional[Type[PaitBaseResponseModel]] = None
-        enable_mock_response_filter_fn: Optional[Callable] = kwargs.pop("enable_mock_response_filter_fn", None)
-        if enable_mock_response_filter_fn and pait_core_model.response_model_list:
-            for _pait_response in pait_core_model.response_model_list:
-                if enable_mock_response_filter_fn(_pait_response):
-                    pait_response = _pait_response
-                    break
-
-        if not pait_response:
-            pait_response = get_pait_response_model(
-                pait_core_model.response_model_list,
-                target_pait_response_class=kwargs.pop("target_pait_response_class", False),
-                find_core_response_model=kwargs.pop("find_coro_response_model", None),
-            )
-        kwargs["pait_response_model"] = pait_response
-        return kwargs
-
-    def mock_response(self) -> Any:
-        raise NotImplementedError()
-
-    @classmethod
-    def build(  # type: ignore
-        cls,  # type: ignore
-        enable_mock_response_filter_fn: Optional[Callable] = None,  # type: ignore
-        target_pait_response_class: Optional[Type["PaitBaseResponseModel"]] = None,  # type: ignore
-        find_core_response_model: bool = False,  # type: ignore
-    ) -> "PluginManager":  # type: ignore
-        return super().build(
-            enable_mock_response_filter_fn=enable_mock_response_filter_fn,
-            target_pait_response_class=target_pait_response_class,
-            find_core_response_model=find_core_response_model,
-        )
-
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
-        return self.mock_response()
-
-
-class BaseMockPlugin(MockPluginProtocol, ABC):
-    """"""
+        pait_response_model: Type[BaseResponseModel] = get_pait_response_model(pait_core_model.response_model_list)
+        if not issubclass(pait_response_model, JsonResponseModel):
+            raise ValueError(f"pait_response_model must {JsonResponseModel} not {pait_response_model}")
+
+        def check_resp_by_dict(response_data: Any, context: PluginContext) -> None:
+            if not isinstance(response_data, dict):
+                response_data = cls.get_json(response_data, context)
+            pait_response_model.response_data(**response_data)  # type: ignore
 
+        kwargs["check_resp_fn"] = check_resp_by_dict
+        return kwargs
 
-class BaseAsyncMockPlugin(MockPluginProtocol, ABC):
-    """"""
+    def _sync_call(self, context: PluginContext) -> Any:
+        response: Any = super().__call__(context)
+        self.check_resp_fn(response, context)
+        return response
+
+    async def _async_call(self, context: PluginContext) -> Any:
+        response: Any = await super().__call__(context)
+        self.check_resp_fn(response, context)
+        return response
+
+    def __call__(self, context: PluginContext) -> Any:
+        if self._is_async_func:
+            return self._async_call(context)
+        else:
+            return self._sync_call(context)
```

### Comparing `pait-0.8.0.2/pait/plugin/cache_response.py` & `pait-1.0.0a1/pait/plugin/cache_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,164 +1,189 @@
 import pickle
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Set, Tuple, Type, Union
 
-from redis import Redis  # type: ignore
-from redis.asyncio import Redis as AsyncioRedis  # type: ignore
+from redis.asyncio import Redis  # type: ignore
+from redis.asyncio import Redis as AsyncioRedis
 
 from pait.app import set_app_attribute
+from pait.field import BaseField, ExtraParam
 from pait.g import pait_context
-from pait.model.response import PaitFileResponseModel
-from pait.plugin.base import PluginProtocol
+from pait.model.response import FileResponseModel
+from pait.plugin.base import PluginContext, PostPluginProtocol
+from pait.util import FuncSig, get_func_sig
 
 if TYPE_CHECKING:
     from pait.model.core import PaitCoreModel
     from pait.plugin.base import PluginManager
 
 
-_cache_plugin_redis_key: str = "_cache_plugin_redis"
+class CacheRespExtraParam(ExtraParam):
+    pass
 
 
-class CacheResponsePlugin(PluginProtocol):
-    is_pre_core: bool = False
+class CacheResponsePlugin(PostPluginProtocol):
+    _cache_plugin_redis_key: str = "_cache_plugin_redis"
+    _cache_name_param_set: Set[str] = set()
+
     name: str
     lock_name: str
     include_exc: Optional[Tuple[Type[Exception]]] = None
     redis: Union[Redis, AsyncioRedis, None] = None
     enable_cache_name_merge_param: bool
     cache_time: Optional[int]
     timeout: Optional[float]
     sleep: Optional[float]
     blocking_timeout: Optional[float]
 
-    def __post_init__(self, pait_core_model: "PaitCoreModel", args: tuple, kwargs: dict) -> None:
+    def __post_init__(self, **kwargs: Any) -> None:
         self.lock_name: str = self.name + ":" + "lock"
 
     @classmethod
     def check_redis(cls, redis: Union[Redis, AsyncioRedis]) -> None:
         if redis.connection_pool.connection_kwargs["decode_responses"] is False:
             raise ValueError("Please set redis`s param:decode_responses to True")
 
     @classmethod
     def set_redis_to_app(cls, app: Any, redis: Union[Redis, AsyncioRedis]) -> None:
         cls.check_redis(redis)
-        set_app_attribute(app, _cache_plugin_redis_key, redis)
+        set_app_attribute(app, cls._cache_plugin_redis_key, redis)
 
     @classmethod
     def pre_check_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> None:
         super().pre_check_hook(pait_core_model, kwargs)
         if not pait_core_model.response_model_list:
             raise RuntimeError(f"{pait_core_model.func} can not found response model")
-        if issubclass(pait_core_model.response_model_list[0], PaitFileResponseModel):
+        if issubclass(pait_core_model.response_model_list[0], FileResponseModel):
             raise RuntimeError(
                 f"Not use {cls.__name__} in {pait_core_model.func.__name__}, "
-                f"{cls.__name__} not support {PaitFileResponseModel.__class__.__name__}"
+                f"{cls.__name__} not support {FileResponseModel.__class__.__name__}"
             )
         if kwargs.get("redis", None) is not None:
             cls.check_redis(kwargs["redis"])
+        return None
 
     @classmethod
     def pre_load_hook(cls, pait_core_model: "PaitCoreModel", kwargs: Dict) -> Dict:
         super().pre_load_hook(pait_core_model, kwargs)
         name: str = kwargs.get("name", "")
         if not name:
             kwargs["name"] = pait_core_model.func.__qualname__
+
+        cache_name_param_set: Set[str] = set()
+        fun_sig: FuncSig = get_func_sig(pait_core_model.func)
+        for param in fun_sig.param_list:
+            default: Any = param.default
+            if not isinstance(default, BaseField):
+                continue
+            for extra_param in default.extra_param_list:
+                if not isinstance(extra_param, CacheRespExtraParam):
+                    continue
+                cache_name_param_set.add(default.alias or param.name)
+        kwargs["_cache_name_param_set"] = cache_name_param_set
         return kwargs
 
     def _get_redis(self) -> Union[Redis, AsyncioRedis]:
         redis: Union[Redis, AsyncioRedis, None] = self.redis or pait_context.get().app_helper.get_attributes(
-            _cache_plugin_redis_key, None
+            self._cache_plugin_redis_key, None
         )
         if not redis:
             raise ValueError("Not found redis client")
         return redis
 
+    def _loads(self, response: Any, *args: Any, **kwargs: Any) -> Any:
+        return pickle.loads(response.encode("latin1"))
+
+    def _dumps(self, response: Any, *args: Any, **kwargs: Any) -> Any:
+        return pickle.dumps(response).decode("latin1")
+
     def _gen_key(self, *args: Any, **kwargs: Any) -> Tuple[str, str]:
         real_key: str = self.name
         real_lock_key: str = self.lock_name
         if self.enable_cache_name_merge_param:
-            args_key_list: list = []
-            if args:
-                args_key_list = [str(i) for i in args]
+            args_key_list: list = [str(i) for i in args] if args else []
             if kwargs:
-                for value in kwargs.values():
-                    args_key_list.append(str(value))
+                if self._cache_name_param_set:
+                    for key, value in kwargs.items():
+                        if key not in self._cache_name_param_set:
+                            continue
+                        args_key_list.append(str(value))
+                else:
+                    for value in kwargs.values():
+                        args_key_list.append(str(value))
             if args_key_list:
-                real_key = f"{self.name}:{':'.join(args_key_list)}"
-                real_lock_key = f"{self.lock_name}:{':'.join(args_key_list)}"
+                key_join_str = ":".join(args_key_list)
+                real_key = f"{self.name}:{key_join_str}"
+                real_lock_key = f"{self.lock_name}:{key_join_str}"
         return real_key, real_lock_key
 
-    def _loads(self, response: Any, *args: Any, **kwargs: Any) -> Any:
-        return pickle.loads(response.encode("latin1"))
-
-    def _dumps(self, response: Any, *args: Any, **kwargs: Any) -> Any:
-        return pickle.dumps(response).decode("latin1")
-
-    async def _async_cache(self, func: Callable, *args: Any, **kwargs: Any) -> Any:
-        real_key, real_lock_key = self._gen_key(*args, **kwargs)
+    async def _async_cache(self, context: PluginContext) -> Any:
+        real_key, real_lock_key = self._gen_key(*context.args, **context.kwargs)
         redis: AsyncioRedis = self._get_redis()
         result: Any = await redis.get(real_key)
         if result:
-            result = self._loads(result, *args, **kwargs)
+            result = self._loads(result, *context.args, **context.kwargs)
         else:
             async with redis.lock(
                 real_lock_key,
                 timeout=self.timeout,
                 sleep=self.sleep,
                 blocking_timeout=self.blocking_timeout,
             ):
                 result = await redis.get(real_key)
                 if result:
-                    result = self._loads(result, *args, **kwargs)
+                    result = self._loads(result, *context.args, **context.kwargs)
                 else:
                     try:
-                        result = await func(*args, **kwargs)
+                        result = await super().__call__(context)
                     except Exception as e:
                         if self.include_exc and isinstance(e, self.include_exc):
                             result = e
                         else:
                             raise e
-                    await redis.set(real_key, self._dumps(result, *args, **kwargs), ex=self.cache_time)  # type: ignore
+                    await redis.set(  # type: ignore
+                        real_key, self._dumps(result, *context.args, **context.kwargs), ex=self.cache_time
+                    )
         if isinstance(result, Exception):
             raise result
         return result
 
-    def _cache(self, func: Callable, *args: Any, **kwargs: Any) -> Any:
-        real_key, real_lock_key = self._gen_key(*args, **kwargs)
+    def _cache(self, context: PluginContext) -> Any:
+        real_key, real_lock_key = self._gen_key(*context.args, **context.kwargs)
         redis: Redis = self._get_redis()
         result: Any = redis.get(real_key)
         if result:
-            result = self._loads(result, *args, **kwargs)
+            result = self._loads(result, *context.args, **context.kwargs)
         else:
             with redis.lock(
                 real_lock_key,
                 timeout=self.timeout,
                 sleep=self.sleep,
                 blocking_timeout=self.blocking_timeout,
             ):
                 result = redis.get(real_key)
                 if result:
-                    result = self._loads(result, *args, **kwargs)
+                    result = self._loads(result, *context.args, **context.kwargs)
                 else:
                     try:
-                        result = func(*args, **kwargs)
+                        result = super().__call__(context)
                     except Exception as e:
                         if self.include_exc and isinstance(e, self.include_exc):
                             result = e
                         else:
                             raise e
-                    redis.set(real_key, self._dumps(result, *args, **kwargs), ex=self.cache_time)
+                    redis.set(real_key, self._dumps(result, *context.args, **context.kwargs), ex=self.cache_time)
         if isinstance(result, Exception):
             raise result
         return result
 
-    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+    def __call__(self, context: PluginContext) -> Any:
         if self._is_async_func:
-            return self._async_cache(self.call_next, *args, **kwargs)
+            return self._async_cache(context)
         else:
-            return self._cache(self.call_next, *args, **kwargs)
+            return self._cache(context)
 
     @classmethod
     def build(  # type: ignore
         cls,
         *,
         redis: Union[Redis, AsyncioRedis, None] = None,
         include_exc: Optional[Tuple[Type[Exception]]] = None,
```

### Comparing `pait-0.8.0.2/pait/types.py` & `pait-1.0.0a1/pait/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import sys
+from typing import Any, Callable, Union
 
 # copy from https://github.com/agronholm/typeguard/blob/master/src/typeguard/__init__.py#L64
 if sys.version_info >= (3, 10):
     from typing import ParamSpec  # pragma: no cover
     from typing import is_typeddict  # pragma: no cover
-    from typing import Literal
+    from typing import Literal, Protocol
 else:
     from typing_extensions import ParamSpec  # type: ignore
-    from typing_extensions import Literal
+    from typing_extensions import Literal, Protocol
 
     _typed_dict_meta_types = ()
     if sys.version_info >= (3, 8):
         from typing import _TypedDictMeta  # pragma: no cover
 
         _typed_dict_meta_types += (_TypedDictMeta,)  # pragma: no cover
 
@@ -22,8 +23,15 @@
     except ImportError:  # pragma: no cover
         pass
 
     def is_typeddict(tp) -> bool:  # type: ignore
         return isinstance(tp, _typed_dict_meta_types)
 
 
-__all__ = ["ParamSpec", "Literal", "is_typeddict"]
+class _CallType(Protocol):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        ...
+
+
+CallType = Union[Callable, _CallType]
+
+__all__ = ["ParamSpec", "Literal", "is_typeddict", "CallType"]
```

### Comparing `pait-0.8.0.2/pait/util/__init__.py` & `pait-1.0.0a1/pait/util/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # flake8: noqa: F403
 from ._func_sig import *  # type: ignore
 from ._gen_tip import *  # type: ignore
-from ._i18n import *  # type: ignore
 from ._lazy_property import *  # type: ignore
 from ._pydantic_util import *  # type: ignore
 from ._types import *  # type: ignore
 from ._util import *  # type: ignore
 
 __all__ = [
     _func_sig.__all__  # type: ignore
     + _gen_tip.__all__  # type: ignore
-    + _i18n.__all__  # type: ignore
     + _lazy_property.__all__  # type: ignore
     + _pydantic_util.__all__  # type: ignore
     + _types.__all__  # type: ignore
     + _util.__all__  # type: ignore
 ]
```

### Comparing `pait-0.8.0.2/pait/util/_func_sig.py` & `pait-1.0.0a1/pait/util/_func_sig.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from dataclasses import dataclass
-from typing import Callable, Dict, List, Optional, Type
+from typing import Any, Callable, Dict, List, Optional, Type
 
 from typing_extensions import Self  # type: ignore
 
 from ._util import get_real_annotation
 
 __all__ = ["FuncSig", "get_func_sig", "is_bounded_func"]
 
@@ -12,25 +12,30 @@
 @dataclass()
 class FuncSig:
     """func inspect.Signature model"""
 
     func: Callable
     sig: "inspect.Signature"
     param_list: List["inspect.Parameter"]
+    return_param: Any
     cbv_class: Optional[Type] = None
 
 
 _func_sig_dict: Dict[Callable, FuncSig] = {}
 
 
 def get_func_sig(func: Callable) -> FuncSig:
     """get func inspect.Signature model"""
     if func in _func_sig_dict:
         return _func_sig_dict[func]
 
+    # __call__ method that supports func override
+    if getattr(func, "_override_call_sig", False):
+        func = getattr(func, "__call__", func)
+
     sig: inspect.Signature = inspect.signature(func)
     param_list: List[inspect.Parameter] = []
     for key in sig.parameters:
         # NOTE:
         #   The cbv func decorated in Pait is unbound, so it can get to self；
         #   Depend func must be bound func when it is used, so it cannot get self；
         if not (sig.parameters[key].annotation != sig.empty or sig.parameters[key].name == "self"):
@@ -38,15 +43,16 @@
                 # If the name of the self variable is not self and the annotation is not Self,
                 # it will be ignored directly
                 continue
         parameter: inspect.Parameter = sig.parameters[key]
         setattr(parameter, "_annotation", get_real_annotation(parameter.annotation, func))
         param_list.append(parameter)
 
-    # return_param = sig.return_annotation
-    func_sig: FuncSig = FuncSig(func=func, sig=sig, param_list=param_list)
+    func_sig: FuncSig = FuncSig(
+        func=func, sig=sig, param_list=param_list, return_param=get_real_annotation(sig.return_annotation, func)
+    )
     _func_sig_dict[func] = func_sig
     return func_sig
 
 
 def is_bounded_func(func: Callable) -> bool:
     return inspect.signature(func).parameters.get("self", None) is None
```

### Comparing `pait-0.8.0.2/pait/util/_gen_tip.py` & `pait-1.0.0a1/pait/util/_gen_tip.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 from pait.util import FuncSig
 
 _indent: str = 4 * " "
 
 __all__ = ["gen_tip_exc"]
 
 
-def gen_tip_exc(_object: Any, exception: "Exception", parameter: Optional[inspect.Parameter] = None) -> Exception:
+def gen_tip_exc(
+    _object: Any,
+    exception: "Exception",
+    parameter: Optional[inspect.Parameter] = None,
+    tip_exception_class: Optional[Type[TipException]] = TipException,
+) -> Exception:
     """Help users understand which parameter is wrong"""
-    if _object is None:
-        return exception
-    if isinstance(exception, TipException):
+    if _object is None or tip_exception_class is None or isinstance(exception, TipException):
         return exception
+
     if parameter:
         param_value: BaseField = parameter.default
         annotation: Type[BaseModel] = parameter.annotation
         param_name: str = parameter.name
 
         parameter_value_name: str = param_value.__class__.__name__
         if param_value is parameter.empty:
@@ -66,8 +70,8 @@
     logging.debug(error_source_tip)
     exc_msg: str = (
         f"{str(exception)} for {_object}   Customer Traceback:\n"
         f'{_indent}File "{file}",'
         f" line {line},"
         f" in {error_object_name}."
     )
-    return TipException(exc_msg, exception)
+    return tip_exception_class(exc_msg, exception)
```

### Comparing `pait-0.8.0.2/pait/util/_lazy_property.py` & `pait-1.0.0a1/pait/util/_lazy_property.py`

 * *Files identical despite different names*

### Comparing `pait-0.8.0.2/pait/util/_util.py` & `pait-1.0.0a1/pait/util/_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 import inspect
 import json
 import os
 import sys
 from dataclasses import MISSING
-from datetime import date, datetime
+from datetime import datetime
 from decimal import Decimal
 from enum import Enum
 from functools import wraps
 from json import JSONEncoder
-from typing import _eval_type  # type: ignore
-from typing import (
+from typing import (  # type: ignore
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     ForwardRef,
     List,
     Optional,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
+    _eval_type,
+    _GenericAlias,
     get_type_hints,
 )
 
 from pydantic import BaseModel
-from pydantic.fields import Undefined, UndefinedType
+from pydantic.fields import FieldInfo, Undefined, UndefinedType
+from typing_extensions import is_typeddict
 
 from pait.field import BaseField, Depends, is_pait_field
-from pait.model.template import TemplateVar
 from pait.types import ParamSpec
 
 from ._types import ParseTypeError, parse_typing
 
 if TYPE_CHECKING:
-    from pait.model.response import PaitBaseResponseModel
+    from pait.model.response import BaseResponseModel
 
 __all__ = [
     "gen_example_dict_from_pydantic_base_model",
     "gen_example_dict_from_schema",
     "gen_example_json_from_schema",
     "get_parameter_list_from_pydantic_basemodel",
     "get_parameter_list_from_class",
-    "CustomJSONEncoder",
     "http_method_tuple",
     "json_type_default_value_dict",
     "python_type_default_value_dict",
     "get_pait_response_model",
     "example_value_handle",
     "ignore_pre_check",
     "gen_example_value_from_python",
     "get_real_annotation",
     "create_factory",
+    "partial_wrapper",
+    "R_T",
+    "P",
 ]
 ignore_pre_check: bool = bool(os.environ.get("PAIT_IGNORE_PRE_CHECK", False))
 http_method_tuple: Tuple[str, ...] = ("get", "post", "head", "options", "delete", "put", "trace", "patch")
 
 json_type_default_value_dict: Dict[str, Any] = {
     "null": None,
     "bool": True,
@@ -65,164 +68,198 @@
     "number": 0.0,
     "float": 0.0,
     "integer": 0,
     "object": {},
     "array": [],
 }
 
-python_type_default_value_dict: Dict[type, Any] = {
+python_type_default_value_dict: Dict = {
     bool: True,
     float: 0.0,
     int: 0,
     str: "",
     list: [],
     tuple: (),
     dict: {},
     datetime: datetime.fromtimestamp(0),
     Decimal: Decimal("0.0"),
+    Any: {},
 }
 
 
 P = ParamSpec("P")
 R_T = TypeVar("R_T")
 
 
-def create_factory(func: Callable[P, R_T]) -> Callable[P, R_T]:  # type: ignore
+def create_factory(func: Callable[P, R_T]) -> Callable[P, Callable[[], R_T]]:
+    """Create a factory that calls the function (Use the syntax hints provided by PEP 612)"""
+
+    @wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Callable[[], R_T]:
+        return lambda: func(*args, **kwargs)
+
+    return wrapper
+
+
+def partial_wrapper(func: Callable[P, R_T], **_customer_kwargs: Any) -> Callable[P, R_T]:  # type: ignore
+    """with type hints partial"""
+
     @wraps(func)
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> R_T:  # type: ignore
-        return lambda: func(*args, **kwargs)  # type: ignore
+        new_kwargs = _customer_kwargs.copy()
+        new_kwargs.update(kwargs)
+        return func(*args, **new_kwargs)
 
     return wrapper
 
 
 def example_value_handle(example_value: Any) -> Any:
-    if getattr(example_value, "__call__", None):
-        example_value = example_value()
-    elif isinstance(example_value, Enum):
+    if isinstance(example_value, Enum):
         example_value = example_value.value
-    elif isinstance(example_value, TemplateVar):
-        example_value = example_value.get_value_from_template_context()
+    elif getattr(example_value, "__call__", None):
+        example_value = example_value()
     return example_value
 
 
 def get_real_annotation(annotation: Union[Type, str], target_obj: Any) -> Type:
+    """
+    get the real annotation from postponed annotations/annotations
+    :param annotation: type hints
+    :param target_obj: The object on which the annotation resides
+    :return: the real annotation
+
+    e.g:
+    >>> def demo(a: "int") -> int: pass
+    >>> assert int = get_real_annotation(demo.__annotations__["a"], demo)
+
+    >>> class Demo:
+    >>>     a: "int"
+    >>> assert int = get_real_annotation(Demo.__annotations__["a"], Demo)
+    """
     global_dict = sys.modules[target_obj.__module__].__dict__
     if not isinstance(annotation, str):
+        # Option["Dict[str, int]"]
         return _eval_type(annotation, global_dict, None)
     if inspect.isclass(target_obj) and annotation in target_obj.__dict__:
         new_annotation: Type = target_obj.__dict__[annotation]
     else:
         # get real type
         value: ForwardRef = ForwardRef(annotation, is_argument=False)
-        new_annotation = value._evaluate(global_dict, None)  # type: ignore
+
+        if sys.version_info >= (3, 9):
+            new_annotation = value._evaluate(global_dict, None, frozenset())  # type: ignore
+        else:
+            new_annotation = value._evaluate(global_dict, None)  # type: ignore
         if not new_annotation:
             raise RuntimeError(f"get real annotation from {target_obj} fail")  # pragma: no cover
     return _eval_type(new_annotation, global_dict, None)
 
 
 def get_pydantic_annotation(key: str, pydantic_base_model: Type[BaseModel]) -> Type:
+    """Get the annotation from BaseModel's properties"""
     annotation: Any = MISSING
     for base in reversed(pydantic_base_model.__mro__):
         ann: Union[str, Type] = base.__dict__.get("__annotations__", {}).get(key, MISSING)
         if ann is not MISSING:
             annotation = ann
             break
     if annotation is MISSING:
-        raise RuntimeError(f"get annotation from {pydantic_base_model} fail")  # pragma: no cover
+        raise RuntimeError(f"get {key}'s annotation from {pydantic_base_model} fail")  # pragma: no cover
     annotation = get_real_annotation(annotation, pydantic_base_model)
 
     if getattr(annotation, "real", None) and annotation != bool:
         # support like pydantic.ConstrainedIntValue
         annotation = annotation.real.__objclass__  # type: ignore
     return annotation
 
 
 def get_pait_response_model(
-    response_model_list: List[Type["PaitBaseResponseModel"]],
-    target_pait_response_class: Optional[Type["PaitBaseResponseModel"]] = None,
-    find_core_response_model: bool = False,
-) -> Type["PaitBaseResponseModel"]:
+    response_model_list: List[Type["BaseResponseModel"]],
+    target_pait_response_class: Optional[Type["BaseResponseModel"]] = None,
+) -> Type["BaseResponseModel"]:
     if target_pait_response_class:
-        core_response_list: List[Type["PaitBaseResponseModel"]] = [
-            i for i in response_model_list if i.is_core and issubclass(i, target_pait_response_class)
-        ]
-    else:
-        core_response_list = [i for i in response_model_list if i.is_core]
-    if find_core_response_model:
-        if len(core_response_list) != 1:
-            raise RuntimeError("Multiple pait response models were found")
-        return core_response_list[0]
-    else:
-        return (core_response_list or response_model_list)[0]
+        response_model_list = [i for i in response_model_list if issubclass(i, target_pait_response_class)]
+    return response_model_list[0]
 
 
 def gen_example_value_from_python(obj: Any) -> Any:
     if isinstance(obj, dict):
-        new_dict: dict = {}
-        for key, value in obj.items():
-            new_dict[key] = gen_example_value_from_python(value)
-        return new_dict
+        return {key: gen_example_value_from_python(value) for key, value in obj.items()}
     else:
         return python_type_default_value_dict.get(type(obj), obj)
 
 
+def gen_example_value_from_type(value_type: type, example_column_name: str = "example") -> Any:
+    """
+    Gets the default value for type
+    :param value_type: type of the value
+    :param example_column_name: Gets sample values from the properties specified by pydantic.FieldInfo
+    """
+    if is_typeddict(value_type):
+        return {k: gen_example_value_from_type(v) for k, v in value_type.__annotations__.items()}
+    elif isinstance(value_type, _GenericAlias):
+        sub_type: Optional[Type] = None
+        try:
+            parse_typing_result = parse_typing(value_type)
+            # If there is more than one type value, only the first one is used
+            real_type: Type = parse_typing_result[0]
+            annotation_arg_list: list = getattr(value_type, "__args__", [])
+            if annotation_arg_list:
+                sub_type_set: Set[Type] = set(annotation_arg_list)
+                if len(sub_type_set) == 1:
+                    sub_type = sub_type_set.pop()
+        except ParseTypeError:
+            real_type = value_type
+        if real_type is list and sub_type:
+            return [gen_example_value_from_type(sub_type, example_column_name=example_column_name)]
+        else:
+            # if real_type is Option[xxx], sub_type is None
+            # so must parse real_type
+            return gen_example_value_from_type(real_type, example_column_name=example_column_name)
+    elif not inspect.isclass(value_type):
+        return python_type_default_value_dict[value_type]
+    elif issubclass(value_type, Enum):
+        return [i for i in value_type.__members__.values()][0].value
+    elif issubclass(value_type, BaseModel):
+        return gen_example_dict_from_pydantic_base_model(value_type, example_column_name=example_column_name)
+    else:
+        return python_type_default_value_dict[value_type]
+
+
 def gen_example_dict_from_pydantic_base_model(
-    pydantic_base_model: Type[BaseModel], use_example_value: bool = True
+    pydantic_base_model: Type[BaseModel], example_column_name: str = "example"
 ) -> dict:
+    """
+    Gets the default value for pydantic.BaseModel
+    :param pydantic_base_model: pydantic.BaseModel
+    :param example_column_name: Gets sample values from the properties specified by pydantic.FieldInfo
+    """
     gen_dict: Dict[str, Any] = {}
     for key, model_field in pydantic_base_model.__fields__.items():
-        if use_example_value:
-            example_value: Any = model_field.field_info.extra.get("example", Undefined)
+        if model_field.alias:
+            key = model_field.alias
+        if example_column_name:
+            example_value: Any = model_field.field_info.extra.get(example_column_name, Undefined)
             if not isinstance(example_value, UndefinedType):
                 gen_dict[key] = example_value_handle(example_value)
                 continue
 
         if not isinstance(model_field.field_info.default, UndefinedType):
             gen_dict[key] = model_field.field_info.default
         elif model_field.field_info.default_factory and not isinstance(
             model_field.field_info.default_factory, UndefinedType
         ):
             gen_dict[key] = model_field.field_info.default_factory()
         else:
             annotation: Type = get_pydantic_annotation(key, pydantic_base_model)
-
-            if inspect.isclass(annotation) and issubclass(annotation, BaseModel):
-                gen_dict[key] = gen_example_dict_from_pydantic_base_model(annotation)
-            else:
-                sub_type: Optional[Type] = None
-                try:
-                    parse_typing_result: Union[List[Type[Any]], Type] = parse_typing(annotation)
-                    if isinstance(parse_typing_result, list):
-                        real_type: Type = parse_typing_result[0]
-                    else:
-                        real_type = parse_typing_result
-                    if getattr(annotation, "__args__", None):
-                        sub_type_set: Set[Type] = set(annotation.__args__)
-                        if len(sub_type_set) == 1:
-                            sub_type = sub_type_set.pop()
-                except ParseTypeError:
-                    real_type = annotation
-                if (
-                    real_type is list
-                    and sub_type is not None
-                    and inspect.isclass(sub_type)
-                    and issubclass(sub_type, BaseModel)
-                ):
-                    gen_dict[key] = [gen_example_dict_from_pydantic_base_model(sub_type)]
-                elif issubclass(real_type, Enum):
-                    gen_dict[key] = [i for i in real_type.__members__.values()][0].value
-                else:
-                    gen_dict[key] = python_type_default_value_dict[real_type]
+            gen_dict[key] = gen_example_value_from_type(annotation, example_column_name=example_column_name)
     return gen_dict
 
 
-def gen_example_dict_from_schema(
-    schema_dict: Dict[str, Any],
-    definition_dict: Optional[dict] = None,
-) -> Dict[str, Any]:
+def gen_example_dict_from_schema(schema_dict: Dict[str, Any], definition_dict: Optional[dict] = None) -> Dict[str, Any]:
     gen_dict: Dict[str, Any] = {}
     if "properties" not in schema_dict:
         return gen_dict
     property_dict: Dict[str, Any] = schema_dict["properties"]
     if not definition_dict:
         _definition_dict: dict = schema_dict.get("definitions", {})
     else:
@@ -254,32 +291,43 @@
     return gen_dict
 
 
 def gen_example_json_from_schema(schema_dict: Dict[str, Any], cls: Optional[Type[JSONEncoder]] = None) -> str:
     return json.dumps(gen_example_dict_from_schema(schema_dict), cls=cls)
 
 
-def get_parameter_list_from_pydantic_basemodel(pait_model: Type[BaseModel]) -> List["inspect.Parameter"]:
+def get_parameter_list_from_pydantic_basemodel(
+    pait_model: Type[BaseModel], default_field_class: Optional[Type[BaseField]] = None
+) -> List["inspect.Parameter"]:
     """get class parameter list by attributes, if attributes not default value, it will be set `Undefined`"""
-    parameter_list: Optional[List["inspect.Parameter"]] = getattr(pait_model, "_parameter_list", None)
+    key = f"_parameter_list:{default_field_class}"
+    parameter_list: Optional[List["inspect.Parameter"]] = getattr(pait_model, key, None)
     if parameter_list is not None:
         return parameter_list
     parameter_list = []
     for key, model_field in pait_model.__fields__.items():
-        if not is_pait_field(model_field.field_info):
-            raise TypeError(f"{model_field.field_info} must instance {BaseField} or {Depends}")  # pragma: no cover
+        field: FieldInfo = model_field.field_info
+        if not is_pait_field(field):
+            if not default_field_class:
+                raise TypeError(  # pragma: no cover
+                    f"{field.__class__} must instance {BaseField} or {Depends} by model {pait_model}"
+                )
+            field = default_field_class.from_pydantic_field(field)
+
+            if getattr(field, "alias", None) is None:
+                field.request_key = key
         parameter = inspect.Parameter(
             key,
             inspect.Parameter.POSITIONAL_ONLY,
-            default=model_field.field_info,
+            default=field,
             annotation=get_pydantic_annotation(key, pait_model),
         )
         parameter_list.append(parameter)
 
-    setattr(pait_model, "_parameter_list", parameter_list)
+    setattr(pait_model, key, parameter_list)
     return parameter_list
 
 
 _class_parameter_list_dict: Dict[type, List["inspect.Parameter"]] = {}
 
 
 def get_parameter_list_from_class(cbv_class: Type) -> List["inspect.Parameter"]:
@@ -302,26 +350,7 @@
                 inspect.Parameter.POSITIONAL_ONLY,
                 default=default,
                 annotation=param_annotation,
             )
             parameter_list.append(parameter)
     _class_parameter_list_dict[cbv_class] = parameter_list
     return parameter_list
-
-
-class CustomJSONEncoder(JSONEncoder):
-    def default(self, obj: Any) -> Any:
-        if isinstance(obj, datetime):
-            return int(obj.timestamp())
-        elif isinstance(obj, date):
-            return obj.strftime("%Y-%m-%d")
-        elif isinstance(obj, Decimal):
-            return float(obj)
-        elif isinstance(obj, Enum):
-            return obj.value
-        elif isinstance(obj, TemplateVar):
-            obj = obj.get_value_from_template_context()
-            if isinstance(obj, UndefinedType):
-                obj = None
-            return obj
-        else:
-            return super().default(obj)  # pragma: no cover
```

### Comparing `pait-0.8.0.2/pait/util/grpc_inspect/stub.py` & `pait-1.0.0a1/pait/grpc/inspect.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,125 @@
 import inspect
 import json
 import logging
 import re
 from dataclasses import dataclass
 from types import ModuleType
-from typing import Any, Dict, List, Optional, Tuple, Type
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from google.protobuf.descriptor import MethodDescriptor, ServiceDescriptor  # type: ignore
-from pydantic import BaseModel, Field
+from google.protobuf.json_format import MessageToDict  # type: ignore
+from pydantic import BaseModel, Field, validator
 
-from pait.util.grpc_inspect.types import Message
+from pait.grpc.types import Message
 
-
-class GrpcServiceModel(BaseModel):
-    name: str = Field("")
-    tag: List[Tuple[str, str]] = Field(default_factory=list)
-    group: str = Field("")
-    desc: str = Field("")
-    summary: str = Field("")
-    url: str = Field("")
-    enable: bool = Field(True)
+__all__ = [
+    "BuildMessageModel",
+    "GrpcServiceOptionModel",
+    "GrpcModel",
+    "get_grpc_service_model_from_option_message",
+    "ParseStub",
+]
+
+
+class BuildMessageModel(BaseModel):
+    exclude_column_name: list = Field(default_factory=list)
+    nested: list = Field(default_factory=list)
+
+    @validator("exclude_column_name", pre=True)
+    def exclude_column_name_validator(cls, v: Union[str, list]) -> list:
+        if isinstance(v, str):
+            return [i for i in v.split(",") if i]
+        return v
+
+    @validator("nested", pre=True)
+    def nested_validator(cls, v: Union[str, list]) -> list:
+        if isinstance(v, str):
+            return [i for i in v.split("/") if i]
+        return v
+
+
+class RequestBuildMessageModel(BuildMessageModel):
+    @validator("nested", pre=True)
+    def nested_validator(cls, v: Union[str, list]) -> list:
+        if isinstance(v, str):
+            return [i for i in v.split("/") if i if not i.startswith("$")]
+        return v
+
+
+class GrpcServiceOptionModel(BaseModel):
+    """grpc service option"""
+
+    name: str = Field("", description="service name")
+    author: Tuple[str] = Field(default_factory=tuple, description="service author")
+    tag: List[Tuple[str, str]] = Field(default_factory=list, description="service openapi tag")
+    group: str = Field("", description="service pait group")
+    desc: str = Field("", description="service openapi description")
+    summary: str = Field("", description="service openapi summary")
+    url: str = Field("", description="service url")
+    enable: bool = Field(True, description="Whether to enable this service")
     http_method: str = Field("POST")
+    request_message: RequestBuildMessageModel = Field(
+        default_factory=RequestBuildMessageModel, description="request message"
+    )
+    response_message: BuildMessageModel = Field(default_factory=BuildMessageModel, description="response message")
 
 
 @dataclass()
 class GrpcModel(object):
     invoke_name: str
-    method: str
-    alias_method: str
-    grpc_service_model: GrpcServiceModel
+    grpc_method_url: str
+    alias_grpc_method_url: str
+    grpc_service_option_model: GrpcServiceOptionModel
     # func: Callable
     request: Type[Message] = Message
     response: Type[Message] = Message
     desc: str = ""
 
 
+def get_grpc_service_model_from_option_message(option_message: Message) -> List[GrpcServiceOptionModel]:
+    grpc_service_model_list: List[GrpcServiceOptionModel] = []
+    pait_dict: dict = {}
+    for rule_filed, value in option_message.ListFields():
+        key: str = rule_filed.name
+        if key == "tag":
+            pait_dict[key] = [(tag.name, tag.desc) for tag in value]
+        elif key == "not_enable":
+            pait_dict["enable"] = not value
+        elif rule_filed.containing_oneof:
+            if value.url:
+                pait_dict["url"] = value.url
+            if key == "custom":
+                logging.warning(f"Not support column:{key}")
+            elif key != "any":
+                pait_dict["http_method"] = key
+        elif key in ("body", "response_body"):
+            logging.warning(f"Not support column:{key}")
+        elif key == "additional_bindings":
+            for item in value:
+                grpc_service_model_list.extend(get_grpc_service_model_from_option_message(item))
+        elif key in ("request_message", "response_message"):
+            if isinstance(value, dict):
+                pait_dict[key] = value
+            else:
+                pait_dict[key] = MessageToDict(value, preserving_proto_field_name=True)
+        else:
+            pait_dict[key] = value
+
+    grpc_service_model: GrpcServiceOptionModel = GrpcServiceOptionModel(**pait_dict)
+    grpc_service_model.http_method = grpc_service_model.http_method.upper()
+    grpc_service_model_list.append(grpc_service_model)
+    return grpc_service_model_list
+
+
 class ParseStub(object):
     def __init__(self, stub: Any):
         self._stub: Any = stub
         self.name: str = self._stub.__name__
         self._method_list_dict: Dict[str, List[GrpcModel]] = {}
-
         self._filename_desc_dict: Dict[str, Dict[str, Dict[str, str]]] = {}
 
         self._parse()
 
     @property
     def method_list_dict(self) -> Dict[str, List[GrpcModel]]:
         return self._method_list_dict
@@ -61,114 +136,103 @@
         setattr(message_model, "_message_module", message_module)
 
         if not issubclass(message_model, Message):
             raise RuntimeError("Can not found message")
 
         return message_model
 
-    def get_grpc_service_model_from_option_message(self, option_message: Message) -> List[GrpcServiceModel]:
-        grpc_service_model_list: List[GrpcServiceModel] = []
-        pait_dict: dict = {}
-        for rule_filed, value in option_message.ListFields():
-            key: str = rule_filed.name
-            if key == "tag":
-                pait_dict[key] = [(tag.name, tag.desc) for tag in value]
-            elif key == "not_enable":
-                pait_dict["enable"] = not value
-            elif rule_filed.containing_oneof:
-                if value.url:
-                    pait_dict["url"] = value.url
-                if key == "custom":
-                    logging.warning(f"Not support column:{key}")
-                elif key != "any":
-                    pait_dict["http_method"] = key
-            elif key in ("body", "response_body"):
-                logging.warning(f"Not support column:{key}")
-            elif key == "additional_bindings":
-                for item in value:
-                    grpc_service_model_list.extend(self.get_grpc_service_model_from_option_message(item))
-            else:
-                pait_dict[key] = value
-        grpc_service_model: GrpcServiceModel = GrpcServiceModel(**pait_dict)
-        grpc_service_model.http_method = grpc_service_model.http_method.upper()
-        grpc_service_model_list.append(grpc_service_model)
-        return grpc_service_model_list
-
-    def get_service_by_message(
+    def get_service_option_from_message(
         self, input_message: Type[Message], out_message: Type[Message]
-    ) -> List[GrpcServiceModel]:
+    ) -> List[GrpcServiceOptionModel]:
         for message in [input_message, out_message]:
             message_module: ModuleType = getattr(message, "_message_module")
             server_list: List[ServiceDescriptor] = message_module.DESCRIPTOR.services_by_name.values()  # type: ignore
             for server_descriptor in server_list:
                 for method in server_descriptor.methods:
                     if not (
                         method.input_type.full_name == input_message.DESCRIPTOR.full_name
                         and method.output_type.full_name == out_message.DESCRIPTOR.full_name
                     ):
                         continue
                     if not method.GetOptions().ListFields():
                         continue
-                    for filed, option_message in method.GetOptions().ListFields():
-                        if not filed.full_name.endswith("api.http"):
+                    for field, option_message in method.GetOptions().ListFields():
+                        if not field.full_name.endswith("api.http"):
                             continue
-                        return self.get_grpc_service_model_from_option_message(option_message)
+                        return get_grpc_service_model_from_option_message(option_message)
         return []
 
     @staticmethod
-    def get_pait_info_from_grpc_desc(desc: str, service_desc: str) -> GrpcServiceModel:
+    def get_service_option_from_grpc_desc(desc: str, service_desc: str) -> List[GrpcServiceOptionModel]:
+        grpc_pait_model_list: List[GrpcServiceOptionModel] = []
         pait_dict: dict = {}
         for line in service_desc.split("\n") + desc.split("\n"):
             line = line.strip()
             if not line.startswith("pait: {"):
                 continue
             line = line.replace("pait:", "")
             pait_dict.update(json.loads(line))
-        grpc_pait_model: GrpcServiceModel = GrpcServiceModel(**pait_dict)
-        grpc_pait_model.http_method = grpc_pait_model.http_method.upper()
-        return grpc_pait_model
+
+        while True:
+            grpc_pait_model: GrpcServiceOptionModel = GrpcServiceOptionModel(**pait_dict)
+            grpc_pait_model.http_method = grpc_pait_model.http_method.upper()
+            grpc_pait_model_list.append(grpc_pait_model)
+            pait_dict = pait_dict.pop("additional_bindings", None)
+            if not pait_dict:
+                break
+
+        return grpc_pait_model_list
 
     def _parse(self) -> None:
+        # get stub source code
         line_list: List[str] = inspect.getsource(self._stub).split("\n")
 
+        # get grpc service
         service_class_name: str = self._stub.__name__.replace("Stub", "Servicer")
         class_module: Optional[ModuleType] = inspect.getmodule(self._stub)
         if not class_module:
             raise RuntimeError(f"Can not found {self._stub} module")
-
         service_class: Type = getattr(class_module, service_class_name)
 
+        # parse source code
         for index, line in enumerate(line_list):
+            # Only need to get the function signature (currently only support 'unary_unary')
             if "self." not in line:
                 continue
             if "channel.unary_unary" not in line:
                 continue
 
             invoke_name: str = line.split("=")[0].replace("self.", "").strip()
-            method: str = line_list[index + 1].strip()[1:-2]
+            # The next line of the calling method must be the URL of the gRPC method
+            grpc_method_url: str = line_list[index + 1].strip()[1:-2]
             request: Type[Message] = self._gen_message(
                 line_list[index + 2], r"request_serializer=(.+).SerializeToString", class_module
             )
             response: Type[Message] = self._gen_message(
                 line_list[index + 3], r"response_deserializer=(.+).FromString", class_module
             )
             service_desc: str = service_class.__doc__ or ""
             desc: str = service_class.__dict__[invoke_name].__doc__ or ""
-            grpc_service_model_list: List[GrpcServiceModel] = self.get_service_by_message(request, response)
-            if not grpc_service_model_list:
-                grpc_service_model_list = [self.get_pait_info_from_grpc_desc(desc, service_desc)]
+
+            # Get the Option for each method in the gRPC Service through protocol optional
+            grpc_service_option_model_list: List[GrpcServiceOptionModel] = self.get_service_option_from_message(
+                request, response
+            )
+            if not grpc_service_option_model_list:
+                # Get the Option for each method in the gRPC Service through comment
+                grpc_service_option_model_list = self.get_service_option_from_grpc_desc(desc, service_desc)
             grpc_model_list: List[GrpcModel] = []
-            for model_index, grpc_service_model in enumerate(grpc_service_model_list):
-                if not grpc_service_model.url:
-                    grpc_service_model.url = method
+            for model_index, grpc_service_option_model in enumerate(grpc_service_option_model_list):
+                if not grpc_service_option_model.url:
+                    grpc_service_option_model.url = grpc_method_url
                 grpc_model_list.append(
                     GrpcModel(
                         invoke_name=invoke_name,
-                        method=method,
-                        alias_method=method + str(model_index),
-                        grpc_service_model=grpc_service_model,
-                        desc=service_class.__dict__[invoke_name].__doc__ or "",
+                        grpc_method_url=grpc_method_url,
+                        alias_grpc_method_url=grpc_method_url + str(model_index),
+                        grpc_service_option_model=grpc_service_option_model,
+                        desc=desc,
                         request=request,
                         response=response,
                     )
                 )
-            self._method_list_dict[method] = grpc_model_list
+            self._method_list_dict[grpc_method_url] = grpc_model_list
```

### Comparing `pait-0.8.0.2/setup.py` & `pait-1.0.0a1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,277 +1,422 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
 00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
 00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
 00000040: 205c 0a5b 2770 6169 7427 2c0a 2027 7061   \.['pait',. 'pa
-00000050: 6974 2e61 7069 5f64 6f63 272c 0a20 2770  it.api_doc',. 'p
-00000060: 6169 742e 6170 695f 646f 632e 6874 6d6c  ait.api_doc.html
-00000070: 272c 0a20 2770 6169 742e 6170 7027 2c0a  ',. 'pait.app',.
-00000080: 2027 7061 6974 2e61 7070 2e62 6173 6527   'pait.app.base'
-00000090: 2c0a 2027 7061 6974 2e61 7070 2e66 6c61  ,. 'pait.app.fla
-000000a0: 736b 272c 0a20 2770 6169 742e 6170 702e  sk',. 'pait.app.
-000000b0: 666c 6173 6b2e 706c 7567 696e 272c 0a20  flask.plugin',. 
-000000c0: 2770 6169 742e 6170 702e 7361 6e69 6327  'pait.app.sanic'
-000000d0: 2c0a 2027 7061 6974 2e61 7070 2e73 616e  ,. 'pait.app.san
-000000e0: 6963 2e70 6c75 6769 6e27 2c0a 2027 7061  ic.plugin',. 'pa
-000000f0: 6974 2e61 7070 2e73 7461 726c 6574 7465  it.app.starlette
-00000100: 272c 0a20 2770 6169 742e 6170 702e 7374  ',. 'pait.app.st
-00000110: 6172 6c65 7474 652e 706c 7567 696e 272c  arlette.plugin',
-00000120: 0a20 2770 6169 742e 6170 702e 746f 726e  . 'pait.app.torn
-00000130: 6164 6f27 2c0a 2027 7061 6974 2e61 7070  ado',. 'pait.app
-00000140: 2e74 6f72 6e61 646f 2e70 6c75 6769 6e27  .tornado.plugin'
-00000150: 2c0a 2027 7061 6974 2e65 7874 7261 272c  ,. 'pait.extra',
-00000160: 0a20 2770 6169 742e 6874 7470 272c 0a20  . 'pait.http',. 
-00000170: 2770 6169 742e 6d6f 6465 6c27 2c0a 2027  'pait.model',. '
-00000180: 7061 6974 2e70 6c75 6769 6e27 2c0a 2027  pait.plugin',. '
-00000190: 7061 6974 2e75 7469 6c27 2c0a 2027 7061  pait.util',. 'pa
-000001a0: 6974 2e75 7469 6c2e 6772 7063 5f69 6e73  it.util.grpc_ins
-000001b0: 7065 6374 275d 0a0a 7061 636b 6167 655f  pect']..package_
-000001c0: 6461 7461 203d 205c 0a7b 2727 3a20 5b27  data = \.{'': ['
-000001d0: 2a27 5d7d 0a0a 696e 7374 616c 6c5f 7265  *']}..install_re
-000001e0: 7175 6972 6573 203d 205c 0a5b 2770 7964  quires = \.['pyd
-000001f0: 616e 7469 633e 3d31 2e37 2e33 2c3c 322e  antic>=1.7.3,<2.
-00000200: 302e 3027 2c20 2774 7970 696e 672d 6578  0.0', 'typing-ex
-00000210: 7465 6e73 696f 6e73 3e3d 342e 312e 312c  tensions>=4.1.1,
-00000220: 3c35 2e30 2e30 275d 0a0a 6578 7472 6173  <5.0.0']..extras
-00000230: 5f72 6571 7569 7265 203d 205c 0a7b 2761  _require = \.{'a
-00000240: 6c6c 273a 205b 2770 726f 746f 6275 662d  ll': ['protobuf-
-00000250: 746f 2d70 7964 616e 7469 633e 3d30 2e31  to-pydantic>=0.1
-00000260: 2e35 2c3c 302e 322e 3027 2c20 2772 6564  .5,<0.2.0', 'red
-00000270: 6973 3e3d 342e 322e 322c 3c35 2e30 2e30  is>=4.2.2,<5.0.0
-00000280: 275d 2c0a 2027 7072 6f74 6f62 7566 273a  '],. 'protobuf':
-00000290: 205b 2770 726f 746f 6275 662d 746f 2d70   ['protobuf-to-p
-000002a0: 7964 616e 7469 633e 3d30 2e31 2e35 2c3c  ydantic>=0.1.5,<
-000002b0: 302e 322e 3027 5d2c 0a20 2772 6564 6973  0.2.0'],. 'redis
-000002c0: 273a 205b 2772 6564 6973 3e3d 342e 322e  ': ['redis>=4.2.
-000002d0: 322c 3c35 2e30 2e30 275d 7d0a 0a73 6574  2,<5.0.0']}..set
-000002e0: 7570 5f6b 7761 7267 7320 3d20 7b0a 2020  up_kwargs = {.  
-000002f0: 2020 276e 616d 6527 3a20 2770 6169 7427    'name': 'pait'
-00000300: 2c0a 2020 2020 2776 6572 7369 6f6e 273a  ,.    'version':
-00000310: 2027 302e 382e 302e 3227 2c0a 2020 2020   '0.8.0.2',.    
-00000320: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
-00000330: 5061 6974 2069 7320 6120 5079 7468 6f6e  Pait is a Python
-00000340: 2061 7069 2074 6f6f 6c2e 2050 6169 7420   api tool. Pait 
-00000350: 656e 6162 6c65 7320 796f 7572 2050 7974  enables your Pyt
-00000360: 686f 6e20 7765 6220 6672 616d 6577 6f72  hon web framewor
-00000370: 6b20 746f 2068 6176 6520 7479 7065 2063  k to have type c
-00000380: 6865 636b 696e 672c 2070 6172 616d 6574  hecking, paramet
-00000390: 6572 2074 7970 6520 636f 6e76 6572 7369  er type conversi
-000003a0: 6f6e 2c20 696e 7465 7266 6163 6520 646f  on, interface do
-000003b0: 6375 6d65 6e74 2067 656e 6572 6174 696f  cument generatio
-000003c0: 6e20 616e 6420 6361 6e20 6469 7370 6c61  n and can displa
-000003d0: 7920 796f 7572 2064 6f63 756d 656e 7473  y your documents
-000003e0: 2074 6872 6f75 6768 2052 6564 6f63 206f   through Redoc o
-000003f0: 7220 5377 6167 6765 7220 2870 6f77 6572  r Swagger (power
-00000400: 2062 7920 696e 7370 6563 742c 2070 7964   by inspect, pyd
-00000410: 616e 7469 6329 272c 0a20 2020 2027 6c6f  antic)',.    'lo
-00000420: 6e67 5f64 6573 6372 6970 7469 6f6e 273a  ng_description':
-00000430: 2027 215b 5d28 6874 7470 733a 2f2f 6364   '![](https://cd
-00000440: 6e2e 6a73 6465 6c69 7672 2e6e 6574 2f67  n.jsdelivr.net/g
-00000450: 682f 736f 316e 2f73 6f31 6e5f 626c 6f67  h/so1n/so1n_blog
-00000460: 5f70 686f 746f 406d 6173 7465 722f 626c  _photo@master/bl
-00000470: 6f67 5f70 686f 746f 2f31 3635 3236 3030  og_photo/1652600
-00000480: 3632 3934 3931 2545 3625 3943 2541 4125  629491%E6%9C%AA%
-00000490: 4535 2539 3125 4244 2545 3525 3930 2538  E5%91%BD%E5%90%8
-000004a0: 442e 6a70 6729 5c6e 3c70 2061 6c69 676e  D.jpg)\n<p align
-000004b0: 3d22 6365 6e74 6572 223e 5c6e 2020 2020  ="center">\n    
-000004c0: 3c65 6d3e 5079 7468 6f6e 204d 6f64 6572  <em>Python Moder
-000004d0: 6e20 4150 4920 546f 6f6c 732c 2066 6173  n API Tools, fas
-000004e0: 7420 746f 2063 6f64 653c 2f65 6d3e 5c6e  t to code</em>\n
-000004f0: 3c2f 703e 5c6e 5c6e 2d2d 2d5c 6e2a 2a44  </p>\n\n---\n**D
-00000500: 6f63 756d 656e 7461 7469 6f6e 2a2a 3a20  ocumentation**: 
-00000510: 5b68 7474 7073 3a2f 2f73 6f31 6e2e 6d65  [https://so1n.me
-00000520: 2f70 6169 742f 5d28 6874 7470 733a 2f2f  /pait/](https://
-00000530: 736f 316e 2e6d 652f 7061 6974 2f29 5c6e  so1n.me/pait/)\n
-00000540: 5c6e 2a2a e4b8 ade6 9687 e696 87e6 a1a3  \n**............
-00000550: 2a2a 3a20 5b68 7474 7073 3a2f 2f73 6f31  **: [https://so1
-00000560: 6e2e 6d65 2f70 6169 742d 7a68 2d64 6f63  n.me/pait-zh-doc
-00000570: 2f5d 2868 7474 7073 3a2f 2f73 6f31 6e2e  /](https://so1n.
-00000580: 6d65 2f70 6169 742d 7a68 2d64 6f63 2f29  me/pait-zh-doc/)
-00000590: 5c6e 5c6e 2d2d 2d5c 6e5c 6e23 2070 6169  \n\n---\n\n# pai
-000005a0: 745c 6e50 6169 7420 6973 2061 6e20 6170  t\nPait is an ap
-000005b0: 6920 746f 6f6c 2074 6861 7420 6361 6e20  i tool that can 
-000005c0: 6265 2075 7365 6420 696e 2061 6e79 2070  be used in any p
-000005d0: 7974 686f 6e20 7765 6220 6672 616d 6577  ython web framew
-000005e0: 6f72 6b20 2863 7572 7265 6e74 6c79 206f  ork (currently o
-000005f0: 6e6c 7920 6066 6c61 736b 602c 2060 7374  nly `flask`, `st
-00000600: 6172 6c65 7474 6560 2c20 6073 616e 6963  arlette`, `sanic
-00000610: 602c 2060 746f 726e 6164 6f60 2061 7265  `, `tornado` are
-00000620: 2073 7570 706f 7274 6564 2c20 6f74 6865   supported, othe
-00000630: 7220 6672 616d 6577 6f72 6b73 2077 696c  r frameworks wil
-00000640: 6c20 6265 2073 7570 706f 7274 6564 206f  l be supported o
-00000650: 6e63 6520 5061 6974 2069 7320 7374 6162  nce Pait is stab
-00000660: 6c65 292e 5c6e 5c6e 3e20 4e6f 7465 3a5c  le).\n\n> Note:\
-00000670: 6e3e 5c6e 3e20 6d79 7079 2063 6865 636b  n>\n> mypy check
-00000680: 2031 3030 255c 6e3e 5c6e 3e20 7465 7374   100%\n>\n> test
-00000690: 2063 6f76 6572 6167 6520 3935 252b 2028   coverage 95%+ (
-000006a0: 6578 636c 7564 6520 6170 695f 646f 6329  exclude api_doc)
-000006b0: 5c6e 3e5c 6e3e 2070 7974 686f 6e20 7665  \n>\n> python ve
-000006c0: 7273 696f 6e20 3e3d 2033 2e37 2028 7375  rsion >= 3.7 (su
-000006d0: 7070 6f72 7420 706f 7374 706f 6e65 6420  pport postponed 
-000006e0: 616e 6e6f 7461 7469 6f6e 7329 5c6e 3e5c  annotations)\n>\
-000006f0: 6e3e 2054 6865 2066 6f6c 6c6f 7769 6e67  n> The following
-00000700: 2063 6f64 6520 646f 6573 206e 6f74 2073   code does not s
-00000710: 7065 6369 6679 2c20 616c 6c20 6465 6661  pecify, all defa
-00000720: 756c 7420 746f 2075 7365 2074 6865 2060  ult to use the `
-00000730: 7374 6172 6c65 7474 6560 2066 7261 6d65  starlette` frame
-00000740: 776f 726b 2e5c 6e5c 6e23 2046 6561 7475  work.\n\n# Featu
-00000750: 7265 5c6e 202d 205b 785d 2050 6172 616d  re\n - [x] Param
-00000760: 6574 6572 2063 6865 636b 7375 6d20 6175  eter checksum au
-00000770: 746f 6d61 7469 6320 636f 6e76 6572 7369  tomatic conversi
-00000780: 6f6e 2028 7061 7261 6d65 7465 7220 6368  on (parameter ch
-00000790: 6563 6b20 6465 7065 6e64 7320 6f6e 2060  eck depends on `
-000007a0: 5079 6461 6e74 6963 6029 5c6e 202d 205b  Pydantic`)\n - [
-000007b0: 785d 2050 6172 616d 6574 6572 2064 6570  x] Parameter dep
-000007c0: 656e 6465 6e63 7920 7665 7269 6669 6361  endency verifica
-000007d0: 7469 6f6e 5c6e 202d 205b 785d 2041 7574  tion\n - [x] Aut
-000007e0: 6f6d 6174 6963 616c 6c79 2067 656e 6572  omatically gener
-000007f0: 6174 6520 6f70 656e 6170 6920 6669 6c65  ate openapi file
-00000800: 735c 6e20 2d20 5b78 5d20 5377 6167 6765  s\n - [x] Swagge
-00000810: 722c 2052 6564 6f63 2072 6f75 7465 5c6e  r, Redoc route\n
-00000820: 202d 205b 785d 2067 5250 4320 4761 7465   - [x] gRPC Gate
-00000830: 7761 7920 726f 7574 655c 6e20 2d20 5b78  way route\n - [x
-00000840: 5d20 5465 7374 436c 6965 6e74 2073 7570  ] TestClient sup
-00000850: 706f 7274 2c20 7375 7070 6f72 7420 7265  port, support re
-00000860: 7370 6f6e 7365 2072 6573 756c 7420 7665  sponse result ve
-00000870: 7269 6669 6361 7469 6f6e 5c6e 202d 205b  rification\n - [
-00000880: 785d 2053 7570 706f 7274 2066 6f72 2070  x] Support for p
-00000890: 6c75 6769 6e20 6578 7465 6e73 696f 6e73  lugin extensions
-000008a0: 2c20 7375 6368 2061 7320 7468 6520 4d6f  , such as the Mo
-000008b0: 636b 2070 6c75 6769 6e5c 6e5c 6e23 2049  ck plugin\n\n# I
-000008c0: 6e73 7461 6c6c 6174 696f 6e5c 6e60 6060  nstallation\n```
-000008d0: 4261 7368 5c6e 7069 7020 696e 7374 616c  Bash\npip instal
-000008e0: 6c20 7061 6974 5c6e 6060 605c 6e23 2053  l pait\n```\n# S
-000008f0: 696d 706c 6520 4578 616d 706c 655c 6e60  imple Example\n`
-00000900: 6060 7079 7468 6f6e 5c6e 6672 6f6d 2074  ``python\nfrom t
-00000910: 7970 696e 6720 696d 706f 7274 2054 7970  yping import Typ
-00000920: 655c 6e69 6d70 6f72 7420 7576 6963 6f72  e\nimport uvicor
-00000930: 6e20 2023 2074 7970 653a 2069 676e 6f72  n  # type: ignor
-00000940: 655c 6e66 726f 6d20 7374 6172 6c65 7474  e\nfrom starlett
-00000950: 652e 6170 706c 6963 6174 696f 6e73 2069  e.applications i
-00000960: 6d70 6f72 7420 5374 6172 6c65 7474 655c  mport Starlette\
-00000970: 6e66 726f 6d20 7374 6172 6c65 7474 652e  nfrom starlette.
-00000980: 7265 7370 6f6e 7365 7320 696d 706f 7274  responses import
-00000990: 204a 534f 4e52 6573 706f 6e73 655c 6e66   JSONResponse\nf
-000009a0: 726f 6d20 7374 6172 6c65 7474 652e 726f  rom starlette.ro
-000009b0: 7574 696e 6720 696d 706f 7274 2052 6f75  uting import Rou
-000009c0: 7465 5c6e 5c6e 6672 6f6d 2070 6169 742e  te\n\nfrom pait.
-000009d0: 6170 702e 7374 6172 6c65 7474 6520 696d  app.starlette im
-000009e0: 706f 7274 2070 6169 742c 2061 6464 5f64  port pait, add_d
-000009f0: 6f63 5f72 6f75 7465 5c6e 6672 6f6d 2070  oc_route\nfrom p
-00000a00: 6169 742e 6669 656c 6420 696d 706f 7274  ait.field import
-00000a10: 2042 6f64 795c 6e66 726f 6d20 7061 6974   Body\nfrom pait
-00000a20: 2e6d 6f64 656c 2e72 6573 706f 6e73 6520  .model.response 
-00000a30: 696d 706f 7274 2050 6169 7452 6573 706f  import PaitRespo
-00000a40: 6e73 654d 6f64 656c 5c6e 6672 6f6d 2070  nseModel\nfrom p
-00000a50: 7964 616e 7469 6320 696d 706f 7274 2042  ydantic import B
-00000a60: 6173 654d 6f64 656c 2c20 4669 656c 645c  aseModel, Field\
-00000a70: 6e5c 6e5c 6e63 6c61 7373 2044 656d 6f52  n\n\nclass DemoR
-00000a80: 6573 706f 6e73 654d 6f64 656c 2850 6169  esponseModel(Pai
-00000a90: 7452 6573 706f 6e73 654d 6f64 656c 293a  tResponseModel):
-00000aa0: 5c6e 2020 2020 636c 6173 7320 5265 7370  \n    class Resp
-00000ab0: 6f6e 7365 4d6f 6465 6c28 4261 7365 4d6f  onseModel(BaseMo
-00000ac0: 6465 6c29 3a5c 6e20 2020 2020 2020 2075  del):\n        u
-00000ad0: 6964 3a20 696e 7420 3d20 4669 656c 6428  id: int = Field(
-00000ae0: 295c 6e20 2020 2020 2020 2075 7365 725f  )\n        user_
-00000af0: 6e61 6d65 3a20 7374 7220 3d20 4669 656c  name: str = Fiel
-00000b00: 6428 295c 6e5c 6e20 2020 2064 6573 6372  d()\n\n    descr
-00000b10: 6970 7469 6f6e 3a20 7374 7220 3d20 2264  iption: str = "d
-00000b20: 656d 6f20 7265 7370 6f6e 7365 225c 6e20  emo response"\n 
-00000b30: 2020 2072 6573 706f 6e73 655f 6461 7461     response_data
-00000b40: 3a20 5479 7065 5b42 6173 654d 6f64 656c  : Type[BaseModel
-00000b50: 5d20 3d20 5265 7370 6f6e 7365 4d6f 6465  ] = ResponseMode
-00000b60: 6c5c 6e5c 6e5c 6e40 7061 6974 2872 6573  l\n\n\n@pait(res
-00000b70: 706f 6e73 655f 6d6f 6465 6c5f 6c69 7374  ponse_model_list
-00000b80: 3d5b 4465 6d6f 5265 7370 6f6e 7365 4d6f  =[DemoResponseMo
-00000b90: 6465 6c5d 295c 6e61 7379 6e63 2064 6566  del])\nasync def
-00000ba0: 2064 656d 6f5f 706f 7374 285c 6e20 2020   demo_post(\n   
-00000bb0: 2075 6964 3a20 696e 7420 3d20 426f 6479   uid: int = Body
-00000bc0: 2e69 2864 6573 6372 6970 7469 6f6e 3d22  .i(description="
-00000bd0: 7573 6572 2069 6422 2c20 6774 3d31 302c  user id", gt=10,
-00000be0: 206c 743d 3130 3030 292c 5c6e 2020 2020   lt=1000),\n    
-00000bf0: 7573 6572 5f6e 616d 653a 2073 7472 203d  user_name: str =
-00000c00: 2042 6f64 792e 6928 6465 7363 7269 7074   Body.i(descript
-00000c10: 696f 6e3d 2275 7365 7220 6e61 6d65 222c  ion="user name",
-00000c20: 206d 696e 5f6c 656e 6774 683d 322c 206d   min_length=2, m
-00000c30: 6178 5f6c 656e 6774 683d 3429 5c6e 2920  ax_length=4)\n) 
-00000c40: 2d3e 204a 534f 4e52 6573 706f 6e73 653a  -> JSONResponse:
-00000c50: 5c6e 2020 2020 7265 7475 726e 204a 534f  \n    return JSO
-00000c60: 4e52 6573 706f 6e73 6528 7b5c 2775 6964  NResponse({\'uid
-00000c70: 5c27 3a20 7569 642c 205c 2775 7365 725f  \': uid, \'user_
-00000c80: 6e61 6d65 5c27 3a20 7573 6572 5f6e 616d  name\': user_nam
-00000c90: 657d 295c 6e5c 6e5c 6e61 7070 203d 2053  e})\n\n\napp = S
-00000ca0: 7461 726c 6574 7465 2872 6f75 7465 733d  tarlette(routes=
-00000cb0: 5b52 6f75 7465 285c 272f 6170 695c 272c  [Route(\'/api\',
-00000cc0: 2064 656d 6f5f 706f 7374 2c20 6d65 7468   demo_post, meth
-00000cd0: 6f64 733d 5b5c 2750 4f53 545c 275d 295d  ods=[\'POST\'])]
-00000ce0: 295c 6e61 6464 5f64 6f63 5f72 6f75 7465  )\nadd_doc_route
-00000cf0: 2861 7070 295c 6e75 7669 636f 726e 2e72  (app)\nuvicorn.r
-00000d00: 756e 2861 7070 295c 6e60 6060 5c6e 5c6e  un(app)\n```\n\n
-00000d10: 2320 486f 7720 746f 2075 7365 6420 696e  # How to used in
-00000d20: 206f 7468 6572 2077 6562 2066 7261 6d65   other web frame
-00000d30: 776f 726b 3f5c 6e49 6620 7468 6520 7765  work?\nIf the we
-00000d40: 6220 6672 616d 6577 6f72 6b20 6973 206e  b framework is n
-00000d50: 6f74 2073 7570 706f 7274 6564 2c20 7768  ot supported, wh
-00000d60: 6963 6820 796f 7520 6172 6520 7573 696e  ich you are usin
-00000d70: 672e 5c6e 5c6e 4361 6e20 6265 206d 6f64  g.\n\nCan be mod
-00000d80: 6966 6965 6420 7379 6e63 2077 6562 2066  ified sync web f
-00000d90: 7261 6d65 776f 726b 2061 6363 6f72 6469  ramework accordi
-00000da0: 6e67 2074 6f20 5b70 6169 742e 6170 702e  ng to [pait.app.
-00000db0: 666c 6173 6b5d 2868 7474 7073 3a2f 2f67  flask](https://g
-00000dc0: 6974 6875 622e 636f 6d2f 736f 316e 2f70  ithub.com/so1n/p
-00000dd0: 6169 742f 626c 6f62 2f6d 6173 7465 722f  ait/blob/master/
-00000de0: 7061 6974 2f61 7070 2f66 6c61 736b 2e70  pait/app/flask.p
-00000df0: 7929 5c6e 5c6e 4361 6e20 6265 206d 6f64  y)\n\nCan be mod
-00000e00: 6966 6965 6420 6173 796e 6320 7765 6220  ified async web 
-00000e10: 6672 616d 6577 6f72 6b20 6163 636f 7264  framework accord
-00000e20: 696e 6720 746f 205b 7061 6974 2e61 7070  ing to [pait.app
-00000e30: 2e73 7461 726c 6574 7465 5d28 6874 7470  .starlette](http
-00000e40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000e50: 6f31 6e2f 7061 6974 2f62 6c6f 622f 6d61  o1n/pait/blob/ma
-00000e60: 7374 6572 2f70 6169 742f 6170 702f 7374  ster/pait/app/st
-00000e70: 6172 6c65 7474 652e 7079 295c 6e23 2049  arlette.py)\n# I
-00000e80: 4445 2053 7570 706f 7274 5c6e 5768 696c  DE Support\nWhil
-00000e90: 6520 7079 6461 6e74 6963 2077 696c 6c20  e pydantic will 
-00000ea0: 776f 726b 2077 656c 6c20 7769 7468 2061  work well with a
-00000eb0: 6e79 2049 4445 206f 7574 206f 6620 7468  ny IDE out of th
-00000ec0: 6520 626f 782e 5c6e 2d20 5b50 7943 6861  e box.\n- [PyCha
-00000ed0: 726d 2070 6c75 6769 6e5d 2868 7474 7073  rm plugin](https
-00000ee0: 3a2f 2f70 7964 616e 7469 632d 646f 6373  ://pydantic-docs
-00000ef0: 2e68 656c 706d 616e 7561 6c2e 696f 2f70  .helpmanual.io/p
-00000f00: 7963 6861 726d 5f70 6c75 6769 6e2f 295c  ycharm_plugin/)\
-00000f10: 6e2d 205b 4d79 7079 2070 6c75 6769 6e5d  n- [Mypy plugin]
-00000f20: 2868 7474 7073 3a2f 2f70 7964 616e 7469  (https://pydanti
-00000f30: 632d 646f 6373 2e68 656c 706d 616e 7561  c-docs.helpmanua
-00000f40: 6c2e 696f 2f6d 7970 795f 706c 7567 696e  l.io/mypy_plugin
-00000f50: 2f29 5c6e 5c6e 2320 4675 6c6c 2065 7861  /)\n\n# Full exa
-00000f60: 6d70 6c65 5c6e 466f 7220 6d6f 7265 2063  mple\nFor more c
-00000f70: 6f6d 706c 6574 6520 6578 616d 706c 6573  omplete examples
-00000f80: 2c20 706c 6561 7365 2072 6566 6572 2074  , please refer t
-00000f90: 6f20 5b65 7861 6d70 6c65 5d28 6874 7470  o [example](http
-00000fa0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000fb0: 6f31 6e2f 7061 6974 2f74 7265 652f 6d61  o1n/pait/tree/ma
-00000fc0: 7374 6572 2f65 7861 6d70 6c65 295c 6e27  ster/example)\n'
-00000fd0: 2c0a 2020 2020 2761 7574 686f 7227 3a20  ,.    'author': 
-00000fe0: 2753 6f31 6e27 2c0a 2020 2020 2761 7574  'So1n',.    'aut
-00000ff0: 686f 725f 656d 6169 6c27 3a20 2773 6f31  hor_email': 'so1
-00001000: 6e38 3937 3034 3630 3236 4067 6d61 696c  n897046026@gmail
-00001010: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
-00001020: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-00001030: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-00001040: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-00001050: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-00001060: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001070: 736f 316e 2f70 6169 7427 2c0a 2020 2020  so1n/pait',.    
-00001080: 2770 6163 6b61 6765 7327 3a20 7061 636b  'packages': pack
-00001090: 6167 6573 2c0a 2020 2020 2770 6163 6b61  ages,.    'packa
-000010a0: 6765 5f64 6174 6127 3a20 7061 636b 6167  ge_data': packag
-000010b0: 655f 6461 7461 2c0a 2020 2020 2769 6e73  e_data,.    'ins
-000010c0: 7461 6c6c 5f72 6571 7569 7265 7327 3a20  tall_requires': 
-000010d0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-000010e0: 2c0a 2020 2020 2765 7874 7261 735f 7265  ,.    'extras_re
-000010f0: 7175 6972 6527 3a20 6578 7472 6173 5f72  quire': extras_r
-00001100: 6571 7569 7265 2c0a 2020 2020 2770 7974  equire,.    'pyt
-00001110: 686f 6e5f 7265 7175 6972 6573 273a 2027  hon_requires': '
-00001120: 3e3d 332e 372c 3c34 2e30 272c 0a7d 0a0a  >=3.7,<4.0',.}..
-00001130: 0a73 6574 7570 282a 2a73 6574 7570 5f6b  .setup(**setup_k
-00001140: 7761 7267 7329 0a                        wargs).
+00000050: 6974 2e61 7070 272c 0a20 2770 6169 742e  it.app',. 'pait.
+00000060: 6170 702e 616e 7927 2c0a 2027 7061 6974  app.any',. 'pait
+00000070: 2e61 7070 2e61 6e79 2e70 6c75 6769 6e27  .app.any.plugin'
+00000080: 2c0a 2027 7061 6974 2e61 7070 2e61 6e79  ,. 'pait.app.any
+00000090: 2e73 6563 7572 6974 7927 2c0a 2027 7061  .security',. 'pa
+000000a0: 6974 2e61 7070 2e62 6173 6527 2c0a 2027  it.app.base',. '
+000000b0: 7061 6974 2e61 7070 2e62 6173 652e 6164  pait.app.base.ad
+000000c0: 6170 7465 7227 2c0a 2027 7061 6974 2e61  apter',. 'pait.a
+000000d0: 7070 2e62 6173 652e 7365 6375 7269 7479  pp.base.security
+000000e0: 272c 0a20 2770 6169 742e 6170 702e 666c  ',. 'pait.app.fl
+000000f0: 6173 6b27 2c0a 2027 7061 6974 2e61 7070  ask',. 'pait.app
+00000100: 2e66 6c61 736b 2e61 6461 7074 6572 272c  .flask.adapter',
+00000110: 0a20 2770 6169 742e 6170 702e 666c 6173  . 'pait.app.flas
+00000120: 6b2e 706c 7567 696e 272c 0a20 2770 6169  k.plugin',. 'pai
+00000130: 742e 6170 702e 666c 6173 6b2e 7365 6375  t.app.flask.secu
+00000140: 7269 7479 272c 0a20 2770 6169 742e 6170  rity',. 'pait.ap
+00000150: 702e 7361 6e69 6327 2c0a 2027 7061 6974  p.sanic',. 'pait
+00000160: 2e61 7070 2e73 616e 6963 2e61 6461 7074  .app.sanic.adapt
+00000170: 6572 272c 0a20 2770 6169 742e 6170 702e  er',. 'pait.app.
+00000180: 7361 6e69 632e 706c 7567 696e 272c 0a20  sanic.plugin',. 
+00000190: 2770 6169 742e 6170 702e 7361 6e69 632e  'pait.app.sanic.
+000001a0: 7365 6375 7269 7479 272c 0a20 2770 6169  security',. 'pai
+000001b0: 742e 6170 702e 7374 6172 6c65 7474 6527  t.app.starlette'
+000001c0: 2c0a 2027 7061 6974 2e61 7070 2e73 7461  ,. 'pait.app.sta
+000001d0: 726c 6574 7465 2e61 6461 7074 6572 272c  rlette.adapter',
+000001e0: 0a20 2770 6169 742e 6170 702e 7374 6172  . 'pait.app.star
+000001f0: 6c65 7474 652e 706c 7567 696e 272c 0a20  lette.plugin',. 
+00000200: 2770 6169 742e 6170 702e 7374 6172 6c65  'pait.app.starle
+00000210: 7474 652e 7365 6375 7269 7479 272c 0a20  tte.security',. 
+00000220: 2770 6169 742e 6170 702e 746f 726e 6164  'pait.app.tornad
+00000230: 6f27 2c0a 2027 7061 6974 2e61 7070 2e74  o',. 'pait.app.t
+00000240: 6f72 6e61 646f 2e61 6461 7074 6572 272c  ornado.adapter',
+00000250: 0a20 2770 6169 742e 6170 702e 746f 726e  . 'pait.app.torn
+00000260: 6164 6f2e 706c 7567 696e 272c 0a20 2770  ado.plugin',. 'p
+00000270: 6169 742e 6170 702e 746f 726e 6164 6f2e  ait.app.tornado.
+00000280: 7365 6375 7269 7479 272c 0a20 2770 6169  security',. 'pai
+00000290: 742e 6578 7472 6127 2c0a 2027 7061 6974  t.extra',. 'pait
+000002a0: 2e67 7270 6327 2c0a 2027 7061 6974 2e67  .grpc',. 'pait.g
+000002b0: 7270 632e 706c 7567 696e 272c 0a20 2770  rpc.plugin',. 'p
+000002c0: 6169 742e 6772 7063 2e70 726f 746f 272c  ait.grpc.proto',
+000002d0: 0a20 2770 6169 742e 6d6f 6465 6c27 2c0a  . 'pait.model',.
+000002e0: 2027 7061 6974 2e6f 7065 6e61 7069 272c   'pait.openapi',
+000002f0: 0a20 2770 6169 742e 7061 7261 6d5f 6861  . 'pait.param_ha
+00000300: 6e64 6c65 272c 0a20 2770 6169 742e 706c  ndle',. 'pait.pl
+00000310: 7567 696e 272c 0a20 2770 6169 742e 7574  ugin',. 'pait.ut
+00000320: 696c 275d 0a0a 7061 636b 6167 655f 6461  il']..package_da
+00000330: 7461 203d 205c 0a7b 2727 3a20 5b27 2a27  ta = \.{'': ['*'
+00000340: 5d7d 0a0a 696e 7374 616c 6c5f 7265 7175  ]}..install_requ
+00000350: 6972 6573 203d 205c 0a5b 2761 6e79 2d61  ires = \.['any-a
+00000360: 7069 3e3d 302e 312e 302e 332c 3c30 2e32  pi>=0.1.0.3,<0.2
+00000370: 2e30 2e30 272c 0a20 2770 7964 616e 7469  .0.0',. 'pydanti
+00000380: 633e 3d31 2e37 2e33 2c3c 322e 302e 3027  c>=1.7.3,<2.0.0'
+00000390: 2c0a 2027 7479 7069 6e67 2d65 7874 656e  ,. 'typing-exten
+000003a0: 7369 6f6e 733e 3d34 2e31 2e31 2c3c 352e  sions>=4.1.1,<5.
+000003b0: 302e 3027 5d0a 0a65 7874 7261 735f 7265  0.0']..extras_re
+000003c0: 7175 6972 6520 3d20 5c0a 7b27 3a65 7874  quire = \.{':ext
+000003d0: 7261 203d 3d20 2267 7270 6322 206f 7220  ra == "grpc" or 
+000003e0: 6578 7472 6120 3d3d 2022 616c 6c22 273a  extra == "all"':
+000003f0: 205b 2770 726f 746f 6275 662d 746f 2d70   ['protobuf-to-p
+00000400: 7964 616e 7469 633e 3d30 2e31 2e37 2e33  ydantic>=0.1.7.3
+00000410: 2c3c 302e 322e 302e 3027 5d2c 0a20 2761  ,<0.2.0.0'],. 'a
+00000420: 6c6c 273a 205b 2772 6564 6973 3e3d 342e  ll': ['redis>=4.
+00000430: 322e 322c 3c35 2e30 2e30 272c 2027 6a69  2.2,<5.0.0', 'ji
+00000440: 6e6a 6132 3e3d 322e 302e 3027 5d2c 0a20  nja2>=2.0.0'],. 
+00000450: 2767 7270 6327 3a20 5b27 6a69 6e6a 6132  'grpc': ['jinja2
+00000460: 3e3d 322e 302e 3027 5d2c 0a20 2772 6564  >=2.0.0'],. 'red
+00000470: 6973 273a 205b 2772 6564 6973 3e3d 342e  is': ['redis>=4.
+00000480: 322e 322c 3c35 2e30 2e30 275d 7d0a 0a65  2.2,<5.0.0']}..e
+00000490: 6e74 7279 5f70 6f69 6e74 7320 3d20 5c0a  ntry_points = \.
+000004a0: 7b27 636f 6e73 6f6c 655f 7363 7269 7074  {'console_script
+000004b0: 7327 3a20 5b27 7072 6f74 6f63 2d67 656e  s': ['protoc-gen
+000004c0: 2d70 6169 742d 726f 7574 6520 3d20 7061  -pait-route = pa
+000004d0: 6974 2e67 7270 632e 706c 7567 696e 2e6d  it.grpc.plugin.m
+000004e0: 6169 6e3a 6d61 696e 275d 7d0a 0a73 6574  ain:main']}..set
+000004f0: 7570 5f6b 7761 7267 7320 3d20 7b0a 2020  up_kwargs = {.  
+00000500: 2020 276e 616d 6527 3a20 2770 6169 7427    'name': 'pait'
+00000510: 2c0a 2020 2020 2776 6572 7369 6f6e 273a  ,.    'version':
+00000520: 2027 312e 302e 3061 3127 2c0a 2020 2020   '1.0.0a1',.    
+00000530: 2764 6573 6372 6970 7469 6f6e 273a 2027  'description': '
+00000540: 5061 6974 2069 7320 6120 5079 7468 6f6e  Pait is a Python
+00000550: 2061 7069 2074 6f6f 6c2e 2050 6169 7420   api tool. Pait 
+00000560: 656e 6162 6c65 7320 796f 7572 2050 7974  enables your Pyt
+00000570: 686f 6e20 7765 6220 6672 616d 6577 6f72  hon web framewor
+00000580: 6b20 746f 2068 6176 6520 7479 7065 2063  k to have type c
+00000590: 6865 636b 696e 672c 2070 6172 616d 6574  hecking, paramet
+000005a0: 6572 2074 7970 6520 636f 6e76 6572 7369  er type conversi
+000005b0: 6f6e 2c20 696e 7465 7266 6163 6520 646f  on, interface do
+000005c0: 6375 6d65 6e74 2067 656e 6572 6174 696f  cument generatio
+000005d0: 6e20 616e 6420 6361 6e20 6469 7370 6c61  n and can displa
+000005e0: 7920 796f 7572 2064 6f63 756d 656e 7473  y your documents
+000005f0: 2074 6872 6f75 6768 2052 6564 6f63 206f   through Redoc o
+00000600: 7220 5377 6167 6765 7220 2870 6f77 6572  r Swagger (power
+00000610: 2062 7920 696e 7370 6563 742c 2070 7964   by inspect, pyd
+00000620: 616e 7469 6329 272c 0a20 2020 2027 6c6f  antic)',.    'lo
+00000630: 6e67 5f64 6573 6372 6970 7469 6f6e 273a  ng_description':
+00000640: 2027 215b 5d28 6874 7470 733a 2f2f 6364   '![](https://cd
+00000650: 6e2e 6a73 6465 6c69 7672 2e6e 6574 2f67  n.jsdelivr.net/g
+00000660: 682f 736f 316e 2f73 6f31 6e5f 626c 6f67  h/so1n/so1n_blog
+00000670: 5f70 686f 746f 406d 6173 7465 722f 626c  _photo@master/bl
+00000680: 6f67 5f70 686f 746f 2f31 3635 3236 3030  og_photo/1652600
+00000690: 3632 3934 3931 2545 3625 3943 2541 4125  629491%E6%9C%AA%
+000006a0: 4535 2539 3125 4244 2545 3525 3930 2538  E5%91%BD%E5%90%8
+000006b0: 442e 6a70 6729 5c6e 3c70 2061 6c69 676e  D.jpg)\n<p align
+000006c0: 3d22 6365 6e74 6572 223e 5c6e 2020 2020  ="center">\n    
+000006d0: 3c65 6d3e 5079 7468 6f6e 204d 6f64 6572  <em>Python Moder
+000006e0: 6e20 4150 4920 546f 6f6c 732c 2066 6173  n API Tools, fas
+000006f0: 7420 746f 2063 6f64 653c 2f65 6d3e 5c6e  t to code</em>\n
+00000700: 3c2f 703e 5c6e 3c70 2061 6c69 676e 3d22  </p>\n<p align="
+00000710: 6365 6e74 6572 223e 5c6e 2020 2020 3c61  center">\n    <a
+00000720: 2068 7265 663d 2268 7474 7073 3a2f 2f63   href="https://c
+00000730: 6f64 6563 6f76 2e69 6f2f 6768 2f73 6f31  odecov.io/gh/so1
+00000740: 6e2f 7061 6974 2220 7461 7267 6574 3d22  n/pait" target="
+00000750: 5f62 6c61 6e6b 223e 5c6e 2020 2020 2020  _blank">\n      
+00000760: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000770: 733a 2f2f 636f 6465 636f 762e 696f 2f67  s://codecov.io/g
+00000780: 682f 736f 316e 2f70 6169 742f 6272 616e  h/so1n/pait/bran
+00000790: 6368 2f6d 6173 7465 722f 6772 6170 682f  ch/master/graph/
+000007a0: 6261 6467 652e 7376 673f 746f 6b65 6e3d  badge.svg?token=
+000007b0: 4e45 564d 3156 4f44 4852 2220 616c 743d  NEVM1VODHR" alt=
+000007c0: 2243 6f76 6572 6167 6522 3e5c 6e20 2020  "Coverage">\n   
+000007d0: 203c 2f61 3e5c 6e3c 2f70 3e5c 6e3c 7020   </a>\n</p>\n<p 
+000007e0: 616c 6967 6e3d 2263 656e 7465 7222 3e5c  align="center">\
+000007f0: 6e20 2020 203c 6120 6872 6566 3d22 6874  n    <a href="ht
+00000800: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000810: 726f 6a65 6374 2f70 6169 742f 2220 7461  roject/pait/" ta
+00000820: 7267 6574 3d22 5f62 6c61 6e6b 223e 5c6e  rget="_blank">\n
+00000830: 2020 2020 2020 2020 3c69 6d67 2061 6c74          <img alt
+00000840: 3d22 5079 5049 202d 2050 7974 686f 6e20  ="PyPI - Python 
+00000850: 5665 7273 696f 6e22 2073 7263 3d22 6874  Version" src="ht
+00000860: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000870: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
+00000880: 696f 6e73 2f70 6169 7422 3e5c 6e20 2020  ions/pait">\n   
+00000890: 203c 2f61 3e5c 6e20 2020 203c 6120 6872   </a>\n    <a hr
+000008a0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000008b0: 2e6f 7267 2f70 726f 6a65 6374 2f70 6169  .org/project/pai
+000008c0: 742f 2220 7461 7267 6574 3d22 5f62 6c61  t/" target="_bla
+000008d0: 6e6b 223e 5c6e 2020 2020 2020 2020 3c69  nk">\n        <i
+000008e0: 6d67 2061 6c74 3d22 5079 5049 2220 7372  mg alt="PyPI" sr
+000008f0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000900: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000910: 2f70 6169 7422 3e5c 6e20 2020 203c 2f61  /pait">\n    </a
+00000920: 3e5c 6e3c 2f70 3e5c 6e3c 7020 616c 6967  >\n</p>\n<p alig
+00000930: 6e3d 2263 656e 7465 7222 3e5c 6e20 2020  n="center">\n   
+00000940: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+00000950: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6f31  //github.com/so1
+00000960: 6e2f 7061 6974 2f61 6374 696f 6e73 3f71  n/pait/actions?q
+00000970: 7565 7279 3d65 7665 6e74 2533 4170 7573  uery=event%3Apus
+00000980: 682b 6272 616e 6368 2533 416d 6173 7465  h+branch%3Amaste
+00000990: 7222 2074 6172 6765 743d 225f 626c 616e  r" target="_blan
+000009a0: 6b22 3e5c 6e20 2020 2020 2020 203c 696d  k">\n        <im
+000009b0: 6720 616c 743d 2247 6974 4875 6220 576f  g alt="GitHub Wo
+000009c0: 726b 666c 6f77 2053 7461 7475 7322 2073  rkflow Status" s
+000009d0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000009e0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+000009f0: 622f 6163 7469 6f6e 732f 776f 726b 666c  b/actions/workfl
+00000a00: 6f77 2f73 7461 7475 732f 736f 316e 2f70  ow/status/so1n/p
+00000a10: 6169 742f 7079 7468 6f6e 2d70 6163 6b61  ait/python-packa
+00000a20: 6765 2e79 6d6c 223e 5c6e 2020 2020 3c2f  ge.yml">\n    </
+00000a30: 613e 5c6e 2020 2020 3c61 2068 7265 663d  a>\n    <a href=
+00000a40: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000a50: 636f 6d2f 736f 316e 2f70 6169 742f 7265  com/so1n/pait/re
+00000a60: 6c65 6173 6573 2220 7461 7267 6574 3d22  leases" target="
+00000a70: 5f62 6c61 6e6b 223e 5c6e 2020 2020 2020  _blank">\n      
+00000a80: 2020 3c69 6d67 2061 6c74 3d22 4769 7448    <img alt="GitH
+00000a90: 7562 2072 656c 6561 7365 2028 7265 6c65  ub release (rele
+00000aa0: 6173 6520 6e61 6d65 2069 6e73 7465 6164  ase name instead
+00000ab0: 206f 6620 7461 6720 6e61 6d65 2922 2073   of tag name)" s
+00000ac0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000ad0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00000ae0: 622f 762f 7265 6c65 6173 652f 736f 316e  b/v/release/so1n
+00000af0: 2f70 6169 743f 696e 636c 7564 655f 7072  /pait?include_pr
+00000b00: 6572 656c 6561 7365 7322 3e5c 6e20 2020  ereleases">\n   
+00000b10: 203c 2f61 3e5c 6e20 2020 203c 6120 6872   </a>\n    <a hr
+00000b20: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000b30: 7562 2e63 6f6d 2f73 6f31 6e2f 7061 6974  ub.com/so1n/pait
+00000b40: 2f61 6374 696f 6e73 3f71 7565 7279 3d65  /actions?query=e
+00000b50: 7665 6e74 2533 4170 7573 682b 6272 616e  vent%3Apush+bran
+00000b60: 6368 2533 416d 6173 7465 7222 2074 6172  ch%3Amaster" tar
+00000b70: 6765 743d 225f 626c 616e 6b22 3e5c 6e20  get="_blank">\n 
+00000b80: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+00000b90: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000ba0: 636f 6d2f 736f 316e 2f70 6169 742f 6163  com/so1n/pait/ac
+00000bb0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000bc0: 7079 7468 6f6e 2d70 6163 6b61 6765 2e79  python-package.y
+00000bd0: 6d6c 2f62 6164 6765 2e73 7667 3f65 7665  ml/badge.svg?eve
+00000be0: 6e74 3d70 7573 6826 6272 616e 6368 3d6d  nt=push&branch=m
+00000bf0: 6173 7465 7222 2061 6c74 3d22 5465 7374  aster" alt="Test
+00000c00: 223e 5c6e 2020 2020 3c2f 613e 5c6e 3c2f  ">\n    </a>\n</
+00000c10: 703e 5c6e 3c70 2061 6c69 676e 3d22 6365  p>\n<p align="ce
+00000c20: 6e74 6572 223e 5c6e 2020 2020 3c61 2068  nter">\n    <a h
+00000c30: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000c40: 6875 622e 636f 6d2f 736f 316e 2f70 6169  hub.com/so1n/pai
+00000c50: 742f 7472 6565 2f6d 6173 7465 722f 6578  t/tree/master/ex
+00000c60: 616d 706c 6522 2074 6172 6765 743d 225f  ample" target="_
+00000c70: 626c 616e 6b22 3e5c 6e20 2020 2020 2020  blank">\n       
+00000c80: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
+00000c90: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000ca0: 6f2f 6261 6467 652f 5375 7070 6f72 7425  o/badge/Support%
+00000cb0: 3230 6672 616d 6577 6f72 6b2d 466c 6173  20framework-Flas
+00000cc0: 6b25 3243 5361 6e69 6325 3243 5374 6172  k%2CSanic%2CStar
+00000cd0: 6c65 7474 6525 3243 546f 726e 6164 6f2d  lette%2CTornado-
+00000ce0: 6272 6967 6874 6772 6565 6e22 2061 6c74  brightgreen" alt
+00000cf0: 3d22 5375 7070 6f72 7420 6672 616d 6577  ="Support framew
+00000d00: 6f72 6b22 3e5c 6e20 2020 203c 2f61 3e5c  ork">\n    </a>\
+00000d10: 6e3c 2f70 3e5c 6e5c 6e5c 6e2d 2d2d 5c6e  n</p>\n\n\n---\n
+00000d20: 2a2a 446f 6375 6d65 6e74 6174 696f 6e2a  **Documentation*
+00000d30: 2a3a 205b 6874 7470 733a 2f2f 736f 316e  *: [https://so1n
+00000d40: 2e6d 652f 7061 6974 2f5d 2868 7474 7073  .me/pait/](https
+00000d50: 3a2f 2f73 6f31 6e2e 6d65 2f70 6169 742f  ://so1n.me/pait/
+00000d60: 295c 6e5c 6e2a 2ae4 b8ad e696 87e6 9687  )\n\n**.........
+00000d70: e6a1 a32a 2a3a 205b 6874 7470 733a 2f2f  ...**: [https://
+00000d80: 736f 316e 2e6d 652f 7061 6974 2d7a 682d  so1n.me/pait-zh-
+00000d90: 646f 632f 5d28 6874 7470 733a 2f2f 736f  doc/](https://so
+00000da0: 316e 2e6d 652f 7061 6974 2d7a 682d 646f  1n.me/pait-zh-do
+00000db0: 632f 295c 6e5c 6e2d 2d2d 5c6e 5c6e 2320  c/)\n\n---\n\n# 
+00000dc0: 7061 6974 5c6e 5c6e 5061 6974 2069 7320  pait\n\nPait is 
+00000dd0: 616e 2061 7069 2074 6f6f 6c20 7468 6174  an api tool that
+00000de0: 2063 616e 2062 6520 7573 6564 2069 6e20   can be used in 
+00000df0: 616e 7920 7079 7468 6f6e 2077 6562 2066  any python web f
+00000e00: 7261 6d65 776f 726b 2028 6375 7272 656e  ramework (curren
+00000e10: 746c 7920 6f6e 6c79 2060 666c 6173 6b60  tly only `flask`
+00000e20: 2c20 6073 7461 726c 6574 7465 602c 2060  , `starlette`, `
+00000e30: 7361 6e69 6360 2c20 6074 6f72 6e61 646f  sanic`, `tornado
+00000e40: 6020 6172 6520 7375 7070 6f72 7465 642c  ` are supported,
+00000e50: 206f 7468 6572 2066 7261 6d65 776f 726b   other framework
+00000e60: 7320 7769 6c6c 2062 6520 7375 7070 6f72  s will be suppor
+00000e70: 7465 6420 6f6e 6365 2050 6169 7420 6973  ted once Pait is
+00000e80: 2073 7461 626c 6529 2e5c 6e5c 6e3e 204e   stable).\n\n> N
+00000e90: 6f74 653a 5c6e 3e5c 6e3e 206d 7970 7920  ote:\n>\n> mypy 
+00000ea0: 6368 6563 6b20 3130 3025 5c6e 3e5c 6e3e  check 100%\n>\n>
+00000eb0: 2074 6573 7420 636f 7665 7261 6765 2039   test coverage 9
+00000ec0: 3525 2b20 2865 7863 6c75 6465 2061 7069  5%+ (exclude api
+00000ed0: 5f64 6f63 295c 6e3e 5c6e 3e20 7079 7468  _doc)\n>\n> pyth
+00000ee0: 6f6e 2076 6572 7369 6f6e 203e 3d20 332e  on version >= 3.
+00000ef0: 3720 2873 7570 706f 7274 2070 6f73 7470  7 (support postp
+00000f00: 6f6e 6564 2061 6e6e 6f74 6174 696f 6e73  oned annotations
+00000f10: 295c 6e3e 5c6e 3e20 5468 6520 666f 6c6c  )\n>\n> The foll
+00000f20: 6f77 696e 6720 636f 6465 2064 6f65 7320  owing code does 
+00000f30: 6e6f 7420 7370 6563 6966 792c 2061 6c6c  not specify, all
+00000f40: 2064 6566 6175 6c74 2074 6f20 7573 6520   default to use 
+00000f50: 7468 6520 6073 7461 726c 6574 7465 6020  the `starlette` 
+00000f60: 6672 616d 6577 6f72 6b2e 5c6e 5c6e 2320  framework.\n\n# 
+00000f70: 5761 726e 696e 675c 6e54 6865 7265 2061  Warning\nThere a
+00000f80: 7265 2063 6861 6e67 6573 2062 6574 7765  re changes betwe
+00000f90: 656e 2074 6865 2063 7572 7265 6e74 2076  en the current v
+00000fa0: 6572 7369 6f6e 2061 6e64 2074 6865 2030  ersion and the 0
+00000fb0: 2e38 2076 6572 7369 6f6e 206f 6620 7468  .8 version of th
+00000fc0: 6520 4150 492c 2046 6f72 206d 6f72 6520  e API, For more 
+00000fd0: 696e 666f 726d 6174 696f 6e2c 2070 6c65  information, ple
+00000fe0: 6173 6520 7265 6665 7220 746f 205b 302e  ase refer to [0.
+00000ff0: 392e 3076 6572 7369 6f6e 2063 6861 6e67  9.0version chang
+00001000: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00001010: 622e 636f 6d2f 736f 316e 2f70 6169 742f  b.com/so1n/pait/
+00001020: 626c 6f62 2f6d 6173 7465 722f 4348 414e  blob/master/CHAN
+00001030: 4745 4c4f 472e 6d64 295c 6e5c 6e23 2046  GELOG.md)\n\n# F
+00001040: 6561 7475 7265 5c6e 202d 205b 785d 2050  eature\n - [x] P
+00001050: 6172 616d 6574 6572 2063 6865 636b 7375  arameter checksu
+00001060: 6d20 6175 746f 6d61 7469 6320 636f 6e76  m automatic conv
+00001070: 6572 7369 6f6e 2028 7061 7261 6d65 7465  ersion (paramete
+00001080: 7220 6368 6563 6b20 6465 7065 6e64 7320  r check depends 
+00001090: 6f6e 2060 5079 6461 6e74 6963 6029 5c6e  on `Pydantic`)\n
+000010a0: 202d 205b 785d 2050 6172 616d 6574 6572   - [x] Parameter
+000010b0: 2064 6570 656e 6465 6e63 7920 7665 7269   dependency veri
+000010c0: 6669 6361 7469 6f6e 5c6e 202d 205b 785d  fication\n - [x]
+000010d0: 2041 7574 6f6d 6174 6963 616c 6c79 2067   Automatically g
+000010e0: 656e 6572 6174 6520 6f70 656e 6170 6920  enerate openapi 
+000010f0: 6669 6c65 735c 6e20 2d20 5b78 5d20 5377  files\n - [x] Sw
+00001100: 6167 6765 722c 2052 6564 6f63 2072 6f75  agger, Redoc rou
+00001110: 7465 5c6e 202d 205b 785d 2067 5250 4320  te\n - [x] gRPC 
+00001120: 4761 7465 7761 7920 726f 7574 655c 6e20  Gateway route\n 
+00001130: 2d20 5b78 5d20 5465 7374 436c 6965 6e74  - [x] TestClient
+00001140: 2073 7570 706f 7274 2c20 7375 7070 6f72   support, suppor
+00001150: 7420 7265 7370 6f6e 7365 2072 6573 756c  t response resul
+00001160: 7420 7665 7269 6669 6361 7469 6f6e 5c6e  t verification\n
+00001170: 202d 205b 785d 2053 7570 706f 7274 2066   - [x] Support f
+00001180: 6f72 2070 6c75 6769 6e20 6578 7465 6e73  or plugin extens
+00001190: 696f 6e73 2c20 7375 6368 2061 7320 7468  ions, such as th
+000011a0: 6520 4d6f 636b 2070 6c75 6769 6e5c 6e5c  e Mock plugin\n\
+000011b0: 6e23 2049 6e73 7461 6c6c 6174 696f 6e5c  n# Installation\
+000011c0: 6e60 6060 4261 7368 5c6e 7069 7020 696e  n```Bash\npip in
+000011d0: 7374 616c 6c20 7061 6974 5c6e 6060 605c  stall pait\n```\
+000011e0: 6e23 2053 696d 706c 6520 4578 616d 706c  n# Simple Exampl
+000011f0: 655c 6e60 6060 7079 7468 6f6e 5c6e 6672  e\n```python\nfr
+00001200: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00001210: 2054 7970 655c 6e69 6d70 6f72 7420 7576   Type\nimport uv
+00001220: 6963 6f72 6e20 2023 2074 7970 653a 2069  icorn  # type: i
+00001230: 676e 6f72 655c 6e66 726f 6d20 7374 6172  gnore\nfrom star
+00001240: 6c65 7474 652e 6170 706c 6963 6174 696f  lette.applicatio
+00001250: 6e73 2069 6d70 6f72 7420 5374 6172 6c65  ns import Starle
+00001260: 7474 655c 6e66 726f 6d20 7374 6172 6c65  tte\nfrom starle
+00001270: 7474 652e 7265 7370 6f6e 7365 7320 696d  tte.responses im
+00001280: 706f 7274 204a 534f 4e52 6573 706f 6e73  port JSONRespons
+00001290: 655c 6e66 726f 6d20 7374 6172 6c65 7474  e\nfrom starlett
+000012a0: 652e 726f 7574 696e 6720 696d 706f 7274  e.routing import
+000012b0: 2052 6f75 7465 5c6e 5c6e 6672 6f6d 2070   Route\n\nfrom p
+000012c0: 6169 742e 6170 702e 7374 6172 6c65 7474  ait.app.starlett
+000012d0: 6520 696d 706f 7274 2070 6169 742c 2061  e import pait, a
+000012e0: 6464 5f64 6f63 5f72 6f75 7465 5c6e 6672  dd_doc_route\nfr
+000012f0: 6f6d 2070 6169 742e 6669 656c 6420 696d  om pait.field im
+00001300: 706f 7274 2042 6f64 795c 6e66 726f 6d20  port Body\nfrom 
+00001310: 7061 6974 2e6d 6f64 656c 2e72 6573 706f  pait.model.respo
+00001320: 6e73 6520 696d 706f 7274 2050 6169 7452  nse import PaitR
+00001330: 6573 706f 6e73 654d 6f64 656c 5c6e 6672  esponseModel\nfr
+00001340: 6f6d 2070 7964 616e 7469 6320 696d 706f  om pydantic impo
+00001350: 7274 2042 6173 654d 6f64 656c 2c20 4669  rt BaseModel, Fi
+00001360: 656c 645c 6e5c 6e5c 6e63 6c61 7373 2044  eld\n\n\nclass D
+00001370: 656d 6f52 6573 706f 6e73 654d 6f64 656c  emoResponseModel
+00001380: 2850 6169 7452 6573 706f 6e73 654d 6f64  (PaitResponseMod
+00001390: 656c 293a 5c6e 2020 2020 636c 6173 7320  el):\n    class 
+000013a0: 5265 7370 6f6e 7365 4d6f 6465 6c28 4261  ResponseModel(Ba
+000013b0: 7365 4d6f 6465 6c29 3a5c 6e20 2020 2020  seModel):\n     
+000013c0: 2020 2075 6964 3a20 696e 7420 3d20 4669     uid: int = Fi
+000013d0: 656c 6428 295c 6e20 2020 2020 2020 2075  eld()\n        u
+000013e0: 7365 725f 6e61 6d65 3a20 7374 7220 3d20  ser_name: str = 
+000013f0: 4669 656c 6428 295c 6e5c 6e20 2020 2064  Field()\n\n    d
+00001400: 6573 6372 6970 7469 6f6e 3a20 7374 7220  escription: str 
+00001410: 3d20 2264 656d 6f20 7265 7370 6f6e 7365  = "demo response
+00001420: 225c 6e20 2020 2072 6573 706f 6e73 655f  "\n    response_
+00001430: 6461 7461 3a20 5479 7065 5b42 6173 654d  data: Type[BaseM
+00001440: 6f64 656c 5d20 3d20 5265 7370 6f6e 7365  odel] = Response
+00001450: 4d6f 6465 6c5c 6e5c 6e5c 6e40 7061 6974  Model\n\n\n@pait
+00001460: 2872 6573 706f 6e73 655f 6d6f 6465 6c5f  (response_model_
+00001470: 6c69 7374 3d5b 4465 6d6f 5265 7370 6f6e  list=[DemoRespon
+00001480: 7365 4d6f 6465 6c5d 295c 6e61 7379 6e63  seModel])\nasync
+00001490: 2064 6566 2064 656d 6f5f 706f 7374 285c   def demo_post(\
+000014a0: 6e20 2020 2075 6964 3a20 696e 7420 3d20  n    uid: int = 
+000014b0: 426f 6479 2e69 2864 6573 6372 6970 7469  Body.i(descripti
+000014c0: 6f6e 3d22 7573 6572 2069 6422 2c20 6774  on="user id", gt
+000014d0: 3d31 302c 206c 743d 3130 3030 292c 5c6e  =10, lt=1000),\n
+000014e0: 2020 2020 7573 6572 5f6e 616d 653a 2073      user_name: s
+000014f0: 7472 203d 2042 6f64 792e 6928 6465 7363  tr = Body.i(desc
+00001500: 7269 7074 696f 6e3d 2275 7365 7220 6e61  ription="user na
+00001510: 6d65 222c 206d 696e 5f6c 656e 6774 683d  me", min_length=
+00001520: 322c 206d 6178 5f6c 656e 6774 683d 3429  2, max_length=4)
+00001530: 5c6e 2920 2d3e 204a 534f 4e52 6573 706f  \n) -> JSONRespo
+00001540: 6e73 653a 5c6e 2020 2020 7265 7475 726e  nse:\n    return
+00001550: 204a 534f 4e52 6573 706f 6e73 6528 7b5c   JSONResponse({\
+00001560: 2775 6964 5c27 3a20 7569 642c 205c 2775  'uid\': uid, \'u
+00001570: 7365 725f 6e61 6d65 5c27 3a20 7573 6572  ser_name\': user
+00001580: 5f6e 616d 657d 295c 6e5c 6e5c 6e61 7070  _name})\n\n\napp
+00001590: 203d 2053 7461 726c 6574 7465 2872 6f75   = Starlette(rou
+000015a0: 7465 733d 5b52 6f75 7465 285c 272f 6170  tes=[Route(\'/ap
+000015b0: 695c 272c 2064 656d 6f5f 706f 7374 2c20  i\', demo_post, 
+000015c0: 6d65 7468 6f64 733d 5b5c 2750 4f53 545c  methods=[\'POST\
+000015d0: 275d 295d 295c 6e61 6464 5f64 6f63 5f72  '])])\nadd_doc_r
+000015e0: 6f75 7465 2861 7070 295c 6e75 7669 636f  oute(app)\nuvico
+000015f0: 726e 2e72 756e 2861 7070 295c 6e60 6060  rn.run(app)\n```
+00001600: 5c6e 5c6e 2320 486f 7720 746f 2075 7365  \n\n# How to use
+00001610: 6420 696e 206f 7468 6572 2077 6562 2066  d in other web f
+00001620: 7261 6d65 776f 726b 3f5c 6e49 6620 7468  ramework?\nIf th
+00001630: 6520 7765 6220 6672 616d 6577 6f72 6b20  e web framework 
+00001640: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+00001650: 2c20 7768 6963 6820 796f 7520 6172 6520  , which you are 
+00001660: 7573 696e 672e 5c6e 5c6e 4361 6e20 6265  using.\n\nCan be
+00001670: 206d 6f64 6966 6965 6420 7379 6e63 2077   modified sync w
+00001680: 6562 2066 7261 6d65 776f 726b 2061 6363  eb framework acc
+00001690: 6f72 6469 6e67 2074 6f20 5b70 6169 742e  ording to [pait.
+000016a0: 6170 702e 666c 6173 6b5d 2868 7474 7073  app.flask](https
+000016b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 736f  ://github.com/so
+000016c0: 316e 2f70 6169 742f 626c 6f62 2f6d 6173  1n/pait/blob/mas
+000016d0: 7465 722f 7061 6974 2f61 7070 2f66 6c61  ter/pait/app/fla
+000016e0: 736b 2e70 7929 5c6e 5c6e 4361 6e20 6265  sk.py)\n\nCan be
+000016f0: 206d 6f64 6966 6965 6420 6173 796e 6320   modified async 
+00001700: 7765 6220 6672 616d 6577 6f72 6b20 6163  web framework ac
+00001710: 636f 7264 696e 6720 746f 205b 7061 6974  cording to [pait
+00001720: 2e61 7070 2e73 7461 726c 6574 7465 5d28  .app.starlette](
+00001730: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001740: 6f6d 2f73 6f31 6e2f 7061 6974 2f62 6c6f  om/so1n/pait/blo
+00001750: 622f 6d61 7374 6572 2f70 6169 742f 6170  b/master/pait/ap
+00001760: 702f 7374 6172 6c65 7474 652e 7079 295c  p/starlette.py)\
+00001770: 6e23 2049 4445 2053 7570 706f 7274 5c6e  n# IDE Support\n
+00001780: 5768 696c 6520 7079 6461 6e74 6963 2077  While pydantic w
+00001790: 696c 6c20 776f 726b 2077 656c 6c20 7769  ill work well wi
+000017a0: 7468 2061 6e79 2049 4445 206f 7574 206f  th any IDE out o
+000017b0: 6620 7468 6520 626f 782e 5c6e 2d20 5b50  f the box.\n- [P
+000017c0: 7943 6861 726d 2070 6c75 6769 6e5d 2868  yCharm plugin](h
+000017d0: 7474 7073 3a2f 2f70 7964 616e 7469 632d  ttps://pydantic-
+000017e0: 646f 6373 2e68 656c 706d 616e 7561 6c2e  docs.helpmanual.
+000017f0: 696f 2f70 7963 6861 726d 5f70 6c75 6769  io/pycharm_plugi
+00001800: 6e2f 295c 6e2d 205b 4d79 7079 2070 6c75  n/)\n- [Mypy plu
+00001810: 6769 6e5d 2868 7474 7073 3a2f 2f70 7964  gin](https://pyd
+00001820: 616e 7469 632d 646f 6373 2e68 656c 706d  antic-docs.helpm
+00001830: 616e 7561 6c2e 696f 2f6d 7970 795f 706c  anual.io/mypy_pl
+00001840: 7567 696e 2f29 5c6e 5c6e 2320 4675 6c6c  ugin/)\n\n# Full
+00001850: 2065 7861 6d70 6c65 5c6e 466f 7220 6d6f   example\nFor mo
+00001860: 7265 2063 6f6d 706c 6574 6520 6578 616d  re complete exam
+00001870: 706c 6573 2c20 706c 6561 7365 2072 6566  ples, please ref
+00001880: 6572 2074 6f20 5b65 7861 6d70 6c65 5d28  er to [example](
+00001890: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000018a0: 6f6d 2f73 6f31 6e2f 7061 6974 2f74 7265  om/so1n/pait/tre
+000018b0: 652f 6d61 7374 6572 2f65 7861 6d70 6c65  e/master/example
+000018c0: 295c 6e27 2c0a 2020 2020 2761 7574 686f  )\n',.    'autho
+000018d0: 7227 3a20 2753 6f31 6e27 2c0a 2020 2020  r': 'So1n',.    
+000018e0: 2761 7574 686f 725f 656d 6169 6c27 3a20  'author_email': 
+000018f0: 2773 6f31 6e38 3937 3034 3630 3236 4067  'so1n897046026@g
+00001900: 6d61 696c 2e63 6f6d 272c 0a20 2020 2027  mail.com',.    '
+00001910: 6d61 696e 7461 696e 6572 273a 2027 4e6f  maintainer': 'No
+00001920: 6e65 272c 0a20 2020 2027 6d61 696e 7461  ne',.    'mainta
+00001930: 696e 6572 5f65 6d61 696c 273a 2027 4e6f  iner_email': 'No
+00001940: 6e65 272c 0a20 2020 2027 7572 6c27 3a20  ne',.    'url': 
+00001950: 2768 7474 7073 3a2f 2f67 6974 6875 622e  'https://github.
+00001960: 636f 6d2f 736f 316e 2f70 6169 7427 2c0a  com/so1n/pait',.
+00001970: 2020 2020 2770 6163 6b61 6765 7327 3a20      'packages': 
+00001980: 7061 636b 6167 6573 2c0a 2020 2020 2770  packages,.    'p
+00001990: 6163 6b61 6765 5f64 6174 6127 3a20 7061  ackage_data': pa
+000019a0: 636b 6167 655f 6461 7461 2c0a 2020 2020  ckage_data,.    
+000019b0: 2769 6e73 7461 6c6c 5f72 6571 7569 7265  'install_require
+000019c0: 7327 3a20 696e 7374 616c 6c5f 7265 7175  s': install_requ
+000019d0: 6972 6573 2c0a 2020 2020 2765 7874 7261  ires,.    'extra
+000019e0: 735f 7265 7175 6972 6527 3a20 6578 7472  s_require': extr
+000019f0: 6173 5f72 6571 7569 7265 2c0a 2020 2020  as_require,.    
+00001a00: 2765 6e74 7279 5f70 6f69 6e74 7327 3a20  'entry_points': 
+00001a10: 656e 7472 795f 706f 696e 7473 2c0a 2020  entry_points,.  
+00001a20: 2020 2770 7974 686f 6e5f 7265 7175 6972    'python_requir
+00001a30: 6573 273a 2027 3e3d 332e 372c 3c34 2e30  es': '>=3.7,<4.0
+00001a40: 272c 0a7d 0a0a 0a73 6574 7570 282a 2a73  ',.}...setup(**s
+00001a50: 6574 7570 5f6b 7761 7267 7329 0a         etup_kwargs).
```

