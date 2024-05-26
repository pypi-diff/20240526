# Comparing `tmp/pqsdk-0.0.8.tar.gz` & `tmp/pqsdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqsdk-0.0.8.tar", last modified: Wed May  8 04:11:27 2024, max compression
+gzip compressed data, was "pqsdk-0.0.9.tar", last modified: Wed May  8 04:21:25 2024, max compression
```

## Comparing `pqsdk-0.0.8.tar` & `pqsdk-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.209627 pqsdk-0.0.8/
--rw-rw-rw-   0        0        0      766 2024-05-08 04:11:27.209627 pqsdk-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.176627 pqsdk-0.0.8/pqsdk/
--rw-rw-rw-   0        0        0      190 2024-05-06 11:07:04.000000 pqsdk-0.0.8/pqsdk/__init__.py
--rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.8/pqsdk/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.191627 pqsdk-0.0.8/pqsdk/api/
--rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.8/pqsdk/api/__init__.py
--rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.8/pqsdk/api/main.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.197626 pqsdk-0.0.8/pqsdk/backtest/
--rw-rw-rw-   0        0        0     3202 2024-05-08 04:09:04.000000 pqsdk-0.0.8/pqsdk/backtest/__init__.py
--rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/backtest/analyzer.py
--rw-rw-rw-   0        0        0    35709 2024-05-07 11:11:40.000000 pqsdk-0.0.8/pqsdk/backtest/context.py
--rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.8/pqsdk/backtest/current_data.py
--rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.8/pqsdk/backtest/instrument.py
--rw-rw-rw-   0        0        0    14065 2024-05-08 03:27:07.000000 pqsdk-0.0.8/pqsdk/backtest/main.py
--rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.8/pqsdk/backtest/order.py
--rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.8/pqsdk/backtest/portfolio.py
--rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.8/pqsdk/backtest/position.py
--rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.8/pqsdk/backtest/run_info.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.198627 pqsdk-0.0.8/pqsdk/enums/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/enums/__init__.py
--rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.8/pqsdk/enums/orderStatus.py
--rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/faxconstant.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.203627 pqsdk-0.0.8/pqsdk/interface/
--rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/interface/__init__.py
--rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/interface/abstractInstrument.py
--rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.8/pqsdk/interface/abstractOrder.py
--rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/interface/abstractPortfolio.py
--rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.8/pqsdk/interface/abstractPosition.py
--rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/interface/abstractRunInfo.py
--rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/interface/abstractStrategyContext.py
--rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/interface/abstractTrader.py
--rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.8/pqsdk/interface/constant.py
--rw-rw-rw-   0        0        0     5757 2024-05-05 10:11:04.000000 pqsdk-0.0.8/pqsdk/logger.py
--rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.8/pqsdk/main.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.207627 pqsdk-0.0.8/pqsdk/utils/
--rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/utils/__init__.py
--rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/utils/dynamic_import.py
--rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/utils/file_util.py
--rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/utils/import_global_modules.py
--rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.8/pqsdk/utils/timer_factory.py
--rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.8/pqsdk/utils/value_type_util.py
--rw-rw-rw-   0        0        0      441 2024-05-08 04:11:15.000000 pqsdk-0.0.8/pqsdk/version.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.190626 pqsdk-0.0.8/pqsdk.egg-info/
--rw-rw-rw-   0        0        0      766 2024-05-08 04:11:27.000000 pqsdk-0.0.8/pqsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1193 2024-05-08 04:11:27.000000 pqsdk-0.0.8/pqsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 04:11:27.000000 pqsdk-0.0.8/pqsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-08 04:11:27.000000 pqsdk-0.0.8/pqsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      183 2024-05-08 04:11:27.000000 pqsdk-0.0.8/pqsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 04:11:27.000000 pqsdk-0.0.8/pqsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 04:11:27.210627 pqsdk-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 04:11:27.208627 pqsdk-0.0.8/tests/
--rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.8/tests/test_backtest.py
--rw-rw-rw-   0        0        0     2137 2024-05-05 08:03:23.000000 pqsdk-0.0.8/tests/test_pqsdk_api.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.799735 pqsdk-0.0.9/
+-rw-rw-rw-   0        0        0      766 2024-05-08 04:21:25.799735 pqsdk-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-04-08 07:45:14.000000 pqsdk-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.767732 pqsdk-0.0.9/pqsdk/
+-rw-rw-rw-   0        0        0      190 2024-05-06 11:07:04.000000 pqsdk-0.0.9/pqsdk/__init__.py
+-rw-rw-rw-   0        0        0     4152 2024-04-10 00:51:13.000000 pqsdk-0.0.9/pqsdk/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.780733 pqsdk-0.0.9/pqsdk/api/
+-rw-rw-rw-   0        0        0      547 2024-04-12 09:45:19.000000 pqsdk-0.0.9/pqsdk/api/__init__.py
+-rw-rw-rw-   0        0        0     1155 2024-04-12 09:39:00.000000 pqsdk-0.0.9/pqsdk/api/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.787733 pqsdk-0.0.9/pqsdk/backtest/
+-rw-rw-rw-   0        0        0     3204 2024-05-08 04:19:24.000000 pqsdk-0.0.9/pqsdk/backtest/__init__.py
+-rw-rw-rw-   0        0        0     3419 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/backtest/analyzer.py
+-rw-rw-rw-   0        0        0    35709 2024-05-07 11:11:40.000000 pqsdk-0.0.9/pqsdk/backtest/context.py
+-rw-rw-rw-   0        0        0     3213 2024-04-10 03:08:27.000000 pqsdk-0.0.9/pqsdk/backtest/current_data.py
+-rw-rw-rw-   0        0        0     6557 2024-04-10 03:08:27.000000 pqsdk-0.0.9/pqsdk/backtest/instrument.py
+-rw-rw-rw-   0        0        0    14065 2024-05-08 03:27:07.000000 pqsdk-0.0.9/pqsdk/backtest/main.py
+-rw-rw-rw-   0        0        0     3840 2024-04-09 09:28:17.000000 pqsdk-0.0.9/pqsdk/backtest/order.py
+-rw-rw-rw-   0        0        0     2687 2024-04-10 03:08:27.000000 pqsdk-0.0.9/pqsdk/backtest/portfolio.py
+-rw-rw-rw-   0        0        0     4500 2024-04-10 03:08:27.000000 pqsdk-0.0.9/pqsdk/backtest/position.py
+-rw-rw-rw-   0        0        0     2021 2024-04-10 03:08:27.000000 pqsdk-0.0.9/pqsdk/backtest/run_info.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.788732 pqsdk-0.0.9/pqsdk/enums/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/enums/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-09 09:33:02.000000 pqsdk-0.0.9/pqsdk/enums/orderStatus.py
+-rw-rw-rw-   0        0        0     8669 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/faxconstant.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.794736 pqsdk-0.0.9/pqsdk/interface/
+-rw-rw-rw-   0        0        0      589 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/interface/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/interface/abstractInstrument.py
+-rw-rw-rw-   0        0        0     2341 2024-04-09 09:27:44.000000 pqsdk-0.0.9/pqsdk/interface/abstractOrder.py
+-rw-rw-rw-   0        0        0     1347 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/interface/abstractPortfolio.py
+-rw-rw-rw-   0        0        0     1677 2024-04-20 13:04:56.000000 pqsdk-0.0.9/pqsdk/interface/abstractPosition.py
+-rw-rw-rw-   0        0        0     2652 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/interface/abstractRunInfo.py
+-rw-rw-rw-   0        0        0    18860 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/interface/abstractStrategyContext.py
+-rw-rw-rw-   0        0        0     2907 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/interface/abstractTrader.py
+-rw-rw-rw-   0        0        0     2170 2024-04-09 09:32:55.000000 pqsdk-0.0.9/pqsdk/interface/constant.py
+-rw-rw-rw-   0        0        0     5757 2024-05-05 10:11:04.000000 pqsdk-0.0.9/pqsdk/logger.py
+-rw-rw-rw-   0        0        0     1650 2024-04-10 04:31:09.000000 pqsdk-0.0.9/pqsdk/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.797735 pqsdk-0.0.9/pqsdk/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/utils/__init__.py
+-rw-rw-rw-   0        0        0     3617 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/utils/dynamic_import.py
+-rw-rw-rw-   0        0        0     1426 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/utils/file_util.py
+-rw-rw-rw-   0        0        0      368 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/utils/import_global_modules.py
+-rw-rw-rw-   0        0        0     5710 2024-04-10 03:08:27.000000 pqsdk-0.0.9/pqsdk/utils/timer_factory.py
+-rw-rw-rw-   0        0        0      780 2024-04-09 09:24:24.000000 pqsdk-0.0.9/pqsdk/utils/value_type_util.py
+-rw-rw-rw-   0        0        0      441 2024-05-08 04:20:56.000000 pqsdk-0.0.9/pqsdk/version.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.779732 pqsdk-0.0.9/pqsdk.egg-info/
+-rw-rw-rw-   0        0        0      766 2024-05-08 04:21:25.000000 pqsdk-0.0.9/pqsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1193 2024-05-08 04:21:25.000000 pqsdk-0.0.9/pqsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 04:21:25.000000 pqsdk-0.0.9/pqsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-08 04:21:25.000000 pqsdk-0.0.9/pqsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      183 2024-05-08 04:21:25.000000 pqsdk-0.0.9/pqsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 04:21:25.000000 pqsdk-0.0.9/pqsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 04:21:25.799735 pqsdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1599 2024-04-12 14:22:50.000000 pqsdk-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 04:21:25.798735 pqsdk-0.0.9/tests/
+-rw-rw-rw-   0        0        0      472 2024-04-10 08:16:28.000000 pqsdk-0.0.9/tests/test_backtest.py
+-rw-rw-rw-   0        0        0     2137 2024-05-05 08:03:23.000000 pqsdk-0.0.9/tests/test_pqsdk_api.py
```

### Comparing `pqsdk-0.0.8/PKG-INFO` & `pqsdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.8/pqsdk/__main__.py` & `pqsdk-0.0.9/pqsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/api/__init__.py` & `pqsdk-0.0.9/pqsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/api/main.py` & `pqsdk-0.0.9/pqsdk/api/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/__init__.py` & `pqsdk-0.0.9/pqsdk/backtest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     # 计算benchmark收盘价时间序列
     bchmk = results['analysis']['time_return']['bchmk_returns']
     bchmk_df = pd.DataFrame({'bchmk_returns': bchmk})
     bchmk_df.index = pd.to_datetime(bchmk_df.index)
     # 重命名benchmark的Column名称，用于Tearsheet显示
     bchmk_df = bchmk_df.rename(columns={"bchmk_returns": results['benchmark']})
-    bchmk_df = bchmk_df.loc[stats_df.index]  # 以持仓日期列表保留benchmark的记录
+    # bchmk_df = bchmk_df.loc[stats_df.index]  # 以持仓日期列表保留benchmark的记录
     bchmk_returns = bchmk_df[results['benchmark']]
 
     # tearsheet保存路径
     ts_path = Path("storage/reports")
     ts_path.mkdir(parents=True, exist_ok=True)
     time_str = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     filename = (
```

### Comparing `pqsdk-0.0.8/pqsdk/backtest/analyzer.py` & `pqsdk-0.0.9/pqsdk/backtest/analyzer.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/context.py` & `pqsdk-0.0.9/pqsdk/backtest/context.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/current_data.py` & `pqsdk-0.0.9/pqsdk/backtest/current_data.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/instrument.py` & `pqsdk-0.0.9/pqsdk/backtest/instrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/main.py` & `pqsdk-0.0.9/pqsdk/backtest/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/order.py` & `pqsdk-0.0.9/pqsdk/backtest/order.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/portfolio.py` & `pqsdk-0.0.9/pqsdk/backtest/portfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/position.py` & `pqsdk-0.0.9/pqsdk/backtest/position.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/backtest/run_info.py` & `pqsdk-0.0.9/pqsdk/backtest/run_info.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/enums/orderStatus.py` & `pqsdk-0.0.9/pqsdk/enums/orderStatus.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/faxconstant.py` & `pqsdk-0.0.9/pqsdk/faxconstant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/__init__.py` & `pqsdk-0.0.9/pqsdk/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractInstrument.py` & `pqsdk-0.0.9/pqsdk/interface/abstractInstrument.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractOrder.py` & `pqsdk-0.0.9/pqsdk/interface/abstractOrder.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractPortfolio.py` & `pqsdk-0.0.9/pqsdk/interface/abstractPortfolio.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractPosition.py` & `pqsdk-0.0.9/pqsdk/interface/abstractPosition.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractRunInfo.py` & `pqsdk-0.0.9/pqsdk/interface/abstractRunInfo.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractStrategyContext.py` & `pqsdk-0.0.9/pqsdk/interface/abstractStrategyContext.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/abstractTrader.py` & `pqsdk-0.0.9/pqsdk/interface/abstractTrader.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/interface/constant.py` & `pqsdk-0.0.9/pqsdk/interface/constant.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/logger.py` & `pqsdk-0.0.9/pqsdk/logger.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/main.py` & `pqsdk-0.0.9/pqsdk/main.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/utils/dynamic_import.py` & `pqsdk-0.0.9/pqsdk/utils/dynamic_import.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/utils/file_util.py` & `pqsdk-0.0.9/pqsdk/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/utils/timer_factory.py` & `pqsdk-0.0.9/pqsdk/utils/timer_factory.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk/utils/value_type_util.py` & `pqsdk-0.0.9/pqsdk/utils/value_type_util.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/pqsdk.egg-info/PKG-INFO` & `pqsdk-0.0.9/pqsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqsdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK for stock analysis and strategy backtest.
 Home-page: https://www.pinkquant.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 Platform: all
```

### Comparing `pqsdk-0.0.8/pqsdk.egg-info/SOURCES.txt` & `pqsdk-0.0.9/pqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/setup.py` & `pqsdk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pqsdk-0.0.8/tests/test_pqsdk_api.py` & `pqsdk-0.0.9/tests/test_pqsdk_api.py`

 * *Files identical despite different names*

