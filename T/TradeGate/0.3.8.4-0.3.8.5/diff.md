# Comparing `tmp/TradeGate-0.3.8.4.tar.gz` & `tmp/TradeGate-0.3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TradeGate-0.3.8.4.tar", last modified: Sat Jun  3 20:51:45 2023, max compression
+gzip compressed data, was "TradeGate-0.3.8.5.tar", last modified: Sat Jun  3 20:58:50 2023, max compression
```

## Comparing `TradeGate-0.3.8.4.tar` & `TradeGate-0.3.8.5.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.262010 TradeGate-0.3.8.4/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1072 2022-02-23 07:14:51.000000 TradeGate-0.3.8.4/LICENSE
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2611 2023-06-03 20:51:45.262096 TradeGate-0.3.8.4/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2238 2023-05-24 11:59:49.000000 TradeGate-0.3.8.4/README.md
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.236784 TradeGate-0.3.8.4/TradeGates/
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.238391 TradeGate-0.3.8.4/TradeGates/Exchanges/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4475 2023-05-31 07:41:47.000000 TradeGate-0.3.8.4/TradeGates/Exchanges/BaseExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    33868 2023-06-03 20:51:36.000000 TradeGate-0.3.8.4/TradeGates/Exchanges/BinanceExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    34904 2023-05-31 07:42:06.000000 TradeGate-0.3.8.4/TradeGates/Exchanges/BybitExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    44638 2023-05-31 07:42:11.000000 TradeGate-0.3.8.4/TradeGates/Exchanges/KuCoinExchange.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       83 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/Exchanges/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.239247 TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2611 2023-06-03 20:51:45.000000 TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5673 2023-06-03 20:51:45.000000 TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/SOURCES.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-06-03 20:51:45.000000 TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/dependency_links.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       89 2023-06-03 20:51:45.000000 TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/requires.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       67 2023-06-03 20:51:45.000000 TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/top_level.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    59019 2023-06-03 20:51:36.000000 TradeGate-0.3.8.4/TradeGates/TradeGate.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.240570 TradeGate-0.3.8.4/TradeGates/Utils/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4281 2023-05-24 18:22:33.000000 TradeGate-0.3.8.4/TradeGates/Utils/BinanceHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    14074 2023-05-24 18:51:07.000000 TradeGate-0.3.8.4/TradeGates/Utils/BybitHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     8515 2023-06-03 20:47:46.000000 TradeGate-0.3.8.4/TradeGates/Utils/DataHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    13473 2023-05-24 18:52:23.000000 TradeGate-0.3.8.4/TradeGates/Utils/KuCoinHelpers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       80 2022-10-02 08:05:21.000000 TradeGate-0.3.8.4/TradeGates/Utils/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.240954 TradeGate-0.3.8.4/TradeGates/Watchers/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/Watchers/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2645 2023-05-24 12:20:18.000000 TradeGate-0.3.8.4/TradeGates/Watchers/futureOrderWatchers.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.242029 TradeGate-0.3.8.4/TradeGates/binance_f/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      112 2022-02-23 05:49:50.000000 TradeGate-0.3.8.4/TradeGates/binance_f/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.242727 TradeGate-0.3.8.4/TradeGates/binance_f/base/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/base/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5597 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/base/printobject.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      597 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/base/printtime.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.243153 TradeGate-0.3.8.4/TradeGates/binance_f/constant/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/constant/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      399 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/constant/system.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      250 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/constant/test.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.243396 TradeGate-0.3.8.4/TradeGates/binance_f/exception/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/exception/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      422 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/exception/binanceapiexception.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.245611 TradeGate-0.3.8.4/TradeGates/binance_f/impl/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)       58 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2680 2022-02-26 09:29:35.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/restapiinvoker.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      310 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/restapirequest.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    36651 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/restapirequestimpl.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.246872 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      240 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1146 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/apisignature.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      156 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/channelparser.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5407 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/channels.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3139 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/inputchecker.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3400 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/jsonwrapper.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      434 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/timeservice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1030 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/urlparamsbuilder.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     7819 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketconnection.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      360 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketrequest.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    15345 2022-03-03 18:09:37.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketrequestimpl.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2243 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketwatchdog.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.255372 TradeGate-0.3.8.4/TradeGates/binance_f/model/
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2976 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/__init__.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     4355 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/accountinformation.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5309 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/accountinformationv2.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2355 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/accountupdate.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      343 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/adlquantile.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      690 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/aggregatetrade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      971 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/aggregatetradeevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/apitradingstatus.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      999 2022-03-02 11:34:30.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/balance.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      854 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/balancev2.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      908 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/blvtinfoevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      706 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/blvtnavcandlestick.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1789 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/blvtnavcandlestickevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1607 2022-02-24 11:54:59.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/candlestick.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2230 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/candlestickevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      438 2022-03-04 10:50:30.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/codeandmsg.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1304 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/compositeindexevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2103 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/constant.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2389 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/continuouscandelstickevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      352 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/countdowncancelall.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1634 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/diffdepthevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3756 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/exchangeinformation.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      433 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/fundingrate.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      791 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/income.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/indexInfo.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      568 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/leverage.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1271 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/leveragebracket.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      937 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/liquidationorder.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1410 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/liquidationorderevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      337 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/listenkeyexpired.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      775 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/longshortratio.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      620 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/markprice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      661 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/markpriceevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      393 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/message.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2369 2022-03-04 07:28:24.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/mytrade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      349 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/openinterest.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      635 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/openintereststats.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3160 2022-03-04 10:20:23.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/order.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1309 2022-06-17 14:41:44.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/orderbook.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1584 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/orderbookevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3015 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/orderupdate.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1978 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/position.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      461 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/positionmargin.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      558 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/positionmarginhistory.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      274 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/positionmode.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      765 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolbooktickerevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      970 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolminitickerevent.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      583 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolorderbook.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      386 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolprice.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1862 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/symboltickerevent.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      531 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/takerbuysellratio.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1691 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/tickerpricechangestatistics.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      896 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/binance_f/model/trade.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    23283 2022-03-23 21:08:19.000000 TradeGate-0.3.8.4/TradeGates/binance_f/requestclient.py
--rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    12780 2021-08-19 21:43:22.000000 TradeGate-0.3.8.4/TradeGates/binance_f/subscriptionclient.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.255786 TradeGate-0.3.8.4/TradeGates/kucoin/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.256158 TradeGate-0.3.8.4/TradeGates/kucoin/base_request/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/base_request/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4269 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/base_request/base_request.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      390 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.256441 TradeGate-0.3.8.4/TradeGates/kucoin/margin/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/margin/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    14243 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/margin/margin.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.256706 TradeGate-0.3.8.4/TradeGates/kucoin/market/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/market/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    16795 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/market/market.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.257052 TradeGate-0.3.8.4/TradeGates/kucoin/trade/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/trade/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    24825 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/trade/trade.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.257465 TradeGate-0.3.8.4/TradeGates/kucoin/user/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/user/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    23869 2022-06-27 12:34:05.000000 TradeGate-0.3.8.4/TradeGates/kucoin/user/user.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.258158 TradeGate-0.3.8.4/TradeGates/kucoin/websocket/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/websocket/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/websocket/websocket.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1594 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/ws_client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.258416 TradeGate-0.3.8.4/TradeGates/kucoin/ws_token/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/ws_token/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      451 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin/ws_token/token.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.258885 TradeGate-0.3.8.4/TradeGates/kucoin_futures/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.259168 TradeGate-0.3.8.4/TradeGates/kucoin_futures/base_request/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/base_request/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4299 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/base_request/base_request.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      376 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.259442 TradeGate-0.3.8.4/TradeGates/kucoin_futures/marke_data/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/marke_data/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    22513 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/marke_data/market_data.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.259825 TradeGate-0.3.8.4/TradeGates/kucoin_futures/trade/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/trade/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    31092 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/trade/trade.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.260163 TradeGate-0.3.8.4/TradeGates/kucoin_futures/user/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/user/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     9818 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/user/user.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.260440 TradeGate-0.3.8.4/TradeGates/kucoin_futures/websocket/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/websocket/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/websocket/websocket.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1620 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/ws_client.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.260725 TradeGate-0.3.8.4/TradeGates/kucoin_futures/ws_token/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/ws_token/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      480 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/TradeGates/kucoin_futures/ws_token/token.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      267 2022-06-17 08:03:32.000000 TradeGate-0.3.8.4/pyproject.toml
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       79 2023-06-03 20:51:45.262327 TradeGate-0.3.8.4/setup.cfg
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1453 2023-06-03 20:51:41.000000 TradeGate-0.3.8.4/setup.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:51:45.261673 TradeGate-0.3.8.4/test/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3863 2023-05-30 21:01:57.000000 TradeGate-0.3.8.4/test/testAccountInfo.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    16024 2022-06-27 15:23:02.000000 TradeGate-0.3.8.4/test/testFutures.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5351 2022-06-16 09:06:16.000000 TradeGate-0.3.8.4/test/testMarketInfo.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     8386 2023-05-24 11:59:49.000000 TradeGate-0.3.8.4/test/testOrdering.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.093975 TradeGate-0.3.8.5/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1072 2022-02-23 07:14:51.000000 TradeGate-0.3.8.5/LICENSE
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2611 2023-06-03 20:58:50.094057 TradeGate-0.3.8.5/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2238 2023-05-24 11:59:49.000000 TradeGate-0.3.8.5/README.md
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.068147 TradeGate-0.3.8.5/TradeGates/
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.070272 TradeGate-0.3.8.5/TradeGates/Exchanges/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4475 2023-05-31 07:41:47.000000 TradeGate-0.3.8.5/TradeGates/Exchanges/BaseExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    33784 2023-06-03 20:58:40.000000 TradeGate-0.3.8.5/TradeGates/Exchanges/BinanceExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    34904 2023-05-31 07:42:06.000000 TradeGate-0.3.8.5/TradeGates/Exchanges/BybitExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    44638 2023-05-31 07:42:11.000000 TradeGate-0.3.8.5/TradeGates/Exchanges/KuCoinExchange.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       83 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/Exchanges/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.071121 TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2611 2023-06-03 20:58:49.000000 TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5673 2023-06-03 20:58:49.000000 TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/SOURCES.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-06-03 20:58:49.000000 TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/dependency_links.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       89 2023-06-03 20:58:49.000000 TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/requires.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       67 2023-06-03 20:58:49.000000 TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/top_level.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    59019 2023-06-03 20:51:36.000000 TradeGate-0.3.8.5/TradeGates/TradeGate.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.072527 TradeGate-0.3.8.5/TradeGates/Utils/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4281 2023-05-24 18:22:33.000000 TradeGate-0.3.8.5/TradeGates/Utils/BinanceHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    14074 2023-05-24 18:51:07.000000 TradeGate-0.3.8.5/TradeGates/Utils/BybitHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     8515 2023-06-03 20:47:46.000000 TradeGate-0.3.8.5/TradeGates/Utils/DataHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    13473 2023-05-24 18:52:23.000000 TradeGate-0.3.8.5/TradeGates/Utils/KuCoinHelpers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       80 2022-10-02 08:05:21.000000 TradeGate-0.3.8.5/TradeGates/Utils/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.072882 TradeGate-0.3.8.5/TradeGates/Watchers/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/Watchers/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2645 2023-05-24 12:20:18.000000 TradeGate-0.3.8.5/TradeGates/Watchers/futureOrderWatchers.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.073963 TradeGate-0.3.8.5/TradeGates/binance_f/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      112 2022-02-23 05:49:50.000000 TradeGate-0.3.8.5/TradeGates/binance_f/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.074725 TradeGate-0.3.8.5/TradeGates/binance_f/base/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/base/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5597 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/base/printobject.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      597 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/base/printtime.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.075233 TradeGate-0.3.8.5/TradeGates/binance_f/constant/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/constant/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      399 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/constant/system.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      250 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/constant/test.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.075478 TradeGate-0.3.8.5/TradeGates/binance_f/exception/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/exception/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      422 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/exception/binanceapiexception.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.077492 TradeGate-0.3.8.5/TradeGates/binance_f/impl/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)       58 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2680 2022-02-26 09:29:35.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/restapiinvoker.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      310 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/restapirequest.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    36651 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/restapirequestimpl.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.078872 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      240 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1146 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/apisignature.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      156 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/channelparser.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     5407 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/channels.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3139 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/inputchecker.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3400 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/jsonwrapper.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      434 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/timeservice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1030 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/urlparamsbuilder.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     7819 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketconnection.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      360 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketrequest.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    15345 2022-03-03 18:09:37.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketrequestimpl.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2243 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketwatchdog.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.087646 TradeGate-0.3.8.5/TradeGates/binance_f/model/
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2976 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/__init__.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     4355 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/accountinformation.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5309 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/accountinformationv2.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2355 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/accountupdate.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      343 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/adlquantile.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      690 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/aggregatetrade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      971 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/aggregatetradeevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/apitradingstatus.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      999 2022-03-02 11:34:30.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/balance.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      854 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/balancev2.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      908 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/blvtinfoevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      706 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/blvtnavcandlestick.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1789 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/blvtnavcandlestickevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1607 2022-02-24 11:54:59.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/candlestick.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2230 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/candlestickevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      438 2022-03-04 10:50:30.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/codeandmsg.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1304 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/compositeindexevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2103 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/constant.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2389 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/continuouscandelstickevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      352 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/countdowncancelall.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1634 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/diffdepthevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3756 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/exchangeinformation.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      433 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/fundingrate.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      791 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/income.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1102 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/indexInfo.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      568 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/leverage.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1271 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/leveragebracket.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      937 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/liquidationorder.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1410 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/liquidationorderevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      337 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/listenkeyexpired.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      775 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/longshortratio.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      620 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/markprice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      661 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/markpriceevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      393 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/message.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     2369 2022-03-04 07:28:24.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/mytrade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      349 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/openinterest.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      635 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/openintereststats.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3160 2022-03-04 10:20:23.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/order.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1309 2022-06-17 14:41:44.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/orderbook.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1584 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/orderbookevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     3015 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/orderupdate.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1978 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/position.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      461 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/positionmargin.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      558 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/positionmarginhistory.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      274 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/positionmode.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      765 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolbooktickerevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      970 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolminitickerevent.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      583 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolorderbook.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      386 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolprice.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1862 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/symboltickerevent.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      531 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/takerbuysellratio.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)     1691 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/tickerpricechangestatistics.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)      896 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/binance_f/model/trade.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    23283 2022-03-23 21:08:19.000000 TradeGate-0.3.8.5/TradeGates/binance_f/requestclient.py
+-rwxr-xr-x   0 rustinsoraki   (501) staff       (20)    12780 2021-08-19 21:43:22.000000 TradeGate-0.3.8.5/TradeGates/binance_f/subscriptionclient.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.088074 TradeGate-0.3.8.5/TradeGates/kucoin/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.088466 TradeGate-0.3.8.5/TradeGates/kucoin/base_request/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/base_request/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4269 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/base_request/base_request.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      390 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.088740 TradeGate-0.3.8.5/TradeGates/kucoin/margin/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/margin/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    14243 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/margin/margin.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.088971 TradeGate-0.3.8.5/TradeGates/kucoin/market/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/market/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    16795 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/market/market.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.089252 TradeGate-0.3.8.5/TradeGates/kucoin/trade/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/trade/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    24825 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/trade/trade.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.089665 TradeGate-0.3.8.5/TradeGates/kucoin/user/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/user/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    23869 2022-06-27 12:34:05.000000 TradeGate-0.3.8.5/TradeGates/kucoin/user/user.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.090280 TradeGate-0.3.8.5/TradeGates/kucoin/websocket/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/websocket/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/websocket/websocket.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1594 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/ws_client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.090571 TradeGate-0.3.8.5/TradeGates/kucoin/ws_token/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/ws_token/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      451 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin/ws_token/token.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.091025 TradeGate-0.3.8.5/TradeGates/kucoin_futures/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.091287 TradeGate-0.3.8.5/TradeGates/kucoin_futures/base_request/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/base_request/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4299 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/base_request/base_request.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      376 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.091559 TradeGate-0.3.8.5/TradeGates/kucoin_futures/marke_data/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/marke_data/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    22513 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/marke_data/market_data.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.091881 TradeGate-0.3.8.5/TradeGates/kucoin_futures/trade/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/trade/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    31092 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/trade/trade.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.092190 TradeGate-0.3.8.5/TradeGates/kucoin_futures/user/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/user/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     9818 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/user/user.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.092474 TradeGate-0.3.8.5/TradeGates/kucoin_futures/websocket/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/websocket/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5633 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/websocket/websocket.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1620 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/ws_client.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.092741 TradeGate-0.3.8.5/TradeGates/kucoin_futures/ws_token/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/ws_token/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      480 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/TradeGates/kucoin_futures/ws_token/token.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      267 2022-06-17 08:03:32.000000 TradeGate-0.3.8.5/pyproject.toml
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       79 2023-06-03 20:58:50.094286 TradeGate-0.3.8.5/setup.cfg
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1453 2023-06-03 20:58:47.000000 TradeGate-0.3.8.5/setup.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-06-03 20:58:50.093626 TradeGate-0.3.8.5/test/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3863 2023-05-30 21:01:57.000000 TradeGate-0.3.8.5/test/testAccountInfo.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    16024 2022-06-27 15:23:02.000000 TradeGate-0.3.8.5/test/testFutures.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5351 2022-06-16 09:06:16.000000 TradeGate-0.3.8.5/test/testMarketInfo.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     8386 2023-05-24 11:59:49.000000 TradeGate-0.3.8.5/test/testOrdering.py
```

### Comparing `TradeGate-0.3.8.4/LICENSE` & `TradeGate-0.3.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/PKG-INFO` & `TradeGate-0.3.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TradeGate
-Version: 0.3.8.4
+Version: 0.3.8.5
 Summary: A Trading Gateway
 Author: Rustin Soraki
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TradeGate-0.3.8.4/README.md` & `TradeGate-0.3.8.5/README.md`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Exchanges/BaseExchange.py` & `TradeGate-0.3.8.5/TradeGates/Exchanges/BaseExchange.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Exchanges/BinanceExchange.py` & `TradeGate-0.3.8.5/TradeGates/Exchanges/BinanceExchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,14 @@
 
     elif order.order_type in ["STOP_LOSS_LIMIT", "TAKE_PROFIT_LIMIT"]:
         check_spot_stop_limit_order_data_validity(order)
 
     elif order.order_type == "LIMIT_MAKER":
         check_spot_limit_maker_order_data_validity(order)
 
-    return False
-
 
 def check_spot_limit_maker_order_data_validity(order):
     if order.quantity is None or order.price is None:
         raise ValueError("For LIMIT_MAKER order quantity and price must be specified.")
 
 
 def check_spot_stop_limit_order_data_validity(order):
@@ -329,16 +327,15 @@
                 ]
         except Exception as e:
             print(e)
             return None
 
     def test_spot_order(self, order_data):
         # sourcery skip: no-conditionals-in-tests
-        if not is_order_data_valid(order_data):
-            raise ValueError("Incomplete data provided.")
+        is_order_data_valid(order_data)
 
         order_data.set_timestamp()
         params = BinanceHelpers.get_spot_order_as_dict(order_data)
 
         return self.client.new_order_test(**params)
 
     def make_spot_order(self, order_data):
```

### Comparing `TradeGate-0.3.8.4/TradeGates/Exchanges/BybitExchange.py` & `TradeGate-0.3.8.5/TradeGates/Exchanges/BybitExchange.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Exchanges/KuCoinExchange.py` & `TradeGate-0.3.8.5/TradeGates/Exchanges/KuCoinExchange.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/PKG-INFO` & `TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TradeGate
-Version: 0.3.8.4
+Version: 0.3.8.5
 Summary: A Trading Gateway
 Author: Rustin Soraki
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TradeGate-0.3.8.4/TradeGates/TradeGate.egg-info/SOURCES.txt` & `TradeGate-0.3.8.5/TradeGates/TradeGate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/TradeGate.py` & `TradeGate-0.3.8.5/TradeGates/TradeGate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Utils/BinanceHelpers.py` & `TradeGate-0.3.8.5/TradeGates/Utils/BinanceHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Utils/BybitHelpers.py` & `TradeGate-0.3.8.5/TradeGates/Utils/BybitHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Utils/DataHelpers.py` & `TradeGate-0.3.8.5/TradeGates/Utils/DataHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Utils/KuCoinHelpers.py` & `TradeGate-0.3.8.5/TradeGates/Utils/KuCoinHelpers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/Watchers/futureOrderWatchers.py` & `TradeGate-0.3.8.5/TradeGates/Watchers/futureOrderWatchers.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/base/printobject.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/base/printobject.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/base/printtime.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/base/printtime.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/restapiinvoker.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/restapiinvoker.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/restapirequestimpl.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/restapirequestimpl.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/apisignature.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/apisignature.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/channels.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/channels.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/inputchecker.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/inputchecker.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/jsonwrapper.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/jsonwrapper.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/utils/urlparamsbuilder.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/utils/urlparamsbuilder.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketconnection.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketconnection.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketrequestimpl.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketrequestimpl.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/impl/websocketwatchdog.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/impl/websocketwatchdog.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/__init__.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/__init__.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/accountinformation.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/accountinformation.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/accountinformationv2.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/accountinformationv2.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/accountupdate.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/accountupdate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/aggregatetrade.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/aggregatetrade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/aggregatetradeevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/aggregatetradeevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/apitradingstatus.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/apitradingstatus.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/balance.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/balance.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/balancev2.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/balancev2.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/blvtinfoevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/blvtinfoevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/blvtnavcandlestick.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/blvtnavcandlestick.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/blvtnavcandlestickevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/blvtnavcandlestickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/candlestick.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/candlestick.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/candlestickevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/candlestickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/compositeindexevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/compositeindexevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/constant.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/constant.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/continuouscandelstickevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/continuouscandelstickevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/diffdepthevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/diffdepthevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/exchangeinformation.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/exchangeinformation.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/income.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/income.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/indexInfo.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/indexInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/leverage.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/leverage.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/leveragebracket.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/leveragebracket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/liquidationorder.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/liquidationorder.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/liquidationorderevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/liquidationorderevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/longshortratio.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/longshortratio.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/markprice.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/markprice.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/markpriceevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/markpriceevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/mytrade.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/mytrade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/openintereststats.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/openintereststats.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/order.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/order.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/orderbook.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/orderbook.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/orderbookevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/orderbookevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/orderupdate.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/orderupdate.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/position.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/position.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/positionmarginhistory.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/positionmarginhistory.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolbooktickerevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolbooktickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolminitickerevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolminitickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/symbolorderbook.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/symbolorderbook.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/symboltickerevent.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/symboltickerevent.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/takerbuysellratio.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/takerbuysellratio.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/tickerpricechangestatistics.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/tickerpricechangestatistics.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/model/trade.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/model/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/requestclient.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/requestclient.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/binance_f/subscriptionclient.py` & `TradeGate-0.3.8.5/TradeGates/binance_f/subscriptionclient.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/base_request/base_request.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/margin/margin.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/margin/margin.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/market/market.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/market/market.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/trade/trade.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/trade/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/user/user.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/user/user.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/websocket/websocket.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin/ws_client.py` & `TradeGate-0.3.8.5/TradeGates/kucoin/ws_client.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin_futures/base_request/base_request.py` & `TradeGate-0.3.8.5/TradeGates/kucoin_futures/base_request/base_request.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin_futures/marke_data/market_data.py` & `TradeGate-0.3.8.5/TradeGates/kucoin_futures/marke_data/market_data.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin_futures/trade/trade.py` & `TradeGate-0.3.8.5/TradeGates/kucoin_futures/trade/trade.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin_futures/user/user.py` & `TradeGate-0.3.8.5/TradeGates/kucoin_futures/user/user.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin_futures/websocket/websocket.py` & `TradeGate-0.3.8.5/TradeGates/kucoin_futures/websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/TradeGates/kucoin_futures/ws_client.py` & `TradeGate-0.3.8.5/TradeGates/kucoin_futures/ws_client.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/setup.py` & `TradeGate-0.3.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     shutil.rmtree("./build")
     shutil.rmtree("./dist")
 except OSError as e:
     print("Error: %s - %s." % (e.filename, e.strerror))
 
 setuptools.setup(
     name="TradeGate",  # This is the name of the package
-    version="0.3.8.4",
+    version="0.3.8.5",
     author="Rustin Soraki",  # Full name of the author
     description="A Trading Gateway",
     long_description=long_description,  # Long description read from the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(
         where="TradeGates"
     ),  # List of all python modules to be installed
```

### Comparing `TradeGate-0.3.8.4/test/testAccountInfo.py` & `TradeGate-0.3.8.5/test/testAccountInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/test/testFutures.py` & `TradeGate-0.3.8.5/test/testFutures.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/test/testMarketInfo.py` & `TradeGate-0.3.8.5/test/testMarketInfo.py`

 * *Files identical despite different names*

### Comparing `TradeGate-0.3.8.4/test/testOrdering.py` & `TradeGate-0.3.8.5/test/testOrdering.py`

 * *Files identical despite different names*

