# Comparing `tmp/litestar-2.0.0a5.tar.gz` & `tmp/litestar-2.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0a5.tar", max compression
+gzip compressed data, was "litestar-2.0.0a6.tar", max compression
```

## Comparing `litestar-2.0.0a5.tar` & `litestar-2.0.0a6.tar`

### file list

```diff
@@ -1,292 +1,305 @@
--rw-r--r--   0        0        0     1092 2023-04-26 13:40:53.109600 litestar-2.0.0a5/LICENSE
--rw-r--r--   0        0        0    49290 2023-04-26 13:40:53.109600 litestar-2.0.0a5/README.md
--rw-r--r--   0        0        0      744 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/__init__.py
--rw-r--r--   0        0        0      103 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     8632 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5938 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3868 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4239 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14907 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20450 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5935 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0    10117 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5525 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1476 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    10196 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     7074 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2104 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    31705 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10970 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5240 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1464 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2338 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     5995 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/field.py
--rw-r--r--   0        0        0       64 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    13178 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     3736 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     6680 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     6510 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/utils.py
--rw-r--r--   0        0        0    35419 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/background_tasks.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/__init__.py
--rw-r--r--   0        0        0    11640 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     4553 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2365 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2224 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0      807 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12358 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/compression.py
--rw-r--r--   0        0        0     5177 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10832 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/request.py
--rw-r--r--   0        0        0     8999 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1098 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4051 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     8324 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28720 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     3978 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6970 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3916 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/mako.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/msgspec/__init__.py
--rw-r--r--   0        0        0      180 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4206 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2206 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0      290 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0     9259 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/abc.py
--rw-r--r--   0        0        0      328 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     1785 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    13409 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3984 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0     3431 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      742 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/__init__.py
--rw-r--r--   0        0        0      319 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/_slots_base.py
--rw-r--r--   0        0        0      504 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/__init__.py
--rw-r--r--   0        0        0      458 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     3602 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0    11308 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/common.py
--rw-r--r--   0        0        0    11500 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
--rw-r--r--   0        0        0     2849 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
--rw-r--r--   0        0        0     1600 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/plugin.py
--rw-r--r--   0        0        0     1447 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/serialization.py
--rw-r--r--   0        0        0    21853 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/repository.py
--rw-r--r--   0        0        0     1856 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/types.py
--rw-r--r--   0        0        0     9559 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/controller.py
--rw-r--r--   0        0        0    16460 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3757 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17316 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9302 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3360 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/url.py
--rw-r--r--   0        0        0     2386 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/di.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/__init__.py
--rw-r--r--   0        0        0      337 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/exceptions.py
--rw-r--r--   0        0        0      188 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/__init__.py
--rw-r--r--   0        0        0    11610 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/abc.py
--rw-r--r--   0        0        0      245 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/__init__.py
--rw-r--r--   0        0        0     4354 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/abc.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/msgspec/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/msgspec/backend.py
--rw-r--r--   0        0        0     7436 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/msgspec/utils.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/__init__.py
--rw-r--r--   0        0        0     2187 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/backend.py
--rw-r--r--   0        0        0     4163 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/utils.py
--rw-r--r--   0        0        0      866 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/utils.py
--rw-r--r--   0        0        0      658 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/config.py
--rw-r--r--   0        0        0      313 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/exc.py
--rw-r--r--   0        0        0     1269 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/field.py
--rw-r--r--   0        0        0     2201 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/stdlib/dataclass.py
--rw-r--r--   0        0        0     2374 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/types.py
--rw-r--r--   0        0        0     1594 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/utils.py
--rw-r--r--   0        0        0     4368 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/interface.py
--rw-r--r--   0        0        0      309 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/types.py
--rw-r--r--   0        0        0     1728 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/events/__init__.py
--rw-r--r--   0        0        0     4597 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/events/emitter.py
--rw-r--r--   0        0        0     1305 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/events/listener.py
--rw-r--r--   0        0        0     1142 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1621 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5330 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3877 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    20202 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     8104 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    25662 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    60867 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0      340 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/__init__.py
--rw-r--r--   0        0        0     6502 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/_utils.py
--rw-r--r--   0        0        0    12896 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/listener.py
--rw-r--r--   0        0        0     3619 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/route_handler.py
--rw-r--r--   0        0        0      147 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     2967 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3430 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5284 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/base.py
--rw-r--r--   0        0        0     8359 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2565 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6466 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7191 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     8990 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13372 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10811 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7935 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10365 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8558 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      231 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/openapi/config.py
--rw-r--r--   0        0        0    16443 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1648 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4218 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    10984 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/pagination.py
--rw-r--r--   0        0        0    16805 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/params.py
--rw-r--r--   0        0        0     7100 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/partial.py
--rw-r--r--   0        0        0     3926 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/py.typed
--rw-r--r--   0        0        0      278 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/__init__.py
--rw-r--r--   0        0        0    12173 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/base.py
--rw-r--r--   0        0        0     9225 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/file.py
--rw-r--r--   0        0        0     2952 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/redirect.py
--rw-r--r--   0        0        0     4883 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/streaming.py
--rw-r--r--   0        0        0     2994 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/template.py
--rw-r--r--   0        0        0    14975 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response_containers.py
--rw-r--r--   0        0        0    15028 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/router.py
--rw-r--r--   0        0        0      191 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6437 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/base.py
--rw-r--r--   0        0        0    13254 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/http.py
--rw-r--r--   0        0        0     3052 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4933 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     7355 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5019 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/static_files/base.py
--rw-r--r--   0        0        0     3582 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4377 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/base.py
--rw-r--r--   0        0        0     5425 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/template/__init__.py
--rw-r--r--   0        0        0     4113 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17445 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5132 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19555 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    31473 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2532 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21905 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8086 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/testing/transport.py
--rw-r--r--   0        0        0     6939 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4105 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/__init__.py
--rw-r--r--   0        0        0     8697 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      453 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2291 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1645 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/composite_types.py
--rw-r--r--   0        0        0      183 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/empty.py
--rw-r--r--   0        0        0     2662 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/file_types.py
--rw-r--r--   0        0        0      344 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1720 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2607 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/protocols.py
--rw-r--r--   0        0        0     1820 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/serialization.py
--rw-r--r--   0        0        0     1906 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/compat.py
--rw-r--r--   0        0        0     3578 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     1483 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/path.py
--rw-r--r--   0        0        0    10434 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2720 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/scope.py
--rw-r--r--   0        0        0     1003 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/sequence.py
--rw-r--r--   0        0        0    13407 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/signature.py
--rw-r--r--   0        0        0     5337 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/sync.py
--rw-r--r--   0        0        0     6405 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/version.py
--rw-r--r--   0        0        0     9638 2023-04-26 13:40:53.145600 litestar-2.0.0a5/pyproject.toml
--rw-r--r--   0        0        0    52838 1970-01-01 00:00:00.000000 litestar-2.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-09 15:45:08.809052 litestar-2.0.0a6/LICENSE
+-rw-r--r--   0        0        0    50573 2023-05-09 15:45:08.809052 litestar-2.0.0a6/README.md
+-rw-r--r--   0        0        0      744 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/__init__.py
+-rw-r--r--   0        0        0      103 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     8651 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5938 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3868 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4239 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14907 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20450 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2759 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     5935 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0    10117 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5525 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1476 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    10196 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     7074 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2104 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    31705 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10970 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5240 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1464 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2338 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_parsers.py
+-rw-r--r--   0        0        0      182 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0     5995 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/field.py
+-rw-r--r--   0        0        0       64 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/__init__.py
+-rw-r--r--   0        0        0    13197 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/attrs_signature_model.py
+-rw-r--r--   0        0        0     3736 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/base.py
+-rw-r--r--   0        0        0     6680 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/models/pydantic_signature_model.py
+-rw-r--r--   0        0        0     6510 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    35419 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/background_tasks.py
+-rw-r--r--   0        0        0      176 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/_redis_flushall_streams.lua
+-rw-r--r--   0        0        0      101 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/_redis_pubsub_publish.lua
+-rw-r--r--   0        0        0      401 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/_redis_xadd_expire.lua
+-rw-r--r--   0        0        0     1300 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/base.py
+-rw-r--r--   0        0        0     2768 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/memory.py
+-rw-r--r--   0        0        0     9208 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/backends/redis.py
+-rw-r--r--   0        0        0    15678 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/plugin.py
+-rw-r--r--   0        0        0     4647 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/channels/subscriber.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.833052 litestar-2.0.0a6/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    11640 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4571 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2365 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2224 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0     1210 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12358 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/compression.py
+-rw-r--r--   0        0        0     5177 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/csrf.py
+-rw-r--r--   0        0        0     1991 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10821 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/base.py
+-rw-r--r--   0        0        0     7698 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/request.py
+-rw-r--r--   0        0        0    11256 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1098 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4051 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     8324 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28722 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     3978 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6970 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3916 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/mako.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/msgspec/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4206 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2206 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0     9259 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/abc.py
+-rw-r--r--   0        0        0      328 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     1785 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0      641 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    13409 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4324 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0     3431 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      742 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     3602 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11308 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11500 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     2849 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1600 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1447 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0    21855 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/repository.py
+-rw-r--r--   0        0        0     1856 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9559 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/controller.py
+-rw-r--r--   0        0        0    16460 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3757 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17316 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9302 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     3360 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     2386 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/di.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/exceptions.py
+-rw-r--r--   0        0        0      188 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0      245 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/__init__.py
+-rw-r--r--   0        0        0    14863 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/abc.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/__init__.py
+-rw-r--r--   0        0        0     1282 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/backend.py
+-rw-r--r--   0        0        0     1836 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/utils.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/__init__.py
+-rw-r--r--   0        0        0     1242 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/backend.py
+-rw-r--r--   0        0        0     1681 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/utils.py
+-rw-r--r--   0        0        0     3161 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/types.py
+-rw-r--r--   0        0        0    10354 2023-05-09 15:45:08.837052 litestar-2.0.0a6/litestar/dto/factory/_backends/utils.py
+-rw-r--r--   0        0        0     7508 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/abc.py
+-rw-r--r--   0        0        0     1193 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/config.py
+-rw-r--r--   0        0        0      313 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/exc.py
+-rw-r--r--   0        0        0     1269 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/field.py
+-rw-r--r--   0        0        0       65 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/stdlib/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0     1088 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/types.py
+-rw-r--r--   0        0        0     1594 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/factory/utils.py
+-rw-r--r--   0        0        0     4465 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/interface.py
+-rw-r--r--   0        0        0      309 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4597 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1305 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/events/listener.py
+-rw-r--r--   0        0        0     1142 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1621 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5330 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3877 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    20202 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     8104 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    25662 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    60867 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6415 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    15216 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3619 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12050 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     2967 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8359 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2565 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6466 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7191 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     8990 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13372 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10811 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7935 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10365 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8558 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      231 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/config.py
+-rw-r--r--   0        0        0    16443 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-05-09 15:45:08.841052 litestar-2.0.0a6/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4218 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    10984 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/pagination.py
+-rw-r--r--   0        0        0    16805 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/params.py
+-rw-r--r--   0        0        0     7100 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/partial.py
+-rw-r--r--   0        0        0     3926 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/py.typed
+-rw-r--r--   0        0        0      278 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/__init__.py
+-rw-r--r--   0        0        0    12173 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/base.py
+-rw-r--r--   0        0        0     9225 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/file.py
+-rw-r--r--   0        0        0     2952 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/redirect.py
+-rw-r--r--   0        0        0     4883 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/streaming.py
+-rw-r--r--   0        0        0     2994 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response/template.py
+-rw-r--r--   0        0        0    14975 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/response_containers.py
+-rw-r--r--   0        0        0    15028 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1757 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6437 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/base.py
+-rw-r--r--   0        0        0    13254 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/http.py
+-rw-r--r--   0        0        0     3052 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4933 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     7355 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/serialization.py
+-rw-r--r--   0        0        0      158 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5019 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3598 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4377 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/base.py
+-rw-r--r--   0        0        0     5425 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4113 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17445 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5132 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19555 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    31473 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2532 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21905 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8086 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/transport.py
+-rw-r--r--   0        0        0     8527 2023-05-09 15:45:08.845052 litestar-2.0.0a6/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4105 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8697 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      453 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2291 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1645 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      183 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/empty.py
+-rw-r--r--   0        0        0     2662 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/file_types.py
+-rw-r--r--   0        0        0      344 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1720 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2607 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/protocols.py
+-rw-r--r--   0        0        0     1820 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/types/serialization.py
+-rw-r--r--   0        0        0     1906 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3578 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     1732 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/path.py
+-rw-r--r--   0        0        0    10434 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2720 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/scope.py
+-rw-r--r--   0        0        0     1003 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/sequence.py
+-rw-r--r--   0        0        0    13743 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/signature.py
+-rw-r--r--   0        0        0     5337 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/sync.py
+-rw-r--r--   0        0        0     6405 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-05-09 15:45:08.849052 litestar-2.0.0a6/litestar/utils/version.py
+-rw-r--r--   0        0        0     9810 2023-05-09 15:45:08.849052 litestar-2.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0    54208 1970-01-01 00:00:00.000000 litestar-2.0.0a6/PKG-INFO
```

### Comparing `litestar-2.0.0a5/LICENSE` & `litestar-2.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/README.md` & `litestar-2.0.0a6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-97-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-100-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -401,17 +401,22 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/giorgiovilardo"><img src="https://avatars.githubusercontent.com/u/56472600?v=4?s=100" width="100px;" alt="Giorgio Vilardo"/><br /><sub><b>Giorgio Vilardo</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=giorgiovilardo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt="Nicholas Bollweg"/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=bollwyvl" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/khiem-doan/"><img src="https://avatars.githubusercontent.com/u/15646249?v=4?s=100" width="100px;" alt="Khiem Doan"/><br /><sub><b>Khiem Doan</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=khiemdoan" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kedod"><img src="https://avatars.githubusercontent.com/u/35638715?v=4?s=100" width="100px;" alt="kedod"/><br /><sub><b>kedod</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=kedod" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a> <a href="#infra-sonpro1296" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://patrickarmengol.com"><img src="https://avatars.githubusercontent.com/u/42473149?v=4?s=100" width="100px;" alt="Patrick Armengol"/><br /><sub><b>Patrick Armengol</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=patrickarmengol" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/erhuabushuo"><img src="https://avatars.githubusercontent.com/u/1642364?v=4?s=100" width="100px;" alt="疯人院主任"/><br /><sub><b>疯人院主任</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=erhuabushuo" title="Documentation">📖</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviral-nayya"><img src="https://avatars.githubusercontent.com/u/121891493?v=4?s=100" width="100px;" alt="aviral-nayya"/><br /><sub><b>aviral-nayya</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=aviral-nayya" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/whiskeyriver"><img src="https://avatars.githubusercontent.com/u/162092?v=4?s=100" width="100px;" alt="whiskeyriver"/><br /><sub><b>whiskeyriver</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=whiskeyriver" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.0.0a5/litestar/__init__.py` & `litestar-2.0.0a6/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_asgi/asgi_router.py` & `litestar-2.0.0a6/litestar/_asgi/asgi_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             handler: sync or async callable that may or may not have an argument.
         """
         async_callable = AsyncCallable(handler)  # type: ignore
 
         if async_callable.num_expected_args > 0:
             await async_callable(self.app.state)  # type: ignore[arg-type]
         else:
-            await async_callable()
+            await async_callable()  # pyright: ignore
 
     def construct_routing_trie(self) -> None:
         """Create a map of the app's routes.
 
         This map is used in the asgi router to route requests.
         """
         new_routes = [route for route in self.app.routes if route not in self._registered_routes]
```

### Comparing `litestar-2.0.0a5/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0a6/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0a6/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0a6/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0a6/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_asgi/utils.py` & `litestar-2.0.0a6/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_kwargs/cleanup.py` & `litestar-2.0.0a6/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_kwargs/dependencies.py` & `litestar-2.0.0a6/litestar/_kwargs/dependencies.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_kwargs/extractors.py` & `litestar-2.0.0a6/litestar/_kwargs/extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0a6/litestar/_kwargs/kwargs_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0a6/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_layers/utils.py` & `litestar-2.0.0a6/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_multipart.py` & `litestar-2.0.0a6/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/parameters.py` & `litestar-2.0.0a6/litestar/_openapi/parameters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/path_item.py` & `litestar-2.0.0a6/litestar/_openapi/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/request_body.py` & `litestar-2.0.0a6/litestar/_openapi/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/responses.py` & `litestar-2.0.0a6/litestar/_openapi/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0a6/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0a6/litestar/_openapi/schema_generation/examples.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0a6/litestar/_openapi/schema_generation/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0a6/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0a6/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0a6/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0a6/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_openapi/utils.py` & `litestar-2.0.0a6/litestar/_openapi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_parsers.py` & `litestar-2.0.0a6/litestar/_parsers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_signature/field.py` & `litestar-2.0.0a6/litestar/_signature/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_signature/models/attrs_signature_model.py` & `litestar-2.0.0a6/litestar/_signature/models/attrs_signature_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 
 def _structure_timedelta(value: Any, cls: type[timedelta]) -> timedelta:
     if isinstance(value, timedelta):
         return value
     if isinstance(value, (float, int, Decimal)):
         return cls(seconds=int(value))
-    return cls(seconds=timeparse(value))
+    return cls(seconds=timeparse(value))  # pyright: ignore
 
 
 def _structure_decimal(value: Any, cls: type[Decimal]) -> Decimal:
     return cls(str(value))
 
 
 def _structure_path(value: Any, cls: type[PurePath]) -> PurePath:
```

### Comparing `litestar-2.0.0a5/litestar/_signature/models/base.py` & `litestar-2.0.0a6/litestar/_signature/models/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_signature/models/pydantic_signature_model.py` & `litestar-2.0.0a6/litestar/_signature/models/pydantic_signature_model.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/_signature/utils.py` & `litestar-2.0.0a6/litestar/_signature/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/app.py` & `litestar-2.0.0a6/litestar/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/background_tasks.py` & `litestar-2.0.0a6/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/cli/_utils.py` & `litestar-2.0.0a6/litestar/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/cli/commands/core.py` & `litestar-2.0.0a6/litestar/cli/commands/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,15 @@
     process_args = {
         "reload": env.reload or reload,
         "host": env.host or host,
         "port": env.port or port,
         "workers": env.web_concurrency or web_concurrency,
         "factory": env.is_app_factory,
     }
-
-    subprocess.run(["uvicorn", env.app_path, *_convert_uvicorn_args(process_args)], check=True)
+    subprocess.run(["uvicorn", env.app_path, *_convert_uvicorn_args(process_args)], check=True)  # noqa: S603 S607
 
 
 @command(name="routes")
 def routes_command(app: Litestar) -> None:  # pragma: no cover
     """Display information about the application's routes."""
 
     tree = Tree("", hide_root=True)
```

### Comparing `litestar-2.0.0a5/litestar/cli/commands/schema.py` & `litestar-2.0.0a6/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/cli/commands/sessions.py` & `litestar-2.0.0a6/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/config/allowed_hosts.py` & `litestar-2.0.0a6/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/config/app.py` & `litestar-2.0.0a6/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/config/compression.py` & `litestar-2.0.0a6/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/config/cors.py` & `litestar-2.0.0a6/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/config/csrf.py` & `litestar-2.0.0a6/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/config/response_cache.py` & `litestar-2.0.0a6/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/connection/__init__.py` & `litestar-2.0.0a6/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/connection/base.py` & `litestar-2.0.0a6/litestar/connection/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         the session data to be cleared.
 
         Returns:
             None.
         """
         self.scope["session"] = Empty
 
-    def url_for(self, name: str, **path_parameters: dict[str, Any]) -> str:
+    def url_for(self, name: str, **path_parameters: Any) -> str:
         """Return the url for a given route handler name.
 
         Args:
             name: The ``name`` of the request route handler.
             **path_parameters: Values for path parameters in the route
 
         Raises:
```

### Comparing `litestar-2.0.0a5/litestar/connection/request.py` & `litestar-2.0.0a6/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/connection/websocket.py` & `litestar-2.0.0a6/litestar/connection/websocket.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Generic, Literal, cast, overload
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Generic, Literal, cast, overload
 
 from litestar.connection.base import (
     ASGIConnection,
     AuthT,
     StateT,
     UserT,
     empty_receive,
     empty_send,
 )
 from litestar.datastructures.headers import Headers
 from litestar.exceptions import WebSocketDisconnect, WebSocketException
-from litestar.serialization import decode_json, default_serializer, encode_json
+from litestar.serialization import decode_json, decode_msgpack, default_serializer, encode_json, encode_msgpack
 from litestar.status_codes import WS_1000_NORMAL_CLOSURE
 
 __all__ = ("WebSocket",)
 
 
 if TYPE_CHECKING:
     from litestar.handlers.websocket_handlers import WebsocketRouteHandler  # noqa: F401
@@ -25,14 +25,15 @@
         Receive,
         ReceiveMessage,
         Scope,
         Send,
         WebSocketAcceptEvent,
         WebSocketCloseEvent,
         WebSocketDisconnectEvent,
+        WebSocketMode,
         WebSocketReceiveEvent,
         WebSocketSendEvent,
     )
 
 DISCONNECT_MESSAGE = "connection is disconnected"
 
 
@@ -148,15 +149,15 @@
     async def receive_data(self, mode: Literal["text"]) -> str:
         ...
 
     @overload
     async def receive_data(self, mode: Literal["binary"]) -> bytes:
         ...
 
-    async def receive_data(self, mode: Literal["binary", "text"]) -> str | bytes:
+    async def receive_data(self, mode: WebSocketMode) -> str | bytes:
         """Receive an 'websocket.receive' event and returns the data stored on it.
 
         Args:
             mode: The respective event key to use.
 
         Returns:
             The event's data.
@@ -166,14 +167,34 @@
         event = cast("WebSocketReceiveEvent | WebSocketDisconnectEvent", await self.receive())
         if event["type"] == "websocket.disconnect":
             raise WebSocketDisconnect(detail="disconnect event", code=event["code"])
         if self.connection_state == "disconnect":
             raise WebSocketDisconnect(detail=DISCONNECT_MESSAGE)  # pragma: no cover
         return event.get("text") or "" if mode == "text" else event.get("bytes") or b""
 
+    @overload
+    def iter_data(self, mode: Literal["text"]) -> AsyncGenerator[str, None]:
+        ...
+
+    @overload
+    def iter_data(self, mode: Literal["binary"]) -> AsyncGenerator[bytes, None]:
+        ...
+
+    async def iter_data(self, mode: WebSocketMode) -> AsyncGenerator[str | bytes, None]:
+        """Continuously receive data and yield it
+
+        Args:
+            mode: Socket mode to use. Either ``text`` or ``binary``
+        """
+        try:
+            while True:
+                yield await self.receive_data(mode)
+        except WebSocketDisconnect:
+            pass
+
     async def receive_text(self) -> str:
         """Receive data as text.
 
         Returns:
             A string.
         """
         return await self.receive_data(mode="text")
@@ -182,32 +203,59 @@
         """Receive data as bytes.
 
         Returns:
             A byte-string.
         """
         return await self.receive_data(mode="binary")
 
-    async def receive_json(
-        self,
-        mode: Literal["text", "binary"] = "text",
-    ) -> Any:
-        """Receive data and loads it into JSON using orson.
+    async def receive_json(self, mode: WebSocketMode = "text") -> Any:
+        """Receive data and decode it as JSON.
 
         Args:
             mode: Either ``text`` or ``binary``.
 
         Returns:
             An arbitrary value
         """
         data = await self.receive_data(mode=mode)
         return decode_json(data)
 
-    async def send_data(
-        self, data: str | bytes, mode: Literal["text", "binary"] = "text", encoding: str = "utf-8"
-    ) -> None:
+    async def receive_msgpack(self) -> Any:
+        """Receive data and decode it as MessagePack.
+
+        Note that since MessagePack is a binary format, this method will always receive
+        data in ``binary`` mode.
+
+        Returns:
+            An arbitrary value
+        """
+        data = await self.receive_data(mode="binary")
+        return decode_msgpack(data)
+
+    async def iter_json(self, mode: WebSocketMode) -> AsyncGenerator[Any, None]:
+        """Continuously receive data and yield it, decoding it as JSON in the process.
+
+        Args:
+            mode: Socket mode to use. Either ``text`` or ``binary``
+        """
+        async for data in self.iter_data(mode):
+            yield decode_json(data)
+
+    async def iter_msgpack(self) -> AsyncGenerator[Any, None]:
+        """Continuously receive data and yield it, decoding it as MessagePack in the
+        process.
+
+        Note that since MessagePack is a binary format, this method will always receive
+        data in ``binary`` mode.
+
+        """
+        async for data in self.iter_data(mode="binary"):
+            yield decode_msgpack(data)
+
+    async def send_data(self, data: str | bytes, mode: WebSocketMode = "text", encoding: str = "utf-8") -> None:
         """Send a 'websocket.send' event.
 
         Args:
             data: Data to send.
             mode: The respective event key to use.
             encoding: Encoding to use when converting bytes / str.
 
@@ -262,27 +310,44 @@
             None
         """
         await self.send_data(data=data, mode="binary", encoding=encoding)
 
     async def send_json(
         self,
         data: Any,
-        mode: Literal["text", "binary"] = "text",
+        mode: WebSocketMode = "text",
         encoding: str = "utf-8",
         serializer: Serializer = default_serializer,
     ) -> None:
         """Send data as JSON.
 
         Args:
             data: A value to serialize.
             mode: Either ``text`` or ``binary``.
             encoding: Encoding to use for binary data.
             serializer: A serializer function.
 
         Returns:
             None
         """
-        await self.send_data(
-            data=encode_json(data, serializer),
-            mode=mode,
-            encoding=encoding,
-        )
+        await self.send_data(data=encode_json(data, serializer), mode=mode, encoding=encoding)
+
+    async def send_msgpack(
+        self,
+        data: Any,
+        encoding: str = "utf-8",
+        serializer: Serializer = default_serializer,
+    ) -> None:
+        """Send data as MessagePack.
+
+        Note that since MessagePack is a binary format, this method will always send
+        data in ``binary`` mode.
+
+        Args:
+            data: A value to serialize.
+            encoding: Encoding to use for binary data.
+            serializer: A serializer function.
+
+        Returns:
+            None
+        """
+        await self.send_data(data=encode_msgpack(data, serializer), mode="binary", encoding=encoding)
```

### Comparing `litestar-2.0.0a5/litestar/constants.py` & `litestar-2.0.0a6/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0a6/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/htmx/request.py` & `litestar-2.0.0a6/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/htmx/response.py` & `litestar-2.0.0a6/litestar/contrib/htmx/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/htmx/types.py` & `litestar-2.0.0a6/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/jinja.py` & `litestar-2.0.0a6/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0a6/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0a6/litestar/contrib/jwt/jwt_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
         return Components(
             security_schemes={
                 self.openapi_security_scheme_name: SecurityScheme(
                     type="oauth2",
                     scheme="Bearer",
                     name=self.auth_header,
                     security_scheme_in="header",
-                    flows=OAuthFlows(password=self.oauth_flow),  # pyright: reportGeneralTypeIssues=false
+                    flows=OAuthFlows(password=self.oauth_flow),  # pyright: ignore[reportGeneralTypeIssues]
                     bearer_format="JWT",
                     description=self.description,
                 )
             }
         )
 
     def login(
```

### Comparing `litestar-2.0.0a5/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0a6/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0a6/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/mako.py` & `litestar-2.0.0a6/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0a6/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0a6/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0a6/litestar/contrib/opentelemetry/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/repository/abc.py` & `litestar-2.0.0a6/litestar/contrib/repository/abc.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/repository/filters.py` & `litestar-2.0.0a6/litestar/contrib/repository/filters.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0a6/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,33 @@
 from sqlalchemy.orm import (
     DeclarativeBase,
     Mapped,
     Session,
     declarative_mixin,
     declared_attr,
     mapped_column,
+    orm_insert_sentinel,
     registry,
 )
 
 from .types import GUID, JSON
 
 if TYPE_CHECKING:
     from sqlalchemy.sql import FromClause
 
-__all__ = ("AuditBase", "AuditColumns", "Base", "CommonTableAttributes", "UUIDPrimaryKey", "touch_updated_timestamp")
+__all__ = (
+    "AuditBase",
+    "AuditColumns",
+    "Base",
+    "CommonTableAttributes",
+    "create_registry",
+    "ModelProtocol",
+    "touch_updated_timestamp",
+    "UUIDPrimaryKey",
+)
 
 
 BaseT = TypeVar("BaseT", bound="Base")
 
 convention = {
     "ix": "ix_%(column_0_label)s",
     "uq": "uq_%(table_name)s_%(column_0_name)s",
@@ -111,26 +121,35 @@
 
     def to_dict(self, exclude: set[str] | None = None) -> dict[str, Any]:
         """Convert model to dictionary.
 
         Returns:
             dict[str, Any]: A dict representation of the model
         """
-        exclude = set(exclude) if exclude else set()
+        exclude = exclude.union("_sentinel") if exclude else {"_sentinel"}
         return {field.name: getattr(self, field.name) for field in self.__table__.columns if field.name not in exclude}
 
+    @declared_attr
+    def _sentinel(cls) -> Mapped[int]:
+        return orm_insert_sentinel()
 
-meta = MetaData(naming_convention=convention)
-orm_registry = registry(
-    metadata=meta,
-    type_annotation_map={UUID: GUID, EmailStr: String, AnyUrl: String, AnyHttpUrl: String, dict: JSON},
-)
+
+def create_registry() -> registry:
+    """Create a new SQLAlchemy registry."""
+    meta = MetaData(naming_convention=convention)
+    return registry(
+        metadata=meta,
+        type_annotation_map={UUID: GUID, EmailStr: String, AnyUrl: String, AnyHttpUrl: String, dict: JSON},
+    )
+
+
+orm_registry = create_registry()
 
 
-class Base(CommonTableAttributes, UUIDPrimaryKey, DeclarativeBase):
+class Base(UUIDPrimaryKey, CommonTableAttributes, DeclarativeBase):
     """Base for all SQLAlchemy declarative models."""
 
     registry = orm_registry
 
 
 class AuditBase(CommonTableAttributes, UUIDPrimaryKey, AuditColumns, DeclarativeBase):
     """Base for declarative models with audit columns."""
```

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/dto.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/dto.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 from sqlalchemy.orm import DeclarativeBase, Mapped
 
 from litestar.dto.factory.abc import AbstractDTOFactory
 from litestar.dto.factory.field import DTO_FIELD_META_KEY
 from litestar.dto.factory.types import FieldDefinition
 from litestar.dto.factory.utils import get_model_type_hints
 from litestar.types.empty import Empty
+from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
     from typing import Any, ClassVar, Collection, Generator
 
     from sqlalchemy import Column
     from sqlalchemy.orm import RelationshipProperty
     from typing_extensions import TypeAlias
 
+    from litestar.utils.signature import ParsedType
+
 
 __all__ = ("SQLAlchemyDTO", "DataT")
 
 DataT = TypeVar("DataT", bound="DeclarativeBase | Collection[DeclarativeBase]")
 AnyDeclarativeT = TypeVar("AnyDeclarativeT", bound="DeclarativeBase")
 ElementType: TypeAlias = "Column[Any] | RelationshipProperty[Any]"
 
@@ -59,28 +62,27 @@
 
             field_def = FieldDefinition(
                 name=key,
                 default=default,
                 parsed_type=parsed_type,
                 default_factory=default_factory,
                 dto_field=elem.info.get(DTO_FIELD_META_KEY),
+                unique_model_name=get_fully_qualified_class_name(model_type),
             )
 
             yield field_def
 
     @classmethod
-    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
-        if field_definition.parsed_type.inner_types:
-            return any(inner.is_subclass_of(DeclarativeBase) for inner in field_definition.parsed_type.inner_types)
-        return field_definition.parsed_type.is_subclass_of(DeclarativeBase)
+    def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
+        return parsed_type.is_subclass_of(DeclarativeBase)
 
 
 def _detect_defaults(elem: ElementType) -> tuple[Any, Any]:
     default: Any = Empty
-    default_factory: Any = Empty  # pyright:ignore
+    default_factory: Any = None  # pyright:ignore
     if sqla_default := getattr(elem, "default", None):
         if sqla_default.is_scalar:
             default = sqla_default.arg
         elif sqla_default.is_callable:
 
             def default_factory(d: Any = sqla_default) -> Any:
                 return d.arg({})
```

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/__init__.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/common.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/engine.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/sync.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/plugin.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/serialization.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/plugins/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/repository.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,15 @@
         """
         data_to_update: list[dict[str, Any]] = [v.to_dict() if isinstance(v, self.model_type) else v for v in data]  # type: ignore
         with wrap_sqlalchemy_exception():
             if self.session.bind.dialect.update_executemany_returning:
                 instances = list(
                     await self.session.scalars(  # type: ignore
                         update(self.model_type).returning(self.model_type),
-                        data_to_update,  # pyright: reportGeneralTypeIssues=false
+                        data_to_update,  # pyright: ignore[reportGeneralTypeIssues]
                     )
                 )
                 await self.session.flush()
                 for instance in instances:
                     self.session.expunge(instance)
                 return instances
             await self.session.execute(
```

### Comparing `litestar-2.0.0a5/litestar/contrib/sqlalchemy/types.py` & `litestar-2.0.0a6/litestar/contrib/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/controller.py` & `litestar-2.0.0a6/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/data_extractors.py` & `litestar-2.0.0a6/litestar/data_extractors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/__init__.py` & `litestar-2.0.0a6/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/cookie.py` & `litestar-2.0.0a6/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/headers.py` & `litestar-2.0.0a6/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0a6/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/response_header.py` & `litestar-2.0.0a6/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/state.py` & `litestar-2.0.0a6/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/upload_file.py` & `litestar-2.0.0a6/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/datastructures/url.py` & `litestar-2.0.0a6/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/di.py` & `litestar-2.0.0a6/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/dto/factory/abc.py` & `litestar-2.0.0a6/litestar/dto/factory/_backends/abc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,296 +1,390 @@
+"""DTO backends do the heavy lifting of decoding and validating raw bytes into domain models, and
+back again, to bytes.
+"""
 from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
+from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Generic, TypeVar
 
-from litestar.dto.factory.backends import MsgspecDTOBackend, PydanticDTOBackend
-from litestar.dto.factory.backends.abc import BackendContext
-from litestar.dto.interface import ConnectionContext, DTOInterface
-from litestar.enums import RequestEncodingType
-from litestar.types.builtin_types import NoneType
-from litestar.utils.signature import ParsedType
-
-from .config import DTOConfig
-from .exc import InvalidAnnotation
-from .field import Mark
-from .types import FieldDefinition, FieldDefinitionsType, NestedFieldDefinition
-from .utils import parse_configs_from_annotation
+from litestar._openapi.schema_generation import create_schema
+from litestar._signature.field import SignatureField
+from litestar.utils.helpers import get_fully_qualified_class_name
+
+from .types import (
+    CollectionType,
+    CompositeType,
+    MappingType,
+    NestedFieldInfo,
+    SimpleType,
+    TransferFieldDefinition,
+    TupleType,
+    UnionType,
+)
+from .utils import (
+    RenameStrategies,
+    build_annotation_for_backend,
+    should_exclude_field,
+    transfer_data,
+)
 
 if TYPE_CHECKING:
-    from typing import Any, ClassVar, Collection, Generator
+    from typing import AbstractSet, Any, Callable, Final, Generator
 
-    from typing_extensions import Self
-
-    from litestar.dto.interface import HandlerContext
+    from litestar.dto.factory import DTOConfig
+    from litestar.dto.factory.types import FieldDefinition
+    from litestar.dto.interface import ConnectionContext
     from litestar.dto.types import ForType
     from litestar.openapi.spec import Reference, Schema
     from litestar.types.serialization import LitestarEncodableType
+    from litestar.utils.signature import ParsedType
+
+    from .types import FieldDefinitionsType
+
+__all__ = ("AbstractDTOBackend", "BackendContext")
+
+BackendT = TypeVar("BackendT")
+
+
+class BackendContext:
+    """Context required by DTO backends to perform their work."""
 
-    from .backends import AbstractDTOBackend
+    __slots__ = (
+        "config",
+        "dto_for",
+        "field_definition_generator",
+        "is_nested_field_predicate",
+        "model_type",
+        "parsed_type",
+    )
 
-__all__ = ["AbstractDTOFactory"]
+    def __init__(
+        self,
+        dto_config: DTOConfig,
+        dto_for: ForType,
+        parsed_type: ParsedType,
+        field_definition_generator: Callable[[Any], Generator[FieldDefinition, None, None]],
+        is_nested_field_predicate: Callable[[ParsedType], bool],
+        model_type: type[Any],
+    ) -> None:
+        """Create a backend context.
 
-DataT = TypeVar("DataT")
+        Args:
+            dto_config: DTO config.
+            dto_for: "data" or "return"
+            parsed_type: Parsed type.
+            field_definition_generator: Generator that produces
+                :class:`FieldDefinition <.dto.factory.types.FieldDefinition>` instances given ``model_type``.
+            is_nested_field_predicate: Function that detects if a field is nested.
+            model_type: Model type.
+        """
+        self.config: Final[DTOConfig] = dto_config
+        self.dto_for: Final[ForType] = dto_for
+        self.parsed_type: Final[ParsedType] = parsed_type
+        self.field_definition_generator: Final[
+            Callable[[Any], Generator[FieldDefinition, None, None]]
+        ] = field_definition_generator
+        self.is_nested_field_predicate: Final[Callable[[ParsedType], bool]] = is_nested_field_predicate
+        self.model_type: Final[type[Any]] = model_type
 
 
-class AbstractDTOFactory(DTOInterface, Generic[DataT], metaclass=ABCMeta):
-    """Base class for DTO types."""
+class NestedDepthExceededError(Exception):
+    """Raised when a nested type exceeds the maximum allowed depth.
 
-    __slots__ = ("connection_context",)
+    Not an exception that is intended to be raised into userland, rather a signal to the process that is iterating over
+    the field definitions that the current field should be skipped.
+    """
 
-    config: ClassVar[DTOConfig]
-    """Config objects to define properties of the DTO."""
-    model_type: ClassVar[type[Any]]
-    """If ``annotation`` is an iterable, this is the inner type, otherwise will be the same as ``annotation``."""
 
-    _reverse_field_mappings: ClassVar[dict[str, FieldDefinition]]
-    _type_backend_map: ClassVar[dict[tuple[ForType, ParsedType, RequestEncodingType | str | None], AbstractDTOBackend]]
-    _handler_backend_map: ClassVar[dict[tuple[ForType, str], AbstractDTOBackend]]
+class AbstractDTOBackend(ABC, Generic[BackendT]):
+    __slots__ = (
+        "annotation",
+        "context",
+        "parsed_field_definitions",
+        "reverse_name_map",
+        "transfer_model_type",
+    )
 
-    def __init__(self, connection_context: ConnectionContext) -> None:
-        """Create an AbstractDTOFactory type.
+    def __init__(self, context: BackendContext) -> None:
+        """Create dto backend instance.
 
         Args:
-            connection_context: A :class:`ConnectionContext <.ConnectionContext>` instance, which provides
-                information about the connection.
+            context: context of the type represented by this backend.
         """
-        self.connection_context = connection_context
+        self.context = context
+        self.parsed_field_definitions = self.parse_model(context.model_type, context.config.exclude)
+        self.transfer_model_type = self.create_transfer_model_type(
+            get_fully_qualified_class_name(context.model_type), self.parsed_field_definitions
+        )
+        self.annotation = build_annotation_for_backend(context.parsed_type.annotation, self.transfer_model_type)
+
+    def parse_model(
+        self,
+        model_type: Any,
+        exclude: AbstractSet[str],
+        nested_depth: int = 0,
+    ) -> FieldDefinitionsType:
+        """Reduce :attr:`model_type` to :class:`FieldDefinitionsType`.
+
+        .. important::
+            Implementations must respect the :attr:`config` object. For example:
+                - fields marked private must never be included in the field definitions.
+                - if a ``purpose`` is declared, then read-only fields must be taken into account.
+                - field renaming must be implemented.
+                - additional fields must be included, subject to ``purpose``.
+                - nested depth and nested recursion depth must be adhered to.
 
-    def __class_getitem__(cls, annotation: Any) -> type[Self]:
-        parsed_type = ParsedType(annotation)
-
-        if (parsed_type.is_optional and len(parsed_type.args) > 2) or (
-            parsed_type.is_union and not parsed_type.is_optional
-        ):
-            raise InvalidAnnotation(
-                "Unions are currently not supported as type argument to DTO. Want this? Open an issue."
-            )
+        Returns:
+            Fields for data transfer.
 
-        if parsed_type.is_forward_ref:
-            raise InvalidAnnotation("Forward references are not supported as type argument to DTO")
+            Key is the name of the new field, and value is a tuple of type and default value pairs.
 
-        # if a configuration is not provided, and the type narrowing is a type var, we don't want to create a subclass
-        configs = parse_configs_from_annotation(parsed_type)
-        if parsed_type.is_type_var and not configs:
-            return cls
-
-        if configs:
-            # provided config is always preferred
-            config = configs[0]
-        elif hasattr(cls, "config"):
-            # if no config is provided, but the class has one assigned, use that
-            config = cls.config
-        else:
-            # otherwise, create a new config
-            config = DTOConfig()
-
-        cls_dict: dict[str, Any] = {
-            "config": config,
-            "_reverse_field_mappings": {},
-            "_type_backend_map": {},
-            "_handler_backend_map": {},
-        }
-        if not parsed_type.is_type_var:
-            cls_dict.update(model_type=parsed_type.annotation)
-
-        return type(f"{cls.__name__}[{annotation}]", (cls,), cls_dict)
-
-    def builtins_to_data_type(self, builtins: Any) -> Any:
-        """Coerce the unstructured data into the data type."""
-        backend = self._handler_backend_map[("data", self.connection_context.handler_id)]
-        return backend.populate_data_from_builtins(builtins)
-
-    def bytes_to_data_type(self, raw: bytes) -> Any:
-        """Return the data held by the DTO."""
-        backend = self._handler_backend_map[("data", self.connection_context.handler_id)]
-        return backend.populate_data_from_raw(raw, self.connection_context)
-
-    def data_to_encodable_type(self, data: DataT | Collection[DataT]) -> LitestarEncodableType:
-        backend = self._handler_backend_map[("return", self.connection_context.handler_id)]
-        return backend.encode_data(data, self.connection_context)
+            Add a new field called "new_field", that is a string, and required:
+            {"new_field": (str, ...)}
 
-    @classmethod
-    @abstractmethod
-    def generate_field_definitions(cls, model_type: type[Any]) -> Generator[FieldDefinition, None, None]:
-        """Generate ``FieldDefinition`` instances from ``model_type``.
+            Add a new field called "new_field", that is a string, and not-required:
+            {"new_field": (str, "default")}
 
-        Yields:
-            ``FieldDefinition`` instances.
+            Add a new field called "new_field", that may be `None`:
+            {"new_field": (str | None, None)}
         """
+        defined_fields = []
+        for field_definition in self.context.field_definition_generator(model_type):
+            if should_exclude_field(field_definition, exclude, self.context.dto_for):
+                continue
+
+            try:
+                transfer_type = self._create_transfer_type(
+                    field_definition.parsed_type,
+                    exclude,
+                    field_definition.name,
+                    field_definition.unique_name(),
+                    nested_depth,
+                )
+            except NestedDepthExceededError:
+                continue
+
+            if rename := self.context.config.rename_fields.get(field_definition.name):
+                serialization_name = rename
+            elif self.context.config.rename_strategy:
+                serialization_name = RenameStrategies(self.context.config.rename_strategy)(field_definition.name)
+            else:
+                serialization_name = field_definition.name
+
+            transfer_field_definition = TransferFieldDefinition.from_field_definition(
+                field_definition=field_definition,
+                serialization_name=serialization_name,
+                transfer_type=transfer_type,
+            )
+            defined_fields.append(transfer_field_definition)
+        return tuple(defined_fields)
 
-    @classmethod
     @abstractmethod
-    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
-        """Return ``True`` if ``field_definition`` represents a nested model field.
+    def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[BackendT]:
+        """Create a model for data transfer.
 
         Args:
-            field_definition: inspect type to determine if field definition represents a nested model.
+            unique_name: name for the type that should be unique across all transfer types.
+            field_definitions: field definitions for the container type.
 
         Returns:
-            ``True`` if ``field_definition`` represents a nested model field.
+            A ``BackendT`` class.
         """
 
-    @classmethod
-    def on_registration(cls, handler_context: HandlerContext) -> None:
-        """Called each time the DTO type is encountered during signature modelling.
+    @abstractmethod
+    def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
+        """Parse raw bytes into transfer model type.
 
         Args:
-            handler_context: A :class:`HandlerContext <.HandlerContext>` instance. Provides information about the
-                handler and application of the DTO.
-        """
+            raw: bytes
+            connection_context: Information about the active connection.
 
-        if handler_context.parsed_type.is_collection:
-            if len(handler_context.parsed_type.inner_types) != 1:
-                raise InvalidAnnotation("AbstractDTOFactory only supports homogeneous collection types")
-            handler_type = handler_context.parsed_type.inner_types[0]
-        else:
-            handler_type = handler_context.parsed_type
-
-        if not handler_type.is_subclass_of(cls.model_type):
-            raise InvalidAnnotation(
-                f"DTO narrowed with '{cls.model_type}', handler type is '{handler_context.parsed_type.annotation}'"
-            )
-
-        key = (handler_context.dto_for, handler_context.parsed_type, handler_context.request_encoding_type)
-        backend = cls._type_backend_map.get(key)
-        if backend is None:
-            backend_type: type[AbstractDTOBackend]
-            if handler_context.request_encoding_type in {
-                RequestEncodingType.URL_ENCODED,
-                RequestEncodingType.MULTI_PART,
-            }:
-                backend_type = PydanticDTOBackend
-            else:
-                backend_type = MsgspecDTOBackend
+        Returns:
+            The raw bytes parsed into transfer model type.
+        """
 
-            backend_context = BackendContext(
-                handler_context.parsed_type,
-                _parse_model(cls, handler_type.annotation, cls.config, handler_context.dto_for),
-                handler_type.annotation,
-            )
-            backend = cls._type_backend_map.setdefault(key, backend_type(backend_context))
-        cls._handler_backend_map[(handler_context.dto_for, handler_context.handler_id)] = backend
+    @abstractmethod
+    def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
+        """Parse builtin types into transfer model type.
 
-    @classmethod
-    def create_openapi_schema(
-        cls,
-        dto_for: ForType,
-        handler_id: str,
-        generate_examples: bool,
-        schemas: dict[str, Schema],
-    ) -> Reference | Schema:
-        """Create an OpenAPI request body.
+        Args:
+            builtins: Builtin type.
+            connection_context: Information about the active connection.
 
         Returns:
-            OpenAPI request body.
+            The builtin type parsed into transfer model type.
         """
-        backend = cls._handler_backend_map[(dto_for, handler_id)]
-        return backend.create_openapi_schema(generate_examples, schemas)
 
+    def populate_data_from_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
+        """Populate model instance from builtin types.
 
-def _parse_model(
-    dto_factory_type: type[AbstractDTOFactory],
-    model_type: Any,
-    config: DTOConfig,
-    dto_for: ForType,
-    nested_depth: int = 0,
-) -> FieldDefinitionsType:
-    """Reduce :attr:`model_type` to :class:`FieldDefinitionsType`.
-
-    .. important::
-        Implementations must respect the :attr:`config` object. For example:
-            - fields marked private must never be included in the field definitions.
-            - if a ``purpose`` is declared, then read-only fields must be taken into account.
-            - field mappings must be implemented.
-            - additional fields must be included, subject to ``purpose``.
-            - nested depth and nested recursion depth must be adhered to.
-
-    Returns:
-        Fields for data transfer.
-
-        Key is the name of the new field, and value is a tuple of type and default value pairs.
-
-        Add a new field called "new_field", that is a string, and required:
-        {"new_field": (str, ...)}
+        Args:
+            builtins: Builtin type.
+            connection_context: Information about the active connection.
 
-        Add a new field called "new_field", that is a string, and not-required:
-        {"new_field": (str, "default")}
+        Returns:
+            Instance or collection of ``model_type`` instances.
+        """
+        return transfer_data(
+            self.context.model_type,
+            self.parse_builtins(builtins, connection_context),
+            self.parsed_field_definitions,
+            "data",
+        )
 
-        Add a new field called "new_field", that may be `None`:
-        {"new_field": (str | None, None)}
-    """
-    defined_fields: dict[str, FieldDefinition | NestedFieldDefinition] = {}
-    for field_definition in dto_factory_type.generate_field_definitions(model_type):
-        if _should_exclude_field(field_definition, config, dto_for):
-            continue
-
-        if rename := config.rename_fields.get(field_definition.name):
-            field_definition = field_definition.copy_with(serialization_name=rename)  # noqa: PLW2901
-
-        if dto_factory_type.detect_nested_field(field_definition):
-            nested_field_definition = _handle_nested(dto_factory_type, field_definition, nested_depth, config, dto_for)
-            if nested_field_definition is not None:
-                defined_fields[field_definition.name] = nested_field_definition
-            continue
-
-        defined_fields[field_definition.name] = field_definition
-    return defined_fields
-
-
-def _should_exclude_field(field_definition: FieldDefinition, config: DTOConfig, dto_for: ForType) -> bool:
-    """Returns ``True`` where a field should be excluded from data transfer.
-
-    Args:
-        field_definition: defined DTO field
-        config: DTO configuration
-        dto_for: indicates whether the DTO is for the request body or response.
+    def populate_data_from_raw(self, raw: bytes, connection_context: ConnectionContext) -> Any:
+        """Parse raw bytes into instance of `model_type`.
 
-    Returns:
-        ``True`` if the field should not be included in any data transfer.
-    """
-    field_name = field_definition.name
-    dto_field = field_definition.dto_field
-    excluded = field_name in config.exclude
-    private = dto_field and dto_field.mark is Mark.PRIVATE
-    read_only_for_write = dto_for == "data" and dto_field and dto_field.mark is Mark.READ_ONLY
-    return bool(excluded or private or read_only_for_write)
-
-
-def _handle_nested(
-    dto_factory_type: type[AbstractDTOFactory],
-    field_definition: FieldDefinition,
-    nested_depth: int,
-    config: DTOConfig,
-    dto_for: ForType,
-) -> NestedFieldDefinition | None:
-    if nested_depth == config.max_nested_depth:
-        return None
-
-    nested = NestedFieldDefinition(
-        field_definition=field_definition,
-        nested_type=_get_model_type(field_definition.annotation),
-    )
+        Args:
+            raw: bytes
+            connection_context: Information about the active connection.
 
-    nested.nested_field_definitions = _parse_model(
-        dto_factory_type, nested.nested_type, config, dto_for, nested_depth + 1
-    )
-    return nested
+        Returns:
+            Instance or collection of ``model_type`` instances.
+        """
+        return transfer_data(
+            self.context.model_type, self.parse_raw(raw, connection_context), self.parsed_field_definitions, "data"
+        )
 
+    def encode_data(self, data: Any, connection_context: ConnectionContext) -> LitestarEncodableType:
+        """Encode data into a ``LitestarEncodableType``.
 
-def _get_model_type(annotation: type) -> Any:
-    """Get model type represented by the DTO.
+        Args:
+            data: Data to encode.
+            connection_context: Information about the active connection.
 
-    If ``annotation`` is a collection, then the inner type is returned.
+        Returns:
+            Encoded data.
+        """
+        return transfer_data(
+            self.transfer_model_type, data, self.parsed_field_definitions, "return"  # type: ignore[arg-type]
+        )
+
+    def create_openapi_schema(self, generate_examples: bool, schemas: dict[str, Schema]) -> Reference | Schema:
+        """Create a RequestBody model for the given RouteHandler or return None."""
+        field = SignatureField.create(self.annotation)
+        return create_schema(field=field, generate_examples=generate_examples, plugins=[], schemas=schemas)
+
+    def _create_transfer_type(
+        self, parsed_type: ParsedType, exclude: AbstractSet[str], field_name: str, unique_name: str, nested_depth: int
+    ) -> CompositeType | SimpleType:
+        exclude = _filter_exclude(exclude, field_name)
+
+        if parsed_type.is_union:
+            return self._create_union_type(parsed_type, exclude, unique_name, nested_depth)
+
+        if parsed_type.is_tuple:
+            if len(parsed_type.inner_types) == 2 and parsed_type.inner_types[1].annotation is Ellipsis:
+                return self._create_collection_type(parsed_type, exclude, unique_name, nested_depth)
+            return self._create_tuple_type(parsed_type, exclude, unique_name, nested_depth)
+
+        if parsed_type.is_mapping:
+            return self._create_mapping_type(parsed_type, exclude, unique_name, nested_depth)
+
+        if parsed_type.is_collection:
+            return self._create_collection_type(parsed_type, exclude, unique_name, nested_depth)
+
+        transfer_model: NestedFieldInfo | None = None
+        if self.context.is_nested_field_predicate(parsed_type):
+            if nested_depth == self.context.config.max_nested_depth:
+                raise NestedDepthExceededError()
+
+            nested_field_definitions = self.parse_model(parsed_type.annotation, exclude, nested_depth + 1)
+            transfer_model = NestedFieldInfo(
+                model=self.create_transfer_model_type(unique_name, nested_field_definitions),
+                field_definitions=nested_field_definitions,
+            )
 
-    Args:
-        annotation: any type.
+        return SimpleType(parsed_type, nested_field_info=transfer_model)
 
-    Returns:
-        The model type that is represented by the DTO.
-    """
-    parsed_type = ParsedType(annotation)
-    if parsed_type.is_collection:
-        return parsed_type.inner_types[0].annotation
-    if parsed_type.is_optional:
-        return next(t for t in parsed_type.inner_types if t.annotation is not NoneType).annotation
-    return parsed_type.annotation
+    def _create_collection_type(
+        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
+    ) -> CollectionType:
+        inner_type = self._create_transfer_type(
+            parsed_type=parsed_type.inner_types[0],
+            exclude=exclude,
+            field_name="0",
+            unique_name=_enumerate_name(unique_name, 0),
+            nested_depth=nested_depth,
+        )
+        return CollectionType(
+            parsed_type=parsed_type, inner_type=inner_type, has_nested=_determine_has_nested(inner_type)
+        )
+
+    def _create_mapping_type(
+        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
+    ) -> MappingType:
+        key_type = self._create_transfer_type(
+            parsed_type=parsed_type.inner_types[0],
+            exclude=exclude,
+            field_name="0",
+            unique_name=_enumerate_name(unique_name, 0),
+            nested_depth=nested_depth,
+        )
+        value_type = self._create_transfer_type(
+            parsed_type=parsed_type.inner_types[1],
+            exclude=exclude,
+            field_name="1",
+            unique_name=_enumerate_name(unique_name, 1),
+            nested_depth=nested_depth,
+        )
+        return MappingType(
+            parsed_type=parsed_type,
+            key_type=key_type,
+            value_type=value_type,
+            has_nested=_determine_has_nested(key_type) or _determine_has_nested(value_type),
+        )
+
+    def _create_tuple_type(
+        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
+    ) -> TupleType:
+        inner_types = tuple(
+            self._create_transfer_type(
+                parsed_type=inner_type,
+                exclude=exclude,
+                field_name=str(i),
+                unique_name=_enumerate_name(unique_name, i),
+                nested_depth=nested_depth,
+            )
+            for i, inner_type in enumerate(parsed_type.inner_types)
+        )
+        return TupleType(
+            parsed_type=parsed_type,
+            inner_types=inner_types,
+            has_nested=any(_determine_has_nested(t) for t in inner_types),
+        )
+
+    def _create_union_type(
+        self, parsed_type: ParsedType, exclude: AbstractSet[str], unique_name: str, nested_depth: int
+    ) -> UnionType:
+        inner_types = tuple(
+            self._create_transfer_type(
+                parsed_type=inner_type,
+                exclude=exclude,
+                field_name=str(i),
+                unique_name=_enumerate_name(unique_name, i),
+                nested_depth=nested_depth,
+            )
+            for i, inner_type in enumerate(parsed_type.inner_types)
+        )
+        return UnionType(
+            parsed_type=parsed_type,
+            inner_types=inner_types,
+            has_nested=any(_determine_has_nested(t) for t in inner_types),
+        )
+
+
+def _filter_exclude(exclude: AbstractSet[str], field_name: str) -> AbstractSet[str]:
+    """Filter exclude set to only include exclusions for the given field name."""
+    return {split[1] for s in exclude if (split := s.split(".", 1))[0] == field_name}
+
+
+def _enumerate_name(name: str, index: int) -> str:
+    """Enumerate ``name`` with ``index``."""
+    return f"{name}_{index}"
+
+
+def _determine_has_nested(transfer_type: SimpleType | CompositeType) -> bool:
+    """Determine if a transfer type has nested types."""
+    if isinstance(transfer_type, SimpleType):
+        return bool(transfer_type.nested_field_info)
+    return transfer_type.has_nested
```

### Comparing `litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/backend.py` & `litestar-2.0.0a6/litestar/dto/factory/_backends/pydantic/backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,36 @@
 from __future__ import annotations
 
-from collections.abc import Collection as CollectionsCollection
-from typing import TYPE_CHECKING, TypeVar, cast
-from uuid import uuid4
+from typing import TYPE_CHECKING, TypeVar
 
 from pydantic import BaseModel, parse_obj_as
 
-from litestar.dto.factory.backends.abc import AbstractDTOBackend, BackendContext
+from litestar.dto.factory._backends.abc import AbstractDTOBackend
 from litestar.serialization import decode_media_type
 
-from .utils import _build_data_from_pydantic_model, _create_model_for_field_definitions
+from .utils import _create_model_for_field_definitions
 
 if TYPE_CHECKING:
     from typing import Any, Collection
 
+    from litestar.dto.factory._backends.types import FieldDefinitionsType
     from litestar.dto.interface import ConnectionContext
-    from litestar.types.serialization import LitestarEncodableType
 
 __all__ = ("PydanticDTOBackend",)
 
 
 T = TypeVar("T")
 
 
 class PydanticDTOBackend(AbstractDTOBackend[BaseModel]):
     __slots__ = ()
 
-    def create_data_container_type(self, context: BackendContext) -> type[BaseModel]:
-        return _create_model_for_field_definitions(str(uuid4()), context.field_definitions)
+    def create_transfer_model_type(self, unique_name: str, field_definitions: FieldDefinitionsType) -> type[BaseModel]:
+        return _create_model_for_field_definitions(unique_name, field_definitions)
 
     def parse_raw(self, raw: bytes, connection_context: ConnectionContext) -> BaseModel | Collection[BaseModel]:
         return decode_media_type(  # type:ignore[no-any-return]
             raw, connection_context.request_encoding_type, type_=self.annotation
         )
 
-    def populate_data_from_builtins(self, data: Any) -> T | Collection[T]:
-        parsed_data = cast("BaseModel | Collection[BaseModel]", parse_obj_as(self.annotation, data))
-        return _build_data_from_pydantic_model(self.context.model_type, parsed_data, self.context.field_definitions)
-
-    def populate_data_from_raw(self, raw: bytes, connection_context: ConnectionContext) -> T | Collection[T]:
-        parsed_data = self.parse_raw(raw, connection_context)
-        return _build_data_from_pydantic_model(self.context.model_type, parsed_data, self.context.field_definitions)
-
-    def encode_data(self, data: Any, connection_context: ConnectionContext) -> LitestarEncodableType:
-        if isinstance(data, CollectionsCollection):
-            return self.context.parsed_type.origin(  # type:ignore[no-any-return]
-                self.data_container_type.from_orm(datum) for datum in data  # pyright:ignore
-            )
-        return self.data_container_type.from_orm(data)
+    def parse_builtins(self, builtins: Any, connection_context: ConnectionContext) -> Any:
+        return parse_obj_as(self.annotation, builtins)
```

### Comparing `litestar-2.0.0a5/litestar/dto/factory/field.py` & `litestar-2.0.0a6/litestar/dto/factory/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/dto/factory/stdlib/dataclass.py` & `litestar-2.0.0a6/litestar/dto/factory/stdlib/dataclass.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from litestar.dto.factory.abc import AbstractDTOFactory
 from litestar.dto.factory.field import DTO_FIELD_META_KEY
 from litestar.dto.factory.types import FieldDefinition
 from litestar.dto.factory.utils import get_model_type_hints
 from litestar.types.empty import Empty
+from litestar.utils.helpers import get_fully_qualified_class_name
 
 if TYPE_CHECKING:
-    from typing import Any, ClassVar, Collection, Generator
+    from typing import ClassVar, Collection, Generator
 
     from litestar.types.protocols import DataclassProtocol
+    from litestar.utils.signature import ParsedType
 
 
 __all__ = ("DataclassDTO", "DataT")
 
 DataT = TypeVar("DataT", bound="DataclassProtocol | Collection[DataclassProtocol]")
 AnyDataclass = TypeVar("AnyDataclass", bound="DataclassProtocol")
 
@@ -31,31 +33,25 @@
     @classmethod
     def generate_field_definitions(cls, model_type: type[DataclassProtocol]) -> Generator[FieldDefinition, None, None]:
         dc_fields = {f.name: f for f in fields(model_type)}
         for key, parsed_type in get_model_type_hints(model_type).items():
             if not (dc_field := dc_fields.get(key)):
                 continue
 
-            default: Any = Empty
-            default_factory: Any = Empty
+            default = dc_field.default if dc_field.default is not MISSING else Empty
 
-            if dc_field.default is not MISSING:
-                default = dc_field.default
-
-            if dc_field.default_factory is not MISSING:
-                default_factory = dc_field.default_factory
+            default_factory = dc_field.default_factory if dc_field.default_factory is not MISSING else None
 
             field_def = FieldDefinition(
                 name=key,
                 parsed_type=parsed_type,
                 default=default,
                 default_factory=default_factory,
                 dto_field=dc_field.metadata.get(DTO_FIELD_META_KEY),
+                unique_model_name=get_fully_qualified_class_name(model_type),
             )
 
             yield field_def
 
     @classmethod
-    def detect_nested_field(cls, field_definition: FieldDefinition) -> bool:
-        if not field_definition.parsed_type.inner_types:
-            return hasattr(field_definition.annotation, "__dataclass_fields__")
-        return any(hasattr(t.annotation, "__dataclass_fields__") for t in field_definition.parsed_type.inner_types)
+    def detect_nested_field(cls, parsed_type: ParsedType) -> bool:
+        return hasattr(parsed_type.annotation, "__dataclass_fields__")
```

### Comparing `litestar-2.0.0a5/litestar/dto/factory/types.py` & `litestar-2.0.0a6/litestar/dto/factory/_backends/msgspec/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,72 +1,55 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, NewType, TypeVar
 
-from litestar.types.empty import Empty
-from litestar.utils.dataclass import simple_asdict
-from litestar.utils.signature import ParsedParameter
+from msgspec import Struct, defstruct, field
 
-if TYPE_CHECKING:
-    from collections.abc import Mapping
-    from typing import Any, Callable
-
-    from typing_extensions import TypeAlias
-
-    from litestar.types import EmptyType
-
-    from .field import DTOField
+from litestar.dto.factory._backends.utils import create_transfer_model_type_annotation
+from litestar.types import Empty
 
-__all__ = ("FieldDefinition", "FieldDefinitionsType", "NestedFieldDefinition")
-
-
-@dataclass(frozen=True)
-class FieldDefinition(ParsedParameter):
-    """A model field representation for purposes of generating a DTO backend model type."""
+if TYPE_CHECKING:
+    from typing import Any
 
-    default_factory: Callable[[], Any] | EmptyType = field(default=Empty)
-    """Default factory of the field."""
-    dto_field: DTOField | None = field(default=None)
-    """DTO field configuration."""
-    serialization_name: str | None = field(default=None)
+    from litestar.dto.factory._backends.types import FieldDefinitionsType
+    from litestar.dto.factory.types import FieldDefinition
 
-    def copy_with(self, **kwargs: Any) -> FieldDefinition:
-        """Copy the field definition with the given keyword arguments.
 
-        Args:
-            **kwargs: Keyword arguments to update the field definition with.
+MsgspecField = NewType("MsgspecField", type)
+StructT = TypeVar("StructT", bound=Struct)
+T = TypeVar("T")
 
-        Returns:
-            Updated field definition.
-        """
-        return FieldDefinition(**{**simple_asdict(self, convert_nested=False), **kwargs})
 
+def _create_msgspec_field(field_definition: FieldDefinition) -> MsgspecField | None:
+    kws: dict[str, Any] = {}
+    if field_definition.default is not Empty:
+        kws["default"] = field_definition.default
 
-@dataclass
-class NestedFieldDefinition:
-    """For representing nested model."""
+    if field_definition.default_factory is not None:
+        kws["default_factory"] = field_definition.default_factory
 
-    field_definition: FieldDefinition
-    nested_type: Any
-    nested_field_definitions: FieldDefinitionsType = field(default_factory=dict)
+    if not kws:
+        return None
 
-    @property
-    def name(self) -> str:
-        """Name of the field."""
-        return self.field_definition.name
+    return field(**kws)  # type:ignore[no-any-return]
 
-    @property
-    def serialization_name(self) -> str | None:
-        """Serialization name of the field."""
-        return self.field_definition.serialization_name
 
-    def make_field_type(self, inner_type: type) -> Any:
-        if self.field_definition.parsed_type.is_collection:
-            return self.field_definition.parsed_type.safe_generic_origin[inner_type]
-        if self.field_definition.parsed_type.is_optional:
-            return self.field_definition.parsed_type.safe_generic_origin[inner_type, None]
-        return inner_type
+def _create_struct_field_def(
+    name: str, type_: type[Any], field_: MsgspecField | None
+) -> tuple[str, type[Any]] | tuple[str, type[Any], MsgspecField]:
+    if field_ is None:
+        return name, type_
+    return name, type_, field_
 
 
-FieldDefinitionsType: TypeAlias = "Mapping[str, FieldDefinition | NestedFieldDefinition]"
-"""Generic representation of names and types."""
+def _create_struct_for_field_definitions(model_name: str, field_definitions: FieldDefinitionsType) -> type[Struct]:
+    struct_fields: list[tuple[str, type] | tuple[str, type, MsgspecField]] = []
+    for field_def in field_definitions:
+        field_name = field_def.serialization_name or field_def.name
+        struct_fields.append(
+            _create_struct_field_def(
+                field_name,
+                create_transfer_model_type_annotation(field_def.transfer_type),
+                _create_msgspec_field(field_def),
+            )
+        )
+    return defstruct(model_name, struct_fields, frozen=True, kw_only=True)
```

### Comparing `litestar-2.0.0a5/litestar/dto/factory/utils.py` & `litestar-2.0.0a6/litestar/dto/factory/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/dto/interface.py` & `litestar-2.0.0a6/litestar/dto/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,24 +58,26 @@
             handler_id=str(connection.route_handler),
             request_encoding_type=getattr(connection, "content_type", (RequestEncodingType.JSON,))[0],
         )
 
 
 @runtime_checkable
 class DTOInterface(Protocol):
-    __slots__ = ()
+    __slots__ = ("connection_context",)
+
+    connection_context: ConnectionContext
 
-    @abstractmethod
     def __init__(self, connection_context: ConnectionContext) -> None:
         """Initialize the DTO.
 
         Args:
             connection_context: A :class:`ConnectionContext <.ConnectionContext>` instance, which provides
                 information about the connection.
         """
+        self.connection_context = connection_context
 
     @abstractmethod
     def data_to_encodable_type(self, data: Any) -> bytes | LitestarEncodableType:
         """Encode data to a type supported by litestar serialization.
 
         Can return either bytes or a type that Litestar can return to bytes.
```

### Comparing `litestar-2.0.0a5/litestar/enums.py` & `litestar-2.0.0a6/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/events/emitter.py` & `litestar-2.0.0a6/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/events/listener.py` & `litestar-2.0.0a6/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/exceptions/__init__.py` & `litestar-2.0.0a6/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0a6/litestar/exceptions/base_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0a6/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0a6/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/file_system.py` & `litestar-2.0.0a6/litestar/file_system.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/__init__.py` & `litestar-2.0.0a6/litestar/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0a6/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/base.py` & `litestar-2.0.0a6/litestar/handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0a6/litestar/handlers/http_handlers/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0a6/litestar/handlers/http_handlers/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0a6/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/handlers/websocket_handlers/_utils.py` & `litestar-2.0.0a6/litestar/handlers/websocket_handlers/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import inspect
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, cast
 
 from litestar.dto.interface import ConnectionContext
-from litestar.exceptions import WebSocketDisconnect
 from litestar.serialization import decode_json
 from litestar.utils import AsyncCallable
 
 if TYPE_CHECKING:
+    from contextlib import AbstractAsyncContextManager
+
     from msgspec.json import Encoder as JsonEncoder
 
     from litestar import WebSocket
     from litestar.dto.interface import DTOInterface
     from litestar.types import AnyCallable, TypeEncodersMap
     from litestar.types.asgi_types import WebSocketMode
     from litestar.utils.signature import ParsedSignature
@@ -107,41 +108,34 @@
             await socket.send_data(data_to_send, send_mode)  # pyright: ignore
 
     return handle_send
 
 
 def create_handler_function(
     listener_context: ListenerContext,
-    on_accept: AsyncCallable | None,
-    on_disconnect: AsyncCallable | None,
+    lifespan_manager: Callable[[WebSocket], AbstractAsyncContextManager],
 ) -> Callable[..., Coroutine[None, None, None]]:
-    async def handler_fn(socket: WebSocket, **kwargs: Any) -> None:
-        await socket.accept()
+    listener_callback = AsyncCallable(listener_context.listener_callback)
 
-        listener_callback = AsyncCallable(listener_context.listener_callback)
+    async def handler_fn(*args: Any, socket: WebSocket, **kwargs: Any) -> None:
         ctx = ConnectionContext.from_connection(socket)
         data_dto = listener_context.resolved_data_dto(ctx) if listener_context.resolved_data_dto else None
         return_dto = listener_context.resolved_return_dto(ctx) if listener_context.resolved_return_dto else None
-
-        if on_accept:
-            await on_accept(socket)
+        handle_receive = listener_context.handle_receive
+        handle_send = listener_context.handle_send if listener_context.can_send_data else None
 
         if listener_context.pass_socket:
             kwargs["socket"] = socket
 
-        while True:
-            try:
-                received_data = await listener_context.handle_receive(socket, data_dto)
-                data_to_send = await listener_callback(data=received_data, **kwargs)
-                if listener_context.can_send_data:
-                    await listener_context.handle_send(socket, data_to_send, return_dto)
-            except WebSocketDisconnect:
-                if on_disconnect:
-                    await on_disconnect(socket)
-                break
+        async with lifespan_manager(socket):
+            while True:
+                received_data = await handle_receive(socket, data_dto)
+                data_to_send = await listener_callback(*args, data=received_data, **kwargs)
+                if handle_send:
+                    await handle_send(socket, data_to_send, return_dto)
 
     return handler_fn
 
 
 def create_handler_signature(callback_signature: inspect.Signature) -> inspect.Signature:
     """Creates a :class:`inspect.Signature` for the handler function for signature modelling.
```

### Comparing `litestar-2.0.0a5/litestar/handlers/websocket_handlers/listener.py` & `litestar-2.0.0a6/litestar/handlers/websocket_handlers/listener.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 from __future__ import annotations
 
+import inspect
 from abc import ABC, abstractmethod
+from contextlib import AbstractAsyncContextManager, asynccontextmanager
 from functools import partial
-from typing import TYPE_CHECKING, Any, Callable, Mapping, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncGenerator,
+    Callable,
+    Mapping,
+    cast,
+)
 
 from msgspec.json import Encoder as JsonEncoder
 
 from litestar._signature import create_signature_model
+from litestar.connection import WebSocket
 from litestar.dto.interface import HandlerContext
-from litestar.exceptions import ImproperlyConfiguredException
+from litestar.exceptions import ImproperlyConfiguredException, WebSocketDisconnect
 from litestar.serialization import default_serializer
 from litestar.types import (
     AnyCallable,
     Dependencies,
     Empty,
     EmptyType,
     ExceptionHandler,
@@ -25,43 +35,47 @@
 from litestar.utils import AsyncCallable
 from litestar.utils.signature import ParsedSignature
 
 from . import _utils
 from .route_handler import WebsocketRouteHandler
 
 if TYPE_CHECKING:
-    from litestar import Litestar, WebSocket
+    from typing import Coroutine
+
+    from litestar import Litestar
     from litestar.dto.interface import DTOInterface
     from litestar.types.asgi_types import WebSocketMode
 
-__all__ = (
-    "WebsocketListener",
-    "websocket_listener",
-)
+
+__all__ = ("WebsocketListener", "websocket_listener")
 
 
 class websocket_listener(WebsocketRouteHandler):
     """A websocket listener that automatically accepts a connection, handles disconnects,
     invokes a callback function every time new data is received and sends any data
     returned
     """
 
-    __slots__ = (
-        "_on_accept",
-        "_on_disconnect",
-        "_pass_socket",
-        "_receive_mode",
-        "_send_mode",
-        "_listener_context",
-    )
+    __slots__ = {
+        "connection_accept_handler": "Callback to accept a WebSocket connection. By default, calls WebSocket.accept",
+        "on_accept": "Callback invoked after a WebSocket connection has been accepted",
+        "on_disconnect": "Callback invoked after a WebSocket connection has been closed",
+        "_pass_socket": None,
+        "_receive_mode": None,
+        "_send_mode": None,
+        "_listener_context": None,
+        "_connection_lifespan": None,
+    }
 
     def __init__(
         self,
         path: str | None | list[str] | None = None,
         *,
+        connection_accept_handler: Callable[[WebSocket], Coroutine[Any, Any, None]] = WebSocket.accept,
+        connection_lifespan: Callable[[WebSocket], AbstractAsyncContextManager[Any]] | None = None,
         dependencies: Dependencies | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
         exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
         guards: list[Guard] | None = None,
         middleware: list[Middleware] | None = None,
         receive_mode: WebSocketMode = "text",
         send_mode: WebSocketMode = "text",
@@ -75,14 +89,18 @@
         **kwargs: Any,
     ) -> None:
         """Initialize ``WebsocketRouteHandler``
 
         Args:
             path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
                 to ``/``
+            connection_accept_handler: A callable that accepts a :class:`WebSocket <.connection.WebSocket>` instance
+                and returns a coroutine that when awaited, will accept the connection. Defaults to ``WebSocket.accept``.
+            connection_lifespan: An asynchronous context manager, handling the lifespan of the connection. By default,
+                it calls the ``connection_accept_handler``, ``on_connect`` and ``on_disconnect``.
             dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
             dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
                 validation of request data.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
             guards: A sequence of :class:`Guard <.types.Guard>` callables.
             middleware: A sequence of :class:`Middleware <.types.Middleware>`.
             receive_mode: Websocket mode to receive data in, either `text` or `binary`.
@@ -101,16 +119,19 @@
                 modelling.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
             **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
         self._listener_context = _utils.ListenerContext()
         self._receive_mode: WebSocketMode = receive_mode
         self._send_mode: WebSocketMode = send_mode
-        self._on_accept = AsyncCallable(on_accept) if on_accept else None
-        self._on_disconnect = AsyncCallable(on_disconnect) if on_disconnect else None
+        self._connection_lifespan = connection_lifespan
+
+        self.connection_accept_handler = connection_accept_handler
+        self.on_accept = AsyncCallable(on_accept) if on_accept else None
+        self.on_disconnect = AsyncCallable(on_disconnect) if on_disconnect else None
         self.type_encoders = type_encoders
 
         super().__init__(
             path=path,
             dependencies=dependencies,
             exception_handlers=exception_handlers,
             guards=guards,
@@ -121,14 +142,36 @@
             **kwargs,
         )
 
         # need to be assigned after the super() call
         self.dto = dto
         self.return_dto = return_dto
 
+    @asynccontextmanager
+    async def default_connection_lifespan(self, socket: WebSocket) -> AsyncGenerator[None, None]:
+        """Handle the connection lifespan of a WebSocket.
+
+        By, default this will
+
+            - Call :attr:`connection_accept_handler` to accept a connection
+            - Call :attr:`on_accept` if defined after a connection has been accepted
+            - Call :attr:`on_disconnect` upon leaving the context
+        """
+        await self.connection_accept_handler(socket)
+
+        if self.on_accept:
+            await self.on_accept(socket)
+        try:
+            yield
+        except WebSocketDisconnect:
+            pass
+        finally:
+            if self.on_disconnect:
+                await self.on_disconnect(socket)
+
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it's set by inspecting its return annotations."""
         # since none of the validation rules of WebsocketRouteHandler apply here, this is let empty. Validation of the
         # user supplied method happens at init time of this handler instead in __call__
 
     def _init_handler_dtos(self) -> None:
         """Initialize the data and return DTOs for the handler."""
@@ -140,26 +183,31 @@
             return_type = self._listener_context.listener_callback_signature.return_type
             return_dto.on_registration(HandlerContext("return", str(self), return_type))
 
     def __call__(self, listener_callback: AnyCallable) -> websocket_listener:
         self._listener_context.listener_callback = listener_callback
         self._listener_context.handler_function = handler_function = _utils.create_handler_function(
             listener_context=self._listener_context,
-            on_accept=self._on_accept,
-            on_disconnect=self._on_disconnect,
+            lifespan_manager=self._connection_lifespan or self.default_connection_lifespan,
         )
         return super().__call__(handler_function)
 
     def on_registration(self, app: Litestar) -> None:
         self._set_listener_context()
         super().on_registration(app)
 
     def _create_signature_model(self, app: Litestar) -> None:
         """Create signature model for handler function."""
         if not self.signature_model:
+            extra_signatures = []
+            if self.on_accept:
+                extra_signatures.append(inspect.signature(self.on_accept))
+            if self.on_disconnect:
+                extra_signatures.append(inspect.signature(self.on_disconnect))
+
             new_signature = _utils.create_handler_signature(
                 self._listener_context.listener_callback_signature.original_signature
             )
             self.signature_model = create_signature_model(
                 dependency_name_set=self.dependency_name_set,
                 fn=cast("AnyCallable", self.fn.value),
                 preferred_validation_backend=app.preferred_validation_backend,
```

### Comparing `litestar-2.0.0a5/litestar/handlers/websocket_handlers/route_handler.py` & `litestar-2.0.0a6/litestar/handlers/websocket_handlers/route_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/logging/_utils.py` & `litestar-2.0.0a6/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/logging/config.py` & `litestar-2.0.0a6/litestar/logging/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/logging/picologging.py` & `litestar-2.0.0a6/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/logging/standard.py` & `litestar-2.0.0a6/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/_utils.py` & `litestar-2.0.0a6/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0a6/litestar/middleware/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/authentication.py` & `litestar-2.0.0a6/litestar/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/base.py` & `litestar-2.0.0a6/litestar/middleware/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/compression.py` & `litestar-2.0.0a6/litestar/middleware/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/cors.py` & `litestar-2.0.0a6/litestar/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/csrf.py` & `litestar-2.0.0a6/litestar/middleware/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0a6/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0a6/litestar/middleware/exceptions/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0a6/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0a6/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/logging.py` & `litestar-2.0.0a6/litestar/middleware/logging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/rate_limit.py` & `litestar-2.0.0a6/litestar/middleware/rate_limit.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/session/base.py` & `litestar-2.0.0a6/litestar/middleware/session/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/session/client_side.py` & `litestar-2.0.0a6/litestar/middleware/session/client_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/middleware/session/server_side.py` & `litestar-2.0.0a6/litestar/middleware/session/server_side.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/config.py` & `litestar-2.0.0a6/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/controller.py` & `litestar-2.0.0a6/litestar/openapi/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/datastructures.py` & `litestar-2.0.0a6/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/__init__.py` & `litestar-2.0.0a6/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/base.py` & `litestar-2.0.0a6/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/callback.py` & `litestar-2.0.0a6/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/components.py` & `litestar-2.0.0a6/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/contact.py` & `litestar-2.0.0a6/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0a6/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/encoding.py` & `litestar-2.0.0a6/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/enums.py` & `litestar-2.0.0a6/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/example.py` & `litestar-2.0.0a6/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0a6/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/header.py` & `litestar-2.0.0a6/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/info.py` & `litestar-2.0.0a6/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/license.py` & `litestar-2.0.0a6/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/link.py` & `litestar-2.0.0a6/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/media_type.py` & `litestar-2.0.0a6/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0a6/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0a6/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/open_api.py` & `litestar-2.0.0a6/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/operation.py` & `litestar-2.0.0a6/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/parameter.py` & `litestar-2.0.0a6/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/path_item.py` & `litestar-2.0.0a6/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/paths.py` & `litestar-2.0.0a6/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/reference.py` & `litestar-2.0.0a6/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/request_body.py` & `litestar-2.0.0a6/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/response.py` & `litestar-2.0.0a6/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/responses.py` & `litestar-2.0.0a6/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/schema.py` & `litestar-2.0.0a6/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0a6/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0a6/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/server.py` & `litestar-2.0.0a6/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0a6/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/tag.py` & `litestar-2.0.0a6/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/openapi/spec/xml.py` & `litestar-2.0.0a6/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/pagination.py` & `litestar-2.0.0a6/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/params.py` & `litestar-2.0.0a6/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/partial.py` & `litestar-2.0.0a6/litestar/partial.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/plugins.py` & `litestar-2.0.0a6/litestar/plugins.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/response/base.py` & `litestar-2.0.0a6/litestar/response/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/response/file.py` & `litestar-2.0.0a6/litestar/response/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/response/redirect.py` & `litestar-2.0.0a6/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/response/streaming.py` & `litestar-2.0.0a6/litestar/response/streaming.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/response/template.py` & `litestar-2.0.0a6/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/response_containers.py` & `litestar-2.0.0a6/litestar/response_containers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/router.py` & `litestar-2.0.0a6/litestar/router.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/routes/asgi.py` & `litestar-2.0.0a6/litestar/routes/asgi.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/routes/base.py` & `litestar-2.0.0a6/litestar/routes/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/routes/http.py` & `litestar-2.0.0a6/litestar/routes/http.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/routes/websocket.py` & `litestar-2.0.0a6/litestar/routes/websocket.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/security/base.py` & `litestar-2.0.0a6/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/security/session_auth/auth.py` & `litestar-2.0.0a6/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/security/session_auth/middleware.py` & `litestar-2.0.0a6/litestar/security/session_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/serialization.py` & `litestar-2.0.0a6/litestar/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/static_files/base.py` & `litestar-2.0.0a6/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/static_files/config.py` & `litestar-2.0.0a6/litestar/static_files/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     html_mode: bool = False
     """Flag dictating whether serving html.
 
     If true, the default file will be 'index.html'.
     """
     name: str | None = None
     """An optional string identifying the static files handler."""
-    file_system: Any = BaseLocalFileSystem()
+    file_system: Any = BaseLocalFileSystem()  # noqa: RUF009
     """The file_system spec to use for serving files.
 
     Notes:
         - A file_system is a class that adheres to the
             :class:`FileSystemProtocol <litestar.types.FileSystemProtocol>`.
         - You can use any of the file systems exported from the
             [fsspec](https://filesystem-spec.readthedocs.io/en/latest/) library for this purpose.
```

### Comparing `litestar-2.0.0a5/litestar/status_codes.py` & `litestar-2.0.0a6/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/stores/base.py` & `litestar-2.0.0a6/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/stores/file.py` & `litestar-2.0.0a6/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/stores/memory.py` & `litestar-2.0.0a6/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/stores/redis.py` & `litestar-2.0.0a6/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/stores/registry.py` & `litestar-2.0.0a6/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/template/base.py` & `litestar-2.0.0a6/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/template/config.py` & `litestar-2.0.0a6/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/__init__.py` & `litestar-2.0.0a6/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/client/__init__.py` & `litestar-2.0.0a6/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/client/async_client.py` & `litestar-2.0.0a6/litestar/testing/client/async_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/client/base.py` & `litestar-2.0.0a6/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/client/sync_client.py` & `litestar-2.0.0a6/litestar/testing/client/sync_client.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/helpers.py` & `litestar-2.0.0a6/litestar/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/life_span_handler.py` & `litestar-2.0.0a6/litestar/testing/life_span_handler.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/request_factory.py` & `litestar-2.0.0a6/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/transport.py` & `litestar-2.0.0a6/litestar/testing/transport.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/testing/websocket_test_session.py` & `litestar-2.0.0a6/litestar/testing/websocket_test_session.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from contextlib import ExitStack
 from queue import Queue
 from typing import TYPE_CHECKING, Any, Literal, cast
 
 from anyio import sleep
 
 from litestar.exceptions import WebSocketDisconnect
-from litestar.serialization import decode_json, encode_json
+from litestar.serialization import decode_json, decode_msgpack, encode_json, encode_msgpack
 from litestar.status_codes import WS_1000_NORMAL_CLOSURE
 
 if TYPE_CHECKING:
     from litestar.testing.client.sync_client import TestClient
     from litestar.types import (
         WebSocketConnectEvent,
         WebSocketDisconnectEvent,
@@ -142,72 +142,108 @@
         """Sends the given data as JSON.
 
         Args:
             data: The data to send.
             mode: Either ``text`` or ``binary``
 
         Returns:
-            None.
+            None
         """
         self.send(encode_json(data), mode=mode)
 
+    def send_msgpack(self, data: Any) -> None:
+        """Sends the given data as MessagePack.
+
+        Args:
+            data: The data to send.
+
+        Returns:
+            None
+        """
+        self.send(encode_msgpack(data), mode="binary")
+
     def close(self, code: int = WS_1000_NORMAL_CLOSURE) -> None:
         """Sends an 'websocket.disconnect' event.
 
         Args:
             code: status code for closing the connection.
 
         Returns:
             None.
         """
         event: WebSocketDisconnectEvent = {"type": "websocket.disconnect", "code": code}
         self.receive_queue.put(event)
 
-    def receive(self) -> WebSocketSendMessage:
+    def receive(self, block: bool = True, timeout: float | None = None) -> WebSocketSendMessage:
         """This is the base receive method.
 
+        Args:
+            block: Block until a message is received
+            timeout: If ``block`` is ``True``, block at most ``timeout`` seconds
+
         Notes:
             - you can use one of the other receive methods to extract the data from the message.
 
         Returns:
             A websocket message.
         """
-        message = cast("WebSocketSendMessage", self.send_queue.get())
+        message = cast("WebSocketSendMessage", self.send_queue.get(block=block, timeout=timeout))
+
         if isinstance(message, BaseException):
             raise message
 
         if message["type"] == "websocket.close":
             raise WebSocketDisconnect(
                 detail=cast("str", message.get("reason", "")),
                 code=message.get("code", WS_1000_NORMAL_CLOSURE),
             )
         return message
 
-    def receive_text(self) -> str:
-        """Returns:
-        A string value.
+    def receive_text(self, block: bool = True, timeout: float | None = None) -> str:
+        """Receive data in ``text`` mode and return a string
+
+        Args:
+            block: Block until a message is received
+            timeout: If ``block`` is ``True``, block at most ``timeout`` seconds
+
+        Returns:
+            A string value.
         """
-        message = self.receive()
+        message = self.receive(block=block, timeout=timeout)
         return cast("str", message.get("text", ""))
 
-    def receive_bytes(self) -> bytes:
-        """Returns:
-        A bytes string value.
+    def receive_bytes(self, block: bool = True, timeout: float | None = None) -> bytes:
+        """Receive data in ``binary`` mode and return bytes
+
+        Args:
+            block: Block until a message is received
+            timeout: If ``block`` is ``True``, block at most ``timeout`` seconds
+
+        Returns:
+            A string value.
         """
-        message = self.receive()
+        message = self.receive(block=block, timeout=timeout)
         return cast("bytes", message.get("bytes", b""))
 
-    def receive_json(self, mode: Literal["text", "binary"] = "text") -> Any:
-        """Receives JSON.
+    def receive_json(
+        self, mode: Literal["text", "binary"] = "text", block: bool = True, timeout: float | None = None
+    ) -> Any:
+        """Receive data in either ``text`` or ``binary`` mode and decode it as JSON.
 
         Args:
             mode: Either ``text`` or ``binary``
+            block: Block until a message is received
+            timeout: If ``block`` is ``True``, block at most ``timeout`` seconds
 
         Returns:
             An arbitrary value
         """
-        message = self.receive()
+        message = self.receive(block=block, timeout=timeout)
 
         if mode == "text":
             return decode_json(cast("str", message.get("text", "")))
 
         return decode_json(cast("bytes", message.get("bytes", b"")))
+
+    def receive_msgpack(self, block: bool = True, timeout: float | None = None) -> Any:
+        message = self.receive(block=block, timeout=timeout)
+        return decode_msgpack(cast("bytes", message.get("bytes", b"")))
```

### Comparing `litestar-2.0.0a5/litestar/types/__init__.py` & `litestar-2.0.0a6/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/asgi_types.py` & `litestar-2.0.0a6/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/callable_types.py` & `litestar-2.0.0a6/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/composite_types.py` & `litestar-2.0.0a6/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/file_types.py` & `litestar-2.0.0a6/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/internal_types.py` & `litestar-2.0.0a6/litestar/types/internal_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/protocols.py` & `litestar-2.0.0a6/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/types/serialization.py` & `litestar-2.0.0a6/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/__init__.py` & `litestar-2.0.0a6/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/compat.py` & `litestar-2.0.0a6/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/dataclass.py` & `litestar-2.0.0a6/litestar/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/deprecation.py` & `litestar-2.0.0a6/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/helpers.py` & `litestar-2.0.0a6/litestar/utils/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Generic, TypeVar, cast
 
-__all__ = ("Ref", "get_enum_string_value", "get_name", "unwrap_partial")
+__all__ = ("Ref", "get_enum_string_value", "get_fully_qualified_class_name", "get_name", "unwrap_partial")
 
 
 T = TypeVar("T")
 
 if TYPE_CHECKING:
     from litestar.types import MaybePartial
 
@@ -23,14 +23,20 @@
         A name string.
     """
     if hasattr(value, "__name__"):
         return cast("str", value.__name__)
     return type(value).__name__
 
 
+def get_fully_qualified_class_name(value: type[Any]) -> str:
+    """Construct the full path name for a type."""
+    module = getattr(value, "__module__", "<no module>")
+    return f"{module}.{value.__qualname__}"
+
+
 def get_enum_string_value(value: Enum | str) -> str:
     """Return the string value of a string enum.
 
     See: https://github.com/litestar-org/litestar/pull/633#issuecomment-1286519267
 
     Args:
         value: An enum or string.
```

### Comparing `litestar-2.0.0a5/litestar/utils/path.py` & `litestar-2.0.0a6/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/predicates.py` & `litestar-2.0.0a6/litestar/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/scope.py` & `litestar-2.0.0a6/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/sequence.py` & `litestar-2.0.0a6/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/signature.py` & `litestar-2.0.0a6/litestar/utils/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import sys
 import typing
+from collections.abc import Collection, Mapping
 from dataclasses import dataclass
 from inspect import Parameter, Signature, getmembers, isclass, ismethod
 from itertools import chain
-from typing import Any, AnyStr, Collection, ForwardRef, TypeVar, Union
+from typing import Any, AnyStr, ForwardRef, TypeVar, Union
 
 from typing_extensions import Annotated, NotRequired, Required, Self, get_args, get_origin, get_type_hints
 
 from litestar import connection, datastructures, types
 from litestar.datastructures import ImmutableState
 from litestar.enums import RequestEncodingType
 from litestar.exceptions import ImproperlyConfiguredException
@@ -153,14 +154,24 @@
 
     @property
     def is_forward_ref(self) -> bool:
         """Whether the annotation is a forward reference or not."""
         return isinstance(self.annotation, (str, ForwardRef))
 
     @property
+    def is_mapping(self) -> bool:
+        """Whether the annotation is a mapping or not."""
+        return self.is_subclass_of(Mapping)
+
+    @property
+    def is_tuple(self) -> bool:
+        """Whether the annotation is a ``tuple`` or not."""
+        return self.is_subclass_of(tuple)
+
+    @property
     def is_type_var(self) -> bool:
         """Whether the annotation is a TypeVar or not."""
         return isinstance(self.annotation, TypeVar)
 
     @property
     def is_union(self) -> bool:
         """Whether the annotation is a union type or not."""
```

### Comparing `litestar-2.0.0a5/litestar/utils/sync.py` & `litestar-2.0.0a6/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/typing.py` & `litestar-2.0.0a6/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/litestar/utils/version.py` & `litestar-2.0.0a6/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a5/pyproject.toml` & `litestar-2.0.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0alpha5"
+version = "2.0.0alpha6"
 description = "Performant, light and flexible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
 maintainers = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
+    "Jacob Coffee <jacob@z7x.org>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://litestar.dev/"
 repository = "https://github.com/litestar-org/litestar"
 documentation = "https://docs.litestar.dev/"
 keywords = [
@@ -71,32 +72,33 @@
 picologging = { version = "*", optional = true }
 polyfactory = ">=2"
 pydantic = "<2"
 python-dateutil = { version = "*", optional = true }
 python-jose = { version = "*", optional = true }
 pytimeparse = { version = "*", optional = true }
 pyyaml = "*"
-redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3", optional = true, extras = ["hiredis"] }
+redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5", optional = true, extras = ["hiredis"] }
 rich = { version = ">=13.0.0", optional = true }
-sqlalchemy = { version = ">=2.0.4", optional = true }
+sqlalchemy = { version = ">=2.0.12", optional = true }
 structlog = { version = "*", optional = true }
 typing-extensions = "*"
 uvicorn = {extras = ["standard"], version = "^0.21.1", optional = true}
+importlib-resources = { version="^5.12.0", python = "<3.9" }
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
 asyncmy = "*"
 asyncpg = "*"
 attrs = "*"
 beautifulsoup4 = "*"
 brotli = "*"
 cattrs = "*"
 click = "*"
 cryptography = "*"
-fakeredis = { extras = ["lua"], version = ">=2.10.2" }
+fakeredis = { extras = ["lua"], version = "2.11.0" }
 freezegun = "*"
 fsspec = "*"
 greenlet = "*"
 hypothesis = "*"
 jinja2 = "*"
 jsbeautifier = "*"
 mako = "*"
@@ -120,14 +122,15 @@
 rich = "*"
 sqlalchemy = ">=2.0"
 starlette = "*"
 structlog = "*"
 tortoise-orm = ">=0.17.0"
 trio = "*"
 uvicorn = "*"
+pytest-rerunfailures = "^11.1.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 auto-pytabs = { extras = ["sphinx"], version = "*" }
 black = "*"
@@ -297,14 +300,15 @@
 [tool.ruff.pep8-naming]
 classmethod-decorators = [
     "classmethod",
     "pydantic.root_validator",
     "pydantic.validator",
     "sqlalchemy.ext.declarative.declared_attr",
     "sqlalchemy.orm.declared_attr.directive",
+    "sqlalchemy.orm.declared_attr"
 ]
 
 [tool.ruff.isort]
 known-first-party = ["litestar", "tests", "examples"]
 
 [tool.ruff.per-file-ignores]
 "tests/**/*.*" = [
```

### Comparing `litestar-2.0.0a5/PKG-INFO` & `litestar-2.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0a5
+Version: 2.0.0a6
 Summary: Performant, light and flexible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -49,30 +49,31 @@
 Requires-Dist: brotli ; extra == "brotli" or extra == "full"
 Requires-Dist: cattrs ; extra == "attrs" or extra == "full"
 Requires-Dist: click ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: cryptography ; extra == "cryptography" or extra == "jwt" or extra == "full"
 Requires-Dist: fast-query-parsers
 Requires-Dist: httpx (>=0.22)
 Requires-Dist: importlib-metadata ; python_version < "3.10"
+Requires-Dist: importlib-resources (>=5.12.0,<6.0.0) ; python_version < "3.9"
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "jinja" or extra == "standard" or extra == "full"
 Requires-Dist: jsbeautifier ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: mako (>=1.2.4)
 Requires-Dist: msgspec
 Requires-Dist: multidict (>=6.0.2)
 Requires-Dist: opentelemetry-instrumentation-asgi ; extra == "opentelemetry" or extra == "full"
 Requires-Dist: picologging ; extra == "picologging"
 Requires-Dist: polyfactory (>=2)
 Requires-Dist: pydantic (<2)
 Requires-Dist: python-dateutil ; extra == "attrs"
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
 Requires-Dist: pytimeparse ; extra == "attrs" or extra == "full"
 Requires-Dist: pyyaml
-Requires-Dist: redis[hiredis] (>=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3) ; extra == "redis" or extra == "full"
+Requires-Dist: redis[hiredis] (>=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3,!=4.5.5) ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
-Requires-Dist: sqlalchemy (>=2.0.4) ; extra == "sqlalchemy" or extra == "full"
+Requires-Dist: sqlalchemy (>=2.0.12) ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: structlog ; extra == "structlog" or extra == "full"
 Requires-Dist: typing-extensions
 Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "cli" or extra == "standard" or extra == "full"
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Repository, https://github.com/litestar-org/litestar
 Description-Content-Type: text/markdown
 
@@ -94,15 +95,15 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-97-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-100-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
 [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
@@ -479,17 +480,22 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/giorgiovilardo"><img src="https://avatars.githubusercontent.com/u/56472600?v=4?s=100" width="100px;" alt="Giorgio Vilardo"/><br /><sub><b>Giorgio Vilardo</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=giorgiovilardo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt="Nicholas Bollweg"/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=bollwyvl" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/khiem-doan/"><img src="https://avatars.githubusercontent.com/u/15646249?v=4?s=100" width="100px;" alt="Khiem Doan"/><br /><sub><b>Khiem Doan</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=khiemdoan" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kedod"><img src="https://avatars.githubusercontent.com/u/35638715?v=4?s=100" width="100px;" alt="kedod"/><br /><sub><b>kedod</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=kedod" title="Documentation">📖</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a> <a href="#infra-sonpro1296" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://patrickarmengol.com"><img src="https://avatars.githubusercontent.com/u/42473149?v=4?s=100" width="100px;" alt="Patrick Armengol"/><br /><sub><b>Patrick Armengol</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=patrickarmengol" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/erhuabushuo"><img src="https://avatars.githubusercontent.com/u/1642364?v=4?s=100" width="100px;" alt="疯人院主任"/><br /><sub><b>疯人院主任</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=erhuabushuo" title="Documentation">📖</a></td>
+    </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/aviral-nayya"><img src="https://avatars.githubusercontent.com/u/121891493?v=4?s=100" width="100px;" alt="aviral-nayya"/><br /><sub><b>aviral-nayya</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=aviral-nayya" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/whiskeyriver"><img src="https://avatars.githubusercontent.com/u/162092?v=4?s=100" width="100px;" alt="whiskeyriver"/><br /><sub><b>whiskeyriver</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=whiskeyriver" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

