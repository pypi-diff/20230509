# Comparing `tmp/servey-2.8.3.tar.gz` & `tmp/servey-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/servey-2.8.3.tar", last modified: Wed Apr 19 00:37:19 2023, max compression
+gzip compressed data, was "servey-2.8.4.tar", last modified: Tue May  9 21:39:32 2023, max compression
```

## Comparing `servey-2.8.3.tar` & `servey-2.8.4.tar`

### file list

```diff
@@ -1,194 +1,193 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.402324 servey-2.8.3/
--rw-r--r--   0 tofarr     (501) staff       (20)    17979 2023-04-19 00:37:19.401919 servey-2.8.3/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)    17465 2023-04-05 22:22:08.000000 servey-2.8.3/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.249573 servey-2.8.3/marshy_config_servey/
--rw-r--r--   0 tofarr     (501) staff       (20)    14673 2023-04-12 03:49:23.000000 servey-2.8.3/marshy_config_servey/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.251662 servey-2.8.3/servey/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-20 13:05:09.000000 servey-2.8.3/servey/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2478 2023-04-05 21:10:12.000000 servey-2.8.3/servey/__main__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.268685 servey-2.8.3/servey/action/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/action/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2763 2023-01-20 16:29:37.000000 servey-2.8.3/servey/action/action.py
--rw-r--r--   0 tofarr     (501) staff       (20)      233 2023-01-05 15:20:43.000000 servey-2.8.3/servey/action/batch_invoker.py
--rw-r--r--   0 tofarr     (501) staff       (20)      460 2022-12-09 15:33:15.000000 servey-2.8.3/servey/action/example.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4148 2023-01-06 03:56:01.000000 servey-2.8.3/servey/action/util.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.271619 servey-2.8.3/servey/cache_control/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-11-17 03:52:02.000000 servey-2.8.3/servey/cache_control/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      467 2022-12-09 17:19:54.000000 servey-2.8.3/servey/cache_control/cache_control_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2307 2023-04-05 21:10:12.000000 servey-2.8.3/servey/cache_control/cache_header.py
--rw-r--r--   0 tofarr     (501) staff       (20)      704 2023-02-03 15:04:24.000000 servey-2.8.3/servey/cache_control/secure_hash_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1356 2022-12-24 00:22:46.000000 servey-2.8.3/servey/cache_control/timestamp_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1274 2023-04-05 21:10:12.000000 servey-2.8.3/servey/cache_control/ttl_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)       39 2022-11-30 20:16:33.000000 servey-2.8.3/servey/errors.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.274063 servey-2.8.3/servey/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/finder/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      836 2023-01-05 15:20:43.000000 servey-2.8.3/servey/finder/action_finder_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1777 2023-01-20 16:29:37.000000 servey-2.8.3/servey/finder/module_action_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1601 2023-01-20 16:29:37.000000 servey-2.8.3/servey/finder/module_subscription_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)      653 2023-01-05 15:20:43.000000 servey-2.8.3/servey/finder/subscription_finder_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.274951 servey-2.8.3/servey/security/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/security/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.277289 servey-2.8.3/servey/security/access_control/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/security/access_control/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      335 2023-03-19 15:03:39.000000 servey-2.8.3/servey/security/access_control/access_control_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      357 2023-01-05 15:20:43.000000 servey-2.8.3/servey/security/access_control/allow_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-01-05 15:20:43.000000 servey-2.8.3/servey/security/access_control/allow_none.py
--rw-r--r--   0 tofarr     (501) staff       (20)      516 2023-01-05 15:20:43.000000 servey-2.8.3/servey/security/access_control/scope_access_control.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.278827 servey-2.8.3/servey/security/authenticator/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 00:28:02.000000 servey-2.8.3/servey/security/authenticator/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      614 2023-01-18 13:36:34.000000 servey-2.8.3/servey/security/authenticator/password_authenticator_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1200 2023-01-18 13:36:35.000000 servey-2.8.3/servey/security/authenticator/root_password_authenticator.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2407 2022-12-18 16:01:20.000000 servey-2.8.3/servey/security/authorization.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.281380 servey-2.8.3/servey/security/authorizer/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/security/authorizer/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      446 2022-09-16 02:42:12.000000 servey-2.8.3/servey/security/authorizer/authorizer_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1343 2022-12-09 15:17:12.000000 servey-2.8.3/servey/security/authorizer/authorizer_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2821 2022-12-16 15:10:54.000000 servey-2.8.3/servey/security/authorizer/jwt_authorizer.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1154 2022-11-30 20:16:33.000000 servey-2.8.3/servey/security/authorizer/jwt_authorizer_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.286316 servey-2.8.3/servey/servey_aws/
--rw-r--r--   0 tofarr     (501) staff       (20)       91 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.288813 servey-2.8.3/servey/servey_aws/authorizer/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_aws/authorizer/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4516 2022-12-17 21:34:00.000000 servey-2.8.3/servey/servey_aws/authorizer/kms_authorizer.py
--rw-r--r--   0 tofarr     (501) staff       (20)      923 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/authorizer/kms_authorizer_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.294234 servey-2.8.3/servey/servey_aws/event_handler/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/event_handler/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6067 2023-04-18 23:17:37.000000 servey-2.8.3/servey/servey_aws/event_handler/api_gateway_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3278 2023-04-19 00:36:44.000000 servey-2.8.3/servey/servey_aws/event_handler/appsync_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6368 2023-04-19 00:03:41.000000 servey-2.8.3/servey/servey_aws/event_handler/event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1063 2023-04-18 23:16:24.000000 servey-2.8.3/servey/servey_aws/event_handler/event_handler_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2644 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/event_handler/sqs_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2089 2023-04-15 12:20:50.000000 servey-2.8.3/servey/servey_aws/lambda_invoker.py
--rw-r--r--   0 tofarr     (501) staff       (20)      878 2023-04-04 04:13:04.000000 servey-2.8.3/servey/servey_aws/lambda_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4214 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/lambda_websocket.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.298288 servey-2.8.3/servey/servey_aws/router/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 13:29:47.000000 servey-2.8.3/servey/servey_aws/router/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1173 2023-04-18 23:10:42.000000 servey-2.8.3/servey/servey_aws/router/api_gateway_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2733 2023-04-18 23:45:35.000000 servey-2.8.3/servey/servey_aws/router/appsync_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)      792 2023-04-18 23:11:48.000000 servey-2.8.3/servey/servey_aws/router/router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1490 2023-04-18 23:10:42.000000 servey-2.8.3/servey/servey_aws/router/router_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.300141 servey-2.8.3/servey/servey_aws/serverless/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_aws/serverless/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1245 2023-03-30 22:57:04.000000 servey-2.8.3/servey/servey_aws/serverless/__main__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.304245 servey-2.8.3/servey/servey_aws/serverless/trigger_handler/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_aws/serverless/trigger_handler/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-18 13:36:35.000000 servey-2.8.3/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)      442 2022-12-17 21:14:47.000000 servey-2.8.3/servey/servey_aws/serverless/trigger_handler/trigger_handler_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1090 2023-01-07 16:53:22.000000 servey-2.8.3/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.313847 servey-2.8.3/servey/servey_aws/serverless/yml_config/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3987 2023-04-05 23:49:53.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/action_function_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5894 2023-04-18 22:49:01.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/appsync_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)    10858 2023-04-15 12:30:22.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/cloudfront_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3593 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/kms_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      625 2023-04-12 04:18:55.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/serverless_template.yml
--rw-r--r--   0 tofarr     (501) staff       (20)     5248 2023-04-12 04:44:32.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     7374 2023-04-06 12:59:59.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/subscription_function_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2947 2023-01-18 13:16:57.000000 servey-2.8.3/servey/servey_aws/serverless/yml_config/yml_config_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2179 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/sqs_subscription_service.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3210 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_aws/websocket_subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.318739 servey-2.8.3/servey/servey_celery/
--rw-r--r--   0 tofarr     (501) staff       (20)       86 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_celery/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1429 2023-01-07 16:31:15.000000 servey-2.8.3/servey/servey_celery/celery_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.323727 servey-2.8.3/servey/servey_celery/celery_config/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 16:19:02.000000 servey-2.8.3/servey/servey_celery/celery_config/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      241 2023-01-07 16:53:22.000000 servey-2.8.3/servey/servey_celery/celery_config/celery_config_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1004 2023-04-01 19:42:31.000000 servey-2.8.3/servey/servey_celery/celery_config/fixed_rate_trigger_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      592 2023-01-07 16:53:22.000000 servey-2.8.3/servey/servey_celery/celery_config/subscription_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1050 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_celery/celery_subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.325746 servey-2.8.3/servey/servey_direct/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-16 16:23:58.000000 servey-2.8.3/servey/servey_direct/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1313 2023-04-05 21:10:12.000000 servey-2.8.3/servey/servey_direct/__main__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.328490 servey-2.8.3/servey/servey_starlette/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_starlette/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.333354 servey-2.8.3/servey/servey_starlette/action_endpoint/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 15:42:17.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)    11862 2023-04-05 21:10:12.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-01-19 13:50:13.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/action_endpoint_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3401 2023-03-19 15:03:39.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2836 2023-03-19 15:03:39.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/caching_action_endpoint.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.338932 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 17:29:46.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2786 2023-01-06 15:28:44.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      822 2022-12-11 13:56:30.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2183 2022-12-11 14:21:14.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1444 2022-12-16 15:10:54.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2260 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      201 2022-12-24 01:22:04.000000 servey-2.8.3/servey/servey_starlette/error_response.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.347800 servey-2.8.3/servey/servey_starlette/route_factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_starlette/route_factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1600 2023-01-06 15:28:44.000000 servey-2.8.3/servey/servey_starlette/route_factory/action_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3026 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_starlette/route_factory/asyncapi_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1928 2023-01-18 13:36:35.000000 servey-2.8.3/servey/servey_starlette/route_factory/authenticator_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2441 2023-01-20 16:29:37.000000 servey-2.8.3/servey/servey_starlette/route_factory/openapi_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      242 2023-01-14 15:50:20.000000 servey-2.8.3/servey/servey_starlette/route_factory/route_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      718 2023-01-18 13:36:35.000000 servey-2.8.3/servey/servey_starlette/route_factory/static_site_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6329 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_starlette/route_factory/subscription_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      521 2023-01-18 13:36:35.000000 servey-2.8.3/servey/servey_starlette/starlette_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.354936 servey-2.8.3/servey/servey_starlette/statics/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-11-30 19:30:04.000000 servey-2.8.3/servey/servey_starlette/statics/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      794 2022-09-16 02:41:41.000000 servey-2.8.3/servey/servey_starlette/statics/index.html
--rw-r--r--   0 tofarr     (501) staff       (20)  1079398 2022-12-04 20:38:25.000000 servey-2.8.3/servey/servey_starlette/statics/swagger-ui-bundle.js
--rw-r--r--   0 tofarr     (501) staff       (20)   192198 2022-09-16 02:41:41.000000 servey-2.8.3/servey/servey_starlette/statics/swagger-ui.css
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.364593 servey-2.8.3/servey/servey_strawberry/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_strawberry/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.377349 servey-2.8.3/servey/servey_strawberry/entity_factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5804 2023-04-05 21:10:12.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/dataclass_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      515 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/entity_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1105 2023-04-18 21:27:38.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/enum_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      890 2022-12-16 11:34:08.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/forward_ref_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1343 2022-12-18 22:53:24.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/generic_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      688 2022-12-18 22:59:58.000000 servey-2.8.3/servey/servey_strawberry/entity_factory/no_op_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.380387 servey-2.8.3/servey/servey_strawberry/handler_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_strawberry/handler_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3179 2023-01-07 04:41:39.000000 servey-2.8.3/servey/servey_strawberry/handler_filter/authorization_handler_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      687 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_strawberry/handler_filter/handler_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1406 2022-12-27 15:18:15.000000 servey-2.8.3/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     7228 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_strawberry/schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      754 2022-12-16 15:10:54.000000 servey-2.8.3/servey/servey_strawberry/schema_factory_lazy_input.py
--rw-r--r--   0 tofarr     (501) staff       (20)      752 2022-12-16 15:10:54.000000 servey-2.8.3/servey/servey_strawberry/schema_factory_lazy_type.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.381711 servey-2.8.3/servey/servey_strawberry/statics/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-11-30 19:30:04.000000 servey-2.8.3/servey/servey_strawberry/statics/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1872 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_strawberry/statics/index.html
--rw-r--r--   0 tofarr     (501) staff       (20)     1726 2023-01-20 16:29:37.000000 servey-2.8.3/servey/servey_strawberry/strawberry_starlette_route_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.383285 servey-2.8.3/servey/servey_test/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-04 20:47:53.000000 servey-2.8.3/servey/servey_test/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1164 2022-12-16 20:57:24.000000 servey-2.8.3/servey/servey_test/test_servey_actions.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.386408 servey-2.8.3/servey/servey_thread/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/servey_thread/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      905 2023-01-05 15:10:21.000000 servey-2.8.3/servey/servey_thread/__main__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1315 2023-01-05 15:20:43.000000 servey-2.8.3/servey/servey_thread/asyncio_subscription_service.py
--rw-r--r--   0 tofarr     (501) staff       (20)      515 2022-12-16 18:31:33.000000 servey-2.8.3/servey/servey_thread/fixed_rate_trigger_thread.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.392261 servey-2.8.3/servey/servey_web_page/
--rw-r--r--   0 tofarr     (501) staff       (20)      213 2023-01-20 16:29:37.000000 servey-2.8.3/servey/servey_web_page/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      103 2023-03-19 15:03:39.000000 servey-2.8.3/servey/servey_web_page/redirect.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1687 2023-04-05 21:10:12.000000 servey-2.8.3/servey/servey_web_page/web_page_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2604 2023-04-05 21:10:12.000000 servey-2.8.3/servey/servey_web_page/web_page_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4335 2023-04-05 21:10:12.000000 servey-2.8.3/servey/servey_web_page/web_page_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)      709 2023-01-20 16:29:37.000000 servey-2.8.3/servey/servey_web_page/web_page_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)      848 2023-01-20 16:29:37.000000 servey-2.8.3/servey/servey_web_page/web_page_trigger_handler.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.396384 servey-2.8.3/servey/subscription/
--rw-r--r--   0 tofarr     (501) staff       (20)      595 2023-01-05 15:20:43.000000 servey-2.8.3/servey/subscription/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      392 2023-01-05 15:20:43.000000 servey-2.8.3/servey/subscription/event_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1698 2023-01-05 15:20:43.000000 servey-2.8.3/servey/subscription/subscription.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1009 2023-01-05 15:20:43.000000 servey-2.8.3/servey/subscription/subscription_event.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1367 2023-01-05 15:20:43.000000 servey-2.8.3/servey/subscription/subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.399128 servey-2.8.3/servey/trigger/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.8.3/servey/trigger/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      165 2022-12-08 23:20:52.000000 servey-2.8.3/servey/trigger/fixed_rate_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)       92 2022-09-16 02:42:12.000000 servey-2.8.3/servey/trigger/trigger_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      762 2023-01-05 22:00:38.000000 servey-2.8.3/servey/trigger/web_trigger.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.401287 servey-2.8.3/servey/util/
--rw-r--r--   0 tofarr     (501) staff       (20)     1289 2023-04-13 14:21:17.000000 servey-2.8.3/servey/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      839 2022-08-10 15:17:22.000000 servey-2.8.3/servey/util/singleton_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      472 2022-12-17 21:18:47.000000 servey-2.8.3/servey/util/to_second_datetime_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-19 00:36:51.000000 servey-2.8.3/servey/version.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-19 00:37:19.266137 servey-2.8.3/servey.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)    17979 2023-04-19 00:37:19.000000 servey-2.8.3/servey.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     7327 2023-04-19 00:37:19.000000 servey-2.8.3/servey.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-19 00:37:19.000000 servey-2.8.3/servey.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)      530 2023-04-19 00:37:19.000000 servey-2.8.3/servey.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       28 2023-04-19 00:37:19.000000 servey-2.8.3/servey.egg-info/top_level.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-19 00:37:19.402463 servey-2.8.3/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)     1680 2023-04-19 00:20:46.000000 servey-2.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-09 21:39:21.000000 servey-2.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-05-09 21:39:32.574175 servey-2.8.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.542175 servey-2.8.4/marshy_config_servey/
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-09 21:39:21.000000 servey-2.8.4/marshy_config_servey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.542175 servey-2.8.4/servey/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-09 21:39:21.000000 servey-2.8.4/servey/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.546175 servey-2.8.4/servey/action/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/batch_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-09 21:39:21.000000 servey-2.8.4/servey/action/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/cache_control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/cache_control_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/cache_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/secure_hash_cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/timestamp_cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-09 21:39:21.000000 servey-2.8.4/servey/cache_control/ttl_cache_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-09 21:39:21.000000 servey-2.8.4/servey/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/finder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/action_finder_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/module_action_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/module_subscription_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-09 21:39:21.000000 servey-2.8.4/servey/finder/subscription_finder_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/access_control/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/access_control_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/allow_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/allow_none.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/access_control/scope_access_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/authenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authenticator/password_authenticator_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authenticator/root_password_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.550175 servey-2.8.4/servey/security/authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/authorizer_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/authorizer_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/jwt_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 21:39:21.000000 servey-2.8.4/servey/security/authorizer/jwt_authorizer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/authorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/authorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/event_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/api_gateway_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/appsync_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/event_handler_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/event_handler/sqs_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/lambda_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/lambda_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/lambda_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/router/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/api_gateway_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/appsync_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/router/router_abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.554175 servey-2.8.4/servey/servey_aws/serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/trigger_handler_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_aws/serverless/yml_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/action_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/appsync_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/cloudfront_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/kms_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/serverless_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/subscription_function_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/serverless/yml_config/yml_config_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/sqs_subscription_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_aws/websocket_subscription_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_celery/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_celery/celery_config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/celery_config_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/fixed_rate_trigger_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_config/subscription_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_celery/celery_subscription_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.558175 servey-2.8.4/servey/servey_direct/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_direct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_direct/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.562175 servey-2.8.4/servey/servey_starlette/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.562175 servey-2.8.4/servey/servey_starlette/action_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/caching_action_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.562175 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/error_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.566175 servey-2.8.4/servey/servey_starlette/route_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/action_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/asyncapi_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/authenticator_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/openapi_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/route_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/static_site_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/route_factory/subscription_route_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/starlette_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.566175 servey-2.8.4/servey/servey_starlette/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1079398 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   192198 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_starlette/statics/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.566175 servey-2.8.4/servey/servey_strawberry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_strawberry/entity_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/dataclass_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/entity_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/enum_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/forward_ref_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/generic_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/entity_factory/no_op_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_strawberry/handler_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/authorization_handler_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/handler_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_strawberry/statics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/statics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/statics/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_strawberry/strawberry_starlette_route_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_test/test_servey_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.570175 servey-2.8.4/servey/servey_thread/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/asyncio_subscription_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_thread/fixed_rate_trigger_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/servey_web_page/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_action_endpoint_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-09 21:39:21.000000 servey-2.8.4/servey/servey_web_page/web_page_trigger_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/event_filter_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/subscription_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-09 21:39:21.000000 servey-2.8.4/servey/subscription/subscription_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/trigger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/fixed_rate_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/trigger_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-09 21:39:21.000000 servey-2.8.4/servey/trigger/web_trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.574175 servey-2.8.4/servey/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-09 21:39:21.000000 servey-2.8.4/servey/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-09 21:39:21.000000 servey-2.8.4/servey/util/singleton_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-09 21:39:21.000000 servey-2.8.4/servey/util/to_second_datetime_marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:39:32.546175 servey-2.8.4/servey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 21:39:32.000000 servey-2.8.4/servey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:39:32.574175 servey-2.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-09 21:39:21.000000 servey-2.8.4/setup.py
```

### Comparing `servey-2.8.3/PKG-INFO` & `servey-2.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servey
-Version: 2.8.3
+Version: 2.8.4
 Summary: A better API layer for python
 Home-page: https://github.com/tofarr/servey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,29 +12,14 @@
 Provides-Extra: dev
 Provides-Extra: server
 Provides-Extra: scheduler
 Provides-Extra: serverless
 Provides-Extra: web_page
 Provides-Extra: all
 
-Example with s3 probably makes the most sense unless you want to put together a full template engine with jinja2.
-Maybe this is wanted.
-Maybe we make it an extra. How would it work?
-
-WebpageTrigger...
-
-On App Load, We execute an action, and then render a result using a Jinja Template.
-WebPageTrigger(
-  path= # defaults to /action_name
-  method= # The method to invoke
-  template= # defaults to /templates/action_name.html
-)
-
-Gives us an efficient way to mount websites as an alternative to s3
-
 # Servey - A Flexible Action Framework For Python
 
 This project specifying metadata for python functions (In a manner similar to FastAPI) which is then used to
 build REST, GraphQL, and Scheduled services. These are locally runnable / runnable in a hosted environment using
 [Starlette](https://www.starlette.io/), [Strawberry](https://strawberry.rocks/) and [Celery](https://docs.celeryq.dev/).
 They may also be run on AWS infrastructure using Serverless and Lambda. Tests and examples may also be specified for
 **actions**. General design goals are:
@@ -472,15 +457,21 @@
 We use marshy for pluggable components. See (marshy_config_servey)[marshy_config_servey/__init__.py]
 
 ## Deployment Patterns
 
 * API in ApiGateway / AppSync, SPA hosted on S3 and cloudfront out in front, Deployment of all via serverless.
 * Docker Image containing Nginx / Starlette app deployed to Heroku / Linode.
 
-## Deploying new versions of this Servey to Pypi
+## Installing local development dependencies
 
 ```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
+python setup.py install easy_install "servey[dev]"
 ```
+
+## Release Procedure
+
+![status](https://github.com/tofarr/servey/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
+* New releases created in github are automatically uploaded to pypi
```

### Comparing `servey-2.8.3/README.md` & `servey-2.8.4/servey.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Example with s3 probably makes the most sense unless you want to put together a full template engine with jinja2.
-Maybe this is wanted.
-Maybe we make it an extra. How would it work?
-
-WebpageTrigger...
-
-On App Load, We execute an action, and then render a result using a Jinja Template.
-WebPageTrigger(
-  path= # defaults to /action_name
-  method= # The method to invoke
-  template= # defaults to /templates/action_name.html
-)
-
-Gives us an efficient way to mount websites as an alternative to s3
+Metadata-Version: 2.1
+Name: servey
+Version: 2.8.4
+Summary: A better API layer for python
+Home-page: https://github.com/tofarr/servey
+Author: Tim O'Farrell
+Author-email: tofarr@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: server
+Provides-Extra: scheduler
+Provides-Extra: serverless
+Provides-Extra: web_page
+Provides-Extra: all
 
 # Servey - A Flexible Action Framework For Python
 
 This project specifying metadata for python functions (In a manner similar to FastAPI) which is then used to
 build REST, GraphQL, and Scheduled services. These are locally runnable / runnable in a hosted environment using
 [Starlette](https://www.starlette.io/), [Strawberry](https://strawberry.rocks/) and [Celery](https://docs.celeryq.dev/).
 They may also be run on AWS infrastructure using Serverless and Lambda. Tests and examples may also be specified for
@@ -454,15 +457,21 @@
 We use marshy for pluggable components. See (marshy_config_servey)[marshy_config_servey/__init__.py]
 
 ## Deployment Patterns
 
 * API in ApiGateway / AppSync, SPA hosted on S3 and cloudfront out in front, Deployment of all via serverless.
 * Docker Image containing Nginx / Starlette app deployed to Heroku / Linode.
 
-## Deploying new versions of this Servey to Pypi
+## Installing local development dependencies
 
 ```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
+python setup.py install easy_install "servey[dev]"
 ```
+
+## Release Procedure
+
+![status](https://github.com/tofarr/servey/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
+* New releases created in github are automatically uploaded to pypi
```

### Comparing `servey-2.8.3/marshy_config_servey/__init__.py` & `servey-2.8.4/marshy_config_servey/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,16 @@
 
 def configure_serverless(context: MarshallerContext):
     try:
         from servey.servey_aws.serverless.yml_config.yml_config_abc import YmlConfigABC
         from servey.servey_aws.serverless.yml_config.action_function_config import (
             ActionFunctionConfig,
         )
+
+        # pylint: disable=E0001
         from servey.servey_aws.serverless.yml_config.appsync_config import AppsyncConfig
         from servey.servey_aws.serverless.yml_config.kms_key_config import KmsKeyConfig
         from servey.servey_aws.serverless.yml_config.subscription_function_config import (
             SubscriptionFunctionConfig,
         )
 
         register_impl(YmlConfigABC, ActionFunctionConfig, context)
@@ -275,18 +277,18 @@
             FixedRateTriggerHandler,
         )
 
         register_impl(TriggerHandlerABC, WebTriggerHandler, context)
         register_impl(TriggerHandlerABC, FixedRateTriggerHandler, context)
 
         from servey.servey_aws.serverless.yml_config.cloudfront_config import (
-            CloudfrontConfig
+            CloudfrontConfig,
         )
         from servey.servey_aws.serverless.yml_config.static_site_bucket_config import (
-            StaticSiteBucketConfig
+            StaticSiteBucketConfig,
         )
 
         register_impl(YmlConfigABC, CloudfrontConfig, context)
         register_impl(YmlConfigABC, StaticSiteBucketConfig, context)
 
     except ModuleNotFoundError as e:
         raise_non_ignored(e)
@@ -315,14 +317,16 @@
 
     except ModuleNotFoundError as e:
         raise_non_ignored(e)
 
 
 def configure_jinja2(context: MarshallerContext):
     try:
+        # We import Template to test that jinja2 is actually present
+        # pylint: disable=W0611
         from jinja2 import Template
 
         configure_web_page_action_endpoint_factory(context)
         configure_web_page_event_handler(context)
         configure_web_page_trigger_handler(context)
     except ModuleNotFoundError as e:
         raise_non_ignored(e)
@@ -383,12 +387,12 @@
     "strawberry",
 }
 
 
 def raise_non_ignored(e: ModuleNotFoundError):
     msg = str(e)
     if msg.startswith(_NO_MODULE_NAMED):
-        module_name = msg[len(_NO_MODULE_NAMED): -1]
+        module_name = msg[len(_NO_MODULE_NAMED) : -1]
         if module_name in _IGNORABLE_MISSING_MODULE_NAMES:
             LOGGER.debug(msg)
             return
     raise e
```

### Comparing `servey-2.8.3/servey/__main__.py` & `servey-2.8.4/servey/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         log_level=LOGLEVEL.lower(),
         reload=DEBUG,
         reload_includes=["*.j2", "*.py"],
         reload_dirs=["."],
     )
 
 
+# pylint: disable=W0611
 def start_scheduler():
     if CELERY_BROKER:
         # noinspection PyUnresolvedReferences
         import servey.servey_celery.celery_app
     else:
         os.environ["SERVEY_DAEMON"] = "1"
         # noinspection PyUnresolvedReferences
@@ -64,26 +65,26 @@
 
 def main():
     parser = argparse.ArgumentParser(description="Servey")
     parser.add_argument("--run", default="server")
     args, _ = parser.parse_known_args()
     if args.run == "sls":
         # noinspection PyUnresolvedReferences
-        from servey.servey_aws.serverless.__main__ import main
+        from servey.servey_aws.serverless.__main__ import main as sls_main
 
-        main()
+        sls_main()
     elif args.run == "openapi":
         generate_openapi_schema()
     elif args.run == "graphql-schema":
         generate_graphql_schema()
     elif args.run == "action":
         # noinspection PyUnresolvedReferences
-        from servey.servey_direct.__main__ import main
+        from servey.servey_direct.__main__ import main as direct_main
 
-        main()
+        direct_main()
     elif args.run == "server":
         start_scheduler()
         start_http_server()
     else:
         raise ServeyError(f"unknown:{args.run}")
```

### Comparing `servey-2.8.3/servey/action/action.py` & `servey-2.8.4/servey/action/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from servey.security.access_control.access_control_abc import (
     AccessControlABC,
 )
 from servey.security.access_control.allow_all import ALLOW_ALL
 from servey.trigger.trigger_abc import TriggerABC
 
 
+# pylint: disable=R0902
 @dataclass(frozen=True)
 class Action:
     """
     Actions provide additional meta about a function and how it should be invoked from an external context such as REST,
     GraphQL, Tests, Mocks, or a scheduler. The intent is that everything required to document and invoke the function
     should be present here
     """
@@ -26,14 +27,15 @@
     triggers: Tuple[TriggerABC, ...] = tuple()
     timeout: int = 15
     examples: Optional[Tuple[Example, ...]] = None
     cache_control: Optional[CacheControlABC] = None
     batch_invoker: Optional[BatchInvoker] = None
 
 
+# pylint: disable=R0913
 def action(
     fn: Optional[Callable] = None,
     access_control: AccessControlABC = Action.access_control,
     triggers: Union[TriggerABC, Tuple[TriggerABC, ...]] = Action.triggers,
     timeout: int = Action.timeout,
     examples: Optional[Tuple[Example, ...]] = None,
     cache_control: Optional[CacheControlABC] = None,
```

### Comparing `servey-2.8.3/servey/action/util.py` & `servey-2.8.4/servey/action/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ) -> Schema:
     if not schema_context:
         schema_context = get_default_schema_context()
     sig = inspect.signature(fn)
     properties = {}
     required = []
     params = list(sig.parameters.values())
-    for i, p in enumerate(params):
+    for p in params:
         if p.name in skip_args:
             continue
         if p.annotation is inspect.Parameter.empty:
             raise TypeError(f"missing_param_annotation:{fn.__name__}:{p.name}")
         schema = schema_context.schema_from_type(p.annotation).schema
         properties[p.name] = _remap_references(f"#/properties/{p.name}", schema)
         if p.default == inspect.Parameter.empty:
@@ -62,20 +62,17 @@
 
 def _remap_references(to_path: str, schema: ExternalType) -> ExternalType:
     if isinstance(schema, dict):
         ref = schema.get("$ref")
         if ref and ref.startswith("#"):
             return {"$ref": to_path + ref[1:]}
         schema = {k: _remap_references(to_path, v) for k, v in schema.items()}
-        return schema
-    elif isinstance(schema, list):
+    if isinstance(schema, list):
         schema = [_remap_references(to_path, i) for i in schema]
-        return schema
-    else:
-        return schema
+    return schema
 
 
 def move_ref_items_to_components(
     root: ExternalItemType, current: ExternalType, components: ExternalItemType
 ) -> ExternalType:
     if isinstance(current, dict):
         name = current.get("name")
@@ -102,11 +99,11 @@
             name = referenced["name"]
             return {"$ref": f"#/components/{name}"}
         schema = {
             k: move_ref_items_to_components(root, v, components)
             for k, v in current.items()
         }
         return schema
-    elif isinstance(current, list):
+    if isinstance(current, list):
         schema = [move_ref_items_to_components(root, i, components) for i in current]
         return schema
     return current
```

### Comparing `servey-2.8.3/servey/cache_control/cache_header.py` & `servey-2.8.4/servey/cache_control/cache_header.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/cache_control/secure_hash_cache_control.py` & `servey-2.8.4/servey/cache_control/secure_hash_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/cache_control/timestamp_cache_control.py` & `servey-2.8.4/servey/cache_control/timestamp_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/cache_control/ttl_cache_control.py` & `servey-2.8.4/servey/cache_control/ttl_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/finder/action_finder_abc.py` & `servey-2.8.4/servey/finder/action_finder_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/finder/module_action_finder.py` & `servey-2.8.4/servey/finder/module_action_finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,21 @@
             # noinspection PyTypeChecker
             yield from _find_actions_in_module(module)
         except ModuleNotFoundError as e:
             LOGGER.warning(f"no_actions_found:{e}")
 
 
 def _find_actions_in_module(module) -> Iterator[Action]:
-    for name, value in module.__dict__.items():
+    for value in module.__dict__.values():
         action = get_action(value)
         if action:
             yield action
+        # pylint: disable=C0123
         if type(value) == type and is_dataclass(value):
-            for param_name, param_value in value.__dict__.items():
+            for param_value in value.__dict__.values():
                 action = get_action(param_value)
                 if action:
                     yield action
     if not hasattr(module, "__path__"):
         return  # Module was not a package...
     paths = []
     paths.extend(module.__path__)
```

### Comparing `servey-2.8.3/servey/finder/module_subscription_finder.py` & `servey-2.8.4/servey/finder/module_subscription_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             # noinspection PyTypeChecker
             yield from _find_subscriptions_in_module(module)
         except ModuleNotFoundError as e:
             LOGGER.info(f"no_subscriptions_found:{e}")
 
 
 def _find_subscriptions_in_module(module) -> Iterator[Subscription]:
-    for name, value in module.__dict__.items():
+    for value in module.__dict__.values():
         if isinstance(value, Subscription):
             yield value
     if not hasattr(module, "__path__"):
         return  # Module was not a package...
     paths = []
     paths.extend(module.__path__)
     module_infos = list(pkgutil.walk_packages(paths))
```

### Comparing `servey-2.8.3/servey/finder/subscription_finder_abc.py` & `servey-2.8.4/servey/finder/subscription_finder_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/security/access_control/scope_access_control.py` & `servey-2.8.4/servey/security/access_control/scope_access_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/security/authenticator/password_authenticator_abc.py` & `servey-2.8.4/servey/security/authenticator/password_authenticator_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/security/authenticator/root_password_authenticator.py` & `servey-2.8.4/servey/security/authenticator/root_password_authenticator.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/security/authorization.py` & `servey-2.8.4/servey/security/authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def has_all_scopes(self, scopes: Set[str]) -> bool:
         has_all = self.scopes.issuperset(scopes)
         return has_all
 
     def check_valid_for_timestamp(self, ts: Optional[datetime] = None):
         if not self.is_valid_for_timestamp(ts):
-            raise AuthorizationError(f"authorization_expired")
+            raise AuthorizationError("authorization_expired")
 
     def check_scope(self, scope: str):
         if not self.has_scope(scope):
             raise AuthorizationError(f"missing:{scope}")
 
     def check_any_scope(self, scopes: Set[str]):
         if not self.has_any_scope(scopes):
```

### Comparing `servey-2.8.3/servey/security/authorizer/authorizer_factory_abc.py` & `servey-2.8.4/servey/security/authorizer/authorizer_factory_abc.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,12 +29,13 @@
         if authorizer:
             return authorizer
 
 
 _default_authorizer = None
 
 
+# pylint: disable=W0603
 def get_default_authorizer():
     global _default_authorizer
     if not _default_authorizer:
         _default_authorizer = create_authorizer()
     return _default_authorizer
```

### Comparing `servey-2.8.3/servey/security/authorizer/jwt_authorizer.py` & `servey-2.8.4/servey/security/authorizer/jwt_authorizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,31 +22,31 @@
     private_key: Any
     algorithm: str = "HS256"
     kid: Optional[str] = None
     iss: Optional[str] = None
     aud: Optional[str] = None
 
     def encode(self, authorization: Authorization) -> str:
-        headers = filter_none(dict(kid=self.kid))
+        headers = filter_none({"kid": self.kid})
         encoded = jwt.encode(
             headers=headers,
             payload=filter_none(
-                dict(
-                    iss=self.iss,
-                    sub=authorization.subject_id,
-                    aud=self.aud,
-                    exp=int(authorization.expire_at.timestamp())
+                {
+                    "iss": self.iss,
+                    "sub": authorization.subject_id,
+                    "aud": self.aud,
+                    "exp": int(authorization.expire_at.timestamp())
                     if authorization.expire_at
                     else None,
-                    nbf=int(authorization.not_before.timestamp())
+                    "nbf": int(authorization.not_before.timestamp())
                     if authorization.not_before
                     else None,
-                    iat=int(datetime.now().timestamp()),
-                    scope=" ".join(authorization.scopes),
-                )
+                    "iat": int(datetime.now().timestamp()),
+                    "scope": " ".join(authorization.scopes),
+                }
             ),
             key=self.private_key,
             algorithm=self.algorithm,
         )
         return encoded
 
     @staticmethod
@@ -68,14 +68,14 @@
                 subject_id=decoded.get("sub"),
                 not_before=date_from_jwt(decoded, "nbf"),
                 expire_at=date_from_jwt(decoded, "exp"),
                 scopes=frozenset(decoded.get("scope").split(" ")),
             )
             return authorization
         except InvalidTokenError as e:
-            raise AuthorizationError(e)
+            raise AuthorizationError(e) from e
 
 
 def date_from_jwt(decoded: ExternalItemType, key: str) -> Optional[datetime]:
     value = decoded.get(key)
     if value:
         return datetime.fromtimestamp(value)
```

### Comparing `servey-2.8.3/servey/security/authorizer/jwt_authorizer_factory.py` & `servey-2.8.4/servey/security/authorizer/jwt_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/authorizer/kms_authorizer.py` & `servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,32 +38,32 @@
 
     def __post_init__(self):
         if not self.kms:
             self.kms = boto3.client("kms")
 
     def encode(self, authorization: Authorization) -> str:
         header = urlsafe_b64encode(
-            json.dumps(dict(typ="JWT", alg="RS256", kid=self.key_id)).encode()
+            json.dumps({"typ": "JWT", "alg": "RS256", "kid": self.key_id}).encode()
         )
         payload = urlsafe_b64encode(
             json.dumps(
                 filter_none(
-                    dict(
-                        iss=self.iss,
-                        sub=authorization.subject_id,
-                        aud=self.aud,
-                        exp=int(authorization.expire_at.timestamp())
+                    {
+                        "iss": self.iss,
+                        "sub": authorization.subject_id,
+                        "aud": self.aud,
+                        "exp": int(authorization.expire_at.timestamp())
                         if authorization.expire_at
                         else None,
-                        nbf=int(authorization.not_before.timestamp())
+                        "nbf": int(authorization.not_before.timestamp())
                         if authorization.not_before
                         else None,
-                        iat=int(datetime.now().timestamp()),
-                        scope=" ".join(authorization.scopes),
-                    )
+                        "iat": int(datetime.now().timestamp()),
+                        "scope": " ".join(authorization.scopes),
+                    }
                 )
             ).encode()
         )
         message = header + b"." + payload
         # noinspection SpellCheckingInspection
         result = self.kms.sign(
             Message=message,
@@ -111,8 +111,8 @@
                 subject_id=decoded.get("sub"),
                 not_before=date_from_jwt(decoded, "nbf"),
                 expire_at=date_from_jwt(decoded, "exp"),
                 scopes=frozenset(decoded.get("scope").split(" ")),
             )
             return authorization
         except DecodeError as e:
-            raise AuthorizationError(e)
+            raise AuthorizationError(e) from e
```

### Comparing `servey-2.8.3/servey/servey_aws/authorizer/kms_authorizer_factory.py` & `servey-2.8.4/servey/servey_aws/authorizer/kms_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/event_handler/api_gateway_event_handler.py` & `servey-2.8.4/servey/servey_aws/event_handler/api_gateway_event_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import inspect
 import json
 from dataclasses import field, dataclass
 from email.utils import parsedate_to_datetime
-from typing import Optional, Any, Awaitable
+from typing import Optional, Awaitable
 
 from marshy import get_default_context, ExternalType
 from marshy.marshaller_context import MarshallerContext
 from marshy.types import ExternalItemType
 from marshy.utils import resolve_forward_refs
 from schemey import get_default_schema_context, SchemaContext
 
@@ -57,15 +57,15 @@
         headers = event.get("headers") or {}
         token = (headers.get("Authorization") or "").strip()
         if not token or not token.startswith("Bearer "):
             return
         token = token[7:]
         return self.authorizer.authorize(token)
 
-    def handle(self, event: ExternalItemType, result: Any) -> ExternalItemType:
+    def handle(self, event: ExternalItemType, context) -> ExternalItemType:
         kwargs = self.parse_kwargs(event)
         result = self.action.fn(**kwargs)
         if isinstance(result, Awaitable):
             loop = asyncio.get_event_loop()
             result = loop.run_until_complete(result)
         dumped = self.result_marshaller.dump(result)
         response = {
```

### Comparing `servey-2.8.3/servey/servey_aws/event_handler/appsync_event_handler.py` & `servey-2.8.4/servey/servey_aws/event_handler/appsync_event_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class AppsyncEventHandler(EventHandler):
     def is_usable(self, event: ExternalType, context) -> bool:
         if isinstance(event, list):
             event = event[0]
         return "arguments" in event
 
     def parse_kwargs(self, event: ExternalItemType):
-        arguments = dict(**event["arguments"])
+        arguments = {**event["arguments"]}
         source = event.get("source")
         if source is not None:
             arguments["self"] = source
         arguments = attrs_to_snake_case(arguments)
         if self.param_schema:
             self.param_schema.validate(arguments)
         kwargs = self.param_marshaller.load(arguments)
@@ -60,37 +60,21 @@
 class AppsyncEventHandlerFactory(EventHandlerFactory):
     priority: int = 100
     event_handler_type: Type[EventHandlerABC] = AppsyncEventHandler
 
 
 def attrs_to_snake_case(arguments: ExternalType) -> ExternalType:
     if isinstance(arguments, dict):
-        result = {
-            to_snake_case(k): attrs_to_snake_case(v)
-            for k, v in arguments.items()
+        arguments = {
+            to_snake_case(k): attrs_to_snake_case(v) for k, v in arguments.items()
         }
-        return result
-    elif isinstance(arguments, list):
-        result = [
-            attrs_to_snake_case(a)
-            for a in arguments
-        ]
-        return result
-    else:
-        return arguments
+    if isinstance(arguments, list):
+        arguments = [attrs_to_snake_case(a) for a in arguments]
+    return arguments
 
 
 def attrs_to_camel_case(result: ExternalType) -> ExternalType:
     if isinstance(result, dict):
-        result = {
-            attr_camel_case(k): attrs_to_camel_case(v)
-            for k, v in result.items()
-        }
-        return result
-    elif isinstance(result, list):
-        result = [
-            attrs_to_camel_case(a)
-            for a in result
-        ]
-        return result
-    else:
-        return result
+        result = {attr_camel_case(k): attrs_to_camel_case(v) for k, v in result.items()}
+    if isinstance(result, list):
+        result = [attrs_to_camel_case(a) for a in result]
+    return result
```

### Comparing `servey-2.8.3/servey/servey_aws/event_handler/event_handler.py` & `servey-2.8.4/servey/servey_aws/event_handler/event_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from servey.security.authorizer.authorizer_factory_abc import get_default_authorizer
 from servey.servey_aws.event_handler.event_handler_abc import (
     EventHandlerABC,
     EventHandlerFactoryABC,
 )
 
 
+# pylint: disable=R0902
 @dataclass
 class EventHandler(EventHandlerABC):
     action: Action
     param_marshaller: MarshallerABC
     param_schema: Optional[Schema]
     result_marshaller: Optional[MarshallerABC]
     result_schema: Optional[Schema] = None
@@ -44,24 +45,23 @@
                 return False
             event = event[0]
         return "params" in event
 
     def handle(self, event: ExternalType, context) -> ExternalType:
         if isinstance(event, list):
             return self.handle_batch(event)
-        else:
-            return self.handle_event(event)
+        return self.handle_event(event)
 
     def handle_batch(self, events: List[ExternalItemType]) -> List[ExternalType]:
         if not events:
             return []
         kwarg_list = [self.parse_kwargs(e) for e in events]
         arg_extractor = self.action.batch_invoker.arg_extractor
-        key_list = [arg_extractor(a['self'])[0] for a in kwarg_list]
-        authorization = kwarg_list[0]['authorization']
+        key_list = [arg_extractor(a["self"])[0] for a in kwarg_list]
+        authorization = kwarg_list[0]["authorization"]
         results = self.action.batch_invoker.fn(key_list, authorization)
         if isinstance(results, Awaitable):
             loop = asyncio.get_event_loop()
             results = loop.run_until_complete(results)
         results = [self.render_result(result) for result in results]
         return results
```

### Comparing `servey-2.8.3/servey/servey_aws/event_handler/event_handler_abc.py` & `servey-2.8.4/servey/servey_aws/event_handler/event_handler_abc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod, ABC
 from typing import List, Optional
 
 from marshy.factory.impl_marshaller_factory import get_impls
-from marshy.types import ExternalItemType, ExternalType
+from marshy.types import ExternalType
 
 from servey.action.action import Action
 
 
 class EventHandlerABC(ABC):
     priority: int = 100
```

### Comparing `servey-2.8.3/servey/servey_aws/event_handler/sqs_event_handler.py` & `servey-2.8.4/servey/servey_aws/event_handler/sqs_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/lambda_invoker.py` & `servey-2.8.4/servey/servey_aws/lambda_invoker.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from servey.action.action import get_action
 from servey.errors import ServeyError
 from servey.servey_aws.event_handler.event_handler_abc import get_event_handlers
 
 
 def invoke(event: ExternalItemType, context) -> ExternalType:
-    _LOGGER.info(json.dumps(dict(lambda_event=event)))
+    _LOGGER.info(json.dumps({"lambda_event": event}))
     for handler in _EVENT_HANDLERS:
         if handler.is_usable(event, context):
             return handler.handle(event, context)
     raise ServeyError("no_handler")
 
 
 def find_action():
@@ -44,18 +44,18 @@
                 p.replace(annotation=action_class) if p.name == "self" else p
                 for p in sig.parameters.values()
             ]
         )
         wrapper.__signature__ = sig
         action_ = dataclasses.replace(action_, fn=wrapper)
         return action_
-    else:
-        action_function = getattr(action_module, action_function_name)
-        action_ = get_action(action_function)
-        return action_
+
+    action_function = getattr(action_module, action_function_name)
+    action_ = get_action(action_function)
+    return action_
 
 
 _ACTION = find_action()
 _EVENT_HANDLERS = get_event_handlers(_ACTION)
 _LOGGER = logging.getLogger(__name__)
 _LOGGER.setLevel(logging.INFO)
 logging.basicConfig(level=logging.INFO)
```

### Comparing `servey-2.8.3/servey/servey_aws/lambda_router.py` & `servey-2.8.4/servey/servey_aws/lambda_router.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from marshy.types import ExternalItemType, ExternalType
 
 from servey.errors import ServeyError
 from servey.servey_aws.router.router_abc import find_routers
 
 
 def invoke(event: ExternalItemType, context) -> ExternalType:
-    _LOGGER.info(json.dumps(dict(lambda_event=event)))
+    _LOGGER.info(json.dumps({"lambda_event": event}))
     for router in _ROUTERS:
         handler = router.create_handler(event, context)
         if handler:
             return handler.handle(event, context)
     raise ServeyError("no_handler")
```

### Comparing `servey-2.8.3/servey/servey_aws/lambda_websocket.py` & `servey-2.8.4/servey/servey_aws/lambda_websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 logging.basicConfig(level=logging.INFO)
 _DYNAMODB_TABLE = boto3.resource("dynamodb").Table(os.environ["CONNECTION_TABLE_NAME"])
 _SUBSCRIPTIONS = [s for s in find_subscriptions() if s.access_control != ALLOW_NONE]
 _AUTH_MARSHALLER = get_default_context().get_marshaller(Optional[Authorization])
 _AUTHORIZER = get_default_authorizer()
 
 
+# pylint: disable=W0613
 # noinspection PyUnusedLocal
 def lambda_handler(event: ExternalItemType, context) -> ExternalType:
-    _LOGGER.info(json.dumps(dict(lambda_event=event)))
+    _LOGGER.info(json.dumps({"lambda_event": event}))
     request_context = event.get("requestContext") or {}
     route_key = request_context.get("routeKey")
     connection_id = request_context.get("connectionId")
     endpoint_url = f"https://{request_context['domainName']}/{request_context['stage']}"
     status_code = 400
     if route_key == "$connect":
         user_authorization = None
@@ -60,53 +61,53 @@
             _LOGGER.warning(f"error_handling_websocket:{e}")
     response = {"statusCode": status_code}
     return response
 
 
 def connect(connection_id: str, user_authorization: Authorization):
     _DYNAMODB_TABLE.put_item(
-        Item=dict(
-            connection_id=connection_id,
-            subscription_name=" ",
-            user_authorization=_AUTH_MARSHALLER.dump(user_authorization),
-            updated_at=datetime.now().isoformat(),
-        )
+        Item={
+            "connection_id": connection_id,
+            "subscription_name": " ",
+            "user_authorization": _AUTH_MARSHALLER.dump(user_authorization),
+            "updated_at": datetime.now().isoformat(),
+        }
     )
 
 
 def disconnect(connection_id: str):
     keys = []
-    kwargs = dict(
-        Select="SPECIFIC_ATTRIBUTES",
-        ProjectionExpression="connection_id,subscription_name",
-        KeyConditionExpression=Key("connection_id").eq(connection_id),
-    )
+    kwargs = {
+        "Select": "SPECIFIC_ATTRIBUTES",
+        "ProjectionExpression": "connection_id,subscription_name",
+        "KeyConditionExpression": Key("connection_id").eq(connection_id),
+    }
     while True:
         response = _DYNAMODB_TABLE.query(**kwargs)
         keys.extend(response["Items"])
         kwargs["ExclusiveStartKey"] = response.get("LastEvaluatedKey")
         if not kwargs["ExclusiveStartKey"]:
             break
 
     with _DYNAMODB_TABLE.batch_writer() as batch:
         for key in keys:
             batch.delete_item(Key=key)
 
 
 def subscribe(connection_id: str, subscription_name: str, endpoint_url: str):
     item = _DYNAMODB_TABLE.get_item(
-        Key=dict(connection_id=connection_id, subscription_name=" ")
+        Key={"connection_id": connection_id, "subscription_name": " "}
     )
     _DYNAMODB_TABLE.put_item(
-        Item=dict(
-            connection_id=connection_id,
-            subscription_name=subscription_name,
-            endpoint_url=endpoint_url,
-            user_authorization=item.get("user_authorization"),
-            updated_at=datetime.now().isoformat(),
-        )
+        Item={
+            "connection_id": connection_id,
+            "subscription_name": subscription_name,
+            "endpoint_url": endpoint_url,
+            "user_authorization": item.get("user_authorization"),
+            "updated_at": datetime.now().isoformat(),
+        }
     )
 
 
 def unsubscribe(connection_id: str, subscription_name: str):
-    key = dict(connection_id=connection_id, subscription_name=subscription_name)
+    key = {"connection_id": connection_id, "subscription_name": subscription_name}
     _DYNAMODB_TABLE.delete_item(Key=key)
```

### Comparing `servey-2.8.3/servey/servey_aws/router/api_gateway_router.py` & `servey-2.8.4/servey/servey_aws/router/api_gateway_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/router/appsync_router.py` & `servey-2.8.4/servey/servey_aws/router/appsync_router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import inspect
 from typing import Optional
 
 from marshy.factory.optional_marshaller_factory import get_optional_type
-from marshy.types import ExternalItemType, ExternalType
+from marshy.types import ExternalType
 
 from servey.action.action import Action, get_action
 from servey.errors import ServeyError
 from servey.servey_aws.event_handler.event_handler_abc import (
     get_event_handlers,
     EventHandlerABC,
 )
@@ -21,48 +21,51 @@
     def create_handler(self, event: ExternalType, context) -> EventHandlerABC:
         if isinstance(event, list):
             event = event[0]
         info = event.get("info", None)  # Diff appsync events
         if info is None:
             return
         field_name = info["fieldName"]
-        source = event.get('source')
+        source = event.get("source")
         if source:
-            action = self.find_action_for_parent_type(info['parentTypeName'], field_name)
+            action = self.find_action_for_parent_type(
+                info["parentTypeName"], field_name
+            )
         else:
             action = self.find_action_for_field_name(field_name)
         if action is None:
             raise ServeyError(f"unknown_field_name:{field_name}")
         handlers = get_event_handlers(action)
         for handler in handlers:
             if handler.is_usable(event, context):
                 return handler
 
     def find_action_for_parent_type(self, parent_type_name: str, field_name: str):
         field_name = to_snake_case(field_name)
-        for action, trigger in self.web_trigger_actions:
+        for action, _ in self.web_trigger_actions:
             sig = inspect.signature(action.fn)
             parent_type = sig.return_annotation
             parent_type = get_optional_type(parent_type) or parent_type
-            if getattr(parent_type, '__name__', None) == parent_type_name:
+            if getattr(parent_type, "__name__", None) == parent_type_name:
                 fn = getattr(parent_type, field_name)
                 nested_action = get_action(fn)
                 sig = inspect.signature(fn)
                 parameters = list(sig.parameters.values())
                 parameters[0] = parameters[0].replace(annotation=parent_type)
                 sig = sig.replace(parameters=parameters)
 
+                # pylint: disable=W0640
                 def wrapper(*args, **kwargs):
                     return fn(*args, **kwargs)
 
                 wrapper.__signature__ = sig
                 nested_action = dataclasses.replace(nested_action, fn=wrapper)
                 wrapper.__servey_action__ = nested_action
                 return nested_action
 
     def find_action_for_field_name(self, field_name: str) -> Optional[Action]:
-        for action, trigger in self.web_trigger_actions:
+        for action, _ in self.web_trigger_actions:
             action_field_name = action.name[0] + action.name.title()[1:].replace(
                 "_", ""
             )
             if action_field_name == field_name:
                 return action
```

### Comparing `servey-2.8.3/servey/servey_aws/router/router.py` & `servey-2.8.4/servey/servey_aws/router/router.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from marshy.types import ExternalItemType, ExternalType
+from marshy.types import ExternalType
 
 from servey.finder.action_finder_abc import find_actions
 from servey.servey_aws.event_handler.event_handler_abc import (
     get_event_handlers,
     EventHandlerABC,
 )
 from servey.servey_aws.router.router_abc import RouterABC
```

### Comparing `servey-2.8.3/servey/servey_aws/router/router_abc.py` & `servey-2.8.4/servey/servey_aws/router/router_abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
 from marshy.factory.impl_marshaller_factory import get_impls
-from marshy.types import ExternalItemType, ExternalType
+from marshy.types import ExternalType
 
 from servey.action.action import Action
 from servey.finder.action_finder_abc import find_actions_with_trigger_type
 from servey.servey_aws.event_handler.event_handler_abc import EventHandlerABC
 from servey.trigger.web_trigger import WebTrigger
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/__main__.py` & `servey-2.8.4/servey/servey_aws/serverless/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py` & `servey-2.8.4/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,9 +27,9 @@
             raise ServeyError("frequency_too_high")  # min is 60!
         for unit, seconds in UNITS.items():
             if not trigger.interval % seconds:
                 rate = int(trigger.interval / seconds)
                 if rate == 1:
                     unit = unit[:-1]  # remove plural
                 # noinspection PyTypeChecker
-                events.append(dict(schedule=dict(rate=f"rate({rate} {unit})")))
+                events.append({"schedule": {"rate": f"rate({rate} {unit})"}})
                 return
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py` & `servey-2.8.4/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,10 +26,9 @@
         events = lambda_definition.get("events")
         if not events:
             events = lambda_definition["events"] = []
         path = trigger.path or self.path_pattern.format(
             action_name=action.name.replace("_", "-")
         )
         events.append(
-            dict(http=dict(path=path, method=trigger.method.value, cors=True))
-            # TODO: Add openapi documentation
+            {"http": {"path": path, "method": trigger.method.value, "cors": True}}
         )
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/action_function_config.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/action_function_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,33 +44,33 @@
         connection_table_name = get_servey_main() + "_connection"
         for action in find_actions():
             use_router = self.use_router_for_all or "<locals>" in action.fn.__qualname__
             if use_router:
                 lambda_name = self.router_name
                 lambda_definition = lambda_definitions.get(lambda_name)
                 if not lambda_definition:
-                    lambda_definition = lambda_definitions[lambda_name] = dict(
-                        handler="servey.servey_aws.lambda_router.invoke",
-                        timeout=30,
-                    )
+                    lambda_definition = lambda_definitions[lambda_name] = {
+                        "handler": "servey.servey_aws.lambda_router.invoke",
+                        "timeout": 30,
+                    }
             else:
                 # noinspection PyUnresolvedReferences
                 lambda_definition = lambda_definitions[action.name] = filter_none(
-                    dict(
-                        handler="servey.servey_aws.lambda_invoker.invoke",
-                        description=action.description.strip()
+                    {
+                        "handler": "servey.servey_aws.lambda_invoker.invoke",
+                        "description": action.description.strip()
                         if action.description
                         else None,
-                        timeout=action.timeout,
-                        environment=dict(
-                            SERVEY_ACTION_MODULE=action.fn.__module__,
-                            SERVEY_ACTION_FUNCTION_NAME=action.fn.__qualname__,
-                            CONNECTION_TABLE_NAME=connection_table_name,
-                        ),
-                    )
+                        "timeout": action.timeout,
+                        "environment": {
+                            "SERVEY_ACTION_MODULE": action.fn.__module__,
+                            "SERVEY_ACTION_FUNCTION_NAME": action.fn.__qualname__,
+                            "CONNECTION_TABLE_NAME": connection_table_name,
+                        },
+                    }
                 )
             for trigger in action.triggers:
                 for handler in trigger_handlers:
                     handler.handle_trigger(action, trigger, lambda_definition)
         for subscription in find_subscriptions():
             for action in subscription.action_subscribers:
                 if action.name in lambda_definitions:
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/appsync_config.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/appsync_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,48 +70,48 @@
 
     def build_servey_action_functions_yml(self) -> ExternalItemType:
         appsync_definitions = {
             "name": get_servey_main(),
             "authentication": {
                 "type": "API_KEY",
             },
-            "apiKeys": [{
-                "name": f"{get_servey_main()}Key",
-            }],
+            "apiKeys": [
+                {
+                    "name": f"{get_servey_main()}Key",
+                }
+            ],
             "resolvers": {},
             "dataSources": {},
             "schema": self.servey_appsync_schema_file,
-            # caching:
-            #    behavior: FULL_REQUEST_CACHING  # or PER_RESOLVER_CACHING. Required
-            #    ttl: 3600  # The TTL of the cache. Optional. Default: 3600
-            #    atRestEncryption:  # Bool, Optional. Enable at rest encryption. disabled by default.
-            #    transitEncryption:  # Bool, Optional. Enable transit encryption. disabled by default.
-            #    type: 'T2_SMALL'  # Cache instance size. Optional. Default: 'T2_SMALL'
         }
         processed_dataclasses = set()
         for action, trigger in find_actions_with_trigger_type(WebTrigger):
             resolver_type = (
                 "Query" if trigger.method == WebTriggerMethod.GET else "Mutation"
             )
             resolver_name = resolver_type + "." + attr_camel_case(action.name)
             self.add_field(action, appsync_definitions, resolver_name)
-            self.build_nested_resolvers(action, appsync_definitions, processed_dataclasses)
+            self.build_nested_resolvers(
+                action, appsync_definitions, processed_dataclasses
+            )
 
         return appsync_definitions
 
-    def add_field(self, action: Action, appsync_definitions: ExternalItemType, resolver_name: str):
+    def add_field(
+        self, action: Action, appsync_definitions: ExternalItemType, resolver_name: str
+    ):
         # data source may be
         use_router = self.use_router_for_all or "<locals>" in action.fn.__qualname__
         data_source_name = "servey_router" if use_router else action.name
         resolver = {
             "kind": "UNIT",
             "dataSource": data_source_name,
         }
         if action.batch_invoker:
-            resolver['maxBatchSize'] = action.batch_invoker.max_batch_size
+            resolver["maxBatchSize"] = action.batch_invoker.max_batch_size
         appsync_definitions["resolvers"][resolver_name] = resolver
         data_source = {
             "type": "AWS_LAMBDA",
             "config": {
                 "functionName": data_source_name,
             },
         }
@@ -119,22 +119,24 @@
             data_source["description"] = action.description.strip()
         appsync_definitions["dataSources"][data_source_name] = data_source
 
     def build_nested_resolvers(
         self,
         action: Action,
         appsync_definitions: ExternalItemType,
-        processed_dataclasses: Set[Type]
+        processed_dataclasses: Set[Type],
     ):
         sig = inspect.signature(action.fn)
         type_ = sig.return_annotation
         type_ = get_optional_type(type_) or type_
         if not dataclasses.is_dataclass(type_) or type_ in processed_dataclasses:
             return
         processed_dataclasses.add(type_)
         members = inspect.getmembers(type_)
         for name, member in members:
             nested_action = get_action(member)
             if nested_action:
-                resolver_name = type_.__name__ + '.' + attr_camel_case(name)
+                resolver_name = type_.__name__ + "." + attr_camel_case(name)
                 self.add_field(nested_action, appsync_definitions, resolver_name)
-                self.build_nested_resolvers(nested_action, appsync_definitions, processed_dataclasses)
+                self.build_nested_resolvers(
+                    nested_action, appsync_definitions, processed_dataclasses
+                )
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/cloudfront_config.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/cloudfront_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,32 @@
 )
 
 
 class CloudfrontConfig(YmlConfigABC):
     """
     Set up some aspect of the serverless environment yml files. (For example, functions, resources, etc...)
     """
-    static_site_directory: Path = Path(os.environ.get("SERVEY_STATIC_SITE_DIR") or "static_site")
-    static_site_bucket_resource_yml_file: str = "serverless_servey/cloudfront_resource.yml"
+
+    static_site_directory: Path = Path(
+        os.environ.get("SERVEY_STATIC_SITE_DIR") or "static_site"
+    )
+    static_site_bucket_resource_yml_file: str = (
+        "serverless_servey/cloudfront_resource.yml"
+    )
 
     def configure(self, main_serverless_yml_file: str):
         has_static_site = self.static_site_directory.exists()
         has_web_page = False
         try:
             # noinspection PyUnresolvedReferences
             from servey.servey_web_page.web_page_trigger import WebPageTrigger
-            has_web_page = next((True for _ in find_actions_with_trigger_type(WebPageTrigger)), False)
+
+            has_web_page = next(
+                (True for _ in find_actions_with_trigger_type(WebPageTrigger)), False
+            )
         except ImportError:
             pass
         if not has_static_site and not has_web_page:
             return
         # If there is a static site
         ensure_ref_in_file(
             main_serverless_yml_file,
@@ -47,128 +55,117 @@
                 "End2EndIndexFn": {
                     "Type": "AWS::CloudFront::Function",
                     "Properties": {
                         "Name": "End2EndIndexFn",
                         "AutoPublish": True,
                         "FunctionConfig": {
                             "Comment": "Add index.html when path ends with /",
-                            "Runtime": "cloudfront-js-1.0"
+                            "Runtime": "cloudfront-js-1.0",
                         },
-                        "FunctionCode": "\n".join((
-                            "function handler(event) {",
-                            "    var request = event.request;",
-                            "    var uri = request.uri;",
-                            "",
-                            "    if (uri.endsWith('/')) {",
-                            "        request.uri += 'index.html';",
-                            "    }",
-                            "    else if (!uri.includes('.')) {",
-                            "        request.uri += '/index.html';",
-                            "    }",
-                            "",
-                            "    return request;",
-                            "}",
-                            ""
-                        ))
-                    }
+                        "FunctionCode": "\n".join(
+                            (
+                                "function handler(event) {",
+                                "    var request = event.request;",
+                                "    var uri = request.uri;",
+                                "",
+                                "    if (uri.endsWith('/')) {",
+                                "        request.uri += 'index.html';",
+                                "    }",
+                                "    else if (!uri.includes('.')) {",
+                                "        request.uri += '/index.html';",
+                                "    }",
+                                "",
+                                "    return request;",
+                                "}",
+                                "",
+                            )
+                        ),
+                    },
                 },
                 "End2EndDistribution": {
                     "Type": "AWS::CloudFront::Distribution",
                     "Properties": {
                         "DistributionConfig": {
                             "Enabled": "true",
                             "DefaultRootObject": "/",
                             "DefaultCacheBehavior": {
-                                "AllowedMethods": [
-                                    "GET",
-                                    "HEAD"
-                                ],
+                                "AllowedMethods": ["GET", "HEAD"],
                                 "MinTTL": "0",
                                 "MaxTTL": "0",
                                 "DefaultTTL": "0",
                                 "TargetOriginId": "s3Origin",
-                                "ForwardedValues": {
-                                    "QueryString": "false"
-                                },
+                                "ForwardedValues": {"QueryString": "false"},
                                 "ViewerProtocolPolicy": "redirect-to-https",
                                 "FunctionAssociations": [
                                     {
                                         "EventType": "viewer-request",
-                                        "FunctionARN": {
-                                            "Ref": "End2EndIndexFn"
-                                        }
+                                        "FunctionARN": {"Ref": "End2EndIndexFn"},
                                     }
-                                ]
+                                ],
                             },
                             "CacheBehaviors": [
                                 {
                                     "AllowedMethods": [
                                         "HEAD",
                                         "DELETE",
                                         "POST",
                                         "GET",
                                         "OPTIONS",
                                         "PUT",
-                                        "PATCH"
+                                        "PATCH",
                                     ],
                                     "TargetOriginId": "apiGatewayAPIOrigin",
                                     "ForwardedValues": {
                                         "QueryString": True,
-                                        "Cookies": {
-                                            "Forward": "all"
-                                        }
+                                        "Cookies": {"Forward": "all"},
                                     },
                                     "ViewerProtocolPolicy": "https-only",
                                     "MinTTL": "0",
                                     "MaxTTL": "6",
                                     "DefaultTTL": "3",
-                                    "PathPattern": "actions/*"
+                                    "PathPattern": "actions/*",
                                 },
                                 {
                                     "AllowedMethods": [
                                         "HEAD",
                                         "DELETE",
                                         "POST",
                                         "GET",
                                         "OPTIONS",
                                         "PUT",
-                                        "PATCH"
+                                        "PATCH",
                                     ],
                                     "TargetOriginId": "appsyncAPIOrigin",
                                     "ForwardedValues": {
                                         "QueryString": False,
-                                        "Cookies": {
-                                            "Forward": "all"
-                                        }
+                                        "Cookies": {"Forward": "all"},
                                     },
                                     "ViewerProtocolPolicy": "https-only",
                                     "MinTTL": "0",
                                     "MaxTTL": "6",
                                     "DefaultTTL": "3",
-                                    "PathPattern": "graphql"
-                                }
+                                    "PathPattern": "graphql",
+                                },
                             ],
                             "Origins": [
                                 {
                                     "DomainName": {
                                         "Fn::Join": [
                                             "",
                                             [
-                                                {
-                                                    "Ref": "ApiGatewayRestApi"
-                                                },
-                                                ".execute-api.${self:provider.region}.amazonaws.com"
-                                            ]
+                                                {"Ref": "ApiGatewayRestApi"},
+                                                ".execute-api.${self:provider.region}.amazonaws.com",
+                                            ],
                                         ]
                                     },
                                     "Id": "apiGatewayAPIOrigin",
                                     "OriginPath": "/${self:provider.stage}",
                                     "CustomOriginConfig": {
                                         "OriginProtocolPolicy": "https-only"
-                                    }
+                                    },
                                 },
                                 {
                                     "DomainName": {
                                         "Fn::Select": [
                                             0,
                                             {
                                                 "Fn::Split": [
@@ -178,47 +175,45 @@
                                                             1,
                                                             {
                                                                 "Fn::Split": [
                                                                     "https://",
                                                                     {
                                                                         "Fn::GetAtt": [
                                                                             "GraphQlApi",
-                                                                            "GraphQLUrl"
+                                                                            "GraphQLUrl",
                                                                         ]
-                                                                    }
+                                                                    },
                                                                 ]
-                                                            }
+                                                            },
                                                         ]
-                                                    }
+                                                    },
                                                 ]
-                                            }
+                                            },
                                         ]
                                     },
                                     "Id": "appsyncAPIOrigin",
                                     "CustomOriginConfig": {
                                         "OriginProtocolPolicy": "https-only"
-                                    }
+                                    },
                                 },
                                 {
                                     "DomainName": "${self:custom.staticBucket}.s3.amazonaws.com",
                                     "Id": "s3Origin",
                                     "S3OriginConfig": {
                                         "OriginAccessIdentity": {
                                             "Fn::Join": [
                                                 "",
                                                 [
                                                     "origin-access-identity/cloudfront/",
-                                                    {
-                                                        "Ref": "OriginAccessIdentity"
-                                                    }
-                                                ]
+                                                    {"Ref": "OriginAccessIdentity"},
+                                                ],
                                             ]
                                         }
-                                    }
-                                }
-                            ]
+                                    },
+                                },
+                            ],
                         }
-                    }
-                }
+                    },
+                },
             }
         }
         return static_site_bucket_resource
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/kms_key_config.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/kms_key_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/serverless_template.yml` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/serverless_template.yml`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 import os
+from dataclasses import dataclass
 from pathlib import Path
 from random import randint
 
 from marshy.types import ExternalItemType
 from ruamel.yaml import YAML
 
 from servey.servey_aws.serverless.yml_config.yml_config_abc import (
     YmlConfigABC,
     ensure_ref_in_file,
     create_yml_file,
 )
 
-ALPHABET = '0123456789abcdefghijklmnopqrstuvwxyz'
+ALPHABET = "0123456789abcdefghijklmnopqrstuvwxyz"
 
 
+@dataclass
 class StaticSiteBucketConfig(YmlConfigABC):
     """
     Set up some aspect of the serverless environment yml files. (For example, functions, resources, etc...)
     """
-    static_site_directory: Path = Path(os.environ.get("SERVEY_STATIC_SITE_DIR") or "static_site")
-    static_site_bucket_resource_yml_file: str = "serverless_servey/static_site_bucket_resource.yml"
+
+    static_site_directory: Path = Path(
+        os.environ.get("SERVEY_STATIC_SITE_DIR") or "static_site"
+    )
+    static_site_bucket_resource_yml_file: str = (
+        "serverless_servey/static_site_bucket_resource.yml"
+    )
 
     def configure(self, main_serverless_yml_file: str):
         if not self.static_site_directory.exists():
             return
         # If there is a static site
         ensure_ref_in_file(
             main_serverless_yml_file,
@@ -36,91 +43,83 @@
             self.static_site_bucket_resource_yml_file, static_site_bucket_resource_yml
         )
 
     def add_custom_bucket_yml(self, main_serverless_yml_file: str):
         yaml = YAML()
         with open(main_serverless_yml_file, "r") as reader:
             root = yaml.load(reader)
-            custom = root.get('custom')
-            static_bucket = custom.get('staticBucket')
+            custom = root.get("custom")
+            static_bucket = custom.get("staticBucket")
             if static_bucket:
                 return static_bucket
-        static_bucket = 'b' + ''.join(ALPHABET[randint(0, 35)] for _ in range(10))
-        custom['staticBucket'] = static_bucket
-        custom['s3Sync'] = [{
-            'bucketName': '${self: custom.staticBucket}',
-            'localDir': self.static_site_directory
-        }]
-        root['plugins'].append('serverless-s3-sync')
+        static_bucket = "b" + "".join(ALPHABET[randint(0, 35)] for _ in range(10))
+        custom["staticBucket"] = static_bucket
+        custom["s3Sync"] = [
+            {
+                "bucketName": "${self: custom.staticBucket}",
+                "localDir": str(self.static_site_directory),
+            }
+        ]
+        root["plugins"].append("serverless-s3-sync")
         with open(main_serverless_yml_file, "w") as writer:
             yaml.dump(root, writer)
         return static_bucket
 
     @staticmethod
     def build_static_site_bucket_resource_yml() -> ExternalItemType:
         static_site_bucket_resource = {
             "Resources": {
                 "OriginAccessIdentity": {
                     "Type": "AWS::CloudFront::CloudFrontOriginAccessIdentity",
                     "Properties": {
                         "CloudFrontOriginAccessIdentityConfig": {
                             "Comment": "Allow cloudfront to access the static bucket"
                         }
-                    }
+                    },
                 },
                 "StaticBucket": {
                     "Type": "AWS::S3::Bucket",
                     "Properties": {
                         "AccessControl": "Private",
                         "BucketName": "${self:custom.staticBucket}",
-                        "WebsiteConfiguration": {
-                            "IndexDocument": "index.html"
-                        }
-                    }
+                        "WebsiteConfiguration": {"IndexDocument": "index.html"},
+                    },
                 },
                 "StaticSiteS3BucketPolicy": {
                     "Type": "AWS::S3::BucketPolicy",
                     "Properties": {
-                        "Bucket": {
-                            "Ref": "StaticBucket"
-                        },
+                        "Bucket": {"Ref": "StaticBucket"},
                         "PolicyDocument": {
                             "Statement": [
                                 {
                                     "Sid": "AllowCloudFrontServicePrincipalReadOnly",
                                     "Effect": "Allow",
                                     "Principal": {
                                         "AWS": {
                                             "Fn::Join": [
                                                 "",
                                                 [
                                                     "arn:aws:iam::cloudfront:user/CloudFront Origin Access Identity ",
-                                                    {
-                                                        "Ref": "OriginAccessIdentity"
-                                                    }
-                                                ]
+                                                    {"Ref": "OriginAccessIdentity"},
+                                                ],
                                             ]
                                         }
                                     },
-                                    "Action": [
-                                        "s3:GetObject"
-                                    ],
+                                    "Action": ["s3:GetObject"],
                                     "Resource": {
                                         "Fn::Join": [
                                             "",
                                             [
                                                 "arn:aws:s3:::",
-                                                {
-                                                    "Ref": "StaticBucket"
-                                                },
-                                                "/*"
-                                            ]
+                                                {"Ref": "StaticBucket"},
+                                                "/*",
+                                            ],
                                         ]
-                                    }
+                                    },
                                 }
                             ]
-                        }
-                    }
-                }
+                        },
+                    },
+                },
             }
         }
         return static_site_bucket_resource
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/subscription_function_config.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/subscription_function_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,59 +133,63 @@
             }
         resource_definitions = {"Resources": resources}
         return resource_definitions
 
     def build_role_statement_yml(self) -> ExternalItemType:
         role_statements = []
         if self.has_websocket_subscriptions:
-            role_statements.append({
-                "Effect": "Allow",
-                "Action": [
-                    "dynamodb:BatchWriteItem",
-                    "dynamodb:DeleteItem",
-                    "dynamodb:GetItem",
-                    "dynamodb:PutItem",
-                    "dynamodb:Query",
-                ],
-                "Resource": [
-                    {
-                        "Fn::GetAtt": [
-                            self.connection_table_name.title().replace("_", ""),
-                            "Arn",
-                        ]
-                    },
-                    {
-                        "Fn::Join": [
-                            "/",
-                            [
-                                {
-                                    "Fn::GetAtt": [
-                                        self.connection_table_name.title().replace(
-                                            "_", ""
-                                        ),
-                                        "Arn",
-                                    ]
-                                },
-                                "index",
-                                "gsi__subscription_name__connection_id",
-                            ],
-                        ]
-                    },
-                ],
-            })
+            role_statements.append(
+                {
+                    "Effect": "Allow",
+                    "Action": [
+                        "dynamodb:BatchWriteItem",
+                        "dynamodb:DeleteItem",
+                        "dynamodb:GetItem",
+                        "dynamodb:PutItem",
+                        "dynamodb:Query",
+                    ],
+                    "Resource": [
+                        {
+                            "Fn::GetAtt": [
+                                self.connection_table_name.title().replace("_", ""),
+                                "Arn",
+                            ]
+                        },
+                        {
+                            "Fn::Join": [
+                                "/",
+                                [
+                                    {
+                                        "Fn::GetAtt": [
+                                            self.connection_table_name.title().replace(
+                                                "_", ""
+                                            ),
+                                            "Arn",
+                                        ]
+                                    },
+                                    "index",
+                                    "gsi__subscription_name__connection_id",
+                                ],
+                            ]
+                        },
+                    ],
+                }
+            )
         if next((True for s in self.subscriptions if s.action_subscribers), False):
-            role_statements.append({
-                "Effect": "Allow",
-                "Action": [
-                    "sqs:SendMessage",
-                    "sqs:ReceiveMessage",
-                    "sqs:DeleteMessage",
-                    "sqs:GetQueueUrl",
-                ],
-                "Resource": [
-                    {"Fn::GetAtt": [s.name.title().replace("_", "") + "SQS", "Arn"]}
-                    for s in self.subscriptions
-                    if s.action_subscribers
-                ],
-            })
+            role_statements.append(
+                {
+                    "Effect": "Allow",
+                    "Action": [
+                        "sqs:SendMessage",
+                        "sqs:ReceiveMessage",
+                        "sqs:DeleteMessage",
+                        "sqs:GetQueueUrl",
+                    ],
+                    "Resource": [
+                        {"Fn::GetAtt": [s.name.title().replace("_", "") + "SQS", "Arn"]}
+                        for s in self.subscriptions
+                        if s.action_subscribers
+                    ],
+                }
+            )
         subscription_policy = {"iamRoleStatements": role_statements}
         return subscription_policy
```

### Comparing `servey-2.8.3/servey/servey_aws/serverless/yml_config/yml_config_abc.py` & `servey-2.8.4/servey/servey_aws/serverless/yml_config/yml_config_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/sqs_subscription_service.py` & `servey-2.8.4/servey/servey_aws/sqs_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_aws/websocket_subscription_service.py` & `servey-2.8.4/servey/servey_aws/websocket_subscription_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,20 @@
         if not api:
             api = boto3.client("apigatewaymanagementapi", endpoint_url=endpoint_url)
             self.apis_by_endpoint_url[endpoint_url] = api
         return api
 
     def publish(self, subscription: Subscription[T], event: T):
         data = json.dumps(subscription.event_marshaller.dump(event)).encode("utf-8")
-        kwargs = dict(
-            Select="SPECIFIC_ATTRIBUTES",
-            ProjectionExpression="connection_id,endpoint_url,user_authorization",
-            IndexName="gsi__subscription_name__connection_id",
-            KeyConditionExpression=Key("subscription_name").eq(subscription.name),
-        )
+        kwargs = {
+            "Select": "SPECIFIC_ATTRIBUTES",
+            "ProjectionExpression": "connection_id,endpoint_url,user_authorization",
+            "IndexName": "gsi__subscription_name__connection_id",
+            "KeyConditionExpression": Key("subscription_name").eq(subscription.name),
+        }
         while True:
             response = self.connection_table.query(**kwargs)
             items = response.get("Items") or []
             for item in items:
                 api = self.get_api_for_endpoint(item["endpoint_url"])
                 if subscription.event_filter:
                     user_authorization = item.get("user_authorization")
```

### Comparing `servey-2.8.3/servey/servey_celery/celery_app.py` & `servey-2.8.4/servey/servey_celery/celery_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_celery/celery_config/fixed_rate_trigger_config.py` & `servey-2.8.4/servey/servey_celery/celery_config/fixed_rate_trigger_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,13 +14,14 @@
             if _action.name not in global_ns:
                 global_ns[_action.name] = app.task(_action.fn)
                 has_triggers = True
 
         if not has_triggers:
             return
 
+        # pylint: disable=W0613
         # noinspection PyUnusedLocal
         @app.on_after_configure.connect
         def setup_periodic_tasks(sender, **kwargs):
             for action, trigger in find_actions_with_trigger_type(FixedRateTrigger):
                 task = global_ns[action.name]
                 sender.add_periodic_task(trigger.interval, task.s())
```

### Comparing `servey-2.8.3/servey/servey_celery/celery_config/subscription_config.py` & `servey-2.8.4/servey/servey_celery/celery_config/subscription_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_celery/celery_subscription_service.py` & `servey-2.8.4/servey/servey_celery/celery_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_direct/__main__.py` & `servey-2.8.4/servey/servey_direct/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,9 @@
     return_annotation = inspect.signature(action.fn).return_annotation
     if return_annotation != inspect.Parameter.empty:
         result = get_default_context().dump(result, return_annotation)
         result_str = json.dumps(result)
         print(result_str)
 
 
+# pylint: disable=W0106
 main() if __name__ == "__main__" else 0  # Weird syntax for coverage
```

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/action_endpoint.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     ActionEndpointABC,
 )
 from servey.trigger.web_trigger import WebTriggerMethod, BODY_METHODS
 
 LOGGER = logging.getLogger(__name__)
 
 
+# pylint: disable=R0902
 @dataclass
 class ActionEndpoint(ActionEndpointABC):
     """
     Wrapper for a function for use within starlette, with everything needed to bind it to a route
     """
 
     action: Action
@@ -86,17 +87,17 @@
                     query_str = query_str.decode("latin-1")
                 json_obj = query_str_to_json_obj(query_str)
                 if request.path_params:
                     json_obj.update(request.path_params)
                 json_obj = _fix_strings(json_obj, self.params_schema.schema)
                 self.params_schema.validate(json_obj)
                 kwargs = self.params_marshaller.load(json_obj)
-            except Exception:
+            except Exception as exc:
                 LOGGER.exception("invalid_input")
-                raise HTTPException(422, "invalid_input")
+                raise HTTPException(422, "invalid_input") from exc
         return kwargs
 
     def render_response(self, result: Any):
         result_content = self.result_marshaller.dump(result)
         if self.result_schema:
             error = next(self.result_schema.iter_errors(result_content), None)
             if error:
@@ -158,15 +159,15 @@
         content = {"schema": schema}
         path_method["requestBody"] = {
             "content": {"application/json": content},
             "required": True,
         }
         if self.action.examples:
             content["examples"] = {
-                e.name: filter_none(dict(summary=e.description, value=e.params))
+                e.name: filter_none({"summary": e.description, "value": e.params})
                 for e in self.action.examples
                 if e.include_in_schema
             }
         responses: ExternalItemType = path_method["responses"]
         responses["422"] = {"description": "Validation Error"}
 
     def query_string_request_to_openapi_schema(self, path_method: ExternalItemType):
@@ -190,15 +191,15 @@
         self, responses: ExternalItemType, components: ExternalItemType
     ):
         schema = self.result_schema.schema
         schema = move_ref_items_to_components(schema, schema, components)
         content = {"schema": schema}
         if self.action.examples:
             content["examples"] = {
-                e.name: filter_none(dict(summary=e.description, value=e.result))
+                e.name: filter_none({"summary": e.description, "value": e.result})
                 for e in self.action.examples
                 if e.include_in_schema
             }
         responses["200"] = {
             "description": "Successful Response",
             "content": {"application/json": content},
         }
@@ -228,15 +229,15 @@
             for example in examples:
                 example_value = example.params
                 for p in path:
                     example_value = example_value.get(p, None)
                     if example_value is None:
                         break
                 if example_value is not None:
-                    example_schema = dict(value=example_value)
+                    example_schema = {"value": example_value}
                     if example.description:
                         example_schema["summary"] = example.description
                     example_schemas[example.name] = example_schema
 
             result = {
                 "required": key in required_properties,
                 "schema": property_schema,
@@ -287,29 +288,29 @@
 
 def _fix_strings(param: ExternalType, schema: ExternalItemType):
     """
     Json urley may have parsed items as strings that should not be
     """
     any_of = schema.get("anyOf")
     if any_of:
-        items = [a for a in any_of if a != dict(type="null")]
+        items = [a for a in any_of if a != {"type": "null"}]
         if len(items) == 1:
             schema = items[0]
     if isinstance(param, dict):
         properties_schema: Dict = schema.get("properties")
         if properties_schema:
             result = {}
             for k, v in param.items():
                 s = properties_schema.get(k)
                 if s:
                     v = _fix_strings(v, s)
                 result[k] = v
             param = result
         return param
-    elif isinstance(param, list):
+    if isinstance(param, list):
         item_schema = schema.get("items")
         if item_schema:
             param = [_fix_strings(i, item_schema) for i in param]
         return param
     if schema.get("type") == "string":
         return str(param)
     return param
```

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/action_endpoint_abc.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/action_endpoint_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         )
 
     async def execute_with_context(
         self, request: Request, context: Dict[str, Any]
     ) -> Response:
         authorization = parse_authorization(self.authorizer, request)
         if not self.get_action().access_control.is_executable(authorization):
-            return JSONResponse(dict(error="unauthorized"), 401)
+            return JSONResponse({"error": "unauthorized"}, 401)
         if self.auth_kwarg_name:
             context[self.auth_kwarg_name] = authorization
         response = await self.action_endpoint.execute_with_context(request, context)
         return response
 
     def to_openapi_schema(self, schema: ExternalItemType):
         self.action_endpoint.to_openapi_schema(schema)
@@ -75,15 +75,15 @@
             if not path_method.get("security"):
                 path_method["security"] = [{"OAuth2PasswordBearer": []}]
             responses: Dict = path_method["responses"]
             responses["403"] = {
                 "description": "unauthorized",
                 "content": {
                     "application/json": {
-                        "schema": {"$ref": f"#components/ErrorResponse"}
+                        "schema": {"$ref": "#components/ErrorResponse"}
                     }
                 },
             }
 
 
 def parse_authorization(
     authorizer: AuthorizerABC, request: Request
```

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/caching_action_endpoint.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/caching_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py` & `servey-2.8.4/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/route_factory/action_route_factory.py` & `servey-2.8.4/servey/servey_starlette/route_factory/action_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/route_factory/asyncapi_route_factory.py` & `servey-2.8.4/servey/servey_starlette/route_factory/asyncapi_route_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     def create_routes(self) -> Iterator[Route]:
         if self.get_subscribable():
             yield Route(
                 "/asyncapi.json", endpoint=self.endpoint, include_in_schema=False
             )
         # There is no "async-docs" endpoint - maybe there should be?
 
+    # pylint: disable=W0613
     # noinspection PyUnusedLocal
     def endpoint(self, request: Request) -> Response:
         schema = self.asyncapi_schema()
         return JSONResponse(schema)
 
     def asyncapi_schema(self) -> ExternalItemType:
         components = {}
```

### Comparing `servey-2.8.3/servey/servey_starlette/route_factory/authenticator_route_factory.py` & `servey-2.8.4/servey/servey_starlette/route_factory/authenticator_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/route_factory/openapi_route_factory.py` & `servey-2.8.4/servey/servey_starlette/route_factory/openapi_route_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         yield Route("/openapi.json", endpoint=self.endpoint, include_in_schema=False)
         yield Mount(
             "/docs",
             app=StaticFiles(packages=["servey.servey_starlette"], html=True),
             name="docs",
         )
 
+    # pylint: disable=W0613
     # noinspection PyUnusedLocal
     def endpoint(self, request: Request) -> Response:
         schema = self.openapi_schema()
         return JSONResponse(schema)
 
     def openapi_schema(self) -> ExternalItemType:
         schema = {
```

### Comparing `servey-2.8.3/servey/servey_starlette/route_factory/static_site_route_factory.py` & `servey-2.8.4/servey/servey_starlette/route_factory/static_site_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/route_factory/subscription_route_factory.py` & `servey-2.8.4/servey/servey_starlette/route_factory/subscription_route_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
     connections: List[_Connection] = field(default_factory=list)
 
 
 _SUBSCRIPTION_CONNECTIONS_BY_NAME: Optional[Dict[str, _SubscriptionConnections]] = None
 _CONNECTIONS_BY_ID: Dict[str, _Connection] = {}
 
 
+# pylint: disable=W0603
 def _get_subscription_connections_by_name() -> Dict[str, _SubscriptionConnections]:
     global _SUBSCRIPTION_CONNECTIONS_BY_NAME
     if _SUBSCRIPTION_CONNECTIONS_BY_NAME is None:
         _SUBSCRIPTION_CONNECTIONS_BY_NAME = {
             s.name: _SubscriptionConnections(s)
             for s in find_subscriptions()
             if s.access_control != ALLOW_NONE
@@ -132,14 +133,15 @@
 
 
 def _get_connections_by_id() -> Dict[str, _Connection]:
     return _CONNECTIONS_BY_ID
 
 
 class _StarletteSubscriptionService(SubscriptionServiceABC):
+    # pylint: disable=W0718
     def publish(self, subscription: Subscription[T], event: T):
         subscription_connections = _get_subscription_connections_by_name().get(
             subscription.name
         )
         if not subscription_connections:
             return
         loop = asyncio.get_event_loop()
```

### Comparing `servey-2.8.3/servey/servey_starlette/starlette_app.py` & `servey-2.8.4/servey/servey_starlette/starlette_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 LOGGER = logging.getLogger(__name__)
 routes = []
 for route_factory in sorted(
     list(get_impls(RouteFactoryABC)), key=lambda f: f.priority, reverse=True
 ):
     routes.extend(route_factory().create_routes())
 for route in routes:
-    LOGGER.debug(f"starlette_path:%s", route.path)
+    LOGGER.debug("starlette_path:%s", route.path)
 
 app = Starlette(routes=routes)
```

### Comparing `servey-2.8.3/servey/servey_starlette/statics/index.html` & `servey-2.8.4/servey/servey_starlette/statics/index.html`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/statics/swagger-ui-bundle.js` & `servey-2.8.4/servey/servey_starlette/statics/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_starlette/statics/swagger-ui.css` & `servey-2.8.4/servey/servey_starlette/statics/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/entity_factory/dataclass_factory.py` & `servey-2.8.4/servey/servey_strawberry/entity_factory/dataclass_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,21 +70,16 @@
         annotations = {}
         params = {"__annotations__": annotations}
         # noinspection PyDataclass
         for f in fields(annotation):
             type_ = f.type
             if f.default is not MISSING:
                 type_ = Optional[type_]
-                if (
-                    f.default is None
-                    or isinstance(f.default, str)
-                    or isinstance(f.default, int)
-                    or isinstance(f.default, bool)
-                    or isinstance(f.default, float)
-                    or isinstance(f.default, Decimal)
+                if f.default is None or isinstance(
+                    f.default, (str, int, bool, float, Decimal)
                 ):
                     params[f.name] = f.default
             elif f.default_factory is not MISSING:
                 type_ = Optional[type_]
                 params[f.name] = dataclasses.field(default_factory=f.default_factory)
             annotations[f.name] = schema_factory.get_input(type_)
```

### Comparing `servey-2.8.3/servey/servey_strawberry/entity_factory/entity_factory_abc.py` & `servey-2.8.4/servey/servey_strawberry/entity_factory/entity_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/entity_factory/enum_factory.py` & `servey-2.8.4/servey/servey_strawberry/entity_factory/enum_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/entity_factory/forward_ref_factory.py` & `servey-2.8.4/servey/servey_strawberry/entity_factory/forward_ref_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/entity_factory/generic_factory.py` & `servey-2.8.4/servey/servey_strawberry/entity_factory/generic_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     list: List,
     set: List,
     frozenset: List,
 }
 
 
 class GenericFactory(EntityFactoryABC):
-    priority: int = 150
+    priority: int = 160
 
     def create_type(
         self, annotation: Type, schema_factory: SchemaFactory
     ) -> Optional[Type]:
         origin = typing_inspect.get_origin(annotation)
         if origin:
             origin = _TYPES_BY_ORIGIN.get(origin) or origin
```

### Comparing `servey-2.8.3/servey/servey_strawberry/entity_factory/no_op_factory.py` & `servey-2.8.4/servey/servey_strawberry/entity_factory/no_op_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/handler_filter/authorization_handler_filter.py` & `servey-2.8.4/servey/servey_strawberry/handler_filter/authorization_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/handler_filter/handler_filter_abc.py` & `servey-2.8.4/servey/servey_strawberry/handler_filter/handler_filter_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py` & `servey-2.8.4/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/schema_factory.py` & `servey-2.8.4/servey/servey_strawberry/schema_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from servey.servey_strawberry.handler_filter.handler_filter_abc import (
     HandlerFilterABC,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 
+# pylint: disable=R0902
 @dataclass
 class SchemaFactory:
     """
     This class is tasked with converting standard python types into types usable by strawberry and therefore graphql.
     """
 
     types: Dict[str, Type] = field(default_factory=dict)
@@ -38,27 +39,27 @@
     query: Dict[str, StrawberryField] = field(default_factory=dict)
     mutation: Dict[str, StrawberryField] = field(default_factory=dict)
     subscription: Dict[str, StrawberryField] = field(default_factory=dict)
     entity_factories: List[EntityFactoryABC] = field(default_factory=list)
     handler_filters: List[HandlerFilterABC] = field(default_factory=list)
 
     def get_input(self, annotation: Type) -> Type:
-        if hasattr(annotation, "__name__"):
+        if getattr(annotation, "__name__", None) not in (None, "Optional"):
             i = self.inputs.get(annotation.__name__)
             if i:
                 return i
         for entity_factory in self.entity_factories:
             i = entity_factory.create_input(annotation, self)
             if i:
                 if hasattr(annotation, "__name__"):
                     self.inputs[annotation.__name__] = i
                 return i
 
     def get_type(self, annotation: Type):
-        if hasattr(annotation, "__name__"):
+        if getattr(annotation, "__name__", None) not in (None, "Optional"):
             type_ = self.types.get(annotation.__name__)
             if type_:
                 return type_
         for entity_factory in self.entity_factories:
             type_ = entity_factory.create_type(annotation, self)
             if type_:
                 if hasattr(annotation, "__name__"):
@@ -74,14 +75,15 @@
         f = strawberry.field(resolver=action.fn)
         f.name = action.name
         if trigger.method in UPDATE_METHODS:
             self.mutation[f.name] = f
         else:
             self.query[f.name] = f
 
+    # pylint: disable=R0911
     def _resolve_type_futures(self, type_, resolved: Set):
         if isinstance(type_, str):
             type_ = self.types[type_]
         if isinstance(type_, StrawberryAnnotation):
             type_.type = self._resolve_type_futures(type_.annotation, resolved)
             return type_
         if isinstance(type_, StrawberryContainer):
@@ -100,35 +102,36 @@
         if origin:
             args = tuple(
                 self._resolve_type_futures(a, resolved)
                 for a in typing_inspect.get_args(type_)
             )
             if origin is list:
                 return List[args]
-            else:
-                return origin[args]
-        if is_dataclass(type_):
-            if type_.__name__ in resolved:
-                return type_
-            resolved.add(type_.__name__)
-            # noinspection PyDataclass
-            for f in fields(type_):
-                if isinstance(f, StrawberryField):
-                    if f.type is UNRESOLVED:
-                        resolver = f.base_resolver
-                        field_type = resolver.signature.return_annotation
-                        field_type = self._resolve_type_futures(field_type, resolved)
-                        resolver_override = StrawberryResolver(
-                            resolver.wrapped_func, type_override=field_type
-                        )
-                        f.base_resolver = resolver_override
-                else:
-                    f.type = self._resolve_type_futures(f.type, resolved)
+            return origin[args]
+        self._resolve_type_futures_for_dataclass(type_, resolved)
         return type_
 
+    def _resolve_type_futures_for_dataclass(self, type_, resolved: Set):
+        if not is_dataclass(type_) or type_.__name__ in resolved:
+            return
+        resolved.add(type_.__name__)
+        # noinspection PyDataclass
+        for f in fields(type_):
+            if isinstance(f, StrawberryField):
+                if f.type is UNRESOLVED:
+                    resolver = f.base_resolver
+                    field_type = resolver.signature.return_annotation
+                    field_type = self._resolve_type_futures(field_type, resolved)
+                    resolver_override = StrawberryResolver(
+                        resolver.wrapped_func, type_override=field_type
+                    )
+                    f.base_resolver = resolver_override
+            else:
+                f.type = self._resolve_type_futures(f.type, resolved)
+
     def create_schema(self):
         resolved = set()
         for f in self.query.values():
             f.type = self._resolve_type_futures(f.type, resolved)
         for f in self.mutation.values():
             f.type = self._resolve_type_futures(f.type, resolved)
```

### Comparing `servey-2.8.3/servey/servey_strawberry/schema_factory_lazy_input.py` & `servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_input.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/schema_factory_lazy_type.py` & `servey-2.8.4/servey/servey_strawberry/schema_factory_lazy_type.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/statics/index.html` & `servey-2.8.4/servey/servey_strawberry/statics/index.html`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_strawberry/strawberry_starlette_route_factory.py` & `servey-2.8.4/servey/servey_strawberry/strawberry_starlette_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_test/test_servey_actions.py` & `servey-2.8.4/servey/servey_test/test_servey_actions.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_thread/__main__.py` & `servey-2.8.4/servey/servey_thread/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_thread/asyncio_subscription_service.py` & `servey-2.8.4/servey/servey_thread/asyncio_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_thread/fixed_rate_trigger_thread.py` & `servey-2.8.4/servey/servey_thread/fixed_rate_trigger_thread.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_web_page/web_page_action_endpoint.py` & `servey-2.8.4/servey/servey_web_page/web_page_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_web_page/web_page_action_endpoint_factory.py` & `servey-2.8.4/servey/servey_web_page/web_page_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_web_page/web_page_event_handler.py` & `servey-2.8.4/servey/servey_web_page/web_page_event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import inspect
 import mimetypes
 from dataclasses import field, dataclass
-from typing import Optional, Any, Awaitable
+from typing import Optional, Awaitable
 
 from marshy import get_default_context
 from marshy.marshaller_context import MarshallerContext
 from marshy.types import ExternalItemType
 from schemey import get_default_schema_context, SchemaContext
 
 from servey.action.action import Action
@@ -32,15 +32,15 @@
     def template(self):
         template = getattr(self, "_template", None)
         if not template:
             template = get_environment().get_template(self.template_name)
             setattr(self, "_template", template)
         return template
 
-    def handle(self, event: ExternalItemType, result: Any) -> ExternalItemType:
+    def handle(self, event: ExternalItemType, context) -> ExternalItemType:
         kwargs = self.parse_kwargs(event)
         result = self.action.fn(**kwargs)
         if isinstance(result, Awaitable):
             loop = asyncio.get_event_loop()
             result = loop.run_until_complete(result)
         if isinstance(result, Redirect):
             return {
```

### Comparing `servey-2.8.3/servey/servey_web_page/web_page_trigger.py` & `servey-2.8.4/servey/servey_web_page/web_page_trigger.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/servey_web_page/web_page_trigger_handler.py` & `servey-2.8.4/servey/servey_web_page/web_page_trigger_handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         if not isinstance(trigger, WebPageTrigger):
             return
         events = lambda_definition.get("events")
         if not events:
             events = lambda_definition["events"] = []
         path = trigger.path or f"/{action.name.replace('_', '-')}"
         events.append(
-            dict(http=dict(path=path, method=trigger.method.value, cors=True))
+            {"http": {"path": path, "method": trigger.method.value, "cors": True}}
         )
```

### Comparing `servey-2.8.3/servey/subscription/__init__.py` & `servey-2.8.4/servey/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/subscription/subscription.py` & `servey-2.8.4/servey/subscription/subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     event_filter: Optional[EventFilterABC] = None
     action_subscribers: Tuple[Action, ...] = tuple()
 
     def publish(self, event: T):
         """
         Publish an event to subscribers
         """
+        # pylint: disable=R0401
         from servey.subscription.subscription_service import get_subscription_services
 
         for subscription_service in get_subscription_services():
             subscription_service.publish(self, event)
 
 
 def subscription(
```

### Comparing `servey-2.8.3/servey/subscription/subscription_event.py` & `servey-2.8.4/servey/subscription/subscription_event.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/subscription/subscription_service.py` & `servey-2.8.4/servey/subscription/subscription_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple, List
 
 from marshy.factory.impl_marshaller_factory import get_impls
 
 from servey.finder.subscription_finder_abc import find_subscriptions
+
+# pylint: disable=R0401
 from servey.subscription.subscription import Subscription, T
 
 
 class SubscriptionServiceABC(ABC):
     """
     Service for sending messages to subscribed clients (Possibly by websocket)
     """
@@ -30,14 +32,15 @@
         Create a subscription service if the current environment supports it.
         """
 
 
 _SUBSCRIPTION_SERVICES = None
 
 
+# pylint: disable=W0603
 def get_subscription_services() -> Tuple[SubscriptionServiceABC, ...]:
     global _SUBSCRIPTION_SERVICES
     if _SUBSCRIPTION_SERVICES is None:
         subscriptions = list(find_subscriptions())
         _SUBSCRIPTION_SERVICES = tuple(
             s
             for s in (
```

### Comparing `servey-2.8.3/servey/trigger/web_trigger.py` & `servey-2.8.4/servey/trigger/web_trigger.py`

 * *Files identical despite different names*

### Comparing `servey-2.8.3/servey/util/__init__.py` & `servey-2.8.4/servey/util/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 
 def to_snake_case(name: str) -> str:
     return _PATTERN.sub("_", name).lower()
 
 
 def entity_to_camel_case(name: str) -> str:
-    parts = name.split('_')
+    parts = name.split("_")
     result = []
     for part in parts:
         result.append(part[0].upper())
         result.append(part[1:].lower())
-    return ''.join(result)
+    return "".join(result)
 
 
 def attr_camel_case(name: str) -> str:
-    parts = name.split('_')
+    parts = name.split("_")
     result = [parts[0].lower()]
     for part in parts[1:]:
         result.append(part[0].upper())
         result.append(part[1:].lower())
-    return ''.join(result)
+    return "".join(result)
 
 
 def secure_hash(item: ExternalType) -> str:
     item_json = json.dumps(item)
     item_bytes = item_json.encode("utf-8")
     return secure_hash_content(item_bytes)
```

### Comparing `servey-2.8.3/servey/util/singleton_abc.py` & `servey-2.8.4/servey/util/singleton_abc.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
             instance = object.__new__(cls)
             setattr(cls, "__instance", instance)
         return instance
 
     def __repr__(self):
         return self.__class__.__name__
 
+    # pylint: disable=W0613
     # noinspection PyUnusedLocal
     @classmethod
     def __marshaller_factory__(cls, marshaller_context):
         return SingletonMarshaller(cls)
 
 
 class SingletonMarshaller(MarshallerABC[T]):
```

### Comparing `servey-2.8.3/servey.egg-info/SOURCES.txt` & `servey-2.8.4/servey.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-README.md
+MANIFEST.in
 setup.py
 marshy_config_servey/__init__.py
 servey/__init__.py
 servey/__main__.py
 servey/errors.py
-servey/version.py
 servey.egg-info/PKG-INFO
 servey.egg-info/SOURCES.txt
 servey.egg-info/dependency_links.txt
 servey.egg-info/requires.txt
 servey.egg-info/top_level.txt
 servey/action/__init__.py
 servey/action/action.py
```

### Comparing `servey-2.8.3/servey.egg-info/requires.txt` & `servey-2.8.4/servey.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-marshy~=4.0
-schemey~=6.0
+cryptography~=37.0
 json-urley~=1.0
+marshy~=4.0
 pyjwt~=2.4
-cryptography~=37.0
+python-dateutil~=2.8
+schemey~=6.0
 
 [all]
-starlette~=0.19
-uvicorn[standard]~=0.18
-requests~=2.28
+pytest-xdist~=3.2
 celery~=5.2
-black
-pygments~=2.13
-pytest
 ruamel.yaml~=0.17
-pyyaml~=6.0
-strawberry-graphql~=0.151
+pytest-cov~=4.0
+pygments~=2.13
+starlette~=0.19
+pytest~=7.2
+requests~=2.28
+black~=23.3
+boto3~=1.26
 Jinja2~=3.1
 python-multipart~=0.0
+pyyaml~=6.0
+uvicorn[standard]~=0.18
+pylint~=2.17
+strawberry-graphql~=0.151
 
 [dev]
-black
-pytest
+black~=23.3
+boto3~=1.26
+pytest~=7.2
+pytest-cov~=4.0
+pytest-xdist~=3.2
+pylint~=2.17
 
 [scheduler]
 celery~=5.2
 
 [server]
 starlette~=0.19
 strawberry-graphql~=0.151
```

### Comparing `servey-2.8.3/setup.py` & `servey-2.8.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import setuptools
 
-from servey.version import __version__
-
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extras_require = {
-    "dev": ["black", "pytest"],
+    "dev": [
+        "black~=23.3",
+        "boto3~=1.26",
+        "pytest~=7.2",
+        "pytest-cov~=4.0",
+        "pytest-xdist~=3.2",
+        "pylint~=2.17",
+    ],
     "server": [
         "starlette~=0.19",
         "strawberry-graphql~=0.151",
         "uvicorn[standard]~=0.18",
         "pygments~=2.13",
         "requests~=2.28",
         "python-multipart~=0.0",
@@ -32,33 +37,35 @@
         for dependency in dependencies
     }
 )
 
 
 setuptools.setup(
     name="servey",
-    version=__version__,
     author="Tim O'Farrell",
     author_email="tofarr@gmail.com",
     description="A better API layer for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tofarr/servey",
     packages=setuptools.find_packages(
         exclude=("tests*", "servey_main*", "static_site", "examples")
     ),
     package_data={"": ["*.html", "*.js", "*.css", "*.yml"]},
     include_package_data=True,
     install_requires=[
-        "marshy~=4.0",
-        "schemey~=6.0",
+        "cryptography~=37.0",
         "json-urley~=1.0",
+        "marshy~=4.0",
         "pyjwt~=2.4",
-        "cryptography~=37.0",
+        "python-dateutil~=2.8",
+        "schemey~=6.0",
     ],
     extras_require=extras_require,
+    setup_requires=["setuptools-git-versioning"],
+    setuptools_git_versioning={"enabled": True, "dirty_template": "{tag}"},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

