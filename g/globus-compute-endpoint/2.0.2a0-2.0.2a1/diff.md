# Comparing `tmp/globus-compute-endpoint-2.0.2a0.tar.gz` & `tmp/globus-compute-endpoint-2.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.2a0.tar", last modified: Mon May  1 15:14:39 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.2a1.tar", last modified: Mon May  8 22:01:11 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.2a0.tar` & `globus-compute-endpoint-2.0.2a1.tar`

### file list

```diff
@@ -1,70 +1,77 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.999767 globus-compute-endpoint-2.0.2a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.2a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-05-01 15:14:38.999832 globus-compute-endpoint-2.0.2a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.2a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.993466 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    19300 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.995486 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    24838 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.996174 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.996431 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.996564 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.998079 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    49946 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    36234 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.998216 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.998604 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 15:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.999264 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5470 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-05-01 15:05:29.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.994151 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1840 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2657 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      308 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-05-01 15:14:38.000000 globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-05-01 15:14:39.000067 globus-compute-endpoint-2.0.2a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3635 2023-05-01 15:05:24.000000 globus-compute-endpoint-2.0.2a0/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-01 15:14:38.999624 globus-compute-endpoint-2.0.2a0/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.0.2a0/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a0/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.169955 globus-compute-endpoint-2.0.2a1/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.2a1/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-05-08 22:01:11.170024 globus-compute-endpoint-2.0.2a1/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-20 03:21:56.000000 globus-compute-endpoint-2.0.2a1/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.153855 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    19319 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.162886 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    26121 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24838 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-05-01 15:02:38.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.163689 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.164014 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/utils/config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.164961 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/
+-rw-r--r--   0 lei        (501) staff       (20)      318 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     5954 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     3725 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/globus_compute.py
+-rw-r--r--   0 lei        (501) staff       (20)     4336 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/helper.py
+-rw-r--r--   0 lei        (501) staff       (20)     3725 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/process_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     3719 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/engines/thread_pool.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.165100 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.167833 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1943 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    35357 2023-04-20 15:03:07.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    49946 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    36129 2023-05-08 21:54:40.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8683 2023-04-21 16:13:24.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    19094 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.168019 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.168505 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12926 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.169229 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5470 2023-05-01 18:50:06.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-05-08 21:58:56.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.154729 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1840 2023-05-08 22:01:11.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2928 2023-05-08 22:01:11.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-05-08 22:01:11.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-05-08 22:01:11.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      308 2023-05-08 22:01:11.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-05-08 22:01:11.000000 globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-05-08 22:01:11.170272 globus-compute-endpoint-2.0.2a1/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3635 2023-05-08 21:58:53.000000 globus-compute-endpoint-2.0.2a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-05-08 22:01:11.169726 globus-compute-endpoint-2.0.2a1/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.2a1/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2709 2023-04-24 21:22:25.000000 globus-compute-endpoint-2.0.2a1/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2925 2023-05-05 16:40:44.000000 globus-compute-endpoint-2.0.2a1/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.2a0/LICENSE` & `globus-compute-endpoint-2.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/PKG-INFO` & `globus-compute-endpoint-2.0.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.2a0
+Version: 2.0.2a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.0.2a0/PyPI.md` & `globus-compute-endpoint-2.0.2a1/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def ensure(cls) -> CommandState:
         return click.get_current_context().ensure_object(CommandState)
 
 
 def init_config_dir() -> pathlib.Path:
     try:
         return ensure_compute_dir()
-    except FileExistsError as e:
+    except (FileExistsError, PermissionError) as e:
         raise ClickException(str(e))
 
 
 def get_config_dir() -> pathlib.Path:
     state = CommandState.ensure()
     return state.endpoint_config_dir
```

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -691,28 +691,29 @@
 
 def _serialize_config(config: Config) -> dict:
     """
     Short-term serialization method until config.py is replaced with config.yaml
     """
 
     expand_list = ["strategy", "provider", "launcher"]
+    pass_through_list = ["allowed_functions"]
 
     def to_dict(o):
         mems = {"_type": type(o).__name__}
 
         for k, v in o.__dict__.items():
             if k.startswith("_"):
                 continue
 
             if k in expand_list:
                 mems[k] = to_dict(v)
-            elif not isinstance(v, str):
-                mems[k] = repr(v)
-            else:
+            elif isinstance(v, str) or k in pass_through_list:
                 mems[k] = v
+            else:
+                mems[k] = repr(v)
 
         return mems
 
     result = to_dict(config)
     # when we move to config.yaml, should only need to support a single executor
     result["executors"] = [to_dict(executor) for executor in config.executors]
```

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         self,
         # Execution backed
         executors: list = _DEFAULT_EXECUTORS,
         # Connection info
         environment: str | None = None,
         funcx_service_address=None,
         multi_tenant: bool | None = None,
+        allowed_functions: list[str] | None = None,
         # Tuning info
         heartbeat_period=30,
         heartbeat_threshold=120,
         idle_heartbeats_soft=0,
         idle_heartbeats_hard=5760,  # Two days, divided by `heartbeat_period`
         detach_endpoint=True,
         # Misc info
@@ -144,14 +145,15 @@
         self.executors = executors  # List of executors
 
         # Connection info
         self.environment = environment
         self.funcx_service_address = funcx_service_address
 
         self.multi_tenant = multi_tenant is True
+        self.allowed_functions = allowed_functions
 
         # Tuning info
         self.heartbeat_period = heartbeat_period
         self.heartbeat_threshold = heartbeat_threshold
         self.idle_heartbeats_soft = int(max(0, idle_heartbeats_soft))
         self.idle_heartbeats_hard = int(max(0, idle_heartbeats_hard))
         self.detach_endpoint = detach_endpoint
```

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from globus_compute_endpoint.executors.high_throughput.messages import (
     ManagerStatusReport,
     Message,
     Task,
 )
 from globus_compute_endpoint.executors.high_throughput.worker_map import WorkerMap
 from globus_compute_endpoint.logging_config import ComputeLogger, setup_logging
-from globus_compute_sdk.serialize import ComputeSerializer
 from parsl.version import VERSION as PARSL_VERSION
 
 RESULT_TAG = 10
 TASK_REQUEST_TAG = 11
 HEARTBEAT_CODE = (2**32) - 1
 
 log: ComputeLogger = logging.getLogger(__name__)  # type: ignore
@@ -237,15 +236,14 @@
 
         self.max_queue_size = max_queue_size + self.max_worker_count
         self.tasks_per_round = 1
 
         self.heartbeat_period = heartbeat_period
         self.heartbeat_threshold = heartbeat_threshold
         self.poll_period = poll_period
-        self.serializer = ComputeSerializer()
         self.next_worker_q: list[str] = []  # FIFO queue for spinning up workers.
         self.worker_procs: dict[str, subprocess.Popen] = {}
 
         self.task_status_deltas: dict[str, list[TaskTransition]] = defaultdict(list)
 
         self._kill_event = threading.Event()
         self._result_pusher_thread = threading.Thread(
```

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.2a0"
+__version__ = "2.0.2a1"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.2a0
+Version: 2.0.2a1
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-endpoint-2.0.2a0/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.2a1/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
 globus_compute_endpoint/endpoint/rabbit_mq/base.py
 globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
 globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
 globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
 globus_compute_endpoint/endpoint/utils/__init__.py
 globus_compute_endpoint/endpoint/utils/config.py
+globus_compute_endpoint/engines/__init__.py
+globus_compute_endpoint/engines/base.py
+globus_compute_endpoint/engines/globus_compute.py
+globus_compute_endpoint/engines/helper.py
+globus_compute_endpoint/engines/process_pool.py
+globus_compute_endpoint/engines/thread_pool.py
 globus_compute_endpoint/executors/__init__.py
 globus_compute_endpoint/executors/high_throughput/__init__.py
 globus_compute_endpoint/executors/high_throughput/container_sched.py
 globus_compute_endpoint/executors/high_throughput/executor.py
 globus_compute_endpoint/executors/high_throughput/interchange.py
 globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
 globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
```

### Comparing `globus-compute-endpoint-2.0.2a0/setup.py` & `globus-compute-endpoint-2.0.2a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk>=2.0.2a0",
+    "globus-compute-sdk>=2.0.2a1",
     "globus-compute-common==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.0.2a0/tests/conftest.py` & `globus-compute-endpoint-2.0.2a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.2a0/tests/utils.py` & `globus-compute-endpoint-2.0.2a1/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -70,7 +70,39 @@
     check_period_s = abs(check_period_ms) / 1000.0
     end = time.monotonic() + timeout_s
     while time.monotonic() < end:
         if test_func():
             return True
         time.sleep(check_period_s)
     return False
+
+
+def ez_pack_function(serializer, func, args, kwargs):
+    serialized_func = serializer.serialize(func)
+    serialized_args = serializer.serialize(args)
+    serialized_kwargs = serializer.serialize(kwargs)
+    return serializer.pack_buffers(
+        [serialized_func, serialized_args, serialized_kwargs]
+    )
+
+
+def double(x: int) -> int:
+    return x * 2
+
+
+def slow_double(x: int, sleep_duration_s: int) -> int:
+    import time
+
+    time.sleep(sleep_duration_s)
+    return x * 2
+
+
+def kill_manager():
+    import os
+    import signal
+
+    manager_pid = os.getppid()
+    os.kill(manager_pid, signal.SIGKILL)
+
+
+def div_zero(x: int):
+    return x / 0
```

