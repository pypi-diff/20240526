# Comparing `tmp/weaver-ai-tools-0.0.1.tar.gz` & `tmp/weaver-ai-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaver-ai-tools-0.0.1.tar", last modified: Sun May 26 07:37:53 2024, max compression
+gzip compressed data, was "weaver-ai-tools-0.0.2.tar", last modified: Sun May 26 08:22:51 2024, max compression
```

## Comparing `weaver-ai-tools-0.0.1.tar` & `weaver-ai-tools-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:37:53.538791 weaver-ai-tools-0.0.1/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-05-26 07:37:53.538690 weaver-ai-tools-0.0.1/PKG-INFO
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       38 2024-05-26 07:37:53.538836 weaver-ai-tools-0.0.1/setup.cfg
--rw-r--r--   0 artemmeahkov   (501) staff       (20)      158 2024-05-26 07:25:50.000000 weaver-ai-tools-0.0.1/setup.py
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:37:53.538114 weaver-ai-tools-0.0.1/weaver-ai-tools/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:19:50.000000 weaver-ai-tools-0.0.1/weaver-ai-tools/__init__.py
-drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:37:53.538547 weaver-ai-tools-0.0.1/weaver_ai_tools.egg-info/
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-05-26 07:37:53.000000 weaver-ai-tools-0.0.1/weaver_ai_tools.egg-info/PKG-INFO
--rw-r--r--   0 artemmeahkov   (501) staff       (20)      192 2024-05-26 07:37:53.000000 weaver-ai-tools-0.0.1/weaver_ai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 artemmeahkov   (501) staff       (20)        1 2024-05-26 07:37:53.000000 weaver-ai-tools-0.0.1/weaver_ai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 artemmeahkov   (501) staff       (20)       16 2024-05-26 07:37:53.000000 weaver-ai-tools-0.0.1/weaver_ai_tools.egg-info/top_level.txt
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 08:22:51.231489 weaver-ai-tools-0.0.2/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-05-26 08:22:51.231311 weaver-ai-tools-0.0.2/PKG-INFO
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       38 2024-05-26 08:22:51.231534 weaver-ai-tools-0.0.2/setup.cfg
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)      158 2024-05-26 08:22:38.000000 weaver-ai-tools-0.0.2/setup.py
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 08:22:51.230282 weaver-ai-tools-0.0.2/weaver_ai_tools/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 07:19:50.000000 weaver-ai-tools-0.0.2/weaver_ai_tools/__init__.py
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 08:22:51.231148 weaver-ai-tools-0.0.2/weaver_ai_tools/v1/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       73 2024-05-26 08:14:21.000000 weaver-ai-tools-0.0.2/weaver_ai_tools/v1/__init__.py
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       18 2024-05-26 07:25:43.000000 weaver-ai-tools-0.0.2/weaver_ai_tools/v1/config.py
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)      137 2024-05-26 08:21:34.000000 weaver-ai-tools-0.0.2/weaver_ai_tools/v1/functions.py
+drwxr-xr-x   0 artemmeahkov   (501) staff       (20)        0 2024-05-26 08:22:51.230785 weaver-ai-tools-0.0.2/weaver_ai_tools.egg-info/
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       59 2024-05-26 08:22:51.000000 weaver-ai-tools-0.0.2/weaver_ai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)      284 2024-05-26 08:22:51.000000 weaver-ai-tools-0.0.2/weaver_ai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)        1 2024-05-26 08:22:51.000000 weaver-ai-tools-0.0.2/weaver_ai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 artemmeahkov   (501) staff       (20)       16 2024-05-26 08:22:51.000000 weaver-ai-tools-0.0.2/weaver_ai_tools.egg-info/top_level.txt
```

