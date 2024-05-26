# Comparing `tmp/tiingo-0.8.0.tar.gz` & `tmp/tiingo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tiingo-0.8.0.tar", last modified: Sat Jul  7 17:48:20 2018, max compression
+gzip compressed data, was "dist/tiingo-0.9.0.tar", last modified: Thu Jan 31 03:45:02 2019, max compression
```

## Comparing `tiingo-0.8.0.tar` & `tiingo-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 cam        (501) staff       (20)        0 2018-07-07 17:48:20.000000 tiingo-0.8.0/
--rw-r--r--   0 cam        (501) staff       (20)    11086 2018-07-07 17:48:20.000000 tiingo-0.8.0/PKG-INFO
--rw-r--r--   0 cam        (501) staff       (20)     1072 2017-08-25 00:37:44.000000 tiingo-0.8.0/LICENSE
--rw-r--r--   0 cam        (501) staff       (20)     3966 2018-07-07 17:46:36.000000 tiingo-0.8.0/CONTRIBUTING.rst
-drwxr-xr-x   0 cam        (501) staff       (20)        0 2018-07-07 17:48:20.000000 tiingo-0.8.0/tests/
--rw-r--r--   0 cam        (501) staff       (20)     7944 2018-07-05 00:52:40.000000 tiingo-0.8.0/tests/test_tiingo.py
--rw-r--r--   0 cam        (501) staff       (20)     2283 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/test_restclient.py
--rw-r--r--   0 cam        (501) staff       (20)       61 2017-08-25 00:37:44.000000 tiingo-0.8.0/tests/__init__.py
--rw-r--r--   0 cam        (501) staff       (20)     3988 2018-07-05 00:52:40.000000 tiingo-0.8.0/tests/test_tiingo_pandas.py
--rw-r--r--   0 cam        (501) staff       (20)     2226 2018-05-01 02:54:51.000000 tiingo-0.8.0/tests/test_api_key_tools.py
-drwxr-xr-x   0 cam        (501) staff       (20)        0 2018-07-07 17:48:20.000000 tiingo-0.8.0/tests/fixtures/
--rw-r--r--   0 cam        (501) staff       (20)     1250 2018-04-21 19:58:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_with_date.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1500 2018-06-14 05:14:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_pandas_weekly.yaml
--rw-r--r--   0 cam        (501) staff       (20)      990 2018-06-14 05:14:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_pandas_single.yaml
--rw-r--r--   0 cam        (501) staff       (20)     2044 2018-07-05 00:52:40.000000 tiingo-0.8.0/tests/fixtures/intraday_price.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1378 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/list_stock_tickers.yaml
--rw-r--r--   0 cam        (501) staff       (20)     2223 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/invalid_url.yaml
--rw-r--r--   0 cam        (501) staff       (20)     3141 2018-06-14 05:14:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_pandas_daily_metric_name.yaml
--rw-r--r--   0 cam        (501) staff       (20)      990 2018-04-21 19:58:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price.yaml
--rw-r--r--   0 cam        (501) staff       (20)      780 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/news_bulk.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1699 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/news.yaml
--rw-r--r--   0 cam        (501) staff       (20)     3053 2018-06-14 05:14:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_pandas_weekly_multiple_tickers.yaml
--rw-r--r--   0 cam        (501) staff       (20)    10026 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/valid_url.yaml
--rw-r--r--   0 cam        (501) staff       (20)      778 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/news_bulk_file_ids.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1370 2018-03-11 19:22:10.000000 tiingo-0.8.0/tests/fixtures/list_etf_tickers.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1370 2018-03-11 19:22:10.000000 tiingo-0.8.0/tests/fixtures/list_fund_tickers.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1784 2017-10-08 16:03:29.000000 tiingo-0.8.0/tests/fixtures/ticker_metadata.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1085 2018-04-21 19:58:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_with_date_csv.yaml
--rw-r--r--   0 cam        (501) staff       (20)     1500 2018-04-21 19:58:22.000000 tiingo-0.8.0/tests/fixtures/ticker_price_weekly.yaml
--rw-r--r--   0 cam        (501) staff       (20)      262 2017-08-25 00:37:44.000000 tiingo-0.8.0/MANIFEST.in
-drwxr-xr-x   0 cam        (501) staff       (20)        0 2018-07-07 17:48:20.000000 tiingo-0.8.0/docs/
--rw-r--r--   0 cam        (501) staff       (20)     1588 2017-10-08 16:11:52.000000 tiingo-0.8.0/docs/index.rst
--rw-r--r--   0 cam        (501) staff       (20)       33 2017-08-25 00:37:44.000000 tiingo-0.8.0/docs/contributing.rst
--rw-r--r--   0 cam        (501) staff       (20)     6762 2017-08-25 00:37:44.000000 tiingo-0.8.0/docs/Makefile
--rwxr-xr-x   0 cam        (501) staff       (20)     8714 2017-10-07 19:09:16.000000 tiingo-0.8.0/docs/conf.py
--rw-r--r--   0 cam        (501) staff       (20)     2515 2017-12-24 18:32:53.000000 tiingo-0.8.0/docs/usage.rst
--rw-r--r--   0 cam        (501) staff       (20)     6459 2017-08-25 00:37:44.000000 tiingo-0.8.0/docs/make.bat
--rw-r--r--   0 cam        (501) staff       (20)       28 2017-08-25 00:37:44.000000 tiingo-0.8.0/docs/history.rst
--rw-r--r--   0 cam        (501) staff       (20)     1168 2017-10-07 18:58:25.000000 tiingo-0.8.0/docs/installation.rst
--rw-r--r--   0 cam        (501) staff       (20)       28 2017-08-25 00:37:44.000000 tiingo-0.8.0/docs/authors.rst
--rw-r--r--   0 cam        (501) staff       (20)       27 2017-08-25 00:37:44.000000 tiingo-0.8.0/docs/readme.rst
--rw-r--r--   0 cam        (501) staff       (20)     2331 2018-06-14 05:14:22.000000 tiingo-0.8.0/setup.py
-drwxr-xr-x   0 cam        (501) staff       (20)        0 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/
--rw-r--r--   0 cam        (501) staff       (20)    11086 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/PKG-INFO
--rw-r--r--   0 cam        (501) staff       (20)        1 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/not-zip-safe
--rw-r--r--   0 cam        (501) staff       (20)     1349 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/SOURCES.txt
--rw-r--r--   0 cam        (501) staff       (20)       32 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/requires.txt
--rw-r--r--   0 cam        (501) staff       (20)        7 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/top_level.txt
--rw-r--r--   0 cam        (501) staff       (20)        1 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo.egg-info/dependency_links.txt
--rw-r--r--   0 cam        (501) staff       (20)     1507 2018-07-07 17:46:38.000000 tiingo-0.8.0/HISTORY.rst
--rw-r--r--   0 cam        (501) staff       (20)      241 2018-07-05 00:52:40.000000 tiingo-0.8.0/AUTHORS.rst
--rw-r--r--   0 cam        (501) staff       (20)      327 2018-07-07 17:48:20.000000 tiingo-0.8.0/setup.cfg
-drwxr-xr-x   0 cam        (501) staff       (20)        0 2018-07-07 17:48:20.000000 tiingo-0.8.0/tiingo/
--rw-r--r--   0 cam        (501) staff       (20)      131 2017-09-17 21:52:32.000000 tiingo-0.8.0/tiingo/__init__.py
--rw-r--r--   0 cam        (501) staff       (20)       46 2018-07-07 17:46:38.000000 tiingo-0.8.0/tiingo/__version__.py
--rw-r--r--   0 cam        (501) staff       (20)    12919 2018-07-05 00:52:40.000000 tiingo-0.8.0/tiingo/api.py
--rw-r--r--   0 cam        (501) staff       (20)     1767 2017-09-11 02:10:35.000000 tiingo-0.8.0/tiingo/restclient.py
--rw-r--r--   0 cam        (501) staff       (20)     6791 2018-07-05 00:52:40.000000 tiingo-0.8.0/README.rst
+drwxr-xr-x   0 cameron    (501) staff       (20)        0 2019-01-31 03:45:02.000000 tiingo-0.9.0/
+-rw-r--r--   0 cameron    (501) staff       (20)      241 2019-01-31 02:12:05.000000 tiingo-0.9.0/AUTHORS.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     3966 2019-01-31 02:12:05.000000 tiingo-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     1667 2019-01-31 03:38:31.000000 tiingo-0.9.0/HISTORY.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     1072 2019-01-31 02:12:05.000000 tiingo-0.9.0/LICENSE
+-rw-r--r--   0 cameron    (501) staff       (20)      262 2019-01-31 02:12:05.000000 tiingo-0.9.0/MANIFEST.in
+-rw-r--r--   0 cameron    (501) staff       (20)    11932 2019-01-31 03:45:02.000000 tiingo-0.9.0/PKG-INFO
+-rw-r--r--   0 cameron    (501) staff       (20)     7306 2019-01-31 03:32:12.000000 tiingo-0.9.0/README.rst
+drwxr-xr-x   0 cameron    (501) staff       (20)        0 2019-01-31 03:45:02.000000 tiingo-0.9.0/docs/
+-rw-r--r--   0 cameron    (501) staff       (20)     6762 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/Makefile
+-rw-r--r--   0 cameron    (501) staff       (20)       28 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/authors.rst
+-rwxr-xr-x   0 cameron    (501) staff       (20)     8714 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/conf.py
+-rw-r--r--   0 cameron    (501) staff       (20)       33 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/contributing.rst
+-rw-r--r--   0 cameron    (501) staff       (20)       28 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/history.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     2087 2019-01-31 03:32:12.000000 tiingo-0.9.0/docs/index.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     1168 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/installation.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     6459 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/make.bat
+-rw-r--r--   0 cameron    (501) staff       (20)       27 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/readme.rst
+-rw-r--r--   0 cameron    (501) staff       (20)     2515 2019-01-31 02:12:05.000000 tiingo-0.9.0/docs/usage.rst
+-rw-r--r--   0 cameron    (501) staff       (20)      306 2019-01-31 03:45:02.000000 tiingo-0.9.0/setup.cfg
+-rw-r--r--   0 cameron    (501) staff       (20)     2338 2019-01-31 03:32:07.000000 tiingo-0.9.0/setup.py
+drwxr-xr-x   0 cameron    (501) staff       (20)        0 2019-01-31 03:45:02.000000 tiingo-0.9.0/tests/
+-rw-r--r--   0 cameron    (501) staff       (20)       61 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/__init__.py
+drwxr-xr-x   0 cameron    (501) staff       (20)        0 2019-01-31 03:45:02.000000 tiingo-0.9.0/tests/fixtures/
+-rw-r--r--   0 cameron    (501) staff       (20)     2044 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/intraday_price.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     2223 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/invalid_url.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1370 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/list_etf_tickers.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1370 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/list_fund_tickers.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1378 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/list_stock_tickers.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1699 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/news.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)      780 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/news_bulk.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)      778 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/news_bulk_file_ids.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1784 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_metadata.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)      990 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     3141 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_pandas_daily_metric_name.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)      990 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_pandas_single.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1500 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_pandas_weekly.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     3053 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_pandas_weekly_multiple_tickers.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1500 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_weekly.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1250 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_with_date.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     1085 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/ticker_price_with_date_csv.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)    10026 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/fixtures/valid_url.yaml
+-rw-r--r--   0 cameron    (501) staff       (20)     2226 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/test_api_key_tools.py
+-rw-r--r--   0 cameron    (501) staff       (20)     2283 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/test_restclient.py
+-rw-r--r--   0 cameron    (501) staff       (20)     7944 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/test_tiingo.py
+-rw-r--r--   0 cameron    (501) staff       (20)     3988 2019-01-31 02:12:05.000000 tiingo-0.9.0/tests/test_tiingo_pandas.py
+drwxr-xr-x   0 cameron    (501) staff       (20)        0 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo/
+-rw-r--r--   0 cameron    (501) staff       (20)      131 2019-01-31 02:12:05.000000 tiingo-0.9.0/tiingo/__init__.py
+-rw-r--r--   0 cameron    (501) staff       (20)       46 2019-01-31 03:32:07.000000 tiingo-0.9.0/tiingo/__version__.py
+-rw-r--r--   0 cameron    (501) staff       (20)    12919 2019-01-31 02:12:05.000000 tiingo-0.9.0/tiingo/api.py
+-rw-r--r--   0 cameron    (501) staff       (20)     1767 2019-01-31 02:12:06.000000 tiingo-0.9.0/tiingo/restclient.py
+drwxr-xr-x   0 cameron    (501) staff       (20)        0 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/
+-rw-r--r--   0 cameron    (501) staff       (20)    11932 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/PKG-INFO
+-rw-r--r--   0 cameron    (501) staff       (20)     1349 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/SOURCES.txt
+-rw-r--r--   0 cameron    (501) staff       (20)        1 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/dependency_links.txt
+-rw-r--r--   0 cameron    (501) staff       (20)        1 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/not-zip-safe
+-rw-r--r--   0 cameron    (501) staff       (20)       32 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/requires.txt
+-rw-r--r--   0 cameron    (501) staff       (20)        7 2019-01-31 03:45:02.000000 tiingo-0.9.0/tiingo.egg-info/top_level.txt
```

### Comparing `tiingo-0.8.0/PKG-INFO` & `tiingo-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tiingo
-Version: 0.8.0
+Version: 0.9.0
 Summary: REST Client for Tiingo Data Platform API
 Home-page: https://github.com/hydrosquall/tiingo-python
 Author: Cameron Yick
 Author-email: cameron.yick@enigma.com
 License: MIT license
 Description: =============
         Tiingo Python
@@ -25,24 +25,36 @@
                 :target: https://tiingo-python.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         .. image:: https://pyup.io/repos/github/hydrosquall/tiingo-python/shield.svg?maxAge=600
              :target: https://pyup.io/repos/github/hydrosquall/tiingo-python/
              :alt: Updates
         
+        .. image:: https://mybinder.org/badge_logo.svg 
+             :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+             :alt: Launch Binder
+        
+        
         
         Tiingo is a financial data platform that makes high quality financial tools available to all. Tiingo has a REST and Real-Time Data API, which this library helps you to access. Presently, the API includes support for the following endpoints:
         
         * Stock Market Ticker Closing Prices + Metadata. Data includes full distribution details and is validated using a proprietary EOD Price Engine.
         * Curated news from top financial news sources + blogs. Stories are tagged with topic tags and relevant stock tickers by Tiingo's algorithms.
         
         
         Usage
         --------
         
+        If you'd like to try this library without installing anything, click the button below. Otherwise, continue reading.
+        
+        .. image:: https://mybinder.org/badge_logo.svg 
+             :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+             :alt: Launch Binder
+        
+        
         First, install the library from PyPi:
         
         .. code-block:: shell
         
            pip install tiingo
         
         If you prefer to receive your results in ``pandas DataFrame`` or ``Series`` format, and you do not already have pandas installed, install it as an optional dependency:
@@ -174,19 +186,25 @@
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         =======
         History
         =======
         
-        0.8.x (2018-XX-XX)
+        
+        0.10.x (2019-XX-XX)
         ------------------
         * New changes go here!
         
         
+        0.9.x (2019-01-30)
+        ------------------
+        * Documentation: Added runnable jupyter notebook sample under "/examples"
+        * Minor: bumped various library dependencies
+        
         0.8.0 (2018-07-06)
         ------------------
         * Major: Add IEX Endpoint to retrieve data with intraday frequencies (@dcwtx #125)
         * Minor: update documentation for contributing/releasing new versions
         * Speed up Travis build process with pip cache
         
         0.7.0 (2018-06-14)
@@ -232,22 +250,23 @@
         * Deprecate the Mutual Funds endpoint
         
         0.1.0 (2017-08-24)
         ------------------
         
         * First release on PyPI.
         
-Keywords: tiingo,finance,stocks
+Keywords: tiingo,finance,stocks,rest
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: pandas
```

### Comparing `tiingo-0.8.0/LICENSE` & `tiingo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/CONTRIBUTING.rst` & `tiingo-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/test_tiingo.py` & `tiingo-0.9.0/tests/test_tiingo.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/test_restclient.py` & `tiingo-0.9.0/tests/test_restclient.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/test_tiingo_pandas.py` & `tiingo-0.9.0/tests/test_tiingo_pandas.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/test_api_key_tools.py` & `tiingo-0.9.0/tests/test_api_key_tools.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_with_date.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_with_date.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_pandas_weekly.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_pandas_weekly.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_pandas_single.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_pandas_single.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/intraday_price.yaml` & `tiingo-0.9.0/tests/fixtures/intraday_price.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/list_stock_tickers.yaml` & `tiingo-0.9.0/tests/fixtures/list_stock_tickers.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/invalid_url.yaml` & `tiingo-0.9.0/tests/fixtures/invalid_url.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_pandas_daily_metric_name.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_pandas_daily_metric_name.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/news_bulk.yaml` & `tiingo-0.9.0/tests/fixtures/news_bulk.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/news.yaml` & `tiingo-0.9.0/tests/fixtures/news.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_pandas_weekly_multiple_tickers.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_pandas_weekly_multiple_tickers.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/valid_url.yaml` & `tiingo-0.9.0/tests/fixtures/valid_url.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/news_bulk_file_ids.yaml` & `tiingo-0.9.0/tests/fixtures/news_bulk_file_ids.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/list_etf_tickers.yaml` & `tiingo-0.9.0/tests/fixtures/list_etf_tickers.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/list_fund_tickers.yaml` & `tiingo-0.9.0/tests/fixtures/list_fund_tickers.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_metadata.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_metadata.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_with_date_csv.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_with_date_csv.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tests/fixtures/ticker_price_weekly.yaml` & `tiingo-0.9.0/tests/fixtures/ticker_price_weekly.yaml`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/docs/index.rst` & `tiingo-0.9.0/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     :target: https://pyup.io/repos/github/hydrosquall/tiingo-python/
     :alt: Updates
 
 .. image:: https://img.shields.io/codecov/c/github/hydrosquall/tiingo-python.svg?maxAge=600
     :target: https://codecov.io/gh/hydrosquall/tiingo-python
     :alt: Coverage
 
+.. image:: https://mybinder.org/badge_logo.svg 
+     :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+     :alt: Launch Binder
+
 
 Contents:
 
 .. toctree::
    :maxdepth: 2
 
    readme
@@ -33,15 +37,22 @@
    authors
    history
 
 
 Tiingo is a financial data platform that makes high quality financial tools available to all. They have a RESTful and Real-Time Data API. Presently, the API includes support for the following endpoints:
 
 * Stock Market Ticker Closing Prices + Metadata. Data includes full distribution details and is validated using a proprietary EOD Price Engine.
-* (Coming Soon): Curated news from top financial news sources + curated blogs. Stories are tagged by Tiingo's algorithms.
+* Curated news from top financial news sources + curated blogs. Stories are tagged by Tiingo's algorithms.
+
+If you'd like to try this library without installing anything, click the button below. Otherwise, continue reading.
+
+.. image:: https://mybinder.org/badge_logo.svg 
+     :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+     :alt: Launch Binder
+
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `tiingo-0.8.0/docs/Makefile` & `tiingo-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/docs/conf.py` & `tiingo-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/docs/usage.rst` & `tiingo-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/docs/make.bat` & `tiingo-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/docs/installation.rst` & `tiingo-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/setup.py` & `tiingo-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,27 +56,27 @@
     url=URL,
     packages=find_packages(include=[NAME]),
     include_package_data=True,
     install_requires=requirements,
     extras_require={'pandas': ['pandas>=0.18']},
     license="MIT license",
     zip_safe=False,
-    keywords=['tiingo', 'finance', 'stocks'],
+    keywords=['tiingo', 'finance', 'stocks', 'rest'],
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Financial and Insurance Industry',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Topic :: Office/Business :: Financial :: Investment',
         "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
     ],
     test_suite='tests',
     tests_require=test_requirements,
     setup_requires=setup_requirements,
 )
```

### Comparing `tiingo-0.8.0/tiingo.egg-info/PKG-INFO` & `tiingo-0.9.0/tiingo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: tiingo
-Version: 0.8.0
+Version: 0.9.0
 Summary: REST Client for Tiingo Data Platform API
 Home-page: https://github.com/hydrosquall/tiingo-python
 Author: Cameron Yick
 Author-email: cameron.yick@enigma.com
 License: MIT license
 Description: =============
         Tiingo Python
@@ -25,24 +25,36 @@
                 :target: https://tiingo-python.readthedocs.io/en/latest/?badge=latest
                 :alt: Documentation Status
         
         .. image:: https://pyup.io/repos/github/hydrosquall/tiingo-python/shield.svg?maxAge=600
              :target: https://pyup.io/repos/github/hydrosquall/tiingo-python/
              :alt: Updates
         
+        .. image:: https://mybinder.org/badge_logo.svg 
+             :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+             :alt: Launch Binder
+        
+        
         
         Tiingo is a financial data platform that makes high quality financial tools available to all. Tiingo has a REST and Real-Time Data API, which this library helps you to access. Presently, the API includes support for the following endpoints:
         
         * Stock Market Ticker Closing Prices + Metadata. Data includes full distribution details and is validated using a proprietary EOD Price Engine.
         * Curated news from top financial news sources + blogs. Stories are tagged with topic tags and relevant stock tickers by Tiingo's algorithms.
         
         
         Usage
         --------
         
+        If you'd like to try this library without installing anything, click the button below. Otherwise, continue reading.
+        
+        .. image:: https://mybinder.org/badge_logo.svg 
+             :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+             :alt: Launch Binder
+        
+        
         First, install the library from PyPi:
         
         .. code-block:: shell
         
            pip install tiingo
         
         If you prefer to receive your results in ``pandas DataFrame`` or ``Series`` format, and you do not already have pandas installed, install it as an optional dependency:
@@ -174,19 +186,25 @@
         .. _Cookiecutter: https://github.com/audreyr/cookiecutter
         .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
         
         =======
         History
         =======
         
-        0.8.x (2018-XX-XX)
+        
+        0.10.x (2019-XX-XX)
         ------------------
         * New changes go here!
         
         
+        0.9.x (2019-01-30)
+        ------------------
+        * Documentation: Added runnable jupyter notebook sample under "/examples"
+        * Minor: bumped various library dependencies
+        
         0.8.0 (2018-07-06)
         ------------------
         * Major: Add IEX Endpoint to retrieve data with intraday frequencies (@dcwtx #125)
         * Minor: update documentation for contributing/releasing new versions
         * Speed up Travis build process with pip cache
         
         0.7.0 (2018-06-14)
@@ -232,22 +250,23 @@
         * Deprecate the Mutual Funds endpoint
         
         0.1.0 (2017-08-24)
         ------------------
         
         * First release on PyPI.
         
-Keywords: tiingo,finance,stocks
+Keywords: tiingo,finance,stocks,rest
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Provides-Extra: pandas
```

### Comparing `tiingo-0.8.0/tiingo.egg-info/SOURCES.txt` & `tiingo-0.9.0/tiingo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/HISTORY.rst` & `tiingo-0.9.0/HISTORY.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 =======
 History
 =======
 
-0.8.x (2018-XX-XX)
+
+0.10.x (2019-XX-XX)
 ------------------
 * New changes go here!
 
 
+0.9.x (2019-01-30)
+------------------
+* Documentation: Added runnable jupyter notebook sample under "/examples"
+* Minor: bumped various library dependencies
+
 0.8.0 (2018-07-06)
 ------------------
 * Major: Add IEX Endpoint to retrieve data with intraday frequencies (@dcwtx #125)
 * Minor: update documentation for contributing/releasing new versions
 * Speed up Travis build process with pip cache
 
 0.7.0 (2018-06-14)
```

### Comparing `tiingo-0.8.0/tiingo/api.py` & `tiingo-0.9.0/tiingo/api.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/tiingo/restclient.py` & `tiingo-0.9.0/tiingo/restclient.py`

 * *Files identical despite different names*

### Comparing `tiingo-0.8.0/README.rst` & `tiingo-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,36 @@
         :target: https://tiingo-python.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://pyup.io/repos/github/hydrosquall/tiingo-python/shield.svg?maxAge=600
      :target: https://pyup.io/repos/github/hydrosquall/tiingo-python/
      :alt: Updates
 
+.. image:: https://mybinder.org/badge_logo.svg 
+     :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+     :alt: Launch Binder
+
+
 
 Tiingo is a financial data platform that makes high quality financial tools available to all. Tiingo has a REST and Real-Time Data API, which this library helps you to access. Presently, the API includes support for the following endpoints:
 
 * Stock Market Ticker Closing Prices + Metadata. Data includes full distribution details and is validated using a proprietary EOD Price Engine.
 * Curated news from top financial news sources + blogs. Stories are tagged with topic tags and relevant stock tickers by Tiingo's algorithms.
 
 
 Usage
 --------
 
+If you'd like to try this library without installing anything, click the button below. Otherwise, continue reading.
+
+.. image:: https://mybinder.org/badge_logo.svg 
+     :target: https://mybinder.org/v2/gh/hydrosquall/tiingo-python/master?filepath=examples%2Fbasic-usage-with-pandas.ipynb
+     :alt: Launch Binder
+
+
 First, install the library from PyPi:
 
 .. code-block:: shell
 
    pip install tiingo
 
 If you prefer to receive your results in ``pandas DataFrame`` or ``Series`` format, and you do not already have pandas installed, install it as an optional dependency:
```

