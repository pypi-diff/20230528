# Comparing `tmp/tradingkit-1.9.5.tar.gz` & `tmp/tradingkit-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingkit-1.9.5.tar", last modified: Tue Nov 30 14:37:37 2021, max compression
+gzip compressed data, was "tradingkit-1.9.6.tar", last modified: Wed Dec  1 10:46:59 2021, max compression
```

## Comparing `tradingkit-1.9.5.tar` & `tradingkit-1.9.6.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.892812 tradingkit-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-11-30 14:36:59.000000 tradingkit-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-11-30 14:36:59.000000 tradingkit-1.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6321 2021-11-30 14:37:37.892812 tradingkit-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5192 2021-11-30 14:36:59.000000 tradingkit-1.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-30 14:37:37.892812 tradingkit-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-11-30 14:36:59.000000 tradingkit-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.880812 tradingkit-1.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.880812 tradingkit-1.9.5/src/tradingkit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.880812 tradingkit-1.9.5/src/tradingkit/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7071 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     9625 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/cli/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/cli/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4109 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/config/config.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/data/adapter/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/adapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/adapter/bitmex_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/adapter/outlier_trade_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/data/feed/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/aggregator_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/backtest_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/bitmex_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/funding_backtest_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     9340 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/kraken_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/list_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2852 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/private_kraken_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/public_kraken_feeder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/feed/websocket_feeder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/data/fetch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/fetch/ccxt_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/data/fetch/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/display/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/display/highstock/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/highstock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14359 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/highstock/highstock_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/display/highstock/lib/
--rw-r--r--   0 runner    (1001) docker     (121)    11157 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/highstock/lib/index.html
--rw-r--r--   0 runner    (1001) docker     (121)    10167 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/highstock/lib/live.html
--rw-r--r--   0 runner    (1001) docker     (121)     8450 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/highstock/lib/live_balance.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.884812 tradingkit-1.9.5/src/tradingkit/display/highstock/server/
--rw-r--r--   0 runner    (1001) docker     (121)     3530 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/highstock/server/plot_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/none_plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/plotly_plotter.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/display/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.888812 tradingkit-1.9.5/src/tradingkit/exchange/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13472 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/exchange/bitmex_backtest.py
--rw-r--r--   0 runner    (1001) docker     (121)    14256 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/exchange/bridge_exchange.py
--rw-r--r--   0 runner    (1001) docker     (121)    10627 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/exchange/testex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.888812 tradingkit-1.9.5/src/tradingkit/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/notifications/logger_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/notifications/telegram_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.888812 tradingkit-1.9.5/src/tradingkit/pubsub/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.888812 tradingkit-1.9.5/src/tradingkit/pubsub/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/core/event.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/core/publisher.py
--rw-r--r--   0 runner    (1001) docker     (121)      246 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/core/subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.888812 tradingkit-1.9.5/src/tradingkit/pubsub/event/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/book.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/candle.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/funding.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/liquidation.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/open_order.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/order.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/position.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/pubsub/event/trade.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.888812 tradingkit-1.9.5/src/tradingkit/state_machine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/state_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/state_machine/state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.892812 tradingkit-1.9.5/src/tradingkit/strategy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/strategy/none_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/strategy/state_machine_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2731 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/strategy/strategy_event.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/strategy/strategy_state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.892812 tradingkit-1.9.5/src/tradingkit/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/config_injector.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/injector.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/serializable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2217 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2021-11-30 14:36:59.000000 tradingkit-1.9.5/src/tradingkit/utils/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 14:37:37.880812 tradingkit-1.9.5/src/tradingkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6321 2021-11-30 14:37:37.000000 tradingkit-1.9.5/src/tradingkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2021-11-30 14:37:37.000000 tradingkit-1.9.5/src/tradingkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-30 14:37:37.000000 tradingkit-1.9.5/src/tradingkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-30 14:37:37.000000 tradingkit-1.9.5/src/tradingkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      245 2021-11-30 14:37:37.000000 tradingkit-1.9.5/src/tradingkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-30 14:37:37.000000 tradingkit-1.9.5/src/tradingkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.690930 tradingkit-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-12-01 10:46:26.000000 tradingkit-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-01 10:46:26.000000 tradingkit-1.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6321 2021-12-01 10:46:59.686930 tradingkit-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5192 2021-12-01 10:46:26.000000 tradingkit-1.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-01 10:46:59.690930 tradingkit-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1688 2021-12-01 10:46:26.000000 tradingkit-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7071 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9625 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/cli/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/cli/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4109 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/config/config.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/data/adapter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/adapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/adapter/bitmex_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/adapter/outlier_trade_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/data/feed/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1421 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/aggregator_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2065 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/backtest_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4854 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/bitmex_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/funding_backtest_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9340 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/kraken_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/list_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2852 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/private_kraken_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/public_kraken_feeder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/feed/websocket_feeder.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/data/fetch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/fetch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4388 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/fetch/ccxt_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/data/fetch/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit/display/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/display/highstock/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/highstock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14359 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/highstock/highstock_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/display/highstock/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)    11157 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/highstock/lib/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)    10167 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/highstock/lib/live.html
+-rw-r--r--   0 runner    (1001) docker     (121)     8450 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/highstock/lib/live_balance.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/display/highstock/server/
+-rw-r--r--   0 runner    (1001) docker     (121)     3530 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/highstock/server/plot_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/none_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2358 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/plotly_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      222 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/display/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/exchange/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13472 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/exchange/bitmex_backtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14256 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/exchange/bridge_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10627 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/exchange/testex.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/notifications/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/notifications/logger_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/notifications/telegram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/pubsub/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/core/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/core/subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/pubsub/event/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/book.py
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/candle.py
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/funding.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/liquidation.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/open_order.py
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/order.py
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/position.py
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/pubsub/event/trade.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/state_machine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/state_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/state_machine/state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/strategy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/strategy/none_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/strategy/state_machine_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2731 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/strategy/strategy_event.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/strategy/strategy_state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.686930 tradingkit-1.9.6/src/tradingkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3910 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/config_injector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/injector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      608 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2217 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2021-12-01 10:46:26.000000 tradingkit-1.9.6/src/tradingkit/utils/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-01 10:46:59.682930 tradingkit-1.9.6/src/tradingkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6321 2021-12-01 10:46:59.000000 tradingkit-1.9.6/src/tradingkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3187 2021-12-01 10:46:59.000000 tradingkit-1.9.6/src/tradingkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-01 10:46:59.000000 tradingkit-1.9.6/src/tradingkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-01 10:46:59.000000 tradingkit-1.9.6/src/tradingkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      245 2021-12-01 10:46:59.000000 tradingkit-1.9.6/src/tradingkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-01 10:46:59.000000 tradingkit-1.9.6/src/tradingkit.egg-info/top_level.txt
```

### Comparing `tradingkit-1.9.5/LICENSE` & `tradingkit-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/PKG-INFO` & `tradingkit-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingkit
-Version: 1.9.5
+Version: 1.9.6
 Summary: Trading and backtesting framework for Python
 Home-page: https://github.com/logictraders/tradingkit
 Author: QBit Artifacts, SL
 Author-email: lluis@logictraders.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tradingkit-1.9.5/README.md` & `tradingkit-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/setup.py` & `tradingkit-1.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 setuptools.setup(
       name="tradingkit",
-      version="1.9.5",
+      version="1.9.6",
       author="QBit Artifacts, SL",
       author_email="lluis@logictraders.com",
       license="MIT",
       description="Trading and backtesting framework for Python",
       long_description=open("README.md", "r").read(),
       long_description_content_type="text/markdown",
       url="https://github.com/logictraders/tradingkit",
```

### Comparing `tradingkit-1.9.5/src/tradingkit/cli/cli.py` & `tradingkit-1.9.6/src/tradingkit/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/cli/optimizer.py` & `tradingkit-1.9.6/src/tradingkit/cli/optimizer.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/cli/runner.py` & `tradingkit-1.9.6/src/tradingkit/cli/runner.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/config/config.json` & `tradingkit-1.9.6/src/tradingkit/config/config.json`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/adapter/bitmex_normalizer.py` & `tradingkit-1.9.6/src/tradingkit/data/adapter/bitmex_normalizer.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/adapter/outlier_trade_filter.py` & `tradingkit-1.9.6/src/tradingkit/data/adapter/outlier_trade_filter.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/aggregator_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/aggregator_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/backtest_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/backtest_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/bitmex_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/bitmex_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/funding_backtest_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/funding_backtest_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/kraken_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/kraken_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/private_kraken_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/private_kraken_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/public_kraken_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/public_kraken_feeder.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/data/feed/websocket_feeder.py` & `tradingkit-1.9.6/src/tradingkit/data/feed/websocket_feeder.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
         ws = websocket.WebSocketApp(
             url=self.url,
             on_message=self.on_message,
             on_open=self.on_open,
             on_error=self.on_error,
             on_close=self.on_close,
         )
-        ws.run_forever(ping_interval=15, ping_timeout=10)
+        ws.run_forever(ping_interval=30, ping_timeout=25)
```

### Comparing `tradingkit-1.9.5/src/tradingkit/data/fetch/ccxt_fetcher.py` & `tradingkit-1.9.6/src/tradingkit/data/fetch/ccxt_fetcher.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/display/highstock/highstock_plotter.py` & `tradingkit-1.9.6/src/tradingkit/display/highstock/highstock_plotter.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/display/highstock/lib/index.html` & `tradingkit-1.9.6/src/tradingkit/display/highstock/lib/index.html`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/display/highstock/lib/live.html` & `tradingkit-1.9.6/src/tradingkit/display/highstock/lib/live.html`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/display/highstock/lib/live_balance.html` & `tradingkit-1.9.6/src/tradingkit/display/highstock/lib/live_balance.html`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/display/highstock/server/plot_server.py` & `tradingkit-1.9.6/src/tradingkit/display/highstock/server/plot_server.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/display/plotly_plotter.py` & `tradingkit-1.9.6/src/tradingkit/display/plotly_plotter.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/exchange/bitmex_backtest.py` & `tradingkit-1.9.6/src/tradingkit/exchange/bitmex_backtest.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/exchange/bridge_exchange.py` & `tradingkit-1.9.6/src/tradingkit/exchange/bridge_exchange.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/exchange/testex.py` & `tradingkit-1.9.6/src/tradingkit/exchange/testex.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/notifications/logger_handler.py` & `tradingkit-1.9.6/src/tradingkit/notifications/logger_handler.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/pubsub/core/publisher.py` & `tradingkit-1.9.6/src/tradingkit/pubsub/core/publisher.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/state_machine/state.py` & `tradingkit-1.9.6/src/tradingkit/state_machine/state.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/strategy/state_machine_strategy.py` & `tradingkit-1.9.6/src/tradingkit/strategy/state_machine_strategy.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/strategy/strategy.py` & `tradingkit-1.9.6/src/tradingkit/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/utils/config_injector.py` & `tradingkit-1.9.6/src/tradingkit/utils/config_injector.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/utils/request_handler.py` & `tradingkit-1.9.6/src/tradingkit/utils/request_handler.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/utils/system.py` & `tradingkit-1.9.6/src/tradingkit/utils/system.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit/utils/web_server.py` & `tradingkit-1.9.6/src/tradingkit/utils/web_server.py`

 * *Files identical despite different names*

### Comparing `tradingkit-1.9.5/src/tradingkit.egg-info/PKG-INFO` & `tradingkit-1.9.6/src/tradingkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingkit
-Version: 1.9.5
+Version: 1.9.6
 Summary: Trading and backtesting framework for Python
 Home-page: https://github.com/logictraders/tradingkit
 Author: QBit Artifacts, SL
 Author-email: lluis@logictraders.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tradingkit-1.9.5/src/tradingkit.egg-info/SOURCES.txt` & `tradingkit-1.9.6/src/tradingkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

