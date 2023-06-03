# Comparing `tmp/propan-0.1.2.7.tar.gz` & `tmp/propan-0.1.2.8.tar.gz`

## Comparing `propan-0.1.2.7.tar` & `propan-0.1.2.8.tar`

### file list

```diff
@@ -1,143 +1,146 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.7/SECURITY.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/kafka/1_direct.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/nats/1_basic.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/redis/pattern.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.7/examples/sqs/1_basic.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/__about__.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/__main__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/py.typed
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/exceptions.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/__init__.py
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/schemas.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/_model/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/__init__.py
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/schema.py
--rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/sqs_broker.py
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/brokers/sqs/sqs_broker.pyi
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/async_app/sqs.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/sqs/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/sqs/router.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/fastapi/sqs/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/log/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/log/formatter.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/log/logging.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/nats.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/redis.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/sqs.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.7/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.7/scripts/test.sh
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 propan-0.1.2.7/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.7/LICENSE
--rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.7/README.md
--rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.7/pyproject.toml
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.8/SECURITY.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.8/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.8/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/__about__.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/__main__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/exceptions.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11272 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8394 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     6709 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    12162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/app.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6703 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/log/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/log/formatter.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/log/logging.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/nats.py
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/sqs.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.8/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.8/scripts/test.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 propan-0.1.2.8/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.8/LICENSE
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 propan-0.1.2.8/README.md
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 propan-0.1.2.8/pyproject.toml
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 propan-0.1.2.8/PKG-INFO
```

### Comparing `propan-0.1.2.7/CONTRIBUTING.md` & `propan-0.1.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/SECURITY.md` & `propan-0.1.2.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/.github/workflows/documentation.yml` & `propan-0.1.2.8/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/.github/workflows/publish_coverage.yml` & `propan-0.1.2.8/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/.github/workflows/publish_pypi.yml` & `propan-0.1.2.8/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/.github/workflows/tests.yml` & `propan-0.1.2.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/3_lifespan_events.py` & `propan-0.1.2.8/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.8/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/5_publishing.py` & `propan-0.1.2.8/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/6_arguments_casting.py` & `propan-0.1.2.8/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/7_handler_errors_processing.py` & `propan-0.1.2.8/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.8/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.8/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.8/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.8/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.8/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/dependencies/7_annotated.py` & `propan-0.1.2.8/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.8/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/rabbit/direct.py` & `propan-0.1.2.8/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/rabbit/fanout.py` & `propan-0.1.2.8/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/rabbit/header.py` & `propan-0.1.2.8/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/rabbit/topic.py` & `propan-0.1.2.8/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/redis/direct.py` & `propan-0.1.2.8/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/examples/redis/pattern.py` & `propan-0.1.2.8/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/__about__.py` & `propan-0.1.2.8/propan/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple and fast framework to create message brokers based microservices"""
 
 from unittest.mock import Mock
 
-__version__ = "0.1.2.7"
+__version__ = "0.1.2.8"
 
 
 INSTALL_MESSAGE = (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
```

### Comparing `propan-0.1.2.7/propan/__init__.py` & `propan-0.1.2.8/propan/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/annotations.py` & `propan-0.1.2.8/propan/annotations.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/types.py` & `propan-0.1.2.8/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/push_back_watcher.py` & `propan-0.1.2.8/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/_model/broker_usecase.py` & `propan-0.1.2.8/propan/brokers/_model/broker_usecase.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/_model/schemas.py` & `propan-0.1.2.8/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/_model/utils.py` & `propan-0.1.2.8/propan/brokers/_model/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.8/propan/brokers/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.8/propan/brokers/kafka/kafka_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.8/propan/brokers/nats/nats_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.8/propan/brokers/nats/nats_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.8/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/nats/schemas.py` & `propan-0.1.2.8/propan/brokers/nats/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.8/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.8/propan/brokers/rabbit/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.8/propan/brokers/redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.8/propan/brokers/redis/redis_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/redis/schemas.py` & `propan-0.1.2.8/propan/brokers/redis/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/sqs/schema.py` & `propan-0.1.2.8/propan/brokers/sqs/schema.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/sqs/sqs_broker.py` & `propan-0.1.2.8/propan/brokers/sqs/sqs_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/brokers/sqs/sqs_broker.pyi` & `propan-0.1.2.8/propan/brokers/sqs/sqs_broker.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/app.py` & `propan-0.1.2.8/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/main.py` & `propan-0.1.2.8/propan/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,17 @@
     log_level: int = logging.INFO,
     app_level: int = logging.INFO,
 ) -> None:
     try:
         propan_app = import_object(module, app)
 
         if not isinstance(propan_app, PropanApp):
-            raise ValueError(f"{propan_app} is not a PropanApp")
+            raise FileNotFoundError(f"{propan_app} is not a PropanApp")
 
-    except (ValueError, FileNotFoundError, AttributeError) as e:
+    except (FileNotFoundError, AttributeError) as e:
         logger.error(e)
         logger.error("Please, input module like [python_file:propan_app_name]")
         exit()
 
     else:
         set_log_level(log_level, propan_app)
```

### Comparing `propan-0.1.2.7/propan/cli/startproject/core.py` & `propan-0.1.2.8/propan/cli/startproject/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/core.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/startproject/async_app/sqs.py` & `propan-0.1.2.8/propan/cli/startproject/async_app/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/supervisors/basereload.py` & `propan-0.1.2.8/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.8/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/supervisors/utils.py` & `propan-0.1.2.8/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.8/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/utils/imports.py` & `propan-0.1.2.8/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/utils/logs.py` & `propan-0.1.2.8/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/cli/utils/parser.py` & `propan-0.1.2.8/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/__init__.py` & `propan-0.1.2.8/propan/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/core/route.py` & `propan-0.1.2.8/propan/fastapi/core/route.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/core/router.py` & `propan-0.1.2.8/propan/fastapi/core/router.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.8/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/nats/router.pyi` & `propan-0.1.2.8/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.8/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/redis/router.pyi` & `propan-0.1.2.8/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/fastapi/sqs/router.pyi` & `propan-0.1.2.8/propan/fastapi/sqs/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/log/formatter.py` & `propan-0.1.2.8/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/log/logging.py` & `propan-0.1.2.8/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/__init__.py` & `propan-0.1.2.8/propan/test/__init__.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/kafka.py` & `propan-0.1.2.8/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/nats.py` & `propan-0.1.2.8/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/rabbit.py` & `propan-0.1.2.8/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/redis.py` & `propan-0.1.2.8/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/sqs.py` & `propan-0.1.2.8/propan/test/sqs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/test/utils.py` & `propan-0.1.2.8/propan/test/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/utils/functions.py` & `propan-0.1.2.8/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/utils/context/main.py` & `propan-0.1.2.8/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/propan/utils/context/types.py` & `propan-0.1.2.8/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/LICENSE` & `propan-0.1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/README.md` & `propan-0.1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/pyproject.toml` & `propan-0.1.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.7/PKG-INFO` & `propan-0.1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.7
+Version: 0.1.2.8
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.7 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.8 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

