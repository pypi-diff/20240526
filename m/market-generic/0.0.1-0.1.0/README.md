# Comparing `tmp/market_generic-0.0.1.tar.gz` & `tmp/market_generic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market_generic-0.0.1.tar", last modified: Mon May 20 18:36:00 2024, max compression
+gzip compressed data, was "market_generic-0.1.0.tar", last modified: Sun May 26 16:23:11 2024, max compression
```

## Comparing `market_generic-0.0.1.tar` & `market_generic-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-20 18:36:00.751809 market_generic-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-20 18:35:46.000000 market_generic-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/market_generic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 18:36:00.000000 market_generic-0.0.1/market_generic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 18:35:46.000000 market_generic-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 18:36:00.751809 market_generic-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-20 18:35:46.000000 market_generic-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.747809 market_generic-0.0.1/trade/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.747809 market_generic-0.0.1/trade/calendar/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/calendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/calendar/calendar_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/calendar/calendar_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/trade/nse/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/nse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/nse/nse_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/nse/nse_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/trade/ticker/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/market.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/stock_generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/ticker/yf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 18:36:00.751809 market_generic-0.0.1/trade/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/df_market_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/gsheet_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/log_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/network_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/op_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-20 18:35:46.000000 market_generic-0.0.1/trade/utils/telegram_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.096953 market_generic-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-26 16:23:11.096953 market_generic-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-26 16:22:57.000000 market_generic-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.096953 market_generic-0.1.0/market_generic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-26 16:23:11.000000 market_generic-0.1.0/market_generic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-26 16:22:57.000000 market_generic-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 16:23:11.096953 market_generic-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-26 16:22:57.000000 market_generic-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/calendar/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/calendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/calendar/calendar_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/calendar/calendar_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/nse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/nse_all_stocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/nse_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/nse/nse_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.092953 market_generic-0.1.0/trade/ticker/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/market.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/stock_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/ticker/yf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 16:23:11.096953 market_generic-0.1.0/trade/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/df_market_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/gsheet_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/html_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/log_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/network_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/op_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-26 16:22:57.000000 market_generic-0.1.0/trade/utils/telegram_api.py
```

### Comparing `market_generic-0.0.1/PKG-INFO` & `market_generic-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-generic
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Generic Python Package for Stock Market Analysis and Trading
 Home-page: https://github.com/sharmasourab93/market-generic
 Author: Sourab S Sharma
 Author-email: sharmasourab93@gmail.com
 Keywords: Market,Trade,Analysis
 Description-Content-Type: text/markdown
 Requires-Dist: black==24.4.2
@@ -14,14 +14,16 @@
 Requires-Dist: dateutils==0.6.12
 Requires-Dist: gspread==6.1.0
 Requires-Dist: python-telegram-bot==21.1.1
 Requires-Dist: yfinance==0.2.38
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pytz~=2024.1
 Requires-Dist: setuptools~=69.5.1
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: openpyxl==3.1.2
 
 # market-generic - A Generic Python Package for Stock Market Analysis and Trading
 
 ### Overview
 
 `market-generic` is a powerful and flexible Python library designed to simplify the process of working with stock market data. It provides a comprehensive set of tools and utilities to handle, analyze, and visualize stock data, enabling developers and analysts to build dynamic stock scanners, trading strategies, and other financial applications with ease.
```

### Comparing `market_generic-0.0.1/README.md` & `market_generic-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/market_generic.egg-info/PKG-INFO` & `market_generic-0.1.0/market_generic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-generic
-Version: 0.0.1
+Version: 0.1.0
 Summary: A Generic Python Package for Stock Market Analysis and Trading
 Home-page: https://github.com/sharmasourab93/market-generic
 Author: Sourab S Sharma
 Author-email: sharmasourab93@gmail.com
 Keywords: Market,Trade,Analysis
 Description-Content-Type: text/markdown
 Requires-Dist: black==24.4.2
@@ -14,14 +14,16 @@
 Requires-Dist: dateutils==0.6.12
 Requires-Dist: gspread==6.1.0
 Requires-Dist: python-telegram-bot==21.1.1
 Requires-Dist: yfinance==0.2.38
 Requires-Dist: requests~=2.31.0
 Requires-Dist: pytz~=2024.1
 Requires-Dist: setuptools~=69.5.1
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: openpyxl==3.1.2
 
 # market-generic - A Generic Python Package for Stock Market Analysis and Trading
 
 ### Overview
 
 `market-generic` is a powerful and flexible Python library designed to simplify the process of working with stock market data. It provides a comprehensive set of tools and utilities to handle, analyze, and visualize stock data, enabling developers and analysts to build dynamic stock scanners, trading strategies, and other financial applications with ease.
```

### Comparing `market_generic-0.0.1/market_generic.egg-info/SOURCES.txt` & `market_generic-0.1.0/market_generic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 market_generic.egg-info/requires.txt
 market_generic.egg-info/top_level.txt
 trade/__init__.py
 trade/calendar/__init__.py
 trade/calendar/calendar_data.py
 trade/calendar/calendar_tool.py
 trade/nse/__init__.py
+trade/nse/nse_all_stocks.py
 trade/nse/nse_config.py
 trade/nse/nse_stock.py
 trade/ticker/__init__.py
 trade/ticker/api_config.py
 trade/ticker/market.py
 trade/ticker/stock_generics.py
 trade/ticker/yf.py
 trade/utils/__init__.py
 trade/utils/df_market_utils.py
 trade/utils/gsheet_util.py
+trade/utils/html_parsing.py
 trade/utils/log_configurator.py
 trade/utils/network_tools.py
 trade/utils/op_utils.py
 trade/utils/telegram_api.py
```

### Comparing `market_generic-0.0.1/setup.py` & `market_generic-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 NAME = "market-generic"
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 DESCRITPION = "A Generic Python Package for Stock Market Analysis and Trading"
 URL = "https://github.com/sharmasourab93/market-generic"
 AUTHOR = "Sourab S Sharma"
 EMAIL = "sharmasourab93@gmail.com"
 
 with open("README.md", "r") as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `market_generic-0.0.1/trade/calendar/calendar_data.py` & `market_generic-0.1.0/trade/calendar/calendar_data.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/calendar/calendar_tool.py` & `market_generic-0.1.0/trade/calendar/calendar_tool.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/nse/nse_config.py` & `market_generic-0.1.0/trade/nse/nse_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Sequence
 from dataclasses import dataclass, field
 from datetime import date, datetime, time
-from functools import cached_property
+from functools import cache, cached_property
 from io import BytesIO
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 import pandas as pd
 import requests
 from yfinance import Ticker
@@ -15,56 +15,85 @@
     MarketHolidayType,
     MarketTimings,
     MarketTimingType,
     WorkingDayDate,
 )
 from trade.ticker import Exchange, ExchangeArgs
 from trade.utils import LoggingType, operations
+from trade.utils.network_tools import CustomHTTPException
 
 DATE_FMT = "%d-%b-%Y"
 TODAY = datetime.today().date().strftime(DATE_FMT)
 TZ = "Asia/Kolkata"
 CONFIG_FILE = Path(__file__).parent.parent.parent / Path("configs/nse.json")
 NSE_START_TIME, NSE_CLOSE_TIME, TIME_CUTOFF = "0915", "1530", "1600"
 MARKET, COUNTRY = "NSE", "INDIA"
 HOLIDAYS_DONOT_EXIST = "Holiday key or holidays do not exist"
 MARKET_API_QUOTE_TYPE = Dict[str, Union[list, str, bool]]
+NSE_TOP = 1000
 TIMINGS = MarketTimings(
     start_time=NSE_START_TIME,
     close_time=NSE_CLOSE_TIME,
     time_zone=TZ,
     time_cutoff=TIME_CUTOFF,
 )
 
 
 class NSEConfig(Exchange):
 
+    def __init__(
+        self,
+        today: str,
+        date_fmt: str = DATE_FMT,
+        config: Union[Path, str] = CONFIG_FILE,
+        market: str = MARKET,
+        country: str = COUNTRY,
+        market_timings: MarketTimingType = TIMINGS,
+        ticker_mod: Optional[Dict[str, str]] = None,
+        log_config: Optional[LoggingType] = None,
+    ):
+
+        super().__init__(
+            today,
+            date_fmt,
+            config,
+            market,
+            country,
+            self.get_market_holidays,
+            market_timings,
+            ticker_mod,
+            log_config,
+        )
+
     @property
     def advanced_header(self) -> Dict[str, str]:
         return self.headers["advanced"]
 
     @property
-    def holiday_url(self) -> str:
+    def simple_headers(self) -> Dict[str, str]:
+        return self.headers["simple"]
 
+    @property
+    def holiday_url(self) -> str:
         return self.main_domain + self.trading
 
+    def replace_holiday_keywords(self, holiday: dict):
+        holiday["trade_day"] = holiday.pop("tradingDate")
+        holiday["week_day"] = holiday.pop("weekDay")
+        _ = holiday.pop("Sr_no")
+        return holiday
+
     def get_market_holidays(self, holiday_key: str = "CM") -> List[MarketHolidayType]:
         response = self.get_request_api(self.holiday_url, self.advanced_header)
         content = response.json().get(holiday_key, None)
 
         if content is None:
             raise KeyError(HOLIDAYS_DONOT_EXIST)
 
-        def replace_holiday_keywords(holiday: dict):
-            holiday["trade_day"] = holiday.pop("tradingDate")
-            holiday["week_day"] = holiday.pop("weekDay")
-            _ = holiday.pop("Sr_no")
-            return holiday
-
-        content = [replace_holiday_keywords(i) for i in content]
+        content = [self.replace_holiday_keywords(i) for i in content]
 
         return content
 
     def get_equity_meta(self, symbol: str) -> MARKET_API_QUOTE_TYPE:
         symbol = symbol.upper()
         url = self.main_domain + self.equity_meta
         url = url.format(symbol)
@@ -99,42 +128,70 @@
         url = self.eq_bhavcopy["url"] + self.eq_bhavcopy["url_params"]
         today = self.working_day.day.as_str
         url = url.format(today)
         result = self.download_data(url, headers)
 
         return result
 
+    def process_mcap_file(self, data: pd.DataFrame) -> pd.DataFrame:
+
+        data.columns = ["sr_no", "symbol", "company_name", "market_cap"]
+        data = data.loc[~data.sr_no.isna(), :]
+        data = data[pd.to_numeric(data.sr_no, errors="coerce").notnull()]
+        data.sr_no = data.sr_no.astype(int)
+        data.loc[:, "market_cap"] = pd.to_numeric(data.market_cap, errors="coerce")
+        data = data.loc[~data.market_cap.isna(), :]
+        # Since the values are in Lakhs, we are making it to crores.
+        data.loc[:, "market_cap"] = data.market_cap / 100
+
+        return data
+
+    def get_mcap_file_url(self) -> str:
+        url = self.main_domain + self.market_cap["page"]
+        tags = tuple(self.market_cap["tags"])
+        return self.parse_through_html(url, self.advanced_header, tags)
+
+    @cache
+    def get_mcap(self) -> pd.DataFrame:
+        url = self.get_mcap_file_url()
+
+        try:
+            content = self.download_data(url, self.advanced_header)
+        except CustomHTTPException:
+            content = self.download_data(url, self.simple_headers)
+
+        content = self.process_mcap_file(content)
+        return content
+
+    def apply_mcap(self, data: pd.DataFrame) -> pd.DataFrame:
+        mcap = self.get_mcap()
+        data = pd.merge(mcap, data, how="left")
+
+        return data
+
     def apply_nse_data_preprocessing(self, data) -> pd.DataFrame:
         data = data.loc[:, ~data.columns.str.contains("^Unnamed")]
         data.columns = [i.lower() for i in data.columns]
         data = data.loc[data.series == "EQ", :]
-        # TODO: NSE Market Capitalization to be applied.
+        data = self.apply_mcap(data)
         return data
 
     def get_eq_listed_stocks(self) -> List[str]:
         data = self.get_eq_bhavcopy()
         data = self.apply_nse_data_preprocessing(data)
         return data.symbol.unique().tolist()
 
-    def __init__(
-        self,
-        today: str,
-        date_fmt: str = DATE_FMT,
-        config: Union[Path, str] = CONFIG_FILE,
-        market: str = MARKET,
-        country: str = COUNTRY,
-        market_timings: MarketTimingType = TIMINGS,
-        ticker_mod: Optional[Dict[str, str]] = None,
-        log_config: Optional[LoggingType] = None,
-    ):
+    def get_eq_stocks_by_mcap(self) -> pd.DataFrame:
 
-        super().__init__(
-            today,
-            date_fmt,
-            config,
-            market,
-            country,
-            self.get_market_holidays,
-            market_timings,
-            ticker_mod,
-            log_config,
-        )
+        data = self.get_eq_bhavcopy()
+        data = self.apply_nse_data_preprocessing(data)
+
+        return data
+
+    def get_nse_stocks(self, nse_top: Optional[int] = None) -> List[str]:
+
+        stock_list = self.get_eq_listed_stocks()
+
+        if nse_top is None:
+            return stock_list
+
+        return stock_list[:nse_top]
```

### Comparing `market_generic-0.0.1/trade/nse/nse_stock.py` & `market_generic-0.1.0/trade/nse/nse_stock.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,95 +1,109 @@
+import json
+from collections import Counter
 from dataclasses import dataclass, field
+from datetime import date, datetime
 from functools import cached_property
 from typing import Dict, List, Optional, Union
 from warnings import simplefilter
 
 import pandas as pd
 from yfinance import Ticker
 
 from trade.calendar import DateObj
-from trade.nse.nse_config import DATE_FMT, NSEConfig
+from trade.nse.nse_config import DATE_FMT, NSE_TOP, NSEConfig
 from trade.ticker import StockGenerics
 from trade.utils import operations
 
 MARKET_API_QUOTE_TYPE = Dict[str, Union[list, str, bool]]
-
+TICKER_MODIFICATION = {"HDFC": "HDFCBANK"}
 simplefilter(action="ignore", category=pd.errors.SettingWithCopyWarning)
 simplefilter(action="ignore", category=RuntimeWarning)
 
 
 @dataclass
-class AllNSEStocks:
-
-    dated: str
-    symbols: Optional[List[str]] = None
-
-    def __post_init__(self):
-        self._nse_config = NSEConfig(self.dated)
-        if self.symbols is None:
-            self.symbols = self._nse_config.get_eq_listed_stocks()
-
-        self.symbols = [NSEStock(i, self.dated) for i in self.symbols]
-
-
-@dataclass
 class NSEStock(StockGenerics):
     symbol: str
     dated: str
     tf: Optional[str] = "1d"
 
     def __post_init__(self):
         self._nse_config = NSEConfig(self.dated)
+
+        if self.symbol in TICKER_MODIFICATION.keys():
+            self.symbol = TICKER_MODIFICATION[self.symbol]
+
         self._yfsymbol = self._nse_config.adjust_yfin_ticker_by_market(self.symbol)
         self.get_curr_bhav()
-        self.curr_ohlc = {
+        self._curr_ohlc = {
             "open": self.open,
             "low": self.low,
             "high": self.high,
             "close": self.close,
+            "diff": self.diff,
             "prev_close": self.prev_close,
             "pct_change": self.pct_change,
             "volume": self.volume,
             "prev_volume": self.prev_volume,
             "volume_diff": self.volume_diff,
         }
 
+    @property
+    def ohlc(self):
+        return self._curr_ohlc
+
     def __str__(self):
         return self.symbol
 
     def __eq__(self, other):
-
         return self.symbol == other
 
     @cached_property
     def get_meta_data(self) -> MARKET_API_QUOTE_TYPE:
         return self._nse_config.get_equity_meta(self.symbol)
 
     @property
-    def get_ticker(self) -> Ticker:
+    def ticker(self) -> Ticker:
         return self._nse_config.yf.Ticker(self._yfsymbol)
 
+    @property
+    def adv_dec(self):
+
+        match self.diff:
+
+            case self.diff if self.diff > 0:
+                return True
+
+            case self.diff if self.diff < 0:
+                return Fals
+
+            case _:
+                return None
+
     def get_curr_bhav(self):
         curr_date = DateObj(self.dated, date_fmt=DATE_FMT)
         start_date = curr_date - 2
         end_date = curr_date + 1
         result = self._nse_config.get_period_data(
             self.symbol,
             start=start_date.as_date,
             end=end_date.as_date,
             interval=self.tf,
         )
-        print(self.symbol)
-        self.prev_volume = result.iloc[-2]["volume"]
+        try:
+            self.prev_volume = result.iloc[-2]["volume"]
+        except IndexError:
+            print()
         (
             _,
             self.open,
             self.high,
             self.low,
             self.close,
             self.volume,
             self.prev_close,
             self.pct_change,
         ) = result.iloc[-1]
         self.volume_diff = (
             operations.calculate_pct_diff(self.volume, self.prev_volume) / 100
         )
+        self.diff = self.close - self.prev_close
```

### Comparing `market_generic-0.0.1/trade/ticker/api_config.py` & `market_generic-0.1.0/trade/ticker/api_config.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/ticker/market.py` & `market_generic-0.1.0/trade/ticker/market.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/ticker/stock_generics.py` & `market_generic-0.1.0/trade/ticker/stock_generics.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/ticker/yf.py` & `market_generic-0.1.0/trade/ticker/yf.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/utils/df_market_utils.py` & `market_generic-0.1.0/trade/utils/df_market_utils.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/utils/gsheet_util.py` & `market_generic-0.1.0/trade/utils/gsheet_util.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/utils/log_configurator.py` & `market_generic-0.1.0/trade/utils/log_configurator.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/utils/network_tools.py` & `market_generic-0.1.0/trade/utils/network_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 import csv
 import os
 from abc import ABC
 from io import BytesIO
-from typing import Optional
+from typing import Optional, Tuple
 from urllib.error import HTTPError
 from urllib.parse import urlparse
 from zipfile import ZipFile
 
 import requests
 from pandas import DataFrame, read_csv, read_excel
 from requests import Session
 from requests.exceptions import ConnectionError, InvalidURL, ReadTimeout
 
+from trade.utils.html_parsing import HtmlParser
+
 CHUNK_SIZE = 1024
 INVALID_URL = "URL: {0}, Status Code:{1}"
 RECEIVED_STATUS = "Status Code Received: {0}"
+UNKNOWN_CONTENT = "Unknown Content type."
+
 
+class CustomHTTPException(Exception):
+    pass
 
-def match_http(result, status_code: int, url: Optional[str] = None):
-    msg = ""
-    match status_code:
-        case 200:
-            return result
-
-        case 404:
-            raise InvalidURL(INVALID_URL.format(url, result.status_code))
-
-        case 403:
-            msg = RECEIVED_STATUS.format(status_code)
-            if url is not None:
-                msg += ". For url: {0}".format(url)
 
-            raise Exception(msg)
+class DownloadTools(ABC):
 
-        case _:
-            raise Exception(RECEIVED_STATUS.format(status_code))
+    def match_http(self, result, status_code: int, url: Optional[str] = None):
+        msg = ""
+        match status_code:
+            case 200:
+                return result
 
+            case 404:
+                raise InvalidURL(INVALID_URL.format(url, result.status_code))
+
+            case 403:
+                msg = RECEIVED_STATUS.format(status_code)
+                if url is not None:
+                    msg += ". For url: {0}".format(url)
+
+                raise CustomHTTPException(msg)
+
+            case _:
+                raise CustomHTTPException(RECEIVED_STATUS.format(status_code))
+
+    def parse_through_html(self, url: str, headers: dict, tags: Tuple[str]) -> str:
+
+        html_parser = HtmlParser(url, headers, tags)
+
+        return html_parser.get_latest_file()
 
-class DownloadTools(ABC):
     def get_cookies(self, base_url: str, headers: dict, timeout: int = 5) -> dict:
 
         url = self.extract_domain(base_url)
 
         session = Session()
         try:
             request = session.get(url, headers=headers, timeout=timeout)
 
         except (ConnectionError, ReadTimeout) as msg:
-            self.logger.debug(msg)
             return self.get_cookies(url, headers)
 
         return dict(request.cookies)
 
     def get_request_api(
         self, url: str, headers: dict, cookies: Optional[dict] = None, **kwargs
     ):
 
         cookies = self.get_cookies(url, headers)
         result = requests.get(url, headers=headers, cookies=cookies, **kwargs)
-        return match_http(result, result.status_code, url)
+        return self.match_http(result, result.status_code, url)
 
     def extract_domain(self, url: str) -> str:
         parsed_url = urlparse(url)
         domain = parsed_url.netloc
 
         return "https://" + domain
 
     def get_headers(self, url):
-
         return requests.head(url)
 
     def download_data(self, url: str, headers: Optional[str] = None) -> DataFrame:
         """
         For a given url and file name
         download data to the provided filename/path.
         """
@@ -80,15 +91,18 @@
         response = self.get_request_api(url, headers, cookies)
 
         bytes_obj = BytesIO(response.content)
 
         if self.is_zip(bytes_obj):
             bytes_obj = self.unzip(bytes_obj)
 
-        result = self.read_from_buffer(bytes_obj)
+        try:
+            result = self.read_from_buffer(bytes_obj)
+        except ValueError:
+            result = self.read_from_buffer(response.content)
 
         return result
 
     def unzip(self, source_buffer: BytesIO) -> bytes:
         """
         Extracts content of the zip file and
         returns a reference to the extracted CSV file.
@@ -106,35 +120,40 @@
         zip_signature = b"PK\x03\x04"
 
         return byte_obj.getvalue().startswith(zip_signature)
 
     def is_xlsx(self, byte_obj: BytesIO) -> bool:
         xlsx_signature = b"PK\x03\x04"
 
-        return byte_obj.startswith(xlsx_signature)
+        if hasattr(byte_obj, "startswith"):
+            return byte_obj.startswith(xlsx_signature)
+
+        return False
 
     def is_csv(self, byte_obj: BytesIO):
         try:
             content = byte_obj.getvalue().decode("utf-8")
             dialect = csv.Sniffer().sniff(content)
             # TODO: Handle _csv.Error here.
             return True
 
-        except (UnicodeDecodeError, csv.Error):
+        except (UnicodeDecodeError, csv.Error, AttributeError):
             return False
 
     def read_csv(self, bytes_obj: BytesIO) -> DataFrame:
         return read_csv(bytes_obj)
 
     def read_xlsx(self, bytes_obj: BytesIO) -> DataFrame:
-        return read_excel(bytes_obj)
+        try:
+            return read_excel(bytes_obj)
+        except ValueError:
+            return read_excel(bytes_obj, engine="openpyxl")
 
     def read_from_buffer(self, bytes_obj: BytesIO):
         if self.is_csv(bytes_obj):
             return self.read_csv(bytes_obj)
 
         elif self.is_xlsx(bytes_obj):
             return self.read_xlsx(bytes_obj)
 
         else:
-            # TODO: Handle this case if need arises.
-            pass
+            raise ValueError(UNKNOWN_CONTENT)
```

### Comparing `market_generic-0.0.1/trade/utils/op_utils.py` & `market_generic-0.1.0/trade/utils/op_utils.py`

 * *Files identical despite different names*

### Comparing `market_generic-0.0.1/trade/utils/telegram_api.py` & `market_generic-0.1.0/trade/utils/telegram_api.py`

 * *Files identical despite different names*

