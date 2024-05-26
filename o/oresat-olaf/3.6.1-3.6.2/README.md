# Comparing `tmp/oresat_olaf-3.6.1.tar.gz` & `tmp/oresat_olaf-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_olaf-3.6.1.tar", last modified: Sat May 25 02:05:33 2024, max compression
+gzip compressed data, was "oresat_olaf-3.6.2.tar", last modified: Sun May 26 20:19:37 2024, max compression
```

## Comparing `oresat_olaf-3.6.1.tar` & `oresat_olaf-3.6.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.162309 oresat_olaf-3.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.142309 oresat_olaf-3.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.146309 oresat_olaf-3.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-25 02:05:33.162309 oresat_olaf-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.146309 oresat_olaf-3.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.146309 oresat_olaf-3.6.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/adc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/app.rst
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/cpufreq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/daemon.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/ecss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/gpio.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/node.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/oresat_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/oresat_file_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/pru.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/resource.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/rest_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/service.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/timer_loop.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/api/updater.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/rest_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.146309 oresat_olaf-3.6.1/docs/updater/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/updater/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/docs/updater/update_archive.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.150309 oresat_olaf-3.6.1/olaf/
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.150309 oresat_olaf-3.6.1/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.150309 oresat_olaf-3.6.1/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/resources/daemons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/resources/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.150309 oresat_olaf-3.6.1/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.150309 oresat_olaf-3.6.1/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.150309 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/daemons.html
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/reset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/updater.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.154309 oresat_olaf-3.6.1/olaf/_internals/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/services/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/services/os_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/services/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/_internals/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 02:05:33.000000 oresat_olaf-3.6.1/olaf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.154309 oresat_olaf-3.6.1/olaf/board/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/board/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/board/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/board/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/board/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/board/pru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.154309 oresat_olaf-3.6.1/olaf/canopen/
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/canopen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/canopen/ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/canopen/master_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/canopen/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    21489 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/canopen/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.154309 oresat_olaf-3.6.1/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.162309 oresat_olaf-3.6.1/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-25 02:05:33.000000 oresat_olaf-3.6.1/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-25 02:05:33.000000 oresat_olaf-3.6.1/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:05:33.000000 oresat_olaf-3.6.1/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-25 02:05:33.000000 oresat_olaf-3.6.1/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 02:05:33.000000 oresat_olaf-3.6.1/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/run.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:05:33.162309 oresat_olaf-3.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.158309 oresat_olaf-3.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.158309 oresat_olaf-3.6.1/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/common/test_oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/common/test_pru.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/common/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.158309 oresat_olaf-3.6.1/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.158309 oresat_olaf-3.6.1/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/resources/test_fwrite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.158309 oresat_olaf-3.6.1/tests/internals/services/
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/services/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/test_rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.158309 oresat_olaf-3.6.1/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:33.162309 oresat_olaf-3.6.1/tests/internals/updater/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test-script.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611940000.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611941111.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611942222.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611943333.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611944444.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611945555.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611946666.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611947777.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611948888.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-25 02:05:28.000000 oresat_olaf-3.6.1/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.190993 oresat_olaf-3.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.170992 oresat_olaf-3.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.174993 oresat_olaf-3.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-26 20:19:37.190993 oresat_olaf-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.174993 oresat_olaf-3.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.174993 oresat_olaf-3.6.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/adc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/cpufreq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/daemon.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/ecss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/gpio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/node.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/oresat_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/oresat_file_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/pru.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/rest_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/service.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/timer_loop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/api/updater.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/rest_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.174993 oresat_olaf-3.6.2/docs/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/updater/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/docs/updater/update_archive.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.178993 oresat_olaf-3.6.2/olaf/
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.178993 oresat_olaf-3.6.2/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.178993 oresat_olaf-3.6.2/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/resources/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/resources/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.178993 oresat_olaf-3.6.2/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.178993 oresat_olaf-3.6.2/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.178993 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/daemons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/reset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/updater.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.182993 oresat_olaf-3.6.2/olaf/_internals/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/services/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/services/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/services/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/_internals/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-26 20:19:37.000000 oresat_olaf-3.6.2/olaf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.182993 oresat_olaf-3.6.2/olaf/board/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/board/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/board/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/board/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/board/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/board/pru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.182993 oresat_olaf-3.6.2/olaf/canopen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/canopen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/canopen/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/canopen/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/canopen/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21489 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/canopen/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.182993 oresat_olaf-3.6.2/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.190993 oresat_olaf-3.6.2/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-26 20:19:37.000000 oresat_olaf-3.6.2/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-26 20:19:37.000000 oresat_olaf-3.6.2/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 20:19:37.000000 oresat_olaf-3.6.2/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-26 20:19:37.000000 oresat_olaf-3.6.2/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-26 20:19:37.000000 oresat_olaf-3.6.2/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 20:19:37.190993 oresat_olaf-3.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.182993 oresat_olaf-3.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.186993 oresat_olaf-3.6.2/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/common/test_oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/common/test_pru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/common/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.186993 oresat_olaf-3.6.2/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.186993 oresat_olaf-3.6.2/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/resources/test_fwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.186993 oresat_olaf-3.6.2/tests/internals/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/services/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/test_rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.186993 oresat_olaf-3.6.2/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 20:19:37.186993 oresat_olaf-3.6.2/tests/internals/updater/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test-script.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611940000.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611941111.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611942222.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611943333.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611944444.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611945555.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611946666.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611947777.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611948888.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-26 20:19:30.000000 oresat_olaf-3.6.2/tests/internals/updater/test_updater.py
```

### Comparing `oresat_olaf-3.6.1/.github/workflows/pypi.yaml` & `oresat_olaf-3.6.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/.github/workflows/tests.yaml` & `oresat_olaf-3.6.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/.gitignore` & `oresat_olaf-3.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/LICENSE` & `oresat_olaf-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/PKG-INFO` & `oresat_olaf-3.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 3.6.1
+Version: 3.6.2
 Summary: Application framework for all OreSat Linux boards
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_olaf-3.6.1/README.rst` & `oresat_olaf-3.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/Makefile` & `oresat_olaf-3.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/api/ecss.rst` & `oresat_olaf-3.6.2/docs/api/ecss.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/api/oresat_file.rst` & `oresat_olaf-3.6.2/docs/api/oresat_file.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/api/rest_api.rst` & `oresat_olaf-3.6.2/docs/api/rest_api.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/conf.py` & `oresat_olaf-3.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/glossary.rst` & `oresat_olaf-3.6.2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/index.rst` & `oresat_olaf-3.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/make.bat` & `oresat_olaf-3.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/rest_api.rst` & `oresat_olaf-3.6.2/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/updater/index.rst` & `oresat_olaf-3.6.2/docs/updater/index.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/docs/updater/update_archive.rst` & `oresat_olaf-3.6.2/docs/updater/update_archive.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/__init__.py` & `oresat_olaf-3.6.2/olaf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from ._internals.app import App, app
 from ._internals.rest_api import RestAPI, render_olaf_template, rest_api
 from ._internals.services.logs import logger_tmp_file_setup
 from ._internals.updater import Updater, UpdaterState
 from .board.adc import Adc
 from .board.cpufreq import A8_CPUFREQS, get_cpufreq, get_cpufreq_gov, set_cpufreq, set_cpufreq_gov
+from .board.eeprom import Eeprom
 from .board.gpio import GPIO_HIGH, GPIO_IN, GPIO_LOW, GPIO_OUT, Gpio, GpioError
 from .board.pru import Pru, PruError, PruState
 from .canopen.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
 from .canopen.master_node import MasterNode
 from .canopen.network import CanNetwork, CanNetworkError, CanNetworkState, NetworkError
 from .canopen.node import Node, NodeStop
 from .common.daemon import Daemon, DaemonState
@@ -134,16 +135,24 @@
         raise ValueError(f"invalid card {name} for {args.oresat}")
 
     od = config.od_db[name]
 
     if args.disable_flight_mode:
         od["flight_mode"].value = False
 
+    version = "0.0"
+    try:
+        eeprom = Eeprom()
+        version = f"{eeprom.major}.{eeprom.minor}"
+        logger.info(f"detected v{version} card")
+    except (PermissionError, FileNotFoundError):
+        logger.warning("could not read hardware info from eeprom")
     if args.hardware_version != "0.0":
-        od["versions"]["hw_version"].value = args.hardware_version
+        version = args.hardware_version
+    od["versions"]["hw_version"].value = version
 
     is_octavo = config.cards[name].processor == "octavo"
     if is_octavo:
         od["versions"]["olaf_version"].value = __version__
 
     network = CanNetwork(args.bus_type, args.bus, args.socketcand_host)
     od_db = config.od_db if name == "c3" else None
```

### Comparing `oresat_olaf-3.6.1/olaf/_internals/app.py` & `oresat_olaf-3.6.2/olaf/_internals/app.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/resources/daemons.py` & `oresat_olaf-3.6.2/olaf/_internals/resources/daemons.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/resources/ecss.py` & `oresat_olaf-3.6.2/olaf/_internals/resources/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/resources/fread.py` & `oresat_olaf-3.6.2/olaf/_internals/resources/fread.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/resources/fwrite.py` & `oresat_olaf-3.6.2/olaf/_internals/resources/fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/resources/system.py` & `oresat_olaf-3.6.2/olaf/_internals/resources/system.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Resource for the system."""
 
 from time import monotonic, time
 
 import psutil
-from loguru import logger
 
-from ...board.eeprom import Eeprom
 from ...canopen.node import NodeStop
 from ...common.resource import Resource
 
 
 class SystemResource(Resource):
     """Resource for the system."""
 
@@ -18,20 +16,14 @@
 
         self.node.add_sdo_callbacks("system", "ram_percent", self.on_read_ram, None)
         self.node.add_sdo_callbacks("system", "storage_percent", self.on_read_storage, None)
         self.node.add_sdo_callbacks("system", "uptime", self.on_read_uptime, None)
         self.node.add_sdo_callbacks("system", "unix_time", self.on_read_unix_time, None)
         self.node.add_sdo_callbacks("system", "reset", None, self.on_write_reset)
 
-        try:
-            eeprom = Eeprom()
-            self.node.od_write("versions", "hw_version", f"{eeprom.major}.{eeprom.minor}")
-        except (PermissionError, FileNotFoundError):
-            logger.warning("could not read hardware info from eeprom")
-
     def on_read_ram(self):
         """SDO read callback for getting the RAM usage percent."""
 
         return int(psutil.virtual_memory().percent)
 
     def on_read_storage(self):
         """SDO read callback for getting the storage usage percent."""
```

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/__init__.py` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/static/favicon.ico` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/_base.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/_base.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/base.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/base.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/daemons.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/daemons.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/fread.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/fwrite.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/logs.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/logs.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/od.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/od.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/os_command.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/os_command.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/reset.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/reset.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/root.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/root.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/rest_api/templates/updater.html` & `oresat_olaf-3.6.2/olaf/_internals/rest_api/templates/updater.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/services/logs.py` & `oresat_olaf-3.6.2/olaf/_internals/services/logs.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/services/os_command.py` & `oresat_olaf-3.6.2/olaf/_internals/services/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/services/updater.py` & `oresat_olaf-3.6.2/olaf/_internals/services/updater.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/_internals/updater.py` & `oresat_olaf-3.6.2/olaf/_internals/updater.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/board/adc.py` & `oresat_olaf-3.6.2/olaf/board/adc.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/board/cpufreq.py` & `oresat_olaf-3.6.2/olaf/board/cpufreq.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/board/eeprom.py` & `oresat_olaf-3.6.2/olaf/board/eeprom.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,18 +55,20 @@
         self.id = data[24:28]
 
         # non oresat card defaults
         self.is_oresat_card = False
         self.major = 0
         self.minor = 0
 
-        if self.nice_name == "pocketbeagle":
-            self.device_tree = "am335x-pocketbeagle.dtb"
-        elif self.nice_name == "boneblack":
-            self.device_tree = "am335x-boneblack.dtb"
-        elif self.nice_name != "unknown":  # aka an oresat card
+        if self.serial_id != "PSAS":
+            if self.nice_name == "pocketbeagle":
+                self.device_tree = "am335x-pocketbeagle.dtb"
+            elif self.nice_name == "boneblack":
+                self.device_tree = "am335x-boneblack.dtb"
+        else:
             self.is_oresat_card = True
-            self.device_tree = f"{self.nice_name}-{self.version}.dtb"
+            if self.nice_name != "unknown":  # aka an oresat card
+                self.device_tree = "unknown"
+            else:
+                self.device_tree = f"{self.nice_name}-{self.version}.dtb"
             self.major = int(data[12:14])
             self.minor = int(data[14:16])
-        else:
-            self.device_tree = "unknown"
```

### Comparing `oresat_olaf-3.6.1/olaf/board/gpio.py` & `oresat_olaf-3.6.2/olaf/board/gpio.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/board/pru.py` & `oresat_olaf-3.6.2/olaf/board/pru.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/canopen/__init__.py` & `oresat_olaf-3.6.2/olaf/canopen/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/canopen/ecss.py` & `oresat_olaf-3.6.2/olaf/canopen/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/canopen/master_node.py` & `oresat_olaf-3.6.2/olaf/canopen/master_node.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/canopen/network.py` & `oresat_olaf-3.6.2/olaf/canopen/network.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/canopen/node.py` & `oresat_olaf-3.6.2/olaf/canopen/node.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/__init__.py` & `oresat_olaf-3.6.2/olaf/common/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/daemon.py` & `oresat_olaf-3.6.2/olaf/common/daemon.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/oresat_file.py` & `oresat_olaf-3.6.2/olaf/common/oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/oresat_file_cache.py` & `oresat_olaf-3.6.2/olaf/common/oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/resource.py` & `oresat_olaf-3.6.2/olaf/common/resource.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/service.py` & `oresat_olaf-3.6.2/olaf/common/service.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/olaf/common/timer_loop.py` & `oresat_olaf-3.6.2/olaf/common/timer_loop.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/oresat_olaf.egg-info/PKG-INFO` & `oresat_olaf-3.6.2/oresat_olaf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 3.6.1
+Version: 3.6.2
 Summary: Application framework for all OreSat Linux boards
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_olaf-3.6.1/oresat_olaf.egg-info/SOURCES.txt` & `oresat_olaf-3.6.2/oresat_olaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/pyproject.toml` & `oresat_olaf-3.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/common/test_ecss.py` & `oresat_olaf-3.6.2/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/common/test_oresat_file.py` & `oresat_olaf-3.6.2/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/common/test_oresat_file_cache.py` & `oresat_olaf-3.6.2/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/common/test_pru.py` & `oresat_olaf-3.6.2/tests/common/test_pru.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/common/test_resources.py` & `oresat_olaf-3.6.2/tests/common/test_resources.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/resources/__init__.py` & `oresat_olaf-3.6.2/tests/internals/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/resources/test_ecss.py` & `oresat_olaf-3.6.2/tests/internals/resources/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/resources/test_fread.py` & `oresat_olaf-3.6.2/tests/internals/resources/test_fread.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/resources/test_fwrite.py` & `oresat_olaf-3.6.2/tests/internals/resources/test_fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/services/__init__.py` & `oresat_olaf-3.6.2/tests/internals/services/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/services/test_os_command.py` & `oresat_olaf-3.6.2/tests/internals/services/test_os_command.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/test_rest_api.py` & `oresat_olaf-3.6.2/tests/internals/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/README.md` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/README.md`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611940000.tar.xz` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611940000.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611942222.tar.xz` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611942222.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611943333.tar.xz` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611943333.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611944444.tar.xz` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611944444.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611945555.tar.xz` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611945555.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_files/test_update_1611946666.tar.xz` & `oresat_olaf-3.6.2/tests/internals/updater/test_files/test_update_1611946666.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.6.1/tests/internals/updater/test_updater.py` & `oresat_olaf-3.6.2/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

