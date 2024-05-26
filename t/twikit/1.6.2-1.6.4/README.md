# Comparing `tmp/twikit-1.6.2.tar.gz` & `tmp/twikit-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.6.2.tar", last modified: Sat May  4 08:01:21 2024, max compression
+gzip compressed data, was "twikit-1.6.4.tar", last modified: Sun May 26 04:01:17 2024, max compression
```

## Comparing `twikit-1.6.2.tar` & `twikit-1.6.4.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 08:01:21.500070 twikit-1.6.2/
--rw-rw-rw-   0        0        0     1079 2024-05-01 18:21:05.000000 twikit-1.6.2/LICENSE
--rw-rw-rw-   0        0        0     3999 2024-05-04 08:01:21.495084 twikit-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     3728 2024-05-01 18:21:05.000000 twikit-1.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 08:01:21.500070 twikit-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-05-04 04:46:09.000000 twikit-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:01:21.303596 twikit-1.6.2/twikit/
--rw-rw-rw-   0        0        0      689 2024-05-04 06:00:07.000000 twikit-1.6.2/twikit/__init__.py
--rw-rw-rw-   0        0        0     1686 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/bookmark.py
--rw-rw-rw-   0        0        0   145687 2024-05-04 06:26:53.000000 twikit-1.6.2/twikit/client.py
--rw-rw-rw-   0        0        0     8639 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/community.py
--rw-rw-rw-   0        0        0     2666 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/group.py
--rw-rw-rw-   0        0        0     2218 2024-05-02 13:58:54.000000 twikit-1.6.2/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/notification.py
--rw-rw-rw-   0        0        0        0 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/py.typed
--rw-rw-rw-   0        0        0     8193 2024-05-04 04:14:29.000000 twikit-1.6.2/twikit/streaming.py
--rw-rw-rw-   0        0        0     2825 2024-05-04 04:17:28.000000 twikit-1.6.2/twikit/trend.py
--rw-rw-rw-   0        0        0    23780 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:01:21.481126 twikit-1.6.2/twikit/twikit_async/
--rw-rw-rw-   0        0        0      610 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0     1758 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/bookmark.py
--rw-rw-rw-   0        0        0   148138 2024-05-04 04:18:05.000000 twikit-1.6.2/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0     8767 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/community.py
--rw-rw-rw-   0        0        0      875 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     2260 2024-05-03 13:08:32.000000 twikit-1.6.2/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     8320 2024-05-04 04:19:04.000000 twikit-1.6.2/twikit/twikit_async/streaming.py
--rw-rw-rw-   0        0        0     2844 2024-05-04 04:17:45.000000 twikit-1.6.2/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    23661 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14740 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14517 2024-05-01 18:21:05.000000 twikit-1.6.2/twikit/user.py
--rw-rw-rw-   0        0        0    30626 2024-05-04 03:25:31.000000 twikit-1.6.2/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-04 08:01:21.366429 twikit-1.6.2/twikit.egg-info/
--rw-rw-rw-   0        0        0     3999 2024-05-04 08:01:20.000000 twikit-1.6.2/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      910 2024-05-04 08:01:20.000000 twikit-1.6.2/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 08:01:20.000000 twikit-1.6.2/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-04 08:01:20.000000 twikit-1.6.2/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-04 08:01:20.000000 twikit-1.6.2/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.501724 twikit-1.6.4/
+-rw-rw-rw-   0        0        0     1079 2024-05-26 04:00:24.000000 twikit-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     3635 2024-05-26 04:01:17.499729 twikit-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3364 2024-05-26 04:00:24.000000 twikit-1.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 04:01:17.501724 twikit-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-05-26 04:00:24.000000 twikit-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.421943 twikit-1.6.4/twikit/
+-rw-rw-rw-   0        0        0      713 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/__init__.py
+-rw-rw-rw-   0        0        0     1686 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/bookmark.py
+-rw-rw-rw-   0        0        0   154823 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/client.py
+-rw-rw-rw-   0        0        0     8639 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/community.py
+-rw-rw-rw-   0        0        0     2666 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/errors.py
+-rw-rw-rw-   0        0        0     2708 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/geo.py
+-rw-rw-rw-   0        0        0     7305 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/group.py
+-rw-rw-rw-   0        0        0     2218 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/notification.py
+-rw-rw-rw-   0        0        0        0 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/py.typed
+-rw-rw-rw-   0        0        0     8193 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/streaming.py
+-rw-rw-rw-   0        0        0     2825 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/trend.py
+-rw-rw-rw-   0        0        0    23780 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.495740 twikit-1.6.4/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      634 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0     1758 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/bookmark.py
+-rw-rw-rw-   0        0        0   157383 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0     8767 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/community.py
+-rw-rw-rw-   0        0        0      875 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     2720 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/geo.py
+-rw-rw-rw-   0        0        0     7509 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     2260 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     8320 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/streaming.py
+-rw-rw-rw-   0        0        0     2844 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    23661 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14740 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14517 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/user.py
+-rw-rw-rw-   0        0        0    31186 2024-05-26 04:00:24.000000 twikit-1.6.4/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 04:01:17.438900 twikit-1.6.4/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3635 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 04:01:17.000000 twikit-1.6.4/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.6.2/LICENSE` & `twikit-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/PKG-INFO` & `twikit-1.6.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.6.2
+Version: 1.6.4
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -15,57 +15,56 @@
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Create%20your%20own%20Twitter%20bot%20for%20free%20with%20%22Twikit%22!%20%23python%20%23twitter%20%23twikit%20%23programming%20%23github%20%23bot&url=https%3A%2F%2Fgithub.com%2Fd60%2Ftwikit)
 [![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/nCrByrr8cX)
 [![BuyMeACoffee](https://img.shields.io/badge/-buy_me_a%C2%A0coffee-gray?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/d60py)
 
+[[日本語](https://github.com/d60/twikit/blob/main/README-ja.md)]
+[[中文](https://github.com/d60/twikit/blob/main/README-zh.md)]
 
 # Twikit <img height="35"  src="https://i.imgur.com/9HSdIl4.png"  valign="bottom">
 
-simple API wrapper to interact with twitter's unofficial API.
+A Simple Twitter API Scraper
 
-You can log in to Twitter using your account username, email address and password and use most features on Twitter, such as posting and retrieving tweets, liking and following users.
+You can use functions such as posting or searching for tweets without an API key using this library.
 
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
 
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
 
-
-If you have any questions, you can ask on [Discord](https://discord.gg/nCrByrr8cX).
+[Discord](https://discord.gg/nCrByrr8cX)
 
 
 
 ## Features
 
 ### No API Key Required
 
-This library uses the unofficial API, therefore does **not require an API key**.
+This library uses scraping and does not require an API key.
 
-### Completely Free
+### Free
 
-This library is completely free to use.
+This library is free to use.
 
 ### Both Synchronous and Asynchronous Support
 
-Whether you prefer **synchronous** or **asynchronous** programming,
-
-Twikit supports both, providing flexibility for different use cases.
+Twikit supports both synchronous and asynchronous.
 
 
 ## Functionality
 
-This library allows you to perform various Twitter-related actions, including:
+By using Twikit, you can access functionalities such as the following:
 
--  **Create tweets**
+-  Create tweets
 
--  **Search tweets**
+-  Search tweets
 
--  **Retrieve trending topics**
+-  Retrieve trending topics
 
 - etc...
 
 
 
 ## Installing
 
@@ -87,15 +86,14 @@
 USERNAME = 'example_user'
 EMAIL = 'email@example.com'
 PASSWORD = 'password0000'
 
 # Initialize client
 client = Client('en-US')
 
-# Login to the service with provided user credentials
 client.login(
     auth_info_1=USERNAME ,
     auth_info_2=EMAIL,
     password=PASSWORD
 )
 ```
 
@@ -112,15 +110,15 @@
 client.create_tweet(
     text='Example Tweet',
     media_ids=media_ids
 )
 
 ```
 
-**Search the latest tweets based on a keywords**
+**Search the latest tweets based on a keyword**
 ```python
 tweets = client.search_tweet('python', 'Latest')
 
 for tweet in tweets:
     print(
         tweet.user.name,
         tweet.text,
@@ -136,14 +134,10 @@
     print(tweet.text)
 ```
 
 More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
 ## Contributing
 
-I would like to hear your thoughts and suggestions.
-
-If you have any features you'd like to see added or encounter any issues,
-
-please let me know in the [issues](https://github.com/d60/twikit/issues) section.
+If you encounter any bugs or issues, please report them on [issues](https://github.com/d60/twikit/issues).
 
-Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
+Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library.
```

### Comparing `twikit-1.6.2/README.md` & `twikit-1.6.4/twikit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,70 @@
+Metadata-Version: 2.1
+Name: twikit
+Version: 1.6.4
+Summary: Twitter API wrapper for python with **no API key required**.
+Home-page: https://github.com/d60/twikit
+License: MIT
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
 
 
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Create%20your%20own%20Twitter%20bot%20for%20free%20with%20%22Twikit%22!%20%23python%20%23twitter%20%23twikit%20%23programming%20%23github%20%23bot&url=https%3A%2F%2Fgithub.com%2Fd60%2Ftwikit)
 [![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/nCrByrr8cX)
 [![BuyMeACoffee](https://img.shields.io/badge/-buy_me_a%C2%A0coffee-gray?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/d60py)
 
+[[日本語](https://github.com/d60/twikit/blob/main/README-ja.md)]
+[[中文](https://github.com/d60/twikit/blob/main/README-zh.md)]
 
 # Twikit <img height="35"  src="https://i.imgur.com/9HSdIl4.png"  valign="bottom">
 
-simple API wrapper to interact with twitter's unofficial API.
+A Simple Twitter API Scraper
 
-You can log in to Twitter using your account username, email address and password and use most features on Twitter, such as posting and retrieving tweets, liking and following users.
+You can use functions such as posting or searching for tweets without an API key using this library.
 
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
 
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
 
-
-If you have any questions, you can ask on [Discord](https://discord.gg/nCrByrr8cX).
+[Discord](https://discord.gg/nCrByrr8cX)
 
 
 
 ## Features
 
 ### No API Key Required
 
-This library uses the unofficial API, therefore does **not require an API key**.
+This library uses scraping and does not require an API key.
 
-### Completely Free
+### Free
 
-This library is completely free to use.
+This library is free to use.
 
 ### Both Synchronous and Asynchronous Support
 
-Whether you prefer **synchronous** or **asynchronous** programming,
-
-Twikit supports both, providing flexibility for different use cases.
+Twikit supports both synchronous and asynchronous.
 
 
 ## Functionality
 
-This library allows you to perform various Twitter-related actions, including:
+By using Twikit, you can access functionalities such as the following:
 
--  **Create tweets**
+-  Create tweets
 
--  **Search tweets**
+-  Search tweets
 
--  **Retrieve trending topics**
+-  Retrieve trending topics
 
 - etc...
 
 
 
 ## Installing
 
@@ -77,15 +86,14 @@
 USERNAME = 'example_user'
 EMAIL = 'email@example.com'
 PASSWORD = 'password0000'
 
 # Initialize client
 client = Client('en-US')
 
-# Login to the service with provided user credentials
 client.login(
     auth_info_1=USERNAME ,
     auth_info_2=EMAIL,
     password=PASSWORD
 )
 ```
 
@@ -102,15 +110,15 @@
 client.create_tweet(
     text='Example Tweet',
     media_ids=media_ids
 )
 
 ```
 
-**Search the latest tweets based on a keywords**
+**Search the latest tweets based on a keyword**
 ```python
 tweets = client.search_tweet('python', 'Latest')
 
 for tweet in tweets:
     print(
         tweet.user.name,
         tweet.text,
@@ -126,14 +134,10 @@
     print(tweet.text)
 ```
 
 More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
 ## Contributing
 
-I would like to hear your thoughts and suggestions.
-
-If you have any features you'd like to see added or encounter any issues,
-
-please let me know in the [issues](https://github.com/d60/twikit/issues) section.
+If you encounter any bugs or issues, please report them on [issues](https://github.com/d60/twikit/issues).
 
-Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
+Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library.
```

### Comparing `twikit-1.6.2/setup.py` & `twikit-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/__init__.py` & `twikit-1.6.4/twikit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 Twikit Twitter API Wrapper
 ==========================
 
 https://github.com/d60/twikit
 A Python library for interacting with the Twitter API.
 """
 
-__version__ = '1.6.2'
+__version__ = '1.6.4'
 
 from .bookmark import BookmarkFolder
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
 from .errors import *
+from .geo import Place
 from .group import Group, GroupMessage
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
 from .user import User
```

### Comparing `twikit-1.6.2/twikit/bookmark.py` & `twikit-1.6.4/twikit/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/client.py` & `twikit-1.6.4/twikit/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 from httpx import Response
 
 from .bookmark import BookmarkFolder
 from .community import Community, CommunityMember
 from .errors import (
     CouldNotTweet,
     InvalidMedia,
+    TweetNotAvailable,
     TwitterException,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
+from .geo import Place, _places_from_response
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import PlaceTrend, PlaceTrends, Location, Trend
 from .streaming import Payload, StreamingSession, _payload_from_data
@@ -1303,14 +1305,125 @@
         if 'result' not in response['data']['user']:
             raise TwitterException(f'Invalid user id: {user_id}')
         user_data = response['data']['user']['result']
         if user_data.get('__typename') == 'UserUnavailable':
             raise UserUnavailable(user_data.get('message'))
         return User(self, user_data)
 
+    def reverse_geocode(
+        self, lat: float, long: float, accuracy: str | float | None = None,
+        granularity: str | None = None, max_results: int | None = None
+    ) -> list[Place]:
+        """
+        Given a latitude and a longitude, searches for up to 20 places that
+
+        Parameters
+        ----------
+        lat : :class:`float`
+            The latitude to search around.
+        long : :class:`float`
+            The longitude to search around.
+        accuracy : :class:`str` | :class:`float` None, default=None
+            A hint on the "region" in which to search.
+        granularity : :class:`str` | None, default=None
+            This is the minimal granularity of place types to return and must
+            be one of: `neighborhood`, `city`, `admin` or `country`.
+        max_results : :class:`int` | None, default=None
+            A hint as to the number of results to return.
+
+        Returns
+        -------
+        list[:class:`.Place`]
+        """
+        params = {
+            'lat': lat,
+            'long': long,
+            'accuracy': accuracy,
+            'granularity': granularity,
+            'max_results': max_results
+        }
+        for k, v in tuple(params.items()):
+            if v is None:
+                params.pop(k)
+
+        response = self.http.get(
+            Endpoint.REVERSE_GEOCODE,
+            params=params,
+            headers=self._base_headers
+        ).json()
+        return _places_from_response(self, response)
+
+    def search_geo(
+        self, lat: float | None = None, long: float | None = None,
+        query: str | None = None, ip: str | None = None,
+        granularity: str | None = None, max_results: int | None = None
+    ) -> list[Place]:
+        """
+        Search for places that can be attached to a Tweet via POST
+        statuses/update.
+
+        Parameters
+        ----------
+        lat : :class:`float` | None
+            The latitude to search around.
+        long : :class:`float` | None
+            	The longitude to search around.
+        query : :class:`str` | None
+            Free-form text to match against while executing a geo-based query,
+            best suited for finding nearby locations by name.
+            Remember to URL encode the query.
+        ip : :class:`str` | None
+            An IP address. Used when attempting to
+            fix geolocation based off of the user's IP address.
+        granularity : :class:`str` | None
+            This is the minimal granularity of place types to return and must
+            be one of: `neighborhood`, `city`, `admin` or `country`.
+        max_results : :class:`int` | None
+            A hint as to the number of results to return.
+
+        Returns
+        -------
+        list[:class:`.Place`]
+        """
+        params = {
+            'lat': lat,
+            'long': long,
+            'query': query,
+            'ip': ip,
+            'granularity': granularity,
+            'max_results': max_results
+        }
+        for k, v in tuple(params.items()):
+            if v is None:
+                params.pop(k)
+
+        response = self.http.get(
+            Endpoint.SEARCH_GEO,
+            params=params,
+            headers=self._base_headers
+        ).json()
+        return _places_from_response(self, response)
+
+    def get_place(self, id: str) -> Place:
+        """
+        Parameters
+        ----------
+        id : :class:`str`
+            The ID of the place.
+
+        Returns
+        -------
+        :class:`.Place`
+        """
+        response = self.http.get(
+            Endpoint.PLACE_BY_ID.format(id),
+            headers=self._base_headers
+        ).json()
+        return Place(self, response)
+
     def _get_tweet_detail(self, tweet_id: str, cursor: str | None):
         variables = {
             'focalTweetId': tweet_id,
             'with_rux_injections': False,
             'includePromotedContent': True,
             'withCommunity': True,
             'withQuickPromoteEligibilityTweetFields': True,
@@ -1391,14 +1504,17 @@
         >>> target_tweet_id = '...'
         >>> tweet = client.get_tweet_by_id(target_tweet_id)
         >>> print(tweet)
         <Tweet id="...">
         """
         response = self._get_tweet_detail(tweet_id, cursor)
 
+        if 'errors' in response:
+            raise TweetNotAvailable(response['errors'][0]['message'])
+
         entries = find_dict(response, 'entries')[0]
         reply_to = []
         replies_list = []
         related_tweets = []
         tweet = None
 
         for entry in entries:
@@ -2818,16 +2934,54 @@
         return Result(
             results,
             partial(self._get_user_friendship,
                     user_id, count, endpoint, next_cursor),
             next_cursor
         )
 
+    def _get_user_friendship_2(
+        self, user_id: str, screen_name: str,
+        count: int, endpoint: str, cursor: str
+    ) -> Result[User]:
+        params = {'count': count}
+        if user_id is not None:
+            params['user_id'] = user_id
+        elif user_id is not None:
+            params['screen_name'] = screen_name
+
+        if cursor is not None:
+            params['cursor'] = cursor
+
+        response = self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        ).json()
+
+        users = response['users']
+        results = []
+        for user in users:
+            results.append(User(self, build_user_data(user)))
+
+        previous_cursor = response['previous_cursor']
+        next_cursor = response['next_cursor']
+
+        return Result(
+            results,
+            partial(self._get_user_friendship_2, user_id,
+                    count, endpoint, next_cursor),
+            next_cursor,
+            partial(self._get_user_friendship_2, user_id,
+                    count, endpoint, previous_cursor),
+            previous_cursor
+        )
+
     def get_user_followers(
-        self, user_id: str, count: int = 20, cursor: str | None = None
+        self, user_id: str,
+        count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of followers for a given user.
 
         Parameters
         ----------
         user_id : :class:`str`
@@ -2843,14 +2997,46 @@
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS,
             cursor
         )
 
+    def get_latest_followers(
+        self, user_id: str | None = None, screen_name: str | None = None,
+        count: int = 200, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest followers.
+        Max count : 200
+        """
+        return self._get_user_friendship_2(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FOLLOWERS2,
+            cursor
+        )
+
+    def get_latest_friends(
+        self, user_id: str | None = None, screen_name: str | None = None,
+        count: int = 200, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest friends (following users).
+        Max count : 200
+        """
+        return self._get_user_friendship_2(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FOLLOWING2,
+            cursor
+        )
+
     def get_user_verified_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of verified followers for a given user.
 
         Parameters
@@ -2943,14 +3129,113 @@
         return self._get_user_friendship(
             user_id,
             count,
             Endpoint.SUBSCRIPTIONS,
             cursor
         )
 
+    def _get_friendship_ids(
+        self,
+        user_id: str | None,
+        screen_name: str | None,
+        count: int,
+        endpoint: str,
+        cursor: str | None
+    ) -> Result[int]:
+        params = {'count': count}
+        if user_id is not None:
+            params['user_id'] = user_id
+        elif user_id is not None:
+            params['screen_name'] = screen_name
+
+        if cursor is not None:
+            params['cursor'] = cursor
+
+        response = self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        ).json()
+        previous_cursor = response['previous_cursor']
+        next_cursor = response['next_cursor']
+
+        return Result(
+            response['ids'],
+            partial(self._get_friendship_ids, user_id,
+                     screen_name, count, endpoint, next_cursor),
+            next_cursor,
+            partial(self._get_friendship_ids, user_id,
+                     screen_name, count, endpoint, previous_cursor),
+            previous_cursor
+        )
+
+    def get_followers_ids(
+        self,
+        user_id: str | None = None,
+        screen_name: str | None = None,
+        count: int = 5000,
+        cursor: str | None = None
+    ) -> Result[int]:
+        """
+        Fetches the IDs of the followers of a specified user.
+
+        Parameters
+        ----------
+        user_id : :class:`str` | None, default=None
+            The ID of the user for whom to return results.
+        screen_name : :class:`str` | None, default=None
+            The screen name of the user for whom to return results.
+        count : :class:`int`, default=5000
+            The maximum number of IDs to retrieve.
+
+        Returns
+        -------
+        :class:`Result`[:class:`int`]
+            A Result object containing the IDs of the followers.
+        """
+        return self._get_friendship_ids(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FOLLOWERS_IDS,
+            cursor
+        )
+
+    def get_friends_ids(
+        self,
+        user_id: str | None = None,
+        screen_name: str | None = None,
+        count: int = 5000,
+        cursor: str | None = None
+    ) -> Result[int]:
+        """
+        Fetches the IDs of the friends (following users) of a specified user.
+
+        Parameters
+        ----------
+        user_id : :class:`str` | None, default=None
+            The ID of the user for whom to return results.
+        screen_name : :class:`str` | None, default=None
+            The screen name of the user for whom to return results.
+        count : :class:`int`, default=5000
+            The maximum number of IDs to retrieve.
+
+        Returns
+        -------
+        :class:`Result`[:class:`int`]
+            A Result object containing the IDs of the friends.
+        """
+        return self._get_friendship_ids(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FRIENDS_IDS,
+            cursor
+        )
+
     def _send_dm(
         self,
         conversation_id: str,
         text: str,
         media_id: str | None,
         reply_to: str | None
     ) -> dict:
```

### Comparing `twikit-1.6.2/twikit/community.py` & `twikit-1.6.4/twikit/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/errors.py` & `twikit-1.6.4/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/group.py` & `twikit-1.6.4/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/http.py` & `twikit-1.6.4/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/list.py` & `twikit-1.6.4/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/message.py` & `twikit-1.6.4/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/notification.py` & `twikit-1.6.4/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/streaming.py` & `twikit-1.6.4/twikit/streaming.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/trend.py` & `twikit-1.6.4/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/tweet.py` & `twikit-1.6.4/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/__init__.py` & `twikit-1.6.4/twikit/twikit_async/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .bookmark import BookmarkFolder
 from ..errors import *
 from ..utils import build_query
 from .client import Client
 from .community import (Community, CommunityCreator, CommunityMember,
                         CommunityRule)
+from .geo import Place
 from .group import Group, GroupMessage
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Trend
 from .tweet import CommunityNote, Poll, ScheduledTweet, Tweet
 from .user import User
```

### Comparing `twikit-1.6.2/twikit/twikit_async/bookmark.py` & `twikit-1.6.4/twikit/twikit_async/bookmark.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/client.py` & `twikit-1.6.4/twikit/twikit_async/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from fake_useragent import UserAgent
 from httpx import Response
 
 from ..errors import (
     CouldNotTweet,
     InvalidMedia,
     TwitterException,
+    TweetNotAvailable,
     UserNotFound,
     UserUnavailable,
     raise_exceptions_from_response
 )
 from ..utils import (
     BOOKMARK_FOLDER_TIMELINE_FEATURES,
     COMMUNITY_TWEETS_FEATURES,
@@ -39,14 +40,15 @@
     urlencode
 )
 from .bookmark import BookmarkFolder
 from .community import (
     Community,
     CommunityMember
 )
+from .geo import Place, _places_from_response
 from .group import Group, GroupMessage
 from .http import HTTPClient
 from .list import List
 from .message import Message
 from .notification import Notification
 from .trend import Location, PlaceTrend, PlaceTrends, Trend
 from .streaming import Payload, StreamingSession, _payload_from_data
@@ -1316,14 +1318,125 @@
         if 'result' not in response['data']['user']:
             raise TwitterException(f'Invalid user id: {user_id}')
         user_data = response['data']['user']['result']
         if user_data.get('__typename') == 'UserUnavailable':
             raise UserUnavailable(user_data.get('message'))
         return User(self, user_data)
 
+    async def reverse_geocode(
+        self, lat: float, long: float, accuracy: str | float | None = None,
+        granularity: str | None = None, max_results: int | None = None
+    ) -> list[Place]:
+        """
+        Given a latitude and a longitude, searches for up to 20 places that
+
+        Parameters
+        ----------
+        lat : :class:`float`
+            The latitude to search around.
+        long : :class:`float`
+            The longitude to search around.
+        accuracy : :class:`str` | :class:`float` None, default=None
+            A hint on the "region" in which to search.
+        granularity : :class:`str` | None, default=None
+            This is the minimal granularity of place types to return and must
+            be one of: `neighborhood`, `city`, `admin` or `country`.
+        max_results : :class:`int` | None, default=None
+            A hint as to the number of results to return.
+
+        Returns
+        -------
+        list[:class:`.Place`]
+        """
+        params = {
+            'lat': lat,
+            'long': long,
+            'accuracy': accuracy,
+            'granularity': granularity,
+            'max_results': max_results
+        }
+        for k, v in tuple(params.items()):
+            if v is None:
+                params.pop(k)
+
+        response = (await self.http.get(
+            Endpoint.REVERSE_GEOCODE,
+            params=params,
+            headers=self._base_headers
+        )).json()
+        return _places_from_response(self, response)
+
+    async def search_geo(
+        self, lat: float | None = None, long: float | None = None,
+        query: str | None = None, ip: str | None = None,
+        granularity: str | None = None, max_results: int | None = None
+    ) -> list[Place]:
+        """
+        Search for places that can be attached to a Tweet via POST
+        statuses/update.
+
+        Parameters
+        ----------
+        lat : :class:`float` | None
+            The latitude to search around.
+        long : :class:`float` | None
+            	The longitude to search around.
+        query : :class:`str` | None
+            Free-form text to match against while executing a geo-based query,
+            best suited for finding nearby locations by name.
+            Remember to URL encode the query.
+        ip : :class:`str` | None
+            An IP address. Used when attempting to
+            fix geolocation based off of the user's IP address.
+        granularity : :class:`str` | None
+            This is the minimal granularity of place types to return and must
+            be one of: `neighborhood`, `city`, `admin` or `country`.
+        max_results : :class:`int` | None
+            A hint as to the number of results to return.
+
+        Returns
+        -------
+        list[:class:`.Place`]
+        """
+        params = {
+            'lat': lat,
+            'long': long,
+            'query': query,
+            'ip': ip,
+            'granularity': granularity,
+            'max_results': max_results
+        }
+        for k, v in tuple(params.items()):
+            if v is None:
+                params.pop(k)
+
+        response = (await self.http.get(
+            Endpoint.SEARCH_GEO,
+            params=params,
+            headers=self._base_headers
+        )).json()
+        return _places_from_response(self, response)
+
+    async def get_place(self, id: str) -> Place:
+        """
+        Parameters
+        ----------
+        id : :class:`str`
+            The ID of the place.
+
+        Returns
+        -------
+        :class:`.Place`
+        """
+        response = (await self.http.get(
+            Endpoint.PLACE_BY_ID.format(id),
+            headers=self._base_headers
+        )).json()
+        return Place(self, response)
+
     async def _get_tweet_detail(self, tweet_id: str, cursor: str | None):
         variables = {
             'focalTweetId': tweet_id,
             'with_rux_injections': False,
             'includePromotedContent': True,
             'withCommunity': True,
             'withQuickPromoteEligibilityTweetFields': True,
@@ -1408,14 +1521,17 @@
         >>> target_tweet_id = '...'
         >>> tweet = client.get_tweet_by_id(target_tweet_id)
         >>> print(tweet)
         <Tweet id="...">
         """
         response = await self._get_tweet_detail(tweet_id, cursor)
 
+        if 'errors' in response:
+            raise TweetNotAvailable(response['errors'][0]['message'])
+
         entries = find_dict(response, 'entries')[0]
         reply_to = []
         replies_list = []
         related_tweets = []
         tweet = None
 
         for entry in entries:
@@ -2838,14 +2954,51 @@
         return Result(
             results,
             partial(self._get_user_friendship,
                     user_id, count, endpoint, next_cursor),
             next_cursor
         )
 
+    async def _get_user_friendship_2(
+        self, user_id: str, screen_name: str,
+        count: int, endpoint: str, cursor: str
+    ) -> Result[User]:
+        params = {'count': count}
+        if user_id is not None:
+            params['user_id'] = user_id
+        elif user_id is not None:
+            params['screen_name'] = screen_name
+
+        if cursor is not None:
+            params['cursor'] = cursor
+
+        response = (await self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        )).json()
+
+        users = response['users']
+        results = []
+        for user in users:
+            results.append(User(self, build_user_data(user)))
+
+        previous_cursor = response['previous_cursor']
+        next_cursor = response['next_cursor']
+
+        return Result(
+            results,
+            partial(self._get_user_friendship_2, user_id,
+                    count, endpoint, next_cursor),
+            next_cursor,
+            partial(self._get_user_friendship_2, user_id,
+                    count, endpoint, previous_cursor),
+            previous_cursor
+        )
+
     async def get_user_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of followers for a given user.
 
         Parameters
@@ -2863,14 +3016,46 @@
         return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.FOLLOWERS,
             cursor
         )
 
+    async def get_latest_followers(
+        self, user_id: str | None = None, screen_name: str | None = None,
+        count: int = 200, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest followers.
+        Max count : 200
+        """
+        return await self._get_user_friendship_2(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FOLLOWERS2,
+            cursor
+        )
+
+    async def get_latest_friends(
+        self, user_id: str | None = None, screen_name: str | None = None,
+        count: int = 200, cursor: str | None = None
+    ) -> Result[User]:
+        """
+        Retrieves the latest friends (following users).
+        Max count : 200
+        """
+        return await self._get_user_friendship_2(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FOLLOWING2,
+            cursor
+        )
+
     async def get_user_verified_followers(
         self, user_id: str, count: int = 20, cursor: str | None = None
     ) -> Result[User]:
         """
         Retrieves a list of verified followers for a given user.
 
         Parameters
@@ -2963,14 +3148,113 @@
         return await self._get_user_friendship(
             user_id,
             count,
             Endpoint.SUBSCRIPTIONS,
             cursor
         )
 
+    async def _get_friendship_ids(
+        self,
+        user_id: str | None,
+        screen_name: str | None,
+        count: int,
+        endpoint: str,
+        cursor: str | None
+    ) -> Result[int]:
+        params = {'count': count}
+        if user_id is not None:
+            params['user_id'] = user_id
+        elif user_id is not None:
+            params['screen_name'] = screen_name
+
+        if cursor is not None:
+            params['cursor'] = cursor
+
+        response = (await self.http.get(
+            endpoint,
+            params=params,
+            headers=self._base_headers
+        )).json()
+        previous_cursor = response['previous_cursor']
+        next_cursor = response['next_cursor']
+
+        return Result(
+            response['ids'],
+            partial(self._get_friendship_ids, user_id,
+                     screen_name, count, endpoint, next_cursor),
+            next_cursor,
+            partial(self._get_friendship_ids, user_id,
+                     screen_name, count, endpoint, previous_cursor),
+            previous_cursor
+        )
+
+    async def get_followers_ids(
+        self,
+        user_id: str | None = None,
+        screen_name: str | None = None,
+        count: int = 5000,
+        cursor: str | None = None
+    ) -> Result[int]:
+        """
+        Fetches the IDs of the followers of a specified user.
+
+        Parameters
+        ----------
+        user_id : :class:`str` | None, default=None
+            The ID of the user for whom to return results.
+        screen_name : :class:`str` | None, default=None
+            The screen name of the user for whom to return results.
+        count : :class:`int`, default=5000
+            The maximum number of IDs to retrieve.
+
+        Returns
+        -------
+        :class:`Result`[:class:`int`]
+            A Result object containing the IDs of the followers.
+        """
+        return await self._get_friendship_ids(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FOLLOWERS_IDS,
+            cursor
+        )
+
+    async def get_friends_ids(
+        self,
+        user_id: str | None = None,
+        screen_name: str | None = None,
+        count: int = 5000,
+        cursor: str | None = None
+    ) -> Result[int]:
+        """
+        Fetches the IDs of the friends (following users) of a specified user.
+
+        Parameters
+        ----------
+        user_id : :class:`str` | None, default=None
+            The ID of the user for whom to return results.
+        screen_name : :class:`str` | None, default=None
+            The screen name of the user for whom to return results.
+        count : :class:`int`, default=5000
+            The maximum number of IDs to retrieve.
+
+        Returns
+        -------
+        :class:`Result`[:class:`int`]
+            A Result object containing the IDs of the friends.
+        """
+        return await self._get_friendship_ids(
+            user_id,
+            screen_name,
+            count,
+            Endpoint.FRIENDS_IDS,
+            cursor
+        )
+
     async def _send_dm(
         self,
         conversation_id: str,
         text: str,
         media_id: str | None,
         reply_to: str | None
     ) -> dict:
```

### Comparing `twikit-1.6.2/twikit/twikit_async/community.py` & `twikit-1.6.4/twikit/twikit_async/community.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/errors.py` & `twikit-1.6.4/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/group.py` & `twikit-1.6.4/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/http.py` & `twikit-1.6.4/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/list.py` & `twikit-1.6.4/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/message.py` & `twikit-1.6.4/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/notification.py` & `twikit-1.6.4/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/streaming.py` & `twikit-1.6.4/twikit/twikit_async/streaming.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/trend.py` & `twikit-1.6.4/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/tweet.py` & `twikit-1.6.4/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/user.py` & `twikit-1.6.4/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/twikit_async/utils.py` & `twikit-1.6.4/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/user.py` & `twikit-1.6.4/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.6.2/twikit/utils.py` & `twikit-1.6.4/twikit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,16 +223,21 @@
     CREATE_BOOKMARK = 'https://twitter.com/i/api/graphql/aoDbu3RHznuiSkQ9aNM67Q/CreateBookmark'
     DELETE_BOOKMARK = 'https://twitter.com/i/api/graphql/Wlmlj2-xzyS1GN3a6cj-mQ/DeleteBookmark'
     CREATE_FRIENDSHIPS = 'https://twitter.com/i/api/1.1/friendships/create.json'
     DESTROY_FRIENDSHIPS = 'https://twitter.com/i/api/1.1/friendships/destroy.json'
     HOME_TIMELINE = 'https://twitter.com/i/api/graphql/-X_hcgQzmHGl29-UXxz4sw/HomeTimeline'
     HOME_LATEST_TIMELINE = 'https://twitter.com/i/api/graphql/U0cdisy7QFIoTfu3-Okw0A/HomeLatestTimeline'
     FOLLOWERS = 'https://twitter.com/i/api/graphql/gC_lyAxZOptAMLCJX5UhWw/Followers'
+    FOLLOWERS2 = 'https://api.twitter.com/1.1/followers/list.json'
+    FOLLOWERS_IDS = 'https://api.twitter.com/1.1/followers/ids.json'
+    FRIENDS_IDS = 'https://api.twitter.com/1.1/friends/ids.json'
+    INCOMING_FRIENDSHIPS = 'https://api.twitter.com/1.1/friendships/incoming.json'
     BLUE_VERIFIED_FOLLOWERS = 'https://twitter.com/i/api/graphql/VmIlPJNEDVQ29HfzIhV4mw/BlueVerifiedFollowers'
     FOLLOWING = 'https://twitter.com/i/api/graphql/2vUj-_Ek-UmBVDNtd8OnQA/Following'
+    FOLLOWING2 = 'https://api.twitter.com/1.1/friends/list.json'
     FOLLOWERS_YOU_KNOW = 'https://twitter.com/i/api/graphql/f2tbuGNjfOE8mNUO5itMew/FollowersYouKnow'
     SUBSCRIPTIONS = 'https://twitter.com/i/api/graphql/Wsm5ZTCYtg2eH7mXAXPIgw/UserCreatorSubscriptions'
     SEND_DM = 'https://twitter.com/i/api/1.1/dm/new2.json'
     DELETE_DM = 'https://twitter.com/i/api/graphql/BJ6DtxA2llfjnRoRjaiIiw/DMMessageDeleteMutation'
     INBOX_INITIAL_STATE = 'https://twitter.com/i/api/1.1/dm/inbox_initial_state.json'
     CONVERSATION = 'https://twitter.com/i/api/1.1/dm/conversation/{}.json'
     CREATE_SCHEDULED_TWEET = 'https://twitter.com/i/api/graphql/LCVzRQGxOaGnOnYH01NQXg/CreateScheduledTweet'
@@ -288,14 +293,17 @@
     CREATE_BOOKMARK_FOLDER = 'https://twitter.com/i/api/graphql/6Xxqpq8TM_CREYiuof_h5w/createBookmarkFolder'
     BOOKMARK_FOLDER_TIMELINE = 'https://twitter.com/i/api/graphql/8HoabOvl7jl9IC1Aixj-vg/BookmarkFolderTimeline'
     BOOKMARK_TO_FOLDER = 'https://twitter.com/i/api/graphql/4KHZvvNbHNf07bsgnL9gWA/bookmarkTweetToFolder'
     PLACE_TRENDS = 'https://api.twitter.com/1.1/trends/place.json'
     AVAILABLE_LOCATIONS = 'https://api.twitter.com/1.1/trends/available.json'
     EVENTS = 'https://api.twitter.com/live_pipeline/events'
     UPDATE_SUBSCRIPTIONS = 'https://api.twitter.com/1.1/live_pipeline/update_subscriptions'
+    REVERSE_GEOCODE = 'https://api.twitter.com/1.1/geo/reverse_geocode.json'
+    SEARCH_GEO = 'https://api.twitter.com/1.1/geo/search.json'
+    PLACE_BY_ID = 'https://api.twitter.com/1.1/geo/id/{}.json'
 
 T = TypeVar('T')
 
 
 class Result(Generic[T]):
     """
     This class is for storing multiple results.
```

### Comparing `twikit-1.6.2/twikit.egg-info/PKG-INFO` & `twikit-1.6.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,60 @@
-Metadata-Version: 2.1
-Name: twikit
-Version: 1.6.2
-Summary: Twitter API wrapper for python with **no API key required**.
-Home-page: https://github.com/d60/twikit
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <img  src="https://i.imgur.com/iJe6rsZ.png"  width="500">
 
 
 
 ![Number of GitHub stars](https://img.shields.io/github/stars/d60/twikit)
 ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/d60/twikit)
 ![Version](https://img.shields.io/pypi/v/twikit?label=PyPI)
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Create%20your%20own%20Twitter%20bot%20for%20free%20with%20%22Twikit%22!%20%23python%20%23twitter%20%23twikit%20%23programming%20%23github%20%23bot&url=https%3A%2F%2Fgithub.com%2Fd60%2Ftwikit)
 [![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/nCrByrr8cX)
 [![BuyMeACoffee](https://img.shields.io/badge/-buy_me_a%C2%A0coffee-gray?logo=buy-me-a-coffee)](https://www.buymeacoffee.com/d60py)
 
+[[日本語](https://github.com/d60/twikit/blob/main/README-ja.md)]
+[[中文](https://github.com/d60/twikit/blob/main/README-zh.md)]
 
 # Twikit <img height="35"  src="https://i.imgur.com/9HSdIl4.png"  valign="bottom">
 
-simple API wrapper to interact with twitter's unofficial API.
+A Simple Twitter API Scraper
 
-You can log in to Twitter using your account username, email address and password and use most features on Twitter, such as posting and retrieving tweets, liking and following users.
+You can use functions such as posting or searching for tweets without an API key using this library.
 
 - [Documentation (English)](https://twikit.readthedocs.io/en/latest/twikit.html)
 
 - [Async Documentation](https://twikit.readthedocs.io/en/latest/twikit.twikit_async.html)
 
 
-
-If you have any questions, you can ask on [Discord](https://discord.gg/nCrByrr8cX).
+[Discord](https://discord.gg/nCrByrr8cX)
 
 
 
 ## Features
 
 ### No API Key Required
 
-This library uses the unofficial API, therefore does **not require an API key**.
+This library uses scraping and does not require an API key.
 
-### Completely Free
+### Free
 
-This library is completely free to use.
+This library is free to use.
 
 ### Both Synchronous and Asynchronous Support
 
-Whether you prefer **synchronous** or **asynchronous** programming,
-
-Twikit supports both, providing flexibility for different use cases.
+Twikit supports both synchronous and asynchronous.
 
 
 ## Functionality
 
-This library allows you to perform various Twitter-related actions, including:
+By using Twikit, you can access functionalities such as the following:
 
--  **Create tweets**
+-  Create tweets
 
--  **Search tweets**
+-  Search tweets
 
--  **Retrieve trending topics**
+-  Retrieve trending topics
 
 - etc...
 
 
 
 ## Installing
 
@@ -87,15 +76,14 @@
 USERNAME = 'example_user'
 EMAIL = 'email@example.com'
 PASSWORD = 'password0000'
 
 # Initialize client
 client = Client('en-US')
 
-# Login to the service with provided user credentials
 client.login(
     auth_info_1=USERNAME ,
     auth_info_2=EMAIL,
     password=PASSWORD
 )
 ```
 
@@ -112,15 +100,15 @@
 client.create_tweet(
     text='Example Tweet',
     media_ids=media_ids
 )
 
 ```
 
-**Search the latest tweets based on a keywords**
+**Search the latest tweets based on a keyword**
 ```python
 tweets = client.search_tweet('python', 'Latest')
 
 for tweet in tweets:
     print(
         tweet.user.name,
         tweet.text,
@@ -136,14 +124,10 @@
     print(tweet.text)
 ```
 
 More Examples: [examples](https://github.com/d60/twikit/tree/main/examples) <br>
 
 ## Contributing
 
-I would like to hear your thoughts and suggestions.
-
-If you have any features you'd like to see added or encounter any issues,
-
-please let me know in the [issues](https://github.com/d60/twikit/issues) section.
+If you encounter any bugs or issues, please report them on [issues](https://github.com/d60/twikit/issues).
 
-Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library⭐! Thank you very much!
+Additionally, if you find this library useful, I would appreciate it if you would star this repository or share this library.
```

### Comparing `twikit-1.6.2/twikit.egg-info/SOURCES.txt` & `twikit-1.6.4/twikit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 twikit/__init__.py
 twikit/bookmark.py
 twikit/client.py
 twikit/community.py
 twikit/errors.py
+twikit/geo.py
 twikit/group.py
 twikit/http.py
 twikit/list.py
 twikit/message.py
 twikit/notification.py
 twikit/py.typed
 twikit/streaming.py
@@ -23,14 +24,15 @@
 twikit.egg-info/requires.txt
 twikit.egg-info/top_level.txt
 twikit/twikit_async/__init__.py
 twikit/twikit_async/bookmark.py
 twikit/twikit_async/client.py
 twikit/twikit_async/community.py
 twikit/twikit_async/errors.py
+twikit/twikit_async/geo.py
 twikit/twikit_async/group.py
 twikit/twikit_async/http.py
 twikit/twikit_async/list.py
 twikit/twikit_async/message.py
 twikit/twikit_async/notification.py
 twikit/twikit_async/streaming.py
 twikit/twikit_async/trend.py
```

