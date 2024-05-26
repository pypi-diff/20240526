# Comparing `tmp/goth-0.8.0.tar.gz` & `tmp/goth-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goth-0.8.0.tar", last modified: Tue Nov  9 16:46:28 2021, max compression
+gzip compressed data, was "goth-0.9.0.tar", last modified: Wed Nov 17 14:10:52 2021, max compression
```

## Comparing `goth-0.8.0.tar` & `goth-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0    35147 2021-11-09 16:46:20.930565 goth-0.8.0/LICENSE
--rw-r--r--   0        0        0     9157 2021-11-09 16:46:20.930565 goth-0.8.0/README.md
--rw-r--r--   0        0        0       47 2021-11-09 16:46:20.930565 goth-0.8.0/goth/__init__.py
--rw-r--r--   0        0        0     3043 2021-11-09 16:46:20.930565 goth-0.8.0/goth/__main__.py
--rw-r--r--   0        0        0     4952 2021-11-09 16:46:20.930565 goth-0.8.0/goth/address.py
--rw-r--r--   0        0        0     6060 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/README.md
--rw-r--r--   0        0        0       47 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/__init__.py
--rw-r--r--   0        0        0    13803 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/api-monitor.svg
--rw-r--r--   0        0        0     7102 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/api_events.py
--rw-r--r--   0        0        0     2340 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/monitor_addon.py
--rw-r--r--   0        0        0     1100 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/nginx.conf
--rw-r--r--   0        0        0     4405 2021-11-09 16:46:20.930565 goth-0.8.0/goth/api_monitor/router_addon.py
--rw-r--r--   0        0        0     2576 2021-11-09 16:46:20.930565 goth-0.8.0/goth/assertions/README.md
--rw-r--r--   0        0        0      252 2021-11-09 16:46:20.930565 goth-0.8.0/goth/assertions/__init__.py
--rw-r--r--   0        0        0    10618 2021-11-09 16:46:20.930565 goth-0.8.0/goth/assertions/assertions.py
--rw-r--r--   0        0        0     1236 2021-11-09 16:46:20.930565 goth-0.8.0/goth/assertions/common.py
--rw-r--r--   0        0        0    13841 2021-11-09 16:46:20.930565 goth-0.8.0/goth/assertions/monitor.py
--rw-r--r--   0        0        0     1448 2021-11-09 16:46:20.930565 goth-0.8.0/goth/assertions/operators.py
--rw-r--r--   0        0        0    12156 2021-11-09 16:46:20.930565 goth-0.8.0/goth/configuration.py
--rw-r--r--   0        0        0       38 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/docker/README.md
--rw-r--r--   0        0        0     1645 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/docker/docker-compose.yml
--rw-r--r--   0        0        0     1455 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/docker/proxy-nginx.Dockerfile
--rw-r--r--   0        0        0      324 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/docker/yagna-goth-deb.Dockerfile
--rw-r--r--   0        0        0      404 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/docker/yagna-goth.Dockerfile
--rw-r--r--   0        0        0     1624 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/goth-config.yml
--rw-r--r--   0        0        0      495 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/keys/001.json
--rw-r--r--   0        0        0      495 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/keys/002.json
--rw-r--r--   0        0        0      489 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/keys/003.json
--rw-r--r--   0        0        0      141 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/provider/hardware.json
--rw-r--r--   0        0        0      876 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/provider/presets.json
--rw-r--r--   0        0        0       96 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/web-root/.gitignore
--rw-r--r--   0        0        0        3 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/web-root/params.json
--rw-r--r--   0        0        0       79 2021-11-09 16:46:20.930565 goth-0.8.0/goth/default-assets/web-root/upload/.gitignore
--rwxr-xr-x   0        0        0     7733 2021-11-09 16:46:20.930565 goth-0.8.0/goth/gftp.py
--rw-r--r--   0        0        0     2212 2021-11-09 16:46:20.930565 goth-0.8.0/goth/interactive.py
--rw-r--r--   0        0        0     1826 2021-11-09 16:46:20.930565 goth-0.8.0/goth/node.py
--rw-r--r--   0        0        0     2300 2021-11-09 16:46:20.930565 goth-0.8.0/goth/payment_config.py
--rw-r--r--   0        0        0      269 2021-11-09 16:46:20.930565 goth-0.8.0/goth/project.py
--rw-r--r--   0        0        0    12959 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/__init__.py
--rw-r--r--   0        0        0      906 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/cli/__init__.py
--rw-r--r--   0        0        0     3694 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/cli/base.py
--rw-r--r--   0        0        0      869 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/cli/typing.py
--rw-r--r--   0        0        0     2343 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/cli/yagna_app_key_cmd.py
--rw-r--r--   0        0        0     2722 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/cli/yagna_id_cmd.py
--rw-r--r--   0        0        0     3606 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/cli/yagna_payment_cmd.py
--rw-r--r--   0        0        0     6613 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/container/__init__.py
--rw-r--r--   0        0        0     7603 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/container/build.py
--rw-r--r--   0        0        0    10424 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/container/compose.py
--rw-r--r--   0        0        0     4601 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/container/payment.py
--rwxr-xr-x   0        0        0     2610 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/container/utils.py
--rw-r--r--   0        0        0     4987 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/container/yagna.py
--rw-r--r--   0        0        0    12193 2021-11-09 16:46:20.930565 goth-0.8.0/goth/runner/download/__init__.py
--rw-r--r--   0        0        0     1290 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/exceptions.py
--rw-r--r--   0        0        0     6244 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/log.py
--rw-r--r--   0        0        0     7416 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/log_monitor.py
--rw-r--r--   0        0        0    16807 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/probe/__init__.py
--rw-r--r--   0        0        0     3347 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/probe/agent.py
--rw-r--r--   0        0        0      524 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/probe/component.py
--rw-r--r--   0        0        0     9189 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/probe/mixin.py
--rw-r--r--   0        0        0     3682 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/probe/rest_client.py
--rw-r--r--   0        0        0     2217 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/process.py
--rw-r--r--   0        0        0     4209 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/proxy.py
--rw-r--r--   0        0        0     1830 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/step.py
--rw-r--r--   0        0        0     3305 2021-11-09 16:46:20.934565 goth-0.8.0/goth/runner/web_server.py
--rw-r--r--   0        0        0     1626 2021-11-09 16:46:20.934565 goth-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10740 2021-11-09 16:46:28.496231 goth-0.8.0/setup.py
--rw-r--r--   0        0        0    10498 2021-11-09 16:46:28.497117 goth-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-11-17 14:10:35.365972 goth-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9157 2021-11-17 14:10:35.365972 goth-0.9.0/README.md
+-rw-r--r--   0        0        0       47 2021-11-17 14:10:35.365972 goth-0.9.0/goth/__init__.py
+-rw-r--r--   0        0        0     3043 2021-11-17 14:10:35.365972 goth-0.9.0/goth/__main__.py
+-rw-r--r--   0        0        0     4952 2021-11-17 14:10:35.365972 goth-0.9.0/goth/address.py
+-rw-r--r--   0        0        0     6060 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/README.md
+-rw-r--r--   0        0        0       47 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/__init__.py
+-rw-r--r--   0        0        0    13803 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/api-monitor.svg
+-rw-r--r--   0        0        0     7102 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/api_events.py
+-rw-r--r--   0        0        0     2340 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/monitor_addon.py
+-rw-r--r--   0        0        0     1100 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/nginx.conf
+-rw-r--r--   0        0        0     4405 2021-11-17 14:10:35.365972 goth-0.9.0/goth/api_monitor/router_addon.py
+-rw-r--r--   0        0        0     2576 2021-11-17 14:10:35.365972 goth-0.9.0/goth/assertions/README.md
+-rw-r--r--   0        0        0      252 2021-11-17 14:10:35.365972 goth-0.9.0/goth/assertions/__init__.py
+-rw-r--r--   0        0        0    10618 2021-11-17 14:10:35.365972 goth-0.9.0/goth/assertions/assertions.py
+-rw-r--r--   0        0        0     1236 2021-11-17 14:10:35.365972 goth-0.9.0/goth/assertions/common.py
+-rw-r--r--   0        0        0    13841 2021-11-17 14:10:35.365972 goth-0.9.0/goth/assertions/monitor.py
+-rw-r--r--   0        0        0     1448 2021-11-17 14:10:35.365972 goth-0.9.0/goth/assertions/operators.py
+-rw-r--r--   0        0        0    12195 2021-11-17 14:10:35.365972 goth-0.9.0/goth/configuration.py
+-rw-r--r--   0        0        0       38 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/docker/README.md
+-rw-r--r--   0        0        0     1648 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/docker/docker-compose-hybrid-net.yml
+-rw-r--r--   0        0        0     1645 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/docker/docker-compose.yml
+-rw-r--r--   0        0        0     1455 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/docker/proxy-nginx.Dockerfile
+-rw-r--r--   0        0        0      324 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/docker/yagna-goth-deb.Dockerfile
+-rw-r--r--   0        0        0      404 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/docker/yagna-goth.Dockerfile
+-rw-r--r--   0        0        0     1723 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/goth-config.yml
+-rw-r--r--   0        0        0      495 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/keys/001.json
+-rw-r--r--   0        0        0      495 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/keys/002.json
+-rw-r--r--   0        0        0      489 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/keys/003.json
+-rw-r--r--   0        0        0      141 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/provider/hardware.json
+-rw-r--r--   0        0        0      876 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/provider/presets.json
+-rw-r--r--   0        0        0       96 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/web-root/.gitignore
+-rw-r--r--   0        0        0        3 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/web-root/params.json
+-rw-r--r--   0        0        0       79 2021-11-17 14:10:35.365972 goth-0.9.0/goth/default-assets/web-root/upload/.gitignore
+-rwxr-xr-x   0        0        0     7733 2021-11-17 14:10:35.365972 goth-0.9.0/goth/gftp.py
+-rw-r--r--   0        0        0     2212 2021-11-17 14:10:35.365972 goth-0.9.0/goth/interactive.py
+-rw-r--r--   0        0        0     1915 2021-11-17 14:10:35.365972 goth-0.9.0/goth/node.py
+-rw-r--r--   0        0        0     2678 2021-11-17 14:10:35.365972 goth-0.9.0/goth/payment_config.py
+-rw-r--r--   0        0        0      269 2021-11-17 14:10:35.365972 goth-0.9.0/goth/project.py
+-rw-r--r--   0        0        0    12959 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/__init__.py
+-rw-r--r--   0        0        0      906 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3694 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/cli/base.py
+-rw-r--r--   0        0        0      869 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/cli/typing.py
+-rw-r--r--   0        0        0     2343 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/cli/yagna_app_key_cmd.py
+-rw-r--r--   0        0        0     2722 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/cli/yagna_id_cmd.py
+-rw-r--r--   0        0        0     3606 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/cli/yagna_payment_cmd.py
+-rw-r--r--   0        0        0     6613 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/container/__init__.py
+-rw-r--r--   0        0        0     7619 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/container/build.py
+-rw-r--r--   0        0        0    10424 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/container/compose.py
+-rw-r--r--   0        0        0     4601 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/container/payment.py
+-rwxr-xr-x   0        0        0     2610 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/container/utils.py
+-rw-r--r--   0        0        0     4987 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/container/yagna.py
+-rw-r--r--   0        0        0    12193 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/download/__init__.py
+-rw-r--r--   0        0        0     1290 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/exceptions.py
+-rw-r--r--   0        0        0     6244 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/log.py
+-rw-r--r--   0        0        0     7416 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/log_monitor.py
+-rw-r--r--   0        0        0    16807 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/probe/__init__.py
+-rw-r--r--   0        0        0     3347 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/probe/agent.py
+-rw-r--r--   0        0        0      524 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/probe/component.py
+-rw-r--r--   0        0        0     9189 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/probe/mixin.py
+-rw-r--r--   0        0        0     3682 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/probe/rest_client.py
+-rw-r--r--   0        0        0     2217 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/process.py
+-rw-r--r--   0        0        0     4209 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/proxy.py
+-rw-r--r--   0        0        0     1830 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/step.py
+-rw-r--r--   0        0        0     3305 2021-11-17 14:10:35.365972 goth-0.9.0/goth/runner/web_server.py
+-rw-r--r--   0        0        0     1626 2021-11-17 14:10:35.369972 goth-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10740 2021-11-17 14:10:52.480517 goth-0.9.0/setup.py
+-rw-r--r--   0        0        0    10498 2021-11-17 14:10:52.481356 goth-0.9.0/PKG-INFO
```

### Comparing `goth-0.8.0/LICENSE` & `goth-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/README.md` & `goth-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/__main__.py` & `goth-0.9.0/goth/__main__.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/address.py` & `goth-0.9.0/goth/address.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/api_monitor/README.md` & `goth-0.9.0/goth/api_monitor/README.md`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/api_monitor/api-monitor.svg` & `goth-0.9.0/goth/api_monitor/api-monitor.svg`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/api_monitor/api_events.py` & `goth-0.9.0/goth/api_monitor/api_events.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/api_monitor/monitor_addon.py` & `goth-0.9.0/goth/api_monitor/monitor_addon.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/api_monitor/nginx.conf` & `goth-0.9.0/goth/api_monitor/nginx.conf`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/api_monitor/router_addon.py` & `goth-0.9.0/goth/api_monitor/router_addon.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/assertions/README.md` & `goth-0.9.0/goth/assertions/README.md`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/assertions/assertions.py` & `goth-0.9.0/goth/assertions/assertions.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/assertions/common.py` & `goth-0.9.0/goth/assertions/common.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/assertions/monitor.py` & `goth-0.9.0/goth/assertions/monitor.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/assertions/operators.py` & `goth-0.9.0/goth/assertions/operators.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/configuration.py` & `goth-0.9.0/goth/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     YagnaBuildEnvironment,
 )
 from goth.runner.container.payment import PaymentIdPool
 from goth.node import node_environment
 from goth.runner.probe import Probe, YagnaContainerConfig
 from goth.payment_config import get_payment_config, PaymentConfig
 
-DEFAULT_PAYMENT_CONFIG_NAME = "zksync"
+DEFAULT_PAYMENT_CONFIG_NAME = "erc20"
 """Determines PaymentConfig object that will be used for containers
 without specified "payment-config" """
 
 Override = Tuple[str, Any]
 """Type representing a single value override in a YAML config file.
 
 First element is a path within the file, e.g.: `"docker-compose.build-environment"`.
@@ -203,26 +203,25 @@
 
         docker_dir = self.get_path("docker-dir")
         assert docker_dir
 
         log_patterns = self.get("compose-log-patterns")
         log_patterns.ensure_type(dict)
 
+        compose_file = self.get("compose-file", DEFAULT_COMPOSE_FILE)
         build_env_config = self.get("build-environment")
         # `build_env_config` may be `None` if no optional build parameters
         # (binary path, commit hash etc.) are specified in the config file
         if build_env_config:
             build_env_config.ensure_type(dict)
             build_env = build_env_config.read_build_env(docker_dir)
         else:
             build_env = YagnaBuildEnvironment(docker_dir)
 
-        return ComposeConfig(
-            build_env, docker_dir / DEFAULT_COMPOSE_FILE, log_patterns.doc
-        )
+        return ComposeConfig(build_env, docker_dir / compose_file, log_patterns.doc)
 
     def read_build_env(self, docker_dir: Path) -> YagnaBuildEnvironment:
         """Read a `YagnaBuildEnvironment` instance from this parser's document."""
         self.ensure_type(dict)
 
         binary_path = self.get_path("binary-path", required=False)
         branch = self.get("branch")
```

### Comparing `goth-0.8.0/goth/default-assets/docker/docker-compose.yml` & `goth-0.9.0/goth/default-assets/docker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/default-assets/docker/proxy-nginx.Dockerfile` & `goth-0.9.0/goth/default-assets/docker/proxy-nginx.Dockerfile`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/default-assets/goth-config.yml` & `goth-0.9.0/goth/default-assets/goth-config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Note: values of keys denoting paths are resolved relative to the directory
 # in which this file is located.
 # The tokens `~` and `~user` are also replaced by the corresponding users's
 # home directory.
 
 docker-compose:
 
+  # Path to compose file to be used, relative to `docker-dir`
+  compose-file: "docker-compose.yml"
   docker-dir: "docker/"
 
   build-environment:
     # TODO:
     # For now these settings are common to all `yagna` containers.
     # In future we may want to have nodes running different versions
     # of `yagna` in the test network.
```

### Comparing `goth-0.8.0/goth/default-assets/provider/presets.json` & `goth-0.9.0/goth/default-assets/provider/presets.json`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/gftp.py` & `goth-0.9.0/goth/gftp.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/interactive.py` & `goth-0.9.0/goth/interactive.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/node.py` & `goth-0.9.0/goth/node.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     rest_api_url_base: str = "",
     account_list: str = "",
     payment_env: Optional[Dict[str, str]] = None,
 ) -> Dict[str, str]:
     """Construct an environment for executing commands in a yagna docker container."""
 
     daemon_env = {
+        # TODO: Remove old net
         "CENTRAL_NET_HOST": f"{ROUTER_HOST}:{ROUTER_PORT}",
+        "NET_RELAY_HOST": f"{ROUTER_HOST}:{ROUTER_PORT}",
         "GSB_URL": YAGNA_BUS_URL.substitute(host="0.0.0.0"),
         "IDLE_AGREEMENT_TIMEOUT": "600s",
         "MEAN_CYCLIC_BCAST_INTERVAL": "3s",
         "MEAN_CYCLIC_UNSUBSCRIBES_INTERVAL": "3s",
         "RUST_BACKTRACE": "1",
         "RUST_LOG": "debug,tokio_core=info,tokio_reactor=info,hyper=info",
         "YAGNA_API_URL": YAGNA_REST_URL.substitute(host="0.0.0.0"),
```

### Comparing `goth-0.8.0/goth/payment_config.py` & `goth-0.9.0/goth/payment_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,36 @@
             "ZKSYNC_FAUCET_ADDR": "http://zksync:3030/zk/donatex",
             "ZKSYNC_RINKEBY_RPC_ADDRESS": "http://zksync:3030",
         },
         "driver": "zksync",
         "network": "rinkeby",
         "token": "tGLM",
     },
-    "erc20": {
+    "erc20_mainnet": {
         "env": {
             "ERC20_MAINNET_REQUIRED_CONFIRMATIONS": REQUIRED_CONFIRMATIONS_COUNT,
             "MAINNET_GETH_ADDR": GETH_ADDR,
             "MAINNET_GLM_CONTRACT_ADDRESS": GLM_CONTRACT_ADDRESS,
             "YA_PAYMENT_NETWORK": "mainnet",
         },
         "driver": "erc20",
         "network": "mainnet",
         "token": "GLM",
     },
+    "erc20": {
+        "env": {
+            "ERC20_RINKEBY_REQUIRED_CONFIRMATIONS": REQUIRED_CONFIRMATIONS_COUNT,
+            "RINKEBY_GETH_ADDR": GETH_ADDR,
+            "RINKEBY_TGLM_CONTRACT_ADDRESS": GLM_CONTRACT_ADDRESS,
+            "YA_PAYMENT_NETWORK": "rinkeby",
+        },
+        "driver": "erc20",
+        "network": "rinkeby",
+        "token": "tGLM",
+    },
     "polygon": {
         "env": {
             "ERC20_POLYGON_REQUIRED_CONFIRMATIONS": REQUIRED_CONFIRMATIONS_COUNT,
             "POLYGON_GETH_ADDR": GETH_ADDR,
             "POLYGON_GLM_CONTRACT_ADDRESS": GLM_CONTRACT_ADDRESS,
             "YA_PAYMENT_NETWORK": "polygon",
         },
```

### Comparing `goth-0.8.0/goth/runner/__init__.py` & `goth-0.9.0/goth/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/cli/__init__.py` & `goth-0.9.0/goth/runner/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/cli/base.py` & `goth-0.9.0/goth/runner/cli/base.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/cli/typing.py` & `goth-0.9.0/goth/runner/cli/typing.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/cli/yagna_app_key_cmd.py` & `goth-0.9.0/goth/runner/cli/yagna_app_key_cmd.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/cli/yagna_id_cmd.py` & `goth-0.9.0/goth/runner/cli/yagna_id_cmd.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/cli/yagna_payment_cmd.py` & `goth-0.9.0/goth/runner/cli/yagna_payment_cmd.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/container/__init__.py` & `goth-0.9.0/goth/runner/container/__init__.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/container/build.py` & `goth-0.9.0/goth/runner/container/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "golemsp",
     "ya-provider",
     "yagna",
 }
 
 DEB_RELEASE_REPOS = [
     "ya-service-bus",
+    "ya-relay",
     "ya-runtime-wasi",
     "ya-runtime-vm",
     "ya-test-runtime-counters",
 ]
 
 PROXY_IMAGE = "proxy-nginx"
```

### Comparing `goth-0.8.0/goth/runner/container/compose.py` & `goth-0.9.0/goth/runner/container/compose.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/container/payment.py` & `goth-0.9.0/goth/runner/container/payment.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/container/utils.py` & `goth-0.9.0/goth/runner/container/utils.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/container/yagna.py` & `goth-0.9.0/goth/runner/container/yagna.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/download/__init__.py` & `goth-0.9.0/goth/runner/download/__init__.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/exceptions.py` & `goth-0.9.0/goth/runner/exceptions.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/log.py` & `goth-0.9.0/goth/runner/log.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/log_monitor.py` & `goth-0.9.0/goth/runner/log_monitor.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/probe/__init__.py` & `goth-0.9.0/goth/runner/probe/__init__.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/probe/agent.py` & `goth-0.9.0/goth/runner/probe/agent.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/probe/component.py` & `goth-0.9.0/goth/runner/probe/component.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/probe/mixin.py` & `goth-0.9.0/goth/runner/probe/mixin.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/probe/rest_client.py` & `goth-0.9.0/goth/runner/probe/rest_client.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/process.py` & `goth-0.9.0/goth/runner/process.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/proxy.py` & `goth-0.9.0/goth/runner/proxy.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/step.py` & `goth-0.9.0/goth/runner/step.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/goth/runner/web_server.py` & `goth-0.9.0/goth/runner/web_server.py`

 * *Files identical despite different names*

### Comparing `goth-0.8.0/pyproject.toml` & `goth-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.black]
 target-version = ['py38']
 exclude= '/(\.eggs|\.git|\.hg|\.mypy_cache|\.nox|\.tox|\.venv|venv|\.svn|_build|buck-out|build|dist|model)/' # Default excludes from black and the generated folder model
 
 [tool.poetry]
 name = "goth"
-version = "0.8.0"
+version = "0.9.0"
 description = "Golem Test Harness - integration testing framework"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "GPL-3.0"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `goth-0.8.0/setup.py` & `goth-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'transitions>=0.8,<0.9',
  'typing_extensions>=3.10.0,<4.0.0',
  'urllib3>=1.26,<2.0',
  'ya-aioclient>=0.6,<0.7']
 
 setup_kwargs = {
     'name': 'goth',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Golem Test Harness - integration testing framework',
     'long_description': '# Golem Test Harness\n\n![codestyle](https://github.com/golemfactory/goth/workflows/codestyle/badge.svg?event=push)\n![test](https://github.com/golemfactory/goth/workflows/test/badge.svg?event=push)\n[![PyPI version](https://badge.fury.io/py/goth.svg)](https://badge.fury.io/py/goth)\n[![GitHub license](https://img.shields.io/github/license/golemfactory/goth)](https://github.com/golemfactory/goth/blob/master/LICENSE)\n\n`goth` is an integration testing framework intended to aid the development process of [`yagna`](https://github.com/golemfactory/yagna) itself, as well as apps built on top of it.\n\n## How it works\n\nKey features:\n- creates a fully local, isolated network of Golem nodes including an Ethereum blockchain (through [`ganache`](https://www.trufflesuite.com/ganache))\n- provides an interface for controlling the local Golem nodes using either `yagna`\'s REST API or CLI\n- includes tools for defining complex integration testing scenarios, e.g. HTTP traffic and log assertions\n- configurable through a YAML file as well as using a number of CLI parameters\n\nWithin a single `goth` invocation (i.e. test session) the framework executes all tests which are defined in its given directory tree.\n\nInternally, `goth` uses `pytest`, therefore each integration test is defined as a function with the `test_` prefix in its name.\n\nEvery test run consists of the following steps:\n1. `docker-compose` is used to start the so-called "static" containers (e.g. local blockchain, HTTP proxy) and create a common Docker network for all containers participating in the given test.\n2. The test runner creates a number of Yagna containers (as defined in `goth-config.yml`) which are then connected to the `docker-compose` network.\n3. For each Yagna container started an interface object called a `Probe` is created and made available inside the test via the `Runner` object.\n4. The integration test scenario is executed as defined in the test function itself.\n5. Once the test is finished, all previously started Docker containers (both "static" and "dynamic") are removed and other cleanup is performed before repeating these steps for the next test.\n\n## Requirements\n- Linux (tested on Ubuntu 18.04 and 20.04)\n- Python 3.8+\n- Docker\n\n#### Python 3.8+\nYou can check your currently installed Python version by running:\n```\npython3 --version\n```\n\nIf you don\'t have Python installed, download the appropriate package and follow instructions from the [releases page](https://www.python.org/downloads/).\n#### Docker\nTo run `goth` you will need to have Docker installed. To install the Docker engine on your system follow these [instructions](https://docs.docker.com/engine/install/).\n\nTo verify your installation you can run the `hello-world` Docker image:\n```\ndocker run hello-world\n```\n\n## Installation\n`goth` is available as a PyPI package:\n```\npip install goth\n```\n\nIt is encouraged to use a Python virtual environment.\n\n## Usage\n\n### Getting a GitHub API token\nWhen starting the local Golem network, `goth` uses the GitHub API to fetch metadata and download artifacts and images. Though all of these assets are public, using this API still requires basic authentication. Therefore, you need to provide `goth` with a personal access token.\n\nTo generate a new token, go to your account\'s [developer settings](https://github.com/settings/tokens).\n\nYou will need to grant your new token the `public_repo` scope, as well as the `read:packages` scope. The packages scope is required in order to pull Docker images from GitHub.\n\nOnce your token is generated you need to do two things:\n1. Log in to GitHub\'s Docker registry by calling: `docker login docker.pkg.github.com -u {username}`, replacing `{username}` with your GitHub username and pasting in your access token as the password. You only need to do this once on your machine.\n2. Export an environment variable named `GITHUB_API_TOKEN` and use the access token as its value. This environment variable will need to be available in the shell from which you run `goth`.\n\n### Starting a local network\n\nFirst, create a copy of the default assets:\n```\npython -m goth create-assets your/output/dir\n```\n\nWhere `your/output/dir` is the path to a directory under which the default assets should be created. The path can be relative and it cannot be pointing to an existing directory.\nThese assets do not need to be re-created between test runs.\n\nWith the default assets created you can run the local test network like so:\n\n```\npython -m goth start your/output/dir/goth-config.yml\n```\n\nIf everything went well you should see the following output:\n```\nLocal goth network ready!\n\nYou can now load the requestor configuration variables to your shell:\n\nsource /tmp/goth_interactive.env\n\nAnd then run your requestor agent from that same shell.\n\nPress Ctrl+C at any moment to stop the local network.\n```\n\nThis is a special case of `goth`\'s usage. Running this command does not execute a test, but rather sets up a local Golem network which can be used for debugging purposes. The parameters required to connect to the requestor `yagna` node running in this network are output to the file `/tmp/goth_interactive.env` and can be `source`d from your shell.\n\n### Creating and running test cases\nTake a look at the `yagna` integration tests [`README`](https://github.com/golemfactory/yagna/blob/master/goth_tests/README.md) to learn more about writing and launching your own test cases.\n\n### Logs from `goth` tests\nAll containers launched during an integration test record their logs in a pre-determined location. By default, this location is: `$TEMP_DIR/goth-tests`, where `$TEMP_DIR` is the path of the directory used for temporary files.\n\nThis path will depend either on the shell environment or the operating system on which the tests are being run (see [`tempfile.gettempdir`](https://docs.python.org/3/library/tempfile.html) for more details).\n\n#### Log directory structure\n```\n.\n└── goth_20210420_093848+0000\n    ├── runner.log                      # debug console logs from the entire test session\n    ├── test_e2e_vm                     # directory with logs from a single test\n    │\xa0\xa0 ├── ethereum.log\n    │\xa0\xa0 ├── provider_1.log              # debug logs from a single yagna node\n    │\xa0\xa0 ├── provider_1_ya-provider.log  # debug logs from an agent running in a yagna node\n    │\xa0\xa0 ├── provider_2.log\n    │\xa0\xa0 ├── provider_2_ya-provider.log\n    │\xa0\xa0 ├── proxy-nginx.log\n    │\xa0\xa0 ├── proxy.log                   # HTTP traffic going into the yagna daemons recorded by a "sniffer" proxy\n    │\xa0\xa0 ├── requestor.log\n    │\xa0\xa0 ├── router.log\n    │\xa0\xa0 ├── test.log                    # debug console logs from this test case only, duplicated in `runner.log`\n    │\xa0\xa0 └── zksync.log\n    └── test_e2e_wasi\n        └── ...\n```\n\n### Test configuration\n\n#### `goth-config.yml`\n`goth` can be configured using a YAML file. The default `goth-config.yml` is located in `goth/default-assets/goth-config.yml` and looks something like this:\n```\ndocker-compose:\n\n  docker-dir: "docker"                          # Where to look for docker-compose.yml and Dockerfiles\n\n  build-environment:                            # Fields related to building the yagna Docker image\n    # binary-path: ...\n    # deb-path: ...\n    # branch: ...\n    # commit-hash: ...\n    # release-tag: ...\n    # use-prerelease: ...\n\n  compose-log-patterns:                         # Log message patterns used for container ready checks\n    ethereum: ".*Wallets supplied."\n    ...\n\nkey-dir: "keys"                                 # Where to look for pre-funded Ethereum keys\n\nnode-types:                                     # User-defined node types to be used in `nodes`\n  - name: "Requestor"\n    class: "goth.runner.probe.RequestorProbe"\n\n  - name: "Provider"\n    class: "goth.runner.probe.ProviderProbe"\n    mount: ...\n\nnodes:                                          # List of yagna nodes to be run in the test\n  - name: "requestor"\n    type: "Requestor"\n\n  - name: "provider-1"\n    type: "Provider"\n    use-proxy: True\n```\n\nWhen you generate test assets using the command `python -m goth create-assets your/output/dir`, this default config file will be present in the output location of your choice. You can make changes to that generated file and always fall back to the default one by re-generating the assets.\n\n## Local development setup\n\n### Poetry\n`goth` uses [`poetry`](https://python-poetry.org/) to manage its dependencies and provide a runner for common tasks.\n\nIf you don\'t have `poetry` available on your system then follow its [installation instructions](https://python-poetry.org/docs/#installation) before proceeding.\nVerify your installation by running:\n```\npoetry --version\n```\n\n### Project dependencies\nTo install the project\'s dependencies run:\n```\npoetry install\n```\nBy default, `poetry` looks for the required Python version on your `PATH` and creates a virtual environment for the project if there\'s none active (or already configured by Poetry).\n\nAll of the project\'s dependencies will be installed to that virtual environment.\n',
     'author': 'Golem Factory',
     'author_email': 'contact@golem.network',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/golemfactory/goth',
```

### Comparing `goth-0.8.0/PKG-INFO` & `goth-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goth
-Version: 0.8.0
+Version: 0.9.0
 Summary: Golem Test Harness - integration testing framework
 Home-page: https://github.com/golemfactory/goth
 License: GPL-3.0
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

