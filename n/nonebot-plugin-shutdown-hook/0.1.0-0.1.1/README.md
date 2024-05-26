# Comparing `tmp/nonebot_plugin_shutdown_hook-0.1.0.tar.gz` & `tmp/nonebot_plugin_shutdown_hook-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_shutdown_hook-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_shutdown_hook-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_shutdown_hook-0.1.0.tar` & `nonebot_plugin_shutdown_hook-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3778 2024-05-26 14:07:34.189109 nonebot_plugin_shutdown_hook-0.1.0/nonebot_plugin_shutdown_hook/__init__.py
--rw-r--r--   0        0        0     1483 2024-05-26 14:42:06.696303 nonebot_plugin_shutdown_hook-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1189 2024-05-26 14:11:52.969279 nonebot_plugin_shutdown_hook-0.1.0/README.md
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 nonebot_plugin_shutdown_hook-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3778 2024-05-26 14:07:34.189109 nonebot_plugin_shutdown_hook-0.1.1/nonebot_plugin_shutdown_hook/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-26 14:56:00.237127 nonebot_plugin_shutdown_hook-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1189 2024-05-26 14:11:52.969279 nonebot_plugin_shutdown_hook-0.1.1/README.md
+-rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 nonebot_plugin_shutdown_hook-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_shutdown_hook-0.1.0/nonebot_plugin_shutdown_hook/__init__.py` & `nonebot_plugin_shutdown_hook-0.1.1/nonebot_plugin_shutdown_hook/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shutdown_hook-0.1.0/pyproject.toml` & `nonebot_plugin_shutdown_hook-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [tool.poetry]
 name = "nonebot-plugin-shutdown-hook"
-version = "0.1.0"
+version = "0.1.1"
 description = "高优先级关闭信号钩子插件"
 authors = ["Sclock <1342810270@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Sclock/nonebot-plugin-shutdown-hook"
 repository = "https://github.com/Sclock/nonebot-plugin-shutdown-hook"
 documentation = "https://github.com/Sclock/nonebot-plugin-shutdown-hook"
 keywords = ["nonebot", "plugin", "shutdown", "hook"]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
+uvicor = ">=0.20.0"
 nonebot2 = ">=2.0.0"
 
 [tool.poetry.dev-dependencies]
-nonebot-adapter-onebot = ">=2.4.3"
+uvicor = ">=0.20.0"
 nonebot2 = {extras = ["fastapi"], version = ">=2.3.0"}
 
 [build-system]
 requires = ["pdm-backend"]
 build-backend = "pdm.backend"
 
 [tool.pdm.build]
```

### Comparing `nonebot_plugin_shutdown_hook-0.1.0/README.md` & `nonebot_plugin_shutdown_hook-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_shutdown_hook-0.1.0/PKG-INFO` & `nonebot_plugin_shutdown_hook-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-shutdown-hook
-Version: 0.1.0
+Version: 0.1.1
 Summary: 高优先级关闭信号钩子插件
 Home-page: https://github.com/Sclock/nonebot-plugin-shutdown-hook
 License: MIT
 Keywords: nonebot,plugin,shutdown,hook
 Author: Sclock
 Author-email: 1342810270@qq.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nonebot2 (>=2.0.0)
+Requires-Dist: uvicor (>=0.20.0)
 Project-URL: Documentation, https://github.com/Sclock/nonebot-plugin-shutdown-hook
 Project-URL: Repository, https://github.com/Sclock/nonebot-plugin-shutdown-hook
 Description-Content-Type: text/markdown
 
 # nonebot-plugin-shutdown-hook
 
 该插件提供一个高优先级关闭信号钩子,用于在关闭时,Bot断开之前执行一些操作
```

