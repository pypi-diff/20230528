# Comparing `tmp/TradeGate-0.3.8.tar.gz` & `tmp/TradeGate-0.3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TradeGate-0.3.8.tar", last modified: Wed May 24 06:59:52 2023, max compression
+gzip compressed data, was "TradeGate-0.3.8.1.tar", last modified: Sun May 28 10:29:51 2023, max compression
```

## Comparing `TradeGate-0.3.8.tar` & `TradeGate-0.3.8.1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.364125 TradeGate-0.3.8/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1072 2022-02-23 07:14:51.000000 TradeGate-0.3.8/LICENSE
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2606 2023-05-24 06:59:52.364225 TradeGate-0.3.8/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2235 2022-06-20 05:37:13.000000 TradeGate-0.3.8/README.md
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.336282 TradeGate-0.3.8/TradeGates/
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.338953 TradeGate-0.3.8/TradeGates/Exchanges/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4226 2023-05-23 18:00:07.000000 TradeGate-0.3.8/TradeGates/Exchanges/BaseExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    32762 2023-05-23 18:00:07.000000 TradeGate-0.3.8/TradeGates/Exchanges/BinanceExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    33920 2023-05-24 06:56:49.000000 TradeGate-0.3.8/TradeGates/Exchanges/BybitExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    43852 2023-05-23 18:00:48.000000 TradeGate-0.3.8/TradeGates/Exchanges/KuCoinExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       83 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/Exchanges/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.339785 TradeGate-0.3.8/TradeGates/TradeGate.egg-info/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2606 2023-05-24 06:59:52.000000 TradeGate-0.3.8/TradeGates/TradeGate.egg-info/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5673 2023-05-24 06:59:52.000000 TradeGate-0.3.8/TradeGates/TradeGate.egg-info/SOURCES.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-05-24 06:59:52.000000 TradeGate-0.3.8/TradeGates/TradeGate.egg-info/dependency_links.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       89 2023-05-24 06:59:52.000000 TradeGate-0.3.8/TradeGates/TradeGate.egg-info/requires.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       67 2023-05-24 06:59:52.000000 TradeGate-0.3.8/TradeGates/TradeGate.egg-info/top_level.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    58566 2023-05-23 18:00:07.000000 TradeGate-0.3.8/TradeGates/TradeGate.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.341287 TradeGate-0.3.8/TradeGates/Utils/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4088 2022-06-27 15:23:02.000000 TradeGate-0.3.8/TradeGates/Utils/BinanceHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    13000 2022-06-27 15:23:02.000000 TradeGate-0.3.8/TradeGates/Utils/BybitHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7822 2022-06-27 15:23:02.000000 TradeGate-0.3.8/TradeGates/Utils/DataHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    13251 2022-06-19 05:59:28.000000 TradeGate-0.3.8/TradeGates/Utils/KuCoinHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       80 2022-10-02 08:05:21.000000 TradeGate-0.3.8/TradeGates/Utils/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.341640 TradeGate-0.3.8/TradeGates/Watchers/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/Watchers/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2561 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/Watchers/futureOrderWatchers.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.342633 TradeGate-0.3.8/TradeGates/binance_f/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      112 2022-02-23 05:49:50.000000 TradeGate-0.3.8/TradeGates/binance_f/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.343355 TradeGate-0.3.8/TradeGates/binance_f/base/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/base/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5597 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/base/printobject.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      597 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/base/printtime.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.343906 TradeGate-0.3.8/TradeGates/binance_f/constant/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/constant/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      399 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/constant/system.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      250 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/constant/test.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.344254 TradeGate-0.3.8/TradeGates/binance_f/exception/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/exception/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      422 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/exception/binanceapiexception.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.346089 TradeGate-0.3.8/TradeGates/binance_f/impl/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)       58 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2680 2022-02-26 09:29:35.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/restapiinvoker.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      310 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/restapirequest.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    36651 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/restapirequestimpl.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.347352 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      240 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1146 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/apisignature.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      156 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/channelparser.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5407 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/channels.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3139 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/inputchecker.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3400 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/jsonwrapper.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      434 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/timeservice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1030 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/utils/urlparamsbuilder.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     7819 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/websocketconnection.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      360 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/websocketrequest.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    15345 2022-03-03 18:09:37.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/websocketrequestimpl.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2243 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/impl/websocketwatchdog.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.357382 TradeGate-0.3.8/TradeGates/binance_f/model/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2976 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     4355 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/accountinformation.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5309 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/accountinformationv2.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2355 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/accountupdate.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      343 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/adlquantile.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      690 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/aggregatetrade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      971 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/aggregatetradeevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/apitradingstatus.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      999 2022-03-02 11:34:30.000000 TradeGate-0.3.8/TradeGates/binance_f/model/balance.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      854 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/balancev2.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      908 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/blvtinfoevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      706 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/blvtnavcandlestick.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1789 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/blvtnavcandlestickevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1607 2022-02-24 11:54:59.000000 TradeGate-0.3.8/TradeGates/binance_f/model/candlestick.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2230 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/candlestickevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      438 2022-03-04 10:50:30.000000 TradeGate-0.3.8/TradeGates/binance_f/model/codeandmsg.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1304 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/compositeindexevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2103 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/constant.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2389 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/continuouscandelstickevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      352 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/countdowncancelall.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1634 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/diffdepthevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3756 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/binance_f/model/exchangeinformation.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      433 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/fundingrate.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      791 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/binance_f/model/income.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/indexInfo.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      568 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/binance_f/model/leverage.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1271 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/leveragebracket.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      937 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/liquidationorder.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1410 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/liquidationorderevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      337 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/listenkeyexpired.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      775 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/longshortratio.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      620 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/markprice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      661 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/markpriceevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      393 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/binance_f/model/message.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2369 2022-03-04 07:28:24.000000 TradeGate-0.3.8/TradeGates/binance_f/model/mytrade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      349 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/openinterest.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      635 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/openintereststats.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3160 2022-03-04 10:20:23.000000 TradeGate-0.3.8/TradeGates/binance_f/model/order.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1309 2022-06-17 14:41:44.000000 TradeGate-0.3.8/TradeGates/binance_f/model/orderbook.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1584 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/orderbookevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3015 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/orderupdate.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1978 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/binance_f/model/position.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      461 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/positionmargin.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      558 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/positionmarginhistory.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      274 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/positionmode.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      765 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/symbolbooktickerevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      970 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/symbolminitickerevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      583 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/symbolorderbook.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      386 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/symbolprice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1862 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/symboltickerevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      531 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/takerbuysellratio.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1691 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/model/tickerpricechangestatistics.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      896 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/binance_f/model/trade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    23283 2022-03-23 21:08:19.000000 TradeGate-0.3.8/TradeGates/binance_f/requestclient.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    12780 2021-08-19 21:43:22.000000 TradeGate-0.3.8/TradeGates/binance_f/subscriptionclient.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.357816 TradeGate-0.3.8/TradeGates/kucoin/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.358181 TradeGate-0.3.8/TradeGates/kucoin/base_request/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/base_request/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4269 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/base_request/base_request.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      390 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.358477 TradeGate-0.3.8/TradeGates/kucoin/margin/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/margin/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    14243 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/margin/margin.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.358814 TradeGate-0.3.8/TradeGates/kucoin/market/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/market/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    16795 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/market/market.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.359174 TradeGate-0.3.8/TradeGates/kucoin/trade/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/trade/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    24825 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/trade/trade.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.359631 TradeGate-0.3.8/TradeGates/kucoin/user/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/user/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    23869 2022-06-27 12:34:05.000000 TradeGate-0.3.8/TradeGates/kucoin/user/user.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.360189 TradeGate-0.3.8/TradeGates/kucoin/websocket/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/websocket/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/websocket/websocket.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1594 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/ws_client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.360507 TradeGate-0.3.8/TradeGates/kucoin/ws_token/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/ws_token/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      451 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin/ws_token/token.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.360899 TradeGate-0.3.8/TradeGates/kucoin_futures/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.361158 TradeGate-0.3.8/TradeGates/kucoin_futures/base_request/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/base_request/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4299 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/base_request/base_request.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      376 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.361397 TradeGate-0.3.8/TradeGates/kucoin_futures/marke_data/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/marke_data/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    22513 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/marke_data/market_data.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.361753 TradeGate-0.3.8/TradeGates/kucoin_futures/trade/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/trade/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    31092 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/trade/trade.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.362064 TradeGate-0.3.8/TradeGates/kucoin_futures/user/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/user/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     9818 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/user/user.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.362337 TradeGate-0.3.8/TradeGates/kucoin_futures/websocket/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/websocket/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/websocket/websocket.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1620 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/ws_client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.362616 TradeGate-0.3.8/TradeGates/kucoin_futures/ws_token/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/ws_token/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      480 2022-06-16 09:06:16.000000 TradeGate-0.3.8/TradeGates/kucoin_futures/ws_token/token.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      267 2022-06-17 08:03:32.000000 TradeGate-0.3.8/pyproject.toml
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       79 2023-05-24 06:59:52.364486 TradeGate-0.3.8/setup.cfg
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1451 2023-05-24 06:59:32.000000 TradeGate-0.3.8/setup.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-24 06:59:52.363742 TradeGate-0.3.8/test/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3894 2023-05-23 18:00:48.000000 TradeGate-0.3.8/test/testAccountInfo.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    16024 2022-06-27 15:23:02.000000 TradeGate-0.3.8/test/testFutures.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5351 2022-06-16 09:06:16.000000 TradeGate-0.3.8/test/testMarketInfo.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7291 2022-06-27 13:57:30.000000 TradeGate-0.3.8/test/testOrdering.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.169289 TradeGate-0.3.8.1/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1072 2022-02-23 07:14:51.000000 TradeGate-0.3.8.1/LICENSE
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2611 2023-05-28 10:29:51.169386 TradeGate-0.3.8.1/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2238 2023-05-24 11:59:49.000000 TradeGate-0.3.8.1/README.md
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.139361 TradeGate-0.3.8.1/TradeGates/
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.141966 TradeGate-0.3.8.1/TradeGates/Exchanges/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4382 2023-05-24 13:36:47.000000 TradeGate-0.3.8.1/TradeGates/Exchanges/BaseExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    33661 2023-05-28 10:29:31.000000 TradeGate-0.3.8.1/TradeGates/Exchanges/BinanceExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    34808 2023-05-24 20:45:01.000000 TradeGate-0.3.8.1/TradeGates/Exchanges/BybitExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    44496 2023-05-24 20:12:33.000000 TradeGate-0.3.8.1/TradeGates/Exchanges/KuCoinExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       83 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/Exchanges/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.142736 TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2611 2023-05-28 10:29:51.000000 TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5673 2023-05-28 10:29:51.000000 TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/SOURCES.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-05-28 10:29:51.000000 TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/dependency_links.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       89 2023-05-28 10:29:51.000000 TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/requires.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       67 2023-05-28 10:29:51.000000 TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/top_level.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    58706 2023-05-24 12:31:23.000000 TradeGate-0.3.8.1/TradeGates/TradeGate.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.144399 TradeGate-0.3.8.1/TradeGates/Utils/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4281 2023-05-24 18:22:33.000000 TradeGate-0.3.8.1/TradeGates/Utils/BinanceHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    14074 2023-05-24 18:51:07.000000 TradeGate-0.3.8.1/TradeGates/Utils/BybitHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     8402 2023-05-24 18:25:02.000000 TradeGate-0.3.8.1/TradeGates/Utils/DataHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    13473 2023-05-24 18:52:23.000000 TradeGate-0.3.8.1/TradeGates/Utils/KuCoinHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       80 2022-10-02 08:05:21.000000 TradeGate-0.3.8.1/TradeGates/Utils/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.144744 TradeGate-0.3.8.1/TradeGates/Watchers/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/Watchers/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2645 2023-05-24 12:20:18.000000 TradeGate-0.3.8.1/TradeGates/Watchers/futureOrderWatchers.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.145704 TradeGate-0.3.8.1/TradeGates/binance_f/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      112 2022-02-23 05:49:50.000000 TradeGate-0.3.8.1/TradeGates/binance_f/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.146448 TradeGate-0.3.8.1/TradeGates/binance_f/base/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/base/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5597 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/base/printobject.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      597 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/base/printtime.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.146928 TradeGate-0.3.8.1/TradeGates/binance_f/constant/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/constant/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      399 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/constant/system.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      250 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/constant/test.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.147165 TradeGate-0.3.8.1/TradeGates/binance_f/exception/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/exception/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      422 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/exception/binanceapiexception.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.150119 TradeGate-0.3.8.1/TradeGates/binance_f/impl/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)       58 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2680 2022-02-26 09:29:35.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/restapiinvoker.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      310 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/restapirequest.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    36651 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/restapirequestimpl.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.151529 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      240 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1146 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/apisignature.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      156 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/channelparser.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5407 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/channels.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3139 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/inputchecker.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3400 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/jsonwrapper.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      434 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/timeservice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1030 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/urlparamsbuilder.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     7819 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketconnection.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      360 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketrequest.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    15345 2022-03-03 18:09:37.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketrequestimpl.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2243 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketwatchdog.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.162705 TradeGate-0.3.8.1/TradeGates/binance_f/model/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2976 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     4355 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/accountinformation.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5309 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/accountinformationv2.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2355 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/accountupdate.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      343 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/adlquantile.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      690 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/aggregatetrade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      971 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/aggregatetradeevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/apitradingstatus.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      999 2022-03-02 11:34:30.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/balance.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      854 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/balancev2.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      908 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/blvtinfoevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      706 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/blvtnavcandlestick.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1789 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/blvtnavcandlestickevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1607 2022-02-24 11:54:59.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/candlestick.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2230 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/candlestickevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      438 2022-03-04 10:50:30.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/codeandmsg.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1304 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/compositeindexevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2103 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/constant.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2389 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/continuouscandelstickevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      352 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/countdowncancelall.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1634 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/diffdepthevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3756 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/exchangeinformation.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      433 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/fundingrate.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      791 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/income.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/indexInfo.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      568 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/leverage.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1271 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/leveragebracket.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      937 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/liquidationorder.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1410 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/liquidationorderevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      337 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/listenkeyexpired.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      775 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/longshortratio.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      620 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/markprice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      661 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/markpriceevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      393 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/message.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2369 2022-03-04 07:28:24.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/mytrade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      349 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/openinterest.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      635 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/openintereststats.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3160 2022-03-04 10:20:23.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/order.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1309 2022-06-17 14:41:44.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/orderbook.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1584 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/orderbookevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3015 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/orderupdate.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1978 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/position.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      461 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/positionmargin.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      558 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/positionmarginhistory.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      274 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/positionmode.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      765 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolbooktickerevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      970 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolminitickerevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      583 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolorderbook.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      386 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolprice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1862 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/symboltickerevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      531 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/takerbuysellratio.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1691 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/tickerpricechangestatistics.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      896 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/binance_f/model/trade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    23283 2022-03-23 21:08:19.000000 TradeGate-0.3.8.1/TradeGates/binance_f/requestclient.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    12780 2021-08-19 21:43:22.000000 TradeGate-0.3.8.1/TradeGates/binance_f/subscriptionclient.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.163126 TradeGate-0.3.8.1/TradeGates/kucoin/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.163537 TradeGate-0.3.8.1/TradeGates/kucoin/base_request/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/base_request/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4269 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/base_request/base_request.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      390 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.163824 TradeGate-0.3.8.1/TradeGates/kucoin/margin/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/margin/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    14243 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/margin/margin.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.164088 TradeGate-0.3.8.1/TradeGates/kucoin/market/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/market/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    16795 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/market/market.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.164425 TradeGate-0.3.8.1/TradeGates/kucoin/trade/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/trade/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    24825 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/trade/trade.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.164917 TradeGate-0.3.8.1/TradeGates/kucoin/user/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/user/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    23869 2022-06-27 12:34:05.000000 TradeGate-0.3.8.1/TradeGates/kucoin/user/user.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.165568 TradeGate-0.3.8.1/TradeGates/kucoin/websocket/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/websocket/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/websocket/websocket.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1594 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/ws_client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.165821 TradeGate-0.3.8.1/TradeGates/kucoin/ws_token/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/ws_token/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      451 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin/ws_token/token.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.166233 TradeGate-0.3.8.1/TradeGates/kucoin_futures/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.166482 TradeGate-0.3.8.1/TradeGates/kucoin_futures/base_request/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/base_request/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4299 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/base_request/base_request.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      376 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.166749 TradeGate-0.3.8.1/TradeGates/kucoin_futures/marke_data/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/marke_data/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    22513 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/marke_data/market_data.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.167049 TradeGate-0.3.8.1/TradeGates/kucoin_futures/trade/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/trade/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    31092 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/trade/trade.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.167350 TradeGate-0.3.8.1/TradeGates/kucoin_futures/user/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/user/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     9818 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/user/user.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.167594 TradeGate-0.3.8.1/TradeGates/kucoin_futures/websocket/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/websocket/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/websocket/websocket.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1620 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/ws_client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.167838 TradeGate-0.3.8.1/TradeGates/kucoin_futures/ws_token/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/ws_token/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      480 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/TradeGates/kucoin_futures/ws_token/token.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      267 2022-06-17 08:03:32.000000 TradeGate-0.3.8.1/pyproject.toml
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       79 2023-05-28 10:29:51.169620 TradeGate-0.3.8.1/setup.cfg
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1453 2023-05-28 10:29:40.000000 TradeGate-0.3.8.1/setup.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-05-28 10:29:51.168880 TradeGate-0.3.8.1/test/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3859 2023-05-24 20:29:43.000000 TradeGate-0.3.8.1/test/testAccountInfo.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    16024 2022-06-27 15:23:02.000000 TradeGate-0.3.8.1/test/testFutures.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5351 2022-06-16 09:06:16.000000 TradeGate-0.3.8.1/test/testMarketInfo.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     8386 2023-05-24 11:59:49.000000 TradeGate-0.3.8.1/test/testOrdering.py
```

### Comparing `TradeGate-0.3.8/LICENSE` & `TradeGate-0.3.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/PKG-INFO` & `TradeGate-0.3.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TradeGate
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: A Trading Gateway
 Author: Rustin Soraki
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,15 +80,15 @@
 import json
 
 with open('/path/to/config/file.json') as f:
     config = json.load(f)
 
 gate = TradeGate(config['Binance'], sandbox=True)
 
-print(gate.getSymbolTickerPrice('BTCUSDT'))
+print(gate.get_symbol_ticker_price('BTCUSDT'))
 ```
 
 ## Current Supported Exchanges
 
 - Binance
 - ByBit
 - KuCoin
```

### Comparing `TradeGate-0.3.8/README.md` & `TradeGate-0.3.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 import json
 
 with open('/path/to/config/file.json') as f:
     config = json.load(f)
 
 gate = TradeGate(config['Binance'], sandbox=True)
 
-print(gate.getSymbolTickerPrice('BTCUSDT'))
+print(gate.get_symbol_ticker_price('BTCUSDT'))
 ```
 
 ## Current Supported Exchanges
 
 - Binance
 - ByBit
 - KuCoin
```

### Comparing `TradeGate-0.3.8/TradeGates/Exchanges/BaseExchange.py` & `TradeGate-0.3.8.1/TradeGates/Exchanges/BaseExchange.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,197 +1,199 @@
 from abc import ABC, abstractmethod
 
 
 class BaseExchange(ABC):
     @abstractmethod
-    def __init__(self, credentials, sandbox=False, unifiedInOuts=True):
+    def __init__(self, credentials, sandbox=False, unified_in_outs=True):
         pass
 
     @abstractmethod
     def get_balance(self, asset="", futures=False):
         pass
 
     @abstractmethod
-    def symbolAccountTradeHistory(self, symbol, futures=False, fromId=None, limit=None):
+    def symbol_account_trade_history(
+        self, symbol, futures=False, from_id=None, limit=None
+    ):
         pass
 
     @abstractmethod
-    def testSpotOrder(self, orderData):
+    def test_spot_order(self, order_data):
         pass
 
     @abstractmethod
-    def makeSpotOrder(self, orderData):
+    def make_spot_order(self, order_data):
         pass
 
     @abstractmethod
-    def createAndTestSpotOrder(
+    def create_and_test_spot_order(
         self,
         symbol,
         side,
-        orderType,
+        order_type,
         quantity=None,
         price=None,
-        timeInForce=None,
-        stopPrice=None,
-        icebergQty=None,
-        newOrderRespType=None,
-        newClientOrderId=None,
-        extraParams=None,
+        time_in_force=None,
+        stop_price=None,
+        iceberg_qty=None,
+        new_order_resp_type=None,
+        new_client_order_id=None,
+        extra_params=None,
     ):
         pass
 
     @abstractmethod
-    def getSymbolOrders(
+    def get_symbol_orders(
         self,
         symbol,
         futures=False,
-        orderId=None,
-        startTime=None,
-        endTime=None,
+        order_id=None,
+        start_time=None,
+        end_time=None,
         limit=None,
     ):
         pass
 
     @abstractmethod
-    def getOpenOrders(self, symbol, futures=False):
+    def get_open_orders(self, symbol, futures=False):
         pass
 
     @abstractmethod
-    def cancelAllSymbolOpenOrders(self, symbol, futures=False):
+    def cancel_all_symbol_open_orders(self, symbol, futures=False):
         pass
 
     @abstractmethod
-    def cancelOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
+    def cancel_order(self, symbol, order_id=None, local_order_id=None, futures=False):
         pass
 
     @abstractmethod
-    def getOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
+    def get_order(self, symbol, order_id=None, local_order_id=None, futures=False):
         pass
 
     @abstractmethod
-    def getTradingFees(self, futures=False):
+    def get_trading_fees(self, futures=False):
         pass
 
     @abstractmethod
-    def getSymbolTickerPrice(self, symbol, futures=False):
+    def get_symbol_ticker_price(self, symbol, futures=False):
         pass
 
     @abstractmethod
-    def getSymbolKlines(
+    def get_symbol_klines(
         self,
         symbol,
         interval,
-        startTime=None,
-        endTime=None,
+        start_time=None,
+        end_time=None,
         limit=None,
         futures=False,
         blvtnav=False,
-        convertDateTime=False,
-        doClean=False,
-        toCleanDataframe=False,
+        convert_date_time=False,
+        do_clean=False,
+        to_clean_dataframe=False,
     ):
         pass
 
     @abstractmethod
-    def getExchangeTime(self, futures=False):
+    def get_exchange_time(self, futures=False):
         pass
 
     @abstractmethod
-    def getSymbol24hTicker(self, symbol):
+    def get_symbol_24h_ticker(self, symbol):
         pass
 
     @abstractmethod
-    def testFuturesOrder(self, futuresOrderData):
+    def test_futures_order(self, futures_order_data):
         pass
 
     @abstractmethod
-    def makeFuturesOrder(self, futuresOrderData):
+    def make_futures_order(self, futures_order_data):
         pass
 
     @abstractmethod
-    def createAndTestFuturesOrder(
+    def create_and_test_futures_order(
         self,
         symbol,
         side,
-        orderType,
-        positionSide=None,
-        timeInForce=None,
+        order_type,
+        position_side=None,
+        time_in_force=None,
         quantity=None,
-        reduceOnly=None,
+        reduce_only=None,
         price=None,
-        newClientOrderId=None,
-        stopPrice=None,
-        closePosition=None,
-        activationPrice=None,
-        callbackRate=None,
-        workingType=None,
-        priceProtect=None,
-        newOrderRespType=None,
-        recvWindow=None,
-        extraParams=None,
+        new_client_order_id=None,
+        stop_price=None,
+        close_position=None,
+        activation_price=None,
+        callback_rate=None,
+        working_type=None,
+        price_protect=None,
+        new_order_resp_type=None,
+        recv_window=None,
+        extra_params=None,
     ):
         pass
 
     @abstractmethod
-    def makeBatchFuturesOrder(self, futuresOrderDatas):
+    def make_batch_futures_order(self, futures_order_datas):
         pass
 
     @abstractmethod
-    def changeInitialLeverage(self, symbol, leverage):
+    def change_initial_leverage(self, symbol, leverage):
         pass
 
     @abstractmethod
-    def changeMarginType(self, symbol, marginType, params):
+    def change_margin_type(self, symbol, margin_type, params):
         pass
 
     @abstractmethod
-    def changePositionMargin(self, symbol, amount):
+    def change_position_margin(self, symbol, amount):
         pass
 
     @abstractmethod
-    def getPosition(self):
+    def get_position(self):
         pass
 
     @abstractmethod
-    def spotBestBidAsks(self, symbol):
+    def spot_best_bid_asks(self, symbol):
         pass
 
     @abstractmethod
-    def getSymbolOrderBook(self, symbol, limit=None, futures=False):
+    def get_symbol_order_book(self, symbol, limit=None, futures=False):
         pass
 
     @abstractmethod
-    def getSymbolRecentTrades(self, symbol, limit=None, futures=False):
+    def get_symbol_recent_trades(self, symbol, limit=None, futures=False):
         pass
 
     @abstractmethod
-    def getPositionInfo(self, symbol=None):
+    def get_position_info(self, symbol=None):
         pass
 
     @abstractmethod
-    def getSymbolMinTrade(self, symbol, futures=False):
+    def get_symbol_min_trade(self, symbol, futures=False):
         pass
 
     @abstractmethod
-    def makeSlTpLimitFuturesOrder(
+    def make_sl_tp_limit_futures_order(
         self,
         symbol,
-        orderSide,
+        order_side,
         quantity=None,
-        quoteQuantity=None,
-        enterPrice=None,
-        takeProfit=None,
-        stopLoss=None,
+        quote_quantity=None,
+        enter_price=None,
+        take_profit=None,
+        stop_loss=None,
         leverage=None,
-        marginType=None,
+        margin_type=None,
     ):
         pass
 
     @abstractmethod
-    def getLongShortRatios(
-        self, symbol, period, limit=None, startTime=None, endTime=None
+    def get_long_short_ratios(
+        self, symbol, period, limit=None, start_time=None, end_time=None
     ):
         pass
 
     @abstractmethod
-    def getDepositAddress(self, coin, network=None):
+    def get_deposit_address(self, coin, network=None):
         pass
```

### Comparing `TradeGate-0.3.8/TradeGates/Exchanges/BinanceExchange.py` & `TradeGate-0.3.8.1/TradeGates/Exchanges/BinanceExchange.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import contextlib
 import logging
 import time
 from datetime import datetime
 
 import pandas as pd
 from binance.spot import Spot
 
@@ -28,82 +29,82 @@
 
 def is_order_data_valid(order: DataHelpers.OrderData):
     check_spot_order_type(order)
     check_order_side(order)
     check_spot_order_response_type(order)
     check_spot_order_time_in_force(order)
 
-    if order.orderType == "LIMIT":
+    if order.order_type == "LIMIT":
         check_limit_order_data_validity(order)
 
-    elif order.orderType == "MARKET":
+    elif order.order_type == "MARKET":
         check_spot_market_order_data_validity(order)
 
-    elif order.orderType in ["STOP_LOSS", "TAKE_PROFIT"]:
+    elif order.order_type in ["STOP_LOSS", "TAKE_PROFIT"]:
         check_spot_stop_market_data_validity(order)
 
-    elif order.orderType in ["STOP_LOSS_LIMIT", "TAKE_PROFIT_LIMIT"]:
+    elif order.order_type in ["STOP_LOSS_LIMIT", "TAKE_PROFIT_LIMIT"]:
         check_spot_stop_limit_order_data_validity(order)
 
-    elif order.orderType == "LIMIT_MAKER":
+    elif order.order_type == "LIMIT_MAKER":
         check_spot_limit_maker_order_data_validity(order)
 
     return False
 
 
 def check_spot_limit_maker_order_data_validity(order):
     if order.quantity is None or order.price is None:
         raise ValueError("For LIMIT_MAKER order quantity and price must be specified.")
 
 
 def check_spot_stop_limit_order_data_validity(order):
     if (
-        order.timeInForce is None
+        order.time_in_force is None
         or order.quantity is None
         or order.price is None
-        or order.stopPrice is None
+        or order.stop_price is None
     ):
         raise ValueError(
             "For STOP_LOSS_LIMIT or TAKE_PROFIT_LIMIT orders timeInForce, quantity, price and stopPrice must be specified."
         )
 
 
 def check_spot_stop_market_data_validity(order):
-    if order.quantity is None or order.stopPrice is None:
+    if order.quantity is None or order.stop_price is None:
         raise ValueError(
             "For STOP_LOSS or TAKE_PROFIT orders quantity and stopPrice must be specified."
         )
 
 
 def check_spot_market_order_data_validity(order):
-    if order.quantity is None and order.quoteOrderQty is None:
+    if order.quantity is None and order.quote_order_qty is None:
         raise ValueError(
             "For MARKET order either quantity or quoteOrderQty must be specified."
         )
 
 
 def check_limit_order_data_validity(order):
-    if order.timeInForce is None or order.quantity is None or order.price is None:
+    if order.time_in_force is None or order.quantity is None or order.price is None:
         raise ValueError(
             "For LIMIT order timeInForce, quantity and price must be specified"
         )
 
 
 def check_spot_order_time_in_force(order):
-    if order.timeInForce not in [None, "GTC", "IOC", "FOK"]:
+    if order.time_in_force not in [None, "GTC", "IOC", "FOK"]:
         raise ValueError("Order time in force is not valid.")
 
 
 def check_spot_order_response_type(order):
-    if order.newOrderRespType not in [None, "ACK", "RESULT", "FULL"]:
+    if order.new_order_resp_type not in [None, "ACK", "RESULT", "FULL"]:
         raise ValueError("Order response type is not valid.")
 
 
 def check_spot_order_type(order):
-    if order.orderType not in BinanceExchange.spotOrderTypes:
+    if order.order_type not in BinanceExchange.spot_order_types:
         raise ValueError("Order type is not valid.")
 
 
 def is_futures_order_data_valid(order: DataHelpers.FuturesOrderData):
     check_order_side(order)
     check_futures_order_type(order)
     check_futures_order_side(order)
@@ -130,101 +131,101 @@
         check_futures_stop_market_order_data_validity(order)
 
     elif order.orderType == "TRAILING_STOP_MARKET":
         check_futures_trailing_order_data_validity(order)
 
 
 def check_futures_trailing_order_data_validity(order):
-    if order.callbackRate is None:
+    if order.callback_rate is None:
         raise ValueError(
             "For futures TRAILING_STOP_MARKET orders callbackRate must be specified."
         )
 
 
 def check_futures_stop_market_order_data_validity(order):
-    if order.stopPrice is None:
+    if order.stop_price is None:
         raise ValueError(
             "For futures STOP_MARKET and TAKE_PROFIT_MARKET orders stopPrice must be specified"
         )
 
 
 def check_futures_stop_limit_order_data_validity(order):
-    if order.quantity is None or order.price is None or order.stopPrice is None:
+    if order.quantity is None or order.price is None or order.stop_price is None:
         raise ValueError(
             "For futures STOP or TAKE_PROFIT order quantity, price and stopPrice must be specified."
         )
 
 
 def check_futures_market_order_data_validity(order):
     if order.quantity is None:
         raise ValueError("For MARKET order quantity must be specified.")
 
 
 def check_simultaneous_close_position_and_reduce_only(order):
-    if order.closePosition is True and order.reduceOnly is True:
+    if order.close_position is True and order.reduce_only is True:
         raise ValueError("Can't set both closePosition and reduceOnly to True.")
 
 
 def check_futures_order_reduce_only(order):
-    if order.reduceOnly not in [None, True, False]:
+    if order.reduce_only not in [None, True, False]:
         raise ValueError("Futures order reduceOnly is not valid.")
 
 
 def check_simultaneous_close_position_and_quantity(order):
-    if order.closePosition is True and order.quantity is not None:
+    if order.close_position is True and order.quantity is not None:
         raise ValueError("Must not specify quantity if closePosition is True.")
 
 
 def check_futures_order_price_protect(order):
-    if order.priceProtect not in [None, True, False]:
+    if order.price_protect not in [None, True, False]:
         raise ValueError("Futures order priceProtect is not valid.")
 
 
 def check_futures_order_callback_rate(order):
-    if order.callbackRate is not None and not (0.1 <= order.callbackRate <= 5):
+    if order.callback_rate is not None and not (0.1 <= order.callback_rate <= 5):
         raise ValueError("Futures order callbackRate is not valid.")
 
 
 def check_futures_order_close_position(order):
-    if order.closePosition not in [None, True, False]:
+    if order.close_position not in [None, True, False]:
         raise ValueError("Futures order closePosition is not valid.")
 
 
 def check_futures_order_response_type(order):
-    if order.newOrderRespType not in [None, "ACK", "RESULT"]:
+    if order.new_order_resp_type not in [None, "ACK", "RESULT"]:
         raise ValueError("Futures order newOrderRespType is not valid.")
 
 
 def check_futures_order_working_type(order):
-    if order.workingType not in [None, "MARK_PRICE", "CONTRACT_PRICE"]:
+    if order.working_type not in [None, "MARK_PRICE", "CONTRACT_PRICE"]:
         raise ValueError("Futures order workingType is not valid.")
 
 
 def check_futures_order_time_in_force(order):
-    if order.timeInForce not in [None, "GTC", "IOC", "FOK", "GTX"]:
+    if order.time_in_force not in [None, "GTC", "IOC", "FOK", "GTX"]:
         raise ValueError("Futures order timeInForce is not valid.")
 
 
 def check_futures_order_side(order):
-    if order.positionSide not in [None, "BOTH", "LONG", "SHORT"]:
+    if order.position_side not in [None, "BOTH", "LONG", "SHORT"]:
         raise ValueError("Futures order side is not valid")
 
 
 def check_futures_order_type(order):
-    if order.orderType not in BinanceExchange.futuresOrderTypes:
+    if order.order_type not in BinanceExchange.futures_order_types:
         raise ValueError("Futures order type is not valid.")
 
 
 def check_order_side(order):
     if order.side not in ["BUY", "SELL"]:
         raise ValueError("Order side can only be 'BUY' or 'SELL'")
 
 
 class BinanceExchange(BaseExchange):
-    timeIntervals = [
+    time_intervals = [
         "1m",
         "3m",
         "5m",
         "15m",
         "30m",
         "1h",
         "2h",
@@ -234,765 +235,773 @@
         "12h",
         "1d",
         "3d",
         "1w",
         "1M",
     ]
 
-    timeIndexesInCandleData = [0, 6]
-    desiredCandleDataIndexes = [0, 1, 2, 3, 4, 5, 6, 8]
+    time_indexes_in_candle_data = [0, 6]
+    desired_candle_data_indexes = [0, 1, 2, 3, 4, 5, 6, 8]
 
-    spotOrderTypes = [
+    spot_order_types = [
         "LIMIT",
         "MARKET",
         "STOP_LOSS",
         "STOP_LOSS_LIMIT",
         "TAKE_PROFIT",
         "TAKE_PROFIT_LIMIT",
         "LIMIT_MAKER",
     ]
 
-    futuresOrderTypes = [
+    futures_order_types = [
         "LIMIT",
         "MARKET",
         "STOP",
         "STOP_MARKET",
         "TAKE_PROFIT",
         "TAKE_PROFIT_MARKET",
         "TRAILING_STOP_MARKET",
     ]
 
     def __init__(self, credentials, sandbox=False, unified_in_outs=True):
         self.credentials = credentials
         self.sandbox = sandbox
-        self.unifiedInOuts = unified_in_outs
+        self.unified_in_outs = unified_in_outs
 
         if sandbox:
             self.client = Spot(
-                key=credentials["spot"]["key"],
-                secret=credentials["spot"]["secret"],
+                credentials["spot"]["key"],
+                credentials["spot"]["secret"],
                 base_url="https://testnet.binance.vision",
             )
-            self.futuresClient = RequestClient(
+            self.futures_client = RequestClient(
                 api_key=credentials["futures"]["key"],
                 secret_key=credentials["futures"]["secret"],
                 url="https://testnet.binancefuture.com",
             )
         else:
             self.client = Spot(
-                key=credentials["spot"]["key"], secret=credentials["spot"]["secret"]
+                credentials["spot"]["key"], credentials["spot"]["secret"]
             )
-            self.futuresClient = RequestClient(
+            self.futures_client = RequestClient(
                 api_key=credentials["futures"]["key"],
                 secret_key=credentials["futures"]["secret"],
                 url="https://fapi.binance.com",
             )
 
-        self.subFutureClient = None
+        self.sub_future_client = None
 
     def get_balance(self, asset="", futures=False):
         if not futures:
             try:
                 balances = self.client.account()["balances"]
             except Exception as e:
                 print(e)
                 return None
             if asset == "" or asset is None:
                 return balances
-            else:
-                for balance in balances:
-                    if balance["asset"] == asset:
-                        return balance
-            return None
+            return next(
+                (balance for balance in balances if balance["asset"] == asset),
+                None,
+            )
         else:
-            balances = []
-            for balance in self.futuresClient.get_balance():
-                balances.append(balance.toDict())
-
+            balances = [
+                balance.toDict() for balance in self.futures_client.get_balance()
+            ]
             if asset == "" or asset is None:
                 return balances
-            else:
-                for balance in balances:
-                    if balance["asset"] == asset:
-                        return balance
-                return Balance.makeFreeBalance(asset)
+            for balance in balances:
+                if balance["asset"] == asset:
+                    return balance
+            return Balance.makeFreeBalance(asset)
 
-    def symbolAccountTradeHistory(self, symbol, futures=False, fromId=None, limit=None):
+    def symbol_account_trade_history(
+        self, symbol, futures=False, from_id=None, limit=None
+    ):
         try:
             if not futures:
-                return self.client.my_trades(symbol, fromId=fromId, limit=limit)
+                return self.client.my_trades(symbol, fromId=from_id, limit=limit)
             else:
-                trades = []
-                for trade in self.futuresClient.get_account_trades(
-                    symbol=symbol, fromId=fromId, limit=limit
-                ):
-                    trades.append(trade.toDict())
-                return trades
-
-        except Exception:
+                return [
+                    trade.toDict()
+                    for trade in self.futures_client.get_account_trades(
+                        symbol=symbol, fromId=from_id, limit=limit
+                    )
+                ]
+        except Exception as e:
+            print(e)
             return None
 
-    def testSpotOrder(self, orderData):
-        if not is_order_data_valid(orderData):
+    def test_spot_order(self, order_data):
+        # sourcery skip: no-conditionals-in-tests
+        if not is_order_data_valid(order_data):
             raise ValueError("Incomplete data provided.")
 
-        orderData.setTimestamp()
-        params = BinanceHelpers.getSpotOrderAsDict(orderData)
+        order_data.set_timestamp()
+        params = BinanceHelpers.get_spot_order_as_dict(order_data)
 
-        response = self.client.new_order_test(**params)
-        return response
+        return self.client.new_order_test(**params)
 
-    def makeSpotOrder(self, orderData):
-        params = BinanceHelpers.getSpotOrderAsDict(orderData)
+    def make_spot_order(self, order_data):
+        params = BinanceHelpers.get_spot_order_as_dict(order_data)
 
         response = self.client.new_order(**params)
         logging.info(response)
         return response
 
-    def createAndTestSpotOrder(
+    def create_and_test_spot_order(
         self,
         symbol,
         side,
-        orderType,
+        order_type,
         quantity=None,
         price=None,
-        timeInForce=None,
-        stopPrice=None,
-        icebergQty=None,
-        newOrderRespType=None,
-        newClientOrderId=None,
-        extraParams=None,
-    ):
-        currOrder = DataHelpers.setSpotOrderData(
-            icebergQty,
-            newClientOrderId,
-            newOrderRespType,
-            orderType,
+        time_in_force=None,
+        stop_price=None,
+        iceberg_qty=None,
+        new_order_resp_type=None,
+        new_client_order_id=None,
+        extra_params=None,
+    ):
+        curr_order = DataHelpers.set_spot_order_data(
+            iceberg_qty,
+            new_client_order_id,
+            new_order_resp_type,
+            order_type,
             price,
             quantity,
             side,
-            stopPrice,
+            stop_price,
             symbol,
-            timeInForce,
-            extraParams,
+            time_in_force,
+            extra_params,
         )
 
-        self.testSpotOrder(currOrder)
+        self.test_spot_order(curr_order)
 
-        return currOrder
+        return curr_order
 
-    def getSymbolOrders(
+    def get_symbol_orders(
         self,
         symbol,
         futures=False,
-        orderId=None,
-        startTime=None,
-        endTime=None,
+        order_id=None,
+        start_time=None,
+        end_time=None,
         limit=None,
     ):
         if not futures:
             return self.client.get_orders(
-                symbol,
-                orderId=orderId,
-                startTime=startTime,
-                endTime=endTime,
+                symbol=symbol,
+                orderId=order_id,
+                startTime=start_time,
+                endTime=end_time,
                 limit=limit,
                 timestamp=time.time(),
             )
         else:
-            orders = []
-            for order in self.futuresClient.get_all_orders(
-                symbol,
-                orderId=orderId,
-                startTime=startTime,
-                endTime=endTime,
-                limit=limit,
-            ):
-                orders.append(order.toDict())
-            return orders
+            return [
+                order.toDict()
+                for order in self.futures_client.get_all_orders(
+                    symbol,
+                    orderId=order_id,
+                    startTime=start_time,
+                    endTime=end_time,
+                    limit=limit,
+                )
+            ]
 
-    def getOpenOrders(self, symbol, futures=False):
+    def get_open_orders(self, symbol, futures=False):
         try:
             if not futures:
                 return self.client.get_open_orders(symbol, timestamp=time.time())
             else:
-                orders = []
-                for order in self.futuresClient.get_open_orders(symbol=symbol):
-                    orders.append(order.toDict())
-                return orders
-        except Exception:
+                return [
+                    order.toDict()
+                    for order in self.futures_client.get_open_orders(symbol=symbol)
+                ]
+        except Exception as e:
+            print(e)
             return None
 
-    def cancelAllSymbolOpenOrders(self, symbol, futures=False):
+    def cancel_all_symbol_open_orders(self, symbol, futures=False):
         if not futures:
-            openOrders = self.getOpenOrders(symbol)
-            if len(openOrders) == 0:
+            open_orders = self.get_open_orders(symbol)
+            if len(open_orders) == 0:
                 return []
             else:
                 return self.client.cancel_open_orders(symbol, timestamp=time.time())
         else:
-            openOrders = self.getOpenOrders(symbol, futures=True)
+            open_orders = self.get_open_orders(symbol, futures=True)
 
-            if len(openOrders) == 0:
+            if len(open_orders) == 0:
                 return []
-            else:
-                orderIds = [order["orderId"] for order in openOrders]
+            order_ids = [order["orderId"] for order in open_orders]
 
-                results = []
-                for res in self.futuresClient.cancel_list_orders(
-                    symbol=symbol, orderIdList=orderIds
-                ):
-                    results.append(res.toDict())
-
-                return results
+            return [
+                res.toDict()
+                for res in self.futures_client.cancel_list_orders(
+                    symbol=symbol, orderIdList=order_ids
+                )
+            ]
 
-    def cancelOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
-        errorMessage = (
+    def cancel_order(self, symbol, order_id=None, local_order_id=None, futures=False):
+        error_message = (
             "Specify either order Id in the exchange or local Id sent with the order"
         )
-        if not futures:
-            if orderId is not None:
-                return self.client.cancel_order(
-                    symbol, orderId=orderId, timestamp=time.time()
-                )
-            elif localOrderId is not None:
-                return self.client.cancel_order(
-                    symbol, origClientOrderId=localOrderId, timestamp=time.time()
-                )
-            else:
-                raise ValueError(errorMessage)
-        else:
-            if orderId is not None:
-                return self.futuresClient.cancel_order(symbol, orderId=orderId).toDict()
-            elif localOrderId is not None:
-                return self.futuresClient.cancel_order(
-                    symbol, origClientOrderId=localOrderId
+        if futures:
+            if order_id is not None:
+                return self.futures_client.cancel_order(
+                    symbol, orderId=order_id
+                ).toDict()
+            elif local_order_id is not None:
+                return self.futures_client.cancel_order(
+                    symbol, origClientOrderId=local_order_id
                 ).toDict()
             else:
-                raise ValueError(errorMessage)
+                raise ValueError(error_message)
 
-    def getOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
-        errorMessage = (
+        elif order_id is not None:
+            return self.client.cancel_order(
+                symbol, orderId=order_id, timestamp=time.time()
+            )
+        elif local_order_id is not None:
+            return self.client.cancel_order(
+                symbol, origClientOrderId=local_order_id, timestamp=time.time()
+            )
+        else:
+            raise ValueError(error_message)
+
+    def get_order(self, symbol, order_id=None, local_order_id=None, futures=False):
+        error_message = (
             "Specify either order Id in the exchange or local Id sent with the order"
         )
-        if not futures:
-            if orderId is not None:
-                return self.client.get_order(
-                    symbol, orderId=orderId, timestamp=time.time()
-                )
-            elif localOrderId is not None:
-                return self.client.get_order(
-                    symbol, origClientOrderId=localOrderId, timestamp=time.time()
-                )
-            else:
-                raise ValueError(errorMessage)
-        else:
-            if orderId is not None:
-                return self.futuresClient.get_order(symbol, orderId=orderId).toDict()
-            elif localOrderId is not None:
-                return self.futuresClient.get_order(
-                    symbol, origClientOrderId=localOrderId
+        if futures:
+            if order_id is not None:
+                return self.futures_client.get_order(symbol, orderId=order_id).toDict()
+            elif local_order_id is not None:
+                return self.futures_client.get_order(
+                    symbol, origClientOrderId=local_order_id
                 ).toDict()
             else:
-                raise ValueError(errorMessage)
+                raise ValueError(error_message)
+
+        elif order_id is not None:
+            return self.client.get_order(
+                symbol, orderId=order_id, timestamp=time.time()
+            )
+        elif local_order_id is not None:
+            return self.client.get_order(
+                symbol, origClientOrderId=local_order_id, timestamp=time.time()
+            )
+        else:
+            raise ValueError(error_message)
 
-    def getTradingFees(self, symbol=None, futures=False):
+    def get_trading_fees(self, symbol=None, futures=False):
         if symbol:
             return self.client.trade_fee(symbol=symbol)[0]
         else:
             return self.client.trade_fee(symbol=symbol)
 
-    def getSymbolTickerPrice(self, symbol, futures=False):
+    def get_symbol_ticker_price(self, symbol, futures=False):
         if futures:
-            return self.futuresClient.get_symbol_price_ticker(symbol=symbol)[0].price
+            return self.futures_client.get_symbol_price_ticker(symbol=symbol)[0].price
         else:
             return float(self.client.ticker_price(symbol)["price"])
 
-    def getSymbolKlines(
+    def get_symbol_klines(
         self,
         symbol,
         interval,
-        startTime=None,
-        endTime=None,
+        start_time=None,
+        end_time=None,
         limit=None,
         futures=False,
         blvtnav=False,
-        convertDateTime=False,
-        doClean=False,
-        toCleanDataframe=False,
+        convert_date_time=False,
+        do_clean=False,
+        to_clean_dataframe=False,
     ):
-        if interval not in BinanceExchange.timeIntervals:
+        if interval not in BinanceExchange.time_intervals:
             raise ValueError("Time interval is not valid.")
 
         if futures:
-            data = self._getFuturesSymbolKlines(
-                blvtnav, endTime, interval, limit, startTime, symbol
+            data = self._get_futures_symbol_klines(
+                blvtnav, end_time, interval, limit, start_time, symbol
             )
         else:
-            data = self._getSpotSymbolKlines(
-                endTime, interval, limit, startTime, symbol
+            data = self._get_spot_symbol_klines(
+                end_time, interval, limit, start_time, symbol
             )
 
-        if convertDateTime or toCleanDataframe:
-            BinanceHelpers.klinesConvertDate(data, self.timeIndexesInCandleData)
+        if convert_date_time or to_clean_dataframe:
+            BinanceHelpers.klines_convert_date(data, self.time_indexes_in_candle_data)
 
-        if doClean or toCleanDataframe:
-            finalDataArray = BinanceHelpers.getKlinesDesiredOnlyCols(
-                data, self.desiredCandleDataIndexes
-            )
-
-            if toCleanDataframe:
-                return BinanceHelpers.klinesConvertToPandas(finalDataArray)
-            return finalDataArray
-        else:
+        if not do_clean and not to_clean_dataframe:
             return data
 
-    def _getSpotSymbolKlines(self, endTime, interval, limit, startTime, symbol):
+        final_data_array = BinanceHelpers.get_klines_desired_only_cols(
+            data, self.desired_candle_data_indexes
+        )
+
+        if to_clean_dataframe:
+            return BinanceHelpers.klines_convert_to_pandas(final_data_array)
+        return final_data_array
+
+    def _get_spot_symbol_klines(self, end_time, interval, limit, start_time, symbol):
         data = self.client.klines(
-            symbol, interval, startTime=startTime, endTime=endTime, limit=limit
+            symbol, interval, startTime=start_time, endTime=end_time, limit=limit
         )
         for datum in data:
             for idx in range(len(datum)):
-                if idx in BinanceExchange.timeIndexesInCandleData:
+                if idx in BinanceExchange.time_indexes_in_candle_data:
                     continue
                 datum[idx] = float(datum[idx])
         return data
 
-    def _getFuturesSymbolKlines(
-        self, blvtnav, endTime, interval, limit, startTime, symbol
+    def _get_futures_symbol_klines(
+        self, blvtnav, end_time, interval, limit, start_time, symbol
     ):
-        data = []
         if blvtnav:
-            candles = self.futuresClient.get_blvt_nav_candlestick_data(
+            candles = self.futures_client.get_blvt_nav_candlestick_data(
                 symbol=symbol,
                 interval=interval,
-                startTime=startTime,
-                endTime=endTime,
+                startTime=start_time,
+                endTime=end_time,
                 limit=limit,
             )
         else:
-            candles = self.futuresClient.get_candlestick_data(
+            candles = self.futures_client.get_candlestick_data(
                 symbol=symbol,
                 interval=interval,
-                startTime=startTime,
-                endTime=endTime,
+                startTime=start_time,
+                endTime=end_time,
                 limit=limit,
             )
-        for candle in candles:
-            data.append(candle.toArray())
-        return data
+        return [candle.toArray() for candle in candles]
 
-    def getExchangeTime(self, futures=False):
+    def get_exchange_time(self, futures=False):
         try:
             if not futures:
                 return self.client.time()["serverTime"]
             else:
-                return self.futuresClient.get_servertime()
-        except Exception:
+                return self.futures_client.get_servertime()
+        except Exception as e:
+            print(e)
             return None
 
-    def getSymbol24hTicker(self, symbol):
+    def get_symbol_24h_ticker(self, symbol):
         try:
             return self.client.ticker_24hr(symbol)
-        except Exception:
+        except Exception as e:
+            print(e)
             return None
 
-    def testFuturesOrder(self, futuresOrderData):
-        if not is_futures_order_data_valid(futuresOrderData):
+    def test_futures_order(self, futures_order_data):
+        # sourcery skip: no-conditionals-in-tests
+        if not is_futures_order_data_valid(futures_order_data):
             raise ValueError("Incomplete data provided.")
-        return futuresOrderData
+        return futures_order_data
 
-    def makeFuturesOrder(self, futuresOrderData):
-        params = BinanceHelpers.getFuturesOrderAsDict(futuresOrderData)
+    def make_futures_order(self, futures_order_data):
+        params = BinanceHelpers.get_futures_order_as_dict(futures_order_data)
 
-        response = self.futuresClient.post_order(**params)
+        response = self.futures_client.post_order(**params)
         return response.toDict()
 
-    def createAndTestFuturesOrder(
+    def create_and_test_futures_order(
         self,
         symbol,
         side,
-        orderType,
-        positionSide=None,
-        timeInForce=None,
+        order_type,
+        position_side=None,
+        time_in_force=None,
         quantity=None,
-        reduceOnly=None,
+        reduce_only=None,
         price=None,
-        newClientOrderId=None,
-        stopPrice=None,
-        closePosition=None,
-        activationPrice=None,
-        callbackRate=None,
-        workingType=None,
-        priceProtect=None,
-        newOrderRespType=None,
-        recvWindow=None,
-        extraParams=None,
-        quoteQuantity=None,
-    ):
-        currOrder = DataHelpers.setFuturesOrderData(
-            activationPrice,
-            callbackRate,
-            closePosition,
-            extraParams,
-            newClientOrderId,
-            newOrderRespType,
-            orderType,
-            positionSide,
+        new_client_order_id=None,
+        stop_price=None,
+        close_position=None,
+        activation_price=None,
+        callback_rate=None,
+        working_type=None,
+        price_protect=None,
+        new_order_resp_type=None,
+        recv_window=None,
+        extra_params=None,
+        quote_quantity=None,
+    ):
+        curr_order = DataHelpers.set_futures_order_data(
+            activation_price,
+            callback_rate,
+            close_position,
+            extra_params,
+            new_client_order_id,
+            new_order_resp_type,
+            order_type,
+            position_side,
             price,
-            priceProtect,
+            price_protect,
             quantity,
-            reduceOnly,
+            reduce_only,
             side,
-            stopPrice,
+            stop_price,
             symbol,
-            timeInForce,
-            workingType,
-            quoteQuantity,
+            time_in_force,
+            working_type,
+            quote_quantity,
         )
 
-        self.testFuturesOrder(currOrder)
+        self.test_futures_order(curr_order)
 
-        return currOrder
+        return curr_order
 
-    def makeBatchFuturesOrder(self, futuresOrderDatas):
-        batchOrders = BinanceHelpers.makeBatchOrderData(futuresOrderDatas)
+    def make_batch_futures_order(self, futures_order_datas):
+        batch_orders = BinanceHelpers.make_batch_order_data(futures_order_datas)
 
-        orderResults = self.futuresClient.post_batch_order(batchOrders)
+        order_results = self.futures_client.post_batch_order(batch_orders)
 
-        return [order.toDict() for order in orderResults]
+        return [order.toDict() for order in order_results]
 
-    def cancelAllSymbolFuturesOrdersWithCountDown(self, symbol, countdownTime):
-        return self.futuresClient.auto_cancel_all_orders(symbol, countdownTime)
+    def cancel_all_symbol_futures_orders_with_countdown(self, symbol, countdown_time):
+        return self.futures_client.auto_cancel_all_orders(symbol, countdown_time)
 
-    def changeInitialLeverage(self, symbol, leverage):
-        return self.futuresClient.change_initial_leverage(
+    def change_initial_leverage(self, symbol, leverage):
+        return self.futures_client.change_initial_leverage(
             symbol=symbol, leverage=leverage
         ).toDict()["leverage"]
 
-    def changeMarginType(self, symbol, marginType, params=None):
-        if marginType not in ["ISOLATED", "CROSSED"]:
+    def change_margin_type(self, symbol, margin_type, params=None):
+        if margin_type not in ["ISOLATED", "CROSSED"]:
             raise ValueError("Margin type specified is not acceptable")
-        try:
-            result = self.futuresClient.change_margin_type(
-                symbol=symbol, marginType=marginType
+        with contextlib.suppress(BinanceApiException):
+            result = self.futures_client.change_margin_type(
+                symbol=symbol, marginType=margin_type
             )
-            if result["code"] == 200:
-                return True
-            else:
-                return False
-        except BinanceApiException:
-            pass
+            return result["code"] == 200
 
-    def changePositionMargin(self, symbol, amount):
-        if amount >= 0:
-            addOrSub = 1
-        else:
-            addOrSub = 2
-        result = self.futuresClient.change_position_margin(
-            symbol=symbol, amount=amount, type=addOrSub
+    def change_position_margin(self, symbol, amount):
+        add_or_sub = 1 if amount >= 0 else 2
+        result = self.futures_client.change_position_margin(
+            symbol=symbol, amount=amount, type=add_or_sub
         )
-        if result["code"] == 200:
-            return True
-        else:
-            return False
+        return result["code"] == 200
 
-    def getPosition(self):
-        return self.futuresClient.get_position()
+    def get_position(self):
+        return self.futures_client.get_position()
 
-    def spotBestBidAsks(self, symbol):
+    def spot_best_bid_asks(self, symbol):
         return self.client.book_ticker(symbol=symbol)
 
-    def getSymbolOrderBook(self, symbol, limit=None, futures=False):
+    def get_symbol_order_book(self, symbol, limit=None, futures=False):
         if not futures:
-            if limit is None:
-                return self.client.depth(symbol)
-            else:
-                return self.client.depth(symbol, limit=limit)
+            return (
+                self.client.depth(symbol)
+                if limit is None
+                else self.client.depth(symbol, limit=limit)
+            )
+        if limit is None:
+            return self.futures_client.get_order_book(symbol=symbol).toDict()
         else:
-            if limit is None:
-                return self.futuresClient.get_order_book(symbol=symbol).toDict()
-            else:
-                return self.futuresClient.get_order_book(
-                    symbol=symbol, limit=limit
-                ).toDict()
+            return self.futures_client.get_order_book(
+                symbol=symbol, limit=limit
+            ).toDict()
 
-    def getSymbolRecentTrades(self, symbol, limit=None, futures=False):
+    def get_symbol_recent_trades(self, symbol, limit=None, futures=False):
         if limit is not None:
             if limit > 1000:
                 limit = 1000
             elif limit < 1:
                 limit = 1
         if not futures:
-            if limit is None:
-                return pd.DataFrame(self.client.trades(symbol))
-            else:
-                return pd.DataFrame(self.client.trades(symbol, limit=limit))
+            return (
+                pd.DataFrame(self.client.trades(symbol=symbol))
+                if limit is None
+                else pd.DataFrame(self.client.trades(symbol, limit=limit))
+            )
+        if limit is None:
+            return pd.DataFrame(
+                self.futures_client.get_recent_trades_list(symbol=symbol)
+            )
         else:
-            if limit is None:
-                return pd.DataFrame(
-                    self.futuresClient.get_recent_trades_list(symbol=symbol)
-                )
-            else:
-                return pd.DataFrame(
-                    self.futuresClient.get_recent_trades_list(
-                        symbol=symbol, limit=limit
-                    )
-                )
+            return pd.DataFrame(
+                self.futures_client.get_recent_trades_list(symbol=symbol, limit=limit)
+            )
 
-    def getPositionInfo(self, symbol=None):
-        return self.futuresClient.get_position_v2(symbol)
+    def get_position_info(self, symbol=None):
+        return self.futures_client.get_position_v2(symbol)
 
-    def getSymbolMinTrade(self, symbol, futures=False):
-        tickerPrice = self.getSymbolTickerPrice(symbol, futures=futures)
+    def get_symbol_min_trade(self, symbol, futures=False):
+        ticker_price = self.get_symbol_ticker_price(symbol, futures=futures)
 
         if futures:
-            exchangeInfo = self.futuresClient.get_exchange_information()
+            exchange_info = self.futures_client.get_exchange_information()
 
-            for sym in exchangeInfo.symbols:
+            for sym in exchange_info.symbols:
                 if sym.symbol == symbol:
-                    symbolFilters = sym.filters
-                    return BinanceHelpers.extractSymbolInfoFromFilters(
-                        symbolFilters, tickerPrice
+                    symbol_filters = sym.filters
+                    return BinanceHelpers.extract_symbol_info_from_filters(
+                        symbol_filters, ticker_price
                     )
-            return None
         else:
-            exchangeInfo = self.client.exchange_info()
+            exchange_info = self.client.exchange_info()
 
-            for sym in exchangeInfo["symbols"]:
+            for sym in exchange_info["symbols"]:
                 if sym["symbol"] == symbol:
-                    symbolFilters = sym["filters"]
-                    return BinanceHelpers.extractSymbolInfoFromFilters(
-                        symbolFilters, tickerPrice
+                    symbol_filters = sym["filters"]
+                    return BinanceHelpers.extract_symbol_info_from_filters(
+                        symbol_filters, ticker_price
                     )
-            return None
+        return None
 
-    def getIncomeHistory(
-        self, symbol, incomeType=None, startTime=None, endTime=None, limit=None
+    def get_income_history(
+        self, symbol, income_type=None, start_time=None, end_time=None, limit=None
     ):
-        return self.futuresClient.get_income_history(
+        return self.futures_client.get_income_history(
             symbol=symbol,
-            incomeType=incomeType,
-            startTime=startTime,
-            endTime=endTime,
+            incomeType=income_type,
+            startTime=start_time,
+            endTime=end_time,
             limit=limit,
         )
 
-    def makeSlTpLimitFuturesOrder(
+    def make_sl_tp_limit_futures_order(
         self,
         symbol,
-        orderSide,
+        order_side,
         quantity=None,
-        quoteQuantity=None,
-        enterPrice=None,
-        takeProfit=None,
-        stopLoss=None,
+        quote_quantity=None,
+        enter_price=None,
+        take_profit=None,
+        stop_loss=None,
         leverage=None,
-        marginType=None,
+        margin_type=None,
     ):
-        symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
+        symbol_info = self.get_symbol_min_trade(symbol=symbol, futures=True)
 
-        quantity = DataHelpers.getQuantity(
-            enterPrice, quantity, quoteQuantity, symbolInfo["precisionStep"]
+        quantity = DataHelpers.get_quantity(
+            enter_price, quantity, quote_quantity, symbol_info["precisionStep"]
+        )
+        self._set_leverage(leverage, symbol)
+        self.change_margin_type(symbol, margin_type)
+        tp_sl_order_side = "BUY" if order_side.upper() == "SELL" else "SELL"
+
+        main_order, stop_loss_order, take_profit_order = self.create_sl_tp_limit_orders(
+            enter_price,
+            order_side,
+            quantity,
+            stop_loss,
+            symbol,
+            take_profit,
+            tp_sl_order_side,
         )
-        self._setLeverage(leverage, symbol)
-        self.changeMarginType(symbol, marginType)
-        tpSlOrderSide = "BUY" if orderSide.upper() == "SELL" else "SELL"
 
-        mainOrder = self.createAndTestFuturesOrder(
+        ordering_result = self.make_batch_futures_order(
+            [main_order, stop_loss_order, take_profit_order]
+        )
+
+        return DataHelpers.get_tp_sl_limit_order_ids(ordering_result)
+
+    def create_sl_tp_limit_orders(
+        self,
+        enter_price,
+        order_side,
+        quantity,
+        stop_loss,
+        symbol,
+        take_profit,
+        tp_sl_order_side,
+    ):
+        main_order = self.create_and_test_futures_order(
             symbol,
-            orderSide.upper(),
+            order_side.upper(),
             "LIMIT",
             quantity=str(quantity),
-            price=str(enterPrice),
-            timeInForce="GTC",
+            price=str(enter_price),
+            time_in_force="GTC",
         )
-
-        stopLossOrder = self.createAndTestFuturesOrder(
+        stop_loss_order = self.create_and_test_futures_order(
             symbol,
-            tpSlOrderSide,
+            tp_sl_order_side,
             "STOP_MARKET",
-            stopPrice=str(stopLoss),
-            closePosition=True,
-            priceProtect=True,
-            workingType="MARK_PRICE",
-            timeInForce="GTC",
+            stop_price=str(stop_loss),
+            close_position=True,
+            price_protect=True,
+            working_type="MARK_PRICE",
+            time_in_force="GTC",
         )
-
-        takeProfitOrder = self.createAndTestFuturesOrder(
+        take_profit_order = self.create_and_test_futures_order(
             symbol,
-            tpSlOrderSide,
+            tp_sl_order_side,
             "TAKE_PROFIT_MARKET",
-            stopPrice=str(takeProfit),
-            closePosition=True,
-            priceProtect=True,
-            workingType="MARK_PRICE",
-            timeInForce="GTC",
+            stop_price=str(take_profit),
+            close_position=True,
+            price_protect=True,
+            working_type="MARK_PRICE",
+            time_in_force="GTC",
         )
+        return main_order, stop_loss_order, take_profit_order
 
-        orderingResult = self.makeBatchFuturesOrder(
-            [mainOrder, stopLossOrder, takeProfitOrder]
-        )
-
-        orderIds = DataHelpers.getTpSlLimitOrderIds(orderingResult)
-
-        return orderIds
-
-    def makeSlTpMarketFuturesOrder(
+    def make_sl_tp_market_futures_order(
         self,
         symbol,
-        orderSide,
+        order_side,
         quantity=None,
-        quoteQuantity=None,
-        takeProfit=None,
-        stopLoss=None,
+        quote_quantity=None,
+        take_profit=None,
+        stop_loss=None,
         leverage=None,
-        marginType=None,
+        margin_type=None,
     ):
-        symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
-        marketPrice = self.getSymbolTickerPrice(symbol=symbol, futures=True)
+        symbol_info = self.get_symbol_min_trade(symbol=symbol, futures=True)
+        market_price = self.get_symbol_ticker_price(symbol=symbol, futures=True)
 
-        quantity = DataHelpers.getQuantity(
-            marketPrice, quantity, quoteQuantity, symbolInfo["precisionStep"]
+        quantity = DataHelpers.get_quantity(
+            market_price, quantity, quote_quantity, symbol_info["precisionStep"]
         )
-        self._setLeverage(leverage, symbol)
-        self.changeMarginType(symbol, marginType)
-        tpSlOrderSide = "BUY" if orderSide.upper() == "SELL" else "SELL"
+        self._set_leverage(leverage, symbol)
+        self.change_margin_type(symbol, margin_type)
+        tp_sl_order_side = "BUY" if order_side.upper() == "SELL" else "SELL"
 
-        ordersList = []
-        mainOrder = self.createAndTestFuturesOrder(
-            symbol, orderSide.upper(), "MARKET", quantity=str(quantity)
+        has_sl, has_tp, orders_list = self.create_sl_tp_market_orders(
+            order_side, quantity, stop_loss, symbol, take_profit, tp_sl_order_side
         )
 
-        ordersList.append(mainOrder)
+        ordering_result = self.make_batch_futures_order(orders_list)
+
+        return DataHelpers.get_tp_sl_market_order_ids(
+            ordering_result, has_sl=has_sl, has_tp=has_tp
+        )
+
+    def create_sl_tp_market_orders(
+        self, order_side, quantity, stop_loss, symbol, take_profit, tp_sl_order_side
+    ):
+        main_order = self.create_and_test_futures_order(
+            symbol, order_side.upper(), "MARKET", quantity=str(quantity)
+        )
+        orders_list = [main_order]
         has_tp = False
         has_sl = False
-        if stopLoss is not None:
-            stopLossOrder = self.createAndTestFuturesOrder(
+        if stop_loss is not None:
+            stop_loss_order = self.create_and_test_futures_order(
                 symbol,
-                tpSlOrderSide,
+                tp_sl_order_side,
                 "STOP_MARKET",
-                stopPrice=str(stopLoss),
-                closePosition=True,
-                priceProtect=True,
-                workingType="MARK_PRICE",
-                timeInForce="GTC",
+                stop_price=str(stop_loss),
+                close_position=True,
+                price_protect=True,
+                working_type="MARK_PRICE",
+                time_in_force="GTC",
             )
-            ordersList.append(stopLossOrder)
+            orders_list.append(stop_loss_order)
             has_sl = True
-
-        if takeProfit is not None:
-            takeProfitOrder = self.createAndTestFuturesOrder(
+        if take_profit is not None:
+            take_profit_order = self.create_and_test_futures_order(
                 symbol,
-                tpSlOrderSide,
+                tp_sl_order_side,
                 "TAKE_PROFIT_MARKET",
-                stopPrice=str(takeProfit),
-                closePosition=True,
-                priceProtect=True,
-                workingType="MARK_PRICE",
-                timeInForce="GTC",
+                stop_price=str(take_profit),
+                close_position=True,
+                price_protect=True,
+                working_type="MARK_PRICE",
+                time_in_force="GTC",
             )
-            ordersList.append(takeProfitOrder)
+            orders_list.append(take_profit_order)
             has_tp = True
+        return has_sl, has_tp, orders_list
 
-        orderingResult = self.makeBatchFuturesOrder(ordersList)
-
-        orderIds = DataHelpers.getTpSlMarketOrderIds(
-            orderingResult, has_sl=has_sl, has_tp=has_tp
-        )
-        return orderIds
-
-    def _setLeverage(self, leverage, symbol):
-        setLeverageResult = self.changeInitialLeverage(symbol, leverage)
+    def _set_leverage(self, leverage, symbol):
+        set_leverage_result = self.change_initial_leverage(symbol, leverage)
         print("Leverage changed.")
-        if isinstance(setLeverageResult, dict):
-            if setLeverageResult["leverage"] != leverage:
-                raise ConnectionError("Could not change leverage.")
-        elif isinstance(setLeverageResult, float):
-            if setLeverageResult != leverage:
-                raise ConnectionError("Could not change leverage.")
-        else:
+        if (
+            isinstance(set_leverage_result, dict)
+            and set_leverage_result["leverage"] != leverage
+            or not isinstance(set_leverage_result, dict)
+            and isinstance(set_leverage_result, float)
+            and set_leverage_result != leverage
+            or not isinstance(set_leverage_result, dict)
+            and not isinstance(set_leverage_result, float)
+        ):
             raise ConnectionError("Could not change leverage.")
 
-    def getSymbolList(self, futures=False):
+    def get_symbol_list(self, futures=False):
         if futures:
-            symbolNames = []
-            for symbolInfo in self.futuresClient.get_exchange_information().symbols:
-                if symbolInfo.status == "TRADING":
-                    symbolNames.append(symbolInfo.symbol)
-            return symbolNames
+            return [
+                symbolInfo.symbol
+                for symbolInfo in self.futures_client.get_exchange_information().symbols
+                if symbolInfo.status == "TRADING"
+            ]
 
-    def getSymbol24hChanges(self, futures=False):
-        symbolDatas = []
+    def get_symbol_24h_changes(self, futures=False):
+        symbol_datas = []
         if futures:
-            symbolStatus = self.futuresClient.get_exchange_information().symbols
-            for symbolInfo in self.futuresClient.get_ticker_price_change_statistics():
+            symbol_status = self.futures_client.get_exchange_information().symbols
+            symbol_datas.extend(
+                (symbolInfo.symbol, symbolInfo.priceChangePercent)
+                for symbolInfo in self.futures_client.get_ticker_price_change_statistics()
                 if is_symbol_status_valid(
-                    symbolInfo.symbol, symbolStatus, futures=True
-                ):
-                    symbolDatas.append(
-                        (symbolInfo.symbol, symbolInfo.priceChangePercent)
-                    )
+                    symbolInfo.symbol, symbol_status, futures=True
+                )
+            )
         else:
-            symbolStatus = self.client.exchange_info()["symbols"]
-            for symbolInfo in self.client.ticker_24hr():
+            symbol_status = self.client.exchange_info()["symbols"]
+            symbol_datas.extend(
+                (symbolInfo["symbol"], float(symbolInfo["priceChangePercent"]))
+                for symbolInfo in self.client.ticker_24hr()
                 if is_symbol_status_valid(
-                    symbolInfo["symbol"], symbolStatus, futures=False
-                ):
-                    symbolDatas.append(
-                        (symbolInfo["symbol"], float(symbolInfo["priceChangePercent"]))
-                    )
-        return sorted(symbolDatas, key=lambda x: x[1], reverse=True)
-
-    def getLatestSymbolNames(self, numOfSymbols=None, futures=False):
-        symbolDatas = []
-        if futures:
-            for symbolInfo in self.futuresClient.get_exchange_information().symbols:
-                symbolDatas.append(
-                    (
-                        symbolInfo.symbol,
-                        datetime.fromtimestamp(float(symbolInfo.onboardDate) / 1000),
-                    )
+                    symbolInfo["symbol"], symbol_status, futures=False
                 )
-                symbolDatas.sort(key=lambda x: x[1], reverse=True)
-            if numOfSymbols is not None and numOfSymbols > len(symbolDatas):
-                numOfSymbols = len(symbolDatas)
-        else:
+            )
+        return sorted(symbol_datas, key=lambda x: x[1], reverse=True)
+
+    def get_latest_symbol_names(self, num_of_symbols=None, futures=False):
+        symbol_datas = []
+        if not futures:
             raise NotImplementedError("Only available for futures market.")
 
-        return symbolDatas[:numOfSymbols]
+        for symbolInfo in self.futures_client.get_exchange_information().symbols:
+            symbol_datas.append(
+                (
+                    symbolInfo.symbol,
+                    datetime.fromtimestamp(float(symbolInfo.onboardDate) / 1000),
+                )
+            )
+            symbol_datas.sort(key=lambda x: x[1], reverse=True)
+        if num_of_symbols is not None and num_of_symbols > len(symbol_datas):
+            num_of_symbols = len(symbol_datas)
+        return symbol_datas[:num_of_symbols]
 
-    def getLongShortRatios(
-        self, symbol, period, limit=None, startTime=None, endTime=None
+    def get_long_short_ratios(
+        self, symbol, period, limit=None, start_time=None, end_time=None
     ):
         if limit is None:
             limit = 30
-        topLongShortAccounts = self.futuresClient.get_top_long_short_accounts(
+        top_long_short_accounts = self.futures_client.get_top_long_short_accounts(
             symbol=symbol,
             period=period,
-            startTime=startTime,
-            endTime=endTime,
+            startTime=start_time,
+            endTime=end_time,
             limit=limit,
         )
-        topLongShortPositions = self.futuresClient.get_top_long_short_positions(
+        top_long_short_positions = self.futures_client.get_top_long_short_positions(
             symbol=symbol,
             period=period,
-            startTime=startTime,
-            endTime=endTime,
+            startTime=start_time,
+            endTime=end_time,
             limit=limit,
         )
-        longShortRatio = self.futuresClient.get_global_long_short_accounts(
+        long_short_ratio = self.futures_client.get_global_long_short_accounts(
             symbol=symbol,
             period=period,
-            startTime=startTime,
-            endTime=endTime,
+            startTime=start_time,
+            endTime=end_time,
             limit=limit,
         )
 
         return {
-            "topLongShortAccounts": topLongShortAccounts,
-            "topLongShortPositions": topLongShortPositions,
-            "longShortRatio": longShortRatio,
+            "topLongShortAccounts": top_long_short_accounts,
+            "topLongShortPositions": top_long_short_positions,
+            "longShortRatio": long_short_ratio,
         }
 
-    def getDepositAddress(self, coin, network=None):
+    def get_deposit_address(self, coin, network=None):
         return self.client.deposit_address(coin=coin, network=network)
```

### Comparing `TradeGate-0.3.8/TradeGates/Exchanges/BybitExchange.py` & `TradeGate-0.3.8.1/TradeGates/Exchanges/BybitExchange.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,139 +4,183 @@
 
 from pybit.unified_trading import HTTP
 
 from Exchanges.BaseExchange import BaseExchange
 from Utils import DataHelpers, BybitHelpers
 
 
-def isOrderDataValid(orderData: DataHelpers.OrderData):
-    if (
-        orderData.symbol is None
-        or orderData.quantity is None
-        or orderData.side is None
-        or orderData.orderType is None
-    ):
-        raise ValueError("Missing mandatory fields.")
+def is_spot_order_data_valid(order_data: DataHelpers.OrderData):
+    check_spot_order_mandatory_fields(order_data)
+
+    check_spot_order_type(order_data)
+
+    check_spot_order_side(order_data)
+
+    check_spot_order_time_in_force(order_data)
+
+    check_spot_order_limit_price(order_data)
+
+
+def check_spot_order_limit_price(order_data):
+    if order_data.order_type in ["LIMIT", "LIMIT_MAKER"] and order_data.price is None:
+        raise ValueError("Price must be specified for limit orders.")
 
-    if orderData.orderType not in BybitExchange.spotOrderTypes:
+
+def check_spot_order_time_in_force(order_data):
+    if order_data.time_in_force not in BybitExchange.spot_time_in_forces:
         raise ValueError(
-            "Order type not correctly specified. Available order types for spot market: {}".format(
-                BybitExchange.spotOrderTypes
+            "Time-in-force not correctly specified. Available time-in-force for spot market: {}".format(
+                BybitExchange.spot_time_in_forces
             )
         )
 
-    if orderData.side not in ["BUY", "SELL"]:
+
+def check_spot_order_mandatory_fields(order_data):
+    if (
+        order_data.symbol is None
+        or order_data.quantity is None
+        or order_data.side is None
+        or order_data.order_type is None
+    ):
+        raise ValueError("Missing mandatory fields.")
+
+
+def check_spot_order_side(order_data):
+    if order_data.side not in ["BUY", "SELL"]:
         raise ValueError("Order side can only be 'BUY' or 'SELL'")
 
-    if orderData.timeInForce not in BybitExchange.spotTimeInForces:
+
+def check_spot_order_type(order_data):
+    if order_data.order_type not in BybitExchange.spot_order_types:
         raise ValueError(
-            "Time-in-force not correctly specified. Available time-in-force for spot market: {}".format(
-                BybitExchange.spotTimeInForces
+            "Order type not correctly specified. Available order types for spot market: {}".format(
+                BybitExchange.spot_order_types
             )
         )
 
-    if orderData.orderType in ["LIMIT", "LIMIT_MAKER"] and orderData.price is None:
-        raise ValueError("Price must be specified for limit orders.")
 
+def is_futures_order_data_valid(order_data: DataHelpers.FuturesOrderData):
+    check_futures_order_symbol(order_data)
+    check_futures_order_quantity(order_data)
+    check_futures_order_side(order_data)
+    check_futures_order_type(order_data)
+    check_futures_order_time_in_force(order_data)
+    check_futures_order_close_position(order_data)
+    check_futures_order_reduce_only(order_data)
 
-def isFuturesOrderDataValid(orderData: DataHelpers.FuturesOrderData):
-    if orderData.symbol is None:
-        raise ValueError("Specify symbol.")
-    if orderData.quantity is None:
-        raise ValueError("Specify quantity.")
-    if orderData.side is None:
-        raise ValueError("Specify order side.")
-    if orderData.orderType is None:
-        raise ValueError("Specify order type.")
-    if orderData.timeInForce is None:
-        raise ValueError("Specify timeInForce.")
-    if orderData.closePosition is None:
-        raise ValueError("Specify closePosition.")
-    if orderData.reduceOnly is None:
+    if order_data.orderType.startswith("STOP"):
+        check_futures_stop_order_datas(order_data)
+
+    if "LIMIT" in order_data.orderType and order_data.price is None:
+        raise ValueError("Specify 'price' for limit orders.")
+
+    if order_data.extra_params is not None:
+        check_futures_order_trigger_by(order_data)
+        check_futures_order_tp_trigger_by(order_data)
+        check_futures_order_sl_trigger_by(order_data)
+        check_futures_order_position_idx(order_data)
+
+
+def check_futures_order_position_idx(order_data):
+    if "positionIdx" in order_data.extra_params.keys() and order_data.extra_params[
+        "positionIdx"
+    ] not in [0, 1, 2]:
+        raise ValueError("'positionIdx' was not correctly specified.")
+
+
+def check_futures_order_sl_trigger_by(order_data):
+    if "slTriggerBy" in order_data.extra_params.keys() and order_data.extra_params[
+        "slTriggerBy"
+    ] not in ["LastPrice", "IndexPrice", "MarkPrice"]:
+        raise ValueError("'slTriggerBy' was not correctly specified.")
+
+
+def check_futures_order_tp_trigger_by(order_data):
+    if "tpTriggerBy" in order_data.extra_params.keys() and order_data.extra_params[
+        "tpTriggerBy"
+    ] not in ["LastPrice", "IndexPrice", "MarkPrice"]:
+        raise ValueError("'tpTriggerBy' was not correctly specified.")
+
+
+def check_futures_order_trigger_by(order_data):
+    if "triggerBy" in order_data.extra_params.keys() and order_data.extra_params[
+        "tpTriggerBy"
+    ] not in ["LastPrice", "IndexPrice", "MarkPrice"]:
+        raise ValueError("'triggerBy' was not correctly specified.")
+
+
+def check_futures_stop_order_datas(order_data):
+    if order_data.extra_params is None:
+        raise ValueError("Specify 'basePrice' in 'extraParams'")
+    if "basePrice" not in order_data.extra_params.keys():
+        raise ValueError("Specify 'basePrice' in 'extraParams'")
+    if order_data.stop_price is None:
+        raise ValueError("Specify 'stopPrice'.")
+
+
+def check_futures_order_reduce_only(order_data):
+    if order_data.reduce_only is None:
         raise ValueError("Specify reduceOnly.")
 
-    if orderData.orderType not in BybitExchange.futuresOrderTypes:
+
+def check_futures_order_close_position(order_data):
+    if order_data.close_position is None:
+        raise ValueError("Specify closePosition.")
+
+
+def check_futures_order_time_in_force(order_data):
+    if order_data.time_in_force is None:
+        raise ValueError("Specify timeInForce.")
+
+    if (
+        order_data.time_in_force not in BybitExchange.futures_time_in_forces.keys()
+        and order_data.time_in_force
+        not in BybitExchange.futures_time_in_forces.values()
+    ):
+        raise ValueError("'timeInForce' is not correct.")
+
+
+def check_futures_order_type(order_data):
+    if order_data.order_type is None:
+        raise ValueError("Specify order type.")
+
+    if order_data.order_type not in BybitExchange.futures_order_types:
         raise ValueError(
             "Bad order type specified. Available order types for futures: {}".format(
-                BybitExchange.futuresOrderTypes
+                BybitExchange.futures_order_types
             )
         )
 
-    if orderData.orderType.startswith("STOP"):
-        if orderData.extraParams is None:
-            raise ValueError("Specify 'basePrice' in 'extraParams'")
-        if "basePrice" not in orderData.extraParams.keys():
-            raise ValueError("Specify 'basePrice' in 'extraParams'")
-        if orderData.stopPrice is None:
-            raise ValueError("Specify 'stopPrice'.")
 
-    if "LIMIT" in orderData.orderType and orderData.price is None:
-        raise ValueError("Specify 'price' for limit orders.")
+def check_futures_order_side(order_data):
+    if order_data.side is None:
+        raise ValueError("Specify order side.")
 
-    if (
-        orderData.timeInForce not in BybitExchange.futuresTimeInForces.keys()
-        and orderData.timeInForce not in BybitExchange.futuresTimeInForces.values()
-    ):
-        raise ValueError("'timeInForce' is not correct.")
 
-    if orderData.extraParams is not None:
-        if "triggerBy" in orderData.extraParams.keys() and orderData.extraParams[
-            "tpTriggerBy"
-        ] not in ["LastPrice", "IndexPrice", "MarkPrice"]:
-            raise ValueError("'triggerBy' was not correctly specified.")
-
-        if "tpTriggerBy" in orderData.extraParams.keys() and orderData.extraParams[
-            "tpTriggerBy"
-        ] not in ["LastPrice", "IndexPrice", "MarkPrice"]:
-            raise ValueError("'tpTriggerBy' was not correctly specified.")
-
-        if "slTriggerBy" in orderData.extraParams.keys() and orderData.extraParams[
-            "slTriggerBy"
-        ] not in ["LastPrice", "IndexPrice", "MarkPrice"]:
-            raise ValueError("'slTriggerBy' was not correctly specified.")
-
-        if "positionIdx" in orderData.extraParams.keys() and orderData.extraParams[
-            "positionIdx"
-        ] not in [0, 1, 2]:
-            raise ValueError("'positionIdx' was not correctly specified.")
+def check_futures_order_quantity(order_data):
+    if order_data.quantity is None:
+        raise ValueError("Specify quantity.")
+
+
+def check_futures_order_symbol(order_data):
+    if order_data.symbol is None:
+        raise ValueError("Specify symbol.")
 
 
 class PyBitHTTP(HTTP):
     def __init__(
         self,
-        endpoint=None,
+        testnet=False,
         api_key=None,
         api_secret=None,
-        logging_level=logging.INFO,
-        log_requests=False,
-        request_timeout=10,
-        recv_window=5000,
-        force_retry=False,
-        retry_codes=None,
-        ignore_codes=None,
-        max_retries=3,
-        retry_delay=3,
-        referral_id=None,
-        spot=False,
     ):
         super().__init__(
-            endpoint,
-            api_key,
-            api_secret,
-            logging_level,
-            log_requests,
-            request_timeout,
-            recv_window,
-            force_retry,
-            retry_codes,
-            ignore_codes,
-            max_retries,
-            retry_delay,
-            referral_id,
-            spot,
+            testnet=testnet,
+            api_key=api_key,
+            api_secret=api_secret,
         )
 
     def query_history_order(self, **kwargs):
         if self.spot is True:
             suffix = "/spot/v1/history-orders"
 
             return self._submit_request(
@@ -153,29 +197,29 @@
                 method="GET", path=self.endpoint + suffix, query=kwargs, auth=True
             )
         else:
             raise NotImplementedError("Not implemented for futures market.")
 
 
 class BybitExchange(BaseExchange):
-    timeIndexesInCandleData = [0, 6]
-    desiredCandleDataIndexes = [0, 1, 2, 3, 4, 5, 6, 8]
+    time_indexes_in_candle_data = [0, 6]
+    desired_candle_data_indexes = [0, 1, 2, 3, 4, 5, 6, 8]
 
-    spotOrderTypes = ["LIMIT", "MARKET", "LIMIT_MAKER"]
-    spotTimeInForces = ["GTC", "FOK", "IOC"]
+    spot_order_types = ["LIMIT", "MARKET", "LIMIT_MAKER"]
+    spot_time_in_forces = ["GTC", "FOK", "IOC"]
 
-    futuresOrderTypes = ["MARKET", "LIMIT", "STOP_MARKET", "STOP_LIMIT"]
-    futuresTimeInForces = {
+    futures_order_types = ["MARKET", "LIMIT", "STOP_MARKET", "STOP_LIMIT"]
+    futures_time_in_forces = {
         "GTC": "GoodTillCancel",
         "IOC": "ImmediateOrCancel",
         "FIK": "FillOrKill",
         "PO": "PostOnly",
     }
 
-    timeIntervals = [
+    time_intervals = [
         "1m",
         "3m",
         "5m",
         "15m",
         "30m",
         "1h",
         "2h",
@@ -183,793 +227,778 @@
         "6h",
         "12h",
         "1d",
         "1w",
         "1M",
     ]
 
-    def __init__(self, credentials, sandbox=False, unifiedInOuts=True):
-        self.apiKey = credentials["spot"]["key"]
+    def __init__(self, credentials, sandbox=False, unified_in_outs=True):
+        self.api_key = credentials["spot"]["key"]
         self.secret = credentials["spot"]["secret"]
         self.sandbox = sandbox
-        self.unifiedInOuts = unifiedInOuts
+        self.unified_in_outs = unified_in_outs
 
         if sandbox:
-            self.spotSession = PyBitHTTP(
-                "https://api-testnet.bybit.com",
-                api_key=self.apiKey,
-                api_secret=self.secret,
-                spot=True,
+            self.spot_session = PyBitHTTP(
+                testnet=True, api_key=self.api_key, api_secret=self.secret
             )
-            self.futuresSession = PyBitHTTP(
-                "https://api-testnet.bybit.com",
-                api_key=self.apiKey,
+            self.futures_session = PyBitHTTP(
+                testnet=True,
+                api_key=self.api_key,
                 api_secret=self.secret,
             )
         else:
-            self.spotSession = PyBitHTTP(
-                "https://api.bybit.com",
-                api_key=self.apiKey,
-                api_secret=self.secret,
-                spot=True,
+            self.spot_session = PyBitHTTP(
+                testnet=False, api_key=self.api_key, api_secret=self.secret
             )
-            self.futuresSession = PyBitHTTP(
-                "https://api.bybit.com", api_key=self.apiKey, api_secret=self.secret
+            self.futures_session = PyBitHTTP(
+                testnet=False, api_key=self.api_key, api_secret=self.secret
             )
 
-        self.futuresSymbols = []
-        for symbol in self.futuresSession.query_symbol()["result"]:
-            if symbol["name"].endswith("USDT"):
-                self.futuresSymbols.append(symbol["name"])
-
     def get_balance(self, asset="", futures=False):
         if futures:
-            if asset in [None, ""]:
-                return BybitHelpers.getBalanceOut(
-                    self.futuresSession.get_wallet_balance()["result"], futures=True
+            return (
+                BybitHelpers.get_balance_out(
+                    self.futures_session.get_wallet_balance(accountType="CONTRACT")[
+                        "result"
+                    ],
+                    futures=True,
                 )
-            else:
-                return BybitHelpers.getBalanceOut(
-                    self.futuresSession.get_wallet_balance(coin=asset)["result"],
+                if asset in [None, ""]
+                else BybitHelpers.get_balance_out(
+                    self.futures_session.get_wallet_balance(
+                        accountType="CONTRACT", coin=asset
+                    )["result"],
                     single=True,
                     futures=True,
                 )
-        else:
-            if asset in [None, ""]:
-                return BybitHelpers.getBalanceOut(
-                    self.spotSession.get_wallet_balance()["result"]["balances"]
-                )
-            else:
-                assets = self.spotSession.get_wallet_balance()["result"]["balances"]
-                for coin in assets:
-                    if asset == coin["coin"]:
-                        return BybitHelpers.getBalanceOut(coin, single=True)
+            )
+        if asset in [None, ""]:
+            return BybitHelpers.get_balance_out(
+                self.spot_session.get_wallet_balance(accountType="SPOT")["result"][
+                    "balances"
+                ]
+            )
+        assets = self.spot_session.get_wallet_balance(accountType="SPOT")["result"][
+            "balances"
+        ]
+        for coin in assets:
+            if asset == coin["coin"]:
+                return BybitHelpers.get_balance_out(coin, single=True)
 
-                try:
-                    self.futuresSession.get_wallet_balance(coin=asset)
-                    return BybitHelpers.makeDummyBalance(asset)
-                except Exception:
-                    raise ValueError("Coin not found.")
+        try:
+            self.futures_session.get_wallet_balance(coin=asset)
+            return BybitHelpers.make_dummy_balance(asset)
+        except Exception as e:
+            raise ValueError("Coin not found.") from e
 
-    def symbolAccountTradeHistory(self, symbol, futures=False, fromId=None, limit=None):
+    def symbol_account_trade_history(
+        self, symbol, futures=False, from_id=None, limit=None
+    ):
         if futures:
-            tradeHistory = self.futuresSession.user_trade_records(
-                symbol=symbol, limit=limit, fromId=fromId
+            trade_history = self.futures_session.user_trade_records(
+                symbol=symbol, limit=limit, fromId=from_id
             )
-            return BybitHelpers.getMyTradeHistoryOut(
-                tradeHistory["result"]["data"], futures=True
+            return BybitHelpers.get_my_trade_history_out(
+                trade_history["result"]["data"], futures=True
             )
         else:
-            tradeHistory = self.spotSession.user_trade_records(
-                symbol=symbol, limit=limit, fromId=fromId
+            trade_history = self.spot_session.user_trade_records(
+                symbol=symbol, limit=limit, fromId=from_id
             )
-            return BybitHelpers.getMyTradeHistoryOut(tradeHistory["result"])
+            return BybitHelpers.get_my_trade_history_out(trade_history["result"])
 
-    def testSpotOrder(self, orderData: DataHelpers.OrderData):
-        isOrderDataValid(orderData)
+    def test_spot_order(self, order_data: DataHelpers.OrderData):
+        is_spot_order_data_valid(order_data)
 
+        # sourcery skip: no-conditionals-in-tests
         if (
-            orderData.icebergQty is not None
-            or orderData.newOrderRespType is not None
-            or orderData.quoteOrderQty is not None
-            or orderData.recvWindow is not None
-            or orderData.stopPrice is not None
+            order_data.iceberg_qty is not None
+            or order_data.new_order_resp_type is not None
+            or order_data.quote_order_qty is not None
+            or order_data.recv_window is not None
+            or order_data.stop_price is not None
         ):
             warnings.warn("Some of the given parameters have no use in ByBit exchange.")
 
-        return orderData
+        return order_data
 
-    def makeSpotOrder(self, orderData):
-        orderParams = BybitHelpers.getSpotOrderAsDict(orderData)
+    def make_spot_order(self, order_data):
+        order_params = BybitHelpers.get_spot_order_as_dict(order_data)
 
-        return BybitHelpers.getMakeSpotOrderOut(
-            self.spotSession.place_active_order(**orderParams)["result"]
+        return BybitHelpers.get_make_spot_order_out(
+            self.spot_session.place_active_order(**order_params)["result"]
         )
 
-    def createAndTestSpotOrder(
+    def create_and_test_spot_order(
         self,
         symbol,
         side,
-        orderType,
+        order_type,
         quantity=None,
         price=None,
-        timeInForce=None,
-        stopPrice=None,
-        icebergQty=None,
-        newOrderRespType=None,
-        newClientOrderId=None,
-        extraParams=None,
-    ):
-        currOrder = DataHelpers.setSpotOrderData(
-            icebergQty,
-            newClientOrderId,
-            newOrderRespType,
-            orderType,
+        time_in_force=None,
+        stop_price=None,
+        iceberg_qty=None,
+        new_order_resp_type=None,
+        new_client_order_id=None,
+        extra_params=None,
+    ):
+        curr_order = DataHelpers.set_spot_order_data(
+            iceberg_qty,
+            new_client_order_id,
+            new_order_resp_type,
+            order_type,
             price,
             quantity,
             side,
-            stopPrice,
+            stop_price,
             symbol,
-            timeInForce,
-            extraParams,
+            time_in_force,
+            extra_params,
         )
 
-        self.testSpotOrder(currOrder)
+        self.test_spot_order(curr_order)
 
-        return currOrder
+        return curr_order
 
-    def getSymbolOrders(
+    def get_symbol_orders(
         self,
         symbol,
         futures=False,
-        orderId=None,
-        startTime=None,
-        endTime=None,
+        order_id=None,
+        start_time=None,
+        end_time=None,
         limit=None,
     ):
         if futures:
-            historyList = []
-            pageNumber = 1
-            endTimeString = None
-            startTimeString = None
+            history_list = []
+            page_number = 1
+            end_time_string = None
+            start_time_string = None
             done = False
 
             while not done:
-                history = self.futuresSession.get_active_order(
-                    symbol=symbol, page=pageNumber, limit=50
+                history = self.futures_session.get_active_order(
+                    symbol=symbol, page=page_number, limit=50
                 )
 
-                if startTime is not None:
-                    startTimeString = startTime.strftime("%Y-%m-%dT%H:%M:%SZ")
-                if endTime is not None:
-                    endTimeString = endTime.strftime("%Y-%m-%dT%H:%M:%SZ")
+                if start_time is not None:
+                    start_time_string = start_time.strftime("%Y-%m-%dT%H:%M:%SZ")
+                if end_time is not None:
+                    end_time_string = end_time.strftime("%Y-%m-%dT%H:%M:%SZ")
 
                 for order in history["result"]["data"]:
-                    if endTime is not None and endTimeString < order["create_time"]:
+                    if end_time is not None and end_time_string < order["create_time"]:
                         continue
 
                     if (
-                        startTime is not None
-                        and order["created_time"] < startTimeString
+                        start_time is not None
+                        and order["created_time"] < start_time_string
                     ):
                         done = True
                         break
 
-                    historyList.append(order)
+                    history_list.append(order)
 
-                if limit is not None and limit <= len(historyList):
+                if limit is not None and limit <= len(history_list):
                     done = True
 
                 if len(history["result"]["data"]) < 50:
                     done = True
 
-                pageNumber += 1
+                page_number += 1
 
-            return historyList
+            return history_list
         else:
-            history = self.spotSession.query_history_order(
+            history = self.spot_session.query_history_order(
                 symbol=symbol,
-                orderId=orderId,
-                startTime=startTime,
-                endtime=endTime,
+                orderId=order_id,
+                startTime=start_time,
+                endtime=end_time,
                 limit=limit,
             )
             return history["result"]
 
-    def getOpenOrders(self, symbol, futures=False):
+    def get_open_orders(self, symbol, futures=False):
         if futures:
-            openOrders = []
-
-            openActiveOrders = self.futuresSession.query_active_order(symbol=symbol)
-            for activeOrder in openActiveOrders["result"]:
-                openOrders.append(BybitHelpers.futuresOrderOut(activeOrder))
+            return self.get_futures_open_orders(symbol)
+        else:
+            return self.get_spot_open_orders(symbol)
 
-            openConditionalOrders = self.futuresSession.query_conditional_order(
-                symbol=symbol
-            )
-            for conditionalOrder in openConditionalOrders["result"]:
-                openOrders.append(
-                    BybitHelpers.futuresOrderOut(conditionalOrder, isConditional=True)
-                )
+    def get_spot_open_orders(self, symbol):
+        open_orders = (
+            self.spot_session.query_active_order()["result"]
+            if symbol is None
+            else self.spot_session.query_active_order(symbol=symbol)["result"]
+        )
+        return BybitHelpers.get_open_orders_out(open_orders)
 
-            return openOrders
-        else:
-            if symbol is None:
-                openOrders = self.spotSession.query_active_order()["result"]
-            else:
-                openOrders = self.spotSession.query_active_order(symbol=symbol)[
-                    "result"
-                ]
-            return BybitHelpers.getOpenOrdersOut(openOrders)
+    def get_futures_open_orders(self, symbol):
+        open_active_orders = self.futures_session.query_active_order(symbol=symbol)
+        open_orders = [
+            BybitHelpers.futures_order_out(activeOrder)
+            for activeOrder in open_active_orders["result"]
+        ]
+        open_conditional_orders = self.futures_session.query_conditional_order(
+            symbol=symbol
+        )
+        open_orders.extend(
+            BybitHelpers.futures_order_out(conditionalOrder, is_conditional=True)
+            for conditionalOrder in open_conditional_orders["result"]
+        )
+        return open_orders
 
-    def cancelAllSymbolOpenOrders(self, symbol, futures=False):
+    def cancel_all_symbol_open_orders(self, symbol, futures=False):
         if futures:
-            canceledOrdersIds = []
-            result = self.futuresSession.cancel_all_active_orders(symbol=symbol)
-            canceledOrdersIds.append(result["result"])
-
-            result = self.futuresSession.cancel_all_conditional_orders(symbol=symbol)
-            canceledOrdersIds.append(result["result"])
+            result = self.futures_session.cancel_all_active_orders(symbol=symbol)
+            canceled_orders_ids = [result["result"]]
+            result = self.futures_session.cancel_all_conditional_orders(symbol=symbol)
+            canceled_orders_ids.append(result["result"])
         else:
-            result = self.spotSession.batch_fast_cancel_active_order(
+            result = self.spot_session.batch_fast_cancel_active_order(
                 symbol=symbol, orderTypes="LIMIT,LIMIT_MAKER,MARKET"
             )
             return result["result"]["success"]
 
-    def cancelOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
+    def cancel_order(self, symbol, order_id=None, local_order_id=None, futures=False):
         if futures:
-            if orderId is not None:
+            return self.cancel_futures_order(local_order_id, order_id, symbol)
+        else:
+            return self.cancel_spot_order(local_order_id, order_id)
+
+    def cancel_spot_order(self, local_order_id, order_id):
+        if order_id is not None:
+            result = self.spot_session.cancel_active_order(orderId=order_id)
+        elif local_order_id is not None:
+            result = self.spot_session.cancel_active_order(orderLinkId=local_order_id)
+        else:
+            raise ValueError("Must specify either 'orderId' or 'localOrderId'")
+        return result
+
+    def cancel_futures_order(self, local_order_id, order_id, symbol):
+        if order_id is not None:
+            try:
+                result = self.futures_session.cancel_active_order(
+                    symbol=symbol, order_id=order_id
+                )
+            except Exception as e:
                 try:
-                    result = self.futuresSession.cancel_active_order(
-                        symbol=symbol, order_id=orderId
+                    result = self.futures_session.cancel_conditional_order(
+                        symbol=symbol, order_id=order_id
                     )
                 except Exception as e:
-                    try:
-                        result = self.futuresSession.cancel_conditional_order(
-                            symbol=symbol, order_id=orderId
-                        )
-                    except Exception as e:
-                        raise RuntimeError(
-                            "Problem in canceling order in bybit: {}".format(str(e))
-                        )
-            elif localOrderId is not None:
+                    raise RuntimeError(
+                        "Problem in canceling order in bybit: {}".format(str(e))
+                    ) from e
+        elif local_order_id is not None:
+            try:
+                result = self.futures_session.cancel_active_order(
+                    symbol=symbol, order_link_id=local_order_id
+                )
+            except Exception as e:
                 try:
-                    result = self.futuresSession.cancel_active_order(
-                        symbol=symbol, order_link_id=localOrderId
+                    result = self.futures_session.cancel_conditional_order(
+                        symbol=symbol, order_link_id=local_order_id
                     )
                 except Exception as e:
-                    try:
-                        result = self.futuresSession.cancel_conditional_order(
-                            symbol=symbol, order_link_id=localOrderId
-                        )
-                    except Exception as e:
-                        raise RuntimeError(
-                            "Problem in canceling order in bybit: {}".format(str(e))
-                        )
-            else:
-                raise ValueError("Must specify either 'orderId' or 'localOrderId'")
-
-            return result["result"]
+                    raise RuntimeError(
+                        "Problem in canceling order in bybit: {}".format(str(e))
+                    ) from e
         else:
-            if orderId is not None:
-                result = self.spotSession.cancel_active_order(orderId=orderId)
-            elif localOrderId is not None:
-                result = self.spotSession.cancel_active_order(orderLinkId=localOrderId)
-            else:
-                raise ValueError("Must specify either 'orderId' or 'localOrderId'")
-            return result["result"]
+            raise ValueError("Must specify either 'orderId' or 'localOrderId'")
+        return result
 
-    def getOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
+    def get_order(self, symbol, order_id=None, local_order_id=None, futures=False):
         if futures:
-            if orderId is not None:
+            order = self.get_futures_order(local_order_id, order_id, symbol)
+            return BybitHelpers.futures_order_out(order["result"])
+        else:
+            order = self.get_spot_order(local_order_id, order_id)
+            return BybitHelpers.get_order_out(order)
+
+    def get_spot_order(self, local_order_id, order_id):
+        if order_id is not None:
+            try:
+                order = self.spot_session.get_active_order_spot(orderId=order_id)[
+                    "result"
+                ]
+            except Exception as e:
+                raise RuntimeError("Problem in fetching order from bybit.") from e
+        elif local_order_id is not None:
+            try:
+                order = self.spot_session.get_active_order_spot(
+                    orderLinkId=local_order_id
+                )["result"]
+            except Exception as e:
+                raise RuntimeError("Problem in fetching order from bybit.") from e
+        else:
+            raise ValueError(
+                "Specify either order Id in the exchange or local Id sent with the order"
+            )
+        return order
+
+    def get_futures_order(self, local_order_id, order_id, symbol):
+        if order_id is not None:
+            try:
+                order = self.futures_session.query_active_order(
+                    symbol=symbol, order_id=order_id
+                )
+            except Exception as e:
                 try:
-                    order = self.futuresSession.query_active_order(
-                        symbol=symbol, order_id=orderId
+                    order = self.futures_session.query_conditional_order(
+                        symbol=symbol, order_id=order_id
                     )
                 except Exception as e:
-                    try:
-                        order = self.futuresSession.query_conditional_order(
-                            symbol=symbol, order_id=orderId
-                        )
-                    except Exception as e:
-                        raise RuntimeError(
-                            "Problem in fetching order from bybit: {}".format(str(e))
-                        )
-            elif localOrderId is not None:
+                    raise RuntimeError(
+                        "Problem in fetching order from bybit: {}".format(str(e))
+                    ) from e
+        elif local_order_id is not None:
+            try:
+                order = self.futures_session.query_active_order(
+                    symbol=symbol, order_link_id=local_order_id
+                )
+            except Exception as e:
                 try:
-                    order = self.futuresSession.query_active_order(
-                        symbol=symbol, order_link_id=localOrderId
+                    order = self.futures_session.query_conditional_order(
+                        symbol=symbol, order_link_id=local_order_id
                     )
                 except Exception as e:
-                    try:
-                        order = self.futuresSession.query_conditional_order(
-                            symbol=symbol, order_link_id=localOrderId
-                        )
-                    except Exception as e:
-                        raise RuntimeError(
-                            "Problem in fetching order from bybit: {}".format(str(e))
-                        )
-            else:
-                raise ValueError(
-                    "Specify either order Id in the exchange or local Id sent with the order"
-                )
-
-            return BybitHelpers.futuresOrderOut(order["result"])
+                    raise RuntimeError(
+                        "Problem in fetching order from bybit: {}".format(str(e))
+                    ) from e
         else:
-            if orderId is not None:
-                try:
-                    order = self.spotSession.get_active_order_spot(orderId=orderId)[
-                        "result"
-                    ]
-                except Exception as e:
-                    raise RuntimeError("Problem in fetching order from bybit.")
-            elif localOrderId is not None:
-                try:
-                    order = self.spotSession.get_active_order_spot(
-                        orderLinkId=localOrderId
-                    )["result"]
-                except Exception as e:
-                    raise RuntimeError("Problem in fetching order from bybit.")
-            else:
-                raise ValueError(
-                    "Specify either order Id in the exchange or local Id sent with the order"
-                )
-
-            return BybitHelpers.getOrderOut(order)
+            raise ValueError(
+                "Specify either order Id in the exchange or local Id sent with the order"
+            )
+        return order
 
-    def getTradingFees(self, futures=False):
+    def get_trading_fees(self, futures=False):
         raise NotImplementedError()
 
-    def getSymbolTickerPrice(self, symbol, futures=False):
+    def get_symbol_ticker_price(self, symbol, futures=False):
         if futures:
-            symbolInfo = self.futuresSession.latest_information_for_symbol(
+            symbol_info = self.futures_session.latest_information_for_symbol(
                 symbol=symbol
             )["result"]
-            return float(symbolInfo[0]["last_price"])
+            return float(symbol_info[0]["last_price"])
         else:
-            symbolInfo = self.spotSession.latest_information_for_symbol(symbol=symbol)
-            return float(symbolInfo["result"]["lastPrice"])
+            symbol_info = self.spot_session.latest_information_for_symbol(symbol=symbol)
+            return float(symbol_info["result"]["lastPrice"])
 
-    def getSymbolKlines(
+    def get_symbol_klines(
         self,
         symbol,
         interval,
-        startTime=None,
-        endTime=None,
+        start_time=None,
+        end_time=None,
         limit=None,
         futures=False,
         blvtnav=False,
-        convertDateTime=False,
-        doClean=False,
-        toCleanDataframe=False,
+        convert_date_time=False,
+        do_clean=False,
+        to_clean_dataframe=False,
     ):
-        if interval not in self.timeIntervals:
+        if interval not in self.time_intervals:
             raise ValueError("Time interval is not valid.")
 
         if futures:
-            data = self._getFuturesSymbolKlines(interval, limit, startTime, symbol)
+            data = self._get_futures_symbol_klines(interval, limit, start_time, symbol)
         else:
-            data = self._getSpotSymbolKlines(
-                endTime, interval, limit, startTime, symbol
+            data = self._get_spot_symbol_klines(
+                end_time, interval, limit, start_time, symbol
             )
 
-        if convertDateTime or toCleanDataframe:
-            BybitHelpers.klinesConvertDate(data, futures, self.timeIndexesInCandleData)
-
-        if doClean or toCleanDataframe:
-            finalDataArray = BybitHelpers.getKlinesDesiredOnlyCols(
-                data, self.desiredCandleDataIndexes
+        if convert_date_time or to_clean_dataframe:
+            BybitHelpers.klines_convert_date(
+                data, futures, self.time_indexes_in_candle_data
             )
 
-            if toCleanDataframe:
-                return BybitHelpers.klinesConvertToPandas(finalDataArray)
-            return finalDataArray
-        else:
+        if not do_clean and not to_clean_dataframe:
             return data
+        final_data_array = BybitHelpers.get_klines_desired_only_cols(
+            data, self.desired_candle_data_indexes
+        )
 
-    def _getSpotSymbolKlines(self, endTime, interval, limit, startTime, symbol):
-        if startTime is not None:
-            startTimestamp = startTime.timestamp() * 1000
-        else:
-            startTimestamp = None
-        if endTime is not None:
-            endTimestamp = endTime.timestamp() * 1000
-        else:
-            endTimestamp = None
+        if to_clean_dataframe:
+            return BybitHelpers.klines_convert_to_pandas(final_data_array)
+        return final_data_array
+
+    def _get_spot_symbol_klines(self, end_time, interval, limit, start_time, symbol):
+        start_timestamp = None if start_time is None else start_time.timestamp() * 1000
+        end_timestamp = end_time.timestamp() * 1000 if end_time is not None else None
 
         if limit is not None:
             if limit > 1000:
                 limit = 1000
             elif limit < 1:
                 limit = 1
-        data = self.spotSession.query_kline(
+
+        data = self.spot_session.query_kline(
             symbol=symbol,
             interval=interval,
-            startTime=startTimestamp,
-            endTime=endTimestamp,
+            startTime=start_timestamp,
+            endTime=end_timestamp,
             limit=limit,
         )["result"]
         for datum in data:
             for idx in range(len(datum)):
-                if idx in self.timeIndexesInCandleData:
+                if idx in self.time_indexes_in_candle_data:
                     continue
                 datum[idx] = float(datum[idx])
         return data
 
-    def _getFuturesSymbolKlines(self, interval, limit, startTime, symbol):
-        futuresInterval = BybitHelpers.convertIntervalToFuturesKlines(interval)
+    def _get_futures_symbol_klines(self, interval, limit, start_time, symbol):
+        futures_interval = BybitHelpers.convert_interval_to_futures_klines(interval)
         data = []
-        if limit is not None:
-            if limit > 200:
-                limit = 200
-            elif limit < 1:
-                limit = 1
-        else:
+
+        if limit is not None and limit > 200 or limit is None:
             limit = 200
-        if startTime is None:
-            startTimestamp = int(
+        elif limit < 1:
+            limit = 1
+
+        if start_time is None:
+            start_timestamp = int(
                 datetime.now().timestamp()
-                - BybitHelpers.getIntervalInSeconds(interval, self.timeIntervals)
+                - BybitHelpers.get_interval_in_seconds(interval, self.time_intervals)
                 * limit
             )
+        elif isinstance(start_time, int):
+            start_timestamp = start_time
         else:
-            if isinstance(startTime, int):
-                startTimestamp = startTime
-            else:
-                startTimestamp = int(startTime.timestamp)
-        candles = self.futuresSession.query_kline(
+            start_timestamp = int(start_time.timestamp)
+
+        candles = self.futures_session.query_kline(
             symbol=symbol,
-            interval=futuresInterval,
-            from_time=startTimestamp,
+            interval=futures_interval,
+            from_time=start_timestamp,
             limit=limit,
         )
         for candle in candles["result"]:
-            dataArray = [
+            data_array = [
                 float(candle["open_time"]),
                 float(candle["open"]),
                 float(candle["high"]),
                 float(candle["low"]),
                 float(candle["close"]),
                 float(candle["volume"]),
                 int(candle["open_time"])
-                + BybitHelpers.getIntervalInSeconds(interval, self.timeIntervals),
+                + BybitHelpers.get_interval_in_seconds(interval, self.time_intervals),
                 None,
                 None,
                 None,
                 None,
             ]
-            data.append(dataArray)
+            data.append(data_array)
         return data
 
-    def getExchangeTime(self, futures=False):
+    def get_exchange_time(self, futures=False):
         if futures:
-            return self.futuresSession.server_time()["time_now"]
+            return self.futures_session.server_time()["time_now"]
         else:
-            return int(self.spotSession.server_time()["result"]["serverTime"])
+            return int(self.spot_session.server_time()["result"]["serverTime"])
 
-    def getSymbol24hTicker(self, symbol):
+    def get_symbol_24h_ticker(self, symbol):
         raise NotImplementedError()
 
-    def testFuturesOrder(self, futuresOrderData):
-        if futuresOrderData.timeInForce is None:
-            futuresOrderData.timeInForce = "GoodTillCancel"
+    def test_futures_order(self, futures_order_data):
+        # sourcery skip: no-conditionals-in-tests
+        if futures_order_data.time_in_force is None:
+            futures_order_data.time_in_force = "GoodTillCancel"
 
-        if futuresOrderData.closePosition is None:
-            futuresOrderData.closePosition = False
+        if futures_order_data.close_position is None:
+            futures_order_data.close_position = False
 
-        if futuresOrderData.reduceOnly is None:
-            futuresOrderData.reduceOnly = False
+        if futures_order_data.reduce_only is None:
+            futures_order_data.reduce_only = False
 
-        isFuturesOrderDataValid(futuresOrderData)
+        is_futures_order_data_valid(futures_order_data)
 
-        return futuresOrderData
+        return futures_order_data
 
-    def makeFuturesOrder(self, futuresOrderData: DataHelpers.FuturesOrderData):
-        orderParams = BybitHelpers.getFuturesOrderAsDict(
-            futuresOrderData, self.futuresTimeInForces
+    def make_futures_order(self, futures_order_data: DataHelpers.FuturesOrderData):
+        order_params = BybitHelpers.get_futures_order_as_dict(
+            futures_order_data, self.futures_time_in_forces
         )
 
-        if "STOP" in futuresOrderData.orderType:
-            result = self.futuresSession.place_conditional_order(**orderParams)
-            return BybitHelpers.futuresOrderOut(result["result"], isConditional=True)
+        if "STOP" in futures_order_data.orderType:
+            result = self.futures_session.place_conditional_order(**order_params)
+            return BybitHelpers.futures_order_out(result["result"], is_conditional=True)
         else:
-            result = self.futuresSession.place_active_order(**orderParams)
-            return BybitHelpers.futuresOrderOut(result["result"])
+            result = self.futures_session.place_active_order(**order_params)
+            return BybitHelpers.futures_order_out(result["result"])
 
-    def createAndTestFuturesOrder(
+    def create_and_test_futures_order(
         self,
         symbol,
         side,
-        orderType,
-        positionSide=None,
-        timeInForce=None,
+        order_type,
+        position_side=None,
+        time_in_force=None,
         quantity=None,
-        reduceOnly=None,
+        reduce_only=None,
         price=None,
-        newClientOrderId=None,
-        stopPrice=None,
-        closePosition=None,
-        activationPrice=None,
-        callbackRate=None,
-        workingType=None,
-        priceProtect=None,
-        newOrderRespType=None,
-        extraParams=None,
-        quoteQuantity=None,
-    ):
-        currOrder = DataHelpers.setFuturesOrderData(
-            activationPrice,
-            callbackRate,
-            closePosition,
-            extraParams,
-            newClientOrderId,
-            newOrderRespType,
-            orderType,
-            positionSide,
+        new_client_order_id=None,
+        stop_price=None,
+        close_position=None,
+        activation_price=None,
+        callback_rate=None,
+        working_type=None,
+        price_protect=None,
+        new_order_resp_type=None,
+        extra_params=None,
+        quote_quantity=None,
+    ):
+        curr_order = DataHelpers.set_futures_order_data(
+            activation_price,
+            callback_rate,
+            close_position,
+            extra_params,
+            new_client_order_id,
+            new_order_resp_type,
+            order_type,
+            position_side,
             price,
-            priceProtect,
+            price_protect,
             quantity,
-            reduceOnly,
+            reduce_only,
             side,
-            stopPrice,
+            stop_price,
             symbol,
-            timeInForce,
-            workingType,
-            quoteQuantity,
+            time_in_force,
+            working_type,
+            quote_quantity,
         )
 
-        self.testFuturesOrder(currOrder)
+        self.test_futures_order(curr_order)
 
-        return currOrder
+        return curr_order
 
-    def makeBatchFuturesOrder(self, futuresOrderDatas):
-        batchOrders = []
-        batchConditionalOrders = []
-        for order in futuresOrderDatas:
-            orderAsDict = BybitHelpers.getFuturesOrderAsDict(
-                order, self.futuresTimeInForces
+    def make_batch_futures_order(self, futures_order_datas):
+        batch_orders = []
+        batch_conditional_orders = []
+        for order in futures_order_datas:
+            order_as_dict = BybitHelpers.get_futures_order_as_dict(
+                order, self.futures_time_in_forces
             )
 
-            if "STOP" in order.orderType:
-                batchConditionalOrders.append(order)
+            if "STOP" in order.order_type:
+                batch_conditional_orders.append(order)
             else:
-                batchOrders.append(orderAsDict)
+                batch_orders.append(order_as_dict)
 
         results = []
-        if len(batchConditionalOrders) > 0:
-            putResults = self.futuresSession.place_conditional_order_bulk(
-                batchConditionalOrders
-            )
-            for result in putResults:
-                results.append(
-                    BybitHelpers.futuresOrderOut(result["result"], isConditional=True)
-                )
-        if len(batchOrders) > 0:
-            putResults = self.futuresSession.place_active_order_bulk(batchOrders)
-            for result in putResults:
-                results.append(BybitHelpers.futuresOrderOut(result["result"]))
-
+        if batch_conditional_orders:
+            put_results = self.futures_session.place_conditional_order_bulk(
+                batch_conditional_orders
+            )
+            results.extend(
+                BybitHelpers.futures_order_out(result["result"], is_conditional=True)
+                for result in put_results
+            )
+        if batch_orders:
+            put_results = self.futures_session.place_active_order_bulk(batch_orders)
+            results.extend(
+                BybitHelpers.futures_order_out(result["result"])
+                for result in put_results
+            )
         return results
 
-    def changeInitialLeverage(self, symbol, leverage):
-        return self.futuresSession.set_leverage(
+    def change_initial_leverage(self, symbol, leverage):
+        return self.futures_session.set_leverage(
             symbol=symbol, buy_leverage=leverage, sell_leverage=leverage
         )["result"]
 
-    def changeMarginType(self, symbol, marginType, params):
+    def change_margin_type(self, symbol, margin_type, params):
         try:
-            buyLeverage = params["buyLeverage"]
-            sellLeverage = params["sellLeverage"]
-            if marginType.upper() == "ISOLATED":
-                isIsolated = True
-            elif marginType.upper() == "CROSS":
-                isIsolated = False
+            buy_leverage = params["buyLeverage"]
+            sell_leverage = params["sellLeverage"]
+            if margin_type.upper() == "ISOLATED":
+                is_isolated = True
+            elif margin_type.upper() == "CROSS":
+                is_isolated = False
             else:
                 raise ValueError("Margin type must either be 'ISOLATED' or 'CROSS'.")
-        except Exception:
-            raise ValueError("Must specify 'buyLeverage' and 'sellLeverage' in 'params")
+        except Exception as e:
+            raise ValueError(
+                "Must specify 'buyLeverage' and 'sellLeverage' in 'params"
+            ) from e
 
-        self.futuresSession.cross_isolated_margin_switch(
+        self.futures_session.cross_isolated_margin_switch(
             symbol=symbol,
-            is_isolated=isIsolated,
-            buy_leverage=buyLeverage,
-            sell_leverage=sellLeverage,
+            is_isolated=is_isolated,
+            buy_leverage=buy_leverage,
+            sell_leverage=sell_leverage,
         )
         return True
 
-    def changePositionMargin(self, symbol, amount):
-        result = self.futuresSession.change_margin(symbol=symbol, margin=amount)
-        if result["ret_code"] == 0:
-            return True
-        else:
-            return False
+    def change_position_margin(self, symbol, amount):
+        result = self.futures_session.change_margin(symbol=symbol, margin=amount)
+        return result["ret_code"] == 0
 
-    def getPosition(self):
-        return self.futuresSession.my_position()["result"]
+    def get_position(self):
+        return self.futures_session.my_position()["result"]
 
-    def spotBestBidAsks(self, symbol=None):
-        return self.spotSession.best_bid_ask_price(symbol=symbol)["result"]
+    def spot_best_bid_asks(self, symbol=None):
+        return self.spot_session.best_bid_ask_price(symbol=symbol)["result"]
 
-    def getSymbolOrderBook(self, symbol, limit=None, futures=False):
+    def get_symbol_order_book(self, symbol, limit=None, futures=False):
         if futures:
-            return self.futuresSession.orderbook(symbol=symbol)["result"]
+            return self.futures_session.orderbook(symbol=symbol)["result"]
         else:
-            return self.spotSession.orderbook(symbol=symbol)["result"]
+            return self.spot_session.orderbook(symbol=symbol)["result"]
 
-    def getSymbolRecentTrades(self, symbol, limit=None, futures=False):
+    def get_symbol_recent_trades(self, symbol, limit=None, futures=False):
         if futures:
-            if limit is not None and limit > 0:
-                limit = 1000 if limit > 1000 else limit
-            else:
-                limit = 500
+            limit = min(limit, 1000) if limit is not None and limit > 0 else 500
 
-            recentTrades = self.futuresSession.public_trading_records(
+            recent_trades = self.futures_session.public_trading_records(
                 symbol=symbol, limit=limit
             )["result"]
-            return BybitHelpers.getRecentTradeHistoryOut(recentTrades, futures=True)
+            return BybitHelpers.get_recent_trade_history_out(
+                recent_trades, futures=True
+            )
         else:
-            if limit is not None and limit > 0:
-                limit = 60 if limit > 60 else limit
-            else:
-                limit = 60
+            limit = min(limit, 60) if limit is not None and limit > 0 else 60
 
-            recentTrades = self.spotSession.public_trading_records(
+            recent_trades = self.spot_session.public_trading_records(
                 symbol=symbol, limit=limit
             )["result"]
-            return BybitHelpers.getRecentTradeHistoryOut(recentTrades)
+            return BybitHelpers.get_recent_trade_history_out(recent_trades)
 
-    def getPositionInfo(self, symbol=None):
-        result = self.futuresSession.my_position(symbol=symbol)
+    def get_position_info(self, symbol=None):
+        result = self.futures_session.my_position(symbol=symbol)
         return result["result"]
 
-    def getSymbolMinTrade(self, symbol, futures=False):
-        symbolTickerPrice = self.getSymbolTickerPrice(symbol=symbol, futures=futures)
+    def get_symbol_min_trade(self, symbol, futures=False):
+        symbol_ticker_price = self.get_symbol_ticker_price(
+            symbol=symbol, futures=futures
+        )
 
-        minQuantity = None
-        minQuoteQuantity = None
-        stepQuantity = None
-        stepPrice = None
+        min_quantity = None
+        min_quote_quantity = None
+        step_quantity = None
+        step_price = None
 
         if futures:
-            symbolInfos = self.futuresSession.query_symbol()["result"]
+            symbol_infos = self.futures_session.query_symbol()["result"]
 
-            for symbolInfo in symbolInfos:
+            for symbolInfo in symbol_infos:
                 if symbolInfo["name"] == symbol:
-                    minQuantity = float(
+                    min_quantity = float(
                         symbolInfo["lot_size_filter"]["min_trading_qty"]
                     )
-                    minQuoteQuantity = symbolTickerPrice * minQuantity
-                    stepQuantity = float(symbolInfo["lot_size_filter"]["qty_step"])
-                    stepPrice = symbolInfo["price_filter"]["tick_size"]
+                    min_quote_quantity = symbol_ticker_price * min_quantity
+                    step_quantity = float(symbolInfo["lot_size_filter"]["qty_step"])
+                    step_price = symbolInfo["price_filter"]["tick_size"]
 
         else:
-            symbolInfos = self.spotSession.query_symbol()["result"]
+            symbol_infos = self.spot_session.query_symbol()["result"]
 
-            for symbolInfo in symbolInfos:
+            for symbolInfo in symbol_infos:
                 if symbolInfo["name"] == symbol:
-                    minQuantity = float(symbolInfo["minTradeQuantity"])
-                    minQuoteQuantity = float(symbolInfo["minTradeAmount"])
-                    stepQuantity = float(symbolInfo["basePrecision"])
-                    stepPrice = symbolInfo["minPricePrecision"]
+                    min_quantity = float(symbolInfo["minTradeQuantity"])
+                    min_quote_quantity = float(symbolInfo["minTradeAmount"])
+                    step_quantity = float(symbolInfo["basePrecision"])
+                    step_price = symbolInfo["minPricePrecision"]
 
         return {
-            "minQuantity": minQuantity,
-            "minQuoteQuantity": minQuoteQuantity,
-            "precisionStep": stepQuantity,
-            "stepPrice": stepPrice,
+            "minQuantity": min_quantity,
+            "minQuoteQuantity": min_quote_quantity,
+            "precisionStep": step_quantity,
+            "stepPrice": step_price,
         }
 
-    def makeSlTpLimitFuturesOrder(
+    def make_sl_tp_limit_futures_order(
         self,
         symbol,
-        orderSide,
+        order_side,
         quantity=None,
-        quoteQuantity=None,
-        enterPrice=None,
-        takeProfit=None,
-        stopLoss=None,
+        quote_quantity=None,
+        enter_price=None,
+        take_profit=None,
+        stop_loss=None,
         leverage=None,
-        marginType=None,
+        margin_type=None,
     ):
         if (
-            enterPrice is None
-            or takeProfit is None
-            or stopLoss is None
+            enter_price is None
+            or take_profit is None
+            or stop_loss is None
             or leverage is None
-            or marginType is None
+            or margin_type is None
         ):
             raise ValueError("Specify all inputs.")
 
-        symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
+        symbol_info = self.get_symbol_min_trade(symbol=symbol, futures=True)
 
-        quantity = DataHelpers.getQuantity(
-            enterPrice, quantity, quoteQuantity, symbolInfo["precisionStep"]
+        quantity = DataHelpers.get_quantity(
+            enter_price, quantity, quote_quantity, symbol_info["precisionStep"]
         )
 
-        self.setMarginLeverage(leverage, marginType, symbol)
-        orderParams = {
-            "takeProfit": takeProfit,
-            "stopLoss": stopLoss,
+        self.set_margin_leverage(leverage, margin_type, symbol)
+        order_params = {
+            "takeProfit": take_profit,
+            "stopLoss": stop_loss,
             "tpTriggerBy": "MarkPrice",
             "slTriggerBy": "MarkPrice",
         }
 
-        futuresOrder = self.createAndTestFuturesOrder(
+        futures_order = self.create_and_test_futures_order(
             symbol=symbol,
-            side=orderSide,
-            orderType="LIMIT",
-            timeInForce="GTC",
+            side=order_side,
+            order_type="LIMIT",
+            time_in_force="GTC",
             quantity=quantity,
-            price=enterPrice,
-            closePosition=False,
-            extraParams=orderParams,
+            price=enter_price,
+            close_position=False,
+            extra_params=order_params,
         )
-        orderingResult = self.makeFuturesOrder(futuresOrder)
-        return orderingResult["orderId"]
+        ordering_result = self.make_futures_order(futures_order)
+        return ordering_result["orderId"]
 
-    def setMarginLeverage(self, leverage, marginType, symbol):
+    def set_margin_leverage(self, leverage, margin_type, symbol):
         params = {"buyLeverage": leverage, "sellLeverage": leverage}
-        self.changeInitialLeverage(leverage, symbol)
-        self.changeMarginType(symbol, marginType, params)
+        self.change_initial_leverage(leverage, symbol)
+        self.change_margin_type(symbol, margin_type, params)
 
-    def getSymbol24hChanges(self, futures=False):
-        changesList = []
+    def get_symbol_24h_changes(self, futures=False):
+        changes_list = []
         if futures:
-            for ticker in self.futuresSession.latest_information_for_symbol()["result"]:
+            for ticker in self.futures_session.latest_information_for_symbol()[
+                "result"
+            ]:
                 print(ticker)
-                if ticker["is_block_trade"] == False:
-                    changesList.append((ticker["symbol"], 0))
-        else:
-            symbolInfos = self.spotSession.query_symbol()["result"]
-            for ticker in symbolInfos:
-                changesList.append((ticker["name"], 0))
-
-        return sorted(changesList, key=lambda x: x[1], reverse=True)
-
-    def getSymbolList(self, futures=False):
-        symbolNames = []
-        if futures:
-            for ticker in self.futuresMarket.get_contracts_list():
-                symbolNames.append(ticker["symbol"])
+                if not ticker["is_block_trade"]:
+                    changes_list.append((ticker["symbol"], 0))
         else:
-            for ticker in self.spotMarket.get_all_tickers()["ticker"]:
-                symbolNames.append(ticker["symbol"])
+            symbol_infos = self.spot_session.query_symbol()["result"]
+            changes_list.extend((ticker["name"], 0) for ticker in symbol_infos)
+        return sorted(changes_list, key=lambda x: x[1], reverse=True)
 
-        return symbolNames
+    def get_symbol_list(self, futures=False):
+        raise NotImplementedError()
 
-    def getLatestSymbolNames(self, numOfSymbols=None, futures=False):
-        symbolDatas = []
-        if futures:
-            for symbolInfo in self.futuresMarket.get_contracts_list():
-                symbolDatas.append(
-                    (
-                        symbolInfo["symbol"],
-                        datetime.fromtimestamp(
-                            float(symbolInfo["firstOpenDate"]) / 1000
-                        ),
-                    )
-                )
-                symbolDatas.sort(key=lambda x: x[1], reverse=True)
-            if numOfSymbols is not None and numOfSymbols > len(symbolDatas):
-                numOfSymbols = len(symbolDatas)
-        else:
-            raise NotImplementedError()
-        return symbolDatas[:numOfSymbols]
+    def get_latest_symbol_names(self, num_of_symbols=None, futures=False):
+        raise NotImplementedError()
 
-    def getIncomeHistory(
-        self, symbol, incomeType=None, startTime=None, endTime=None, limit=None
+    def get_income_history(
+        self, symbol, income_type=None, start_time=None, end_time=None, limit=None
     ):
         args = {
-            "start_date": startTime,
-            "end_date": endTime,
-            "wallet_fund_type": incomeType,
+            "start_date": start_time,
+            "end_date": end_time,
+            "wallet_fund_type": income_type,
             "limit": limit,
             "coin": symbol,
         }
         args = {k: v for k, v in args.items() if v is not None}
 
-        return self.futuresSession.wallet_fund_records(**args)
+        return self.futures_session.wallet_fund_records(**args)
 
-    def getLongShortRatios(
-        self, symbol, period, limit=None, startTime=None, endTime=None
+    def get_long_short_ratios(
+        self, symbol, period, limit=None, start_time=None, end_time=None
     ):
-        pass
+        raise NotImplementedError()
+
+    def get_deposit_address(self, coin, network=None):
+        raise NotImplementedError()
```

### Comparing `TradeGate-0.3.8/TradeGates/Exchanges/KuCoinExchange.py` & `TradeGate-0.3.8.1/TradeGates/Exchanges/KuCoinExchange.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,142 +28,142 @@
 
 
 def checkSpotOrderDataValid(orderData: DataHelpers.OrderData):
     checkOrderSide(orderData, futures=False)
     checkOrderSymbol(orderData)
     checkOrderType(orderData, futures=False)
 
-    if orderData.orderType == "market":
+    if orderData.order_type == "market":
         checkOrderSize(orderData)
     else:
-        if "limit" in orderData.orderType:
+        if "limit" in orderData.order_type:
             checkOrderPrice(orderData)
             checkOrderSize(orderData)
-        elif "stop" in orderData.orderType:
+        elif "stop" in orderData.order_type:
             checkStopOrderDatas(orderData)
 
         checkOrderTimeInForce(orderData)
         checkExtraParams(orderData)
 
 
 def checkFuturesOrderDataValid(orderData):
     checkOrderSide(orderData, futures=True)
     checkOrderSymbol(orderData)
     checkOrderType(orderData, futures=True)
 
-    if orderData.orderType == "market":
+    if orderData.order_type == "market":
         checkOrderSize(orderData, futures=True)
-    elif orderData.orderType == "limit":
+    elif orderData.order_type == "limit":
         checkOrderPrice(orderData)
         checkOrderSize(orderData, futures=True)
         checkOrderTimeInForce(orderData, futures=True)
         checkExtraParams(orderData, futures=True)
-    if orderData.stopPrice is not None:
+    if orderData.stop_price is not None:
         checkStopOrderDatas(orderData, futures=True)
 
 
 def checkExtraParams(orderData, futures=False):
-    if orderData.extraParams is not None:
+    if orderData.extra_params is not None:
         if futures:
             checkPostOnlyOrder(orderData, futures)
             checkIceBergOrder(orderData)
             checkOrderLeverage(orderData)
         else:
             checkCancelAfterOrder(orderData)
             checkPostOnlyOrder(orderData, futures)
 
 
 def checkCancelAfterOrder(orderData):
-    if "cancelAfter" in orderData.extraParams.keys():
-        if orderData.timeInForce != "GTT":
+    if "cancelAfter" in orderData.extra_params.keys():
+        if orderData.time_in_force != "GTT":
             raise ValueError(
                 "'cancelAfter' field can only be used with 'GTT' as 'timeInForce' field."
             )
 
 
 def checkOrderLeverage(orderData):
-    if "leverage" not in orderData.extraParams.keys():
-        if orderData.closePosition is None:
+    if "leverage" not in orderData.extra_params.keys():
+        if orderData.close_position is None:
             raise ValueError("Missing 'leverage' field.")
-        if not orderData.closePosition:
+        if not orderData.close_position:
             raise ValueError("Missing 'leverage' field.")
 
 
 def checkIceBergOrder(orderData):
-    if "iceberg" in orderData.extraParams.keys():
-        if "visibleSize" not in orderData.extraParams.keys():
+    if "iceberg" in orderData.extra_params.keys():
+        if "visibleSize" not in orderData.extra_params.keys():
             raise ValueError("Specify 'visibleSize' with 'iceberg' set as true")
 
 
 def checkPostOnlyOrder(orderData, futures=False):
-    if "postOnly" in orderData.extraParams.keys():
+    if "postOnly" in orderData.extra_params.keys():
         if futures:
-            if orderData.timeInForce in ["FOK"]:
+            if orderData.time_in_force in ["FOK"]:
                 raise ValueError(
                     "'postOnly' field can not be used with 'IOC' as 'timeInForce' field."
                 )
-            if "hidden" in orderData.extraParams.keys():
+            if "hidden" in orderData.extra_params.keys():
                 raise ValueError("Can't use 'hidden' with 'postOnly'")
-            if "iceberg" in orderData.extraParams.keys():
+            if "iceberg" in orderData.extra_params.keys():
                 raise ValueError("Can't use 'iceberg' with 'postOnly'")
         else:
-            if orderData.timeInForce in ["IOC", "FOK"]:
+            if orderData.time_in_force in ["IOC", "FOK"]:
                 raise ValueError(
                     "'postOnly' field can not be used with 'IOC' or 'FOK' as 'timeInForce' field."
                 )
 
 
 def checkOrderTimeInForce(orderData, futures=False):
     errorString = "Invalid value for 'timeInForce' specified"
 
     if futures:
         validValues = ["GTC", "IOC"]
     else:
         validValues = ["GTC", "GTT", "IOC", "FOK"]
 
-    if orderData.timeInForce not in validValues:
+    if orderData.time_in_force not in validValues:
         raise ValueError(errorString)
 
 
 def checkOrderPrice(orderData):
     if orderData.price is None:
         raise ValueError("Missing 'price' field for limit order type.")
 
 
 def checkStopOrderDatas(orderData, futures=False):
     if futures:
-        if "stop" not in orderData.extraParams.keys():
+        if "stop" not in orderData.extra_params.keys():
             raise ValueError(
                 "Specify 'stop' inside 'extraParams'. Either 'down' or 'up'."
             )
-        if "stopPriceType" not in orderData.extraParams.keys():
+        if "stopPriceType" not in orderData.extra_params.keys():
             raise ValueError(
                 "Specify 'stopPriceType' inside 'extraParams'. Either 'TP', 'IP' or 'MP'."
             )
     else:
-        if orderData.extraParams is not None:
-            if "stop" not in orderData.extraParams.keys():
+        if orderData.extra_params is not None:
+            if "stop" not in orderData.extra_params.keys():
                 raise ValueError("Specify 'stop' in 'extraParams' for stop order.")
         else:
             raise ValueError("Specify 'stopPrice' in 'extraParams' for stop order.")
 
         if orderData.quantity is None:
             raise ValueError("Missing 'quantity' field for stop order type.")
 
 
 def checkOrderSize(orderData, futures=False):
     errorString = "Provide either 'quantity' or 'quoteOrderQty'."
     if futures:
-        if orderData.quantity is None and orderData.quoteQuantity is None:
-            if orderData.closePosition is None:
+        if orderData.quantity is None and orderData.quote_quantity is None:
+            if orderData.close_position is None:
                 raise ValueError(errorString)
-            if not orderData.closePosition:
+            if not orderData.close_position:
                 raise ValueError(errorString)
     else:
-        if orderData.quantity is None and orderData.quoteOrderQty is None:
+        if orderData.quantity is None and orderData.quote_order_qty is None:
             raise ValueError(errorString)
 
 
 def checkOrderType(orderData, futures=False):
     if futures:
         validTypes = ["limit", "market", "LIMIT", "MARKET", "Limit", "Market"]
     else:
@@ -175,17 +175,17 @@
             "MARKET",
             "STOP_MARKET",
             "Limit",
             "Market",
             "Stop_Market",
         ]
 
-    if orderData.orderType is None or orderData.orderType not in validTypes:
+    if orderData.order_type is None or orderData.order_type not in validTypes:
         raise ValueError("Missing 'type' field.")
-    orderData.orderType = orderData.orderType.lower()
+    orderData.order_type = orderData.order_type.lower()
 
 
 def checkOrderSymbol(orderData):
     if orderData.symbol is None:
         raise ValueError("Missing 'symbol' field.")
 
 
@@ -196,17 +196,17 @@
             "buy",
             "sell",
             "BUY",
             "SELL",
             "Buy",
             "Sell",
         ]:
-            if orderData.closePosition is None:
+            if orderData.close_position is None:
                 raise ValueError(errorString)
-            if not orderData.closePosition:
+            if not orderData.close_position:
                 raise ValueError(errorString)
         if orderData.side is not None:
             orderData.side = orderData.side.lower()
     else:
         if orderData.side is None or orderData.side not in [
             "buy",
             "sell",
@@ -252,25 +252,25 @@
         "1w": "1week",
     }
 
     noOrderIdsErrorString = (
         "Specify either 'orderId' or 'localOrderId' (only for active orders)"
     )
 
-    def __init__(self, credentials, sandbox=False, unifiedInOuts=True):
+    def __init__(self, credentials, sandbox=False, unified_in_outs=True):
         self.spotApiKey = credentials["spot"]["key"]
         self.spotSecret = credentials["spot"]["secret"]
         self.spotPassphrase = credentials["spot"]["passphrase"]
 
         self.futuresApiKey = credentials["futures"]["key"]
         self.futuresSecret = credentials["futures"]["secret"]
         self.futuresPassphrase = credentials["futures"]["passphrase"]
 
         self.sandbox = sandbox
-        self.unifiedInOuts = unifiedInOuts
+        self.unifiedInOuts = unified_in_outs
 
         self.unavailableErrorText = "This method is unavailable in KuCoin exchange"
 
         if sandbox:
             self.spotUser = User(
                 key=self.spotApiKey,
                 secret=self.spotSecret,
@@ -340,210 +340,215 @@
                 secret=self.futuresSecret,
                 passphrase=self.futuresPassphrase,
             )
 
     def get_balance(self, asset=None, futures=False):
         if futures:
             if asset is None:
-                return KuCoinHelpers.unifyGetBalanceFuturesOut(
+                return KuCoinHelpers.unify_get_balance_futures_out(
                     [
                         self.futuresUser.get_account_overview(),
                         self.futuresUser.get_account_overview(currency="USDT"),
                     ]
                 )
             else:
-                return KuCoinHelpers.unifyGetBalanceFuturesOut(
-                    self.futuresUser.get_account_overview(currency=asset), isSingle=True
+                return KuCoinHelpers.unify_get_balance_futures_out(
+                    self.futuresUser.get_account_overview(currency=asset),
+                    is_single=True,
                 )
 
         else:
             if asset is None:
-                return KuCoinHelpers.unifyGetBalanceSpotOut(
+                return KuCoinHelpers.unify_get_balance_spot_out(
                     self.spotUser.get_account_list(currency=asset)
                 )
             else:
-                return KuCoinHelpers.unifyGetBalanceSpotOut(
-                    self.spotUser.get_account_list(currency=asset), isSingle=True
+                return KuCoinHelpers.unify_get_balance_spot_out(
+                    self.spotUser.get_account_list(currency=asset), is_single=True
                 )
 
-    def symbolAccountTradeHistory(self, symbol, futures=False, fromId=None, limit=None):
+    def symbol_account_trade_history(
+        self, symbol, futures=False, from_id=None, limit=None
+    ):
         if futures:
-            return KuCoinHelpers.unifyTradeHistory(
+            return KuCoinHelpers.unify_trade_history(
                 self.futuresTrade.get_fills_details(symbol=symbol)["items"],
                 futures=True,
             )
         else:
-            return KuCoinHelpers.unifyTradeHistory(
+            return KuCoinHelpers.unify_trade_history(
                 self.spotTrade.get_fill_list(tradeType="TRADE")["items"]
             )
 
-    def testSpotOrder(self, orderData):
-        checkSpotOrderDataValid(orderData)
-        return orderData
+    def test_spot_order(self, order_data):
+        checkSpotOrderDataValid(order_data)
+        return order_data
 
-    def makeSpotOrder(self, orderData):
-        params = KuCoinHelpers.getSpotOrderAsDict(orderData)
+    def make_spot_order(self, order_data):
+        params = KuCoinHelpers.get_spot_order_as_dict(order_data)
         response = None
 
         if params["type"] == "market":
             response = self.spotTrade.create_market_order(**params)
         if params["type"] == "limit":
             response = self.spotTrade.create_limit_order(**params)
         if params["type"] == "stop_limit":
             params["type"] = "limit"
             response = self.spotTrade.create_limit_stop_order(**params)
         if params["type"] == "stop_market":
             params["type"] = "market"
             response = self.spotTrade.create_market_stop_order(**params)
 
-        return self.getOrder(
-            params["symbol"], orderId=response["orderId"], futures=False
+        return self.get_order(
+            params["symbol"], order_id=response["orderId"], futures=False
         )
 
-    def createAndTestSpotOrder(
+    def create_and_test_spot_order(
         self,
         symbol,
         side,
-        orderType,
+        order_type,
         quantity=None,
         price=None,
-        timeInForce=None,
-        stopPrice=None,
-        icebergQty=None,
-        newOrderRespType=None,
-        newClientOrderId=None,
-        extraParams=None,
+        time_in_force=None,
+        stop_price=None,
+        iceberg_qty=None,
+        new_order_resp_type=None,
+        new_client_order_id=None,
+        extra_params=None,
     ):
-        currOrder = DataHelpers.setSpotOrderData(
-            icebergQty,
-            newClientOrderId,
-            newOrderRespType,
-            orderType,
+        currOrder = DataHelpers.set_spot_order_data(
+            iceberg_qty,
+            new_client_order_id,
+            new_order_resp_type,
+            order_type,
             price,
             quantity,
             side,
-            stopPrice,
+            stop_price,
             symbol,
-            timeInForce,
-            extraParams,
+            time_in_force,
+            extra_params,
         )
 
-        self.testSpotOrder(currOrder)
+        self.test_spot_order(currOrder)
 
         return currOrder
 
-    def getSymbolOrders(
+    def get_symbol_orders(
         self,
         symbol,
         futures=False,
-        orderId=None,
-        startTime=None,
-        endTime=None,
+        order_id=None,
+        start_time=None,
+        end_time=None,
         limit=None,
     ):
         if futures:
             args = {}
-            if startTime is not None:
-                args["startAt"] = startTime
-            if endTime is not None:
-                args["endAt"] = endTime
+            if start_time is not None:
+                args["startAt"] = start_time
+            if end_time is not None:
+                args["endAt"] = end_time
             args["symbol"] = symbol
             orderList = self.futuresTrade.get_order_list(**args)["items"]
-            return KuCoinHelpers.unifyGetSymbolOrders(orderList, futures=True)
+            return KuCoinHelpers.unify_get_symbol_orders(orderList, futures=True)
         else:
             args = {}
-            if startTime is not None:
-                args["startAt"] = startTime
-            if endTime is not None:
-                args["endAt"] = endTime
+            if start_time is not None:
+                args["startAt"] = start_time
+            if end_time is not None:
+                args["endAt"] = end_time
             args["symbol"] = symbol
             orderList = self.spotTrade.get_order_list(**args)["items"]
-            return KuCoinHelpers.unifyGetSymbolOrders(orderList)
+            return KuCoinHelpers.unify_get_symbol_orders(orderList)
 
-    def getOpenOrders(self, symbol, futures=False):
+    def get_open_orders(self, symbol, futures=False):
         args = {"symbol": symbol, "status": "active"}
         if futures:
-            lotSize = self.getSymbolMinTrade(symbol=symbol, futures=True)[
+            lotSize = self.get_symbol_min_trade(symbol=symbol, futures=True)[
                 "precisionStep"
             ]
             orderList = self.futuresTrade.get_order_list(**args)["items"]
-            return KuCoinHelpers.unifyGetSymbolOrders(
-                orderList, futures=True, lotSize=lotSize
+            return KuCoinHelpers.unify_get_symbol_orders(
+                orderList, futures=True, lot_size=lotSize
             )
         else:
             orderList = self.spotTrade.get_order_list(**args)["items"]
-            return KuCoinHelpers.unifyGetSymbolOrders(orderList)
+            return KuCoinHelpers.unify_get_symbol_orders(orderList)
 
-    def cancelAllSymbolOpenOrders(self, symbol, futures=False):
+    def cancel_all_symbol_open_orders(self, symbol, futures=False):
         if futures:
             result = self.futuresTrade.cancel_all_limit_order(symbol)[
                 "cancelledOrderIds"
             ]
             result.append(
                 self.futuresTrade.cancel_all_stop_order(symbol)["cancelledOrderIds"]
             )
             return result
         else:
             args = {"symbol": symbol}
             result = self.spotTrade.cancel_all_orders(**args)
             return result["cancelledOrderIds"]
 
-    def cancelOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
+    def cancel_order(self, symbol, order_id=None, local_order_id=None, futures=False):
         if futures:
-            if orderId is not None:
-                cancelledOrderId = self.futuresTrade.cancel_order(orderId)[
+            if order_id is not None:
+                cancelledOrderId = self.futuresTrade.cancel_order(order_id)[
                     "cancelledOrderIds"
                 ][0]
-            elif localOrderId is not None:
-                orderData = self.getOrder(
-                    symbol=symbol, localOrderId=localOrderId, futures=True
+            elif local_order_id is not None:
+                orderData = self.get_order(
+                    symbol=symbol, local_order_id=local_order_id, futures=True
                 )
                 cancelledOrderId = self.futuresTrade.cancel_order(
                     orderId=orderData["orderId"]
                 )["cancelledOrderIds"][0]
             else:
                 raise ValueError(self.noOrderIdsErrorString)
-            return self.getOrder(symbol, orderId=cancelledOrderId, futures=True)
+            return self.get_order(symbol, order_id=cancelledOrderId, futures=True)
         else:
-            if orderId is not None:
-                cancelledOrderId = self.spotTrade.cancel_order(orderId)[
+            if order_id is not None:
+                cancelledOrderId = self.spotTrade.cancel_order(order_id)[
                     "cancelledOrderIds"
                 ][0]
-            elif localOrderId is not None:
-                cancelledOrderId = self.spotTrade.cancel_client_order(localOrderId)[
+            elif local_order_id is not None:
+                cancelledOrderId = self.spotTrade.cancel_client_order(local_order_id)[
                     "cancelledOrderId"
                 ]
             else:
                 raise ValueError(self.noOrderIdsErrorString)
-            return self.getOrder(symbol, orderId=cancelledOrderId, futures=False)
+            return self.get_order(symbol, order_id=cancelledOrderId, futures=False)
 
-    def getOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
+    def get_order(self, symbol, order_id=None, local_order_id=None, futures=False):
         if futures:
-            if orderId is not None:
-                orderData = self.futuresTrade.get_order_details(orderId)
-            elif localOrderId is not None:
-                orderData = self.futuresTrade.get_client_order_details(localOrderId)
+            if order_id is not None:
+                orderData = self.futuresTrade.get_order_details(order_id)
+            elif local_order_id is not None:
+                orderData = self.futuresTrade.get_client_order_details(local_order_id)
             else:
                 raise ValueError(self.noOrderIdsErrorString)
 
-            lotSize = self.getSymbolMinTrade(symbol=symbol, futures=True)[
+            lotSize = self.get_symbol_min_trade(symbol=symbol, futures=True)[
                 "precisionStep"
             ]
-            return KuCoinHelpers.unifyGetOrder(orderData, futures=True, lotSize=lotSize)
+            return KuCoinHelpers.unify_get_order(
+                orderData, futures=True, lot_size=lotSize
+            )
         else:
-            if orderId is not None:
-                orderData = self.spotTrade.get_order_details(orderId)
-            elif localOrderId is not None:
-                orderData = self.spotTrade.get_client_order_details(localOrderId)
+            if order_id is not None:
+                orderData = self.spotTrade.get_order_details(order_id)
+            elif local_order_id is not None:
+                orderData = self.spotTrade.get_client_order_details(local_order_id)
             else:
                 raise ValueError(self.noOrderIdsErrorString)
 
-            return KuCoinHelpers.unifyGetOrder(orderData)
+            return KuCoinHelpers.unify_get_order(orderData)
 
-    def getTradingFees(self, symbol=None, futures=False):
+    def get_trading_fees(self, symbol=None, futures=False):
         if futures:
             if symbol is None:
                 raise ValueError("Must specify futures contract symbol name.")
             contractInfo = self.futuresMarket.get_contract_detail(symbol=symbol)
             return {
                 "symbol": contractInfo["symbol"],
                 "takerCommission": contractInfo["takerFeeRate"],
@@ -557,80 +562,80 @@
 
                 return {
                     "symbol": feeData["symbol"],
                     "takerCommission": feeData["takerFeeRate"],
                     "makerCommission": feeData["makerFeeRate"],
                 }
 
-    def getSymbolTickerPrice(self, symbol, futures=False):
+    def get_symbol_ticker_price(self, symbol, futures=False):
         if futures:
             return float(self.futuresMarket.get_ticker(symbol=symbol)["price"])
         else:
             return float(self.spotMarket.get_ticker(symbol=symbol)["price"])
 
-    def getSymbolKlines(
+    def get_symbol_klines(
         self,
         symbol,
         interval,
-        startTime=None,
-        endTime=None,
+        start_time=None,
+        end_time=None,
         limit=500,
         futures=False,
         blvtnav=False,
-        convertDateTime=False,
-        doClean=False,
-        toCleanDataframe=False,
+        convert_date_time=False,
+        do_clean=False,
+        to_clean_dataframe=False,
     ):
         if interval not in KuCoinExchange.timeIntervals:
             if interval in KuCoinExchange.timeIntervalTranslate.keys():
                 timeInterval = KuCoinExchange.timeIntervalTranslate[interval]
             else:
                 raise ValueError("Time interval is not valid.")
         else:
             timeInterval = interval
 
-        if startTime is not None and not isinstance(startTime, int):
-            startTime = int(
-                datetime.timestamp(datetime.strptime(startTime, "%Y-%m-%d %H:%M:%S"))
-            )
-        if endTime is not None and not isinstance(endTime, int):
-            endTime = int(
-                datetime.timestamp(datetime.strptime(endTime, "%Y-%m-%d %H:%M:%S"))
+        if start_time is not None and not isinstance(start_time, int):
+            start_time = int(
+                datetime.timestamp(datetime.strptime(start_time, "%Y-%m-%d %H:%M:%S"))
+            )
+        if end_time is not None and not isinstance(end_time, int):
+            end_time = int(
+                datetime.timestamp(datetime.strptime(end_time, "%Y-%m-%d %H:%M:%S"))
             )
 
         if futures:
             data = self._getFuturesSymbolKlines(
-                endTime, timeInterval, limit, startTime, symbol
+                end_time, timeInterval, limit, start_time, symbol
             )
         else:
-            if startTime is not None:
-                startTime = int(str(startTime)[:-3])
+            if start_time is not None:
+                start_time = int(str(start_time)[:-3])
 
-            if endTime is not None:
-                endTime = int(str(endTime)[:-3])
+            if end_time is not None:
+                end_time = int(str(end_time)[:-3])
 
             data = self._getSpotSymbolKlines(
-                endTime, timeInterval, limit, startTime, symbol
+                end_time, timeInterval, limit, start_time, symbol
             )
 
-        if convertDateTime or toCleanDataframe:
+        if convert_date_time or to_clean_dataframe:
             if futures:
                 for datum in data:
                     datum.append(datum[-1])
                     datum[-1] = datetime.fromtimestamp((float(datum[0]) - 1) / 1000)
                     datum[0] = datetime.fromtimestamp(float(datum[0]) / 1000)
                     datum.append(None)
             else:
                 for datum in data:
                     datum.append(datum[-1])
                     datum[-2] = datetime.fromtimestamp(float(datum[0]) - 1)
                     datum[0] = datetime.fromtimestamp(float(datum[0]))
 
-        if doClean or toCleanDataframe:
-            if toCleanDataframe:
+        if do_clean or to_clean_dataframe:
+            if to_clean_dataframe:
                 if futures:
                     cleanDataFrame = pd.DataFrame(
                         data,
                         columns=[
                             "date",
                             "open",
                             "high",
@@ -835,49 +840,49 @@
         elif timeInterval == "12hour":
             return 12 * 3600
         elif timeInterval == "1day":
             return 24 * 3600
         elif timeInterval == "1week":
             return 7 * 24 * 3600
 
-    def getExchangeTime(self, futures=False):
+    def get_exchange_time(self, futures=False):
         if futures:
             return self.futuresMarket.get_server_timestamp()
         else:
             return self.spotMarket.get_server_timestamp()
 
-    def getSymbol24hTicker(self, symbol):
+    def get_symbol_24h_ticker(self, symbol):
         return self.spotMarket.get_24h_stats(symbol)
 
-    def testFuturesOrder(self, futuresOrderData):
-        checkFuturesOrderDataValid(futuresOrderData)
+    def test_futures_order(self, futures_order_data):
+        checkFuturesOrderDataValid(futures_order_data)
 
-    def makeFuturesOrder(self, futuresOrderData):
-        if futuresOrderData.quantity is None:
-            if futuresOrderData.quoteQuantity is not None:
-                lotSize = self.getSymbolMinTrade(
-                    symbol=futuresOrderData.symbol, futures=True
+    def make_futures_order(self, futures_order_data):
+        if futures_order_data.quantity is None:
+            if futures_order_data.quote_quantity is not None:
+                lotSize = self.get_symbol_min_trade(
+                    symbol=futures_order_data.symbol, futures=True
                 )["precisionStep"]
-                if futuresOrderData.price is None:
-                    currPrice = self.getSymbolTickerPrice(
-                        futuresOrderData.symbol, futures=True
+                if futures_order_data.price is None:
+                    currPrice = self.get_symbol_ticker_price(
+                        futures_order_data.symbol, futures=True
                     )
-                    futuresOrderData.quantity = int(
-                        round(futuresOrderData.quoteQuantity / currPrice / lotSize)
+                    futures_order_data.quantity = int(
+                        round(futures_order_data.quote_quantity / currPrice / lotSize)
                     )
                 else:
-                    futuresOrderData.quantity = int(
+                    futures_order_data.quantity = int(
                         round(
-                            futuresOrderData.quoteQuantity
-                            / futuresOrderData.price
+                            futures_order_data.quote_quantity
+                            / futures_order_data.price
                             / lotSize
                         )
                     )
 
-        params = KuCoinHelpers.getFuturesOrderAsDict(futuresOrderData)
+        params = KuCoinHelpers.get_futures_order_as_dict(futures_order_data)
 
         symbol = params["symbol"]
         del params["symbol"]
 
         side = params["side"]
         del params["side"]
 
@@ -898,204 +903,206 @@
             del params["price"]
 
             result = self.futuresTrade.create_limit_order(
                 symbol, side, leverage, size, price, **params
             )
         else:
             result = None
-        return self.getOrder(symbol, orderId=result["orderId"], futures=True)
+        return self.get_order(symbol, order_id=result["orderId"], futures=True)
 
-    def createAndTestFuturesOrder(
+    def create_and_test_futures_order(
         self,
         symbol,
         side,
-        orderType,
-        positionSide=None,
-        timeInForce=None,
+        order_type,
+        position_side=None,
+        time_in_force=None,
         quantity=None,
-        reduceOnly=None,
+        reduce_only=None,
         price=None,
-        newClientOrderId=None,
-        stopPrice=None,
-        closePosition=None,
-        activationPrice=None,
-        callbackRate=None,
-        workingType=None,
-        priceProtect=None,
-        newOrderRespType=None,
-        extraParams=None,
+        new_client_order_id=None,
+        stop_price=None,
+        close_position=None,
+        activation_price=None,
+        callback_rate=None,
+        working_type=None,
+        price_protect=None,
+        new_order_resp_type=None,
+        extra_params=None,
         quoteQuantity=None,
     ):
-        currOrder = DataHelpers.setFuturesOrderData(
-            activationPrice,
-            callbackRate,
-            closePosition,
-            extraParams,
-            newClientOrderId,
-            newOrderRespType,
-            orderType,
-            positionSide,
+        currOrder = DataHelpers.set_futures_order_data(
+            activation_price,
+            callback_rate,
+            close_position,
+            extra_params,
+            new_client_order_id,
+            new_order_resp_type,
+            order_type,
+            position_side,
             price,
-            priceProtect,
+            price_protect,
             quantity,
-            reduceOnly,
+            reduce_only,
             side,
-            stopPrice,
+            stop_price,
             symbol,
-            timeInForce,
-            workingType,
+            time_in_force,
+            working_type,
             quoteQuantity,
         )
 
-        lotSize = self.getSymbolMinTrade(symbol=symbol, futures=True)["precisionStep"]
+        lotSize = self.get_symbol_min_trade(symbol=symbol, futures=True)[
+            "precisionStep"
+        ]
         if currOrder.quantity is not None:
             currOrder.quantity /= lotSize
 
-        self.testFuturesOrder(currOrder)
+        self.test_futures_order(currOrder)
 
         return currOrder
 
-    def makeBatchFuturesOrder(self, futuresOrderDatas):
+    def make_batch_futures_order(self, futures_order_datas):
         raise NotImplementedError(self.unavailableErrorText)
 
-    def changeInitialLeverage(self, symbol, leverage):
+    def change_initial_leverage(self, symbol, leverage):
         raise NotImplementedError(self.unavailableErrorText)
 
-    def changeMarginType(self, symbol, marginType, params=None):
-        if marginType.upper() == "CROSSED":
+    def change_margin_type(self, symbol, margin_type, params=None):
+        if margin_type.upper() == "CROSSED":
             autoAdd = True
-        elif marginType.upper() == "ISOLATED":
+        elif margin_type.upper() == "ISOLATED":
             autoAdd = False
         else:
             raise ValueError(
                 "Invalid value specified for 'marginType'. Must be either 'ISOLATED' or 'CROSSED'."
             )
         return self.futuresTrade.modify_auto_deposit_margin(symbol, autoAdd)["data"]
 
-    def changePositionMargin(self, symbol, amount):
+    def change_position_margin(self, symbol, amount):
         newPosition = self.futuresTrade.add_margin_manually(
             symbol=symbol, margin=amount, bizNo=str(time.time())
         )
 
         return True
 
-    def getPosition(self):
+    def get_position(self):
         return self.futuresTrade.get_all_position()
 
-    def spotBestBidAsks(self, symbol):
+    def spot_best_bid_asks(self, symbol):
         tickerData = self.spotMarket.get_ticker(symbol)
-        return KuCoinHelpers.unifyGetBestBidAsks(tickerData, symbol)
+        return KuCoinHelpers.unify_get_best_bid_asks(tickerData, symbol)
 
-    def getSymbolOrderBook(self, symbol, limit=None, futures=False):
+    def get_symbol_order_book(self, symbol, limit=None, futures=False):
         if futures:
             orderBook = self.futuresMarket.l2_order_book(symbol)
             return orderBook
         else:
             orderBook = self.spotMarket.get_aggregated_order(symbol)
             return orderBook
 
-    def getSymbolRecentTrades(self, symbol, limit=None, futures=False):
+    def get_symbol_recent_trades(self, symbol, limit=None, futures=False):
         if futures:
             tradeHistory = self.futuresMarket.get_trade_history(symbol=symbol)
             return pd.DataFrame(
-                KuCoinHelpers.unifyRecentTrades(tradeHistory, futures=True)
+                KuCoinHelpers.unify_recent_trades(tradeHistory, futures=True)
             )
         else:
             tradeHistory = self.spotMarket.get_trade_histories(symbol=symbol)
-            return pd.DataFrame(KuCoinHelpers.unifyRecentTrades(tradeHistory))
+            return pd.DataFrame(KuCoinHelpers.unify_recent_trades(tradeHistory))
 
-    def getPositionInfo(self, symbol=None):
+    def get_position_info(self, symbol=None):
         if symbol is None:
             positionInfos = self.futuresTrade.get_all_position()
-            return KuCoinHelpers.unifyGetPositionInfos(positionInfos)
+            return KuCoinHelpers.unify_get_position_infos(positionInfos)
         else:
             positionInfo = self.futuresTrade.get_position_details(symbol=symbol)
-            return [KuCoinHelpers.unifyGetPositionInfo(positionInfo)]
+            return [KuCoinHelpers.unify_get_position_info(positionInfo)]
 
-    def getSymbolMinTrade(self, symbol, futures=False):
+    def get_symbol_min_trade(self, symbol, futures=False):
         if futures:
             contractInfos = self.futuresMarket.get_contract_detail(symbol)
-            return KuCoinHelpers.unifyMinTrade(contractInfos, futures=True)
+            return KuCoinHelpers.unify_min_trade(contractInfos, futures=True)
         else:
             symbolInfoList = self.spotMarket.get_symbol_list()
 
             symbolInfo = None
             for info in symbolInfoList:
                 if info["symbol"] == symbol:
                     symbolInfo = info
-            return KuCoinHelpers.unifyMinTrade(symbolInfo)
+            return KuCoinHelpers.unify_min_trade(symbolInfo)
 
-    def makeSlTpLimitFuturesOrder(
+    def make_sl_tp_limit_futures_order(
         self,
         symbol,
-        orderSide,
+        order_side,
         quantity=None,
-        quoteQuantity=None,
-        enterPrice=None,
-        takeProfit=None,
-        stopLoss=None,
+        quote_quantity=None,
+        enter_price=None,
+        take_profit=None,
+        stop_loss=None,
         leverage=None,
-        marginType=None,
+        margin_type=None,
     ):
-        symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
+        symbolInfo = self.get_symbol_min_trade(symbol=symbol, futures=True)
 
         if quantity is None:
-            if quoteQuantity is None:
+            if quote_quantity is None:
                 raise ValueError("Specify either quantity or quoteQuantity")
             quantity = (
-                int(quoteQuantity / enterPrice / symbolInfo["precisionStep"])
+                int(quote_quantity / enter_price / symbolInfo["precisionStep"])
                 * symbolInfo["precisionStep"]
             )
 
         if quantity < symbolInfo["minQuantity"]:
             raise ValueError("Quantity is lower than minimum quantity allowed.")
 
-        mainOrder = self.createAndTestFuturesOrder(
+        mainOrder = self.create_and_test_futures_order(
             symbol,
-            orderSide.upper(),
+            order_side.upper(),
             "LIMIT",
             quantity=quantity,
-            price=enterPrice,
-            timeInForce="GTC",
-            extraParams={"leverage": leverage},
+            price=enter_price,
+            time_in_force="GTC",
+            extra_params={"leverage": leverage},
         )
 
-        tpSlSide = "sell" if orderSide.upper() == "BUY" else "buy"
+        tpSlSide = "sell" if order_side.upper() == "BUY" else "buy"
 
         slExtraParams = {
-            "stop": "down" if orderSide.upper() == "BUY" else "up",
+            "stop": "down" if order_side.upper() == "BUY" else "up",
             "stopPriceType": "TP",
         }
-        stopLossOrder = self.createAndTestFuturesOrder(
+        stopLossOrder = self.create_and_test_futures_order(
             symbol=symbol,
             side=tpSlSide,
-            orderType="MARKET",
-            stopPrice=stopLoss,
-            closePosition=True,
-            timeInForce="GTC",
-            extraParams=slExtraParams,
+            order_type="MARKET",
+            stop_price=stop_loss,
+            close_position=True,
+            time_in_force="GTC",
+            extra_params=slExtraParams,
         )
 
         tpExtraParams = {
-            "stop": "up" if orderSide.upper() == "BUY" else "down",
+            "stop": "up" if order_side.upper() == "BUY" else "down",
             "stopPriceType": "TP",
         }
-        takeProfitOrder = self.createAndTestFuturesOrder(
+        takeProfitOrder = self.create_and_test_futures_order(
             symbol=symbol,
             side=tpSlSide,
-            orderType="MARKET",
-            stopPrice=takeProfit,
-            closePosition=True,
-            timeInForce="GTC",
-            extraParams=tpExtraParams,
+            order_type="MARKET",
+            stop_price=take_profit,
+            close_position=True,
+            time_in_force="GTC",
+            extra_params=tpExtraParams,
         )
 
-        mainOrderRes = self.makeFuturesOrder(mainOrder)
-        slOrderRes = self.makeFuturesOrder(stopLossOrder)
-        tpOrderRes = self.makeFuturesOrder(takeProfitOrder)
+        mainOrderRes = self.make_futures_order(mainOrder)
+        slOrderRes = self.make_futures_order(stopLossOrder)
+        tpOrderRes = self.make_futures_order(takeProfitOrder)
 
         orderIds = {
             "mainOrder": mainOrderRes["orderId"],
             "stopLoss": slOrderRes["orderId"],
             "takeProfit": tpOrderRes["orderId"],
         }
 
@@ -1108,16 +1115,16 @@
         quantity=None,
         quoteQuantity=None,
         takeProfit=None,
         stopLoss=None,
         leverage=None,
         marginType=None,
     ):
-        symbolInfo = self.getSymbolMinTrade(symbol=symbol, futures=True)
-        marketPrice = self.getSymbolTickerPrice(symbol=symbol, futures=True)
+        symbolInfo = self.get_symbol_min_trade(symbol=symbol, futures=True)
+        marketPrice = self.get_symbol_ticker_price(symbol=symbol, futures=True)
 
         if leverage is None:
             raise ValueError("Must specify 'leverage' parameter for KuCoin orders.")
 
         if quantity is None:
             if quoteQuantity is None:
                 raise ValueError("Specify either quantity or quoteQuantity")
@@ -1125,55 +1132,55 @@
                 int(quoteQuantity / marketPrice / symbolInfo["precisionStep"])
                 * symbolInfo["precisionStep"]
             )
 
         if quantity < symbolInfo["minQuantity"]:
             raise ValueError("Quantity is lower than minimum quantity allowed.")
 
-        mainOrder = self.createAndTestFuturesOrder(
+        mainOrder = self.create_and_test_futures_order(
             symbol,
             orderSide.upper(),
             "MARKET",
             quantity=quantity,
-            extraParams={"leverage": leverage},
+            extra_params={"leverage": leverage},
         )
 
         tpSlSide = "sell" if orderSide.upper() == "BUY" else "buy"
 
         slExtraParams = {
             "stop": "down" if orderSide.upper() == "BUY" else "up",
             "stopPriceType": "TP",
         }
-        stopLossOrder = self.createAndTestFuturesOrder(
+        stopLossOrder = self.create_and_test_futures_order(
             symbol=symbol,
             side=tpSlSide,
-            orderType="MARKET",
-            stopPrice=stopLoss,
-            closePosition=True,
-            timeInForce="GTC",
-            extraParams=slExtraParams,
+            order_type="MARKET",
+            stop_price=stopLoss,
+            close_position=True,
+            time_in_force="GTC",
+            extra_params=slExtraParams,
         )
 
         tpExtraParams = {
             "stop": "up" if orderSide.upper() == "BUY" else "down",
             "stopPriceType": "TP",
         }
-        takeProfitOrder = self.createAndTestFuturesOrder(
+        takeProfitOrder = self.create_and_test_futures_order(
             symbol=symbol,
             side=tpSlSide,
-            orderType="MARKET",
-            stopPrice=takeProfit,
-            closePosition=True,
-            timeInForce="GTC",
-            extraParams=tpExtraParams,
+            order_type="MARKET",
+            stop_price=takeProfit,
+            close_position=True,
+            time_in_force="GTC",
+            extra_params=tpExtraParams,
         )
 
-        mainOrderRes = self.makeFuturesOrder(mainOrder)
-        slOrderRes = self.makeFuturesOrder(stopLossOrder)
-        tpOrderRes = self.makeFuturesOrder(takeProfitOrder)
+        mainOrderRes = self.make_futures_order(mainOrder)
+        slOrderRes = self.make_futures_order(stopLossOrder)
+        tpOrderRes = self.make_futures_order(takeProfitOrder)
 
         orderIds = {
             "mainOrder": mainOrderRes["orderId"],
             "stopLoss": slOrderRes["orderId"],
             "takeProfit": tpOrderRes["orderId"],
         }
 
@@ -1235,15 +1242,18 @@
             "endAt": endTime,
             "type": incomeType,
             "maxCount": limit,
             "currency": currency,
         }
         args = {k: v for k, v in args.items() if v is not None}
 
-        return KuCoinHelpers.unifyGetIncome(
+        return KuCoinHelpers.unify_get_income(
             self.futuresUser.get_transaction_history(**args)["dataList"]
         )
 
-    def getLongShortRatios(
-        self, symbol, period, limit=None, startTime=None, endTime=None
+    def get_long_short_ratios(
+        self, symbol, period, limit=None, start_time=None, end_time=None
     ):
         pass
+
+    def get_deposit_address(self, coin, network=None):
+        pass
```

### Comparing `TradeGate-0.3.8/TradeGates/TradeGate.egg-info/PKG-INFO` & `TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TradeGate
-Version: 0.3.8
+Version: 0.3.8.1
 Summary: A Trading Gateway
 Author: Rustin Soraki
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -80,15 +80,15 @@
 import json
 
 with open('/path/to/config/file.json') as f:
     config = json.load(f)
 
 gate = TradeGate(config['Binance'], sandbox=True)
 
-print(gate.getSymbolTickerPrice('BTCUSDT'))
+print(gate.get_symbol_ticker_price('BTCUSDT'))
 ```
 
 ## Current Supported Exchanges
 
 - Binance
 - ByBit
 - KuCoin
```

### Comparing `TradeGate-0.3.8/TradeGates/TradeGate.egg-info/SOURCES.txt` & `TradeGate-0.3.8.1/TradeGates/TradeGate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/TradeGate.py` & `TradeGate-0.3.8.1/TradeGates/TradeGate.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         stopPrice=None,
         icebergQty=None,
         newOrderRespType=None,
         newClientOrderId=None,
         extraParams=None,
     ):
         """ Create a OrderData object and test the given parameters for validity. The object returned is then used \
-        to send an order to the exchange by :func:`makeSpotOrder() <TradeGate.TradeGate.makeSpotOrder>`
+        to send an order to the exchange by :func:`make_spot_order() <TradeGate.TradeGate.make_spot_order>`
 
         :param symbol: Symbol of the order
         :type symbol: str
         :param side: Side of the order. Either '**BUY**' or '**SELL**'
         :type side: str
         :param orderType: Type of the order. can be '**MARKET**', '**LIMIT**' or others (Check exchange's API documentation)
         :type orderType: str
@@ -112,15 +112,15 @@
         :param newOrderRespType: Only for Binance. Response of the order, either '**ACK**' or '**RESULT**'.
         :type newOrderRespType: str , optional
         :param newClientOrderId: Custom string to identify your order for yourself.
         :type newClientOrderId: str , optional
         :param extraParams: Extra parameters for other exchanges than Binance.
         :type extraParams: dict , optional
         :return: An orderData object of the created order, ready to be submitted using \
-        :func:`makeSpotOrder() <TradeGate.TradeGate.makeSpotOrder>`
+        :func:`make_spot_order() <TradeGate.TradeGate.make_spot_order>`
         :rtype: OrderData
 
         :Notes:
 
             * Input parameters are based on Binance API. We map the appropriate parameters from input to the exchange \
             requirements, but other parameters must be inside the '**extraParams**' dictionary.
             * Some parameters have values that are only valid for some exchanges. See each exchange's documentation for\
@@ -141,15 +141,15 @@
                 only if '**timeInForce**' value is **GTT**
                 * You can send '**postOnly**', '**hidden**', '**iceberg**' (bool) and '**visibleSize**' parameters inside \
                 '**extraParams**'.
                 * Valid values for the '**timeInForce**' variable: **GTC** (Good Till Cancel), **IOC** \
                 (Immediate Or Cancel), **GTT** (Good Till Time) and **FOK** (Fill Or Kill)
 
         """
-        return self.exchange.createAndTestSpotOrder(
+        return self.exchange.create_and_test_spot_order(
             symbol,
             side,
             orderType,
             quantity,
             price,
             timeInForce,
             stopPrice,
@@ -158,15 +158,15 @@
             newClientOrderId,
             extraParams,
         )
 
     def makeSpotOrder(self, orderData):
         """Make a spot order
 
-        :param orderData: OrderData created using :func:`makeSpotOrder() <TradeGate.TradeGate.makeSpotOrder>`
+        :param orderData: OrderData created using :func:`make_spot_order() <TradeGate.TradeGate.make_spot_order>`
         :type orderData: OrderData
         :return: submitted order information
         :rtype: dict
         :Output:
 
             .. code-block:: python
 
@@ -184,15 +184,15 @@
                     'timeInForce': 'GTC',
                     'type': 'LIMIT',
                     'side': 'BUY',
                     'fills': []
                 }
 
         """
-        return self.exchange.makeSpotOrder(orderData)
+        return self.exchange.make_spot_order(orderData)
 
     def getSymbolOrders(
         self,
         symbol,
         futures=False,
         orderId=None,
         startTime=None,
@@ -263,20 +263,20 @@
                 ]
 
         :Notes:
 
             * Specify the symbol for better output.
 
         """
-        return self.exchange.getSymbolOrders(
+        return self.exchange.get_symbol_orders(
             symbol=symbol,
             futures=futures,
-            orderId=orderId,
-            startTime=startTime,
-            endTime=endTime,
+            order_id=orderId,
+            start_time=startTime,
+            end_time=endTime,
             limit=limit,
         )
 
     def getOpenOrders(self, symbol, futures=False):
         """Get order datas of all open orders for a symbol
 
         :param symbol: The symbol
@@ -342,15 +342,15 @@
                             'priceRate': None,
                             'closePosition': False
                         }
                     }
                 ]
 
         """
-        return self.exchange.getOpenOrders(symbol, futures)
+        return self.exchange.get_open_orders(symbol, futures)
 
     def getOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
         """Get an order's data
 
         :param symbol: The Order's symbol
         :type symbol: str
         :param orderId: Exchange assigned '**orderId**' of the order.
@@ -393,15 +393,15 @@
                 }
 
         :Notes:
 
             * Must specify either '**orderId**' or '**localOrderId**'
 
         """
-        return self.exchange.getOrder(symbol, orderId, localOrderId, futures=futures)
+        return self.exchange.get_order(symbol, orderId, localOrderId, futures=futures)
 
     def cancelAllSymbolOpenOrders(self, symbol, futures=False):
         """Cancel all active orders of a symbol
 
         :param symbol: The symbol
         :type symbol: str
         :param futures: False for spot market and True for futures market, defaults to False
@@ -464,15 +464,15 @@
                             'priceRate': None,
                             'closePosition': False
                         }
                     }
                 ]
 
         """
-        return self.exchange.cancelAllSymbolOpenOrders(symbol, futures)
+        return self.exchange.cancel_all_symbol_open_orders(symbol, futures)
 
     def cancelOrder(self, symbol, orderId=None, localOrderId=None, futures=False):
         """Cancel an active order
 
         :param symbol: The Order's symbol
         :type symbol: str
         :param orderId: Exchange assigned '**orderId**' of the order.
@@ -515,15 +515,15 @@
                 }
 
         :Notes:
 
             * Must specify either '**orderId**' or '**localOrderId**'
 
         """
-        return self.exchange.cancelOrder(symbol, orderId, localOrderId, futures)
+        return self.exchange.cancel_order(symbol, orderId, localOrderId, futures)
 
     def getTradingFees(self, symbol=None, futures=None):
         """Get the fee structure of the exchange
 
         :param symbol: Trading fee for a specific symbol
         :type symbol: str, optional
         :param futures: False for spot market and True for futures market, defaults to False
@@ -540,15 +540,15 @@
                     'takerCommission': '0.001'
                 }
 
         :Notes:
 
             * Specify the symbol for better output.
         """
-        return self.exchange.getTradingFees(symbol=symbol, futures=futures)
+        return self.exchange.get_trading_fees(symbol=symbol, futures=futures)
 
     def getSymbolTickerPrice(self, symbol, futures=False):
         """Get the latest price of a symbol
 
         :param symbol: Symbol
         :type symbol: str
         :param futures: False for spot market and True for futures market, defaults to False
@@ -558,15 +558,15 @@
         :Output:
 
             .. code-block:: python
 
                 21275.84
 
         """
-        return self.exchange.getSymbolTickerPrice(symbol, futures)
+        return self.exchange.get_symbol_ticker_price(symbol, futures)
 
     def getSymbolKlines(
         self,
         symbol,
         interval,
         startTime=None,
         endTime=None,
@@ -655,15 +655,15 @@
             latest data.
             * '**limit**' parameter has a maximum value (usually 1000). if the given limit number is bigger than that, \
             only the maximum number will be fetched.
             * Desired columns are: **open** - **high** - **low** - **close** - **volume** - **closeDate** \
             - **tradesNum**
 
         """
-        return self.exchange.getSymbolKlines(
+        return self.exchange.get_symbol_klines(
             symbol,
             interval,
             startTime,
             endTime,
             limit,
             futures,
             blvtnav,
@@ -682,15 +682,15 @@
         :Output:
 
             .. code-block:: python
 
                 1656330049381
 
         """
-        return self.exchange.getExchangeTime(futures)
+        return self.exchange.get_exchange_time(futures)
 
     def createAndTestFuturesOrder(
         self,
         symbol,
         side,
         orderType,
         positionSide=None,
@@ -706,15 +706,15 @@
         workingType=None,
         priceProtect=None,
         newOrderRespType=None,
         extraParams=None,
         quoteQuantity=None,
     ):
         """ Create a FuturesOrderData object and test the given parameters for validity. The object returned is then used \
-        to send an order to the exchange by :func:`makeFuturesOrder() <TradeGate.TradeGate.makeFuturesOrder>`
+        to send an order to the exchange by :func:`make_futures_order() <TradeGate.TradeGate.make_futures_order>`
 
         :param symbol: Symbol of the order
         :type symbol: str
         :param side: Side of the order. Either '**BUY**' or '**SELL**'
         :type side: str
         :param orderType: Type of the order. can be '**MARKET**', '**LIMIT**' or others (Check exchange's API documentation)
         :type orderType: str
@@ -748,15 +748,15 @@
         :param newOrderRespType: Only for Binance. Response of the order, either '**ACK**' or '**RESULT**'.
         :type newOrderRespType: str , optional
         :param extraParams: Extra parameters for other exchanges than Binance.
         :type extraParams: dict , optional
         :param quoteQuantity: The amount of quote asset of the order.
         :type quoteQuantity: float , optional
         :return: An orderData object of the created order, ready to be submitted using \
-        :func:`makeFuturesOrder() <TradeGate.TradeGate.makeFuturesOrder>`
+        :func:`make_futures_order() <TradeGate.TradeGate.make_futures_order>`
         :rtype: OrderData
 
         :Notes:
 
             * Input parameters are based on Binance API. We map the appropriate parameters from input to the exchange \
             requirements, but other parameters must be inside the '**extraParams**' dictionary.
             * Preferably use '**quantity**' instead of '**quoteQuantity**'. Some exchanges don't accept this parameter \
@@ -764,16 +764,16 @@
             * Some parameters have values that are only valid for some exchanges. See each exchange's documentation for\
              these values.
             * ValueError exception is raised when wrong combination of parameters are sent. Check the exception's \
             message for guidance.
             * Do not send '**price**' with '**MARKET**' orders.
             * You must specify '**price**' for '**LIMIT**' orders.
             * Other than **ByBit**, \
-            use :func:`makeSlTpLimitFuturesOrder() <TradeGate.TradeGate.makeSlTpLimitFuturesOrder>` or \
-            :func:`makeSlTpMarketFuturesOrder() <TradeGate.TradeGate.makeSlTpMarketFuturesOrder>` to send take profit \
+            use :func:`make_sl_tp_limit_futures_order() <TradeGate.TradeGate.make_sl_tp_limit_futures_order>` or \
+            :func:`make_sl_tp_market_futures_order() <TradeGate.TradeGate.make_sl_tp_market_futures_order>` to send take profit \
             and stop loss.
             * if '**closePosition**' is used, do not specify '**quantity**' or '**quoteQuantity**'.
             * For **ByBit**:
 
                 * You can send take profit by specifying '**take_profit**' (price) and '**tp_trigger_by**' \
                 ('**LastPrice**', '**IndexPrice**' or '**MarkPrice**') in '**extraParams**'.
                 * You can send take profit by specifying '**stop_loss**' (price) and '**sl_trigger_by**' \
@@ -787,15 +787,15 @@
                 * You can send '**postOnly**', '**hidden**', '**iceberg**' and '**visibleSize**' parameters inside \
                 '**extraParams**'.
                 * There are two values for the '**timeInForce**' variable: '**GTC**' (Good Till Cancel) and '**IOC**' \
                 (Immediate Or Cancel)
 
 
         """
-        return self.exchange.createAndTestFuturesOrder(
+        return self.exchange.create_and_test_futures_order(
             symbol,
             side,
             orderType,
             positionSide,
             timeInForce,
             quantity,
             reduceOnly,
@@ -810,15 +810,15 @@
             newOrderRespType,
             extraParams,
         )
 
     def makeFuturesOrder(self, futuresOrderData):
         """Make a futures order
 
-        :param futuresOrderData: OrderData created using :func:`makeFuturesOrder() <TradeGate.TradeGate.makeFuturesOrder>`
+        :param futuresOrderData: OrderData created using :func:`make_futures_order() <TradeGate.TradeGate.make_futures_order>`
         :type futuresOrderData: OrderData
         :return: submitted order information
         :rtype: dict
         :Output:
 
             .. code-block:: python
 
@@ -847,20 +847,20 @@
                             'activatePrice': None,
                             'priceRate': None,
                             'closePosition': False
                         }
                     }
 
         """
-        return self.exchange.makeFuturesOrder(futuresOrderData)
+        return self.exchange.make_futures_order(futuresOrderData)
 
     def makeBatchFuturesOrder(self, batchOrders):
         """ Make multiple futures order with single request
 
-        :param batchOrders: list of OrderDatas created using :func:`makeFuturesOrder() <TradeGate.TradeGate.makeFuturesOrder>`
+        :param batchOrders: list of OrderDatas created using :func:`make_futures_order() <TradeGate.TradeGate.make_futures_order>`
         :type batchOrders: list(OrderData)
         :return: List of order information submitted
         :rtype: list(dict)
         :Output:
 
             .. code-block:: python
 
@@ -924,15 +924,15 @@
         :Notes:
 
             * Not available for **KuCoin** exchange.
             * The execution of orders in the batch are not dependent on each other, so be careful if orders depend on \
             one another.
 
         """
-        return self.exchange.makeBatchFuturesOrder(batchOrders)
+        return self.exchange.make_batch_futures_order(batchOrders)
 
     def changeInitialLeverage(self, symbol, leverage):
         """Change initial leverage for a symbol
 
         :param symbol: Futures symbol
         :type symbol: str
         :param leverage: Initial leverage number.
@@ -946,15 +946,15 @@
                 10
 
         :Notes:
 
             * Not available for **KuCoin** exchange. You must specify leverage when sending an order for this exchange.
 
         """
-        return self.exchange.changeInitialLeverage(symbol, leverage)
+        return self.exchange.change_initial_leverage(symbol, leverage)
 
     def changeMarginType(self, symbol, marginType, params=None):
         """ Change position margin of a symbol
 
         :param symbol: Symbol of the position
         :type symbol: str
         :param marginType: Type of the margin. Either '**ISOLATED**' or '**CROSSED**'.
@@ -972,15 +972,15 @@
         :Notes:
 
             * For **KuCoin**, '**CROSSED**' means enabling '**auto_add_margin**', and '**ISOLATED**' means disabling it.
             * For **ByBit**, you must specify '**buyLeverage**' and '**sellLeverage**' inside params. If switching from \
             '**CROSSED**' to '**ISOLATED**', theses two numbers must be equal.
 
         """
-        return self.exchange.changeMarginType(symbol, marginType, params)
+        return self.exchange.change_margin_type(symbol, marginType, params)
 
     def changePositionMargin(self, symbol, amount):
         """ Change position margin of a symbol
 
         :param symbol: Symbol of the position
         :type symbol: str
         :param amount: Amount to be added (or subtracted)
@@ -992,19 +992,19 @@
             .. code-block:: python
 
                 True
 
         :Notes:
 
             * The amount can be positive or negative for **Binance** exchange but it must be positive for other exchanges.
-            * Use :func:`changeMarginType() <TradeGate.TradeGate.changeMarginType>` to make current position available \
+            * Use :func:`change_margin_type() <TradeGate.TradeGate.change_margin_type>` to make current position available \
             for changing amount.
 
         """
-        return self.exchange.changePositionMargin(symbol, amount)
+        return self.exchange.change_position_margin(symbol, amount)
 
     def spotBestBidAsks(self, symbol=None):
         """Returns best bid and best ask price with their quantities
 
         :param symbol: Symbol name of the orders
         :type symbol: str
         :return: A dictionary with best bid and ask with their quantity
@@ -1018,15 +1018,15 @@
                     'bidPrice': '18125.7',
                     'bidQty': '0.00839998',
                     'askPrice': '18126',
                     'askQty': '0.00496777'
                 }
 
         """
-        return self.exchange.spotBestBidAsks(symbol)
+        return self.exchange.spot_best_bid_asks(symbol)
 
     def getSymbolOrderBook(self, symbol, limit=None, futures=False):
         """Returns list of current orders in the orderbook of the exchange
 
         :param symbol: Symbol name of the orders
         :type symbol: str
         :param limit: Maximum number of returned bids and asks
@@ -1054,15 +1054,15 @@
                         ['18010.70', '0.099'],
                         ['18010.90', '0.017'],
                         ['18011.20', '0.206']
                     ]
                 }
 
         """
-        return self.exchange.getSymbolOrderBook(symbol, limit, futures)
+        return self.exchange.get_symbol_order_book(symbol, limit, futures)
 
     def getSymbolRecentTrades(self, symbol, limit=None, futures=False):
         """Returns list of the recent trades for a symbol
 
         :param symbol: Symbol name of the trades
         :type symbol: str
         :param limit: Maximum number of returned trade datas
@@ -1077,15 +1077,15 @@
             * **price** (:py:class:`float`) - Price of the trade
             * **qty** (:py:class:`float`) - Amount of the base asset
             * **quoteQty** (:py:class:`float`) - Amount of the quote asset
             * **time** (:py:class:`int`) - Timestamp of the trade
             * **isBuyerMaker** (:py:class:`bool`) - If trade is buyer-maker
 
         """
-        return self.exchange.getSymbolRecentTrades(symbol, limit, futures)
+        return self.exchange.get_symbol_recent_trades(symbol, limit, futures)
 
     def symbolAccountTradeHistory(self, symbol, fromId=None, limit=None, futures=False):
         """Returns list of the trade history for user orders
 
         :param symbol: Symbol name of the trades
         :type symbol: str
         :param fromId: Only return trades from the specified id forward.
@@ -1135,16 +1135,16 @@
                 ]
 
         :Notes:
 
             * The **orderListId** returned parameter is either None or -1 if order was made with API.
             * The **isBestMatch** returned parameter is not reliable and not available on most of the exchanges.
         """
-        return self.exchange.symbolAccountTradeHistory(
-            symbol=symbol, futures=futures, fromId=fromId, limit=limit
+        return self.exchange.symbol_account_trade_history(
+            symbol=symbol, futures=futures, from_id=fromId, limit=limit
         )
 
     def makeSlTpLimitFuturesOrder(
         self,
         symbol,
         orderSide,
         enterPrice,
@@ -1196,15 +1196,15 @@
                 * KuCoin
 
             * The **marginType** is currently only valid for **Binance** exchange.
             * Be careful with the **takeProfit** and **stopLoss** prices, if they would trigger immidietly, there will be an error.
             * Use with a try catch block preferably.
 
         """
-        return self.exchange.makeSlTpLimitFuturesOrder(
+        return self.exchange.make_sl_tp_limit_futures_order(
             symbol,
             orderSide,
             quantity,
             quoteQuantity,
             enterPrice,
             takeProfit,
             stopLoss,
@@ -1261,15 +1261,15 @@
 
                 * KuCoin
             * The **marginType** is currently only valid for **Binance** exchange.
             * Be careful with the **takeProfit** and **stopLoss** prices, if they would trigger immidietly, there will be an error.
             * Use with a try catch block preferably.
 
         """
-        return self.exchange.makeSlTpMarketFuturesOrder(
+        return self.exchange.make_sl_tp_market_futures_order(
             symbol,
             orderSide,
             quantity,
             quoteQuantity,
             takeProfit,
             stopLoss,
             leverage,
@@ -1337,15 +1337,15 @@
                         'isolatedMargin': 0.0,
                         'positionSide': 'BOTH'
                     },
                     ...
                 ]
 
         """
-        return self.exchange.getPositionInfo(symbol)
+        return self.exchange.get_position_info(symbol)
 
     def getSymbolMinTrade(self, symbol, futures=False):
         """Returns information of valid minimum quantity, quote quantity and price precision.
 
         :param symbol: The symbol which the information is for.
         :type symbol: str
         :param futures: False for spot market and True for futures market, defaults to False
@@ -1375,15 +1375,15 @@
                     'stepPrice': 0.01,
                     'minQuantity': 1e-05,
                     'precisionStep': 1e-05,
                     'minQuoteQuantity': 0.19279200000000002
                 }
 
         """
-        return self.exchange.getSymbolMinTrade(symbol, futures)
+        return self.exchange.get_symbol_min_trade(symbol, futures)
 
     def getIncomeHistory(
         self, symbol, incomeType=None, startTime=None, endTime=None, limit=None
     ):
         """Returns list of changes to the account balance. (Only for futures accounts)
 
         :param symbol: The symbol which the incomes are related to
@@ -1425,15 +1425,15 @@
                         'time': 1655281638000
                     },
                     ...
                 ]
 
         """
 
-        return self.exchange.getIncomeHistory(
+        return self.exchange.get_income_history(
             symbol, incomeType, startTime, endTime, limit
         )
 
     def getSymbolList(self, futures=False):
         """Returns list of symbol names available for trade
 
         :param futures: False for spot market and True for futures market, defaults to False
@@ -1452,15 +1452,15 @@
                     'EOSUSDT',
                     'LTCUSDT',
                     'TRXUSDT',
                     ...
                 ]
 
         """
-        return self.exchange.getSymbolList(futures=futures)
+        return self.exchange.get_symbol_list(futures=futures)
 
     def getSymbol24hChanges(self, futures=False):
         """Returns all symbols 24-hour change percentages
 
         :param futures: False for spot market and True for futures market, defaults to False
         :type futures: bool , optional
         :return: Returns a list of tuples containing asset names and percentage of change in 24-hour
@@ -1479,15 +1479,15 @@
                     ('CTXCBTC', 20.551),
                     ('CTXCUSDT', 19.959),
                     ('CTXCBUSD', 19.776),
                     ...
                 ]
 
         """
-        return self.exchange.getSymbol24hChanges(futures=futures)
+        return self.exchange.get_symbol_24h_changes(futures=futures)
 
     def getLatestSymbolNames(self, numOfSymbols=None, futures=True):
         """Returns list of newly added symbols to the exchange. Currently, only working for futures market.
 
         :param numOfSymbols: Number of symbols returned, sorted for the newest to oldest.
         :type numOfSymbols: int, optional
         :param futures: False for spot market and True for futures market, defaults to False
@@ -1508,21 +1508,21 @@
                     ('GALABUSD', datetime.datetime(2022, 5, 25, 11, 30)),
                     ('TRXBUSD', datetime.datetime(2022, 5, 25, 11, 30)),
                     ('DODOBUSD', datetime.datetime(2022, 5, 24, 11, 30)),
                     ('ANCBUSD', datetime.datetime(2022, 5, 24, 11, 30))
                 ]
 
         """
-        return self.exchange.getLatestSymbolNames(
-            numOfSymbols=numOfSymbols, futures=futures
+        return self.exchange.get_latest_symbol_names(
+            num_of_symbols=numOfSymbols, futures=futures
         )
 
     def getLongShortRatios(
         self, symbol, period, limit=None, startTime=None, endTime=None
     ):
         print(self.exchange)
-        return self.exchange.getLongShortRatios(
+        return self.exchange.get_long_short_ratios(
             symbol, period, limit, startTime, endTime
         )
 
     def getDepositAddress(self, coin, network=None):
-        return self.exchange.getDepositAddress(coin, network)
+        return self.exchange.get_deposit_address(coin, network)
```

### Comparing `TradeGate-0.3.8/TradeGates/Utils/BinanceHelpers.py` & `TradeGate-0.3.8.1/TradeGates/Utils/BinanceHelpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,135 +2,148 @@
 from datetime import datetime
 
 import pandas as pd
 
 from Utils import DataHelpers
 
 
-def getSpotOrderAsDict(order: DataHelpers.OrderData):
+def get_spot_order_as_dict(order: DataHelpers.OrderData):
     if order.timestamp is None:
-        raise ValueError('Timestamp must be set')
+        raise ValueError("Timestamp must be set")
 
-    params = {'symbol': order.symbol, 'side': order.side, 'type': order.orderType, 'timestamp': order.timestamp}
+    params = {
+        "symbol": order.symbol,
+        "side": order.side,
+        "type": order.order_type,
+        "timestamp": order.timestamp,
+    }
 
-    if order.timeInForce is not None:
-        params['timeInForce'] = order.timeInForce
+    if order.time_in_force is not None:
+        params["timeInForce"] = order.time_in_force
 
     if order.quantity is not None:
-        params['quantity'] = order.quantity
+        params["quantity"] = order.quantity
 
-    if order.quoteOrderQty is not None:
-        params['quoteOrderQty'] = order.quoteOrderQty
+    if order.quote_order_qty is not None:
+        params["quoteOrderQty"] = order.quote_order_qty
 
     if order.price is not None:
-        params['price'] = order.price
+        params["price"] = order.price
 
-    if order.newOrderRespType is not None:
-        params['newOrderRespType'] = order.newOrderRespType
+    if order.new_order_resp_type is not None:
+        params["newOrderRespType"] = order.new_order_resp_type
 
-    if order.stopPrice is not None:
-        params['stopPrice'] = order.stopPrice
+    if order.stop_price is not None:
+        params["stopPrice"] = order.stop_price
 
-    if order.icebergQty is not None:
-        params['icebergQty'] = order.icebergQty
+    if order.iceberg_qty is not None:
+        params["icebergQty"] = order.iceberg_qty
 
-    if order.newClientOrderId is not None:
-        params['newClientOrderId'] = order.newClientOrderId
+    if order.new_client_order_id is not None:
+        params["newClientOrderId"] = order.new_client_order_id
 
-    if order.recvWindow is not None:
-        params['recvWindow'] = order.recvWindow
+    if order.recv_window is not None:
+        params["recvWindow"] = order.recv_window
 
     return params
 
 
-def getFuturesOrderAsDict(order: DataHelpers.FuturesOrderData, allStr=False):
-    params = {'symbol': order.symbol, 'side': order.side, 'ordertype': order.orderType}
+def get_futures_order_as_dict(order: DataHelpers.FuturesOrderData, all_str=False):
+    params = {"symbol": order.symbol, "side": order.side, "ordertype": order.orderType}
 
-    if order.positionSide is not None:
-        params['positionSide'] = order.positionSide
+    if order.position_side is not None:
+        params["positionSide"] = order.position_side
 
-    if order.timeInForce is not None:
-        params['timeInForce'] = order.timeInForce
+    if order.time_in_force is not None:
+        params["timeInForce"] = order.time_in_force
 
     if order.quantity is not None:
-        params['quantity'] = order.quantity
+        params["quantity"] = order.quantity
 
-    if order.reduceOnly is not None:
-        params['reduceOnly'] = order.reduceOnly
+    if order.reduce_only is not None:
+        params["reduceOnly"] = order.reduce_only
 
     if order.price is not None:
-        params['price'] = order.price
+        params["price"] = order.price
 
-    if order.newClientOrderId is not None:
-        params['newClientOrderId'] = order.newClientOrderId
+    if order.new_client_order_id is not None:
+        params["newClientOrderId"] = order.new_client_order_id
 
-    if order.stopPrice is not None:
-        params['stopPrice'] = order.stopPrice
+    if order.stop_price is not None:
+        params["stopPrice"] = order.stop_price
 
-    if order.closePosition is not None:
-        params['closePosition'] = order.closePosition
+    if order.close_position is not None:
+        params["closePosition"] = order.close_position
 
-    if order.activationPrice is not None:
-        params['activationPrice'] = order.activationPrice
+    if order.activation_price is not None:
+        params["activationPrice"] = order.activation_price
 
-    if order.callbackRate is not None:
-        params['callbackRate'] = order.callbackRate
+    if order.callback_rate is not None:
+        params["callbackRate"] = order.callback_rate
 
-    if order.workingType is not None:
-        params['workingType'] = order.workingType
+    if order.working_type is not None:
+        params["workingType"] = order.working_type
 
-    if order.priceProtect is not None:
-        params['priceProtect'] = order.priceProtect
+    if order.price_protect is not None:
+        params["priceProtect"] = order.price_protect
 
-    if order.newOrderRespType is not None:
-        params['newOrderRespType'] = order.newOrderRespType
+    if order.new_order_resp_type is not None:
+        params["newOrderRespType"] = order.new_order_resp_type
 
-    if allStr:
+    if all_str:
         for key, value in params.items():
             params[key] = str(value)
 
     return params
 
 
-def getKlinesDesiredOnlyCols(data, desiredIndexes):
-    finalDataArray = []
-    for datum in data:
-        finalDataArray.append([datum[index] for index in desiredIndexes])
-    return finalDataArray
+def get_klines_desired_only_cols(data, desired_indexes):
+    return [[datum[index] for index in desired_indexes] for datum in data]
 
 
-def klinesConvertToPandas(outArray):
-    df = pd.DataFrame(outArray,
-                      columns=['date', 'open', 'high', 'low', 'close', 'volume', 'closeDate', 'tradesNum'])
-    df.set_index('date', inplace=True)
+def klines_convert_to_pandas(out_array):
+    df = pd.DataFrame(
+        out_array,
+        columns=[
+            "date",
+            "open",
+            "high",
+            "low",
+            "close",
+            "volume",
+            "closeDate",
+            "tradesNum",
+        ],
+    )
+    df.set_index("date", inplace=True)
     return df
 
 
-def klinesConvertDate(data, timeColIdxs):
+def klines_convert_date(data, time_col_idxs):
     for datum in data:
-        for idx in timeColIdxs:
+        for idx in time_col_idxs:
             datum[idx] = datetime.fromtimestamp(float(datum[idx]) / 1000)
 
 
-def extractSymbolInfoFromFilters(symbolFilters, tickerPrice):
+def extract_symbol_info_from_filters(symbol_filters, ticker_price):
     params = {}
-    for symbolFilter in symbolFilters:
-        if symbolFilter['filterType'] == 'LOT_SIZE':
-            params['minQuantity'] = float(symbolFilter['minQty'])
-            params['precisionStep'] = float(symbolFilter['stepSize'])
-            params['minQuoteQuantity'] = tickerPrice * params['minQuantity']
+    for symbolFilter in symbol_filters:
+        if symbolFilter["filterType"] == "LOT_SIZE":
+            params["minQuantity"] = float(symbolFilter["minQty"])
+            params["precisionStep"] = float(symbolFilter["stepSize"])
+            params["minQuoteQuantity"] = ticker_price * params["minQuantity"]
 
-        if symbolFilter['filterType'] == 'PRICE_FILTER':
-            params['stepPrice'] = float(symbolFilter['tickSize'])
+        if symbolFilter["filterType"] == "PRICE_FILTER":
+            params["stepPrice"] = float(symbolFilter["tickSize"])
     return params
 
 
-def makeBatchOrderData(futuresOrderDatas):
-    batchOrders = []
-    for order in futuresOrderDatas:
-        orderAsDict = getFuturesOrderAsDict(order, allStr=True)
-        orderAsDict['type'] = orderAsDict.pop('ordertype')
+def make_batch_order_data(futures_order_datas):
+    batch_orders = []
+    for order in futures_order_datas:
+        order_as_dict = get_futures_order_as_dict(order, all_str=True)
+        order_as_dict["type"] = order_as_dict.pop("ordertype")
 
-        orderJSON = json.dumps(orderAsDict)
+        order_json = json.dumps(order_as_dict)
 
-        batchOrders.append(orderJSON)
-    return batchOrders
+        batch_orders.append(order_json)
+    return batch_orders
```

### Comparing `TradeGate-0.3.8/TradeGates/Watchers/futureOrderWatchers.py` & `TradeGate-0.3.8.1/TradeGates/Watchers/futureOrderWatchers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,81 @@
 import time
 
 
-def watchFuturesLimitTrigger(gate, symbol, orderId, doPutTpSl, cancelIfNotOpened, params):
+def watchFuturesLimitTrigger(
+    gate, symbol, orderId, doPutTpSl, cancelIfNotOpened, params
+):
     if doPutTpSl:
-        if 'tpSlOrderSide' not in params.keys() or 'stopLoss' not in params.keys() or 'takeProfit' not in params.keys():
-            raise ValueError('Must specify \'tpSlOrderSide\' and \'stopLoss\' and \'takeProfit\'')
+        if (
+            "tpSlOrderSide" not in params.keys()
+            or "stopLoss" not in params.keys()
+            or "takeProfit" not in params.keys()
+        ):
+            raise ValueError(
+                "Must specify 'tpSlOrderSide' and 'stopLoss' and 'takeProfit'"
+            )
 
     if cancelIfNotOpened:
-        if 'cancelDelaySec' not in params.keys():
-            raise ValueError('Must specify \'cancelDelaySec\'')
-        delayTimeSec = float(params['cancelDelaySec'])
+        if "cancelDelaySec" not in params.keys():
+            raise ValueError("Must specify 'cancelDelaySec'")
+        delayTimeSec = float(params["cancelDelaySec"])
         startDelayTime = time.time()
 
-    print('Watching order')
+    print("Watching order")
     while True:
         time.sleep(0.1)
-        order = gate.getOrder(symbol=symbol, orderId=orderId, futures=True)
+        order = gate.get_order(symbol=symbol, order_id=orderId, futures=True)
 
         if cancelIfNotOpened:
             if time.time() - startDelayTime > delayTimeSec:
-                gate.cancelOrder(symbol=symbol, orderId=orderId, futures=True)
+                gate.cancel_order(symbol=symbol, order_id=orderId, futures=True)
                 break
 
-        if order['status'] == 'NEW':
+        if order["status"] == "NEW":
             continue
-        elif order['status'] == 'FILLED':
+        elif order["status"] == "FILLED":
             if doPutTpSl:
-                orderSide = params['tpSlOrderSide']
-                stopLoss = params['stopLoss']
-                takeProfit = params['takeProfit']
-
-                stopLossOrder = gate.createAndTestFuturesOrder(symbol, orderSide, 'STOP_MARKET',
-                                                               stopPrice=str(stopLoss), closePosition=True,
-                                                               priceProtect=True, workingType='MARK_PRICE',
-                                                               timeInForce='GTC')
-
-                takeProfitOrder = gate.createAndTestFuturesOrder(symbol, orderSide, 'TAKE_PROFIT_MARKET',
-                                                                 stopPrice=str(takeProfit), closePosition=True,
-                                                                 priceProtect=True, workingType='MARK_PRICE',
-                                                                 timeInForce='GTC')
-                result = gate.makeBatchFuturesOrder([stopLossOrder, takeProfitOrder])
+                orderSide = params["tpSlOrderSide"]
+                stopLoss = params["stopLoss"]
+                takeProfit = params["takeProfit"]
+
+                stopLossOrder = gate.create_and_test_futures_order(
+                    symbol,
+                    orderSide,
+                    "STOP_MARKET",
+                    stop_price=str(stopLoss),
+                    close_position=True,
+                    price_protect=True,
+                    working_type="MARK_PRICE",
+                    time_in_force="GTC",
+                )
+
+                takeProfitOrder = gate.create_and_test_futures_order(
+                    symbol,
+                    orderSide,
+                    "TAKE_PROFIT_MARKET",
+                    stop_price=str(takeProfit),
+                    close_position=True,
+                    price_protect=True,
+                    working_type="MARK_PRICE",
+                    time_in_force="GTC",
+                )
+                result = gate.make_batch_futures_order([stopLossOrder, takeProfitOrder])
                 # print(result)
                 break
-        elif order['status'] == 'CANCELED':
+        elif order["status"] == "CANCELED":
             break
 
-    print('Watching position')
+    print("Watching position")
     while True:
         time.sleep(0.1)
-        position = gate.getPositionInfo(symbol)[0]
+        position = gate.get_position_info(symbol)[0]
 
-        if float(position['entryPrice']) == 0.0:
-            gate.cancelAllSymbolOpenOrders(symbol, futures=True)
+        if float(position["entryPrice"]) == 0.0:
+            gate.cancel_all_symbol_open_orders(symbol, futures=True)
             break
 
+
 # if __name__ == '__main__':
 #     print(sys.argv)
 #     time.sleep(3)
 #     with open('helloWorld.txt')
```

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/base/printobject.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/base/printobject.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/base/printtime.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/base/printtime.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/restapiinvoker.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/restapiinvoker.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/restapirequestimpl.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/restapirequestimpl.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/utils/apisignature.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/apisignature.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/utils/channels.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/channels.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/utils/inputchecker.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/inputchecker.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/utils/jsonwrapper.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/jsonwrapper.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/utils/urlparamsbuilder.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/utils/urlparamsbuilder.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/websocketconnection.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketconnection.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/websocketrequestimpl.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketrequestimpl.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/impl/websocketwatchdog.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/impl/websocketwatchdog.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/__init__.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/__init__.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/accountinformation.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/accountinformation.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/accountinformationv2.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/accountinformationv2.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/accountupdate.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/accountupdate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/aggregatetrade.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/aggregatetrade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/aggregatetradeevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/aggregatetradeevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/apitradingstatus.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/apitradingstatus.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/balance.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/balance.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/balancev2.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/balancev2.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/blvtinfoevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/blvtinfoevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/blvtnavcandlestick.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/blvtnavcandlestick.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/blvtnavcandlestickevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/blvtnavcandlestickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/candlestick.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/candlestick.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/candlestickevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/candlestickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/compositeindexevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/compositeindexevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/constant.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/constant.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/continuouscandelstickevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/continuouscandelstickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/diffdepthevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/diffdepthevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/exchangeinformation.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/exchangeinformation.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/income.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/income.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/indexInfo.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/indexInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/leverage.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/leverage.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/leveragebracket.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/leveragebracket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/liquidationorder.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/liquidationorder.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/liquidationorderevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/liquidationorderevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/longshortratio.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/longshortratio.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/markprice.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/markprice.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/markpriceevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/markpriceevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/mytrade.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/mytrade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/openintereststats.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/openintereststats.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/order.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/order.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/orderbook.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/orderbook.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/orderbookevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/orderbookevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/orderupdate.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/orderupdate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/position.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/position.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/positionmarginhistory.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/positionmarginhistory.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/symbolbooktickerevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolbooktickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/symbolminitickerevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolminitickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/symbolorderbook.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/symbolorderbook.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/symboltickerevent.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/symboltickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/takerbuysellratio.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/takerbuysellratio.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/tickerpricechangestatistics.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/tickerpricechangestatistics.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/model/trade.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/model/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/requestclient.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/requestclient.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/binance_f/subscriptionclient.py` & `TradeGate-0.3.8.1/TradeGates/binance_f/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/base_request/base_request.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/margin/margin.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/margin/margin.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/market/market.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/market/market.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/trade/trade.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/trade/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/user/user.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/user/user.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/websocket/websocket.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin/ws_client.py` & `TradeGate-0.3.8.1/TradeGates/kucoin/ws_client.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin_futures/base_request/base_request.py` & `TradeGate-0.3.8.1/TradeGates/kucoin_futures/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin_futures/marke_data/market_data.py` & `TradeGate-0.3.8.1/TradeGates/kucoin_futures/marke_data/market_data.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin_futures/trade/trade.py` & `TradeGate-0.3.8.1/TradeGates/kucoin_futures/trade/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin_futures/user/user.py` & `TradeGate-0.3.8.1/TradeGates/kucoin_futures/user/user.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin_futures/websocket/websocket.py` & `TradeGate-0.3.8.1/TradeGates/kucoin_futures/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/TradeGates/kucoin_futures/ws_client.py` & `TradeGate-0.3.8.1/TradeGates/kucoin_futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/setup.py` & `TradeGate-0.3.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     shutil.rmtree("./build")
     shutil.rmtree("./dist")
 except OSError as e:
     print("Error: %s - %s." % (e.filename, e.strerror))
 
 setuptools.setup(
     name="TradeGate",  # This is the name of the package
-    version="0.3.8",
+    version="0.3.8.1",
     author="Rustin Soraki",  # Full name of the author
     description="A Trading Gateway",
     long_description=long_description,  # Long description read from the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(
         where="TradeGates"
     ),  # List of all python modules to be installed
```

### Comparing `TradeGate-0.3.8/test/testAccountInfo.py` & `TradeGate-0.3.8.1/test/testAccountInfo.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,28 +7,24 @@
 
 loglevel = logging.INFO
 logging.basicConfig(level=loglevel)
 log = logging.getLogger(__name__)
 
 
 @pytest.fixture
-def getGates():
-    gates = []
+def get_gates():
     with open("../../config.json") as f:
         config = json.load(f)
 
-    for key in config.keys():
-        gates.append(TradeGate(config[key], sandbox=True))
+    return [TradeGate(config[key], sandbox=True) for key in config.keys()]
 
-    return gates
 
-
-def testFullBalance(getGates):
-    for gate in getGates:
-        balance = gate.get_balance()
+def testFullBalance(get_gates):
+    for gate in get_gates:
+        balance = gate.getBalance()
         print("\nFull Balance from {} exchange: {}".format(gate.exchangeName, balance))
         assert (
             balance is not None
         ), "Problem in fetching balance from {} exchange.".format(gate.exchangeName)
 
         errorMessage = "Bad fetch balance interface for {} exchange,".format(
             gate.exchangeName
@@ -44,16 +40,16 @@
                     ["asset", "free", "locked"]
                 ):
                     assert False, errorMessage
         except Exception:
             assert False, errorMessage
 
 
-def testSingleCoinBalance(getGates):
-    for gate in getGates:
+def testSingleCoinBalance(get_gates):
+    for gate in get_gates:
         balance = gate.get_balance("BTC")
         print(
             "\nSingle coin balance from {} exchange: {}".format(
                 gate.exchangeName, balance
             )
         )
         assert (
@@ -76,20 +72,20 @@
             else:
                 if sorted(list(balance.keys())) != sorted(["asset", "free", "locked"]):
                     assert False, errorMessage
         except Exception:
             assert False, errorMessage
 
 
-def testTradeHistory(getGates):
-    for gate in getGates:
+def testTradeHistory(get_gates):
+    for gate in get_gates:
         if gate.exchangeName.lower() == "kucoin":
-            tradeHistory = gate.symbolAccountTradeHistory("BTC-USDT", futures=False)
+            tradeHistory = gate.symbol_account_trade_history("BTC-USDT", futures=False)
         else:
-            tradeHistory = gate.symbolAccountTradeHistory("BTCUSDT", futures=False)
+            tradeHistory = gate.symbol_account_trade_history("BTCUSDT", futures=False)
         # print('\nTrade history from {} exchange: {}'.format(gate.exchangeName, tradeHistory))
 
         assert (
             tradeHistory is not None
         ), "Problem in fetching trade history from {} exchange.".format(
             gate.exchangeName
         )
```

### Comparing `TradeGate-0.3.8/test/testFutures.py` & `TradeGate-0.3.8.1/test/testFutures.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/test/testMarketInfo.py` & `TradeGate-0.3.8.1/test/testMarketInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8/test/testOrdering.py` & `TradeGate-0.3.8.1/test/testOrdering.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,150 +11,237 @@
 log = logging.getLogger(__name__)
 
 
 @pytest.fixture
 def getGatesAndSymbolNames():
     gates = []
     symbolNames = {}
-    with open('../../config.json') as f:
+    with open("../../config.json") as f:
         config = json.load(f)
 
     for key in config.keys():
         gates.append(TradeGate(config[key], sandbox=True))
-        if gates[-1].exchangeName.lower() == 'kucoin':
-            symbolNames[gates[-1].exchangeName] = 'BTC-USDT'
+        if gates[-1].exchangeName.lower() == "kucoin":
+            symbolNames[gates[-1].exchangeName] = "BTC-USDT"
         else:
-            symbolNames[gates[-1].exchangeName] = 'BTCUSDT'
+            symbolNames[gates[-1].exchangeName] = "BTCUSDT"
 
     return gates, symbolNames
 
 
 def testNewTestOrder(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
         symbolName = symbolNamesDict[gate.exchangeName]
         try:
-            res = gate.createAndTestSpotOrder(symbolName, 'SELL', 'LIMIT', timeInForce='GTC', quantity=0.002,
-                                              price=20000)
-            assert res is not None, 'Problem in testing making order from {} exchange'.format(gate.exchangeName)
+            res = gate.create_and_test_spot_order(
+                symbolName,
+                "SELL",
+                "LIMIT",
+                time_in_force="GTC",
+                quantity=0.002,
+                price=20000,
+            )
+            assert (
+                res is not None
+            ), "Problem in testing making order from {} exchange".format(
+                gate.exchangeName
+            )
         except Exception as e:
-            assert False, 'From {} exchange : {}'.format(gate.exchangeName, str(e))
+            assert False, "From {} exchange : {}".format(gate.exchangeName, str(e))
 
 
 def testNewTestOrderBadOrderType(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
         symbolName = symbolNamesDict[gate.exchangeName]
         try:
-            res = gate.createAndTestSpotOrder(symbolName, 'SELL', 'LINIT', timeInForce='GTC', quantity=0.002,
-                                              price=30000)
-            assert res is None, 'Bad order type and information provided. Must fail (Exchange: {})'.format(
-                gate.exchangeName)
+            res = gate.create_and_test_spot_order(
+                symbolName,
+                "SELL",
+                "LINIT",
+                time_in_force="GTC",
+                quantity=0.002,
+                price=30000,
+            )
+            assert (
+                res is None
+            ), "Bad order type and information provided. Must fail (Exchange: {})".format(
+                gate.exchangeName
+            )
         except Exception as e:
-            assert True, 'Bad order type and information provided. Must fail (Exchange: {})'.format(gate.exchangeName)
+            assert (
+                True
+            ), "Bad order type and information provided. Must fail (Exchange: {})".format(
+                gate.exchangeName
+            )
 
 
 def testNewOrder(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
         symbolName = symbolNamesDict[gate.exchangeName]
         try:
-            verifiedOrder = gate.createAndTestSpotOrder(symbolName, 'BUY', 'LIMIT', quantity=0.002, price=20000,
-                                                        timeInForce='GTC')
-            result = gate.makeSpotOrder(verifiedOrder)
+            verifiedOrder = gate.create_and_test_spot_order(
+                symbolName,
+                "BUY",
+                "LIMIT",
+                quantity=0.002,
+                price=20000,
+                time_in_force="GTC",
+            )
+            result = gate.make_spot_order(verifiedOrder)
             print(result)
-            assert result is not None, 'Problem in making new order in {} exchange'.format(gate.exchangeName)
+            assert (
+                result is not None
+            ), "Problem in making new order in {} exchange".format(gate.exchangeName)
         except Exception:
-            assert False, 'Problem in making new order in {} exchange'.format(gate.exchangeName)
+            assert False, "Problem in making new order in {} exchange".format(
+                gate.exchangeName
+            )
 
 
 def testGetOrders(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
-        if gate.exchangeName.lower() == 'binance':
+        if gate.exchangeName.lower() == "binance":
             continue
         symbolName = symbolNamesDict[gate.exchangeName]
-        orders = gate.getSymbolOrders(symbolName, futures=False)
+        orders = gate.get_symbol_orders(symbolName, futures=False)
         # print('\nGetting order history for BTCUSDT symbol from {}: {}'.format(gate.exchangeName, orders[0]))
 
-        assert orders is not None, 'Problem in getting list of all orders from {} exchange.'.format(gate.exchangeName)
+        assert (
+            orders is not None
+        ), "Problem in getting list of all orders from {} exchange.".format(
+            gate.exchangeName
+        )
 
 
 def testGetOpenOrders(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
-        if gate.exchangeName.lower() == 'binance':
+        if gate.exchangeName.lower() == "binance":
             continue
         symbolName = symbolNamesDict[gate.exchangeName]
-        symbolOpenOrders = gate.getOpenOrders(symbolName)
+        symbolOpenOrders = gate.get_open_orders(symbolName)
         # print('\nGetting BTCUSDT open orders list from {} exchange: {}'.format(gate.exchangeName, symbolOpenOrders))
-        assert symbolOpenOrders is not None, 'Problem in getting list of open orders with symbol from {} exchange.'.format(
-            gate.exchangeName)
+        assert (
+            symbolOpenOrders is not None
+        ), "Problem in getting list of open orders with symbol from {} exchange.".format(
+            gate.exchangeName
+        )
 
 
 def testGetOrder(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
-        if gate.exchangeName.lower() == 'binance':
+        if gate.exchangeName.lower() == "binance":
             continue
         symbolName = symbolNamesDict[gate.exchangeName]
         try:
-            verifiedOrder = gate.createAndTestSpotOrder(symbolName, 'BUY', 'LIMIT', quantity=0.02, price=30000,
-                                                        timeInForce='GTC', newClientOrderId=str(int(time.time())))
-            result = gate.makeSpotOrder(verifiedOrder)
+            verifiedOrder = gate.create_and_test_spot_order(
+                symbolName,
+                "BUY",
+                "LIMIT",
+                quantity=0.02,
+                price=30000,
+                time_in_force="GTC",
+                new_client_order_id=str(int(time.time())),
+            )
+            result = gate.make_spot_order(verifiedOrder)
         except Exception as e:
-            assert False, 'Problem in making order from {} exchange: {}'.format(gate.exchangeName, str(e))
+            assert False, "Problem in making order from {} exchange: {}".format(
+                gate.exchangeName, str(e)
+            )
 
         # print('Submitted order on {} exchange: {}'.format(gate.exchangeName, result))
 
-        order = gate.getOrder(symbolName, orderId=result['orderId'])
-        assert order['clientOrderId'] == result['clientOrderId'], \
-            'Fetch client orderID is not equal to the actual client orderID from {} exchange.'.format(gate.exchangeName)
+        order = gate.get_order(symbolName, order_id=result["orderId"])
+        assert (
+            order["clientOrderId"] == result["clientOrderId"]
+        ), "Fetch client orderID is not equal to the actual client orderID from {} exchange.".format(
+            gate.exchangeName
+        )
         # print('Correct \'clientOrderId\'.')
 
-        order = gate.getOrder(symbolName, localOrderId=result['clientOrderId'])
-        assert order['orderId'] == result['orderId'], \
-            'Fetch orderID is not equal to the actual orderID from {} exchange.'.format(gate.exchangeName)
+        order = gate.get_order(symbolName, local_order_id=result["clientOrderId"])
+        assert (
+            order["orderId"] == result["orderId"]
+        ), "Fetch orderID is not equal to the actual orderID from {} exchange.".format(
+            gate.exchangeName
+        )
         # print('Correct \'orderId\'.')
 
-        gate.cancelOrder('BTCUSDT', orderId=result['orderId'])
+        gate.cancel_order("BTCUSDT", order_id=result["orderId"])
 
 
 def testCancelingAllOpenOrders(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
         symbolName = symbolNamesDict[gate.exchangeName]
-        result = gate.cancelAllSymbolOpenOrders(symbolName)
+        result = gate.cancel_all_symbol_open_orders(symbolName)
 
-        openOrders = gate.getOpenOrders(symbolName)
-        assert len(openOrders) == 0, 'Problem in canceling all Open Orders in {} exchange.'.format(gate.exchangeName)
+        openOrders = gate.get_open_orders(symbolName)
+        assert (
+            len(openOrders) == 0
+        ), "Problem in canceling all Open Orders in {} exchange.".format(
+            gate.exchangeName
+        )
 
 
 def testCancelingOrder(getGatesAndSymbolNames):
     gates, symbolNamesDict = getGatesAndSymbolNames
     for gate in gates:
         symbolName = symbolNamesDict[gate.exchangeName]
         try:
-            verifiedOrder = gate.createAndTestSpotOrder(symbolName, 'BUY', 'LIMIT', quantity=0.002, price=28000,
-                                                        timeInForce='GTC', newClientOrderId=str(int(time.time())))
-            result = gate.makeSpotOrder(verifiedOrder)
+            verifiedOrder = gate.create_and_test_spot_order(
+                symbolName,
+                "BUY",
+                "LIMIT",
+                quantity=0.002,
+                price=28000,
+                time_in_force="GTC",
+                new_client_order_id=str(int(time.time())),
+            )
+            result = gate.make_spot_order(verifiedOrder)
         except Exception as e:
-            assert False, 'Problem in making order in {} exchange: {}'.format(gate.exchangeName, str(e))
-
-        result = gate.cancelOrder(symbol=symbolName, orderId=result['orderId'])
-        result = gate.getOrder(symbol=symbolName, orderId=result['orderId'])
-
-        assert result['status'].upper() in ['CANCELED', 'CANCELLED'], \
-            'Problem in canceling specified Open Orders in {} exchange.'.format(gate.exchangeName)
-
-        try:
-            verifiedOrder = gate.createAndTestSpotOrder(symbolName, 'BUY', 'LIMIT', quantity=0.002, price=28000,
-                                                        timeInForce='GTC', newClientOrderId=str(int(time.time())))
-            result = gate.makeSpotOrder(verifiedOrder)
+            assert False, "Problem in making order in {} exchange: {}".format(
+                gate.exchangeName, str(e)
+            )
+
+        result = gate.cancel_order(symbol=symbolName, order_id=result["orderId"])
+        result = gate.get_order(symbol=symbolName, order_id=result["orderId"])
+
+        assert result["status"].upper() in [
+            "CANCELED",
+            "CANCELLED",
+        ], "Problem in canceling specified Open Orders in {} exchange.".format(
+            gate.exchangeName
+        )
+
+        try:
+            verifiedOrder = gate.create_and_test_spot_order(
+                symbolName,
+                "BUY",
+                "LIMIT",
+                quantity=0.002,
+                price=28000,
+                time_in_force="GTC",
+                new_client_order_id=str(int(time.time())),
+            )
+            result = gate.make_spot_order(verifiedOrder)
         except Exception as e:
-            assert False, 'Problem in making order in {} exchange: {}'.format(gate.exchangeName, str(e))
-
-        result = gate.cancelOrder(symbol=symbolName, localOrderId=result['clientOrderId'])
-        result = gate.getOrder(symbol=symbolName, orderId=result['orderId'])
-
-        assert result['status'].upper() in ['CANCELED', 'CANCELLED'], \
-            'Problem in canceling specified Open Orders in {} exchange.'.format(gate.exchangeName)
+            assert False, "Problem in making order in {} exchange: {}".format(
+                gate.exchangeName, str(e)
+            )
+
+        result = gate.cancel_order(
+            symbol=symbolName, local_order_id=result["clientOrderId"]
+        )
+        result = gate.get_order(symbol=symbolName, order_id=result["orderId"])
+
+        assert result["status"].upper() in [
+            "CANCELED",
+            "CANCELLED",
+        ], "Problem in canceling specified Open Orders in {} exchange.".format(
+            gate.exchangeName
+        )
```

