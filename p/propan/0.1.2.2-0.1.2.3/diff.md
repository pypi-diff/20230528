# Comparing `tmp/propan-0.1.2.2.tar.gz` & `tmp/propan-0.1.2.3.tar.gz`

## Comparing `propan-0.1.2.2.tar` & `propan-0.1.2.3.tar`

### file list

```diff
@@ -1,131 +1,142 @@
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 propan-0.1.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.2/SECURITY.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 propan-0.1.2.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/5_publishing.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/8_rpc_over_mq.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/9_noblocking_callbacks.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/native_fastapi.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/kafka/1_direct.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/direct.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/header.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/rabbit/topic.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/redis/direct.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.2/examples/redis/pattern.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/__about__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/__main__.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/annotations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/py.typed
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/__init__.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/kafka_broker.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/kafka_broker.pyi
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/kafka/schemas.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/model/utils.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/__init__.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/redis_broker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/redis_broker.pyi
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/brokers/redis/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/__init__.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/app.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/main.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/app.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/core.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/__init__.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/app.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/core.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/kafka.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/nats.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/rabbit.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/async_app/redis.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/sync_app/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/startproject/sync_app/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/imports.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/core/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/core/route.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/core/router.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/kafka/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/kafka/router.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/kafka/router.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/nats/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/nats/router.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/nats/router.pyi
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/rabbit/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/rabbit/router.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/rabbit/router.pyi
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/redis/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/redis/router.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/fastapi/redis/router.pyi
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/log/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/log/logging.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/kafka.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/nats.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/rabbit.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/redis.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/test/utils.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/classes.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/functions.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/context/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/context/main.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.2/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.2/scripts/test.sh
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.2/LICENSE
--rw-r--r--   0        0        0    12237 2020-02-02 00:00:00.000000 propan-0.1.2.2/README.md
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 propan-0.1.2.2/pyproject.toml
--rw-r--r--   0        0        0    15742 2020-02-02 00:00:00.000000 propan-0.1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 propan-0.1.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.1.2.3/SECURITY.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 propan-0.1.2.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/kafka/1_direct.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/nats/1_basic.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/direct.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/header.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/rabbit/topic.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/redis/direct.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/redis/pattern.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 propan-0.1.2.3/examples/sqs/1_basic.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/__about__.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/__main__.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/annotations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/py.typed
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/__init__.py
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/broker_usecase.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/schemas.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/_model/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/kafka_broker.pyi
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/kafka/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/__init__.py
+-rw-r--r--   0        0        0     8176 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/redis_broker.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/redis_broker.pyi
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/redis/schemas.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/__init__.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/schema.py
+-rw-r--r--   0        0        0    10585 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/sqs_broker.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/brokers/sqs/sqs_broker.pyi
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/__init__.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/app.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/main.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/app.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/core.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/app.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/core.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/kafka.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/nats.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/rabbit.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/redis.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/async_app/sqs.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/sync_app/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/startproject/sync_app/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/kafka/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/kafka/router.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/kafka/router.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/nats/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/nats/router.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/nats/router.pyi
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/rabbit/router.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/rabbit/router.pyi
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/redis/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/redis/router.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/redis/router.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/sqs/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/sqs/router.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/fastapi/sqs/router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/log/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/log/logging.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/kafka.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/nats.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/rabbit.py
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/redis.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/sqs.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/test/utils.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/classes.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/context/main.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 propan-0.1.2.3/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.1.2.3/scripts/test.sh
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 propan-0.1.2.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.1.2.3/LICENSE
+-rw-r--r--   0        0        0    12356 2020-02-02 00:00:00.000000 propan-0.1.2.3/README.md
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 propan-0.1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    15986 2020-02-02 00:00:00.000000 propan-0.1.2.3/PKG-INFO
```

### Comparing `propan-0.1.2.2/CONTRIBUTING.md` & `propan-0.1.2.3/CONTRIBUTING.md`

 * *Files 5% similar despite different names*

```diff
@@ -117,14 +117,19 @@
       - KAFKA_CFG_CONTROLLER_LISTENER_NAMES=CONTROLLER
       - KAFKA_CFG_LISTENERS=PLAINTEXT://:9092,CONTROLLER://:9093
       - KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP=CONTROLLER:PLAINTEXT,PLAINTEXT:PLAINTEXT
       - KAFKA_CFG_ADVERTISED_LISTENERS=PLAINTEXT://127.0.0.1:9092
       - KAFKA_BROKER_ID=1
       - KAFKA_CFG_CONTROLLER_QUORUM_VOTERS=1@kafka:9093
       - ALLOW_PLAINTEXT_LISTENER=yes
+  
+  sqs:
+    image: softwaremill/elasticmq-native
+    ports:
+      - 9324:9324
 ```
 
 ```bash
 docker compose up -d
 ```
 
 #### Hatch
```

### Comparing `propan-0.1.2.2/SECURITY.md` & `propan-0.1.2.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/.github/workflows/documentation.yml` & `propan-0.1.2.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/.github/workflows/publish_coverage.yml` & `propan-0.1.2.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/.github/workflows/publish_pypi.yml` & `propan-0.1.2.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/.github/workflows/tests.yml` & `propan-0.1.2.3/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,19 @@
           KAFKA_CFG_LISTENERS: "PLAINTEXT://:9092,CONTROLLER://:9093"
           KAFKA_CFG_LISTENER_SECURITY_PROTOCOL_MAP: "CONTROLLER:PLAINTEXT,PLAINTEXT:PLAINTEXT"
           KAFKA_CFG_ADVERTISED_LISTENERS: "PLAINTEXT://127.0.0.1:9092"
           KAFKA_BROKER_ID: "1"
           KAFKA_CFG_CONTROLLER_QUORUM_VOTERS: "1@kafka:9093"
           ALLOW_PLAINTEXT_LISTENER: "true"
 
+      sqs:
+        image: softwaremill/elasticmq-native
+        ports:
+          - 9324:9324
+
       nats:
         image: nats
         ports:
           - 4222:4222
 
       redis:
         image: redis
```

### Comparing `propan-0.1.2.2/examples/3_lifespan_events.py` & `propan-0.1.2.3/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/4_cli_attributes_promotion.py` & `propan-0.1.2.3/examples/4_cli_attributes_promotion.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/5_publishing.py` & `propan-0.1.2.3/examples/5_publishing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/6_arguments_casting.py` & `propan-0.1.2.3/examples/6_arguments_casting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/7_handler_errors_processing.py` & `propan-0.1.2.3/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/dependencies/1_dependency_injection.py` & `propan-0.1.2.3/examples/dependencies/1_dependency_injection.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/dependencies/2_dependency_declaration.py` & `propan-0.1.2.3/examples/dependencies/2_dependency_declaration.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.1.2.3/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/dependencies/5_dependency_nesting.py` & `propan-0.1.2.3/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/dependencies/6_dependecy_calling.py` & `propan-0.1.2.3/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/dependencies/7_annotated.py` & `propan-0.1.2.3/examples/dependencies/7_annotated.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/blacksheep.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/falcon.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/fastapi.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/quart.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/quart.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/sanic.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/http_frameworks_integrations/tornado.py` & `propan-0.1.2.3/examples/http_frameworks_integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/rabbit/direct.py` & `propan-0.1.2.3/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/rabbit/fanout.py` & `propan-0.1.2.3/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/rabbit/header.py` & `propan-0.1.2.3/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/rabbit/topic.py` & `propan-0.1.2.3/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/redis/direct.py` & `propan-0.1.2.3/examples/redis/direct.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/examples/redis/pattern.py` & `propan-0.1.2.3/examples/redis/pattern.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/__init__.py` & `propan-0.1.2.3/propan/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,22 @@
     RedisBroker = None  # type: ignore
 
 try:
     from propan.brokers.kafka import KafkaBroker
 except Exception:
     KafkaBroker = None  # type: ignore
 
-assert any((RabbitBroker, NatsBroker, RedisBroker)), INSTALL_MESSAGE
+try:
+    from propan.brokers.sqs import SQSBroker
+except Exception:
+    SQSBroker = None  # type: ignore
+
+assert any(
+    (RabbitBroker, NatsBroker, RedisBroker, SQSBroker, KafkaBroker)
+), INSTALL_MESSAGE
 
 __all__ = (  # noqa: F405
     # app
     "PropanApp",
     # log
     "logger",
     "access_logger",
@@ -41,8 +48,9 @@
     "ContextRepo" "Alias",
     "Depends",
     # brokers
     "NatsBroker",
     "RabbitBroker",
     "RedisBroker",
     "KafkaBroker",
+    "SQSBroker",
 )
```

### Comparing `propan-0.1.2.2/propan/annotations.py` & `propan-0.1.2.3/propan/annotations.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,49 +15,70 @@
 try:
     import aio_pika
 
     from propan.brokers.rabbit import RabbitBroker as RB
 
     RabbitBroker = Annotated[RB, ContextField("broker")]
     RabbitMessage = Annotated[aio_pika.message.IncomingMessage, ContextField("message")]
+    Channel = Annotated[
+        aio_pika.robust_channel.RobustChannel, ContextField("broker._channel")
+    ]
 except Exception:
-    RabbitBroker = RabbitMessage = None  # type: ignore
+    RabbitBroker = RabbitMessage = Channel = None  # type: ignore
 
 
 try:
     from nats.aio.msg import Msg
 
     from propan.brokers.nats import NatsBroker as NB
 
     NatsBroker = Annotated[NB, ContextField("broker")]
     NatsMessage = Annotated[Msg, ContextField("message")]
 except Exception:
     NatsBroker = NatsMessage = None  # type: ignore
 
 
 try:
+    from redis.asyncio.client import Redis as R
+
     from propan.brokers.redis import RedisBroker as RedB
 
     RedisBroker = Annotated[RedB, ContextField("broker")]
+    Redis = Annotated[R, ContextField("broker._connection")]
 except Exception:
-    RedisBroker = None  # type: ignore
+    RedisBroker = Redis = None  # type: ignore
 
 
 try:
+    from aiokafka import AIOKafkaProducer
     from aiokafka.structs import ConsumerRecord
 
     from propan.brokers.kafka import KafkaBroker as KB
 
     KafkaBroker = Annotated[KB, ContextField("broker")]
     KafkaMessage = Annotated[ConsumerRecord, ContextField("message")]
+    Producer = Annotated[AIOKafkaProducer, ContextField("producer")]
 except Exception:
     KafkaBroker = KafkaMessage = None  # type: ignore
 
 
+try:
+    from aiobotocore.client import AioBaseClient
+
+    from propan.brokers.sqs import SQSBroker as SB
+
+    SQSBroker = Annotated[SB, ContextField("broker")]
+    client = Annotated[AioBaseClient, ContextField("client")]
+    queue_url = Annotated[str, ContextField("queue_url")]
+except Exception:
+    SQSBroker = client = queue_url = None  # type: ignore
+
+
 assert any(
     (
-        all((RabbitBroker, RabbitMessage)),
+        all((RabbitBroker, RabbitMessage, Channel)),
         all((NatsBroker, NatsMessage)),
-        RedisBroker,
-        all((KafkaBroker, KafkaMessage)),
+        all((RedisBroker, Redis)),
+        all((KafkaBroker, KafkaMessage, Producer)),
+        all((SQSBroker, client, queue_url)),
     )
 ), INSTALL_MESSAGE
```

### Comparing `propan-0.1.2.2/propan/types.py` & `propan-0.1.2.3/propan/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/brokers/push_back_watcher.py` & `propan-0.1.2.3/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/brokers/kafka/kafka_broker.py` & `propan-0.1.2.3/propan/brokers/kafka/kafka_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
+import logging
 from functools import partial, wraps
 from typing import Any, Callable, Dict, List, NoReturn, Optional, Sequence, Tuple, Union
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord
 from typing_extensions import TypeVar
 
 from propan.__about__ import __version__
+from propan.brokers._model.broker_usecase import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.kafka.schemas import Handler
-from propan.brokers.model.broker_usecase import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.types import (
     AnyCallable,
     AnyDict,
     DecoratedCallable,
     SendableMessage,
     Wrapper,
@@ -118,15 +119,15 @@
         for handler in self.handlers:  # pragma: no branch
             c = self._get_log_context(None, handler.topics)
             self._log(f"`{handler.callback.__name__}` waiting for messages", extra=c)
 
             consumer = self._connection(*handler.topics, **handler.consumer_kwargs)
             await consumer.start()
             handler.consumer = consumer
-            handler.task = asyncio.create_task(_consume(handler))
+            handler.task = asyncio.create_task(self._consume(handler))
 
     @staticmethod
     async def _parse_message(message: ConsumerRecord) -> PropanMessage:
         headers = {i: j.decode() for i, j in message.headers}
         return PropanMessage(
             body=message.value,
             raw_message=message,
@@ -183,24 +184,30 @@
             f"%(topic)-{self.__max_topic_len}s | "
             "%(message_id)-10s "
             "- %(message)s"
         )
 
     def _get_log_context(
         self,
-        message: PropanMessage,
+        message: Optional[PropanMessage],
         topics: Sequence[str] = (),
     ) -> Dict[str, Any]:
         if topics:
             topic = ", ".join(topics)
         else:
             topic = message.raw_message.topic
 
         return {
             "topic": topic,
             **super()._get_log_context(message),
         }
 
+    async def _consume(self, handler: Handler) -> NoReturn:
+        c = self._get_log_context(None, handler.topics)
 
-async def _consume(handler: Handler) -> NoReturn:
-    async for msg in handler.consumer:
-        await handler.callback(msg)
+        while True:
+            try:
+                msg = await handler.consumer.getone()
+            except Exception as e:
+                self._log(e, logging.WATNING, c)
+            else:
+                await handler.callback(msg)
```

### Comparing `propan-0.1.2.2/propan/brokers/kafka/kafka_broker.pyi` & `propan-0.1.2.3/propan/brokers/kafka/kafka_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from aiokafka.structs import ConsumerRecord
 from kafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from kafka.partitioner.default import DefaultPartitioner
 from typing_extensions import Literal, TypeVar
 
 from propan.__about__ import __version__
+from propan.brokers._model.broker_usecase import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.kafka.schemas import Handler
-from propan.brokers.model.broker_usecase import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import SendableMessage, Wrapper
 
 T = TypeVar("T")
 Partition = TypeVar("Partition")
 
@@ -182,10 +182,10 @@
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
     ) -> Any: ...
     @property
     def fmt(self) -> str: ...
     def _get_log_context(  # type: ignore[override]
         self,
-        message: PropanMessage,
+        message: Optional[PropanMessage],
         topics: Sequence[str] = (),
     ) -> Dict[str, Any]: ...
```

### Comparing `propan-0.1.2.2/propan/brokers/model/broker_usecase.py` & `propan-0.1.2.3/propan/brokers/_model/broker_usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
-from propan.brokers.model.schemas import (
+from propan.brokers._model.schemas import (
     ContentType,
     ContentTypes,
     PropanMessage,
     SendableModel,
 )
-from propan.brokers.model.utils import (
+from propan.brokers._model.utils import (
     change_logger_handlers,
     get_watcher,
     set_message_context,
     suppress_decor,
 )
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
@@ -76,14 +76,15 @@
         raise NotImplementedError()
 
     @abstractmethod
     async def publish(
         self,
         message: SendableMessage,
         *args: Any,
+        reply_to: str = "",
         callback: bool = False,
         callback_timeout: Optional[float] = None,
         raise_timeout: bool = False,
         **kwargs: Any,
     ) -> Any:
         raise NotImplementedError()
 
@@ -98,15 +99,15 @@
     @abstractmethod
     def _process_message(
         self, func: Callable[[PropanMessage], T], watcher: Optional[BaseWatcher]
     ) -> Callable[[PropanMessage], T]:
         raise NotImplementedError()
 
     def _get_log_context(
-        self, message: PropanMessage, **kwargs: Dict[str, str]
+        self, message: Optional[PropanMessage], **kwargs: Dict[str, str]
     ) -> Dict[str, Any]:
         return {
             "message_id": message.message_id[:10] if message else "",
         }
 
     @abstractmethod
     def handle(
```

### Comparing `propan-0.1.2.2/propan/brokers/model/schemas.py` & `propan-0.1.2.3/propan/brokers/_model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/brokers/model/utils.py` & `propan-0.1.2.3/propan/brokers/_model/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     func: Callable[[Any], Awaitable[T]]
 ) -> Callable[[Any], Awaitable[Optional[T]]]:
     @wraps(func)
     async def wrapper(message: Any, reraise_exc: bool = False) -> Optional[T]:
         try:
             return await func(message)
         except Exception as e:
+            print(e)
             if reraise_exc is True:
                 raise e
             return None
 
     return wrapper
```

### Comparing `propan-0.1.2.2/propan/brokers/nats/nats_broker.py` & `propan-0.1.2.3/propan/brokers/nats/nats_broker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,59 @@
 import asyncio
+import logging
 from functools import wraps
 from secrets import token_hex
 from typing import Any, Callable, Dict, List, Optional, TypeVar
 
 import nats
-from nats.aio.client import Client
+from nats.aio.client import Callback, Client, ErrorCallback
 from nats.aio.msg import Msg
 
-from propan.brokers.model import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.types import AnyDict, DecoratedCallable, SendableMessage
 
 T = TypeVar("T")
 
 
 class NatsBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[Client]
 
     __max_queue_len: int
     __max_subject_len: int
+    __is_connected: bool
 
     def __init__(self, *args: Any, log_fmt: Optional[str] = None, **kwargs: AnyDict):
         super().__init__(*args, log_fmt=log_fmt, **kwargs)
 
         self._connection = None
 
         self.__max_queue_len = 0
         self.__max_subject_len = 4
+        self.__is_connected = True
 
     async def _connect(
         self,
         *args: Any,
         url: Optional[str] = None,
+        error_cb: Optional[ErrorCallback] = None,
+        reconnected_cb: Optional[Callback] = None,
         **kwargs: Any,
     ) -> Client:
         if url is not None:
             kwargs["servers"] = kwargs.pop("servers", []) + [url]
-        return await nats.connect(*args, **kwargs)
+        return await nats.connect(
+            *args,
+            error_cb=self.log_connection_broken(error_cb),
+            reconnected_cb=self.log_reconnected(reconnected_cb),
+            **kwargs,
+        )
 
     def handle(
         self,
         subject: str,
         queue: str = "",
         **original_kwargs,
     ) -> Callable[[DecoratedCallable], None]:
@@ -180,7 +190,35 @@
 
             if message.reply_to:
                 await self.publish(r, message.reply_to)
 
             return r
 
         return wrapper
+
+    def log_connection_broken(
+        self, error_cb: Optional[ErrorCallback] = None
+    ) -> ErrorCallback:
+        c = self._get_log_context(None, "")
+
+        async def wrapper(err: Exception) -> None:
+            if error_cb is not None:
+                await error_cb(err)
+
+            if self.__is_connected is True:
+                self._log(err, logging.WARNING, c)
+                self.__is_connected = False
+
+        return wrapper
+
+    def log_reconnected(self, cb: Optional[Callback] = None) -> Callback:
+        c = self._get_log_context(None, "")
+
+        async def wrapper() -> None:
+            if cb is not None:
+                await cb()
+
+            if self.__is_connected is False:
+                self._log("Connection established", logging.INFO, c)
+                self.__is_connected = True
+
+        return wrapper
```

### Comparing `propan-0.1.2.2/propan/brokers/nats/nats_broker.pyi` & `propan-0.1.2.3/propan/brokers/nats/nats_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     Credentials,
     ErrorCallback,
     JWTCallback,
     SignatureCallback,
 )
 from nats.aio.msg import Msg
 
-from propan.brokers.model import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
 from propan.types import HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
```

### Comparing `propan-0.1.2.2/propan/brokers/nats/nats_js_broker.py` & `propan-0.1.2.3/propan/brokers/nats/nats_js_broker.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/brokers/nats/schemas.py` & `propan-0.1.2.3/propan/brokers/nats/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from typing import Optional, Sequence
 
 from nats.aio.subscription import Subscription
 from nats.js.api import DEFAULT_PREFIX
 from pydantic import BaseModel
 
-from propan.brokers.model.schemas import BaseHandler
+from propan.brokers._model.schemas import BaseHandler
 
 
 @dataclass
 class Handler(BaseHandler):
     subject: str
     queue: str = ""
```

### Comparing `propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.py` & `propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar, Union
 from uuid import uuid4
 
 import aio_pika
 import aiormq
 from aio_pika.abc import DeliveryMode
 
-from propan.brokers.model import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher, WatcherContext
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.types import AnyDict, DecoratedCallable, HandlerWrapper, SendableMessage
 
 TimeoutType = Optional[Union[int, float]]
 PikaSendableMessage = Union[aio_pika.message.Message, SendableMessage]
 T = TypeVar("T")
```

### Comparing `propan-0.1.2.2/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.1.2.3/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import aio_pika
 import aiormq
 from pamqp.common import FieldTable
 from typing_extensions import ParamSpec
 from yarl import URL
 
-from propan.brokers.model import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
 from propan.types import SendableMessage
 
 P = ParamSpec("P")
 T = TypeVar("T")
```

### Comparing `propan-0.1.2.2/propan/brokers/rabbit/schemas.py` & `propan-0.1.2.3/propan/brokers/rabbit/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from aio_pika.abc import ExchangeType, TimeoutType
 from pydantic import Field
 
-from propan.brokers.model.schemas import BaseHandler, NameRequired, Queue
+from propan.brokers._model.schemas import BaseHandler, NameRequired, Queue
 
 __all__ = (
     "RabbitQueue",
     "RabbitExchange",
     "Handler",
     "ExchangeType",
 )
```

### Comparing `propan-0.1.2.2/propan/brokers/redis/redis_broker.py` & `propan-0.1.2.3/propan/brokers/redis/redis_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import asyncio
 import logging
 from functools import wraps
 from typing import Any, Callable, Coroutine, Dict, List, NoReturn, Optional, TypeVar
 from uuid import uuid4
 
 from redis.asyncio.client import PubSub, Redis
+from redis.asyncio.connection import ConnectionPool, parse_url
 
-from propan.brokers.model import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage, RawDecoced
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage, RawDecoced
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.redis.schemas import Handler, RedisMessage
 from propan.types import (
     AnyCallable,
     DecodedMessage,
     DecoratedCallable,
     HandlerWrapper,
@@ -40,15 +41,18 @@
         self._polling_interval = polling_interval
 
     async def _connect(
         self,
         url: str,
         **kwargs: Any,
     ) -> Redis:
-        return Redis.from_url(url, **kwargs)
+        url_options = parse_url(url)
+        url_options.update(kwargs)
+        pool = ConnectionPool(**url_options)
+        return Redis(connection_pool=pool)
 
     async def connect(
         self,
         url: Optional[str] = None,
         *args: Any,
         **kwargs: Any,
     ) -> Coroutine[Any, Any, Any]:
@@ -204,15 +208,17 @@
 
     async def _decode_message(self, message: PropanMessage) -> DecodedMessage:
         if message.headers.get("content-type") is not None:
             return await super()._decode_message(message)
         else:
             return RawDecoced(message=message.body).message
 
-    def _get_log_context(self, message: PropanMessage, channel: str) -> Dict[str, Any]:
+    def _get_log_context(
+        self, message: Optional[PropanMessage], channel: str
+    ) -> Dict[str, Any]:
         context = {
             "channel": channel,
             **super()._get_log_context(message),
         }
         return context
 
     @property
```

### Comparing `propan-0.1.2.2/propan/brokers/redis/redis_broker.pyi` & `propan-0.1.2.3/propan/brokers/redis/redis_broker.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from typing import Any, Callable, Dict, List, Mapping, Optional, Type, TypeVar, Union
 
 from redis.asyncio.client import Redis
 from redis.asyncio.connection import BaseParser, Connection, DefaultParser, Encoder
 
-from propan.brokers.model import BrokerUsecase
-from propan.brokers.model.schemas import PropanMessage
+from propan.brokers._model import BrokerUsecase
+from propan.brokers._model.schemas import PropanMessage
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.redis.schemas import Handler
 from propan.log import access_logger
 from propan.types import DecodedMessage, HandlerWrapper, SendableMessage
 
 T = TypeVar("T")
 
@@ -46,15 +46,15 @@
         encoder_class: Type[Encoder] = Encoder,
         # broker kwargs
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
     ) -> None: ...
-    async def _connect(
+    async def connect(
         self,
         url: str = "redis://localhost:6379",
         host: str = "localhost",
         port: Union[str, int] = 6379,
         db: Union[str, int] = 0,
         password: Optional[str] = None,
         socket_timeout: Optional[float] = None,
@@ -69,14 +69,15 @@
         parser_class: Type[BaseParser] = DefaultParser,
         socket_read_size: int = 65536,
         health_check_interval: float = 0,
         client_name: Optional[str] = None,
         username: Optional[str] = None,
         encoder_class: Type[Encoder] = Encoder,
     ) -> Redis[bytes]: ...
+    async def _connect(self, *args: Any, **kwargs: Any) -> Redis[bytes]: ...
     async def close(self) -> None: ...
     @staticmethod
     async def _parse_message(message: Any) -> PropanMessage: ...
     def _process_message(
         self,
         func: Callable[[PropanMessage], T],
         watcher: Optional[BaseWatcher],
@@ -84,15 +85,15 @@
     def handle(  # type: ignore[override]
         self,
         channel: str,
         *,
         pattern: bool = False,
     ) -> HandlerWrapper: ...
     def _get_log_context(  # type: ignore[override]
-        self, message: PropanMessage, channel: str
+        self, message: Optional[PropanMessage], channel: str
     ) -> Dict[str, Any]: ...
     @staticmethod
     async def _decode_message(message: PropanMessage) -> DecodedMessage: ...
     @property
     def fmt(self) -> str: ...
     async def start(self) -> None: ...
     async def publish(  # type: ignore[override]
```

### Comparing `propan-0.1.2.2/propan/brokers/redis/schemas.py` & `propan-0.1.2.3/propan/brokers/redis/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from pydantic import BaseModel, Field
 from redis.asyncio.client import PubSub
 
-from propan.brokers.model.schemas import BaseHandler
+from propan.brokers._model.schemas import BaseHandler
 
 
 @dataclass
 class Handler(BaseHandler):
     channel: str
     pattern: bool = False
```

### Comparing `propan-0.1.2.2/propan/cli/app.py` & `propan-0.1.2.3/propan/cli/app.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/main.py` & `propan-0.1.2.3/propan/cli/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/startproject/core.py` & `propan-0.1.2.3/propan/cli/startproject/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -63,31 +63,36 @@
     write_file(
         config_dir / ".env",
         "APP_DEBUG=True",
         f"APP_BROKER__URL={url}",
     )
 
 
-def create_config_dir(config: Path) -> Path:
+def create_config_dir(config: Path, *broker_settings: str) -> Path:
+    if not broker_settings:
+        broker_settings = (
+            "class BrokerSettings(BaseModel):",
+            "    url: str = Field(...)",
+        )
+
     config_dir = touch_dir(config)
 
     write_file(
         config_dir / "settings.py",
         "from pathlib import Path",
         "from typing import Optional",
         "",
         "from pydantic import BaseSettings, BaseModel, Field",
         "",
         "",
         "CONFIG_DIR = Path(__file__).resolve().parent",
         "BASE_DIR = CONFIG_DIR.parent",
         "",
         "",
-        "class BrokerSettings(BaseModel):",
-        "    url: str = Field(...)",
+        *broker_settings,
         "",
         "",
         "class Settings(BaseSettings):",
         "    debug: bool = Field(True)",
         "    broker: BrokerSettings = Field(default_factory=BrokerSettings)",
         "    base_dir: Path = BASE_DIR",
         "",
```

### Comparing `propan-0.1.2.2/propan/cli/startproject/async_app/app.py` & `propan-0.1.2.3/propan/cli/startproject/async_app/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import typer
 
 from propan.cli.startproject.async_app.kafka import create_kafka
 from propan.cli.startproject.async_app.nats import create_nats
 from propan.cli.startproject.async_app.rabbit import create_rabbit
 from propan.cli.startproject.async_app.redis import create_redis
+from propan.cli.startproject.async_app.sqs import create_sqs
 
 async_app = typer.Typer(pretty_exceptions_short=True)
 
 
 @async_app.command()
 def rabbit(appname: str) -> None:
     """Create an asyncronous RabbiMQ Propan project at [APPNAME] directory"""
@@ -32,7 +33,14 @@
 
 
 @async_app.command()
 def kafka(appname: str) -> None:
     """Create an asyncronous Kafka Propan project at [APPNAME] directory"""
     project = create_kafka(Path.cwd() / appname)
     typer.echo(f"Create an asyncronous Kafka Propan project at: {project}")
+
+
+@async_app.command()
+def sqs(appname: str) -> None:
+    """Create an asyncronous SQS Propan project at [APPNAME] directory"""
+    project = create_sqs(Path.cwd() / appname)
+    typer.echo(f"Create an asyncronous SQS Propan project at: {project}")
```

### Comparing `propan-0.1.2.2/propan/cli/startproject/async_app/core.py` & `propan-0.1.2.3/propan/cli/startproject/async_app/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from pathlib import Path
+from typing import Sequence
 
 from propan.cli.startproject.utils import write_file
 
 
-def create_app_file(app_dir: Path, broker_annotation: str) -> None:
+def create_app_file(
+    app_dir: Path,
+    broker_annotation: str,
+    imports: Sequence[str] = (),
+    broker_init: Sequence[str] = ("    await broker.connect(settings.broker.url)",),
+) -> None:
     write_file(
         app_dir / "serve.py",
         "import logging",
         "from typing import Optional",
         "",
+        *imports,
         "from propan import PropanApp",
         f"from propan.annotations import {broker_annotation}, ContextRepo",
+        "",
         "from core import broker",
         "from config import init_settings",
         "",
         "from apps import *  # import to register handlers  # NOQA",
         "",
         "",
         "app = PropanApp(broker)",
@@ -25,13 +33,13 @@
         "    settings = init_settings(env)",
         '    context.set_global("settings", settings)',
         "",
         "    logger_level = logging.DEBUG if settings.debug else logging.INFO",
         "    app.logger.setLevel(logger_level)",
         "    broker.logger.setLevel(logger_level)",
         "",
-        "    await broker.connect(settings.broker.url)",
+        *broker_init,
         "",
         "",
         'if __name__ == "__main__":',
         "    app.run()",
     )
```

### Comparing `propan-0.1.2.2/propan/cli/startproject/async_app/kafka.py` & `propan-0.1.2.3/propan/cli/startproject/async_app/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/startproject/async_app/nats.py` & `propan-0.1.2.3/propan/cli/startproject/async_app/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/startproject/async_app/rabbit.py` & `propan-0.1.2.3/propan/cli/startproject/async_app/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/startproject/async_app/redis.py` & `propan-0.1.2.3/propan/cli/startproject/async_app/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/supervisors/basereload.py` & `propan-0.1.2.3/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/supervisors/multiprocess.py` & `propan-0.1.2.3/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/supervisors/utils.py` & `propan-0.1.2.3/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/supervisors/watchfiles.py` & `propan-0.1.2.3/propan/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/utils/imports.py` & `propan-0.1.2.3/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/utils/logs.py` & `propan-0.1.2.3/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/cli/utils/parser.py` & `propan-0.1.2.3/propan/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/fastapi/__init__.py` & `propan-0.1.2.3/propan/fastapi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,10 +16,17 @@
     KafkaRouter = None  # type: ignore
 
 try:
     from propan.fastapi.nats import NatsRouter
 except Exception:
     NatsRouter = None  # type: ignore
 
-assert any((RabbitRouter, RedisRouter, KafkaRouter, NatsRouter)), INSTALL_MESSAGE
+try:
+    from propan.fastapi.sqs import SQSRouter
+except Exception:
+    SQSRouter = None  # type: ignore
+
+assert any(
+    (RabbitRouter, RedisRouter, KafkaRouter, NatsRouter, SQSRouter)
+), INSTALL_MESSAGE
 
-__all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter", "NatsRouter")
+__all__ = ("RabbitRouter", "RedisRouter", "KafkaRouter", "NatsRouter", "SQSRouter")
```

### Comparing `propan-0.1.2.2/propan/fastapi/core/route.py` & `propan-0.1.2.3/propan/fastapi/core/route.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,38 +6,38 @@
 from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_dependant, solve_dependencies
 from fastapi.routing import run_endpoint_function
 from pydantic import ValidationError, create_model
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
-from propan.brokers.model import BrokerUsecase
+from propan.brokers._model import BrokerUsecase
 from propan.types import AnyDict
 
 NativeMessage = Union[str, AnyDict, bytes]
 
 
 class PropanRoute(BaseRoute):
     def __init__(
         self,
         path: str,
         endpoint: Callable[..., Any],
         broker: BrokerUsecase,
         *,
         dependency_overrides_provider: Optional[Any] = None,
-        **hanle_kwargs: AnyDict,
+        **handle_kwargs: AnyDict,
     ) -> None:
         self.path = path
         self.broker = broker
         self.dependant = get_dependant(path=path, call=endpoint)
 
         handler = PropanMessage.get_session(
             self.dependant, dependency_overrides_provider
         )
-        broker.handle(path, **hanle_kwargs)(handler)  # type: ignore
+        broker.handle(path, **handle_kwargs)(handler)  # type: ignore
 
 
 class PropanMessage(Request):
     scope: AnyDict
     _cookies: AnyDict
     _headers: AnyDict  # type: ignore
     _body: AnyDict  # type: ignore
```

### Comparing `propan-0.1.2.2/propan/fastapi/core/router.py` & `propan-0.1.2.3/propan/fastapi/core/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fastapi.types import DecoratedCallable
 from fastapi.utils import generate_unique_id
 from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.types import ASGIApp
 from typing_extensions import ClassVar
 
-from propan.brokers.model import BrokerUsecase
+from propan.brokers._model import BrokerUsecase
 from propan.fastapi.core.route import PropanRoute
 from propan.types import AnyDict
 
 
 class PropanRouter(APIRouter):
     broker_class: ClassVar[Type[BrokerUsecase]]
     broker: BrokerUsecase
```

### Comparing `propan-0.1.2.2/propan/fastapi/kafka/router.pyi` & `propan-0.1.2.3/propan/fastapi/kafka/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/fastapi/nats/router.pyi` & `propan-0.1.2.3/propan/fastapi/nats/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/fastapi/rabbit/router.pyi` & `propan-0.1.2.3/propan/fastapi/rabbit/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/fastapi/redis/router.pyi` & `propan-0.1.2.3/propan/fastapi/redis/router.pyi`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/log/formatter.py` & `propan-0.1.2.3/propan/log/formatter.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/log/logging.py` & `propan-0.1.2.3/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/test/__init__.py` & `propan-0.1.2.3/propan/test/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,17 +16,23 @@
     TestKafkaBroker = None  # type: ignore
 
 try:
     from propan.test.nats import TestNatsBroker
 except Exception:
     TestNatsBroker = None  # type: ignore
 
+try:
+    from propan.test.sqs import TestSQSBroker
+except Exception:
+    TestSQSBroker = None  # type: ignore
+
 assert any(
-    (TestRabbitBroker, TestRedisBroker, TestKafkaBroker, TestNatsBroker)
+    (TestRabbitBroker, TestRedisBroker, TestKafkaBroker, TestNatsBroker, TestSQSBroker)
 ), INSTALL_MESSAGE
 
 __all__ = (
     "TestRabbitBroker",
     "TestRedisBroker",
     "TestKafkaBroker",
     "TestNatsBroker",
+    "TestSQSBroker",
 )
```

### Comparing `propan-0.1.2.2/propan/test/kafka.py` & `propan-0.1.2.3/propan/test/kafka.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/test/nats.py` & `propan-0.1.2.3/propan/test/nats.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/test/rabbit.py` & `propan-0.1.2.3/propan/test/rabbit.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/test/redis.py` & `propan-0.1.2.3/propan/test/redis.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/test/utils.py` & `propan-0.1.2.3/propan/test/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from typing import Any, Optional
 
-from propan.brokers.model.schemas import BaseHandler
+from propan.brokers._model.schemas import BaseHandler
 
 
 async def call_handler(
     handler: BaseHandler,
     message: Any,
     callback: bool = False,
     callback_timeout: Optional[float] = 30.0,
```

### Comparing `propan-0.1.2.2/propan/utils/functions.py` & `propan-0.1.2.3/propan/utils/functions.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/utils/context/main.py` & `propan-0.1.2.3/propan/utils/context/main.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/propan/utils/context/types.py` & `propan-0.1.2.3/propan/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/LICENSE` & `propan-0.1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.1.2.2/README.md` & `propan-0.1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 
 ### Supported MQ brokers
 
 |                   | async                                                   | sync                 |
 |-------------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
-| **Nats**          | :heavy_check_mark: **beta** :heavy_check_mark:          | :mag: planning :mag: |
+| **Nats**          | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag: |
-| **SQS**           | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
+| **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
@@ -140,29 +140,33 @@
 pip install "propan[async-rabbit]"
 # or
 pip install "propan[async-nats]"
 # or
 pip install "propan[async-redis]"
 # or
 pip install "propan[async-kafka]"
+# or
+pip install "propan[async-sqs]"
 ```
 
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
 from propan import PropanApp
 from propan import RabbitBroker
 # from propan import RedisBroker
 # from propan import NatsBroker
+# from propan import SQSBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
 # broker = RedisBroker("redis://localhost:6379")
+# broker = SQSBroker("http://localhost:9324", ...)
 
 app = PropanApp(broker)
 
 @broker.handle("test")
 async def base_handler(body):
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
```

#### html2text {}

```diff
@@ -22,50 +22,51 @@
 the project environment * application code *hot reload* * robust application
 templates * **Testability**: **Propan** allows you to test your app without
 external dependencies: you do not have to set up a Message Broker, you can use
 a virtual one! ### Supported MQ brokers | | async | sync | |-------------------
 |:-------------------------------------------------------:|:-------------------
 -:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
 planning :mag: | | **Redis** | :heavy_check_mark: **stable** :heavy_check_mark:
-| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **beta** :
+| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **stable** :
 heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **SQS** | :hammer_and_wrench: **in
-progress** :hammer_and_wrench: | :mag: planning :mag: | | **NatsJS** | :
-hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
-| **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams**
-| :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :
-mag: | :mag: planning :mag: | ### Community If you are interested in this
-project, please give me feedback by star or/and watch repository. If you have
-any questions or ideas about features to implement, welcome to [discussions]
-(https://github.com/Lancetnik/Propan/discussions). --- ## Declarative? With
-declarative tools you can define **what you need to get**. With traditional
-imperative tools you must write **what you need to do**. Take a look at classic
-imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
-**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
-async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
-guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
-await connection.channel() queue = await channel.declare_queue(queue_name)
-async with queue.iterator() as queue_iter: async for message in queue_iter:
-async with message.process(): print(message.body) asyncio.run(main()) ```
-**aio-pika** is a great tool with a really easy learning curve. But it's still
-imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
-yourself. Also, you need to manage *connection*, *message*, *queue* context to
-avoid any troubles. It is not a bad way, but it can be much easier. ```python
-from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
-async def base_handler(body): print(body) ``` This is the **Propan**
-declarative way to write the same code. That is so much easier, isn't it? --
-- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
-rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
-redis]" # or pip install "propan[async-kafka]" ``` ### Basic usage Create an
+warning: | :mag: planning :mag: | | **SQS** | :warning: **beta** :warning: | :
+mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :
+hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
+:mag: planning :mag: | | **Redis Streams** | :mag: planning :mag: | :mag:
+planning :mag: | | **Pulsar** | :mag: planning :mag: | :mag: planning :mag: |
+### Community If you are interested in this project, please give me feedback by
+star or/and watch repository. If you have any questions or ideas about features
+to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
+discussions). --- ## Declarative? With declarative tools you can define **what
+you need to get**. With traditional imperative tools you must write **what you
+need to do**. Take a look at classic imperative tools, such as aio-pika, pika,
+redis-py, nats-py, etc. This is the **Quickstart** with the *aio-pika*:
+```python import asyncio import aio_pika async def main(): connection = await
+aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
+"test_queue" async with connection: channel = await connection.channel() queue
+= await channel.declare_queue(queue_name) async with queue.iterator() as
+queue_iter: async for message in queue_iter: async with message.process():
+print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be much easier. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
+kafka]" # or pip install "propan[async-sqs]" ``` ### Basic usage Create an
 application with the following code at `serve.py`: ```python from propan import
 PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
-= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
+from propan import NatsBroker # from propan import SQSBroker broker =
+RabbitBroker("amqp://guest:guest@localhost:5672/") # broker = NatsBroker("nats:
+//localhost:4222") # broker = RedisBroker("redis://localhost:6379") # broker =
+SQSBroker("http://localhost:9324", ...) app = PropanApp(broker) @broker.handle
 ("test") async def base_handler(body): '''Handle all default exchange messages
 with `test` routing key''' print(body) ``` And just run it: ```shell propan run
 serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
 function arguments to types according to their annotation. ```python from
 pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
 (broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
```

### Comparing `propan-0.1.2.2/pyproject.toml` & `propan-0.1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,24 @@
     "redis>=4.2.0rc1"
 ]
 
 async-kafka = [
     "aiokafka>=0.8"
 ]
 
+async-sqs = [
+    "aiobotocore"
+]
+
 test = [
     "propan[async-rabbit]",
     "propan[async-nats]",
     "propan[async-redis]",
     "propan[async-kafka]",
+    "propan[async-sqs]",
 
     "coverage[toml]>=7.2",
     "pytest>=7",
     "pytest-asyncio>=0.21",
 
     "fastapi",
 
@@ -212,14 +217,15 @@
 ]
 markers = [
     "slow",
     "rabbit",
     "nats",
     "redis",
     "kafka",
+    "sqs",
     "all",
 ]
 
 [tool.coverage.run]
 parallel = true
 branch = true
 concurrency = [
```

### Comparing `propan-0.1.2.2/PKG-INFO` & `propan-0.1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.1.2.2
+Version: 0.1.2.3
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -43,14 +43,16 @@
 Requires-Dist: aiokafka>=0.8; extra == 'async-kafka'
 Provides-Extra: async-nats
 Requires-Dist: nats-py>=2; extra == 'async-nats'
 Provides-Extra: async-rabbit
 Requires-Dist: aio-pika>=9; extra == 'async-rabbit'
 Provides-Extra: async-redis
 Requires-Dist: redis>=4.2.0rc1; extra == 'async-redis'
+Provides-Extra: async-sqs
+Requires-Dist: aiobotocore; extra == 'async-sqs'
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev'
 Requires-Dist: mypy==1.1.1; extra == 'dev'
 Requires-Dist: propan[doc]; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev'
 Requires-Dist: ruff==0.0.261; extra == 'dev'
@@ -66,14 +68,15 @@
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
 Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi; extra == 'test'
 Requires-Dist: propan[async-kafka]; extra == 'test'
 Requires-Dist: propan[async-nats]; extra == 'test'
 Requires-Dist: propan[async-rabbit]; extra == 'test'
 Requires-Dist: propan[async-redis]; extra == 'test'
+Requires-Dist: propan[async-sqs]; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.21; extra == 'test'
 Requires-Dist: pytest>=7; extra == 'test'
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="https://lancetnik.github.io/Propan/" target="_blank">
         <img src="https://lancetnik.github.io/Propan/assets/img/logo-no-background.png" alt="Propan logo" style="height: 250px; width: 600px;"/>
@@ -136,17 +139,17 @@
 
 ### Supported MQ brokers
 
 |                   | async                                                   | sync                 |
 |-------------------|:-------------------------------------------------------:|:--------------------:|
 | **RabbitMQ**      | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Redis**         | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
-| **Nats**          | :heavy_check_mark: **beta** :heavy_check_mark:          | :mag: planning :mag: |
+| **Nats**          | :heavy_check_mark: **stable** :heavy_check_mark:        | :mag: planning :mag: |
 | **Kafka**         | :warning: **beta** :warning:                            | :mag: planning :mag: |
-| **SQS**           | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
+| **SQS**           | :warning: **beta** :warning:                            | :mag: planning :mag: |
 | **NatsJS**        | :hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
 | **MQTT**          | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Redis Streams** | :mag: planning :mag:                                    | :mag: planning :mag: |
 | **Pulsar**        | :mag: planning :mag:                                    | :mag: planning :mag: |
 
 ### Community
 
@@ -216,29 +219,33 @@
 pip install "propan[async-rabbit]"
 # or
 pip install "propan[async-nats]"
 # or
 pip install "propan[async-redis]"
 # or
 pip install "propan[async-kafka]"
+# or
+pip install "propan[async-sqs]"
 ```
 
 ### Basic usage
 
 Create an application with the following code at `serve.py`:
 
 ```python
 from propan import PropanApp
 from propan import RabbitBroker
 # from propan import RedisBroker
 # from propan import NatsBroker
+# from propan import SQSBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 # broker = NatsBroker("nats://localhost:4222")
 # broker = RedisBroker("redis://localhost:6379")
+# broker = SQSBroker("http://localhost:9324", ...)
 
 app = PropanApp(broker)
 
 @broker.handle("test")
 async def base_handler(body):
     '''Handle all default exchange messages with `test` routing key'''
     print(body)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.1.2.2 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.1.2.3 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-File: LICENSE Keywords: framework,message brokers,rabbitmq
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -24,30 +24,32 @@
 Typed Requires-Python: >=3.7 Requires-Dist: fast-depends>=1.1.4 Requires-Dist:
 typer Requires-Dist: uvloop!=0.15.0,!=0.15.1,>=0.14.0; sys_platform != 'win32'
 and (sys_platform != 'cygwin' and platform_python_implementation != 'PyPy')
 Requires-Dist: watchfiles Provides-Extra: async-kafka Requires-Dist:
 aiokafka>=0.8; extra == 'async-kafka' Provides-Extra: async-nats Requires-Dist:
 nats-py>=2; extra == 'async-nats' Provides-Extra: async-rabbit Requires-Dist:
 aio-pika>=9; extra == 'async-rabbit' Provides-Extra: async-redis Requires-Dist:
-redis>=4.2.0rc1; extra == 'async-redis' Provides-Extra: dev Requires-Dist:
+redis>=4.2.0rc1; extra == 'async-redis' Provides-Extra: async-sqs Requires-
+Dist: aiobotocore; extra == 'async-sqs' Provides-Extra: dev Requires-Dist:
 black==23.3.0; extra == 'dev' Requires-Dist: isort>=5; extra == 'dev' Requires-
 Dist: mypy==1.1.1; extra == 'dev' Requires-Dist: propan[doc]; extra == 'dev'
 Requires-Dist: propan[test]; extra == 'dev' Requires-Dist: ruff==0.0.261; extra
 == 'dev' Requires-Dist: typer[all]; extra == 'dev' Requires-Dist: types-redis;
 extra == 'dev' Provides-Extra: doc Requires-Dist: mdx-include<2.0.0,>=1.4.1;
 extra == 'doc' Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7;
 extra == 'doc' Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Requires-Dist: mkdocs-static-i18n; extra == 'doc' Requires-Dist: typer[all];
 extra == 'doc' Provides-Extra: test Requires-Dist: asyncmock; python_version <
 '3.8' and extra == 'test' Requires-Dist: coverage[toml]>=7.2; extra == 'test'
 Requires-Dist: fastapi; extra == 'test' Requires-Dist: propan[async-kafka];
 extra == 'test' Requires-Dist: propan[async-nats]; extra == 'test' Requires-
 Dist: propan[async-rabbit]; extra == 'test' Requires-Dist: propan[async-redis];
-extra == 'test' Requires-Dist: pytest-asyncio>=0.21; extra == 'test' Requires-
-Dist: pytest>=7; extra == 'test' Description-Content-Type: text/markdown
+extra == 'test' Requires-Dist: propan[async-sqs]; extra == 'test' Requires-
+Dist: pytest-asyncio>=0.21; extra == 'test' Requires-Dist: pytest>=7; extra ==
+'test' Description-Content-Type: text/markdown
                                  [Propan_logo]
           [Tests_coverage] [Coverage] [Package_version] [downloads]
                      [Supported_Python_versions] [GitHub]
 # Propan **Propan** - just *~~an another one HTTP~~* a **declarative Python MQ
 framework**. It's following by *fastapi*, simplify Message Brokers around code
 writing and provides a helpful development toolkit, which existed only in HTTP-
 frameworks world until now. It's designed to create reactive microservices
@@ -68,50 +70,51 @@
 the project environment * application code *hot reload* * robust application
 templates * **Testability**: **Propan** allows you to test your app without
 external dependencies: you do not have to set up a Message Broker, you can use
 a virtual one! ### Supported MQ brokers | | async | sync | |-------------------
 |:-------------------------------------------------------:|:-------------------
 -:| | **RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
 planning :mag: | | **Redis** | :heavy_check_mark: **stable** :heavy_check_mark:
-| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **beta** :
+| :mag: planning :mag: | | **Nats** | :heavy_check_mark: **stable** :
 heavy_check_mark: | :mag: planning :mag: | | **Kafka** | :warning: **beta** :
-warning: | :mag: planning :mag: | | **SQS** | :hammer_and_wrench: **in
-progress** :hammer_and_wrench: | :mag: planning :mag: | | **NatsJS** | :
-hammer_and_wrench: **in progress** :hammer_and_wrench: | :mag: planning :mag: |
-| **MQTT** | :mag: planning :mag: | :mag: planning :mag: | | **Redis Streams**
-| :mag: planning :mag: | :mag: planning :mag: | | **Pulsar** | :mag: planning :
-mag: | :mag: planning :mag: | ### Community If you are interested in this
-project, please give me feedback by star or/and watch repository. If you have
-any questions or ideas about features to implement, welcome to [discussions]
-(https://github.com/Lancetnik/Propan/discussions). --- ## Declarative? With
-declarative tools you can define **what you need to get**. With traditional
-imperative tools you must write **what you need to do**. Take a look at classic
-imperative tools, such as aio-pika, pika, redis-py, nats-py, etc. This is the
-**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
-async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
-guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
-await connection.channel() queue = await channel.declare_queue(queue_name)
-async with queue.iterator() as queue_iter: async for message in queue_iter:
-async with message.process(): print(message.body) asyncio.run(main()) ```
-**aio-pika** is a great tool with a really easy learning curve. But it's still
-imperative. You need to *connect*, declare *channel*, *queues*, *exchanges* by
-yourself. Also, you need to manage *connection*, *message*, *queue* context to
-avoid any troubles. It is not a bad way, but it can be much easier. ```python
-from propan import PropanApp, RabbitBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") app = PropanApp(broker) @broker.handle("test_queue")
-async def base_handler(body): print(body) ``` This is the **Propan**
-declarative way to write the same code. That is so much easier, isn't it? --
-- ## Quickstart Install using `pip`: ```shell pip install "propan[async-
-rabbit]" # or pip install "propan[async-nats]" # or pip install "propan[async-
-redis]" # or pip install "propan[async-kafka]" ``` ### Basic usage Create an
+warning: | :mag: planning :mag: | | **SQS** | :warning: **beta** :warning: | :
+mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :
+hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag: planning :mag: |
+:mag: planning :mag: | | **Redis Streams** | :mag: planning :mag: | :mag:
+planning :mag: | | **Pulsar** | :mag: planning :mag: | :mag: planning :mag: |
+### Community If you are interested in this project, please give me feedback by
+star or/and watch repository. If you have any questions or ideas about features
+to implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
+discussions). --- ## Declarative? With declarative tools you can define **what
+you need to get**. With traditional imperative tools you must write **what you
+need to do**. Take a look at classic imperative tools, such as aio-pika, pika,
+redis-py, nats-py, etc. This is the **Quickstart** with the *aio-pika*:
+```python import asyncio import aio_pika async def main(): connection = await
+aio_pika.connect_robust( "amqp://guest:guest@127.0.0.1/" ) queue_name =
+"test_queue" async with connection: channel = await connection.channel() queue
+= await channel.declare_queue(queue_name) async with queue.iterator() as
+queue_iter: async for message in queue_iter: async with message.process():
+print(message.body) asyncio.run(main()) ``` **aio-pika** is a great tool with a
+really easy learning curve. But it's still imperative. You need to *connect*,
+declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
+*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
+way, but it can be much easier. ```python from propan import PropanApp,
+RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
+PropanApp(broker) @broker.handle("test_queue") async def base_handler(body):
+print(body) ``` This is the **Propan** declarative way to write the same code.
+That is so much easier, isn't it? --- ## Quickstart Install using `pip`:
+```shell pip install "propan[async-rabbit]" # or pip install "propan[async-
+nats]" # or pip install "propan[async-redis]" # or pip install "propan[async-
+kafka]" # or pip install "propan[async-sqs]" ``` ### Basic usage Create an
 application with the following code at `serve.py`: ```python from propan import
 PropanApp from propan import RabbitBroker # from propan import RedisBroker #
-from propan import NatsBroker broker = RabbitBroker("amqp://guest:
-guest@localhost:5672/") # broker = NatsBroker("nats://localhost:4222") # broker
-= RedisBroker("redis://localhost:6379") app = PropanApp(broker) @broker.handle
+from propan import NatsBroker # from propan import SQSBroker broker =
+RabbitBroker("amqp://guest:guest@localhost:5672/") # broker = NatsBroker("nats:
+//localhost:4222") # broker = RedisBroker("redis://localhost:6379") # broker =
+SQSBroker("http://localhost:9324", ...) app = PropanApp(broker) @broker.handle
 ("test") async def base_handler(body): '''Handle all default exchange messages
 with `test` routing key''' print(body) ``` And just run it: ```shell propan run
 serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
 function arguments to types according to their annotation. ```python from
 pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
 (broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
```

