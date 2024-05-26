# Comparing `tmp/mptradelib-0.5.8.tar.gz` & `tmp/mptradelib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.5.8.tar", max compression
+gzip compressed data, was "mptradelib-0.5.9.tar", max compression
```

## Comparing `mptradelib-0.5.8.tar` & `mptradelib-0.5.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.8/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.8/mptradelib/__init__.py
--rw-r--r--   0        0        0     4786 2024-05-25 17:34:22.689097 mptradelib-0.5.8/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.8/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11072 2024-05-25 17:30:54.602294 mptradelib-0.5.8/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.8/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.8/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.8/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.8/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.8/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.8/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.8/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.8/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.8/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.8/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.8/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     8569 2024-05-23 19:20:16.364263 mptradelib-0.5.8/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.8/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.8/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0     1316 2024-05-25 17:35:22.328037 mptradelib-0.5.8/mptradelib/utils/downloader.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.8/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0    10818 2024-05-24 03:38:04.967978 mptradelib-0.5.8/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.8/mptradelib/utils/utils.py
--rw-r--r--   0        0        0        0 2024-05-23 19:19:31.018101 mptradelib-0.5.8/mptradelib/widgets/__init__.py
--rw-r--r--   0        0        0     2005 2024-05-23 19:19:52.537757 mptradelib-0.5.8/mptradelib/widgets/daterangepicker.py
--rw-r--r--   0        0        0      822 2024-05-25 17:35:29.870447 mptradelib-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.9/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4786 2024-05-25 17:34:22.689097 mptradelib-0.5.9/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.9/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11072 2024-05-25 17:30:54.602294 mptradelib-0.5.9/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.9/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.9/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.9/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.9/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.9/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.9/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.9/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.9/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.9/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.9/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.9/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     8569 2024-05-23 19:20:16.364263 mptradelib-0.5.9/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.9/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.9/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0     3163 2024-05-25 20:40:51.738596 mptradelib-0.5.9/mptradelib/utils/chart.py
+-rw-r--r--   0        0        0     1316 2024-05-25 17:35:22.328037 mptradelib-0.5.9/mptradelib/utils/downloader.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.9/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0    11002 2024-05-25 20:40:16.840750 mptradelib-0.5.9/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.9/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:19:31.018101 mptradelib-0.5.9/mptradelib/widgets/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-23 19:19:52.537757 mptradelib-0.5.9/mptradelib/widgets/daterangepicker.py
+-rw-r--r--   0        0        0      822 2024-05-25 20:40:58.170818 mptradelib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.9/PKG-INFO
```

### Comparing `mptradelib-0.5.8/README.md` & `mptradelib-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/backtest.py` & `mptradelib-0.5.9/mptradelib/backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/broker/broker.py` & `mptradelib-0.5.9/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/broker/session.py` & `mptradelib-0.5.9/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/broker/shoonya.py` & `mptradelib-0.5.9/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/broker/ticker.py` & `mptradelib-0.5.9/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/cli/new.py` & `mptradelib-0.5.9/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5.9/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5.9/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5.9/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/feed.py` & `mptradelib-0.5.9/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/livetrade.py` & `mptradelib-0.5.9/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/optimizers/walkforward.py` & `mptradelib-0.5.9/mptradelib/optimizers/walkforward.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/test_renko.py` & `mptradelib-0.5.9/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/utils/downloader.py` & `mptradelib-0.5.9/mptradelib/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5.9/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/utils/tearsheet.py` & `mptradelib-0.5.9/mptradelib/utils/tearsheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import pandas as pd
 import numpy as np
 from .simulated_trades import SimulateTrades
-import pydantic as pyd
-from typing import List
 import datetime as dt
+from .chart import *
 try:
     from plotly.subplots import make_subplots
     import plotly.graph_objects as go
     import plotly.express as px
 except ImportError:
     print("please install plotly by 'pip install plotly' to enable plotting")
 
-class Line(pyd.BaseModel):
-    colname: str
-    name: str = None
-    overlay: bool = True
 
 class Tearsheet:
     chart_fig: go.Figure = None
 
     def __init__(self, result: pd.DataFrame, seed=10000, leverage=1) -> None:
         self.df = result
         self._seed = seed
@@ -221,69 +216,73 @@
 
     def _get_holidays(self, dates):
         start = dates.head(1).iloc[0].date()
         end = dates.tail(1).iloc[0].date()
         date_range = pd.date_range(start, end).difference(dates)
         return list(date_range.strftime('%Y-%m-%d'))
 
+    def _get_row_heights(self, charts):
+        row_height = round(1/(len(charts) - 1 + 4), 2)
+        row_heights = [ row_height for _ in range(len(charts) - 1)]
+        return [4 * row_height] + row_heights
 
     def plot_chart(self, name, df, trades, 
                    from_date = dt.datetime.now().date(), 
                    to_date = dt.datetime.now().date() + dt.timedelta(days=1),
-                   lines: List[Line] = [], jupyter=False):
-        row_count = 1 + len([l for l in lines if not l.overlay])
-        filtered_df = df[(df.datetime.dt.date >= from_date) & (df.datetime.dt.date < to_date)]
-        filtered_trades = trades[(trades.entry_time.dt.date >= from_date) & (trades.entry_time.dt.date >= to_date)]
-
-        cs_chart = go.Candlestick(
-            x=filtered_df.datetime,
-            open=filtered_df.open,
-            high=filtered_df.high,
-            low=filtered_df.low,
-            close=filtered_df.close,
-            showlegend=False,
-            name=name,
-        )
-
-        main_trace = [cs_chart]
-        non_overlay_traces = []
-        for l in lines:
-            trace = go.Scatter(
-                x=filtered_df.datetime,
-                y=filtered_df[l.colname],
-                name=l.name,
-            )
-            
-            if l.overlay:
-                main_trace.append(trace)
-            else:
-                non_overlay_traces.append(trace)
-
-        row_height = round(1/(len(non_overlay_traces) + 4), 1)
-        row_heights = [ row_height for _ in range(len(non_overlay_traces) + 1)]
-        row_heights[0] = 4 * row_height
+                   charts: List[Chart] = [], jupyter=False):
         
         if self.chart_fig is None:
             fig = make_subplots(
-                rows=len(non_overlay_traces) + 1, 
+                rows=len(charts),
                 cols=1, 
-                subplot_titles=tuple([name] + [t.name for t in non_overlay_traces]),
-                row_heights=row_heights,
+                subplot_titles=tuple([name] + [t.name for t in charts]),
+                row_heights=self._get_row_heights(charts),
                 vertical_spacing=0.02,
                 shared_xaxes=True,
             )
             self.chart_fig = go.FigureWidget(fig) if jupyter is True else fig
         else:
             self.chart_fig.data = []
+        
+        row_count = len(charts)
+        filtered_df = df[(df.datetime.dt.date >= from_date) & (df.datetime.dt.date < to_date)]
+        filtered_trades = trades[(trades.entry_time.dt.date >= from_date) & (trades.entry_time.dt.date <= to_date)]
 
-        for t in main_trace:
-            self.chart_fig.add_trace(t, row=1, col=1)
+        cs_chart = go.Candlestick(
+            x=filtered_df.datetime,
+            open=filtered_df.open,
+            high=filtered_df.high,
+            low=filtered_df.low,
+            close=filtered_df.close,
+            showlegend=False,
+            name=name,
+        )
 
-        for i in range(len(non_overlay_traces)):
-            self.chart_fig.add_trace(non_overlay_traces[i], row=2+i, col=1)
+        self.chart_fig.add_trace(cs_chart, row=1, col=1)
+        for i in range(len(charts)):
+            chart = charts[i]
+            for c in chart.children:
+                if isinstance(c, Line):
+                    self.chart_fig.add_trace(
+                        c.get_trace(filtered_df), 
+                        row=1 if chart.main else i + 1, 
+                        col=1
+                    )
+                elif isinstance(c, Rect):
+                    self.chart_fig.add_shape(
+                        c.get_trace(filtered_df),
+                        row=1 if chart.main else i + 1, 
+                        col=1
+                    )
+                elif isinstance(c, Background):
+                    self.chart_fig.add_vrect(
+                        **c.get_trace(filtered_df), 
+                        row=1 if chart.main else i + 1, 
+                        col=1
+                    )
 
         for row in filtered_trades.itertuples():
             self.chart_fig.add_annotation(x=row.entry_time, y=row.entry_price,
                 text= "LE" if row.direction > 0 else "SE",
                 showarrow=True,
                 arrowhead=1,
                 bgcolor="#ff7f0e",
```

### Comparing `mptradelib-0.5.8/mptradelib/utils/utils.py` & `mptradelib-0.5.9/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/mptradelib/widgets/daterangepicker.py` & `mptradelib-0.5.9/mptradelib/widgets/daterangepicker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.8/pyproject.toml` & `mptradelib-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.5.8"
+version = "0.5.9"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.5.8/PKG-INFO` & `mptradelib-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.5.8
+Version: 0.5.9
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

