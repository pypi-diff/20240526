# Comparing `tmp/wi1-bot-1.4.3.tar.gz` & `tmp/wi1-bot-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wi1-bot-1.4.3.tar", last modified: Sat Apr  6 03:35:26 2024, max compression
+gzip compressed data, was "wi1-bot-1.4.4.tar", last modified: Sun May 26 05:31:28 2024, max compression
```

## Comparing `wi1-bot-1.4.3.tar` & `wi1-bot-1.4.4.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.965023 wi1-bot-1.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.969023 wi1-bot-1.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.969023 wi1-bot-1.4.3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.969023 wi1-bot-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/tests/movie_downloaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.969023 wi1-bot-1.4.3/wi1_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/wi1_bot/arr/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/arr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/arr/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/arr/episode.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/arr/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/arr/radarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/arr/sonarr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/wi1_bot/discord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/discord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/wi1_bot/discord/cogs/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/discord/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/discord/cogs/movie.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/discord/cogs/series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/discord/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/push.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/wi1_bot/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/scripts/add_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/scripts/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/scripts/transcode_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/wi1_bot/transcoder/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/transcoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/transcoder/transcode_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/transcoder/transcoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-06 03:35:19.000000 wi1-bot-1.4.3/wi1_bot/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.973024 wi1-bot-1.4.3/wi1_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 03:35:26.000000 wi1-bot-1.4.3/wi1_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.758413 wi1-bot-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.750413 wi1-bot-1.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.750413 wi1-bot-1.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-26 05:31:28.758413 wi1-bot-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 05:31:28.758413 wi1-bot-1.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/tests/movie_downloaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 05:31:27.000000 wi1-bot-1.4.4/wi1_bot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/arr/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/episode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/radarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/arr/sonarr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/discord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/discord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/cogs/movie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/cogs/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/discord/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/push.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/add_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/scripts/transcode_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot/transcoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/transcoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/transcoder/transcode_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8788 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/transcoder/transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-26 05:31:22.000000 wi1-bot-1.4.4/wi1_bot/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 05:31:28.754413 wi1-bot-1.4.4/wi1_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-26 05:31:28.000000 wi1-bot-1.4.4/wi1_bot.egg-info/top_level.txt
```

### Comparing `wi1-bot-1.4.3/.github/workflows/pypi-publish.yml` & `wi1-bot-1.4.4/.github/workflows/pypi-publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name: Upload to PyPI
 
 on:
   push:
     tags:
-      - "*"
+      - "v*"
 
 permissions:
   contents: read
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
```

### Comparing `wi1-bot-1.4.3/LICENSE` & `wi1-bot-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/PKG-INFO` & `wi1-bot-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.3
+Version: 1.4.4
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
         
@@ -53,14 +53,15 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
+- use sqlite
 - have config.discord.users be a dict with 'quotas' and 'name' for *arr tags
 - Better pushover notifications
   - Failures for pretty much everything
   - Notifications for grabs/downloads of personal watchlist
 - Tag user who added movie when it's downloaded
   - Would replace Radarr/Sonarr's Discord webhooks
   - !notify \<query\> to also be tagged when a movie/show someone else added is downloaded
```

### Comparing `wi1-bot-1.4.3/README.md` & `wi1-bot-1.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
+- use sqlite
 - have config.discord.users be a dict with 'quotas' and 'name' for *arr tags
 - Better pushover notifications
   - Failures for pretty much everything
   - Notifications for grabs/downloads of personal watchlist
 - Tag user who added movie when it's downloaded
   - Would replace Radarr/Sonarr's Discord webhooks
   - !notify \<query\> to also be tagged when a movie/show someone else added is downloaded
```

### Comparing `wi1-bot-1.4.3/config.yaml.template` & `wi1-bot-1.4.4/config.yaml.template`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/pyproject.toml` & `wi1-bot-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/arr/download.py` & `wi1-bot-1.4.4/wi1_bot/arr/download.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/arr/episode.py` & `wi1-bot-1.4.4/wi1_bot/arr/episode.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/arr/movie.py` & `wi1-bot-1.4.4/wi1_bot/arr/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/arr/radarr.py` & `wi1-bot-1.4.4/wi1_bot/arr/radarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/arr/sonarr.py` & `wi1-bot-1.4.4/wi1_bot/arr/sonarr.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/config.py` & `wi1-bot-1.4.4/wi1_bot/config.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/discord/bot.py` & `wi1-bot-1.4.4/wi1_bot/discord/bot.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/discord/cogs/movie.py` & `wi1-bot-1.4.4/wi1_bot/discord/cogs/movie.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/discord/cogs/series.py` & `wi1-bot-1.4.4/wi1_bot/discord/cogs/series.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/discord/helpers.py` & `wi1-bot-1.4.4/wi1_bot/discord/helpers.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/push.py` & `wi1-bot-1.4.4/wi1_bot/push.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/scripts/add_tag.py` & `wi1-bot-1.4.4/wi1_bot/scripts/add_tag.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/scripts/start.py` & `wi1-bot-1.4.4/wi1_bot/scripts/start.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/scripts/transcode_item.py` & `wi1-bot-1.4.4/wi1_bot/scripts/transcode_item.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/transcoder/transcode_queue.py` & `wi1-bot-1.4.4/wi1_bot/transcoder/transcode_queue.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot/transcoder/transcoder.py` & `wi1-bot-1.4.4/wi1_bot/transcoder/transcoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,18 @@
                     last_output = line.strip()
 
             status = proc.wait()
 
             if status != 0:
                 self.logger.error(f"ffmpeg failed (status {status}): {last_output}")
 
-                if "No such file or directory" in last_output:
+                if (
+                    "No such file or directory" in last_output
+                    and "shared object file" not in last_output
+                ):
                     self.logger.debug(
                         f"file does not exist: {path}, skipping transcoding"
                     )
                     raise FileNotFoundError
 
                 if "received signal 15" in last_output:
                     self.logger.debug(
```

### Comparing `wi1-bot-1.4.3/wi1_bot/webhook.py` & `wi1-bot-1.4.4/wi1_bot/webhook.py`

 * *Files identical despite different names*

### Comparing `wi1-bot-1.4.3/wi1_bot.egg-info/PKG-INFO` & `wi1-bot-1.4.4/wi1_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wi1-bot
-Version: 1.4.3
+Version: 1.4.4
 Summary: Discord bot for Radarr/Sonarr integration
 Home-page: https://github.com/wthueb/wi1-bot
 Author-email: William Huebner <wilhueb@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 William Huebner
         
@@ -53,14 +53,15 @@
 3. `pip install -e .[dev]`
 4. `pre-commit install`
 
 Requires Python >=3.10.
 
 ### TODO
 
+- use sqlite
 - have config.discord.users be a dict with 'quotas' and 'name' for *arr tags
 - Better pushover notifications
   - Failures for pretty much everything
   - Notifications for grabs/downloads of personal watchlist
 - Tag user who added movie when it's downloaded
   - Would replace Radarr/Sonarr's Discord webhooks
   - !notify \<query\> to also be tagged when a movie/show someone else added is downloaded
```

### Comparing `wi1-bot-1.4.3/wi1_bot.egg-info/SOURCES.txt` & `wi1-bot-1.4.4/wi1_bot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+.dockerignore
 .gitignore
 .pre-commit-config.yaml
+Dockerfile
 LICENSE
 README.md
+compose.yaml
 config.yaml.template
 pyproject.toml
 setup.cfg
 .github/workflows/pypi-publish.yml
 .vscode/launch.json
 .vscode/settings.json
 tests/movie_downloaded.py
```

