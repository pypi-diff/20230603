# Comparing `tmp/quantplay-1.2.94.tar.gz` & `tmp/quantplay-1.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.94.tar", last modified: Fri Jun  2 03:09:04 2023, max compression
+gzip compressed data, was "quantplay-1.2.95.tar", last modified: Sat Jun  3 09:13:01 2023, max compression
```

## Comparing `quantplay-1.2.94.tar` & `quantplay-1.2.95.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.912576 quantplay-1.2.94/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-02 03:09:04.912633 quantplay-1.2.94/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.94/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.901507 quantplay-1.2.94/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.902347 quantplay-1.2.94/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.94/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.904281 quantplay-1.2.94/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.904575 quantplay-1.2.94/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.94/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.904823 quantplay-1.2.94/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.94/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.94/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.94/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.94/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-02 03:08:35.000000 quantplay-1.2.94/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.905582 quantplay-1.2.94/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.94/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.94/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.94/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.905700 quantplay-1.2.94/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.905924 quantplay-1.2.94/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906136 quantplay-1.2.94/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.94/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906383 quantplay-1.2.94/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.94/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906568 quantplay-1.2.94/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906766 quantplay-1.2.94/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.906961 quantplay-1.2.94/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907261 quantplay-1.2.94/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907367 quantplay-1.2.94/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907746 quantplay-1.2.94/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.94/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.907963 quantplay-1.2.94/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908071 quantplay-1.2.94/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908368 quantplay-1.2.94/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908663 quantplay-1.2.94/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.94/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.908991 quantplay-1.2.94/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.94/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11801 2023-05-31 03:18:14.000000 quantplay-1.2.94/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909103 quantplay-1.2.94/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.94/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909198 quantplay-1.2.94/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.94/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909299 quantplay-1.2.94/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.94/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909388 quantplay-1.2.94/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.94/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909495 quantplay-1.2.94/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.94/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909591 quantplay-1.2.94/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.94/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.909679 quantplay-1.2.94/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.94/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.910121 quantplay-1.2.94/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.94/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.910310 quantplay-1.2.94/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.94/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.94/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.911334 quantplay-1.2.94/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.94/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.94/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.94/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.902116 quantplay-1.2.94/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-02 03:09:04.000000 quantplay-1.2.94/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-02 03:09:04.912833 quantplay-1.2.94/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-02 03:09:02.000000 quantplay-1.2.94/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.911550 quantplay-1.2.94/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.94/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.911775 quantplay-1.2.94/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.912071 quantplay-1.2.94/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-02 03:09:04.912450 quantplay-1.2.94/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.94/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.217653 quantplay-1.2.95/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-03 09:13:01.217774 quantplay-1.2.95/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.95/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.198494 quantplay-1.2.95/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.199540 quantplay-1.2.95/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.95/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.203456 quantplay-1.2.95/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.204234 quantplay-1.2.95/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.95/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.204779 quantplay-1.2.95/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.95/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.95/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.95/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.95/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.95/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19145 2023-06-02 03:08:35.000000 quantplay-1.2.95/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.206484 quantplay-1.2.95/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.95/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6456 2023-06-02 03:04:08.000000 quantplay-1.2.95/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.95/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.206575 quantplay-1.2.95/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.206754 quantplay-1.2.95/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.207199 quantplay-1.2.95/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.95/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.208328 quantplay-1.2.95/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.95/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.208515 quantplay-1.2.95/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.95/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.95/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.208758 quantplay-1.2.95/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.209056 quantplay-1.2.95/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.209696 quantplay-1.2.95/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.209868 quantplay-1.2.95/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.210467 quantplay-1.2.95/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.95/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.210704 quantplay-1.2.95/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.210876 quantplay-1.2.95/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.211210 quantplay-1.2.95/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.211623 quantplay-1.2.95/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.95/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.95/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.212381 quantplay-1.2.95/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.95/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10711 2023-06-03 09:12:45.000000 quantplay-1.2.95/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.212584 quantplay-1.2.95/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.95/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.212683 quantplay-1.2.95/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.95/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.212786 quantplay-1.2.95/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.95/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.212898 quantplay-1.2.95/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.95/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.212998 quantplay-1.2.95/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.95/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.213102 quantplay-1.2.95/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.95/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.213194 quantplay-1.2.95/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.95/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.213988 quantplay-1.2.95/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.95/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.95/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.95/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.95/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.214267 quantplay-1.2.95/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.95/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.95/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.216308 quantplay-1.2.95/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.95/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.95/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.95/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.199305 quantplay-1.2.95/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-03 09:13:01.000000 quantplay-1.2.95/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-06-03 09:13:01.000000 quantplay-1.2.95/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-03 09:13:01.000000 quantplay-1.2.95/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-03 09:13:01.000000 quantplay-1.2.95/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-03 09:13:01.000000 quantplay-1.2.95/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-03 09:13:01.218074 quantplay-1.2.95/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-03 09:12:58.000000 quantplay-1.2.95/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.216590 quantplay-1.2.95/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.95/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.216829 quantplay-1.2.95/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.217070 quantplay-1.2.95/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-03 09:13:01.217474 quantplay-1.2.95/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.95/test/test_motilal.py
```

### Comparing `quantplay-1.2.94/PKG-INFO` & `quantplay-1.2.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.94
+Version: 1.2.95
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.94/quantplay/backtest/backtest_trades.py` & `quantplay-1.2.95/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/angelone.py` & `quantplay-1.2.95/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/broker_client.py` & `quantplay-1.2.95/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.2.95/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/generics/broker.py` & `quantplay-1.2.95/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/iifl.py` & `quantplay-1.2.95/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/iifl_xts.py` & `quantplay-1.2.95/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/kite_utils.py` & `quantplay-1.2.95/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/motilal.py` & `quantplay-1.2.95/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/shoonya.py` & `quantplay-1.2.95/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/symphony.py` & `quantplay-1.2.95/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/xts.py` & `quantplay-1.2.95/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.2.95/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.2.95/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.2.95/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.2.95/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/broker/zerodha.py` & `quantplay-1.2.95/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.2.95/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/brokerage/generics/broker.py` & `quantplay-1.2.95/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.2.95/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/config/qplay_config.py` & `quantplay-1.2.95/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/create_sample_data.py` & `quantplay-1.2.95/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/data_modify_script.py` & `quantplay-1.2.95/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/date_fix.py` & `quantplay-1.2.95/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/exception/exceptions.py` & `quantplay-1.2.95/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/executor/strategy_executor.py` & `quantplay-1.2.95/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/indicators/Indicator.py` & `quantplay-1.2.95/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/model/exchange/instrument.py` & `quantplay-1.2.95/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/model/exchange/order.py` & `quantplay-1.2.95/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/model/exchange/tick.py` & `quantplay-1.2.95/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.2.95/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/order_execution/mean_price.py` & `quantplay-1.2.95/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/reporting/strategy_report.py` & `quantplay-1.2.95/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/reporting/visuals.py` & `quantplay-1.2.95/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/services/market.py` & `quantplay-1.2.95/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/services/tradelens.py` & `quantplay-1.2.95/quantplay/services/tradelens.py`

 * *Files 10% similar despite different names*

```diff
@@ -194,59 +194,27 @@
                 "date_only": date_only,
                 "backtesting_pnl": trades[trades.date_only.astype(str) == date_only].profit.sum(),
                 "minimum_pnl": response["minimum_pnl"]
             })
 
         return pd.DataFrame(trade_analysis)
 
-    def alpha_runner(alpha: typing.Callable, day_candles: pd.DataFrame):
-        """
-        Passes Required Parameters to the alpha function
-        """
-        return alpha(
-            open=day_candles.open,
-            low=day_candles.low,
-            high=day_candles.high,
-            close=day_candles.close,
-            volume=day_candles.volume,
-            vwap=day_candles.vwap,
-            returns=day_candles.returns,
-            adv5=day_candles.adv5,
-            adv10=day_candles.adv10,
-            adv15=day_candles.adv15,
-            adv20=day_candles.adv20,
-            adv30=day_candles.adv30,
-            adv40=day_candles.adv40,
-            adv50=day_candles.adv50,
-            adv60=day_candles.adv60,
-            adv81=day_candles.adv81,
-            adv120=day_candles.adv120,
-            adv150=day_candles.adv150,
-            adv180=day_candles.adv180,
-        )
-
-
     @staticmethod
-    def validate_alpha(self, day_candles, alpha, num_buckets=10):
+    def validate_alpha(day_candles, alpha_name, num_buckets=10):
         """Validate alphas by bucketing them into 10 buckets and checking the returns
 
         Args:
             day_candles (DataFrame): Dataframe containing day candles
-            alpha (Function): function for calculating alpha
+            alpha (string): name of the alpha
             num_buckets (int, optional): No of brackets required. Defaults to 10.
         """
         try:
-            alpha_name = alpha.__name__
             alpha_bucket_name = "{}_bucket".format(alpha_name)
 
-            alpha_candles = day_candles[["date"]]
-
-            alpha_candles.loc[:, alpha_name] = self.alpha_runner(alpha=alpha, day_candles=day_candles)
-            
-            
+            alpha_candles = day_candles
             alpha_candles.loc[:, f"{alpha_name}_rank"] = alpha_candles.groupby("date")[
                 alpha_name
             ].rank(ascending=False)
 
             alpha_candles.loc[:, "is_top500"] = np.where(
                 (alpha_candles[f"{alpha_name}_rank"] <= 500), True, False
             )
@@ -280,14 +248,14 @@
             t_df = (
                 alpha_candles.groupby(alpha_bucket_name)
                 .next_day_intraday_return.mean()
                 .reset_index()
             )
 
             plt.clf()
-            plt.title(alpha_name)
+            plt.title(f"{alpha_name} intraday return analysis")
             plt.bar(t_df[alpha_bucket_name], -1 *
                     t_df.next_day_intraday_return)
             plt.show()
 
         except Exception as e:
-            print(alpha, inspect.signature(alpha), e)
+            print(e)
```

### Comparing `quantplay-1.2.94/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.2.95/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.2.95/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/strategy/base.py` & `quantplay-1.2.95/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/config_util.py` & `quantplay-1.2.95/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/constant.py` & `quantplay-1.2.95/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/data_utils.py` & `quantplay-1.2.95/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/exchange.py` & `quantplay-1.2.95/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/number_utils.py` & `quantplay-1.2.95/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/selenium_utils.py` & `quantplay-1.2.95/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay/utils/transaction_utils.py` & `quantplay-1.2.95/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/quantplay.egg-info/PKG-INFO` & `quantplay-1.2.95/quantplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.94
+Version: 1.2.95
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.94/quantplay.egg-info/SOURCES.txt` & `quantplay-1.2.95/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/setup.py` & `quantplay-1.2.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.94",
+    version="1.2.95",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.94/test/strategy/sample_strategy.py` & `quantplay-1.2.95/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.94/test/test_motilal.py` & `quantplay-1.2.95/test/test_motilal.py`

 * *Files identical despite different names*

