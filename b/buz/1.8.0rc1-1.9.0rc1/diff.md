# Comparing `tmp/buz-1.8.0rc1.tar.gz` & `tmp/buz-1.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buz-1.8.0rc1.tar", max compression
+gzip compressed data, was "buz-1.9.0rc1.tar", max compression
```

## Comparing `buz-1.8.0rc1.tar` & `buz-1.9.0rc1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     1062 2022-09-19 15:02:30.814345 buz-1.8.0rc1/LICENSE
--rw-r--r--   0        0        0      104 2022-09-19 15:02:30.814345 buz-1.8.0rc1/README.md
--rw-r--r--   0        0        0     1389 2022-09-19 15:02:30.814345 buz-1.8.0rc1/pyproject.toml
--rw-r--r--   0        0        0      109 2022-09-19 15:02:30.814345 buz-1.8.0rc1/src/buz/__init__.py
--rw-r--r--   0        0        0      302 2022-09-19 15:02:30.814345 buz-1.8.0rc1/src/buz/command/__init__.py
--rw-r--r--   0        0        0      680 2022-09-19 15:02:30.814345 buz-1.8.0rc1/src/buz/command/base_command_handler.py
--rw-r--r--   0        0        0      193 2022-09-19 15:02:30.814345 buz-1.8.0rc1/src/buz/command/command.py
--rw-r--r--   0        0        0      175 2022-09-19 15:02:30.814345 buz-1.8.0rc1/src/buz/command/command_bus.py
--rw-r--r--   0        0        0      316 2022-09-19 15:02:30.814345 buz-1.8.0rc1/src/buz/command/command_handler.py
--rw-r--r--   0        0        0      370 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/middleware/__init__.py
--rw-r--r--   0        0        0      709 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      385 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1031 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      266 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/sync/__init__.py
--rw-r--r--   0        0        0      401 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/sync/more_than_one_command_handler_related_exception.py
--rw-r--r--   0        0        0     1115 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/command/sync/sync_command_bus.py
--rw-r--r--   0        0        0      256 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/__init__.py
--rw-r--r--   0        0        0      645 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/base_subscriber.py
--rw-r--r--   0        0        0      189 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/event.py
--rw-r--r--   0        0        0      293 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/event_bus.py
--rw-r--r--   0        0        0      656 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/__init__.py
--rw-r--r--   0        0        0      263 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/consume_strategy/__init__.py
--rw-r--r--   0        0        0      179 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
--rw-r--r--   0        0        0      756 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
--rw-r--r--   0        0        0      215 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/event_not_published_exception.py
--rw-r--r--   0        0        0      302 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/event_restore_exception.py
--rw-r--r--   0        0        0      258 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/execution_strategy/__init__.py
--rw-r--r--   0        0        0      192 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
--rw-r--r--   0        0        0      429 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
--rw-r--r--   0        0        0     5529 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/kombu_consumer.py
--rw-r--r--   0        0        0     3251 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/kombu_event_bus.py
--rw-r--r--   0        0        0      285 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/publish_strategy/__init__.py
--rw-r--r--   0        0        0      382 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
--rw-r--r--   0        0        0      309 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
--rw-r--r--   0        0        0      894 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/__init__.py
--rw-r--r--   0        0        0      361 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/consume_retrier.py
--rw-r--r--   0        0        0      229 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/consumed_event_retry.py
--rw-r--r--   0        0        0      449 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
--rw-r--r--   0        0        0     1332 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
--rw-r--r--   0        0        0      230 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
--rw-r--r--   0        0        0      993 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py
--rw-r--r--   0        0        0      241 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/reject_callback.py
--rw-r--r--   0        0        0     1236 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
--rw-r--r--   0        0        0       75 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/serializer_enum.py
--rw-r--r--   0        0        0      695 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py
--rw-r--r--   0        0        0      704 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/kombu/worker.py
--rw-r--r--   0        0        0      773 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/__init__.py
--rw-r--r--   0        0        0      651 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/base_consume_middleware.py
--rw-r--r--   0        0        0      531 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/base_publish_middleware.py
--rw-r--r--   0        0        0      363 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/consume_middleware.py
--rw-r--r--   0        0        0     1021 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
--rw-r--r--   0        0        0      315 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/publish_middleware.py
--rw-r--r--   0        0        0      949 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
--rw-r--r--   0        0        0      303 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/subscriber.py
--rw-r--r--   0        0        0       91 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/sync/__init__.py
--rw-r--r--   0        0        0     1413 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/sync/sync_event_bus.py
--rw-r--r--   0        0        0     1209 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/__init__.py
--rw-r--r--   0        0        0      506 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
--rw-r--r--   0        0        0      779 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
--rw-r--r--   0        0        0      515 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py
--rw-r--r--   0        0        0      860 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_record.py
--rw-r--r--   0        0        0      281 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_record_stream_finder.py
--rw-r--r--   0        0        0      708 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
--rw-r--r--   0        0        0      509 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_repository.py
--rw-r--r--   0        0        0       89 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_sorting_criteria.py
--rw-r--r--   0        0        0      903 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
--rw-r--r--   0        0        0     2416 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
--rw-r--r--   0        0        0      272 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/handler.py
--rw-r--r--   0        0        0      293 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/__init__.py
--rw-r--r--   0        0        0      206 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/handler_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/locator.py
--rw-r--r--   0        0        0      206 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/message_fqn_not_found_exception.py
--rw-r--r--   0        0        0      512 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/pypendency/__init__.py
--rw-r--r--   0        0        0     3517 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/pypendency/container_locator.py
--rw-r--r--   0        0        0      246 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/pypendency/handler_already_registered_exception.py
--rw-r--r--   0        0        0      240 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/pypendency/handler_not_found_exception.py
--rw-r--r--   0        0        0      235 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
--rw-r--r--   0        0        0      370 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/sync/__init__.py
--rw-r--r--   0        0        0      245 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/sync/handler_already_registered_exception.py
--rw-r--r--   0        0        0      234 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/sync/handler_not_registered_exception.py
--rw-r--r--   0        0        0     2082 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/locator/sync/instance_locator.py
--rw-r--r--   0        0        0     1043 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/message.py
--rw-r--r--   0        0        0      176 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/middleware/__init__.py
--rw-r--r--   0        0        0       54 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/middleware/middleware.py
--rw-r--r--   0        0        0     1002 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/middleware/middleware_chain_builder.py
--rw-r--r--   0        0        0        0 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/py.typed
--rw-r--r--   0        0        0      320 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/__init__.py
--rw-r--r--   0        0        0      627 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/base_query_handler.py
--rw-r--r--   0        0        0      364 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/middleware/__init__.py
--rw-r--r--   0        0        0      783 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/middleware/base_handle_middleware.py
--rw-r--r--   0        0        0      400 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/middleware/handle_middleware.py
--rw-r--r--   0        0        0     1052 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/middleware/handle_middleware_chain_resolver.py
--rw-r--r--   0        0        0      189 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/query.py
--rw-r--r--   0        0        0      189 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/query_bus.py
--rw-r--r--   0        0        0      328 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/query_handler.py
--rw-r--r--   0        0        0      153 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/query_response.py
--rw-r--r--   0        0        0      250 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/sync/__init__.py
--rw-r--r--   0        0        0      375 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/sync/more_than_one_query_handler_related_exception.py
--rw-r--r--   0        0        0     1104 2022-09-19 15:02:30.818345 buz-1.8.0rc1/src/buz/query/sync/sync_query_bus.py
--rw-r--r--   0        0        0     1422 2022-09-19 15:02:46.343636 buz-1.8.0rc1/setup.py
--rw-r--r--   0        0        0     1178 2022-09-19 15:02:46.343914 buz-1.8.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-11-15 14:44:53.618677 buz-1.9.0rc1/LICENSE
+-rw-r--r--   0        0        0      104 2022-11-15 14:44:53.618677 buz-1.9.0rc1/README.md
+-rw-r--r--   0        0        0     1389 2022-11-15 14:44:53.618677 buz-1.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      109 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/__init__.py
+-rw-r--r--   0        0        0      302 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/__init__.py
+-rw-r--r--   0        0        0      680 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/base_command_handler.py
+-rw-r--r--   0        0        0      193 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/command.py
+-rw-r--r--   0        0        0      175 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/command_bus.py
+-rw-r--r--   0        0        0      316 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/command_handler.py
+-rw-r--r--   0        0        0      370 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/__init__.py
+-rw-r--r--   0        0        0      709 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      385 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1031 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      266 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/sync/__init__.py
+-rw-r--r--   0        0        0      401 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/sync/more_than_one_command_handler_related_exception.py
+-rw-r--r--   0        0        0     1115 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/command/sync/sync_command_bus.py
+-rw-r--r--   0        0        0      256 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/__init__.py
+-rw-r--r--   0        0        0      645 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/base_subscriber.py
+-rw-r--r--   0        0        0      189 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/event.py
+-rw-r--r--   0        0        0      293 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/event_bus.py
+-rw-r--r--   0        0        0      656 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/__init__.py
+-rw-r--r--   0        0        0      263 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/__init__.py
+-rw-r--r--   0        0        0      179 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/consume_strategy.py
+-rw-r--r--   0        0        0      756 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py
+-rw-r--r--   0        0        0      215 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/event_not_published_exception.py
+-rw-r--r--   0        0        0      302 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/event_restore_exception.py
+-rw-r--r--   0        0        0      258 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/execution_strategy/__init__.py
+-rw-r--r--   0        0        0      192 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/execution_strategy/execution_strategy.py
+-rw-r--r--   0        0        0      429 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/execution_strategy/self_process_execution_strategy.py
+-rw-r--r--   0        0        0     5529 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/kombu_consumer.py
+-rw-r--r--   0        0        0     3251 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/kombu_event_bus.py
+-rw-r--r--   0        0        0      285 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/publish_strategy/__init__.py
+-rw-r--r--   0        0        0      382 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/publish_strategy/fanout_exchange_per_event_publish_strategy.py
+-rw-r--r--   0        0        0      309 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/publish_strategy/publish_strategy.py
+-rw-r--r--   0        0        0      894 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/__init__.py
+-rw-r--r--   0        0        0      361 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/consume_retrier.py
+-rw-r--r--   0        0        0      229 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/consumed_event_retry.py
+-rw-r--r--   0        0        0      449 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/consumed_event_retry_repository.py
+-rw-r--r--   0        0        0     1332 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py
+-rw-r--r--   0        0        0      230 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/max_retries_negative_exception.py
+-rw-r--r--   0        0        0      993 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py
+-rw-r--r--   0        0        0      241 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/reject_callback.py
+-rw-r--r--   0        0        0     1236 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py
+-rw-r--r--   0        0        0       75 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/serializer_enum.py
+-rw-r--r--   0        0        0      695 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py
+-rw-r--r--   0        0        0      704 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/kombu/worker.py
+-rw-r--r--   0        0        0      773 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/__init__.py
+-rw-r--r--   0        0        0      651 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/base_consume_middleware.py
+-rw-r--r--   0        0        0      531 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/base_publish_middleware.py
+-rw-r--r--   0        0        0      363 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/consume_middleware.py
+-rw-r--r--   0        0        0     1021 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      315 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/publish_middleware.py
+-rw-r--r--   0        0        0      949 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      303 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/subscriber.py
+-rw-r--r--   0        0        0       91 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/sync/__init__.py
+-rw-r--r--   0        0        0     1413 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/sync/sync_event_bus.py
+-rw-r--r--   0        0        0     1209 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/__init__.py
+-rw-r--r--   0        0        0      506 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/event_to_outbox_record_translator.py
+-rw-r--r--   0        0        0      779 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py
+-rw-r--r--   0        0        0      515 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py
+-rw-r--r--   0        0        0      860 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record.py
+-rw-r--r--   0        0        0      281 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record_stream_finder.py
+-rw-r--r--   0        0        0      708 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py
+-rw-r--r--   0        0        0      509 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_repository.py
+-rw-r--r--   0        0        0       89 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_sorting_criteria.py
+-rw-r--r--   0        0        0      903 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py
+-rw-r--r--   0        0        0     2416 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py
+-rw-r--r--   0        0        0      272 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/handler.py
+-rw-r--r--   0        0        0      293 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/__init__.py
+-rw-r--r--   0        0        0      206 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/handler_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      512 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/locator.py
+-rw-r--r--   0        0        0      206 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/message_fqn_not_found_exception.py
+-rw-r--r--   0        0        0      512 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/__init__.py
+-rw-r--r--   0        0        0     3517 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/container_locator.py
+-rw-r--r--   0        0        0      246 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/handler_already_registered_exception.py
+-rw-r--r--   0        0        0      240 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/handler_not_found_exception.py
+-rw-r--r--   0        0        0      235 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/pypendency/handler_not_registered_exception.py
+-rw-r--r--   0        0        0      370 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/__init__.py
+-rw-r--r--   0        0        0      245 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/handler_already_registered_exception.py
+-rw-r--r--   0        0        0      234 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/handler_not_registered_exception.py
+-rw-r--r--   0        0        0     2082 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/locator/sync/instance_locator.py
+-rw-r--r--   0        0        0     1359 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/message.py
+-rw-r--r--   0        0        0      176 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/middleware/__init__.py
+-rw-r--r--   0        0        0       54 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/middleware/middleware.py
+-rw-r--r--   0        0        0     1002 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/middleware/middleware_chain_builder.py
+-rw-r--r--   0        0        0        0 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/py.typed
+-rw-r--r--   0        0        0      320 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/__init__.py
+-rw-r--r--   0        0        0      627 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/base_query_handler.py
+-rw-r--r--   0        0        0      364 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/__init__.py
+-rw-r--r--   0        0        0      783 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/base_handle_middleware.py
+-rw-r--r--   0        0        0      400 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/handle_middleware.py
+-rw-r--r--   0        0        0     1052 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/middleware/handle_middleware_chain_resolver.py
+-rw-r--r--   0        0        0      189 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query.py
+-rw-r--r--   0        0        0      189 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query_bus.py
+-rw-r--r--   0        0        0      328 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query_handler.py
+-rw-r--r--   0        0        0      153 2022-11-15 14:44:53.618677 buz-1.9.0rc1/src/buz/query/query_response.py
+-rw-r--r--   0        0        0      250 2022-11-15 14:44:53.622677 buz-1.9.0rc1/src/buz/query/sync/__init__.py
+-rw-r--r--   0        0        0      375 2022-11-15 14:44:53.622677 buz-1.9.0rc1/src/buz/query/sync/more_than_one_query_handler_related_exception.py
+-rw-r--r--   0        0        0     1104 2022-11-15 14:44:53.622677 buz-1.9.0rc1/src/buz/query/sync/sync_query_bus.py
+-rw-r--r--   0        0        0     1422 2022-11-15 14:45:18.261402 buz-1.9.0rc1/setup.py
+-rw-r--r--   0        0        0     1178 2022-11-15 14:45:18.261790 buz-1.9.0rc1/PKG-INFO
```

### Comparing `buz-1.8.0rc1/LICENSE` & `buz-1.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/pyproject.toml` & `buz-1.9.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "buz"
-version = "1.8.0rc1"
+version = "1.9.0rc1"
 description = "Buz is a set of light, simple and extensible implementations of event, command and query buses."
 readme = "README.md"
 authors = ["Luis Pintado Lozano <luis.pintado.lozano@gmail.com>"]
 license = "MIT License"
 classifiers=[
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `buz-1.8.0rc1/src/buz/command/base_command_handler.py` & `buz-1.9.0rc1/src/buz/command/base_command_handler.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/command/middleware/base_handle_middleware.py` & `buz-1.9.0rc1/src/buz/command/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/command/middleware/handle_middleware_chain_resolver.py` & `buz-1.9.0rc1/src/buz/command/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/command/sync/sync_command_bus.py` & `buz-1.9.0rc1/src/buz/command/sync/sync_command_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/base_subscriber.py` & `buz-1.9.0rc1/src/buz/event/base_subscriber.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/__init__.py` & `buz-1.9.0rc1/src/buz/event/kombu/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py` & `buz-1.9.0rc1/src/buz/event/kombu/consume_strategy/queue_per_subscriber_consume_strategy.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/kombu_consumer.py` & `buz-1.9.0rc1/src/buz/event/kombu/kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/kombu_event_bus.py` & `buz-1.9.0rc1/src/buz/event/kombu/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/retry/__init__.py` & `buz-1.9.0rc1/src/buz/event/kombu/retry/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py` & `buz-1.9.0rc1/src/buz/event/kombu/retry/max_retries_consume_retrier.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py` & `buz-1.9.0rc1/src/buz/event/kombu/retry/publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py` & `buz-1.9.0rc1/src/buz/event/kombu/retry/simple_publish_retry_policy.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py` & `buz-1.9.0rc1/src/buz/event/kombu/subscribers_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/kombu/worker.py` & `buz-1.9.0rc1/src/buz/event/kombu/worker.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/middleware/__init__.py` & `buz-1.9.0rc1/src/buz/event/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/middleware/base_consume_middleware.py` & `buz-1.9.0rc1/src/buz/event/middleware/base_consume_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/middleware/base_publish_middleware.py` & `buz-1.9.0rc1/src/buz/event/middleware/base_publish_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py` & `buz-1.9.0rc1/src/buz/event/middleware/consume_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py` & `buz-1.9.0rc1/src/buz/event/middleware/publish_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/sync/sync_event_bus.py` & `buz-1.9.0rc1/src/buz/event/sync/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/__init__.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/fqn_to_event_mapper.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_criteria.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_record.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/outbox_record_to_event_translator.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_event_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py` & `buz-1.9.0rc1/src/buz/event/transactional_outbox/transactional_outbox_worker.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/locator/locator.py` & `buz-1.9.0rc1/src/buz/locator/locator.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/locator/pypendency/__init__.py` & `buz-1.9.0rc1/src/buz/locator/pypendency/__init__.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/locator/pypendency/container_locator.py` & `buz-1.9.0rc1/src/buz/locator/pypendency/container_locator.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/locator/sync/instance_locator.py` & `buz-1.9.0rc1/src/buz/locator/sync/instance_locator.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/message.py` & `buz-1.9.0rc1/src/buz/message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import inspect
 from abc import ABC
 from dataclasses import field, dataclass
 from datetime import datetime
-from typing import Any, ClassVar
+from typing import Any, ClassVar, Dict
 from uuid import uuid4
 
 
 @dataclass(frozen=True)
 class Message(ABC):
     DATE_TIME_FORMAT: ClassVar[str] = "%Y-%m-%d %H:%M:%S.%f"
 
@@ -19,15 +20,21 @@
         return f"{cls.__module__}.{cls.__name__}"
 
     @classmethod
     def restore(cls, **kwargs: Any) -> "Message":  # type: ignore[misc]
         message_id = kwargs.pop("id")
         created_at = kwargs.pop("created_at")
 
-        instance = cls(**kwargs)  # type: ignore
+        instance = cls.__from_dict(kwargs)  # type: ignore
 
         object.__setattr__(instance, "id", message_id)
         object.__setattr__(instance, "created_at", created_at)
         return instance
 
+    @classmethod
+    def __from_dict(cls, data: Dict) -> "Message":
+        expected_params = inspect.signature(cls).parameters
+        actual_params = {key: value for key, value in data.items() if key in expected_params}
+        return cls(**actual_params)  # type: ignore[call-arg]
+
     def parsed_created_at(self) -> datetime:
         return datetime.strptime(self.created_at, self.DATE_TIME_FORMAT)
```

### Comparing `buz-1.8.0rc1/src/buz/middleware/middleware_chain_builder.py` & `buz-1.9.0rc1/src/buz/middleware/middleware_chain_builder.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/query/base_query_handler.py` & `buz-1.9.0rc1/src/buz/query/base_query_handler.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/query/middleware/base_handle_middleware.py` & `buz-1.9.0rc1/src/buz/query/middleware/base_handle_middleware.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/query/middleware/handle_middleware_chain_resolver.py` & `buz-1.9.0rc1/src/buz/query/middleware/handle_middleware_chain_resolver.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/src/buz/query/sync/sync_query_bus.py` & `buz-1.9.0rc1/src/buz/query/sync/sync_query_bus.py`

 * *Files identical despite different names*

### Comparing `buz-1.8.0rc1/setup.py` & `buz-1.9.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 extras_require = \
 {':python_full_version < "3.7.0"': ['dataclasses>=0.8,<0.9'],
  'kombu': ['kombu>=4.6.11'],
  'pypendency': ['pypendency>=0.1.0,<0.2.0']}
 
 setup_kwargs = {
     'name': 'buz',
-    'version': '1.8.0rc1',
+    'version': '1.9.0rc1',
     'description': 'Buz is a set of light, simple and extensible implementations of event, command and query buses.',
     'long_description': '# Buz\n\nBuz is a set of light, simple and extensible implementations of event, command and query buses.\n ',
     'author': 'Luis Pintado Lozano',
     'author_email': 'luis.pintado.lozano@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `buz-1.8.0rc1/PKG-INFO` & `buz-1.9.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buz
-Version: 1.8.0rc1
+Version: 1.9.0rc1
 Summary: Buz is a set of light, simple and extensible implementations of event, command and query buses.
 License: MIT
 Author: Luis Pintado Lozano
 Author-email: luis.pintado.lozano@gmail.com
 Requires-Python: >=3.6.9,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

