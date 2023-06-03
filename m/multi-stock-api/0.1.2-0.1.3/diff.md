# Comparing `tmp/multi_stock_api-0.1.2.tar.gz` & `tmp/multi_stock_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_stock_api-0.1.2.tar", last modified: Sun May 28 13:14:09 2023, max compression
+gzip compressed data, was "multi_stock_api-0.1.3.tar", last modified: Sat Jun  3 11:01:57 2023, max compression
```

## Comparing `multi_stock_api-0.1.2.tar` & `multi_stock_api-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/
--rw-rw-r--   0 emir      (1001) emir      (1001)     1064 2023-05-28 08:50:15.000000 multi_stock_api-0.1.2/LICENSE
--rw-rw-r--   0 emir      (1001) emir      (1001)      348 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/PKG-INFO
--rw-rw-r--   0 emir      (1001) emir      (1001)       96 2023-05-28 12:28:24.000000 multi_stock_api-0.1.2/README.md
-drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:14:09.958508 multi_stock_api-0.1.2/multi_stock_api/
--rw-rw-r--   0 emir      (1001) emir      (1001)       26 2023-05-28 12:17:47.000000 multi_stock_api-0.1.2/multi_stock_api/__init__.py
--rw-rw-r--   0 emir      (1001) emir      (1001)     1322 2023-05-28 12:18:46.000000 multi_stock_api-0.1.2/multi_stock_api/app.py
--rw-rw-r--   0 emir      (1001) emir      (1001)     1534 2023-05-28 12:18:38.000000 multi_stock_api-0.1.2/multi_stock_api/configurations.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      915 2023-05-28 12:18:32.000000 multi_stock_api-0.1.2/multi_stock_api/external_api_access.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      326 2023-05-28 12:01:51.000000 multi_stock_api-0.1.2/multi_stock_api/helpers.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      831 2023-05-28 12:18:52.000000 multi_stock_api-0.1.2/multi_stock_api/mappers.py
--rw-rw-r--   0 emir      (1001) emir      (1001)      654 2023-05-28 12:03:50.000000 multi_stock_api-0.1.2/multi_stock_api/models.py
-drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/multi_stock_api.egg-info/
--rw-rw-r--   0 emir      (1001) emir      (1001)      348 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/PKG-INFO
--rw-rw-r--   0 emir      (1001) emir      (1001)      424 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/SOURCES.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)        1 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/dependency_links.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)      490 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/requires.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)       16 2023-05-28 13:14:09.000000 multi_stock_api-0.1.2/multi_stock_api.egg-info/top_level.txt
--rw-rw-r--   0 emir      (1001) emir      (1001)       38 2023-05-28 13:14:09.962508 multi_stock_api-0.1.2/setup.cfg
--rw-rw-r--   0 emir      (1001) emir      (1001)      745 2023-05-28 13:08:47.000000 multi_stock_api-0.1.2/setup.py
+drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-06-03 11:01:57.041738 multi_stock_api-0.1.3/
+-rw-rw-r--   0 emir      (1001) emir      (1001)     1064 2023-05-28 08:50:15.000000 multi_stock_api-0.1.3/LICENSE
+-rw-rw-r--   0 emir      (1001) emir      (1001)      491 2023-06-03 11:01:57.041738 multi_stock_api-0.1.3/PKG-INFO
+-rw-rw-r--   0 emir      (1001) emir      (1001)      239 2023-06-03 11:01:55.000000 multi_stock_api-0.1.3/README.md
+drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-06-03 11:01:57.041738 multi_stock_api-0.1.3/multi_stock_api/
+-rw-rw-r--   0 emir      (1001) emir      (1001)       26 2023-05-28 12:17:47.000000 multi_stock_api-0.1.3/multi_stock_api/__init__.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)     2037 2023-06-03 10:56:07.000000 multi_stock_api-0.1.3/multi_stock_api/app.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)     1638 2023-06-03 08:08:06.000000 multi_stock_api-0.1.3/multi_stock_api/configurations.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      915 2023-06-03 08:06:38.000000 multi_stock_api-0.1.3/multi_stock_api/external_api_access.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      326 2023-05-28 12:01:51.000000 multi_stock_api-0.1.3/multi_stock_api/helpers.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)     1283 2023-06-03 10:54:45.000000 multi_stock_api-0.1.3/multi_stock_api/mappers.py
+-rw-rw-r--   0 emir      (1001) emir      (1001)      773 2023-06-03 10:47:25.000000 multi_stock_api-0.1.3/multi_stock_api/models.py
+drwxrwxr-x   0 emir      (1001) emir      (1001)        0 2023-06-03 11:01:57.041738 multi_stock_api-0.1.3/multi_stock_api.egg-info/
+-rw-rw-r--   0 emir      (1001) emir      (1001)      491 2023-06-03 11:01:57.000000 multi_stock_api-0.1.3/multi_stock_api.egg-info/PKG-INFO
+-rw-rw-r--   0 emir      (1001) emir      (1001)      424 2023-06-03 11:01:57.000000 multi_stock_api-0.1.3/multi_stock_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)        1 2023-06-03 11:01:57.000000 multi_stock_api-0.1.3/multi_stock_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)      490 2023-06-03 11:01:57.000000 multi_stock_api-0.1.3/multi_stock_api.egg-info/requires.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)       16 2023-06-03 11:01:57.000000 multi_stock_api-0.1.3/multi_stock_api.egg-info/top_level.txt
+-rw-rw-r--   0 emir      (1001) emir      (1001)       38 2023-06-03 11:01:57.041738 multi_stock_api-0.1.3/setup.cfg
+-rw-rw-r--   0 emir      (1001) emir      (1001)      745 2023-06-03 10:59:09.000000 multi_stock_api-0.1.3/setup.py
```

### Comparing `multi_stock_api-0.1.2/LICENSE` & `multi_stock_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.2/multi_stock_api/app.py` & `multi_stock_api-0.1.3/multi_stock_api/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,35 @@
 from .external_api_access import ExternalApiAccess
 from .mappers import Mappers
 from .models import SymbolInfo
 
 
 class StockInfo:
-    def __init__(self):        
+    def __init__(self):
         self._markets_info = ExternalApiAccess.get_market_data()
 
+    def get_symbols(self):
+        """
+        Get all available symbols
+        """
+        results = []        
+        
+        if self._markets_info is not None:
+            for market_info in self._markets_info:
+                for symbol_data in market_info.data:
+                    try:
+                        result = Mappers.map_api_results_to_symbol_info_basic(market_info, symbol_data)
+                        if result is not None:
+                            # Get first available symbol result in any market
+                            results.append(result)
+                    except Exception as ex:
+                        print(f"Error retrieving market data - {ex}")
+        
+        return results 
+
     def get_symbol_info(self, symbol: str) -> SymbolInfo:
         """
         Get single symbol info
 
         :param symbols: Ticker symbol
         """
         results = self.get_symbols_info([symbol])
```

### Comparing `multi_stock_api-0.1.2/multi_stock_api/configurations.py` & `multi_stock_api-0.1.3/multi_stock_api/configurations.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     def __init__(self):
         self._markets.append(
             MarketInfo(
                 content_type='application/x-www-form-urlencoded',
                 field_name='SymbolDescription',
                 field_average_percentage_change='AvgPerChange',
+                field_description="SymbolDescription",
                 field_latest_price='LastTradePrice',
                 field_symbol='Symbol',
                 name=Markets.SASE,
                 request_type='POST',
                 root_url='http://www.sase.ba',
                 status_url='FeedServices/HandlerChart.ashx',
                 type='json',
@@ -27,14 +28,15 @@
             )
         )
 
         self._markets.append(
             MarketInfo(
                 field_name='Description',
                 field_average_percentage_change='AvgPerChange',
+                field_description="Description",
                 field_latest_price='AvgPrice',
                 field_symbol='Code',
                 name=Markets.BLBE,
                 request_type='GET',
                 root_url='https://www.blberza.com',
                 status_url='services/defaultTicker.ashx',
                 type='json',
```

### Comparing `multi_stock_api-0.1.2/multi_stock_api/external_api_access.py` & `multi_stock_api-0.1.3/multi_stock_api/external_api_access.py`

 * *Files identical despite different names*

### Comparing `multi_stock_api-0.1.2/multi_stock_api/mappers.py` & `multi_stock_api-0.1.3/multi_stock_api/mappers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from .helpers import Helpers
-from .models import MarketInfo, SymbolInfo
+from .models import MarketInfo, SymbolInfo, SymbolInfoBasic
 
 class Mappers:
     @staticmethod
-    def map_api_results_to_symbol_info(market_info: MarketInfo, symbol: str) -> SymbolInfo:
+    def map_api_results_to_symbol_info_basic(market_info: MarketInfo, api_data: object) -> SymbolInfo:
         try:
-            api_data = next(filter(lambda symbol_data: symbol_data[market_info.field_symbol] == symbol, market_info.data))
-            result = SymbolInfo(
+            return SymbolInfoBasic(
                 market_name=market_info.name.value,
-                average_percentage_change=Helpers.convert_to_percentage(str(api_data[market_info.field_average_percentage_change])),
-                latest_price=Helpers.convert_to_money(api_data[market_info.field_latest_price]),
-                symbol=symbol
+                description=str(api_data[market_info.field_description]),
+                symbol=api_data[market_info.field_symbol]
             )
+        except Exception as ex:
+            print(f"Error parsing info - {ex}")
+            return None
+
+    @staticmethod
+    def map_api_results_to_symbol_info(market_info: MarketInfo, symbol: str) -> SymbolInfo:
+        try:
+            api_data = next(filter(lambda symbol_data: symbol_data[market_info.field_symbol] == symbol, market_info.data))
+            result = Mappers.map_api_results_to_symbol_info_basic(market_info, api_data)
+
+            result.average_percentage_change=Helpers.convert_to_percentage(str(api_data[market_info.field_average_percentage_change]))
+            result.latest_price=Helpers.convert_to_money(api_data[market_info.field_latest_price])
+    
             return result
         except Exception as ex:
             print(f"Error parsing info - {ex}")
             return None
-
```

### Comparing `multi_stock_api-0.1.2/multi_stock_api/models.py` & `multi_stock_api-0.1.3/multi_stock_api/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,16 +16,22 @@
     name: Markets
     request_type: str
     root_url: str
     status_url: str
     type: str
     data: Optional[dict] = None
     field_average_percentage_change: Optional[str] = None
+    field_description: Optional[str] = None
     content_type: Optional[str] = "application/json"
     request_info_params: Optional[dict] = None
 
 @dataclass
-class SymbolInfo:
+class SymbolInfoBasic:
     market_name: str
+    description: str
+    symbol: str
+
+
+@dataclass
+class SymbolInfo(SymbolInfoBasic):
     average_percentage_change: str
     latest_price: str
-    symbol: str
```

### Comparing `multi_stock_api-0.1.2/setup.py` & `multi_stock_api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     long_description = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='multi_stock_api',
-    version='0.1.2',
+    version='0.1.3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Emir Moćević',
     author_email='emirmocevic88@gmail.com',
     license='MIT',
     packages=['multi_stock_api'],
     include_package_data=True,
```

