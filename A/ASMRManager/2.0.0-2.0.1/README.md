# Comparing `tmp/asmrmanager-2.0.0.tar.gz` & `tmp/asmrmanager-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmrmanager-2.0.0.tar", last modified: Fri Apr 19 17:51:35 2024, max compression
+gzip compressed data, was "asmrmanager-2.0.1.tar", last modified: Sun May 26 18:01:22 2024, max compression
```

## Comparing `asmrmanager-2.0.0.tar` & `asmrmanager-2.0.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1065 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/LICENSE
--rw-r--r--   0        0        0     7221 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/README.md
--rw-r--r--   0        0        0      269 2023-12-29 06:07:22.402888 asmrmanager-2.0.0/asmrmanager/__init__.py
--rw-r--r--   0        0        0       46 2024-01-30 08:57:30.179230 asmrmanager-2.0.0/asmrmanager/__main__.py
--rw-r--r--   0        0        0       21 2024-04-19 17:51:35.292944 asmrmanager-2.0.0/asmrmanager/_version.py
--rw-r--r--   0        0        0    14684 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/asmrmanager/cli/core.py
--rw-r--r--   0        0        0     5720 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/asmrmanager/cli/dl.py
--rw-r--r--   0        0        0     6292 2024-04-19 17:50:58.539612 asmrmanager-2.0.0/asmrmanager/cli/file.py
--rw-r--r--   0        0        0      612 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/hold.py
--rw-r--r--   0        0        0     2274 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/info.py
--rw-r--r--   0        0        0     2060 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/main.py
--rw-r--r--   0        0        0     2353 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/pl.py
--rw-r--r--   0        0        0     1076 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/play.py
--rw-r--r--   0        0        0     1599 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/query.py
--rw-r--r--   0        0        0     1008 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/review.py
--rw-r--r--   0        0        0     2140 2024-01-13 17:33:20.948158 asmrmanager-2.0.0/asmrmanager/cli/sql.py
--rw-r--r--   0        0        0     1768 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/utils.py
--rw-r--r--   0        0        0     1934 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/view.py
--rw-r--r--   0        0        0      971 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/cli/which.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/__init__.py
--rw-r--r--   0        0        0      821 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/browse_params.py
--rw-r--r--   0        0        0      527 2023-12-21 14:14:16.443072 asmrmanager-2.0.0/asmrmanager/common/download_params.py
--rw-r--r--   0        0        0     1115 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/common/fileconverter.py
--rw-r--r--   0        0        0      612 2024-04-09 08:45:58.879878 asmrmanager-2.0.0/asmrmanager/common/output.py
--rw-r--r--   0        0        0      719 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/parse_filter.py
--rw-r--r--   0        0        0     1768 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/common/rj_parse.py
--rw-r--r--   0        0        0      913 2024-03-29 06:19:00.412674 asmrmanager-2.0.0/asmrmanager/common/select.py
--rw-r--r--   0        0        0      894 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/common/types.py
--rw-r--r--   0        0        0     1331 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/common/vtt2lrc.py
--rw-r--r--   0        0        0     2637 2024-03-14 05:43:28.099361 asmrmanager-2.0.0/asmrmanager/config.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/database.py
--rw-r--r--   0        0        0      343 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/engine.py
--rw-r--r--   0        0        0     5793 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/manage.py
--rw-r--r--   0        0        0      619 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/orm_type.py
--rw-r--r--   0        0        0     1485 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/database/q_func.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/utils/__init__.py
--rw-r--r--   0        0        0      480 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/utils/add2db.py
--rw-r--r--   0        0        0     1290 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/database/utils/uuid_sqlite.py
--rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/filemanager/__init__.py
--rw-r--r--   0        0        0      312 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/filemanager/appdirs_.py
--rw-r--r--   0        0        0      108 2023-12-17 15:01:39.136126 asmrmanager-2.0.0/asmrmanager/filemanager/exceptions.py
--rw-r--r--   0        0        0      477 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/file_zipper.py
--rw-r--r--   0        0        0    12030 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/filemanager/manager.py
--rw-r--r--   0        0        0     3194 2024-03-14 05:39:35.879370 asmrmanager-2.0.0/asmrmanager/filemanager/resources/config.example.toml
--rw-r--r--   0        0        0       65 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/circle_name.sql
--rw-r--r--   0        0        0      425 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/score.sql
--rw-r--r--   0        0        0     1663 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/search.sql
--rw-r--r--   0        0        0       92 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/tags.sql
--rw-r--r--   0        0        0      602 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/test.sql
--rw-r--r--   0        0        0       53 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/vas.sql
--rw-r--r--   0        0        0     1579 2024-03-29 06:23:40.599330 asmrmanager-2.0.0/asmrmanager/filemanager/utils.py
--rw-r--r--   0        0        0     1038 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/logger/__init__.py
--rw-r--r--   0        0        0       68 2023-12-24 08:26:10.649470 asmrmanager-2.0.0/asmrmanager/lrcplayer/__init__.py
--rw-r--r--   0        0        0     2318 2023-12-31 11:19:36.902077 asmrmanager-2.0.0/asmrmanager/lrcplayer/lrcparse.py
--rw-r--r--   0        0        0      328 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/lrcplayer/main.css
--rw-r--r--   0        0        0     5379 2024-04-08 06:16:03.019693 asmrmanager-2.0.0/asmrmanager/lrcplayer/main.py
--rw-r--r--   0        0        0     3845 2024-04-05 09:59:01.476032 asmrmanager-2.0.0/asmrmanager/lrcplayer/player/base.py
--rw-r--r--   0        0        0     4767 2024-04-08 06:16:03.006360 asmrmanager-2.0.0/asmrmanager/lrcplayer/player/mpdplayer.py
--rw-r--r--   0        0        0     1777 2023-12-31 11:19:36.902077 asmrmanager-2.0.0/asmrmanager/lrcplayer/player/pygameplayer.py
--rw-r--r--   0        0        0       75 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/spider/__init__.py
--rw-r--r--   0        0        0     5368 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/spider/asmrapi.py
--rw-r--r--   0        0        0    10001 2024-04-19 17:50:58.542946 asmrmanager-2.0.0/asmrmanager/spider/downloader.py
--rw-r--r--   0        0        0     9594 2024-04-19 17:50:58.546279 asmrmanager-2.0.0/asmrmanager/spider/interface.py
--rw-r--r--   0        0        0     1844 2024-04-19 17:50:58.546279 asmrmanager-2.0.0/asmrmanager/spider/playlist.py
--rw-r--r--   0        0        0     4092 2023-12-17 15:01:39.139459 asmrmanager-2.0.0/asmrmanager/spider/utils/IDMHelper.py
--rw-r--r--   0        0        0     1355 2024-03-30 06:44:45.769287 asmrmanager-2.0.0/asmrmanager/spider/utils/aria2_downloader.py
--rw-r--r--   0        0        0     1554 2024-04-19 17:51:35.296278 asmrmanager-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8632 1970-01-01 00:00:00.000000 asmrmanager-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/LICENSE
+-rw-r--r--   0        0        0     7221 2024-04-19 17:50:58.539612 asmrmanager-2.0.1/README.md
+-rw-r--r--   0        0        0      269 2023-12-29 06:07:22.402888 asmrmanager-2.0.1/asmrmanager/__init__.py
+-rw-r--r--   0        0        0       46 2024-01-30 08:57:30.179230 asmrmanager-2.0.1/asmrmanager/__main__.py
+-rw-r--r--   0        0        0       21 2024-05-26 18:01:22.296649 asmrmanager-2.0.1/asmrmanager/_version.py
+-rw-r--r--   0        0        0    14684 2024-04-19 17:50:58.539612 asmrmanager-2.0.1/asmrmanager/cli/core.py
+-rw-r--r--   0        0        0     5720 2024-05-23 16:20:50.349004 asmrmanager-2.0.1/asmrmanager/cli/dl.py
+-rw-r--r--   0        0        0     6292 2024-04-19 17:50:58.539612 asmrmanager-2.0.1/asmrmanager/cli/file.py
+-rw-r--r--   0        0        0      612 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/hold.py
+-rw-r--r--   0        0        0     2274 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/info.py
+-rw-r--r--   0        0        0     2060 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/main.py
+-rw-r--r--   0        0        0     2353 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/pl.py
+-rw-r--r--   0        0        0     1076 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/play.py
+-rw-r--r--   0        0        0     1599 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/query.py
+-rw-r--r--   0        0        0     1008 2024-04-24 02:39:13.549599 asmrmanager-2.0.1/asmrmanager/cli/review.py
+-rw-r--r--   0        0        0     2140 2024-01-13 17:33:20.948158 asmrmanager-2.0.1/asmrmanager/cli/sql.py
+-rw-r--r--   0        0        0     1768 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/utils.py
+-rw-r--r--   0        0        0     1934 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/cli/view.py
+-rw-r--r--   0        0        0      975 2024-04-24 02:35:35.659608 asmrmanager-2.0.1/asmrmanager/cli/which.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/common/__init__.py
+-rw-r--r--   0        0        0      821 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/common/browse_params.py
+-rw-r--r--   0        0        0      527 2023-12-21 14:14:16.443072 asmrmanager-2.0.1/asmrmanager/common/download_params.py
+-rw-r--r--   0        0        0     1115 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/common/fileconverter.py
+-rw-r--r--   0        0        0      612 2024-04-09 08:45:58.879878 asmrmanager-2.0.1/asmrmanager/common/output.py
+-rw-r--r--   0        0        0      719 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/common/parse_filter.py
+-rw-r--r--   0        0        0     1768 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/common/rj_parse.py
+-rw-r--r--   0        0        0      913 2024-03-29 06:19:00.412674 asmrmanager-2.0.1/asmrmanager/common/select.py
+-rw-r--r--   0        0        0      894 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/common/types.py
+-rw-r--r--   0        0        0     1331 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/common/vtt2lrc.py
+-rw-r--r--   0        0        0     2637 2024-03-14 05:43:28.099361 asmrmanager-2.0.1/asmrmanager/config.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/database/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/database/database.py
+-rw-r--r--   0        0        0      343 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/database/engine.py
+-rw-r--r--   0        0        0     5793 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/database/manage.py
+-rw-r--r--   0        0        0      619 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/database/orm_type.py
+-rw-r--r--   0        0        0     1503 2024-04-24 02:41:12.109594 asmrmanager-2.0.1/asmrmanager/database/q_func.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/database/utils/__init__.py
+-rw-r--r--   0        0        0      480 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/database/utils/add2db.py
+-rw-r--r--   0        0        0     1290 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/database/utils/uuid_sqlite.py
+-rw-r--r--   0        0        0        0 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/filemanager/__init__.py
+-rw-r--r--   0        0        0      312 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/filemanager/appdirs_.py
+-rw-r--r--   0        0        0      108 2023-12-17 15:01:39.136126 asmrmanager-2.0.1/asmrmanager/filemanager/exceptions.py
+-rw-r--r--   0        0        0      477 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/file_zipper.py
+-rw-r--r--   0        0        0    12030 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/filemanager/manager.py
+-rw-r--r--   0        0        0     3194 2024-03-14 05:39:35.879370 asmrmanager-2.0.1/asmrmanager/filemanager/resources/config.example.toml
+-rw-r--r--   0        0        0       65 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/circle_name.sql
+-rw-r--r--   0        0        0      425 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/score.sql
+-rw-r--r--   0        0        0     1663 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/search.sql
+-rw-r--r--   0        0        0       92 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/tags.sql
+-rw-r--r--   0        0        0      602 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/test.sql
+-rw-r--r--   0        0        0       53 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/vas.sql
+-rw-r--r--   0        0        0     1579 2024-03-29 06:23:40.599330 asmrmanager-2.0.1/asmrmanager/filemanager/utils.py
+-rw-r--r--   0        0        0     1038 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/logger/__init__.py
+-rw-r--r--   0        0        0       68 2023-12-24 08:26:10.649470 asmrmanager-2.0.1/asmrmanager/lrcplayer/__init__.py
+-rw-r--r--   0        0        0     2318 2023-12-31 11:19:36.902077 asmrmanager-2.0.1/asmrmanager/lrcplayer/lrcparse.py
+-rw-r--r--   0        0        0      328 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/lrcplayer/main.css
+-rw-r--r--   0        0        0     5379 2024-04-08 06:16:03.019693 asmrmanager-2.0.1/asmrmanager/lrcplayer/main.py
+-rw-r--r--   0        0        0     3845 2024-04-05 09:59:01.476032 asmrmanager-2.0.1/asmrmanager/lrcplayer/player/base.py
+-rw-r--r--   0        0        0     4767 2024-04-08 06:16:03.006360 asmrmanager-2.0.1/asmrmanager/lrcplayer/player/mpdplayer.py
+-rw-r--r--   0        0        0     1777 2023-12-31 11:19:36.902077 asmrmanager-2.0.1/asmrmanager/lrcplayer/player/pygameplayer.py
+-rw-r--r--   0        0        0       75 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/spider/__init__.py
+-rw-r--r--   0        0        0     5368 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/spider/asmrapi.py
+-rw-r--r--   0        0        0    10001 2024-04-19 17:50:58.542946 asmrmanager-2.0.1/asmrmanager/spider/downloader.py
+-rw-r--r--   0        0        0     9603 2024-05-11 09:20:34.211637 asmrmanager-2.0.1/asmrmanager/spider/interface.py
+-rw-r--r--   0        0        0     1844 2024-04-19 17:50:58.546279 asmrmanager-2.0.1/asmrmanager/spider/playlist.py
+-rw-r--r--   0        0        0     4092 2023-12-17 15:01:39.139459 asmrmanager-2.0.1/asmrmanager/spider/utils/IDMHelper.py
+-rw-r--r--   0        0        0     1355 2024-03-30 06:44:45.769287 asmrmanager-2.0.1/asmrmanager/spider/utils/aria2_downloader.py
+-rw-r--r--   0        0        0     1548 2024-05-26 18:01:22.306649 asmrmanager-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8626 1970-01-01 00:00:00.000000 asmrmanager-2.0.1/PKG-INFO
```

### Comparing `asmrmanager-2.0.0/LICENSE` & `asmrmanager-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/README.md` & `asmrmanager-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/core.py` & `asmrmanager-2.0.1/asmrmanager/cli/core.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/dl.py` & `asmrmanager-2.0.1/asmrmanager/cli/dl.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/file.py` & `asmrmanager-2.0.1/asmrmanager/cli/file.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/hold.py` & `asmrmanager-2.0.1/asmrmanager/cli/hold.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/info.py` & `asmrmanager-2.0.1/asmrmanager/cli/info.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/main.py` & `asmrmanager-2.0.1/asmrmanager/cli/main.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/pl.py` & `asmrmanager-2.0.1/asmrmanager/cli/pl.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/play.py` & `asmrmanager-2.0.1/asmrmanager/cli/play.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/query.py` & `asmrmanager-2.0.1/asmrmanager/cli/query.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/review.py` & `asmrmanager-2.0.1/asmrmanager/cli/review.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/sql.py` & `asmrmanager-2.0.1/asmrmanager/cli/sql.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/utils.py` & `asmrmanager-2.0.1/asmrmanager/cli/utils.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/view.py` & `asmrmanager-2.0.1/asmrmanager/cli/view.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/cli/which.py` & `asmrmanager-2.0.1/asmrmanager/cli/which.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from asmrmanager.logger import logger
 
 
 @click.command()
 @rj_argument("local")
 @click.option("--show", is_flag=True, default=False, show_default=True)
 def which(source_id: LocalSourceID, show: bool):
-    """Get the path from the given rj_id"""
+    """Get the path from the given source_id"""
     from asmrmanager.cli.core import fm
 
     path = str(fm.get_path(source_id))
 
     if not show:
         click.echo(path)
     else:
```

### Comparing `asmrmanager-2.0.0/asmrmanager/common/browse_params.py` & `asmrmanager-2.0.1/asmrmanager/common/browse_params.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/download_params.py` & `asmrmanager-2.0.1/asmrmanager/common/download_params.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/fileconverter.py` & `asmrmanager-2.0.1/asmrmanager/common/fileconverter.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/output.py` & `asmrmanager-2.0.1/asmrmanager/common/output.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/parse_filter.py` & `asmrmanager-2.0.1/asmrmanager/common/parse_filter.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/rj_parse.py` & `asmrmanager-2.0.1/asmrmanager/common/rj_parse.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/select.py` & `asmrmanager-2.0.1/asmrmanager/common/select.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/types.py` & `asmrmanager-2.0.1/asmrmanager/common/types.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/common/vtt2lrc.py` & `asmrmanager-2.0.1/asmrmanager/common/vtt2lrc.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/config.py` & `asmrmanager-2.0.1/asmrmanager/config.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/database/database.py` & `asmrmanager-2.0.1/asmrmanager/database/database.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/database/manage.py` & `asmrmanager-2.0.1/asmrmanager/database/manage.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/database/orm_type.py` & `asmrmanager-2.0.1/asmrmanager/database/orm_type.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/database/q_func.py` & `asmrmanager-2.0.1/asmrmanager/database/q_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
     def get_tag_name(self, tid: int):
         res = self.ss.query(Tag).filter(Tag.id == tid).one_or_none()
         if res:
             return res.name
         return None
 
-    def get_stored(self, rj_id: int):
-        res = self.ss.query(ASMR).get(rj_id)
+    def get_stored(self, source_id: LocalSourceID):
+        res = self.ss.query(ASMR).get(source_id)
         return res.stored if res is not None else None
 
     def get_local_id(self, remote_id: int) -> int | None:
         res = self.ss.query(ASMR).filter_by(remote_id=remote_id).one_or_none()
         if res:
             return typing.cast(int, res.id)
```

### Comparing `asmrmanager-2.0.0/asmrmanager/database/utils/uuid_sqlite.py` & `asmrmanager-2.0.1/asmrmanager/database/utils/uuid_sqlite.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/filemanager/manager.py` & `asmrmanager-2.0.1/asmrmanager/filemanager/manager.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/filemanager/resources/config.example.toml` & `asmrmanager-2.0.1/asmrmanager/filemanager/resources/config.example.toml`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/search.sql` & `asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/search.sql`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/filemanager/resources/sqls.example/test.sql` & `asmrmanager-2.0.1/asmrmanager/filemanager/resources/sqls.example/test.sql`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/filemanager/utils.py` & `asmrmanager-2.0.1/asmrmanager/filemanager/utils.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/logger/__init__.py` & `asmrmanager-2.0.1/asmrmanager/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/lrcplayer/lrcparse.py` & `asmrmanager-2.0.1/asmrmanager/lrcplayer/lrcparse.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/lrcplayer/main.py` & `asmrmanager-2.0.1/asmrmanager/lrcplayer/main.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/lrcplayer/player/base.py` & `asmrmanager-2.0.1/asmrmanager/lrcplayer/player/base.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/lrcplayer/player/mpdplayer.py` & `asmrmanager-2.0.1/asmrmanager/lrcplayer/player/mpdplayer.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/lrcplayer/player/pygameplayer.py` & `asmrmanager-2.0.1/asmrmanager/lrcplayer/player/pygameplayer.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/spider/asmrapi.py` & `asmrmanager-2.0.1/asmrmanager/spider/asmrapi.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/spider/downloader.py` & `asmrmanager-2.0.1/asmrmanager/spider/downloader.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/spider/interface.py` & `asmrmanager-2.0.1/asmrmanager/spider/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         super().__init__(self.downloader)
         self.id_should_download = id_should_download or (lambda _: True)
 
     async def get(self, ids: List[RemoteSourceID]):
         tasks = []
         for id_ in ids:
             if not self.id_should_download(id_):
-                logger.info(f"RJ{id_} already exists.")
+                logger.info(f"Remote ID: {id_} already exists.")
                 continue
             tasks.append(self.downloader.download(id_))
         await asyncio.gather(*tasks)
 
     async def search(
         self,
         text: str,
```

### Comparing `asmrmanager-2.0.0/asmrmanager/spider/playlist.py` & `asmrmanager-2.0.1/asmrmanager/spider/playlist.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/spider/utils/IDMHelper.py` & `asmrmanager-2.0.1/asmrmanager/spider/utils/IDMHelper.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/asmrmanager/spider/utils/aria2_downloader.py` & `asmrmanager-2.0.1/asmrmanager/spider/utils/aria2_downloader.py`

 * *Files identical despite different names*

### Comparing `asmrmanager-2.0.0/pyproject.toml` & `asmrmanager-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,17 @@
     "textual==0.26.0",
     "mutagen>=1.46.0",
     "appdirs>=1.4.4",
     "toml>=0.10.2",
     "beaupy>=3.7.2",
     "asyncstdlib>=3.12.2",
 ]
-requires-python = ">=3.10,<3.12"
+requires-python = ">=3.10"
 readme = "README.md"
-version = "2.0.0"
+version = "2.0.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/slqy123/ASMRManager"
 
@@ -51,15 +51,15 @@
 idm = [
     "comtypes>=1.2.0",
 ]
 tui = [
     "trogon==0.4.0",
 ]
 pygame = [
-    "pygame==2.4.0",
+    "pygame>=2.5.0",
 ]
 mpd = [
     "python-mpd2>=3.1.0",
 ]
 dev = [
     "black>=23.12.0",
     "autoflake>=2.2.1",
```

### Comparing `asmrmanager-2.0.0/PKG-INFO` & `asmrmanager-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ASMRManager
-Version: 2.0.0
+Version: 2.0.1
 Summary: download, manage and play the voices on asmr.one
 Keywords: asmr,downloader,music,player,manager,cli,tui,commandline,terminal
 Author-Email: SLQY <sqiyel@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/slqy123/ASMRManager
-Requires-Python: <3.12,>=3.10
+Requires-Python: >=3.10
 Requires-Dist: aiohttp>=3.8.6
 Requires-Dist: chardet>=5.1.0
 Requires-Dist: click>=8.1.3
 Requires-Dist: colorlog>=6.7.0
 Requires-Dist: pylrc==0.1.2
 Requires-Dist: rich>=13.0.0
 Requires-Dist: SQLAlchemy==2.0.10
@@ -19,15 +19,15 @@
 Requires-Dist: appdirs>=1.4.4
 Requires-Dist: toml>=0.10.2
 Requires-Dist: beaupy>=3.7.2
 Requires-Dist: asyncstdlib>=3.12.2
 Requires-Dist: aioaria2>=1.3.4; extra == "aria2"
 Requires-Dist: comtypes>=1.2.0; extra == "idm"
 Requires-Dist: trogon==0.4.0; extra == "tui"
-Requires-Dist: pygame==2.4.0; extra == "pygame"
+Requires-Dist: pygame>=2.5.0; extra == "pygame"
 Requires-Dist: python-mpd2>=3.1.0; extra == "mpd"
 Requires-Dist: black>=23.12.0; extra == "dev"
 Requires-Dist: autoflake>=2.2.1; extra == "dev"
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: pyinstrument>=4.6.2; extra == "dev"
 Requires-Dist: asmrmanager[aria2,idm,mpd,pygame,tui]; extra == "all"
 Provides-Extra: aria2
```

