# Comparing `tmp/tinyticker-0.7.4.tar.gz` & `tmp/tinyticker-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.7.4.tar", max compression
+gzip compressed data, was "tinyticker-0.7.5.tar", max compression
```

## Comparing `tinyticker-0.7.4.tar` & `tinyticker-0.7.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1068 2024-05-25 17:14:32.547655 tinyticker-0.7.4/LICENSE
--rw-r--r--   0        0        0     3955 2024-05-25 17:14:32.547655 tinyticker-0.7.4/README.md
--rw-r--r--   0        0        0      917 2024-05-25 17:14:32.547655 tinyticker-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      518 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/__init__.py
--rw-r--r--   0        0        0     4712 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/config.py
--rw-r--r--   0        0        0     4813 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/display.py
--rw-r--r--   0        0        0     5247 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/layouts.py
--rw-r--r--   0        0        0      345 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/paths.py
--rw-r--r--   0        0        0     5483 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2584 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1558 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     8428 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/command.py
--rw-r--r--   0        0        0      593 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/startup.py
--rw-r--r--   0        0        0   274777 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    14743 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2449 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     3173 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/startup.html
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-25 21:05:00.960920 tinyticker-0.7.5/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-25 21:05:00.960920 tinyticker-0.7.5/README.md
+-rw-r--r--   0        0        0      917 2024-05-25 21:05:00.960920 tinyticker-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      518 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/__init__.py
+-rw-r--r--   0        0        0     4712 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/config.py
+-rw-r--r--   0        0        0     4803 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/display.py
+-rw-r--r--   0        0        0     5315 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/layouts.py
+-rw-r--r--   0        0        0      345 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/paths.py
+-rw-r--r--   0        0        0     5483 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     3583 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1558 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-25 21:05:00.964920 tinyticker-0.7.5/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     8428 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/command.py
+-rw-r--r--   0        0        0      593 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14743 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     3173 2024-05-25 21:05:00.968920 tinyticker-0.7.5/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.5/PKG-INFO
```

### Comparing `tinyticker-0.7.4/LICENSE` & `tinyticker-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/README.md` & `tinyticker-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/pyproject.toml` & `tinyticker-0.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.7.4"
+version = "0.7.5"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.7.4/tinyticker/__init__.py` & `tinyticker-0.7.5/tinyticker/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/__main__.py` & `tinyticker-0.7.5/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/config.py` & `tinyticker-0.7.5/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/display.py` & `tinyticker-0.7.5/tinyticker/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         flip: bool = False,
     ) -> None:
         self._log = logging.getLogger(__name__)
         self.flip = flip
         self.epd = epd
         self.has_highlight = isinstance(self.epd, EPDHighlight)
         self.init_epd()
-        self.layout = LAYOUTS["default"]
 
     def init_epd(self):
         """Initialize the ePaper display module."""
         self._log.info("Init ePaper display.")
         self.epd.init()
         self.epd.Clear()
 
@@ -123,9 +122,10 @@
         # I think this wakes it from sleep
         self.epd.init()
         self._show_image(image, highlight_image)
         self._log.info("Display sleep.")
         self.epd.sleep()
 
     def show(self, ticker: TickerBase, resp: TickerResponse) -> None:
-        image = self.layout.func((self.epd.height, self.epd.width), ticker, resp)
+        layout = LAYOUTS["default"]
+        image = layout.func((self.epd.height, self.epd.width), ticker, resp)
         self.show_image(image)
```

### Comparing `tinyticker-0.7.4/tinyticker/layouts.py` & `tinyticker-0.7.5/tinyticker/layouts.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,32 @@
 They should not care about the capabilities of the display device, only about the content to display.
 """
 
 import dataclasses as dc
 import logging
 from typing import Callable, Optional, Tuple
 
-import matplotlib as mpl
 import matplotlib.pyplot as plt
 import mplfinance as mpf
 import numpy as np
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from PIL import Image
 
 from .tickers._base import TickerBase, TickerResponse
 
-mpl.use("Agg")
-
 MARKETCOLORS = mpf.make_marketcolors(
     up="white",
     down="black",
     edge="black",
     wick="black",
     ohlc="black",
     volume="black",
 )
 MARKETCOLORS["vcedge"] = {"up": "black", "down": "black"}
-# STYLE = mpf.make_mpf_style(marketcolors=MARKETCOLORS, mavcolors=["k"])
 STYLE = mpf.make_mpf_style(marketcolors=MARKETCOLORS, mavcolors=["r"])
 TEXT_BBOX = {
     "boxstyle": "square,pad=0",
     "facecolor": "white",
     "edgecolor": "white",
 }
 LAYOUTS = {}
@@ -142,53 +138,58 @@
 
     # if incomplete data, leave space for the missing data
     if len(resp.historical) < ticker.lookback:
         # the floats are to leave padding left and right of the edge candles
         kwargs["xlim"] = (-0.75, ticker.lookback - 0.25)
 
     if ticker.config.volume:
-        fig, axes = _create_fig_ax(
+        fig, (ax, volume_ax) = _create_fig_ax(
             dimensions, n_axes=2, gridspec_kw={"height_ratios": [3, 1]}
         )
-        volume_ax = axes[1]
     else:
-        fig, axes = _create_fig_ax(dimensions, n_axes=1)
+        fig, (ax,) = _create_fig_ax(dimensions, n_axes=1)
         volume_ax = False
-    ax: Axes = axes[0]
-    # remove Nones, it doesn't play well with mplfinance
+    ax: Axes
+    volume_ax: Axes | bool
     mpf.plot(
         resp.historical,
         type=ticker.config.plot_type,
         ax=ax,
         update_width_config={"line_width": 1},
         style=STYLE,
         volume=volume_ax,
         linecolor="k",
         **kwargs,
     )
 
-    # Fall back to using the last closing price
-    if top_string is None:
-        top_string = str(resp.historical["Close"].iloc[-1])
-
-    ax.text(
+    top_text = ax.text(
         0,
         1,
         top_string,
         transform=ax.transAxes,
         fontsize=10,
         weight="bold",
         bbox=TEXT_BBOX,
+        verticalalignment="top",
+    )
+    ax_height = ax.get_position().height * dimensions[1]
+    ax.text(
+        0,
+        (ax_height - top_text.get_window_extent().height + 1) / ax_height,
+        sub_string,
+        transform=ax.transAxes,
+        fontsize=8,
+        weight="bold",
+        bbox=TEXT_BBOX,
+        verticalalignment="top",
     )
-    if sub_string is not None:
-        ax.text(
-            0,
-            0.88,
-            sub_string,
-            transform=ax.transAxes,
-            fontsize=8,
-            weight="bold",
-            bbox=TEXT_BBOX,
+    gaps = resp.historical.index.to_series().diff()
+    large_gaps = np.arange(0, len(gaps))[gaps > gaps.median()]
+    for gap in large_gaps:
+        ax.axvline(
+            gap - 0.5,
+            color="black",
+            linestyle=":",
+            linewidth=1,
         )
-    fig.tight_layout(pad=0)
 
     return _fig_to_image(fig)
```

### Comparing `tinyticker-0.7.4/tinyticker/sequence.py` & `tinyticker-0.7.5/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/tickers/__init__.py` & `tinyticker-0.7.5/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/tickers/_base.py` & `tinyticker-0.7.5/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/tickers/crypto.py` & `tinyticker-0.7.5/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/tickers/stock.py` & `tinyticker-0.7.5/tinyticker/tickers/stock.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,14 +36,30 @@
         start -= pd.to_timedelta("2d") * (end.week - start.week) * 1.5
         # go back before weekend
         # start.weekday() returns 6 for Sunday, and 5 for Saturday
         # max(0, start.weekday() - 4) is 0 for Mon-Fri, 1 for Sat, 2 for Sun
         start -= pd.to_timedelta("1d") * max(0, start.weekday() - 4)
         return (start, end)
 
+    def _fix_prepost(self, historical: pd.DataFrame) -> pd.DataFrame:
+        # when the market is closed, the volume is 0
+        prepost_range = historical["Volume"] == 0
+        # When in prepost, the high & lows can be off
+        to_correct_high = (
+            historical["High"].diff()[prepost_range] > historical["High"].std()
+        )
+        to_correct_low = (
+            historical["Low"].diff()[prepost_range]
+            < historical["Low"].mean() - historical["Low"].std()
+        )
+        # we could also set them to the avg of the previous and next high/low
+        historical.loc[prepost_range & to_correct_high, "High"] = historical["Close"]
+        historical.loc[prepost_range & to_correct_low, "Low"] = historical["Close"]
+        return historical
+
     def _single_tick(self) -> Tuple[pd.DataFrame, Optional[float]]:
         LOGGER.info("Stock tick: %s", self.config.symbol)
         start, end = self._get_yfinance_start_end()
         current_price: Optional[float] = self._yf_ticker.fast_info.get(
             "lastPrice", None
         )
         historical = self._yf_ticker.history(
@@ -58,8 +74,12 @@
                 f"No historical data returned from yfinance API for {self.config.symbol}."
             )
         # drop the extra data
         if len(historical) > self.lookback:
             historical = historical.iloc[-self.lookback :]
         if historical.index.tzinfo is None:  # type: ignore
             historical.index = historical.index.tz_localize("utc")  # type: ignore
+        if self.config.prepost:
+            # yfinance gives some weird data for the high/low values during the pre/post market
+            # hours, so we hide very them
+            historical = self._fix_prepost(historical)
         return (historical, current_price)
```

### Comparing `tinyticker-0.7.4/tinyticker/utils.py` & `tinyticker-0.7.5/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/device.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/waveshare_lib/models.py` & `tinyticker-0.7.5/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/__main__.py` & `tinyticker-0.7.5/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/app.py` & `tinyticker-0.7.5/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/command.py` & `tinyticker-0.7.5/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/startup.py` & `tinyticker-0.7.5/tinyticker/web/startup.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.7.5/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.7.5/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.7.5/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.7.5/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/index.html` & `tinyticker-0.7.5/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/js/index.js` & `tinyticker-0.7.5/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.7.5/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.7.5/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/logfiles.html` & `tinyticker-0.7.5/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/tinyticker/web/templates/startup.html` & `tinyticker-0.7.5/tinyticker/web/templates/startup.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.4/PKG-INFO` & `tinyticker-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.7.4
+Version: 0.7.5
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.7.4 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.7.5 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

