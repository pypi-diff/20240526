# Comparing `tmp/hyper-shell-2.4.0.tar.gz` & `tmp/hyper_shell-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-shell-2.4.0.tar", last modified: Thu Jun  8 21:00:08 2023, max compression
+gzip compressed data, was "hyper_shell-2.5.0.tar", max compression
```

## Comparing `hyper-shell-2.4.0.tar` & `hyper_shell-2.5.0.tar`

### file list

```diff
@@ -1,48 +1,30 @@
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.783147 hyper-shell-2.4.0/
--rw-r--r--   0 geoffrey   (501) staff       (20)    11357 2020-12-21 02:22:57.000000 hyper-shell-2.4.0/LICENSE
--rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-06-08 21:00:08.783044 hyper-shell-2.4.0/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)     2883 2023-04-02 14:55:21.000000 hyper-shell-2.4.0/README.rst
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.778245 hyper-shell-2.4.0/man/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.779183 hyper-shell-2.4.0/man/man1/
--rw-r--r--   0 geoffrey   (501) staff       (20)    63611 2023-06-08 20:56:49.000000 hyper-shell-2.4.0/man/man1/hyper-shell.1
--rw-r--r--   0 geoffrey   (501) staff       (20)      100 2022-01-10 02:23:40.000000 hyper-shell-2.4.0/pyproject.toml
--rw-r--r--   0 geoffrey   (501) staff       (20)       38 2023-06-08 21:00:08.783178 hyper-shell-2.4.0/setup.cfg
--rw-r--r--   0 geoffrey   (501) staff       (20)     2652 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/setup.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.778416 hyper-shell-2.4.0/src/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.779886 hyper-shell-2.4.0/src/hyper_shell.egg-info/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)     1067 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       48 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/entry_points.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/requires.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       11 2023-06-08 21:00:08.000000 hyper-shell-2.4.0/src/hyper_shell.egg-info/top_level.txt
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.780580 hyper-shell-2.4.0/src/hypershell/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3573 2023-06-08 20:56:49.000000 hyper-shell-2.4.0/src/hypershell/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    39835 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/client.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.781066 hyper-shell-2.4.0/src/hypershell/cluster/
--rw-r--r--   0 geoffrey   (501) staff       (20)    18282 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     3460 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/local.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    18159 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/remote.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     8520 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/cluster/ssh.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    11715 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/config.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.782575 hyper-shell-2.4.0/src/hypershell/core/
--rw-r--r--   0 geoffrey   (501) staff       (20)      118 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     5906 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/ansi.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     9811 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/config.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     5087 2023-06-08 20:51:45.000000 hyper-shell-2.4.0/src/hypershell/core/exceptions.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     2010 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/fsm.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1964 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/heartbeat.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     6373 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/logging.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     2952 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/core/platform.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     5347 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/queue.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     6733 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/remote.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     7244 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/template.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1597 2023-04-13 15:30:41.000000 hyper-shell-2.4.0/src/hypershell/core/thread.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      793 2023-04-02 14:55:21.000000 hyper-shell-2.4.0/src/hypershell/core/types.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-06-08 21:00:08.782880 hyper-shell-2.4.0/src/hypershell/data/
--rw-r--r--   0 geoffrey   (501) staff       (20)     4611 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/data/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     7873 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/data/core.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    20916 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/data/model.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    36448 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/server.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    22576 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/submit.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    31601 2023-06-08 20:51:46.000000 hyper-shell-2.4.0/src/hypershell/task.py
+-rw-r--r--   0        0        0    11357 2020-12-21 02:22:57.000000 hyper_shell-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3220 2024-05-26 04:15:05.396754 hyper_shell-2.5.0/README.rst
+-rw-r--r--   0        0        0     2243 2024-05-26 04:15:05.406103 hyper_shell-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3292 2024-05-26 04:15:05.406381 hyper_shell-2.5.0/src/hypershell/__init__.py
+-rw-r--r--   0        0        0    48899 2024-05-26 04:15:05.406559 hyper_shell-2.5.0/src/hypershell/client.py
+-rw-r--r--   0        0        0    18491 2024-05-26 04:15:05.406716 hyper_shell-2.5.0/src/hypershell/cluster/__init__.py
+-rw-r--r--   0        0        0     3668 2024-05-26 04:15:05.406848 hyper_shell-2.5.0/src/hypershell/cluster/local.py
+-rw-r--r--   0        0        0    18647 2024-05-26 04:15:05.406980 hyper_shell-2.5.0/src/hypershell/cluster/remote.py
+-rw-r--r--   0        0        0     8799 2024-05-26 04:15:05.407175 hyper_shell-2.5.0/src/hypershell/cluster/ssh.py
+-rw-r--r--   0        0        0    14724 2024-05-26 04:15:05.407372 hyper_shell-2.5.0/src/hypershell/config.py
+-rw-r--r--   0        0        0      118 2024-05-26 04:15:05.407487 hyper_shell-2.5.0/src/hypershell/core/__init__.py
+-rw-r--r--   0        0        0    12260 2024-05-26 04:15:05.407677 hyper_shell-2.5.0/src/hypershell/core/config.py
+-rw-r--r--   0        0        0     5078 2024-05-26 04:15:05.407798 hyper_shell-2.5.0/src/hypershell/core/exceptions.py
+-rw-r--r--   0        0        0     2012 2024-05-26 04:15:05.407905 hyper_shell-2.5.0/src/hypershell/core/fsm.py
+-rw-r--r--   0        0        0     1963 2024-05-26 04:15:05.408011 hyper_shell-2.5.0/src/hypershell/core/heartbeat.py
+-rw-r--r--   0        0        0     6364 2024-05-26 04:15:05.408140 hyper_shell-2.5.0/src/hypershell/core/logging.py
+-rw-r--r--   0        0        0     4323 2024-05-26 04:15:05.408269 hyper_shell-2.5.0/src/hypershell/core/platform.py
+-rw-r--r--   0        0        0     5347 2024-05-26 04:15:05.408389 hyper_shell-2.5.0/src/hypershell/core/queue.py
+-rw-r--r--   0        0        0     6733 2024-05-26 04:15:05.408508 hyper_shell-2.5.0/src/hypershell/core/remote.py
+-rw-r--r--   0        0        0     1416 2024-05-26 04:15:05.408585 hyper_shell-2.5.0/src/hypershell/core/signal.py
+-rw-r--r--   0        0        0     7244 2024-05-26 04:15:05.408707 hyper_shell-2.5.0/src/hypershell/core/template.py
+-rw-r--r--   0        0        0     1597 2024-05-26 04:15:05.408823 hyper_shell-2.5.0/src/hypershell/core/thread.py
+-rw-r--r--   0        0        0      742 2024-05-26 04:15:05.408934 hyper_shell-2.5.0/src/hypershell/core/types.py
+-rw-r--r--   0        0        0     4407 2024-05-26 04:15:05.409062 hyper_shell-2.5.0/src/hypershell/data/__init__.py
+-rw-r--r--   0        0        0     7873 2024-05-26 04:15:05.409183 hyper_shell-2.5.0/src/hypershell/data/core.py
+-rw-r--r--   0        0        0    23479 2024-05-26 04:15:05.409319 hyper_shell-2.5.0/src/hypershell/data/model.py
+-rw-r--r--   0        0        0    46380 2024-05-26 04:15:05.409505 hyper_shell-2.5.0/src/hypershell/server.py
+-rw-r--r--   0        0        0    25542 2024-05-26 04:15:05.409660 hyper_shell-2.5.0/src/hypershell/submit.py
+-rw-r--r--   0        0        0    45898 2024-05-26 04:15:05.409845 hyper_shell-2.5.0/src/hypershell/task.py
+-rw-r--r--   0        0        0     4541 1970-01-01 00:00:00.000000 hyper_shell-2.5.0/PKG-INFO
```

### Comparing `hyper-shell-2.4.0/LICENSE` & `hyper_shell-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.4.0/PKG-INFO` & `hyper_shell-2.5.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: hyper-shell
-Version: 2.4.0
-Summary: Process shell commands over a distributed, asynchronous queue.
-Home-page: https://github.com/glentner/hyper-shell
-Author: Geoffrey Lentner
-Author-email: glentner@purdue.edu
-License: Apache Software License
-Keywords: distributed-computing command-line-tool shell-scripting high-performance-computing
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/x-rst
-Provides-Extra: postgres
-License-File: LICENSE
-
 HyperShell v2: Distributed Task Execution for HPC
 =================================================
 
 .. image:: https://img.shields.io/badge/license-Apache-blue.svg?style=flat
     :target: https://www.apache.org/licenses/LICENSE-2.0
     :alt: License
 
@@ -35,33 +13,38 @@
     :target: https://pypi.org/project/hyper-shell
     :alt: Python Versions
 
 .. image:: https://readthedocs.org/projects/hyper-shell/badge/?version=latest&style=flat
     :target: https://hyper-shell.readthedocs.io
     :alt: Documentation
 
-.. image:: https://pepy.tech/badge/hyper-shell
-    :target: https://pepy.tech/badge/hyper-shell
+.. image:: https://static.pepy.tech/badge/hyper-shell
+    :target: https://pepy.tech/project/hyper-shell
     :alt: Downloads
 
 |
 
-*HyperShell* is an elegant, cross-platform, high-performance computing utility for
+*HyperShell* is an elegant, cross-platform, high-throughput computing utility for
 processing shell commands over a distributed, asynchronous queue. It is a highly
 scalable workflow automation tool for *many-task* scenarios.
 
+Built on Python and tested on Linux, macOS, and Windows.
+
 Several tools offer similar functionality but not all together in a single tool with
-the ergonomics we provide. Novel design elements include but are not limited to
-(1) cross-platform, (2) client-server design, (3) staggered launch for large scales,
-(4) persistent hosting of the server, and optionally (5) a database in-the-loop for
-persisting task metadata and automated retries.
-
-*HyperShell* is pure Python and is tested on Linux, macOS, and Windows 10 in
-Python 3.9+ environments. The server and client don't even need to use the same
-platform simultaneously.
+the user ergonomics we provide. Novel design elements include but are not limited to
+
+* **Cross-platform:** run on any platform where Python runs. In fact, the server and
+  client can run on different platforms in the same cluster.
+* **Client-server:** workloads do not need to be monolithic. Run the server as a
+  stand-alone service with SQLite or Postgres as a persistent database and dynamically
+  scale clients as needed.
+* **Staggered launch:** At the largest scales (1000s of nodes, 100k+ of workers),
+  the launch process can be challenging. Come up gradually to balance the workload.
+* **Database in-the-loop:** run in-memory for quick, ad-hoc workloads. Otherwise,
+  include a database for persistence, recovery when restarting, and search.
 
 
 Documentation
 -------------
 
 Documentation is available at `hyper-shell.readthedocs.io <https://hyper-shell.readthedocs.io>`_.
 For basic usage information on the command line use: ``hyper-shell --help``. For a more
```

### Comparing `hyper-shell-2.4.0/src/hypershell/__init__.py` & `hyper_shell-2.5.0/src/hypershell/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Initialization and entry-point for console application."""
 
 
 # standard libs
 import sys
+from importlib.metadata import version as get_version
 
 # external libs
 from cmdkit.app import Application, ApplicationGroup
 from cmdkit.cli import Interface
 
 # internal libs
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.logging import Logger, initialize_logging
+from hypershell.core.signal import register_handlers
 from hypershell.submit import SubmitApp
 from hypershell.server import ServerApp
 from hypershell.client import ClientApp
 from hypershell.cluster import ClusterApp
 from hypershell.task import TaskGroupApp
 from hypershell.config import ConfigApp
 from hypershell.data import InitDBApp
 
 # public interface
-__all__ = ['HyperShellApp', 'main', '__version__', '__license__']
+__all__ = ['HyperShellApp', 'main', '__version__']
 
 # project metadata
-__version__     = '2.4.0'
-__authors__     = 'Geoffrey Lentner'
-__contact__     = 'glentner@purdue.edu'
-__license__     = 'Apache Software License'
-__copyright__   = '2019-2023. All Rights Reserved.'
+__version__     = get_version('hyper-shell')
 __website__     = 'https://github.com/glentner/hyper-shell'
-__keywords__    = 'distributed-computing command-line-tool shell-scripting high-performance-computing'
 __description__ = 'Process shell commands over a distributed, asynchronous queue.'
 __citation__    = """\
 @inproceedings{lentner_2022,
     author = {Lentner, Geoffrey and Gorenstein, Lev},
     title = {HyperShell v2: Distributed Task Execution for HPC},
     year = {2022},
     isbn = {9781450391610},
@@ -55,20 +51,19 @@
 
 
 # inject logger setup into command-line framework
 Application.log_critical = log.critical
 Application.log_exception = log.exception
 
 
-APP_NAME = 'hyper-shell'
+APP_NAME = 'hs'
 APP_USAGE = f"""\
-Usage: 
-{APP_NAME} [-h] [-v] <command> [<args>...]
-
-{__description__}\
+Usage:
+  {APP_NAME} [-h] [-v] <command> [<args>...]
+  {__description__}\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
 Commands:
   config                 {ConfigApp.__doc__}
@@ -91,18 +86,15 @@
 citing us (see --citation).\
 """
 
 
 class HyperShellApp(ApplicationGroup):
     """Top-level application class for console application."""
 
-    interface = Interface(APP_NAME,
-                          colorize_usage(APP_USAGE),
-                          colorize_usage(APP_HELP))
-
+    interface = Interface(APP_NAME, APP_USAGE, APP_HELP)
     interface.add_argument('-v', '--version', action='version', version=__version__)
     interface.add_argument('--citation', action='version', version=__citation__)
     interface.add_argument('command')
 
     command = None
     commands = {
         'submit': SubmitApp,
@@ -114,8 +106,9 @@
         'initdb': InitDBApp,
     }
 
 
 def main() -> int:
     """Entry-point for console application."""
     initialize_logging()
+    register_handlers()
     return HyperShellApp.main(sys.argv[1:])
```

### Comparing `hyper-shell-2.4.0/src/hypershell/client.py` & `hyper_shell-2.5.0/src/hypershell/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Connect to server and run tasks.
 
 Example:
     >>> from hypershell.client import run_client
@@ -26,59 +26,75 @@
     some few moments before it shutsdown on its own. If your main program exits however,
     the thread will be stopped regardless because it runs as a `daemon`.
 """
 
 
 # type annotations
 from __future__ import annotations
-from typing import List, Tuple, Optional, Callable, Dict, IO, Type
+from typing import List, Tuple, Optional, Callable, Dict, IO, Type, Final
 from types import TracebackType
 
 # standard libs
 import os
 import sys
 import time
 import json
 import random
-import signal
 import functools
 from enum import Enum
 from datetime import datetime, timedelta
 from queue import Queue, Empty as QueueEmpty, Full as QueueFull
 from subprocess import Popen, TimeoutExpired
 from socket import gaierror
 from dataclasses import dataclass
-from multiprocessing import AuthenticationError
+from multiprocessing import AuthenticationError, cpu_count
 
 # external libs
 from cmdkit.app import Application, exit_status
 from cmdkit.cli import Interface, ArgumentError
 from cmdkit.config import Namespace
 
 # internal libs
 from hypershell.data.model import Task
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.heartbeat import Heartbeat, ClientState
 from hypershell.core.platform import default_path
-from hypershell.core.config import default, config, load_task_env
+from hypershell.core.config import default, config, load_task_env, SSH_GROUPS
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.thread import Thread
+from hypershell.core.signal import check_signal, SIGNAL_MAP, SIGUSR1, SIGUSR2, SIGINT
 from hypershell.core.queue import QueueClient, QueueConfig
 from hypershell.core.logging import HOSTNAME, INSTANCE, Logger
 from hypershell.core.template import Template, DEFAULT_TEMPLATE
 from hypershell.core.exceptions import (handle_exception, handle_disconnect,
                                         handle_address_unknown, HostAddressInfo, get_shared_exception_mapping)
 
 # public interface
-__all__ = ['run_client', 'ClientThread', 'ClientApp', 'ClientInfo', 'DEFAULT_NUM_TASKS', 'DEFAULT_DELAY', ]
+__all__ = ['run_client', 'ClientThread', 'ClientApp', 'ClientInfo',
+           'DEFAULT_BUNDLESIZE', 'DEFAULT_BUNDLEWAIT', 'DEFAULT_TEMPLATE',
+           'DEFAULT_NUM_TASKS', 'DEFAULT_DELAY', 'DEFAULT_SIGNALWAIT',
+           'DEFAULT_HEARTRATE', 'DEFAULT_HOST', 'DEFAULT_PORT', 'DEFAULT_AUTH',
+           'set_client_standalone']
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
+# NOTE:
+# The UNIX signal facility works on stand-alone server/client, but when running a LocalCluster with
+# a client as a local thread, the USR1/USR2 signals prevent clients from sending the proper finalization
+# messages. This flag is set by LocalCluster to prevent greedy client-side shutdown behavior.
+CLIENT_STANDALONE_MODE: bool = True
+
+
+def set_client_standalone(mode: bool) -> None:
+    """Set global flag to prevent greedy shutdown from USR1/USR2 signals."""
+    global CLIENT_STANDALONE_MODE
+    CLIENT_STANDALONE_MODE = mode
+
+
 @dataclass
 class ClientInfo:
     """Client instance ID/hostname and task ID mapping."""
 
     client_id: str
     client_host: str
     task_ids: List[str]
@@ -174,14 +190,17 @@
         """Jump to GET_REMOTE state."""
         timeout_label = self.timeout or 'no'
         log.debug(f'Started (scheduler: {timeout_label} timeout)')
         return SchedulerState.GET_REMOTE
 
     def get_remote(self: ClientScheduler) -> SchedulerState:
         """Get the next task bundle from the server."""
+        if check_signal() in (SIGUSR1, SIGUSR2) and CLIENT_STANDALONE_MODE:
+            log.warning(f'Signal interrupt ({SIGNAL_MAP[check_signal()]})')
+            return SchedulerState.FINAL
         try:
             self.bundle = self.queue.scheduled.get(timeout=2)
             self.queue.scheduled.task_done()
             self.previous_received = datetime.now()
             if self.bundle is not None:
                 log.debug(f'Received {len(self.bundle)} tasks ({HOSTNAME}: {INSTANCE})')
                 return SchedulerState.UNPACK
@@ -221,15 +240,15 @@
             return SchedulerState.PUT_LOCAL
         except IndexError:
             return SchedulerState.GET_REMOTE
 
     def put_local(self: ClientScheduler) -> SchedulerState:
         """Put latest task on the local task queue."""
         try:
-            self.local.put(self.task, timeout=2)
+            self.local.put(self.task, timeout=1)
             return SchedulerState.POP_TASK
         except QueueFull:
             return SchedulerState.PUT_LOCAL
 
     @staticmethod
     def finalize() -> SchedulerState:
         """Stop scheduler."""
@@ -256,16 +275,19 @@
     def stop(self: ClientSchedulerThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (scheduler)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
-DEFAULT_BUNDLESIZE: int = default.client.bundlesize
-DEFAULT_BUNDLEWAIT: int = default.client.bundlewait
+DEFAULT_BUNDLESIZE: Final[int] = default.client.bundlesize
+"""Default size of task bundles."""
+
+DEFAULT_BUNDLEWAIT: Final[int] = default.client.bundlewait
+"""Default waiting period before forcing task bundle push."""
 
 
 class CollectorState(State, Enum):
     """Finite states of collector."""
     START = 0
     GET_LOCAL = 1
     CHECK_BUNDLE = 2
@@ -347,23 +369,26 @@
     def pack_bundle(self: ClientCollector) -> CollectorState:
         """Pack tasks into bundle before pushing back to server."""
         self.bundle = [task.pack() for task in self.tasks]
         return CollectorState.PUT_REMOTE
 
     def put_remote(self: ClientCollector) -> CollectorState:
         """Push out bundle of completed tasks."""
-        if self.bundle:
-            self.queue.completed.put(self.bundle)
-            log.trace(f'Bundle returned ({len(self.bundle)} tasks)')
-            self.tasks.clear()
-            self.bundle.clear()
-            self.previous_send = datetime.now()
-        else:
-            log.trace('Bundle empty')
-        return CollectorState.GET_LOCAL
+        try:
+            if self.bundle:
+                self.queue.completed.put(self.bundle, timeout=2)
+                log.trace(f'Bundle returned ({len(self.bundle)} tasks)')
+                self.tasks.clear()
+                self.bundle.clear()
+                self.previous_send = datetime.now()
+            else:
+                log.trace('Bundle empty')
+            return CollectorState.GET_LOCAL
+        except QueueFull:
+            return CollectorState.PUT_REMOTE
 
     def finalize(self: ClientCollector) -> CollectorState:
         """Push out any remaining tasks and halt."""
         self.put_remote()
         log.debug('Done (collector)')
         return CollectorState.HALT
 
@@ -384,55 +409,69 @@
     def stop(self: ClientCollectorThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (collector)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
+DEFAULT_SIGNALWAIT: Final[int] = default.task.signalwait
+"""Default signal escalation wait period in seconds."""
+
+
 def task_env(task: Task) -> Dict[str, str]:
     """Build environment dictionary for the given `task`."""
     task_data = task.to_json()
-    task_data.pop('tag')  # do not include tags in environ
+    try:
+        # We have to flatten tag data separately, otherwise we'd have TASK_TAG='{...}'
+        tag_data = Namespace(task_data.pop('tag')).to_env().flatten(prefix='TASK_TAG')
+    except Exception:  # noqa: any exception
+        tag_data = {}
     return {
         **os.environ,
         **load_task_env(),
         **Namespace.from_dict(task_data).to_env().flatten(prefix='TASK'),
+        **tag_data,
         'TASK_CWD': config.task.cwd,
         'TASK_OUTPATH': os.path.join(default_path.lib, 'task', f'{task.id}.out'),
         'TASK_ERRPATH': os.path.join(default_path.lib, 'task', f'{task.id}.err'),
     }
 
 
 class TaskState(State, Enum):
     """Finite states for task executor."""
     START = 0
     GET_LOCAL = 1
     CREATE_TASK = 2
     START_TASK = 3
     WAIT_TASK = 4
-    STOP_TASK = 5
-    TERM_TASK = 6
-    KILL_TASK = 7
-    PUT_LOCAL = 8
-    FINAL = 9
-    HALT = 10
+    CHECK_TASK = 5
+    WAIT_SIGNAL = 6
+    STOP_TASK = 7
+    TERM_TASK = 8
+    KILL_TASK = 9
+    PUT_LOCAL = 10
+    FINAL = 11
+    HALT = 12
 
 
 class TaskExecutor(StateMachine):
     """Run tasks locally."""
 
     id: int
     task: Task
     process: Popen
     template: Template
     redirect_output: IO
     redirect_errors: IO
     capture: bool
 
+    elapsed: timedelta
     timeout: Optional[int]
+    signalwait: int
+    stop_requested: Optional[datetime]
     attempted_sigint: bool
     attempted_sigterm: bool
     attempted_sigkill: bool
 
     inbound: Queue[Optional[Task]]
     outbound: Queue[Optional[Task]]
 
@@ -443,33 +482,37 @@
                  id: int,
                  inbound: Queue[Optional[Task]],
                  outbound: Queue[Optional[Task]],
                  template: str = DEFAULT_TEMPLATE,
                  redirect_output: IO = None,
                  redirect_errors: IO = None,
                  capture: bool = False,
-                 timeout: int = None) -> None:
+                 timeout: int = None,
+                 signalwait: int = DEFAULT_SIGNALWAIT) -> None:
         """Initialize task executor."""
         self.id = id
         self.template = Template(template)
         self.inbound = inbound
         self.outbound = outbound
         self.redirect_output = redirect_output or sys.stdout
         self.redirect_errors = redirect_errors or sys.stderr
         self.capture = capture
         self.timeout = timeout
+        self.signalwait = signalwait
 
     @functools.cached_property
     def actions(self: TaskExecutor) -> Dict[TaskState, Callable[[], TaskState]]:
         return {
             TaskState.START: self.start,
             TaskState.GET_LOCAL: self.get_local,
             TaskState.CREATE_TASK: self.create_task,
             TaskState.START_TASK: self.start_task,
             TaskState.WAIT_TASK: self.wait_task,
+            TaskState.CHECK_TASK: self.check_task,
+            TaskState.WAIT_SIGNAL: self.wait_signal,
             TaskState.STOP_TASK: self.stop_task,
             TaskState.TERM_TASK: self.term_task,
             TaskState.KILL_TASK: self.kill_task,
             TaskState.PUT_LOCAL: self.put_local,
             TaskState.FINAL: self.finalize,
         }
 
@@ -499,23 +542,24 @@
             self.task.start_time = datetime.now().astimezone()
             self.task.completion_time = datetime.now().astimezone()
             self.task.exit_status = -1
             return TaskState.PUT_LOCAL
 
     def start_task(self: TaskExecutor) -> TaskState:
         """Start current task locally."""
+        # NOTE: enforce tz aware submit_time (in case of sqlite backend)
+        self.task.start_time = datetime.now().astimezone()
+        self.task.waited = int((self.task.start_time - self.task.submit_time.astimezone()).total_seconds())
         env = task_env(self.task)
         if self.capture:
             self.task.outpath = env['TASK_OUTPATH']
             self.task.errpath = env['TASK_ERRPATH']
             self.redirect_output = open(self.task.outpath, mode='w')
             self.redirect_errors = open(self.task.errpath, mode='w')
-        self.task.start_time = datetime.now().astimezone()
-        # NOTE: enforce tz aware submit_time (in case of sqlite backend)
-        self.task.waited = int((self.task.start_time - self.task.submit_time.astimezone()).total_seconds())
+        self.stop_requested = None
         self.attempted_sigint = False
         self.attempted_sigterm = False
         self.attempted_sigkill = False
         self.process = Popen(self.task.command, shell=True,
                              stdout=self.redirect_output, stderr=self.redirect_errors,
                              cwd=config.task.cwd, env=env)
         log.info(f'Running task ({self.task.id})')
@@ -531,57 +575,77 @@
             self.task.duration = int((self.task.completion_time - self.task.start_time).total_seconds())
             log.debug(f'Completed task ({self.task.id})')
             if self.capture:
                 self.redirect_output.close()
                 self.redirect_errors.close()
             return TaskState.PUT_LOCAL
         except TimeoutExpired:
-            # Only include time elapsed to the nearest second (we don't need fractions)
-            elapsed = timedelta(seconds=round((datetime.now().astimezone() - self.task.start_time).total_seconds()))
-            log.trace(f'Waiting on task ({self.task.id}: {elapsed})')
-            if self.timeout is None or elapsed.total_seconds() < self.timeout:
-                return TaskState.WAIT_TASK
-            elif self.attempted_sigint is False:
-                log.warning(f'Task exceeded walltime limit ({elapsed})')
-                return TaskState.STOP_TASK
-            elif self.attempted_sigterm is False:
-                log.error(f'Interrupt ignored ({self.task.id})')
-                return TaskState.TERM_TASK
+            # Only display time elapsed to the nearest second
+            self.elapsed = timedelta(seconds=round((datetime.now().astimezone() -
+                                                    self.task.start_time).total_seconds()))
+            log.trace(f'Waiting on task ({self.task.id}: {self.elapsed})')
+            if self.stop_requested:
+                return TaskState.WAIT_SIGNAL
             else:
-                log.error(f'Terminate ignored ({self.task.id})')
-                return TaskState.KILL_TASK
+                return TaskState.CHECK_TASK
+
+    def check_task(self: TaskExecutor) -> TaskState:
+        """Check for timeout or interrupts."""
+        if check_signal() == SIGUSR2:  # NOTE: regardless of CLIENT_STANDALONE_MODE
+            log.warning(f'Signal interrupt (SIGUSR2: executor-{self.id})')
+            self.stop_requested = datetime.now()
+            return TaskState.WAIT_SIGNAL
+        elif self.timeout is None or self.elapsed.total_seconds() < self.timeout:
+            return TaskState.WAIT_TASK
+        else:
+            log.warning(f'Task exceeded walltime limit ({self.elapsed})')
+            self.stop_requested = datetime.now()
+            return TaskState.WAIT_SIGNAL
+
+    def wait_signal(self: TaskExecutor) -> TaskState:
+        """Wait on interrupts."""
+        if self.attempted_sigint is False:
+            return TaskState.STOP_TASK
+        elif (datetime.now() - self.stop_requested).total_seconds() < 1 * self.signalwait:
+            return TaskState.WAIT_TASK
+        elif self.attempted_sigterm is False:
+            log.error(f'Interrupt ignored ({self.task.id})')
+            return TaskState.TERM_TASK
+        elif (datetime.now() - self.stop_requested).total_seconds() < 2 * self.signalwait:
+            return TaskState.WAIT_TASK
+        elif self.attempted_sigkill is False:
+            log.error(f'Terminate ignored ({self.task.id})')
+            return TaskState.KILL_TASK
+        elif (datetime.now() - self.stop_requested).total_seconds() < 3 * self.signalwait:
+            return TaskState.WAIT_TASK
+        else:
+            log.critical(f'Process ignored SIGKILL ({self.task.id}: {self.process.pid})')
+            log.critical(f'Shutting down executor ({self.id})')
+            return TaskState.FINAL
 
     def stop_task(self: TaskExecutor) -> TaskState:
         """Send SIGINT to task process."""
         log.debug(f'Sending SIGINT ({self.task.id}: {self.process.pid})')
-        self.process.send_signal(signal.SIGINT)
+        self.process.send_signal(SIGINT)
         self.attempted_sigint = True
-        time.sleep(2)  # additional grace period
         return TaskState.WAIT_TASK
 
     def term_task(self: TaskExecutor) -> TaskState:
         """Send SIGTERM to task process."""
         log.debug(f'Sending SIGTERM ({self.task.id}: {self.process.pid})')
         self.process.terminate()
         self.attempted_sigterm = True
-        time.sleep(2)  # additional grace period
         return TaskState.WAIT_TASK
 
     def kill_task(self: TaskExecutor) -> TaskState:
         """Send SIGKILL or halt executor if ignored."""
-        if self.attempted_sigkill is False:
-            log.debug(f'Sending SIGKILL ({self.task.id}: {self.process.pid})')
-            self.process.kill()
-            self.attempted_sigkill = True
-            time.sleep(2)  # additional grace period
-            return TaskState.WAIT_TASK
-        else:
-            log.critical(f'Process ignored SIGKILL ({self.task.id}: {self.process.pid})')
-            log.critical(f'Shutting down executor ({self.id})')
-            return TaskState.FINAL
+        log.debug(f'Sending SIGKILL ({self.task.id}: {self.process.pid})')
+        self.process.kill()
+        self.attempted_sigkill = True
+        return TaskState.WAIT_TASK
 
     def put_local(self: TaskExecutor) -> TaskState:
         """Put completed task on outbound queue."""
         try:
             self.outbound.put(self.task, timeout=1)
             return TaskState.GET_LOCAL
         except QueueFull:
@@ -606,21 +670,22 @@
                  id: int,
                  inbound: Queue[Optional[str]],
                  outbound: Queue[Optional[str]],
                  template: str = DEFAULT_TEMPLATE,
                  capture: bool = False,
                  redirect_output: IO = None,
                  redirect_errors: IO = None,
-                 timeout: int = None) -> None:
+                 timeout: int = None,
+                 signalwait: int = DEFAULT_SIGNALWAIT) -> None:
         """Initialize task executor."""
         self.id = id
         super().__init__(name=f'hypershell-executor-{id}')
         self.machine = TaskExecutor(id=id, inbound=inbound, outbound=outbound, template=template,
                                     redirect_output=redirect_output, redirect_errors=redirect_errors,
-                                    capture=capture, timeout=timeout)
+                                    capture=capture, timeout=timeout, signalwait=signalwait)
 
     def run_with_exceptions(self: TaskThread) -> None:
         """Run machine."""
         self.machine.run()
 
     def stop(self: TaskThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
@@ -634,15 +699,16 @@
     START = 0
     SUBMIT = 1
     WAIT = 2
     FINAL = 3
     HALT = 4
 
 
-DEFAULT_HEARTRATE: int = default.client.heartrate
+DEFAULT_HEARTRATE: Final[int] = default.client.heartrate
+"""Period in seconds to wait between heartbeats."""
 
 
 class ClientHeartbeat(StateMachine):
     """Register heartbeats with remote server."""
 
     queue: QueueClient
     heartrate: timedelta
@@ -729,23 +795,102 @@
     def stop(self: ClientHeartbeatThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (heartbeat)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
-# Only create one task executor by default
-DEFAULT_NUM_TASKS = 1
+DEFAULT_NUM_TASKS: Final[int] = 1
+"""Default number of task executors per client."""
 
 # We do not delay connecting to the server unless explicitly specified
-DEFAULT_DELAY = 0
+DEFAULT_DELAY: Final[int] = 0
+"""Default delay in seconds on client startup."""
+
+DEFAULT_HOST: Final[str] = QueueConfig.host
+"""Default host for server connection."""
+
+DEFAULT_PORT: Final[int] = QueueConfig.port
+"""Default port for server connection."""
+
+DEFAULT_AUTH: Final[str] = QueueConfig.auth
+"""Default authentication key for server (**DO NOT USE THIS**)."""
 
 
 class ClientThread(Thread):
-    """Manage asynchronous task bundle scheduling and receiving."""
+    """
+    Run client within dedicated thread.
+    Run until either disconnect requested from server or `client_timeout` reached.
+
+    Args:
+        num_tasks (int, optional):
+            Number of parallel task executor threads.
+            See :const:`DEFAULT_NUM_TASKS`.
+
+        bundlesize (int optional):
+            Size of task bundles returned to server.
+            See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int optional):
+            Waiting period in seconds before forcing return of task bundle to server.
+            See :const:`DEFAULT_BUNDLEWAIT`.
+
+        address (tuple, optional):
+            Server host address for server with port number.
+            See :const:`DEFAULT_HOST` and :const:`DEFAULT_PORT`.
+
+        auth (str, optional):
+            Server authentication key.
+            See :const:`DEFAULT_AUTH`.
+
+        template (str, optional):
+            Template command pattern. See :const:`DEFAULT_TEMPLATE`.
+
+        redirect_output (IO, optional):
+            Optional file-like object for <stdout> redirect.
+
+        redirect_errors (IO, optional):
+            Optional file-like object for <stderr> redirect.
+
+        heartrate (int, optional):
+            Period in seconds to wait between heartbeats.
+            See :const:`DEFAULT_HEARTRATE`,
+
+        capture (bool, optional):
+            Isolate task <stdout> and <stderr> in discrete files.
+            Defaults to `False`.
+
+        delay_start (float, optional):
+            Delay in seconds before connecting to server.
+            See :const:`DEFAULT_DELAY`.
+
+        no_confirm (bool, optional):
+            Disable client confirmation of tasks received.
+
+        client_timeout (int, optional):
+            Timeout in seconds before disconnecting from server.
+            By default, the client waits for server tor request disconnect.
+
+        task_timeout (int, optional):
+            Task-level walltime limit in seconds.
+            By default, the client waits indefinitely on tasks.
+
+        task_signalwait (int, optional):
+            Signal escalation waiting period in seconds on task timeout.
+            See :const:`DEFAULT_SIGNALWAIT`.
+
+    Example:
+        >>> from hypershell.client import ClientThread
+        >>> client = ClientThread.new(num_tasks=16, address=('localhost', 54321),
+        ...                           auth='my-secret-key', capture=True)
+        >>> client.join()
+
+    See Also:
+        - :meth:`run_client`
+    """
 
     client: QueueClient
     num_tasks: int
     delay_start: float
     no_confirm: bool
 
     inbound: Queue[Optional[Task]]
@@ -754,25 +899,26 @@
     collector: ClientCollectorThread
     executors: List[TaskThread]
 
     def __init__(self: ClientThread,
                  num_tasks: int = DEFAULT_NUM_TASKS,
                  bundlesize: int = DEFAULT_BUNDLESIZE,
                  bundlewait: int = DEFAULT_BUNDLEWAIT,
-                 address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port),
-                 auth: str = QueueConfig.auth,
+                 address: Tuple[str, int] = (DEFAULT_HOST, DEFAULT_PORT),
+                 auth: str = DEFAULT_AUTH,
                  template: str = DEFAULT_TEMPLATE,
                  redirect_output: IO = None,
                  redirect_errors: IO = None,
                  heartrate: int = DEFAULT_HEARTRATE,
                  capture: bool = False,
                  delay_start: float = DEFAULT_DELAY,
                  no_confirm: bool = False,
                  client_timeout: int = None,
-                 task_timeout: int = None) -> None:
+                 task_timeout: int = None,
+                 task_signalwait: int = DEFAULT_SIGNALWAIT) -> None:
         """Initialize queue manager and child threads."""
         super().__init__(name='hypershell-client')
         self.num_tasks = num_tasks
         self.delay_start = delay_start
         self.no_confirm = no_confirm
         self.client = QueueClient(config=QueueConfig(host=address[0], port=address[1], auth=auth))
         self.inbound = Queue(maxsize=bundlesize)
@@ -781,15 +927,16 @@
                                                no_confirm=no_confirm, timeout=client_timeout)
         self.heartbeat = ClientHeartbeatThread(queue=self.client, heartrate=heartrate)
         self.collector = ClientCollectorThread(queue=self.client, local=self.outbound,
                                                bundlesize=bundlesize, bundlewait=bundlewait)
         self.executors = [TaskThread(id=count+1,
                                      inbound=self.inbound, outbound=self.outbound,
                                      redirect_output=redirect_output, redirect_errors=redirect_errors,
-                                     template=template, capture=capture, timeout=task_timeout)
+                                     template=template, capture=capture, timeout=task_timeout,
+                                     signalwait=task_signalwait)
                           for count in range(num_tasks)]
 
     def run_with_exceptions(self: ClientThread) -> None:
         """Start child threads, wait."""
         log.debug(f'Started ({self.num_tasks} executors)')
         self.wait_start()
         with self.client:
@@ -850,50 +997,134 @@
         log.warning('Stopping')
         self.scheduler.stop(wait=wait, timeout=timeout)
         self.collector.stop(wait=wait, timeout=timeout)
         super().stop(wait=wait, timeout=timeout)
 
 
 def run_client(num_tasks: int = DEFAULT_NUM_TASKS,
-               bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-               address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
-               template: str = DEFAULT_TEMPLATE, redirect_output: IO = None, redirect_errors: IO = None,
-               capture: bool = False, heartrate: int = DEFAULT_HEARTRATE,
-               delay_start: float = DEFAULT_DELAY, no_confirm: bool = False,
-               client_timeout: int = None, task_timeout: int = None) -> None:
-    """Run client until disconnect signal received."""
-    thread = ClientThread.new(num_tasks=num_tasks, bundlesize=bundlesize, bundlewait=bundlewait,
-                              address=address, auth=auth, template=template, capture=capture,
-                              redirect_output=redirect_output, redirect_errors=redirect_errors,
-                              heartrate=heartrate, delay_start=delay_start, no_confirm=no_confirm,
-                              client_timeout=client_timeout, task_timeout=task_timeout)
+               bundlesize: int = DEFAULT_BUNDLESIZE,
+               bundlewait: int = DEFAULT_BUNDLEWAIT,
+               address: Tuple[str, int] = (DEFAULT_HOST, DEFAULT_PORT),
+               auth: str = DEFAULT_AUTH,
+               template: str = DEFAULT_TEMPLATE,
+               redirect_output: IO = None,
+               redirect_errors: IO = None,
+               capture: bool = False,
+               heartrate: int = DEFAULT_HEARTRATE,
+               delay_start: float = DEFAULT_DELAY,
+               no_confirm: bool = False,
+               client_timeout: int = None,
+               task_timeout: int = None,
+               task_signalwait: int = DEFAULT_SIGNALWAIT) -> None:
+    """
+    Run client until disconnect signal received or `client_timeout` reached.
+
+    Args:
+        num_tasks (int, optional):
+            Number of parallel task executor threads.
+            See :const:`DEFAULT_NUM_TASKS`.
+
+        bundlesize (int optional):
+            Size of task bundles returned to server.
+            See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int optional):
+            Waiting period in seconds before forcing return of task bundle to server.
+            See :const:`DEFAULT_BUNDLEWAIT`.
+
+        address (tuple, optional):
+            Server host address for server with port number.
+            See :const:`DEFAULT_HOST` and :const:`DEFAULT_PORT`.
+
+        auth (str, optional):
+            Server authentication key.
+            See :const:`DEFAULT_AUTH`.
+
+        template (str, optional):
+            Template command pattern. See :const:`DEFAULT_TEMPLATE`.
+
+        redirect_output (IO, optional):
+            Optional file-like object for <stdout> redirect.
+
+        redirect_errors (IO, optional):
+            Optional file-like object for <stderr> redirect.
+
+        heartrate (int, optional):
+            Period in seconds to wait between heartbeats.
+            See :const:`DEFAULT_HEARTRATE`,
+
+        capture (bool, optional):
+            Isolate task <stdout> and <stderr> in discrete files.
+            Defaults to `False`.
+
+        delay_start (float, optional):
+            Delay in seconds before connecting to server.
+            See :const:`DEFAULT_DELAY`.
+
+        no_confirm (bool, optional):
+            Disable client confirmation of tasks received.
+
+        client_timeout (int, optional):
+            Timeout in seconds before disconnecting from server.
+            By default, the client waits for server tor request disconnect.
+
+        task_timeout (int, optional):
+            Task-level walltime limit in seconds.
+            By default, the client waits indefinitely on tasks.
+
+        task_signalwait (int, optional):
+            Signal escalation waiting period in seconds on task timeout.
+            See :const:`DEFAULT_SIGNALWAIT`.
+
+    Example:
+        >>> from hypershell.client import run_client
+        >>> run_client(num_tasks=16, address=('localhost', 54321),
+        ...            auth='my-secret-key', capture=True)
+
+    See Also:
+        - :meth:`ClientThread`
+    """
+    thread = ClientThread.new(num_tasks=num_tasks,
+                              bundlesize=bundlesize,
+                              bundlewait=bundlewait,
+                              address=address,
+                              auth=auth,
+                              template=template,
+                              capture=capture,
+                              redirect_output=redirect_output,
+                              redirect_errors=redirect_errors,
+                              heartrate=heartrate,
+                              delay_start=delay_start,
+                              no_confirm=no_confirm,
+                              client_timeout=client_timeout,
+                              task_timeout=task_timeout,
+                              task_signalwait=task_signalwait)
     try:
         thread.join()
     except Exception:
         thread.stop()
         raise
 
 
-APP_NAME = 'hyper-shell client'
+APP_NAME = 'hs client'
 APP_USAGE = f"""\
 Usage:
-hyper-shell client [-h] [-N NUM] [-t CMD] [-b SIZE] [-w SEC] [-H ADDR] [-p PORT]
-                   [-k KEY] [--capture | [-o PATH] [-e PATH]] [--no-confirm]
-                   [--delay-start SEC] [--timeout SEC] [--task-timeout SEC]
+  hs client [-h] [-N NUM] [-t CMD] [-b SIZE] [-w SEC] [-H ADDR] [-p PORT] [-k KEY] 
+            [--capture | [-o PATH] [-e PATH]] [--no-confirm] [-d SEC] [-T SEC] [-W SEC] [-S SEC]
 
-Launch client directly, run tasks in parallel.\
+  Launch client directly, run tasks in parallel.\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
-Tasks are pulled off of the shared queue in bundles from the server and run
-locally within the same shell as the client. By default the bundle size is one,
-meaning that at small scales there is greater responsiveness. It is recommended
-to coordinate these parameters to be the same as the server.
+  Tasks are pulled off of the shared queue in bundles from the server and run
+  locally within the same shell as the client. By default the bundle size is one,
+  meaning that at small scales there is greater responsiveness. It is recommended
+  to coordinate these parameters to be the same as the server.
 
 Options:
   -N, --num-tasks     NUM   Number of tasks to run in parallel (default: {DEFAULT_NUM_TASKS}).
   -t, --template      CMD   Command-line template pattern (default: "{DEFAULT_TEMPLATE}").
   -b, --bundlesize    SIZE  Bundle size for finished tasks (default: {DEFAULT_BUNDLESIZE}).
   -w, --bundlewait    SEC   Seconds to wait before flushing tasks (default: {DEFAULT_BUNDLEWAIT}).
   -H, --host          ADDR  Hostname for server.
@@ -902,25 +1133,24 @@
   -d, --delay-start   SEC   Seconds to wait before start-up (default: {DEFAULT_DELAY}).
       --no-confirm          Disable confirmation of task bundle received.
   -o, --output        PATH  Redirect task output (default: <stdout>).
   -e, --errors        PATH  Redirect task errors (default: <stderr>).
   -c, --capture             Capture individual task <stdout> and <stderr>.
   -T, --timeout       SEC   Automatically shutdown if no tasks received (default: never).
   -W, --task-timeout  SEC   Task-level walltime limit (default: none).
+  -S, --signalwait    SEC   Task-level signal escalation wait period (default: {DEFAULT_SIGNALWAIT}).
   -h, --help                Show this message and exit.\
 """
 
 
 class ClientApp(Application):
     """Run individual client directly."""
 
     name = APP_NAME
-    interface = Interface(APP_NAME,
-                          colorize_usage(APP_USAGE),
-                          colorize_usage(APP_HELP))
+    interface = Interface(APP_NAME, APP_USAGE, APP_HELP)
 
     num_tasks: int = DEFAULT_NUM_TASKS
     interface.add_argument('-N', '--num-tasks', type=int, default=num_tasks)
 
     host: str = config.server.bind
     interface.add_argument('-H', '--host', default=host)
 
@@ -943,25 +1173,32 @@
     interface.add_argument('-d', '--delay-start', type=float, default=delay_start)
 
     task_timeout: int = config.task.timeout
     client_timeout: int = config.client.timeout
     interface.add_argument('-T', '--timeout', type=int, default=client_timeout, dest='client_timeout')
     interface.add_argument('-W', '--task-timeout', type=int, default=task_timeout, dest='task_timeout')
 
+    task_signalwait: int = config.task.signalwait
+    interface.add_argument('-S', '--task-signalwait', type=int, default=task_signalwait, dest='task_signalwait')
+
     no_confirm: bool = False
     interface.add_argument('--no-confirm', action='store_true')
 
     output_path: str = None
     errors_path: str = None
     interface.add_argument('-o', '--output', default=None, dest='output_path')
     interface.add_argument('-e', '--errors', default=None, dest='errors_path')
 
     capture: bool = False
     interface.add_argument('-c', '--capture', action='store_true')
 
+    # Hidden options used as helpers for shell completion
+    interface.add_argument('--available-cores', action='version', version=str(cpu_count()))
+    interface.add_argument('--available-ssh-groups', action='version', version='\n'.join(SSH_GROUPS))
+
     exceptions = {
         EOFError: functools.partial(handle_disconnect, logger=log),
         ConnectionResetError: functools.partial(handle_disconnect, logger=log),
         ConnectionRefusedError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
         AuthenticationError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
         HostAddressInfo: functools.partial(handle_address_unknown, logger=log, status=exit_status.runtime_error),
         **get_shared_exception_mapping(__name__),
@@ -980,15 +1217,16 @@
                        redirect_output=self.output_stream,
                        redirect_errors=self.errors_stream,
                        capture=self.capture,
                        delay_start=self.delay_start,
                        no_confirm=self.no_confirm,
                        heartrate=config.client.heartrate,
                        client_timeout=self.client_timeout,
-                       task_timeout=self.task_timeout)
+                       task_timeout=self.task_timeout,
+                       task_signalwait=self.task_signalwait)
         except gaierror:
             raise HostAddressInfo(f'Could not resolve host \'{self.host}\'')
 
     def check_args(self: ClientApp) -> None:
         """Check for logical errors in command-line arguments."""
         if self.capture and (self.output_path or self.errors_path):
             raise ArgumentError('Cannot specify --capture with either --output or --errors')
```

### Comparing `hyper-shell-2.4.0/src/hypershell/cluster/__init__.py` & `hyper_shell-2.5.0/src/hypershell/cluster/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Run full cluster with server and managed clients."""
 
 
 # type annotations
 from __future__ import annotations
 from typing import IO, Optional, Iterable, Dict, Callable, Type
 from types import TracebackType
 
 # standard libs
 import sys
+import shlex
 from functools import cached_property
 
 # external libs
 from cmdkit.app import Application
 from cmdkit.cli import Interface, ArgumentError
 
 # internal libs
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.config import config, blame
 from hypershell.core.queue import QueueConfig
 from hypershell.core.logging import Logger
 from hypershell.core.template import DEFAULT_TEMPLATE
 from hypershell.core.exceptions import get_shared_exception_mapping
 from hypershell.data import initdb, checkdb
-from hypershell.client import DEFAULT_NUM_TASKS, DEFAULT_DELAY
+from hypershell.client import DEFAULT_NUM_TASKS, DEFAULT_DELAY, DEFAULT_SIGNALWAIT
 from hypershell.server import DEFAULT_BUNDLESIZE, DEFAULT_ATTEMPTS
 from hypershell.submit import DEFAULT_BUNDLEWAIT
 from hypershell.cluster.ssh import run_ssh, SSHCluster, NodeList
 from hypershell.cluster.local import run_local, LocalCluster
 from hypershell.cluster.remote import (run_cluster, RemoteCluster, AutoScalingCluster,
                                        DEFAULT_AUTOSCALE_FACTOR, DEFAULT_AUTOSCALE_PERIOD,
                                        DEFAULT_AUTOSCALE_MIN_SIZE, DEFAULT_AUTOSCALE_MAX_SIZE,
@@ -40,24 +40,24 @@
            'LocalCluster', 'RemoteCluster', 'AutoScalingCluster', 'SSHCluster',
            'ClusterApp', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
-APP_NAME = 'hyper-shell cluster'
-APP_USAGE = f"""\
+APP_NAME = 'hs cluster'
+APP_USAGE = """\
 Usage:
-hyper-shell cluster [-h] [FILE | --restart | --forever] [-N NUM] [-t CMD] [-b SIZE] [-w SEC]
-                    [-p PORT] [-r NUM [--eager]] [-f PATH] [--capture | [-o PATH] [-e PATH]]
-                    [--ssh [HOST... | --ssh-group NAME] [--env] | --mpi | --launcher=ARGS...]
-                    [--no-db | --initdb] [--no-confirm] [--delay-start SEC] [-T SEC] [-W SEC]
-                    [--autoscaling [MODE] [-P SEC] [-F VALUE] [-I NUM] [-X NUM] [-Y NUM]] 
+  hs cluster [-h] [FILE | --restart | --forever] [-N NUM] [-t CMD] [-b SIZE] [-w SEC]
+             [-p PORT] [-r NUM [--eager]] [-f PATH] [--capture | [-o PATH] [-e PATH]]
+             [--ssh [HOST... | --ssh-group NAME] [--env] | --mpi | --launcher=ARGS...]
+             [--no-db | --initdb] [--no-confirm] [-d SEC] [-T SEC] [-W SEC] [-S SEC]
+             [--autoscaling [MODE] [-P SEC] [-F VALUE] [-I NUM] [-X NUM] [-Y NUM]]
 
-Start cluster locally, over SSH, or with a custom launcher.\
+  Start cluster locally, over SSH, or with a custom launcher.\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
 Arguments:
   FILE                         Path to input task file (default: <stdin>).
@@ -79,41 +79,40 @@
       --initdb                 Auto-initialize database.
       --no-confirm             Disable client confirmation of task bundle received.
       --forever                Schedule forever.
       --restart                Start scheduling from last completed task.
       --ssh-args      ARGS     Command-line arguments for SSH.
       --ssh-group     NAME     SSH nodelist group in config.
   -E, --env                    Send environment variables.
+      --remote-exe    PATH     Path to executable on remote hosts.
   -d, --delay-start   SEC      Delay time for launching clients (default: {DEFAULT_DELAY}).
-  -c, --capture                Capture individual task <stdout> and <stderr>.         
+  -c, --capture                Capture individual task <stdout> and <stderr>.
   -o, --output        PATH     File path for task outputs (default: <stdout>).
   -e, --errors        PATH     File path for task errors (default: <stderr>).
   -f, --failures      PATH     File path to write failed task args (default: <none>).
   -T, --timeout       SEC      Automatically shutdown clients if no tasks received (default: never).
   -W, --task-timeout  SEC      Task-level walltime limit (default: none).
+  -S, --signalwait    SEC      Task-level signal escalation wait period (default: {DEFAULT_SIGNALWAIT}).
   -A, --autoscaling  [MODE]    Enable autoscaling (default: disabled). Used with --launcher.
   -F, --factor        VALUE    Scaling factor (default: 1).
   -P, --period        SEC      Scaling period in seconds (default: {DEFAULT_AUTOSCALE_PERIOD}).
   -I, --init-size     SIZE     Initial size of cluster (default: {DEFAULT_AUTOSCALE_INIT_SIZE}).
   -X, --min-size      SIZE     Minimum size of cluster (default: {DEFAULT_AUTOSCALE_MIN_SIZE}).
   -Y, --max-size      SIZE     Maximum size of cluster (default: {DEFAULT_AUTOSCALE_MAX_SIZE}).
   -h, --help                   Show this message and exit.\
 """
 
 
 class ClusterApp(Application):
     """Run managed cluster."""
 
     name = APP_NAME
-    interface = Interface(APP_NAME,
-                          colorize_usage(APP_USAGE),
-                          colorize_usage(APP_HELP))
+    interface = Interface(APP_NAME, APP_USAGE, APP_HELP)
 
     filepath: str
-    source: Optional[IO] = None
     interface.add_argument('filepath', nargs='?', default=None)
 
     num_tasks: int = 1
     interface.add_argument('-N', '--num-tasks', type=int, default=num_tasks)
 
     template: str = DEFAULT_TEMPLATE
     interface.add_argument('-t', '--template', default=template)
@@ -181,14 +180,17 @@
     interface.add_argument('-f', '--failures', default=None, dest='failure_path')
 
     task_timeout: int = config.task.timeout
     client_timeout: int = config.client.timeout
     interface.add_argument('-T', '--timeout', type=int, default=client_timeout, dest='client_timeout')
     interface.add_argument('-W', '--task-timeout', type=int, default=task_timeout, dest='task_timeout')
 
+    task_signalwait: int = config.task.signalwait
+    interface.add_argument('-S', '--signalwait', type=int, default=task_signalwait, dest='task_signalwait')
+
     autoscaling_policy: str = None
     autoscaling_factor: float = config.autoscale.factor
     autoscaling_period: int = config.autoscale.period
     autoscaling_minimum: int = config.autoscale.size.min
     autoscaling_maximum: int = config.autoscale.size.max
     autoscaling_initial: int = config.autoscale.size.init
     interface.add_argument('-A', '--autoscaling', nargs='?', default=None,
@@ -207,15 +209,16 @@
         """Run cluster."""
         launcher = self.launchers.get(self.mode)
         launcher(source=self.source, num_tasks=self.num_tasks, template=self.template,
                  bundlesize=self.bundlesize, bundlewait=self.bundlewait, max_retries=self.max_retries,
                  in_memory=self.in_memory, no_confirm=self.no_confirm, forever_mode=self.forever_mode,
                  restart_mode=self.restart_mode, redirect_failures=self.failure_stream,
                  delay_start=self.delay_start, capture=self.capture,
-                 client_timeout=self.client_timeout, task_timeout=self.task_timeout)
+                 client_timeout=self.client_timeout, task_timeout=self.task_timeout,
+                 task_signalwait=self.task_signalwait)
 
     def run_local(self: ClusterApp, **options) -> None:
         """Run local cluster."""
         run_local(**options, redirect_output=self.output_stream, redirect_errors=self.errors_stream)
 
     def run_launch(self: ClusterApp, **options) -> None:
         """Run remote cluster with custom launcher."""
@@ -229,15 +232,15 @@
 
     def run_ssh(self: ClusterApp, **options) -> None:
         """Run remote cluster with SSH."""
         if self.ssh_group:
             nodelist = NodeList.from_config(self.ssh_group)
         else:
             nodelist = NodeList.from_cmdline(self.ssh_mode if self.ssh_mode != '<default>' else None)
-        run_ssh(**options, launcher='ssh', launcher_args=[self.ssh_args, ], nodelist=nodelist,
+        run_ssh(**options, launcher='ssh', launcher_args=shlex.split(self.ssh_args), nodelist=nodelist,
                 remote_exe=self.remote_exe, bind=('0.0.0.0', self.port), export_env=self.export_env)
 
     def run_autoscaling(self: ClusterApp, **options) -> None:
         """Run remote cluster with custom launcher and autoscaling."""
         run_cluster(**options, autoscaling=True, launcher=(self.launch_mode or ''),
                     policy=self.autoscaling_policy, factor=self.autoscaling_factor,
                     period=self.autoscaling_period, init_size=self.autoscaling_initial,
```

### Comparing `hyper-shell-2.4.0/src/hypershell/cluster/local.py` & `hyper_shell-2.5.0/src/hypershell/cluster/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Local cluster implementation."""
 
 
 # type annotations
 from __future__ import annotations
@@ -14,15 +14,15 @@
 
 # internal libs
 from hypershell.core.thread import Thread
 from hypershell.core.logging import Logger
 from hypershell.core.template import DEFAULT_TEMPLATE
 from hypershell.submit import DEFAULT_BUNDLEWAIT
 from hypershell.server import ServerThread, DEFAULT_BUNDLESIZE, DEFAULT_ATTEMPTS
-from hypershell.client import ClientThread, DEFAULT_DELAY
+from hypershell.client import ClientThread, DEFAULT_DELAY, DEFAULT_SIGNALWAIT, set_client_standalone
 
 # public interface
 __all__ = ['run_local', 'LocalCluster']
 
 # initialize logger
 log = Logger.with_name('hypershell.cluster')
 
@@ -57,29 +57,32 @@
                  eager: bool = False,
                  redirect_failures: IO = None,
                  redirect_output: IO = None,
                  redirect_errors: IO = None,
                  delay_start: float = DEFAULT_DELAY,
                  capture: bool = False,
                  client_timeout: int = None,
-                 task_timeout: int = None) -> None:
+                 task_timeout: int = None,
+                 task_signalwait: int = DEFAULT_SIGNALWAIT) -> None:
         """Initialize server and client threads."""
         auth = secrets.token_hex(64)
         self.server = ServerThread(source=source, auth=auth, in_memory=in_memory, no_confirm=no_confirm,
                                    bundlesize=bundlesize, bundlewait=bundlewait,
                                    max_retries=max_retries, eager=eager, forever_mode=forever_mode,
                                    restart_mode=restart_mode, redirect_failures=redirect_failures)
         self.client = ClientThread(num_tasks=num_tasks, template=template, auth=auth, no_confirm=no_confirm,
                                    bundlesize=bundlesize, bundlewait=bundlewait, delay_start=delay_start,
                                    redirect_output=redirect_output, redirect_errors=redirect_errors,
-                                   capture=capture, client_timeout=client_timeout, task_timeout=task_timeout)
+                                   capture=capture, client_timeout=client_timeout, task_timeout=task_timeout,
+                                   task_signalwait=task_signalwait)
         super().__init__(name='hypershell-cluster')
 
     def run_with_exceptions(self: LocalCluster) -> None:
         """Start child threads, wait."""
+        set_client_standalone(False)
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         self.client.start()
         self.client.join()
         self.server.join()
 
     def stop(self: LocalCluster, wait: bool = False, timeout: int = None) -> None:
```

### Comparing `hyper-shell-2.4.0/src/hypershell/cluster/remote.py` & `hyper_shell-2.5.0/src/hypershell/cluster/remote.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Remote cluster implementation."""
 
+
 # type annotations
 from __future__ import annotations
 from typing import Tuple, List, Dict, IO, Iterable, Callable, Type
 
 # standard libs
 import os
 import sys
 import time
+import shlex
 import secrets
 from enum import Enum
 from datetime import datetime, timedelta
 from functools import cached_property
 from subprocess import Popen
 
 # internal libs
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.config import default, load_task_env
 from hypershell.core.queue import QueueConfig
 from hypershell.core.thread import Thread
 from hypershell.core.logging import Logger, HOSTNAME
 from hypershell.core.template import DEFAULT_TEMPLATE
 from hypershell.data.model import Task, Client
-from hypershell.client import DEFAULT_DELAY
+from hypershell.client import DEFAULT_DELAY, DEFAULT_SIGNALWAIT
 from hypershell.submit import DEFAULT_BUNDLEWAIT
 from hypershell.server import ServerThread, DEFAULT_BUNDLESIZE, DEFAULT_ATTEMPTS
 
 # public interface
 __all__ = ['run_cluster', 'RemoteCluster', 'AutoScalingCluster',
            'DEFAULT_AUTOSCALE_POLICY', 'DEFAULT_AUTOSCALE_PERIOD', 'DEFAULT_AUTOSCALE_FACTOR',
            'DEFAULT_AUTOSCALE_INIT_SIZE', 'DEFAULT_AUTOSCALE_MIN_SIZE', 'DEFAULT_AUTOSCALE_MAX_SIZE',
@@ -53,15 +55,15 @@
 
 
 class RemoteCluster(Thread):
     """Run server with remote clients via external launcher (e.g., MPI)."""
 
     server: ServerThread
     clients: Popen
-    client_argv: str
+    client_argv: List[str]
 
     def __init__(self: RemoteCluster,
                  source: Iterable[str] = None,
                  num_tasks: int = 1,
                  template: str = DEFAULT_TEMPLATE,
                  bundlesize: int = DEFAULT_BUNDLESIZE,
                  bundlewait: int = DEFAULT_BUNDLEWAIT,
@@ -75,42 +77,50 @@
                  max_retries: int = DEFAULT_ATTEMPTS,
                  eager: bool = False,
                  redirect_failures: IO = None,
                  in_memory: bool = False,
                  no_confirm: bool = False,
                  capture: bool = False,
                  client_timeout: int = None,
-                 task_timeout: int = None) -> None:
+                 task_timeout: int = None,
+                 task_signalwait: int = DEFAULT_SIGNALWAIT) -> None:
         """Initialize server and client threads with external launcher."""
         auth = secrets.token_hex(64)
         self.server = ServerThread(source=source, auth=auth, bundlesize=bundlesize, bundlewait=bundlewait,
                                    in_memory=in_memory, no_confirm=no_confirm, max_retries=max_retries, eager=eager,
                                    address=bind, forever_mode=forever_mode, restart_mode=restart_mode,
                                    redirect_failures=redirect_failures)
-        launcher_args = '' if launcher_args is None else ' '.join(launcher_args)
-        client_args = ''
+        launcher = shlex.split(launcher)
+        if launcher_args is None:
+            launcher_args = []
+        else:
+            launcher_args = [arg for arg_group in launcher_args for arg in shlex.split(arg_group)]
+        client_args = []
         if capture is True:
-            client_args += ' --capture'
+            client_args.append('--capture')
         if no_confirm is True:
-            client_args += ' --no-confirm'
+            client_args.append('--no-confirm')
         if client_timeout is not None:
-            client_args += f' -T {client_timeout}'
+            client_args.extend(['-T', str(client_timeout)])
         if task_timeout is not None:
-            client_args += f' -W {task_timeout}'
-        self.client_argv = (f'{launcher} {launcher_args} {remote_exe} client -H {HOSTNAME} -p {bind[1]} '
-                            f'-N {num_tasks} -b {bundlesize} -w {bundlewait} -t "{template}" -k {auth} '
-                            f'-d {delay_start} {client_args}')
+            client_args.extend(['-W', str(task_timeout)])
+        self.client_argv = [
+            *launcher, *launcher_args, remote_exe, 'client',
+            '-H', HOSTNAME, '-p', str(bind[1]), '-N', str(num_tasks), '-b', str(bundlesize), '-w', str(bundlewait),
+            '-t', template, '-k', auth, '-d', str(delay_start), '-S', str(task_signalwait), *client_args
+        ]
         super().__init__(name='hypershell-cluster')
 
     def run_with_exceptions(self: RemoteCluster) -> None:
         """Start child threads, wait."""
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         log.debug(f'Launching clients: {self.client_argv}')
-        self.clients = Popen(self.client_argv, shell=True, stdout=sys.stdout, stderr=sys.stderr,
+        self.clients = Popen(self.client_argv,
+                             stdout=sys.stdout, stderr=sys.stderr,
                              env={**os.environ, **load_task_env()})
         self.clients.wait()
         self.server.join()
 
     def stop(self: RemoteCluster, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         self.server.stop(wait=wait, timeout=timeout)
@@ -168,32 +178,32 @@
 
     policy: AutoScalerPolicy
     factor: float
     period: int
     init_size: int
     min_size: int
     max_size: int
-    launcher: str
+    launcher: List[str]
 
     clients: List[Popen]
     last_check: datetime
     wait_check: timedelta
 
     phase: AutoScalerPhase = AutoScalerPhase.INIT
     state: AutoScalerState = AutoScalerState.START
     states: Type[State] = AutoScalerState
 
     def __init__(self: AutoScaler,
+                 launcher: List[str],
                  policy: str = DEFAULT_AUTOSCALE_POLICY,
                  factor: float = DEFAULT_AUTOSCALE_FACTOR,
                  period: int = DEFAULT_AUTOSCALE_PERIOD,
                  init_size: int = DEFAULT_AUTOSCALE_INIT_SIZE,
                  min_size: int = DEFAULT_AUTOSCALE_MIN_SIZE,
                  max_size: int = DEFAULT_AUTOSCALE_MAX_SIZE,
-                 launcher: str = DEFAULT_AUTOSCALE_LAUNCHER,
                  ) -> None:
         """Initialize with scaling parameters."""
         self.policy = AutoScalerPolicy.from_name(policy)
         self.factor = factor
         self.period = period
         self.init_size = init_size
         self.min_size = min_size
@@ -302,15 +312,15 @@
                 return AutoScalerState.SCALE
             else:
                 log.debug('Autoscale pause (waiting on clients to complete initial tasks)')
                 return AutoScalerState.WAIT
 
     def scale(self: AutoScaler) -> AutoScalerState:
         """Launch new client."""
-        proc = Popen(self.launcher, shell=True, stdout=sys.stdout, stderr=sys.stderr,
+        proc = Popen(self.launcher, stdout=sys.stdout, stderr=sys.stderr,
                      bufsize=0, universal_newlines=True, env={**os.environ, **load_task_env()})
         log.trace(f'Autoscale adding client ({proc.pid})')
         self.clients.append(proc)
         if self.phase is AutoScalerPhase.INIT:
             return AutoScalerState.INIT
         else:
             return AutoScalerState.WAIT
@@ -336,27 +346,26 @@
         return AutoScalerState.HALT
 
 
 class AutoScalerThread(Thread):
     """Run AutoScaler within dedicated thread."""
 
     def __init__(self: AutoScalerThread,
+                 launcher: List[str],
                  policy: str = DEFAULT_AUTOSCALE_POLICY,
                  factor: float = DEFAULT_AUTOSCALE_FACTOR,
                  period: int = DEFAULT_AUTOSCALE_PERIOD,
                  init_size: int = DEFAULT_AUTOSCALE_INIT_SIZE,
                  min_size: int = DEFAULT_AUTOSCALE_MIN_SIZE,
                  max_size: int = DEFAULT_AUTOSCALE_MAX_SIZE,
-                 launcher: str = DEFAULT_AUTOSCALE_LAUNCHER,
                  ) -> None:
         """Initialize task executor."""
         super().__init__(name=f'hypershell-autoscaler')
-        self.machine = AutoScaler(policy=policy, factor=factor, period=period,
-                                  init_size=init_size, min_size=min_size, max_size=max_size,
-                                  launcher=launcher)
+        self.machine = AutoScaler(launcher, policy=policy, factor=factor, period=period,
+                                  init_size=init_size, min_size=min_size, max_size=max_size)
 
     def run_with_exceptions(self: AutoScalerThread) -> None:
         """Run machine."""
         self.machine.run()
 
     def stop(self: AutoScalerThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
@@ -394,33 +403,41 @@
                  min_size: int = DEFAULT_AUTOSCALE_MIN_SIZE,
                  max_size: int = DEFAULT_AUTOSCALE_MAX_SIZE,
                  forever_mode: bool = False,  # noqa: ignored (passed by ClusterApp)
                  restart_mode: bool = False,  # noqa: ignored (passed by ClusterApp)
                  in_memory: bool = False,  # noqa: ignored (passed by ClusterApp)
                  no_confirm: bool = False,  # noqa: ignored (passed by ClusterApp)
                  client_timeout: int = None,
-                 task_timeout: int = None
+                 task_timeout: int = None,
+                 task_signalwait: int = DEFAULT_SIGNALWAIT,
                  ) -> None:
         """Initialize server and autoscaler."""
         auth = secrets.token_hex(64)
         self.server = ServerThread(source=source, auth=auth, bundlesize=bundlesize, bundlewait=bundlewait,
                                    max_retries=max_retries, eager=eager, address=bind, forever_mode=True,
                                    redirect_failures=redirect_failures)
-        launcher_args = '' if launcher_args is None else ' '.join(launcher_args)
-        client_args = '' if not capture else '--capture'
+        launcher = shlex.split(launcher)
+        if launcher_args is None:
+            launcher_args = []
+        else:
+            launcher_args = [arg for arg_group in launcher_args for arg in shlex.split(arg_group)]
+        client_args = []
+        if capture:
+            client_args.append('--capture')
         if client_timeout is not None:
-            client_args += f' -T {client_timeout}'
+            client_args.extend(['-T', str(client_timeout)])
         if task_timeout is not None:
-            client_args += f' -W {task_timeout}'
-        launcher = (f'{launcher} {launcher_args} {remote_exe} client -H {HOSTNAME} -p {bind[1]} '
-                    f'-N {num_tasks} -b {bundlesize} -w {bundlewait} -t "{template}" -k {auth} '
-                    f'-d {delay_start} {client_args}')
-        self.autoscaler = AutoScalerThread(policy=policy, factor=factor, period=period,
-                                           init_size=init_size, min_size=min_size, max_size=max_size,
-                                           launcher=launcher)
+            client_args.extend(['-W', str(task_timeout)])
+        launcher.extend([
+            *launcher_args, remote_exe, 'client',
+            '-H', HOSTNAME, '-p', str(bind[1]), '-N', str(num_tasks), '-b', str(bundlesize), '-w', str(bundlewait),
+            '-t', template, '-k', auth, '-d', str(delay_start), '-S', str(task_signalwait), *client_args
+        ])
+        self.autoscaler = AutoScalerThread(launcher, policy=policy, factor=factor, period=period,
+                                           init_size=init_size, min_size=min_size, max_size=max_size)
         super().__init__(name='hypershell-cluster')
 
     def run_with_exceptions(self: AutoScalingCluster) -> None:
         """Start child threads, wait."""
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         self.autoscaler.start()
```

### Comparing `hyper-shell-2.4.0/src/hypershell/cluster/ssh.py` & `hyper_shell-2.5.0/src/hypershell/cluster/ssh.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """SSH-based cluster implementation."""
 
 
 # type annotations
 from __future__ import annotations
 from typing import Type, List, Iterable, Tuple, IO
 
 # standard libs
 import re
 import sys
 import time
+import shlex
 import secrets
 from subprocess import Popen
 
 # external libs
 from cmdkit.config import ConfigurationError, Namespace
 
 # internal libs
 from hypershell.core.config import config, blame
 from hypershell.core.thread import Thread
 from hypershell.core.logging import Logger, HOSTNAME
 from hypershell.core.queue import QueueConfig
 from hypershell.core.template import DEFAULT_TEMPLATE
-from hypershell.client import DEFAULT_DELAY
+from hypershell.client import DEFAULT_DELAY, DEFAULT_SIGNALWAIT
 from hypershell.submit import DEFAULT_BUNDLEWAIT
 from hypershell.server import ServerThread, DEFAULT_BUNDLESIZE, DEFAULT_ATTEMPTS
 
 # public interface
 __all__ = ['run_ssh', 'SSHCluster', 'NodeList']
 
 # initialize logger
@@ -46,15 +47,15 @@
 
 
 class SSHCluster(Thread):
     """Run server with individual external ssh clients."""
 
     server: ServerThread
     clients: List[Popen]
-    client_argv: List[str]
+    client_argv: List[List[str]]
 
     def __init__(self: SSHCluster,
                  source: Iterable[str] = None,
                  num_tasks: int = 1,
                  template: str = DEFAULT_TEMPLATE,
                  forever_mode: bool = False,
                  restart_mode: bool = False,
@@ -70,52 +71,55 @@
                  in_memory: bool = False,
                  no_confirm: bool = False,
                  redirect_failures: IO = None,
                  export_env: bool = False,
                  delay_start: float = DEFAULT_DELAY,
                  capture: bool = False,
                  client_timeout: int = None,
-                 task_timeout: int = None) -> None:
+                 task_timeout: int = None,
+                 task_signalwait: int = DEFAULT_SIGNALWAIT) -> None:
         """Initialize server and client threads."""
         if nodelist is None:
             raise AttributeError('Expected nodelist')
         auth = secrets.token_hex(64)
         self.server = ServerThread(source=source, auth=auth, bundlesize=bundlesize, bundlewait=bundlewait,
                                    max_retries=max_retries, eager=eager, address=bind,
                                    forever_mode=forever_mode, restart_mode=restart_mode,
                                    in_memory=in_memory, no_confirm=no_confirm,
                                    redirect_failures=redirect_failures)
-        launcher_env = '' if not export_env else compile_env()
+        launcher = shlex.split(launcher)
+        launcher_env = shlex.split('' if not export_env else compile_env())
         if launcher_args is None:
-            launcher_args = config.ssh.get('args', '')
-        else:
-            launcher_args = config.ssh.get('args', '') + ' ' + ' '.join(launcher_args)
-        client_args = ''
-        if capture is True:
-            client_args += ' --capture'
+            launcher_args = shlex.split(config.ssh.get('args', ''))
+        client_args = []
+        if capture:
+            client_args.append('--capture')
         if no_confirm:
-            client_args += ' --no-confirm'
+            client_args.append('--no-confirm')
         if client_timeout is not None:
-            client_args += f' -T {client_timeout}'
+            client_args.extend(['-T', str(client_timeout)])
         if task_timeout is not None:
-            client_args += f' -W {task_timeout}'
-        self.client_argv = [f'{launcher} {launcher_args} {host} {launcher_env} {remote_exe} '
-                            f'client -H {HOSTNAME} -p {bind[1]} -N {num_tasks} -b {bundlesize} -w {bundlewait} '
-                            f'-t \'"{template}"\' -k {auth} -d {delay_start} {client_args}'
-                            for host in nodelist]
+            client_args.extend(['-W', str(task_timeout)])
+        self.client_argv = [
+            [*launcher, *launcher_args, host, *launcher_env, remote_exe, 'client', '-H', HOSTNAME,
+             '-p', str(bind[1]), '-N', str(num_tasks), '-b', str(bundlesize), '-w', str(bundlewait),
+             '-t', f'\'{template}\'', '-k', auth, '-d', str(delay_start),
+             '-S', str(task_signalwait), *client_args]
+            for host in nodelist
+        ]
         super().__init__(name='hypershell-cluster')
 
     def run_with_exceptions(self: SSHCluster) -> None:
         """Start child threads, wait."""
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         self.clients = []
         for argv in self.client_argv:
             log.debug(f'Launching client: {argv}')
-            self.clients.append(Popen(argv, shell=True, stdout=sys.stdout, stderr=sys.stderr))
+            self.clients.append(Popen(argv, stdout=sys.stdout, stderr=sys.stderr))
         for client in self.clients:
             client.wait()
         self.server.join()
 
     def stop(self: SSHCluster, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         self.server.stop(wait=wait, timeout=timeout)
@@ -146,29 +150,36 @@
 
         if 'ssh' not in config:
             raise ConfigurationError('No `ssh` section found in configuration')
         if 'nodelist' not in config.ssh:
             raise ConfigurationError('No `ssh.nodelist` section found in configuration')
 
         label = blame(config, 'ssh', 'nodelist')
+        nodelist = config.ssh.nodelist
+
         if groupname is None:
-            if isinstance(config.ssh.nodelist, list):
-                return cls(config.ssh.nodelist)
-            elif isinstance(config.ssh.nodelist, dict):
+            if isinstance(nodelist, str):
+                return cls.from_pattern(nodelist)
+            elif isinstance(nodelist, list):
+                return cls(nodelist)
+            elif isinstance(nodelist, dict):
                 raise ConfigurationError(f'SSH group unspecified but multiple groups in `ssh.nodelist` ({label})')
             else:
                 raise ConfigurationError(f'Expected list for `ssh.nodelist` ({label})')
 
-        if isinstance(config.ssh.nodelist, dict):
-            if groupname not in config.ssh.nodelist:
+        if isinstance(nodelist, dict):
+            nodelist = nodelist.get(groupname, None)
+            if not nodelist:
                 raise ConfigurationError(f'No list \'{groupname}\' found in `ssh.nodelist` section ({label})')
-            elif not isinstance(config.ssh.nodelist.get(groupname), list):
-                raise ConfigurationError(f'Expected list for `ssh.nodelist.{groupname}` ({label})')
+            elif isinstance(nodelist, str):
+                return cls.from_pattern(nodelist)
+            elif isinstance(nodelist, list):
+                return cls(nodelist)
             else:
-                return cls(config.ssh.nodelist.get(groupname))
+                raise ConfigurationError(f'Expected list for `ssh.nodelist.{groupname}` ({label})')
         else:
             raise ConfigurationError(f'Expected either list or section for `ssh.nodelist` ({label})')
 
     @classmethod
     def from_pattern(cls: Type[NodeList], pattern: str) -> NodeList:
         """Expand a `pattern` to multiple hostnames."""
         pattern = pattern.strip(',')
@@ -201,8 +212,7 @@
                 result.extend([group, ])
         return result
 
 
 def compile_env() -> str:
     """Build environment variable argument expansion for remote client launch command."""
     return ' '.join([f'{key}="{value}"' for key, value in Namespace.from_env('HYPERSHELL').items()])
-
```

### Comparing `hyper-shell-2.4.0/src/hypershell/config.py` & `hyper_shell-2.5.0/src/hypershell/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,173 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Manage configuration."""
 
 
 # type annotations
 from __future__ import annotations
 from typing import Any
 
 # standard libs
 import os
+import io
 import sys
 import json
+import contextlib
 import subprocess
 
 # external libs
 import toml
+from pygments.styles import STYLE_MAP as CONSOLE_THEMES
 from cmdkit.app import Application, ApplicationGroup
 from cmdkit.cli import Interface, ArgumentError
 from cmdkit.config import ConfigurationError
 from rich.console import Console
 from rich.syntax import Syntax
 
 # internal libs
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.platform import path
 from hypershell.core.types import smart_coerce
-from hypershell.core.config import load_file, update, config as full_config
 from hypershell.core.logging import Logger
 from hypershell.core.exceptions import get_shared_exception_mapping
+from hypershell.core.config import (load_file, update, ACTIVE_CONFIG_VARS,
+                                    default as default_config, config as full_config)
 
 # public interface
 __all__ = ['ConfigApp', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
-EDIT_PROGRAM = 'hyper-shell config edit'
+EDIT_PROGRAM = 'hs config edit'
+EDIT_SYNOPSIS = f'{EDIT_PROGRAM} [-h] [--system | --user | --local]'
 EDIT_USAGE = f"""\
 Usage:
-{EDIT_PROGRAM} [-h] [--system | --user]
+  {EDIT_SYNOPSIS}
 
-Edit configuration with default editor.
-The EDITOR/VISUAL environment variable must be set.\
+  Edit configuration with default editor.
+  The EDITOR/VISUAL environment variable must be set.\
 """
 
 EDIT_HELP = f"""\
 {EDIT_USAGE}
 
 Options:
       --system         Edit system configuration.
-      --user           Edit user configuration (default).
+      --user           Edit user configuration. (default)
+      --local          Edit local configuration.
   -h, --help           Show this message and exit.\
 """
 
 
 class ConfigEditApp(Application):
     """Edit configuration with default editor."""
 
-    interface = Interface(EDIT_PROGRAM,
-                          colorize_usage(EDIT_USAGE),
-                          colorize_usage(EDIT_HELP))
+    interface = Interface(EDIT_PROGRAM, EDIT_USAGE, EDIT_HELP)
 
     site_name: str = 'user'
     site_interface = interface.add_mutually_exclusive_group()
-    site_interface.add_argument('--user', action='store_const', const='user')
-    site_interface.add_argument('--system', action='store_const', const='system')
+    site_interface.add_argument('--system', action='store_const', const='system', dest='site_name')
+    site_interface.add_argument('--user', action='store_const', const='user', dest='site_name')
+    site_interface.add_argument('--local', action='store_const', const='local', dest='site_name')
 
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: ConfigEditApp) -> None:
         """Business logic for `config edit`."""
 
-        config_path = path[self.site_name].config
         editor = os.getenv('EDITOR', os.getenv('VISUAL', None))
         if not editor:
             raise RuntimeError('EDITOR or VISUAL environment variable not defined')
 
+        config_path = path[self.site_name].config
+        os.makedirs(os.path.dirname(config_path), exist_ok=True)
+
         log.debug(f'Opening {config_path}')
         log.debug(f'Editor: {editor}')
         subprocess.run([editor, config_path])
 
 
-GET_PROGRAM = 'hyper-shell config get'
+GET_PROGRAM = 'hs config get'
+GET_SYNOPSIS = f'{GET_PROGRAM} [-h] SECTION[...].VAR [-x] [-r] [--system | --user | --local | --default]'
 GET_USAGE = f"""\
 Usage:
-{GET_PROGRAM} [-h] [-x] SECTION[...].VAR [--system | --user]
-
-Get configuration option.\
+  {GET_SYNOPSIS}
+  Get configuration option.\
 """
 
 GET_HELP = f"""\
 {GET_USAGE}
 
-If --user/--system not specified, the output is the merged configuration
-from all sources. Use `hyper-shell config which` to see where a specific
-option originates from.
+  If source is not specified, the output is the merged configuration
+  from all sources. Use `hs config which` to see where a specific
+  option originates from.
+  
+  If a single value is requested, use -r/--raw to strip formatting. 
 
 Arguments:
   SECTION[...].VAR          Path to variable (default: '.').
 
 Options:
       --system              Load from system configuration.
       --user                Load from user configuration.
+      --local               Load from local configuration.
+      --default             Load from default configuration.
   -x, --expand              Expand variable.
+  -r, --raw                 Disable formatting on single value output.
   -h, --help                Show this message and exit.\
 """
 
 
 class ConfigGetApp(Application):
     """Get configuration option."""
 
-    interface = Interface(GET_PROGRAM,
-                          colorize_usage(GET_USAGE),
-                          colorize_usage(GET_HELP))
+    interface = Interface(GET_PROGRAM, GET_USAGE, GET_HELP)
 
     varpath: str = None
     interface.add_argument('varpath', nargs='?', default='.')
 
     site_name: str = None
     site_interface = interface.add_mutually_exclusive_group()
-    site_interface.add_argument('--user', action='store_const', const='user', dest='site_name')
     site_interface.add_argument('--system', action='store_const', const='system', dest='site_name')
+    site_interface.add_argument('--user', action='store_const', const='user', dest='site_name')
+    site_interface.add_argument('--local', action='store_const', const='local', dest='site_name')
+    site_interface.add_argument('--default', action='store_const', const='default', dest='site_name')
 
     expand: bool = False
     interface.add_argument('-x', '--expand', action='store_true')
 
+    raw_mode: bool = False
+    interface.add_argument('-r', '--raw', action='store_true', dest='raw_mode')
+
+    # Hidden options used as helpers for completion script
+    list_available: bool = False
+    list_console_themes: bool = False
+    completion_interface = interface.add_mutually_exclusive_group()
+    completion_interface.add_argument('--list-available', action='version', version=' '.join(ACTIVE_CONFIG_VARS))
+    completion_interface.add_argument('--list-console-themes', action='version',
+                                      version=' '.join(list(CONSOLE_THEMES)))
+
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: ConfigGetApp) -> None:
         """Business logic for `config get`."""
 
         if self.site_name is None:
             config_path = 'configuration'  # Note: not meaningful for merged configuration
             config = full_config
+        elif self.site_name == 'default':
+            config_path = 'default'
+            config = default_config
         else:
             config_path = path[self.site_name].config
             if os.path.exists(config_path):
                 config = load_file(config_path)
             else:
                 raise ConfigurationError(f'{config_path} does not exist')
 
@@ -190,15 +215,15 @@
             self.print_output(config_section[variable])
         else:
             raise ConfigurationError(f'"{self.varpath}" not found in {config_path}')
 
     def print_output(self: ConfigGetApp, value: Any) -> None:
         """Format and print final `value`."""
         value = self.format_output(value)
-        if sys.stdout.isatty():
+        if sys.stdout.isatty() and not self.raw_mode:
             output = Syntax(value, 'toml', word_wrap=True,
                             theme = full_config.console.theme,
                             background_color = 'default')
             Console().print(output)
         else:
             # NOTE: JSON formatting puts quotations - we don't want these on raw output
             print(value.strip('"'), file=sys.stdout, flush=True)
@@ -225,53 +250,53 @@
                 lines.append(line)
             else:
                 lines.append(line.replace('"', ''))
         value = '\n'.join(lines)
         return value
 
 
-SET_PROGRAM = 'hyper-shell config set'
+SET_PROGRAM = 'hs config set'
+SET_SYNOPSIS = f'{SET_PROGRAM} [-h] SECTION[...].VAR VALUE [--system | --user | --local]'
 SET_USAGE = f"""\
 Usage: 
-{SET_PROGRAM} [-h] SECTION[...].VAR VALUE [--system | --user]
-
-Set configuration option.\
+  {SET_SYNOPSIS}
+  Set configuration option.\
 """
 
 SET_HELP = f"""\
 {SET_USAGE}
 
 Arguments:
   SECTION[...].VAR        Path to variable.
   VALUE                   Value to be set.
 
 Options:
       --system            Apply to system configuration.
-      --user              Apply to user configuration (default).
+      --user              Apply to user configuration. (default)
+      --local             Apply to local configuration.
   -h, --help              Show this message and exit.\
 """
 
 
 class ConfigSetApp(Application):
     """Set configuration option."""
 
-    interface = Interface(SET_PROGRAM,
-                          colorize_usage(SET_USAGE),
-                          colorize_usage(SET_HELP))
+    interface = Interface(SET_PROGRAM, SET_USAGE, SET_HELP)
 
     varpath: str = None
     interface.add_argument('varpath', metavar='VAR')
 
     value: str = None
     interface.add_argument('value', type=smart_coerce)
 
     site_name: str = 'user'
     site_interface = interface.add_mutually_exclusive_group()
     site_interface.add_argument('--user', action='store_const', const='user', dest='site_name', default=site_name)
     site_interface.add_argument('--system', action='store_const', const='system', dest='site_name')
+    site_interface.add_argument('--local', action='store_const', const='local', dest='site_name')
 
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: ConfigSetApp) -> None:
         """Business logic for `config set`."""
@@ -288,100 +313,139 @@
                 config_section[subsection] = dict()
             config_section = config_section[subsection]
 
         config_section[variable] = self.value
         update(self.site_name, config)
 
 
-WHICH_PROGRAM = 'hyper-shell config which'
+WHICH_PROGRAM = 'hs config which'
+WHICH_SYNOPSIS = f'{WHICH_PROGRAM} [-h] SECTION[...].VAR [--site]'
 WHICH_USAGE = f"""\
 Usage: 
-{WHICH_PROGRAM} [-h] SECTION[...].VAR
-
-Show origin of configuration option.\
+  {WHICH_SYNOPSIS}
+  Show origin of configuration option.\
 """
 
 WHICH_HELP = f"""\
 {WHICH_USAGE}
 
 Arguments:
   SECTION[...].VAR        Path to variable.
 
 Options:
+      --site              Output originating site name only.
   -h, --help              Show this message and exit.\
 """
 
 
 class ConfigWhichApp(Application):
     """Show origin of configuration option."""
 
-    interface = Interface(WHICH_PROGRAM,
-                          colorize_usage(WHICH_USAGE),
-                          colorize_usage(WHICH_HELP))
+    interface = Interface(WHICH_PROGRAM, WHICH_USAGE, WHICH_HELP)
 
     varpath: str = None
     interface.add_argument('varpath', metavar='VAR')
 
+    site_only: bool = False
+    interface.add_argument('--site', action='store_true', dest='site_only')
+
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: ConfigWhichApp) -> None:
         """Business logic for `config which`."""
         try:
             site = full_config.which(*self.varpath.split('.'))
         except KeyError:
             log.critical(f'"{self.varpath}" not found')
             return
-        if site in ('default', 'env', 'logging', ):
+        if self.site_only:
             print(site)
+            return
+        try:
+            with contextlib.redirect_stdout(io.StringIO()) as stdout:
+                with ConfigGetApp.from_cmdline([self.varpath, '--raw']) as app:
+                    app.run()
+        except ConfigurationError:
+            value = 'null'
+        else:
+            value = stdout.getvalue().strip()
+        try:
+            with contextlib.redirect_stdout(io.StringIO()) as stdout:
+                with ConfigGetApp.from_cmdline([self.varpath, '--raw', '--default']) as app:
+                    app.run()
+        except ConfigurationError:
+            default_value = 'null'
         else:
-            print(f'{site}: {path[site].config}')
+            default_value = stdout.getvalue().strip()
+        if '[' in value:
+            value = '[...]'
+        if '[' in default_value:
+            default_value = '[...]'
+        if site in ('default', 'logging', ):
+            print(f'{value} ({site})')
+        elif site == 'env':
+            env_varname = 'HYPERSHELL_' + self.varpath.upper().replace('.', '_')
+            if value == '[...]':
+                for name in full_config.namespaces.env.to_env().flatten(prefix='HYPERSHELL'):
+                    if name.startswith(env_varname):
+                        env_varname = name
+            print(f'{value} (env: {env_varname} | default: {default_value})')
+        else:
+            print(f'{value} ({site}: {path[site].config} | default: {default_value})')
 
 
 if os.name == 'nt':
-    SYSTEM_CONFIG_PATH = '%ProgramData%\\HyperShell\\Config.toml'
-    USER_CONFIG_PATH = '%AppData%\\HyperShell\\Config.toml'
+    CONFIG_PATH_INFO = f"""\
+  --system         %ProgramData%\\HyperShell\\Config.toml
+  --user           %AppData%\\HyperShell\\Config.toml
+  --local          {path.local.config}
+"""
 else:
-    SYSTEM_CONFIG_PATH = '/etc/hypershell.toml'
-    USER_CONFIG_PATH = '~/.hypershell/config.toml'
+    CONFIG_PATH_INFO = f"""\
+  --system         /etc/hypershell.toml
+  --user           ~/.hypershell/config.toml
+  --local          {path.local.config}
+"""
 
 
-PROGRAM = 'hyper-shell config'
+PROGRAM = 'hs config'
 USAGE = f"""\
-Usage: 
-{PROGRAM} [-h] <command> [<args>...]
+Usage:
+  {PROGRAM} [-h]
+  {GET_SYNOPSIS}
+  {SET_SYNOPSIS}
+  {EDIT_SYNOPSIS}
+  {WHICH_SYNOPSIS}
 
-{__doc__}\
+  {__doc__}\
 """
 
 HELP = f"""\
 {USAGE}
 
 Commands:
-  get                   {ConfigGetApp.__doc__}
-  set                   {ConfigSetApp.__doc__}
-  edit                  {ConfigEditApp.__doc__}
-  which                 {ConfigWhichApp.__doc__}
+  get              {ConfigGetApp.__doc__}
+  set              {ConfigSetApp.__doc__}
+  edit             {ConfigEditApp.__doc__}
+  which            {ConfigWhichApp.__doc__}
 
 Options:
-  -h, --help            Show this message and exit.
+  -h, --help       Show this message and exit.
 
 Files:
-  (system)  {SYSTEM_CONFIG_PATH}
-    (user)  {USER_CONFIG_PATH}
+{CONFIG_PATH_INFO}\
 """
 
 
 class ConfigApp(ApplicationGroup):
     """Manage configuration."""
 
-    interface = Interface(PROGRAM,
-                          colorize_usage(USAGE),
-                          colorize_usage(HELP))
+    interface = Interface(PROGRAM, USAGE, HELP)
 
     interface.add_argument('command')
 
     command = None
     commands = {'get': ConfigGetApp,
                 'set': ConfigSetApp,
                 'edit': ConfigEditApp,
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/config.py` & `hyper_shell-2.5.0/src/hypershell/core/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Runtime configuration for HyperShell."""
 
 
 # type annotations
 from __future__ import annotations
-from typing import TypeVar, Union, List, Optional, Protocol
+from typing import TypeVar, Union, List, Optional, Protocol, Final, Iterator
 
 # standard libs
 import os
+import re
 import sys
 import shutil
 import tomlkit
 import logging
+import socket
 import functools
 from datetime import datetime
 
 # external libs
 from cmdkit.config import Namespace, Configuration, Environ, ConfigurationError
 from cmdkit.app import exit_status
 
 # internal libs
 from hypershell.core.platform import path, home
 from hypershell.core.exceptions import write_traceback
 
 # public interface
 __all__ = ['config', 'update', 'default', 'ConfigurationError', 'Namespace', 'blame',
-           'load', 'reload', 'load_file', 'reload_file', 'load_env', 'reload_env', 'load_task_env',
-           'DEFAULT_LOGGING_STYLE', 'LOGGING_STYLES', ]
+           'load', 'reload', 'reload_local', 'load_file', 'reload_file', 'load_env', 'reload_env', 'load_task_env',
+           'DEFAULT_LOGGING_STYLE', 'LOGGING_STYLES', 'ACTIVE_CONFIG_VARS', 'SSH_GROUPS',
+           'find_available_ports']
 
 # partial logging (not yet configured - initialized afterward)
 log = logging.getLogger(__name__)
 
 
 DEFAULT_LOGGING_STYLE = 'default'
 LOGGING_STYLES = {
@@ -55,70 +58,81 @@
     }
 }
 
 
 # environment variables and configuration files are automatically
 # depth-first merged with defaults
 default = Namespace({
+
     'database': {
         'provider': 'sqlite',
     },
+
     'logging': {
         'color': True,
         'level': 'warning',
         'datefmt': '%Y-%m-%d %H:%M:%S',
         'style': DEFAULT_LOGGING_STYLE,
         **LOGGING_STYLES.get(DEFAULT_LOGGING_STYLE),
     },
+
     'task': {
         'cwd': os.getcwd(),
-        'timeout': None,  # Seconds, period to wait before killing tasks
+        'timeout': None,    # seconds, period to wait before killing tasks
+        'signalwait': 10,   # seconds to wait between signal escalation (INT, TERM, KILL)
     },
+
     'submit': {
-        'bundlesize': 1,
-        'bundlewait': 5  # seconds
+        'bundlesize': 1,    # size of task bundle to accumulate before committing
+        'bundlewait': 5     # seconds to wait before committing regardless of size
     },
+
     'server': {
         'bind': 'localhost',
         'port': 50_001,
         'auth': '__HYPERSHELL__BAD__AUTHKEY__',
-        'queuesize': 1,  # only allow a single bundle (scheduler must wait)
+        'queuesize': 1,     # only allow a single bundle (scheduler must wait)
         'bundlesize': 1,
-        'bundlewait': 5,   # seconds
+        'bundlewait': 5,    # seconds
         'attempts': 1,
-        'eager': False,  # prefer failed tasks to new tasks
-        'wait': 5,  # seconds to wait between database queries
-        'evict': 600,  # assume client is gone if no heartbeat after this many seconds
+        'eager': False,     # prefer failed tasks to new tasks
+        'wait': 5,          # seconds to wait between database queries
+        'evict': 600,       # assume client is gone if no heartbeat after this many seconds
     },
+
     'client': {
-        'bundlesize': 1,
-        'bundlewait': 5,  # Seconds
-        'heartrate': 10,  # Seconds, period to wait between heartbeats
-        'timeout': None,  # seconds, period to wait on tasks before shutting down
+        'bundlesize': 1,    # size of task bundle to accumulate before returning
+        'bundlewait': 5,    # seconds to wait before returning regardless of size
+        'heartrate': 10,    # seconds to wait between heartbeats
+        'timeout': None,    # seconds to wait for bundle from server before shutting down
     },
+
     'ssh': {
         'config': os.path.join(home, '.ssh', 'config'),
+        'nodelist': {}  # Populated by user configuration
     },
+
     'autoscale': {
         'policy': 'fixed',  # Either 'fixed' or 'dynamic'
         'factor': 1,
         'period': 60,  # seconds to wait between checks
-        'launcher': '',  # empty means just 'hyper-shell client'
+        'launcher': '',  # empty means just 'hs client'
         'size': {
             'init': 1,
             'min': 0,
             'max': 2,
         },
     },
+
     'console': {
         'theme': 'monokai',
     },
-    'export': {
-        # NOTE: defining HYPERSHELL_EXPORT_XXX defines XXX within task env
-    }
+
+    # NOTE: defining HYPERSHELL_EXPORT_XXX defines XXX within task env
+    'export': {}
 })
 
 
 def reload_file(filepath: str) -> Namespace:
     """Force reloading configuration file."""
     if not os.path.exists(filepath):
         return Namespace({})
@@ -141,32 +155,38 @@
 
 @functools.lru_cache(maxsize=None)
 def load_env() -> Environ:
     """Load environment variables and expand hierarchy as namespace."""
     return reload_env()
 
 
-def partial_load(**preload: Namespace) -> Configuration:
+def partial_load(system: Optional[str] = path.system.config,
+                 user: Optional[str] = path.user.config,
+                 local: Optional[str] = path.local.config,
+                 **preload: Namespace) -> Configuration:
     """Load configuration from files and merge environment variables."""
     return Configuration(**{
         'default': default, **preload,
-        'system': load_file(path.system.config),
-        'user': load_file(path.user.config),
-        'local': load_file(path.local.config),
+        'system': {} if not system else load_file(system),
+        'user': {} if not user else load_file(user),
+        'local': {} if not user else load_file(local),
         'env': load_env(),
     })
 
 
-def partial_reload(**preload: Namespace) -> Configuration:
+def partial_reload(system: Optional[str] = path.system.config,
+                   user: Optional[str] = path.user.config,
+                   local: Optional[str] = path.local.config,
+                   **preload: Namespace) -> Configuration:
     """Force reload configuration from files and merge environment variables."""
     return Configuration(**{
         'default': default, **preload,
-        'system': reload_file(path.system.config),
-        'user': reload_file(path.user.config),
-        'local': reload_file(path.local.config),
+        'system': {} if not system else reload_file(system),
+        'user': {} if not user else reload_file(user),
+        'local': {} if not local else reload_file(local),
         'env': reload_env(),
     })
 
 
 def blame(base: Configuration, *varpath: str) -> Optional[str]:
     """Construct filename or variable assignment string based on precedent of `varpath`."""
     source = base.which(*varpath)
@@ -196,15 +216,19 @@
 def build_preloads(base: Configuration) -> Namespace:
     """Build 'preload' namespace from base configuration."""
     return Namespace({'logging': LOGGING_STYLES.get(get_logging_style(base))})
 
 
 class LoaderImpl(Protocol):
     """Loader interface for building configuration."""
-    def __call__(self: LoaderImpl, **preloads: Namespace) -> Configuration: ...
+    def __call__(self: LoaderImpl,
+                 system: Optional[str] = path.system.config,
+                 user: Optional[str] = path.user.config,
+                 local: Optional[str] = path.local.config,
+                 **preload: Namespace) -> Configuration: ...
 
 
 def build_configuration(loader: LoaderImpl) -> Configuration:
     """Construct full configuration."""
     return loader(preload=build_preloads(base=loader()))
 
 
@@ -214,21 +238,60 @@
 
 
 def reload() -> Configuration:
     """Load configuration from files and merge environment variables."""
     return build_configuration(loader=partial_reload)
 
 
+def reload_local(filepath: Optional[str] = None) -> Configuration:
+    """Load configuration but only include one file."""
+    loader = functools.partial(partial_reload, system=None, user=None, local=filepath)
+    return build_configuration(loader=loader)
+
+
 try:
-    config = load()
+    if (local_config := os.getenv('HYPERSHELL_CONFIG_FILE', None)) is not None:
+        path.local.config = local_config  # Modified as to not lie to the user
+        config = reload_local(local_config)
+    else:
+        config = load()
 except Exception as error:
     write_traceback(error, module=__name__)
     sys.exit(exit_status.bad_config)
 
 
+ACTIVE_CONFIG_VARS: Final[List[str]] = [
+    re.sub(r'_(?!(env|eval))', r'.', name.lower())
+    for name in Namespace(config).to_env().flatten()
+]
+
+
+SSH_GROUPS = []
+try:
+    if isinstance(config.ssh.nodelist, dict):
+        SSH_GROUPS = list(config.ssh.nodelist)
+except KeyError:
+    pass
+
+
+def find_available_ports(start: int = default.server.port,
+                         end: int = default.server.port + 1_000) -> Iterator[int]:
+    """Yield available ports by testing each in turn."""
+    for port in range(start, end + 1):
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+            sock.settimeout(1)
+            try:
+                sock.bind(("0.0.0.0", port))
+                yield port
+            except socket.error:
+                pass
+    else:
+        raise RuntimeError(f'Could not find available port in range {start}-{end}')
+
+
 DEFAULT_CONFIG_HEADERS = f"""\
 # File automatically created on {datetime.now()}
 # Settings here are merged automatically with defaults and environment variables
 """
 
 
 def update(scope: str, partial: dict) -> None:
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/exceptions.py` & `hyper_shell-2.5.0/src/hypershell/core/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Core exception handling useful for import-time issues."""
 
 
 # type annotations
 from __future__ import annotations
@@ -16,17 +16,17 @@
 import traceback
 from datetime import datetime
 
 # external libs
 from cmdkit.app import exit_status
 from cmdkit.config import Namespace
 from cmdkit.config import ConfigurationError
+from cmdkit.ansi import faint, bold, magenta, yellow, red, COLOR_STDERR
 
 # internal libs
-from hypershell.core.ansi import faint, bold, magenta, yellow, red, COLOR_STDERR
 from hypershell.core.platform import default_path
 
 # public interface
 __all__ = ['display_warning', 'display_error', 'display_critical', 'traceback_filepath', 'write_traceback',
            'handle_exception', 'handle_exception_silently', 'handle_disconnect', 'handle_address_unknown',
            'HostAddressInfo', 'DatabaseUninitialized',
            'get_shared_exception_mapping', ]
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/fsm.py` & `hyper_shell-2.5.0/src/hypershell/core/fsm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Instrumentation for building finite state machines."""
 
 
 # type annotations
 from __future__ import annotations
@@ -50,15 +50,15 @@
         except Exception as error:
             log.critical(f'Uncaught exception from {self.__class__}')
             write_traceback(error, logger=log, module=__name__)
             raise
         else:
             # NOTE: Development aids not typically engaged
             # time.sleep(random.uniform(0, 5))  # FUZZ
-            log.devel(f'{self.__class__.__name__}: {previous_state} -> {next_state}')
+            # log.devel(f'{self.__class__.__name__}: {previous_state} -> {next_state}')
             return next_state
 
     def run(self) -> None:
         """Run machine until state is set to `HALT`."""
         while self.state is not self.states.HALT:  # noqa: HALT defined in implemented State enums
             self.state = self.next()
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/heartbeat.py` & `hyper_shell-2.5.0/src/hypershell/core/heartbeat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Heartbeat data passed between client and server."""
 
 
 # type annotations
 from __future__ import annotations
@@ -64,8 +64,7 @@
     @classmethod
     def unpack(cls: Type[Heartbeat], data: bytes) -> Heartbeat:
         """Deserialize from raw `data`."""
         data = json.loads(data.decode('utf-8'))
         data['time'] = datetime.fromisoformat(data['time'])
         data['state'] = ClientState.from_value(data['state'])
         return cls(**data)
-
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/logging.py` & `hyper_shell-2.5.0/src/hypershell/core/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Logging configuration."""
 
 
 # type annotations
 from __future__ import annotations
@@ -15,17 +15,17 @@
 import logging
 import functools
 import datetime
 
 # external libs
 from cmdkit.app import exit_status
 from cmdkit.config import ConfigurationError
+from cmdkit.ansi import Ansi, COLOR_STDERR
 
 # internal libs
-from hypershell.core.ansi import Ansi, COLOR_STDERR
 from hypershell.core.config import config, blame
 from hypershell.core.exceptions import write_traceback
 
 # public interface
 __all__ = ['Logger', 'HOSTNAME', 'INSTANCE', 'handler', 'initialize_logging', ]
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/platform.py` & `hyper_shell-2.5.0/src/hypershell/core/platform.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Platform specific file paths and initialization."""
 
 
+# NOTE:
+# A lot of the work done in this core module is provided by CmdKit at this point.
+# For continuity and for fear of breaking other parts of the project we have decided
+# to leave this module in place for the time being.
+
+
 # standard libs
 import os
 import sys
 import ctypes
+import platform
 
 # external libs
 from cmdkit.config import Namespace
 from cmdkit.app import exit_status
-
-# internal libs
-from hypershell.core.ansi import bold, magenta
+from cmdkit.ansi import bold, magenta
 
 # public interface
 __all__ = ['cwd', 'home', 'site', 'path', 'default_path']
 
 
 cwd = os.getcwd()
 home = os.path.expanduser('~')
@@ -28,15 +33,15 @@
     local_site = os.getenv('HYPERSHELL_SITE')
     if not os.path.isdir(local_site):
         print(f'{bold(magenta("CRITICAL"))} [{__name__}] '
               f'Directory does not exist (HYPERSHELL_SITE={local_site})', file=sys.stderr)
         sys.exit(exit_status.bad_config)
 
 
-if os.name == 'nt':
+if platform.system() == 'Windows':
     is_admin = ctypes.windll.shell32.IsUserAnAdmin() == 1
     site = Namespace(system=os.path.join(os.getenv('ProgramData'), 'HyperShell'),
                      user=os.path.join(os.getenv('AppData'), 'HyperShell'),
                      local=local_site)
     path = Namespace({
         'system': {
             'lib': os.path.join(site.system, 'Library'),
@@ -47,15 +52,34 @@
             'log': os.path.join(site.user, 'Logs'),
             'config': os.path.join(site.user, 'Config.toml')},
         'local': {
             'lib': os.path.join(site.local, 'Library'),
             'log': os.path.join(site.local, 'Logs'),
             'config': os.path.join(site.local, 'Config.toml')}
     })
-else:
+
+elif platform.system() == 'Darwin':
+    is_admin = os.getuid() == 0
+    site = Namespace(system='/', user=home, local=local_site)
+    path = Namespace({
+        'system': {
+            'lib': os.path.join(site['system'], 'Library', 'HyperShell'),
+            'log': os.path.join(site['system'], 'Library', 'Logs', 'HyperShell'),
+            'config': os.path.join(site['system'], 'Library', 'Preferences', 'HyperShell', 'config.toml')},
+        'user': {
+            'lib': os.path.join(site['user'], 'Library', 'HyperShell'),
+            'log': os.path.join(site['user'], 'Library', 'Logs', 'HyperShell'),
+            'config': os.path.join(site['user'], 'Library', 'Preferences', 'HyperShell', 'config.toml')},
+        'local': {
+            'lib': os.path.join(site['local'], 'Library'),
+            'log': os.path.join(site['local'], 'Logs'),
+            'config': os.path.join(site['local'], 'config.toml')}
+    })
+
+elif os.name == 'posix':  # NOTE: likely Linux
     is_admin = os.getuid() == 0
     site = Namespace(system='/', user=os.path.join(home, '.hypershell'),
                      local=local_site)
     path = Namespace({
         'system': {
             'lib': os.path.join(site.system, 'var', 'lib', 'hypershell'),
             'log': os.path.join(site.system, 'var', 'log', 'hypershell'),
@@ -66,14 +90,19 @@
             'config': os.path.join(site.user, 'config.toml')},
         'local': {
             'lib': os.path.join(site.local, 'lib'),
             'log': os.path.join(site.local, 'log'),
             'config': os.path.join(site.local, 'config.toml')}
     })
 
+else:
+    print(f'{bold(magenta("CRITICAL"))} [{__name__}] '
+          f'Platform unrecognized ({platform.system()})', file=sys.stderr)
+    sys.exit(exit_status.bad_config)
+
 
 if 'HYPERSHELL_SITE' in os.environ:
     default_path = path.local
 else:
     default_path = path.user if not is_admin else path.system
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/queue.py` & `hyper_shell-2.5.0/src/hypershell/core/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Queue server/client implementation."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/remote.py` & `hyper_shell-2.5.0/src/hypershell/core/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Manage remote connections and data."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/template.py` & `hyper_shell-2.5.0/src/hypershell/core/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Template expansion facility for task execution."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.4.0/src/hypershell/core/thread.py` & `hyper_shell-2.5.0/src/hypershell/core/thread.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Thread base class implementation."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.4.0/src/hypershell/data/__init__.py` & `hyper_shell-2.5.0/src/hypershell/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,45 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Database interface, models, and methods."""
 
 
 # type annotations
 from __future__ import annotations
+from typing import Final
 
 # standard libs
 import sys
 import functools
 
 # external libs
 from cmdkit.app import Application, exit_status
 from cmdkit.cli import Interface
 from cmdkit.config import ConfigurationError
 from sqlalchemy import inspect
 from sqlalchemy.orm import close_all_sessions
 from sqlalchemy.exc import OperationalError
 
 # internal libs
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.logging import Logger
 from hypershell.core.config import config
-from hypershell.core.exceptions import (write_traceback, handle_exception, DatabaseUninitialized,
-                                        get_shared_exception_mapping)
+from hypershell.core.exceptions import handle_exception, DatabaseUninitialized, get_shared_exception_mapping
 from hypershell.data.core import engine, in_memory, schema
 from hypershell.data.model import Entity, Task
 
 # public interface
 __all__ = ['InitDBApp', 'initdb', 'truncatedb', 'checkdb', 'ensuredb', 'DATABASE_ENABLED', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
-try:
-    if not in_memory:
-        DATABASE_ENABLED = True
-    else:
-        DATABASE_ENABLED = False
-except Exception as error:
-    write_traceback(error, module=__name__)
-    sys.exit(exit_status.bad_config)
+DATABASE_ENABLED: Final[bool] = not in_memory
+"""Set if database has been configured."""
 
 
 def initdb() -> None:
     """Initialize database tables."""
     Entity.metadata.create_all(engine)
 
 
@@ -64,31 +57,35 @@
 def checkdb() -> None:
     """Ensure database connection and tables exist."""
     if not inspect(engine).has_table('task', schema=schema):
         raise DatabaseUninitialized('Use \'initdb\' to initialize the database')
 
 
 def ensuredb(auto_init: bool = False) -> None:
-    """Ensure database configuration before applying any operations."""
+    """
+    Ensure database configuration before applying any operations.
+
+    If SQLite and `auto_init` we run :meth:`initdb`, else :meth:`checkdb`.
+    """
     db = config.database.get('file', None) or config.database.get('database', None)
     if config.database.provider == 'sqlite' and db in ('', ':memory:', None):
         raise ConfigurationError('Missing database configuration')
     if config.database.provider == 'sqlite' or auto_init is True:
         initdb()
     else:
         checkdb()
 
 
-INITDB_PROGRAM = 'hyper-shell initdb'
+INITDB_PROGRAM = 'hs initdb'
 INITDB_USAGE = f"""\
 Usage:
-{INITDB_PROGRAM} [-h] [--truncate [--yes]]
+  {INITDB_PROGRAM} [-h] [--truncate [--yes]]
 
-Initialize database (not needed for SQLite).
-Use --truncate to zero out the task metadata.\
+  Initialize database (not needed for SQLite).
+  Use --truncate to zero out the task metadata.\
 """
 
 INITDB_HELP = f"""\
 {INITDB_USAGE}
 
 Options:
   -t, --truncate       Truncate database (task metadata will be lost).
@@ -96,17 +93,15 @@
   -h, --help           Show this message and exit.\
 """
 
 
 class InitDBApp(Application):
     """Initialize database (not needed for SQLite)."""
 
-    interface = Interface(INITDB_PROGRAM,
-                          colorize_usage(INITDB_USAGE),
-                          colorize_usage(INITDB_HELP))
+    interface = Interface(INITDB_PROGRAM, INITDB_USAGE, INITDB_HELP)
 
     ALLOW_NOARGS = True
 
     truncate: bool = False
     interface.add_argument('-t', '--truncate', action='store_true')
 
     auto_confirm: bool = False
```

### Comparing `hyper-shell-2.4.0/src/hypershell/data/core.py` & `hyper_shell-2.5.0/src/hypershell/data/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Core interface for database engine and session manager."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.4.0/src/hypershell/data/model.py` & `hyper_shell-2.5.0/src/hypershell/data/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Database models."""
 
 
 # type annotations
 from __future__ import annotations
 from typing import List, Dict, Any, Type, TypeVar, Union, Optional
 
 # standard libs
+import re
 import json
 from uuid import uuid4 as gen_uuid
 from datetime import datetime
 
 # external libs
 from sqlalchemy import Column, Index, func
-from sqlalchemy.orm import Query
+from sqlalchemy.orm import Query, DeclarativeBase, Mapped, mapped_column
 from sqlalchemy.orm.exc import NoResultFound, MultipleResultsFound
-from sqlalchemy.ext.declarative import declarative_base, declared_attr
+from sqlalchemy.ext.declarative import declared_attr
 from sqlalchemy.types import Integer, DateTime, Text, Boolean, JSON as _JSON
-from sqlalchemy.dialects.postgresql import UUID as PostgresUUID, JSONB as PostgresJSON
+from sqlalchemy.dialects.postgresql import UUID as POSTGRES_UUID, JSONB as POSTGRES_JSON
 
 # internal libs
 from hypershell.core.logging import Logger, HOSTNAME, INSTANCE
 from hypershell.core.heartbeat import Heartbeat
+from hypershell.core.types import JSONValue
 from hypershell.data.core import schema, Session
 
 # public interface
 __all__ = ['Task', 'Client', 'Entity', 'to_json_type', 'from_json_type', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
@@ -45,110 +47,111 @@
     """Exception specific to multiple records found when only one should have been."""
 
 
 class AlreadyExists(DatabaseError):
     """Exception specific to a record with unique properties already existing."""
 
 
+# Extended value type contains datetime types
+# These are not valid JSON and must be converted
 VT = TypeVar('VT', bool, int, float, str, type(None), datetime)
-RT = TypeVar('RT', bool, int, float, str, type(None))
 
 
-def to_json_type(value: VT) -> Union[VT, RT]:
+def to_json_type(value: VT) -> Union[VT, JSONValue]:
     """Convert `value` to alternate representation for JSON."""
     return value if not isinstance(value, datetime) else value.isoformat(sep=' ')
 
 
-def from_json_type(value: RT) -> Union[RT, VT]:
+def from_json_type(value: JSONValue) -> Union[JSONValue, VT]:
     """Convert `value` to richer type if possible."""
     try:
         # NOTE: minor detail in PyPy datetime implementation
         if isinstance(value, str) and len(value) > 5:
             return datetime.fromisoformat(value)
         else:
             return value
     except ValueError:
         return value
 
 
-# Column types used by models
-UUID = Text().with_variant(PostgresUUID(as_uuid=False), 'postgresql')
+# Pre-defining types shortens declarations and makes changes easier
+UUID = Text().with_variant(POSTGRES_UUID(as_uuid=False), 'postgresql')
 TEXT = Text()
 INTEGER = Integer()
 DATETIME = DateTime(timezone=True)
 BOOLEAN = Boolean()
-JSON = _JSON().with_variant(PostgresJSON(), 'postgresql')
+JSON = _JSON().with_variant(POSTGRES_JSON(), 'postgresql')
 
 
-class EntityInterface:
+class Entity(DeclarativeBase):
     """Core mixin class for all entities."""
 
     columns: Dict[str, type] = {}
 
     @declared_attr
-    def __tablename__(cls: Type[EntityInterface]) -> str:  # noqa: cls
+    def __tablename__(cls: Type[Entity]) -> str:  # noqa: cls
         """The table name should be lower-case."""
         return cls.__name__.lower()
 
     @declared_attr
     def __table_args__(cls) -> Dict[str, Any]:  # noqa: cls
         """Common table attributes."""
         return {'schema': schema, }
 
-    def __repr__(self: EntityInterface) -> str:
+    def __repr__(self: Entity) -> str:
         """String representation."""
         attrs = ', '.join([f'{name}={repr(getattr(self, name))}' for name in self.columns])
         return f'{self.__class__.__name__}({attrs})'
 
-    def to_tuple(self: EntityInterface) -> tuple:
+    def to_tuple(self: Entity) -> tuple:
         """Convert fields into standard tuple."""
         return tuple([getattr(self, name) for name in self.columns])
 
-    def to_dict(self: EntityInterface) -> Dict[str, Any]:
+    def to_dict(self: Entity) -> Dict[str, Any]:
         """Convert record to dictionary."""
         return dict(zip(self.columns, self.to_tuple()))
 
-    def to_json(self: EntityInterface) -> Dict[str, RT]:
+    def to_json(self: Entity) -> Dict[str, JSONValue]:
         """Convert record to JSON-serializable dictionary."""
         return {key: to_json_type(value) for key, value in self.to_dict().items()}
 
-    def pack(self: EntityInterface) -> bytes:
+    def pack(self: Entity) -> bytes:
         """Encode as raw JSON bytes."""
         return json.dumps(self.to_json()).encode()
 
     @classmethod
-    def from_dict(cls: Type[EntityInterface], data: Dict[str, VT]) -> EntityInterface:
+    def from_dict(cls: Type[Entity], data: Dict[str, VT]) -> Entity:
         """Build from existing dictionary."""
         return cls(**data)  # noqa: __init__ instrumented by declarative_base
 
     @classmethod
-    def from_json(cls: Type[EntityInterface], data: Dict[str, RT]) -> EntityInterface:
+    def from_json(cls: Type[Entity], data: Dict[str, JSONValue]) -> Entity:
         """Build from JSON `text` string."""
         return cls.from_dict({key: from_json_type(value) for key, value in data.items()})
 
     @classmethod
-    def unpack(cls: Type[EntityInterface], data: bytes) -> EntityInterface:
+    def unpack(cls: Type[Entity], data: bytes) -> Entity:
         """Unpack raw JSON byte string."""
         return cls.from_json(json.loads(data.decode()))
 
     @classmethod
-    def query(cls: Type[EntityInterface], *fields: Column, caching: bool = True) -> Query:
+    def query(cls: Type[Entity], *fields: Column, caching: bool = True) -> Query:
         """Get query interface for entity with scoped session."""
         target = fields or [cls, ]
         if not caching:
             Session.expire_all()
         return Session.query(*target)
 
     @classmethod
-    def count(cls: Type[EntityInterface]) -> int:
+    def count(cls: Type[Entity]) -> int:
         """Count of total existing records in database."""
         return cls.query().count()
 
     @classmethod
-    def add_all(cls: Type[EntityInterface], items: List[EntityInterface]) -> List[EntityInterface]:
+    def add_all(cls: Type[Entity], items: List[Entity]) -> List[Entity]:
         """Add many items to the database at once."""
         # NOTE: pull id first because access after commit could trigger query
         item_ids = [item.id for item in items]  # noqa: id not defined on base
         try:
             Session.add_all(items)
             Session.commit()
         except Exception:
@@ -156,81 +159,77 @@
             raise
         else:
             for item_id in item_ids:
                 log.trace(f'Added {cls.__tablename__} ({item_id})')
             return items
 
     @classmethod
-    def add(cls: Type[EntityInterface], item: EntityInterface) -> None:
+    def add(cls: Type[Entity], item: Entity) -> None:
         """Add single item to database."""
         cls.add_all([item, ])
 
     @classmethod
-    def update_all(cls: Type[EntityInterface], changes: List[Dict[str, Any]]) -> None:
+    def update_all(cls: Type[Entity], changes: List[Dict[str, Any]]) -> None:
         """Bulk update."""
         if changes:
             Session.bulk_update_mappings(cls, changes)
             Session.commit()  # NOTE: why is this necessary?
             log.trace(f'Updated {len(changes)} {cls.__tablename__}s')
 
     @classmethod
-    def update(cls: Type[EntityInterface], id: str, **changes) -> None:
+    def update(cls: Type[Entity], id: str, **changes) -> None:
         """Update by `id` with `changes`."""
         cls.update_all([{'id': id, **changes}, ])
 
     @classmethod
-    def from_id(cls: Type[EntityInterface], id: str) -> EntityInterface:
+    def from_id(cls: Type[Entity], id: str) -> Entity:
         """Load by unique `id`."""
         raise NotImplementedError()  # NOTE: non-strict requirement of base
 
     @classmethod
-    def new(cls: Type[EntityInterface], **attrs: Any) -> EntityInterface:
+    def new(cls: Type[Entity], **attrs: Any) -> Entity:
         """Create new instance with default values."""
         raise NotImplementedError()  # NOTE: non-strict requirement of base
 
 
-# declarative base inherits common interface
-Entity = declarative_base(cls=EntityInterface)
-
-
 class Task(Entity):
-    """Database entity for task metadata."""
+    """Task entity within database implements task methods."""
 
-    id = Column(UUID, primary_key=True, nullable=False)
-    args = Column(TEXT, nullable=False)
+    id: Mapped[str] = mapped_column(UUID, primary_key=True, nullable=False)
+    args: Mapped[str] = mapped_column(TEXT, nullable=False)
 
-    submit_id = Column(UUID, nullable=False)
-    submit_time = Column(DATETIME, nullable=False)
-    submit_host = Column(TEXT, nullable=True)
+    submit_id: Mapped[str] = mapped_column(UUID, nullable=False)
+    submit_time: Mapped[datetime] = mapped_column(DATETIME, nullable=False)
+    submit_host: Mapped[Optional[str]] = mapped_column(TEXT, nullable=True)
 
-    server_id = Column(UUID, nullable=True)
-    server_host = Column(TEXT, nullable=True)
-    schedule_time = Column(DATETIME, nullable=True)
+    server_id: Mapped[Optional[str]] = mapped_column(UUID, nullable=True)
+    server_host: Mapped[Optional[str]] = mapped_column(TEXT, nullable=True)
+    schedule_time: Mapped[Optional[datetime]] = mapped_column(DATETIME, nullable=True)
 
-    client_id = Column(UUID, nullable=True)
-    client_host = Column(TEXT, nullable=True)
+    client_id: Mapped[Optional[str]] = mapped_column(UUID, nullable=True)
+    client_host: Mapped[Optional[str]] = mapped_column(TEXT, nullable=True)
 
-    command = Column(TEXT, nullable=True)
-    start_time = Column(DATETIME, nullable=True)
-    completion_time = Column(DATETIME, nullable=True)
-    exit_status = Column(INTEGER, nullable=True)
+    command: Mapped[Optional[str]] = mapped_column(TEXT, nullable=True)
+    start_time: Mapped[Optional[datetime]] = mapped_column(DATETIME, nullable=True)
+    completion_time: Mapped[Optional[datetime]] = mapped_column(DATETIME, nullable=True)
+    exit_status: Mapped[Optional[int]] = mapped_column(INTEGER, nullable=True)
 
-    outpath = Column(TEXT, nullable=True)
-    errpath = Column(TEXT, nullable=True)
+    outpath: Mapped[Optional[str]] = mapped_column(TEXT, nullable=True)
+    errpath: Mapped[Optional[str]] = mapped_column(TEXT, nullable=True)
 
-    attempt = Column(INTEGER, nullable=False)
-    retried = Column(BOOLEAN, nullable=False)
+    attempt: Mapped[int] = mapped_column(INTEGER, nullable=False)
+    retried: Mapped[bool] = mapped_column(BOOLEAN, nullable=False)
 
-    waited = Column(INTEGER, nullable=True)
-    duration = Column(INTEGER, nullable=True)
+    waited: Mapped[Optional[int]] = mapped_column(INTEGER, nullable=True)
+    duration: Mapped[Optional[int]] = mapped_column(INTEGER, nullable=True)
 
-    previous_id = Column(UUID, unique=True, nullable=True)
-    next_id = Column(UUID, unique=True, nullable=True)
+    previous_id: Mapped[Optional[str]] = mapped_column(UUID, unique=True, nullable=True)
+    next_id: Mapped[Optional[str]] = mapped_column(UUID, unique=True, nullable=True)
 
-    tag = Column(JSON, nullable=False, default={})
+    tag: Mapped[dict] = mapped_column(JSON, nullable=False, default={})
 
     columns = {
         'id': str,
         'args': str,
         'submit_id': str,
         'submit_time': datetime,
         'submit_host': str,
@@ -242,15 +241,15 @@
         'command': str,
         'start_time': datetime,
         'completion_time': datetime,
         'exit_status': int,
         'outpath': str,
         'errpath': str,
         'attempt': int,
-        'retried': int,
+        'retried': bool,
         'waited': int,
         'duration': int,
         'previous_id': str,
         'next_id': str,
         'tag': dict,
     }
 
@@ -271,20 +270,42 @@
         except NoResultFound as error:
             raise cls.NotFound(f'No task with id={id}') from error
         except MultipleResultsFound as error:
             raise cls.NotDistinct(f'Multiple tasks with id={id}') from error
 
     @classmethod
     def new(cls: Type[Task], args: str, attempt: int = 1, retried: bool = False,
-            tag: Dict[str, str] = None, **other) -> Task:
+            tag: Dict[str, JSONValue] = None, **other) -> Task:
         """Create a new Task."""
+        cls.ensure_valid_tag(tag)
         return Task(id=str(gen_uuid()), args=str(args).strip(),
                     submit_id=INSTANCE, submit_host=HOSTNAME, submit_time=datetime.now().astimezone(),
                     attempt=attempt, retried=retried, tag=(tag or {}), **other)
 
+    @staticmethod
+    def ensure_valid_tag(tag: Dict[str, JSONValue]) -> None:
+        """Check tag dictionary and raise if invalid."""
+        if not isinstance(tag, (dict, type(None))):
+            raise TypeError('Expected dict or None for tag data')
+        if tag is None:
+            return
+        for key, value in tag.items():
+            if not isinstance(key, str):
+                raise TypeError(f'Tag key, {key} ({type(key)}) is not string')
+            if not isinstance(value, (str, int, float, bool, type(None))):
+                raise TypeError(f'Invalid type for tag value, {type(value)})')
+            if isinstance(value, str):
+                if not value.strip():
+                    return  # Empty value is a naked tag (no value).
+                if len(value) > 120:
+                    raise ValueError(f'Tag size ({len(value)}) exceeds 120 characters ({key}: {value})')
+                if not re.match(r'^[A-Za-z0-9_.+-]+$', value):
+                    raise ValueError(f'Tag must only contain alphanumerics and basic symbols [+._-]: '
+                                     f'({key}: {value})')
+
     @classmethod
     def select_new(cls: Type[Task], limit: int) -> List[Task]:
         """Select unscheduled tasks up to some `limit` in order of submit_time."""
         return (cls.query()
                 .order_by(cls.submit_time)
                 .filter(cls.schedule_time.is_(None))
                 .limit(limit).all())
@@ -337,15 +358,18 @@
     @classmethod
     def __schedule_next_failed_tasks(cls: Type[Task], attempts: int, limit: int) -> List[Task]:
         """Select previously failed tasks for scheduling."""
         tasks = []
         failed_tasks = cls.select_failed(attempts=attempts, limit=limit)
         if failed_tasks:
             log.trace(f'Selected {len(failed_tasks)} previously failed tasks')
-            new_tasks = [cls.new(args=task.args, attempt=task.attempt + 1, previous_id=task.id)
+            new_tasks = [cls.new(args=task.args,
+                                 attempt=task.attempt + 1,
+                                 previous_id=task.id,
+                                 tag=task.tag)
                          for task in failed_tasks]
             tasks.extend(new_tasks)
             cls.add_all(tasks)
             cls.update_all([{'id': old_task.id, 'retried': True, 'next_id': new_task.id}
                             for old_task, new_task in zip(failed_tasks, new_tasks)])
         return tasks
 
@@ -409,14 +433,33 @@
     @classmethod
     def revert_interrupted(cls: Type[Task]) -> None:
         """Revert scheduled but incomplete tasks to un-scheduled state."""
         while tasks := cls.select_interrupted(100):
             cls.revert_all([task.id for task in tasks])
 
     @classmethod
+    def cancel_all(cls: Type[Task], ids: List[str]) -> None:
+        """Cancel all tasks identified by `ids`."""
+        cls.update_all([
+            {
+                'id': id,
+                'schedule_time': datetime.now().astimezone(),
+                'exit_status': -1,
+             }
+            for id in ids
+        ])
+        for id in ids:
+            log.trace(f'Cancelled task ({id})')
+
+    @classmethod
+    def cancel(cls: Type[Task], id: str) -> None:
+        """Cancel single task by `id`."""
+        cls.cancel_all([id, ])
+
+    @classmethod
     def select_orphaned(cls: Type[Task], client_id: str, limit: int) -> List[Task]:
         """Select tasks that were orphaned from an evicted client."""
         return (
             cls.query()
             .order_by(cls.schedule_time)
             .filter(cls.schedule_time.isnot(None))
             .filter(cls.completion_time.is_(None))
@@ -513,25 +556,25 @@
 # Indices for efficient queries
 index_scheduled = Index('task_scheduled_index', Task.schedule_time)
 index_retried = Index('task_retries_index', Task.exit_status, Task.retried)
 index_client_completed = Index('task_client_completed_index', Task.client_id, Task.completion_time)
 
 
 class Client(Entity):
-    """Database entity for client metadata."""
+    """Client entity within database implements client methods."""
 
-    id = Column(UUID, primary_key=True, nullable=False)
-    host = Column(TEXT, nullable=False)
+    id: Mapped[str] = mapped_column(UUID, primary_key=True, nullable=False)
+    host: Mapped[str] = mapped_column(TEXT, nullable=False)
 
-    server_id = Column(UUID, nullable=False)
-    server_host = Column(TEXT, nullable=False)
+    server_id: Mapped[str] = mapped_column(UUID, nullable=False)
+    server_host: Mapped[str] = mapped_column(TEXT, nullable=False)
 
-    connected_at = Column(DATETIME, nullable=True)
-    disconnected_at = Column(DATETIME, nullable=True)
-    evicted = Column(BOOLEAN, nullable=False)
+    connected_at: Mapped[Optional[str]] = mapped_column(DATETIME, nullable=True)
+    disconnected_at: Mapped[Optional[datetime]] = mapped_column(DATETIME, nullable=True)
+    evicted: Mapped[bool] = mapped_column(BOOLEAN, nullable=False)
 
     columns = {
         'id': str,
         'host': str,
         'server_id': str,
         'server_host': str,
         'connected_at': datetime,
```

### Comparing `hyper-shell-2.4.0/src/hypershell/server.py` & `hyper_shell-2.5.0/src/hypershell/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Schedule and update bundles of tasks from the database.
 
 The server can submit tasks for you so no need to directly submit before
 invoking the server (see `hypershell.submit`).
@@ -38,46 +38,48 @@
     your main program exits however, the thread will be stopped regardless because it
     runs as a `daemon`.
 """
 
 
 # type annotations
 from __future__ import annotations
-from typing import List, Dict, Tuple, Iterable, IO, Optional, Callable, Type
+from typing import List, Dict, Tuple, Iterable, IO, Optional, Callable, Type, Final
 from types import TracebackType
 
 # standard libs
 import sys
 import time
 from enum import Enum
 from datetime import datetime, timedelta
 from functools import cached_property
+from itertools import islice
 from queue import Empty as QueueEmpty, Full as QueueFull
 
 # external libs
 from cmdkit.app import Application
 from cmdkit.cli import Interface, ArgumentError
 
 # internal libs
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.exceptions import get_shared_exception_mapping
-from hypershell.core.config import config, default
+from hypershell.core.config import config, default, find_available_ports
 from hypershell.core.logging import Logger
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.thread import Thread
 from hypershell.core.queue import QueueServer, QueueConfig
+from hypershell.core.signal import check_signal, SIGNAL_MAP, SIGUSR1, SIGUSR2
 from hypershell.core.heartbeat import Heartbeat, ClientState
 from hypershell.data.model import Task, Client
 from hypershell.data import ensuredb, DATABASE_ENABLED
 from hypershell.submit import SubmitThread, LiveSubmitThread, DEFAULT_BUNDLEWAIT
 from hypershell.client import ClientInfo
 
 # public interface
 __all__ = ['serve_from', 'serve_file', 'serve_forever', 'ServerThread', 'ServerApp',
-           'DEFAULT_BUNDLESIZE', 'DEFAULT_ATTEMPTS', ]
+           'DEFAULT_BUNDLESIZE', 'DEFAULT_BUNDLEWAIT', 'DEFAULT_ATTEMPTS',
+           'DEFAULT_EVICT', 'DEFAULT_EAGER_MODE', 'DEFAULT_QUERY_PAUSE']
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
 class SchedulerState(State, Enum):
     """Finite states of the scheduler."""
@@ -85,20 +87,28 @@
     LOAD = 1
     PACK = 2
     POST = 3
     FINAL = 4
     HALT = 5
 
 
-# Note: unless specified otherwise for larger problems, a bundle of size one allows
-# for greater concurrency on smaller workloads.
-DEFAULT_BUNDLESIZE: int = default.server.bundlesize
-DEFAULT_ATTEMPTS: int = default.server.attempts
-DEFAULT_EAGER_MODE: bool = default.server.eager
-DEFAULT_QUERY_PAUSE: int = default.server.wait
+# Note:
+#   Unless specified otherwise for larger problems, a bundle of size one allows
+#   for greater concurrency on smaller workloads.
+DEFAULT_BUNDLESIZE: Final[int] = default.server.bundlesize
+"""Default size for task bundles."""
+
+DEFAULT_ATTEMPTS: Final[int] = default.server.attempts
+"""Default number of attempts for task retries."""
+
+DEFAULT_EAGER_MODE: Final[bool] = default.server.eager
+"""When enabled tasks are retried immediately ahead scheduling new tasks."""
+
+DEFAULT_QUERY_PAUSE: Final[int] = default.server.wait
+"""Default polling interval between database queries if no tasks are available."""
 
 
 class Scheduler(StateMachine):
     """Enqueue tasks from database."""
 
     tasks: List[Task]
     queue: QueueServer
@@ -156,14 +166,17 @@
                 log.info(f'Found {tasks_remaining} unfinished task(s)')
                 Task.revert_interrupted()
                 log.info(f'Reverted {tasks_interrupted} previously interrupted task(s)')
         return SchedulerState.LOAD
 
     def load_bundle(self: Scheduler) -> SchedulerState:
         """Load the next task bundle from the database."""
+        if check_signal() in (SIGUSR1, SIGUSR2):
+            log.warning(f'Signal interrupt ({SIGNAL_MAP[check_signal()]})')
+            return SchedulerState.FINAL
         self.tasks = Task.next(limit=self.bundlesize, attempts=self.attempts, eager=self.eager)
         if self.tasks:
             self.startup_phase = False
             return SchedulerState.PACK
         # An empty database must wait for at least one task
         elif not self.forever_mode and Task.count() > 0 and Task.count_remaining() == 0 and not self.startup_phase:
             return SchedulerState.FINAL
@@ -418,15 +431,16 @@
     SWITCH = 3
     CHECK = 4
     SIGNAL = 5
     FINAL = 6
     HALT = 7
 
 
-DEFAULT_EVICT: int = default.server.evict
+DEFAULT_EVICT: Final[int] = default.server.evict
+"""Default client eviction period in seconds."""
 
 
 class HeartMonitor(StateMachine):
     """Collect heartbeat messages from connected clients."""
 
     in_memory: bool
     no_confirm: bool
@@ -490,20 +504,27 @@
         except QueueEmpty:
             return HeartbeatState.SWITCH
 
     def update_client(self: HeartMonitor) -> HeartbeatState:
         """Update client with heartbeat or disconnect."""
         hb = self.latest_heartbeat
         if hb.state is not ClientState.FINISHED:
-            if hb.uuid not in self.beats:
+            if hb.uuid in self.beats:
+                log.trace(f'Heartbeat - running ({hb.host}: {hb.uuid})')
+            else:
                 log.debug(f'Registered client ({hb.host}: {hb.uuid})')
                 if not self.in_memory:
-                    Client.add(Client.from_heartbeat(hb))
-            else:
-                log.trace(f'Heartbeat - running ({hb.host}: {hb.uuid})')
+                    new_client = Client.from_heartbeat(hb)
+                    try:
+                        # Check to see if we are re-registering a falsely-evicted client (Issue #29)
+                        old_client = Client.from_id(new_client.id)
+                        log.warning(f'Existing client re-registered ({old_client.host}: {old_client.id})')
+                        Client.update(old_client.id, disconnected_at=None, evicted=False)
+                    except Client.NotFound:
+                        Client.add(new_client)
             self.beats[hb.uuid] = hb
             return HeartbeatState.SWITCH
         else:
             log.trace(f'Client disconnected ({hb.host}: {hb.uuid})')
             if hb.uuid in self.beats:
                 self.beats.pop(hb.uuid)
                 if not self.in_memory:
@@ -582,34 +603,111 @@
     def stop(self: HeartMonitorThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (heartbeat)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
+DEFAULT_BIND: Final[str] = QueueConfig.host
+"""Default bind address for server."""
+
+DEFAULT_PORT: Final[int] = QueueConfig.port
+"""Default port number for server."""
+
+DEFAULT_AUTH: Final[str] = QueueConfig.auth
+"""Default authentication key for server (**DO NOT USE THIS**)."""
+
+
 class ServerThread(Thread):
-    """Manage asynchronous task bundle scheduling and receiving."""
+    """
+    Run server within dedicated thread.
+
+    Args:
+        source (Iterable[str], optional):
+            Any iterable of command-line tasks.
+            A new `source` results in a :class:`~hypershell.submit.SubmitThread` populating
+            either the database or the queue directly depending on `in_memory`.
+
+        restart_mode (bool, optional):
+            If `source` is empty, this option allows for the server to continue
+            with scheduling from the database until complete.
+            Conflicts with `in_memory`. Default is `False`.
+
+        forever_mode (bool, optional):
+            Regardless of `source`, if enabled schedule forever.
+            Conflicts with `restart_mode` and `in_memory`. Default is `False`.
+
+        bundlesize (int, optional):
+            Size of task bundles. See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int, optional):
+            Waiting period before forcing task bundle push.
+            See :const:`~hypershell.submit.DEFAULT_BUNDLEWAIT`.
+
+        in_memory (bool, optional):
+            If True, revert to basic in-memory queue.
+
+        no_confirm (bool, optional):
+            If True, do not check for client confirmation messages.
+
+        address (tuple, optional):
+            Bind address for server with port number.
+            See :const:`DEFAULT_BIND` and :const:`DEFAULT_PORT`.
+
+        auth (str, optional):
+            Server authentication key. See :const:`DEFAULT_AUTH`.
+
+        max_retries (int, optional):
+            Number of allowed task retries. See :const:`DEFAULT_ATTEMPTS`.
+
+        eager (bool, optional):
+            When enabled tasks are retried immediately ahead scheduling new tasks.
+            See :const:`DEFAULT_EAGER_MODE`.
+
+        redirect_failures (bool, optional):
+            Open file descriptor to write failed tasks.
+
+        evict_after (int, optional):
+            Period in seconds to wait before evicting clients that miss heartbeats.
+            See :const:`DEFAULT_EVICT`.
+
+    Example:
+        >>> from hypershell.server import ServerThread
+        >>> server = ServerThread.new(restart_mode=True, auth='my-secret-key')
+        >>> server.join()
+
+    See Also:
+        - :meth:`serve_from`
+        - :meth:`serve_file`
+        - :meth:`serve_forever`
+    """
 
     queue: QueueServer
     submitter: Optional[SubmitThread]
     scheduler: Optional[SchedulerThread]
     confirm: Optional[ConfirmThread]
     receiver: ReceiverThread
     heartmonitor: HeartMonitorThread
     in_memory: bool
     no_confirm: bool
 
     def __init__(self: ServerThread,
                  source: Iterable[str] = None,
-                 in_memory: bool = False, no_confirm: bool = False,
-                 forever_mode: bool = False, restart_mode: bool = False,
-                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-                 address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
-                 max_retries: int = DEFAULT_ATTEMPTS - 1, eager: bool = False,
-                 redirect_failures: IO = None, evict_after: int = DEFAULT_EVICT) -> None:
+                 bundlesize: int = DEFAULT_BUNDLESIZE,
+                 bundlewait: int = DEFAULT_BUNDLEWAIT,
+                 in_memory: bool = False,
+                 no_confirm: bool = False,
+                 forever_mode: bool = False,
+                 restart_mode: bool = False,
+                 address: Tuple[str, int] = (DEFAULT_BIND, DEFAULT_PORT),
+                 auth: str = DEFAULT_AUTH,
+                 max_retries: int = DEFAULT_ATTEMPTS - 1,
+                 eager: bool = False,
+                 redirect_failures: IO = None,
+                 evict_after: int = DEFAULT_EVICT) -> None:
         """Initialize queue manager and child threads."""
         self.in_memory = in_memory
         self.no_confirm = no_confirm
         if not self.in_memory and not DATABASE_ENABLED:
             log.warning('No database configured - automatically disabled')
             self.in_memory = True
         if self.in_memory and max_retries > 0:
@@ -700,88 +798,277 @@
         self.receiver.stop(wait=wait, timeout=timeout)
         if not self.no_confirm:
             self.queue.confirmed.put(None)
             self.confirm.stop(wait=wait, timeout=timeout)
         super().stop(wait=wait, timeout=timeout)
 
 
-def serve_from(source: Iterable[str], in_memory: bool = False, no_confirm: bool = False,
-               bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-               address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
-               max_retries: int = DEFAULT_ATTEMPTS - 1, eager: bool = DEFAULT_EAGER_MODE,
-               redirect_failures: IO = None, restart_mode: bool = False, evict_after: int = DEFAULT_EVICT) -> None:
-    """Run server with the given task `source`, run until complete."""
-    thread = ServerThread.new(source=source, in_memory=in_memory, no_confirm=no_confirm,
-                              bundlesize=bundlesize, bundlewait=bundlewait, address=address, auth=auth,
-                              max_retries=max_retries, eager=eager, restart_mode=restart_mode,
-                              redirect_failures=redirect_failures, evict_after=evict_after)
+def serve_from(source: Iterable[str],
+               restart_mode: bool = False,
+               bundlesize: int = DEFAULT_BUNDLESIZE,
+               bundlewait: int = DEFAULT_BUNDLEWAIT,
+               in_memory: bool = False,
+               no_confirm: bool = False,
+               address: Tuple[str, int] = (DEFAULT_BIND, DEFAULT_PORT),
+               auth: str = DEFAULT_AUTH,
+               max_retries: int = DEFAULT_ATTEMPTS - 1,
+               eager: bool = DEFAULT_EAGER_MODE,
+               redirect_failures: IO = None,
+               evict_after: int = DEFAULT_EVICT) -> None:
+    """
+    Start server with given task `source`, run until complete.
+
+    Args:
+        source (Iterable[str]):
+            Any iterable of command-line tasks.
+
+        restart_mode (bool, optional):
+            If `source` is empty, this option allows for the server to continue
+            with scheduling from the database until complete.
+            Conflicts with `in_memory`. Default is `False`.
+
+        bundlesize (int, optional):
+            Size of task bundles. See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int, optional):
+            Waiting period before forcing task bundle push.
+            See :const:`~hypershell.submit.DEFAULT_BUNDLEWAIT`.
+
+        in_memory (bool, optional):
+            If True, revert to basic in-memory queue.
+
+        no_confirm (bool, optional):
+            If True, do not check for client confirmation messages.
+
+        address (tuple, optional):
+            Bind address for server with port number.
+            See :const:`DEFAULT_BIND` and :const:`DEFAULT_PORT`.
+
+        auth (str, optional):
+            Server authentication key. See :const:`DEFAULT_AUTH`.
+
+        max_retries (int, optional):
+            Number of allowed task retries. See :const:`DEFAULT_ATTEMPTS`.
+
+        eager (bool, optional):
+            When enabled tasks are retried immediately ahead scheduling new tasks.
+            See :const:`DEFAULT_EAGER_MODE`.
+
+        redirect_failures (bool, optional):
+            Open file descriptor to write failed tasks.
+
+        evict_after (int, optional):
+            Period in seconds to wait before evicting clients that miss heartbeats.
+            See :const:`DEFAULT_EVICT`.
+
+    Example:
+        >>> from hypershell.server import serve_from
+        >>> serve_from(['echo AA', 'echo BB', 'echo CC'], auth='my-secret-key')
+
+    See Also:
+        - :meth:`serve_file`
+        - :meth:`serve_forever`
+    """
+    thread = ServerThread.new(source=source,
+                              restart_mode=restart_mode,
+                              bundlesize=bundlesize,
+                              bundlewait=bundlewait,
+                              in_memory=in_memory,
+                              no_confirm=no_confirm,
+                              address=address, auth=auth,
+                              max_retries=max_retries,
+                              eager=eager,
+                              redirect_failures=redirect_failures,
+                              evict_after=evict_after)
     try:
         thread.join()
     except Exception:
         thread.stop()
         raise
 
 
-def serve_file(path: str, in_memory: bool = False, no_confirm: bool = False, redirect_failures: IO = None,
-               bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-               address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
-               max_retries: int = DEFAULT_ATTEMPTS - 1, eager: bool = DEFAULT_EAGER_MODE,
-               evict_after: int = DEFAULT_EVICT, **file_options) -> None:
-    """Run server with tasks from a local file `path`, run until complete."""
+def serve_file(path: str,
+               bundlesize: int = DEFAULT_BUNDLESIZE,
+               bundlewait: int = DEFAULT_BUNDLEWAIT,
+               in_memory: bool = False,
+               no_confirm: bool = False,
+               address: Tuple[str, int] = (DEFAULT_BIND, DEFAULT_PORT),
+               auth: str = DEFAULT_AUTH,
+               max_retries: int = DEFAULT_ATTEMPTS - 1,
+               eager: bool = DEFAULT_EAGER_MODE,
+               redirect_failures: IO = None,
+               evict_after: int = DEFAULT_EVICT,
+               **file_options) -> None:
+    """
+    Run server with tasks from a local file `path`, run until complete.
+
+    Args:
+        path (str):
+            Path to file containing command-line tasks.
+
+        bundlesize (int, optional):
+            Size of task bundles. See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int, optional):
+            Waiting period before forcing task bundle push.
+            See :const:`~hypershell.submit.DEFAULT_BUNDLEWAIT`.
+
+        in_memory (bool, optional):
+            If True, revert to basic in-memory queue.
+
+        no_confirm (bool, optional):
+            If True, do not check for client confirmation messages.
+
+        address (tuple, optional):
+            Bind address for server with port number.
+            See :const:`DEFAULT_BIND` and :const:`DEFAULT_PORT`.
+
+        auth (str, optional):
+            Server authentication key. See :const:`DEFAULT_AUTH`.
+
+        max_retries (int, optional):
+            Number of allowed task retries. See :const:`DEFAULT_ATTEMPTS`.
+
+        eager (bool, optional):
+            When enabled tasks are retried immediately ahead scheduling new tasks.
+            See :const:`DEFAULT_EAGER_MODE`.
+
+        redirect_failures (bool, optional):
+            Open file descriptor to write failed tasks.
+
+        evict_after (int, optional):
+            Period in seconds to wait before evicting clients that miss heartbeats.
+            See :const:`DEFAULT_EVICT`.
+
+    Keyword Args:
+        file_options (Any, optional):
+            Forwarded to :meth:`open` function.
+
+    Example:
+        >>> from hypershell.server import serve_file
+        >>> serve_from('/tmp/tasks.in', auth='my-secret-key', bundlesize=10)
+
+    See Also:
+        - :meth:`serve_from`
+        - :meth:`serve_forever`
+    """
     with open(path, mode='r', **file_options) as stream:
-        serve_from(stream, in_memory=in_memory, no_confirm=no_confirm, redirect_failures=redirect_failures,
-                   bundlesize=bundlesize, bundlewait=bundlewait, address=address, auth=auth,
-                   max_retries=max_retries, eager=eager, evict_after=evict_after)
-
-
-def serve_forever(bundlesize: int = DEFAULT_BUNDLESIZE, in_memory: bool = False, no_confirm: bool = False,
-                  address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
-                  max_retries: int = DEFAULT_ATTEMPTS - 1, eager: bool = DEFAULT_EAGER_MODE,
-                  redirect_failures: IO = None, evict_after: int = DEFAULT_EVICT) -> None:
-    """Run server forever."""
-    thread = ServerThread.new(source=None, in_memory=in_memory, no_confirm=no_confirm,
-                              bundlesize=bundlesize, address=address, auth=auth, redirect_failures=redirect_failures,
-                              forever_mode=True, max_retries=max_retries, eager=eager, evict_after=evict_after)
+        serve_from(stream,
+                   bundlesize=bundlesize,
+                   bundlewait=bundlewait,
+                   in_memory=in_memory,
+                   no_confirm=no_confirm,
+                   address=address,
+                   auth=auth,
+                   max_retries=max_retries,
+                   eager=eager,
+                   redirect_failures=redirect_failures,
+                   evict_after=evict_after)
+
+
+def serve_forever(bundlesize: int = DEFAULT_BUNDLESIZE,
+                  in_memory: bool = False,
+                  no_confirm: bool = False,
+                  address: Tuple[str, int] = (DEFAULT_BIND, DEFAULT_PORT),
+                  auth: str = DEFAULT_AUTH,
+                  max_retries: int = DEFAULT_ATTEMPTS - 1,
+                  eager: bool = DEFAULT_EAGER_MODE,
+                  redirect_failures: IO = None,
+                  evict_after: int = DEFAULT_EVICT) -> None:
+    """
+    Run server forever.
+
+    Args:
+        bundlesize (int, optional):
+            Size of task bundles. See :const:`DEFAULT_BUNDLESIZE`.
+
+        in_memory (bool, optional):
+            If True, revert to basic in-memory queue.
+
+        no_confirm (bool, optional):
+            If True, do not check for client confirmation messages.
+
+        address (tuple, optional):
+            Bind address for server with port number.
+            See :const:`DEFAULT_BIND` and :const:`DEFAULT_PORT`.
+
+        auth (str, optional):
+            Server authentication key. See :const:`DEFAULT_AUTH`.
+
+        max_retries (int, optional):
+            Number of allowed task retries. See :const:`DEFAULT_ATTEMPTS`.
+
+        eager (bool, optional):
+            When enabled tasks are retried immediately ahead scheduling new tasks.
+            See :const:`DEFAULT_EAGER_MODE`.
+
+        redirect_failures (bool, optional):
+            Open file descriptor to write failed tasks.
+
+        evict_after (int, optional):
+            Period in seconds to wait before evicting clients that miss heartbeats.
+            See :const:`DEFAULT_EVICT`.
+
+    Example:
+        >>> from hypershell.server import serve_forever
+        >>> serve_forever(address=('0.0.0.0', 54321), auth='my-secret-key',
+        ...               max_retries=2, eager=True, evict_after=600)
+
+    See Also:
+        - :meth:`serve_from`
+        - :meth:`serve_file`
+    """
+    thread = ServerThread.new(source=None,
+                              bundlesize=bundlesize,
+                              in_memory=in_memory,
+                              no_confirm=no_confirm,
+                              address=address,
+                              auth=auth,
+                              redirect_failures=redirect_failures,
+                              forever_mode=True,
+                              max_retries=max_retries,
+                              eager=eager,
+                              evict_after=evict_after)
     try:
         thread.join()
     except Exception:
         thread.stop()
         raise
 
 
-APP_NAME = 'hyper-shell server'
+APP_NAME = 'hs server'
 APP_USAGE = f"""\
 Usage:
-hyper-shell server [-h] [FILE | --forever | --restart] [-b NUM] [-w SEC] [-r NUM [--eager]]
-                   [-H ADDR] [-p PORT] [-k KEY] [--no-db | --initdb] [--print | -f PATH] [--no-confirm]
+  hs server [-h] [FILE | --forever | --restart] [-b NUM] [-w SEC] [-r NUM [--eager]]
+            [-H ADDR] [-p PORT] [-k KEY] [--no-db | --initdb] [--print | -f PATH] [--no-confirm]
 
-Launch server, schedule directly or asynchronously from database.\
+  Launch server, schedule directly or asynchronously from database.\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
-The server includes a scheduler component that pulls tasks from the database and offers
-them up on a distributed queue to clients. It also has a receiver that collects the results
-of finished tasks. Optionally, the server can submit tasks (FILE). When submitting tasks,
-the -w/--bundlewait and -b/--bundlesize options are the same as for 'hyper-shell submit'.
-
-With --max-retries greater than zero and with the database configured, the scheduler will 
-check for a non-zero exit status for tasks and re-submit them if their previous number of 
-attempts is less.
+  The server includes a scheduler component that pulls tasks from the database and offers
+  them up on a distributed queue to clients. It also has a receiver that collects the results
+  of finished tasks. Optionally, the server can submit tasks (FILE). When submitting tasks,
+  the -w/--bundlewait and -b/--bundlesize options are the same as for 'hs submit'.
+
+  With --max-retries greater than zero and with the database configured, the scheduler will 
+  check for a non-zero exit status for tasks and re-submit them if their previous number of 
+  attempts is less.
 
-Tasks are bundled and clients pull them in these bundles. However, by default the bundle
-size is one, meaning that at small scales there is greater responsiveness.
+  Tasks are bundled and clients pull them in these bundles. However, by default the bundle
+  size is one, meaning that at small scales there is greater responsiveness.
 
 Arguments:
   FILE                        Path to input task file (default: <stdin>).
 
 Options:
-  -H, --bind            ADDR  Bind address (default: {QueueConfig.host}).
-  -p, --port            NUM   Port number (default: {QueueConfig.port}).
+  -H, --bind            ADDR  Bind address (default: {DEFAULT_BIND}).
+  -p, --port            NUM   Port number (default: {DEFAULT_PORT}).
   -k, --auth            KEY   Cryptographic key to secure server.
       --forever               Schedule forever.
       --restart               Start scheduling from last completed task.
   -b, --bundlesize      NUM   Size of task bundle (default: {DEFAULT_BUNDLESIZE}).
   -w, --bundlewait      SEC   Seconds to wait before flushing tasks (default: {DEFAULT_BUNDLEWAIT}).
   -r, --max-retries     NUM   Auto-retry failed tasks (default: {DEFAULT_ATTEMPTS - 1}).
       --eager                 Schedule failed tasks before new tasks.
@@ -794,17 +1081,15 @@
 """
 
 
 class ServerApp(Application):
     """Run server in stand-alone mode."""
 
     name = APP_NAME
-    interface = Interface(APP_NAME,
-                          colorize_usage(APP_USAGE),
-                          colorize_usage(APP_HELP))
+    interface = Interface(APP_NAME, APP_USAGE, APP_HELP)
 
     filepath: str
     interface.add_argument('filepath', nargs='?', default=None)
 
     bundlesize: int = config.server.bundlesize
     interface.add_argument('-b', '--bundlesize', type=int, default=bundlesize)
 
@@ -842,30 +1127,47 @@
 
     print_mode: bool = False
     failure_path: str = None
     output_interface = interface.add_mutually_exclusive_group()
     output_interface.add_argument('--print', action='store_true', dest='print_mode')
     output_interface.add_argument('-f', '--failures', default=None, dest='failure_path')
 
+    # Hidden options used as helpers for shell completion
+    interface.add_argument('--available-ports', action='version',
+                           version='\n'.join(map(str, islice(find_available_ports(), 10))))
+
     exceptions = {
         **get_shared_exception_mapping(__name__)
     }
 
     def run(self: ServerApp) -> None:
         """Run server."""
         if self.forever_mode:
-            serve_forever(bundlesize=self.bundlesize, address=(self.host, self.port), auth=self.auth,
-                          in_memory=self.in_memory, no_confirm=self.no_confirm,
-                          max_retries=self.max_retries, eager=self.eager_mode,
-                          redirect_failures=self.failure_stream, evict_after=config.server.evict)
+            serve_forever(bundlesize=self.bundlesize,
+                          address=(self.host, self.port),
+                          auth=self.auth,
+                          in_memory=self.in_memory,
+                          no_confirm=self.no_confirm,
+                          max_retries=self.max_retries,
+                          eager=self.eager_mode,
+                          redirect_failures=self.failure_stream,
+                          evict_after=config.server.evict)
         else:
-            serve_from(source=self.input_stream, bundlesize=self.bundlesize, bundlewait=self.bundlewait,
-                       address=(self.host, self.port), auth=self.auth, max_retries=self.max_retries,
-                       in_memory=self.in_memory, no_confirm=self.no_confirm, evict_after=config.server.evict,
-                       redirect_failures=self.failure_stream, restart_mode=self.restart_mode, eager=self.eager_mode)
+            serve_from(source=self.input_stream,
+                       bundlesize=self.bundlesize,
+                       bundlewait=self.bundlewait,
+                       address=(self.host, self.port),
+                       auth=self.auth,
+                       in_memory=self.in_memory,
+                       no_confirm=self.no_confirm,
+                       restart_mode=self.restart_mode,
+                       max_retries=self.max_retries,
+                       eager=self.eager_mode,
+                       redirect_failures=self.failure_stream,
+                       evict_after=config.server.evict)
 
     def check_args(self: ServerApp):
         """Fail particular argument combinations."""
         if self.filepath and self.forever_mode:
             raise ArgumentError('Cannot specify both FILE and --forever')
         if self.filepath is None and not self.forever_mode:
             self.filepath = '-'  # NOTE: assume STDIN
```

### Comparing `hyper-shell-2.4.0/src/hypershell/submit.py` & `hyper_shell-2.5.0/src/hypershell/submit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2024 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Submit tasks to the database.
 
 Any iterable of command lines can be submitted directly.
 Example:
@@ -35,15 +35,15 @@
     your main program exits however, the thread will be stopped regardless because it
     runs as a `daemon`.
 """
 
 
 # type annotations
 from __future__ import annotations
-from typing import List, Iterable, Iterator, IO, Optional, Dict, Callable, Type
+from typing import List, Iterable, Iterator, IO, Optional, Dict, Callable, Type, Final
 from types import TracebackType
 
 # standard libs
 import io
 import sys
 import functools
 from enum import Enum
@@ -52,29 +52,29 @@
 
 # external libs
 from cmdkit.config import ConfigurationError
 from cmdkit.app import Application
 from cmdkit.cli import Interface
 
 # internal libs
-from hypershell.core.ansi import colorize_usage
 from hypershell.core.logging import Logger
 from hypershell.core.config import config, default
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.queue import QueueClient, QueueConfig
 from hypershell.core.thread import Thread
 from hypershell.core.template import Template, DEFAULT_TEMPLATE
 from hypershell.core.exceptions import get_shared_exception_mapping
+from hypershell.core.types import JSONValue
 from hypershell.data.model import Task
 from hypershell.data import initdb, checkdb
 from hypershell.task import Tag
 
 # public interface
 __all__ = ['submit_from', 'submit_file', 'SubmitThread', 'LiveSubmitThread',
-           'SubmitApp', 'DEFAULT_BUNDLESIZE', 'DEFAULT_BUNDLEWAIT']
+           'SubmitApp', 'DEFAULT_BUNDLESIZE', 'DEFAULT_BUNDLEWAIT', 'DEFAULT_TEMPLATE']
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
 class LoaderState(State, Enum):
     """Finite states of loader machine."""
@@ -178,16 +178,19 @@
     START = 0
     GET = 1
     COMMIT = 2
     FINAL = 3
     HALT = 4
 
 
-DEFAULT_BUNDLESIZE: int = default.submit.bundlesize
-DEFAULT_BUNDLEWAIT: int = default.submit.bundlewait
+DEFAULT_BUNDLESIZE: Final[int] = default.submit.bundlesize
+"""Default size of task bundles."""
+
+DEFAULT_BUNDLEWAIT: Final[int] = default.submit.bundlewait
+"""Default waiting period before forcing task bundle push."""
 
 
 class DatabaseCommitter(StateMachine):
     """Commit tasks from local queue to database."""
 
     queue: Queue[Optional[Task]]
     tasks: List[Task]
@@ -274,24 +277,59 @@
         """Stop machine."""
         log.warning('Stopping (committer: database)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class SubmitThread(Thread):
-    """Manage asynchronous task queueing and submission workload."""
+    """
+    Submit tasks to database within dedicated thread.
+
+    Args:
+        source (Iterable[str]):
+            Any iterable of command-line tasks.
+
+        bundlesize (int, optional):
+            Size of task bundles.
+            See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int, optional):
+            Waiting period before forcing task bundle push.
+            See :const:`DEFAULT_BUNDLEWAIT`.
+
+        template (str, optional):
+            Task command-line template pattern.
+            See :const:`DEFAULT_TEMPLATE`.
+
+        tags (Dict[str, JSONValue], optional):
+            Tag dictionary for all submitted tasks.
+
+    Example:
+        >>> from hypershell.submit import SubmitThread
+        >>> submitter = SubmitThread.new(['AAA', 'BBB', 'CCC'],
+        ...                              template='my-script {}'
+        ...                              tags={'site': 'zzz', 'group': 37})
+        >>> submitter.join()
+
+    See Also:
+        - :meth:`submit_from`
+        - :meth:`submit_file`
+    """
 
     source: Iterable[str]
     queue: Queue[Optional[Task]]
     loader: LoaderThread
     committer: DatabaseCommitterThread
 
-    def __init__(self: SubmitThread, source: Iterable[str], bundlesize: int = DEFAULT_BUNDLESIZE,
-                 bundlewait: int = DEFAULT_BUNDLEWAIT, template: str = DEFAULT_TEMPLATE,
-                 tags: Dict[str, str] = None) -> None:
+    def __init__(self: SubmitThread,
+                 source: Iterable[str],
+                 bundlesize: int = DEFAULT_BUNDLESIZE,
+                 bundlewait: int = DEFAULT_BUNDLEWAIT,
+                 template: str = DEFAULT_TEMPLATE,
+                 tags: Dict[str, JSONValue] = None) -> None:
         """Initialize queue and child threads."""
         self.source = source
         self.queue = Queue(maxsize=bundlesize)
         self.loader = LoaderThread(source=source, queue=self.queue, template=template, tags=tags)
         self.committer = DatabaseCommitterThread(queue=self.queue, bundlesize=bundlesize, bundlewait=bundlewait)
         super().__init__(name='hypershell-submit')
 
@@ -444,15 +482,53 @@
         """Stop machine."""
         log.warning('Stopping (committer: no database)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class LiveSubmitThread(Thread):
-    """Manage asynchronous task queueing and submission workload."""
+    """
+    Submit tasks directly to queue within dedicated thread.
+
+    Args:
+        source (Iterable[str]):
+            Any iterable of command-line tasks.
+
+        queue_config (:class:`~hypershell.core.queue.QueueConfig`):
+            QueueConfig instance with `host`, `port`, and `auth`.
+
+        bundlesize (int, optional):
+            Size of task bundles.
+            See :const:`DEFAULT_BUNDLESIZE`.
+
+        bundlewait (int, optional):
+            Waiting period before forcing task bundle push.
+            See :const:`DEFAULT_BUNDLEWAIT`.
+
+        template (str, optional):
+            Task command-line template pattern.
+            See :const:`DEFAULT_TEMPLATE`.
+
+        tags (Dict[str, JSONValue], optional):
+            Tag dictionary for all submitted tasks.
+
+    Example:
+        >>> from hypershell.submit import LiveSubmitThread
+        >>> from hypershell.core.queue import QueueConfig
+        >>> queue_config = QueueConfig(host='localhost', port=54321, auth='my-secret-key')
+        >>> submitter = LiveSubmitThread.new(['AAA', 'BBB', 'CCC'],
+        ...                                  queue_config=queue_config,
+        ...                                  template='my-script {}'
+        ...                                  tags={'site': 'zzz', 'group': 37})
+        >>> submitter.join()
+
+    See Also:
+        - :meth:`submit_from`
+        - :meth:`submit_file`
+    """
 
     source: Iterable[str]
     local: Queue[Optional[Task]]
     client: QueueClient
     loader: LoaderThread
     committer: QueueCommitterThread
 
@@ -505,48 +581,71 @@
 
     @property
     def task_count(self: LiveSubmitThread) -> int:
         """Count of submitted tasks."""
         return self.loader.machine.count
 
 
-def submit_from(source: Iterable[str], queue_config: QueueConfig = None,
-                bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-                template: str = DEFAULT_TEMPLATE, tags: Dict[str, str] = None) -> int:
-    """Submit all task arguments from `source`, return count of submitted tasks."""
+def submit_from(source: Iterable[str],
+                queue_config: QueueConfig = None,
+                bundlesize: int = DEFAULT_BUNDLESIZE,
+                bundlewait: int = DEFAULT_BUNDLEWAIT,
+                template: str = DEFAULT_TEMPLATE,
+                tags: Dict[str, JSONValue] = None) -> int:
+    """
+    Submit all task arguments from `source`, return count of submitted tasks.
+
+    Returns:
+        task_count (int): Count of submitted tasks.
+    """
     if not queue_config:
-        thread = SubmitThread.new(source=source, bundlesize=bundlesize, bundlewait=bundlewait,
-                                  template=template, tags=tags)
+        thread = SubmitThread.new(source=source,
+                                  bundlesize=bundlesize,
+                                  bundlewait=bundlewait,
+                                  template=template,
+                                  tags=tags)
     else:
-        thread = LiveSubmitThread.new(source=source, queue_config=queue_config, template=template,
-                                      bundlesize=bundlesize, bundlewait=bundlewait, tags=tags)
+        thread = LiveSubmitThread.new(source=source,
+                                      queue_config=queue_config,
+                                      template=template,
+                                      bundlesize=bundlesize,
+                                      bundlewait=bundlewait,
+                                      tags=tags)
     try:
         thread.join()
     except Exception:
         thread.stop()
         raise
     else:
         return thread.task_count
 
 
-def submit_file(path: str, queue_config: QueueConfig = None,
-                bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
-                template: str = DEFAULT_TEMPLATE, **options) -> int:
-    """Submit tasks by reading argument lines from local file `path`."""
-    with open(path, mode='r', **options) as stream:
+def submit_file(path: str,
+                queue_config: QueueConfig = None,
+                bundlesize: int = DEFAULT_BUNDLESIZE,
+                bundlewait: int = DEFAULT_BUNDLEWAIT,
+                template: str = DEFAULT_TEMPLATE,
+                tags: Dict[str, JSONValue] = None,
+                **file_options) -> int:
+    """
+    Submit all task arguments by reading them from file `path`.
+
+    Returns:
+        task_count (int): Count of submitted tasks.
+    """
+    with open(path, mode='r', **file_options) as stream:
         return submit_from(stream, queue_config=queue_config, bundlesize=bundlesize,
-                           bundlewait=bundlewait, template=template)
+                           bundlewait=bundlewait, template=template, tags=tags)
 
 
-APP_NAME = 'hyper-shell submit'
+APP_NAME = 'hs submit'
 APP_USAGE = f"""\
 Usage:
-{APP_NAME} [-h] [FILE] [-b NUM] [-w SEC] [-t CMD] [--initdb] [--tag TAG [TAG...]]
-
-Submit tasks from a file.\
+  {APP_NAME} [-h] [FILE] [-b NUM] [-w SEC] [-t CMD] [--initdb] [--tag TAG [TAG...]]
+  Submit tasks from a file.\
 """
 
 APP_HELP = f"""\
 {APP_USAGE}
 
 Arguments:
   FILE                       Path to task file ("-" for <stdin>).
@@ -561,17 +660,15 @@
 """
 
 
 class SubmitApp(Application):
     """Submit tasks to the database."""
 
     name = APP_NAME
-    interface = Interface(APP_NAME,
-                          colorize_usage(APP_USAGE),
-                          colorize_usage(APP_HELP))
+    interface = Interface(APP_NAME, APP_USAGE, APP_HELP)
 
     source: IO
     filepath: str
     interface.add_argument('filepath', nargs='?', default='-')
 
     bundlesize: int = config.submit.bundlesize
     interface.add_argument('-b', '--bundlesize', type=int, default=bundlesize)
```

