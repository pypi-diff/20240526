# Comparing `tmp/xmppy-0.11.tar.gz` & `tmp/xmppy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xmppy-0.11.tar", last modified: Fri Nov  1 13:04:50 2019, max compression
+gzip compressed data, was "xmppy-0.2.tar", max compression
```

## Comparing `xmppy-0.11.tar` & `xmppy-0.2.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 albert    (1000) users      (985)        0 2019-11-01 13:04:50.000000 xmppy-0.11/
--rw-r--r--   0 albert    (1000) users      (985)      269 2019-11-01 13:04:50.000000 xmppy-0.11/PKG-INFO
--rw-r--r--   0 albert    (1000) users      (985)     3183 2019-07-03 19:23:39.000000 xmppy-0.11/README.md
--rw-r--r--   0 albert    (1000) users      (985)       38 2019-11-01 13:04:50.000000 xmppy-0.11/setup.cfg
--rw-r--r--   0 albert    (1000) users      (985)      469 2019-11-01 12:57:43.000000 xmppy-0.11/setup.py
-drwxr-xr-x   0 albert    (1000) users      (985)        0 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy/
--rw-r--r--   0 albert    (1000) users      (985)     6485 2019-11-01 12:52:25.000000 xmppy-0.11/xmppy/Messenger.py
--rw-r--r--   0 albert    (1000) users      (985)       24 2019-06-29 00:48:55.000000 xmppy-0.11/xmppy/__init__.py
--rw-r--r--   0 albert    (1000) users      (985)     4680 2019-06-30 08:01:02.000000 xmppy-0.11/xmppy/gpg_holder.py
-drwxr-xr-x   0 albert    (1000) users      (985)        0 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/
--rw-r--r--   0 albert    (1000) users      (985)      269 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/PKG-INFO
--rw-r--r--   0 albert    (1000) users      (985)      251 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/SOURCES.txt
--rw-r--r--   0 albert    (1000) users      (985)        1 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/dependency_links.txt
--rw-r--r--   0 albert    (1000) users      (985)       48 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/entry_points.txt
--rw-r--r--   0 albert    (1000) users      (985)       33 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/requires.txt
--rw-r--r--   0 albert    (1000) users      (985)        6 2019-11-01 13:04:50.000000 xmppy-0.11/xmppy.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1075 2023-09-15 00:04:48.813931 xmppy-0.2/LICENSE
+-rw-r--r--   0        0        0     3349 2024-05-25 15:45:00.185447 xmppy-0.2/README.md
+-rw-r--r--   0        0        0      434 2024-05-25 15:22:33.877571 xmppy-0.2/pyproject.toml
+-rw-r--r--   0        0        0     6485 2023-09-15 00:04:48.817265 xmppy-0.2/xmppy/Messenger.py
+-rw-r--r--   0        0        0       24 2023-09-15 00:04:48.817265 xmppy-0.2/xmppy/__init__.py
+-rw-r--r--   0        0        0     4680 2023-09-15 00:04:48.817265 xmppy-0.2/xmppy/gpg_holder.py
+-rw-r--r--   0        0        0     3899 1970-01-01 00:00:00.000000 xmppy-0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xmppy-0.11/README.md` & `xmppy-0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 
 ![tag](https://img.shields.io/github/tag-date/aszadzinski/xmppy.svg)
 ![commit](https://img.shields.io/github/last-commit/aszadzinski/xmppy.svg)
 ![license](https://img.shields.io/github/license/aszadzinski/xmppy.svg)
 
 ![status](https://img.shields.io/badge/build-passing-green.svg?style=flat&logo=Linux) ![status](https://img.shields.io/badge/build-falling-red.svg?style=flat&logo=Windows)
 
+**The repository is no longer being developed**
+
 Python module for receiving and sending message using XMPP protocol.
 
+**Requires python >=3.8, <3.10**
+
+**Attention**: Module DO NOT provide any layers of encryption. You use it at your own risk.
+
 Repos: [GitHub](https://github.com/aszadzinski/xmppy.git) [GitLab](https://gitlab.com/aszadzinski/xmppBot)
 
 ---
 
 ## Table of Contents
 
 - [Installation](#Installation)
@@ -33,32 +39,32 @@
 ---
 
 ## Installation
 
 
 ### From source
 
-``` python3 setup.py install```
-
-**Depedencies:**
-
-- sleekxmpp
-- python-gnupg
+```console
+# using poetry
+user@host:~$ poetry install 
+# using pip
+user@host:~$ pip install .
+```
 
 ### Using pip
 
-`pip install xmppy`
-
-or using .whl from [releases](https://github.com/aszadzinski/xmppy/releases):
-
-`pip install xmppy-XXX.whl`
+```console
+user@host:~$ pip install xmppy
+```
 
 ### AUR (TODO)
 
-`makepkg xmppy`
+```console
+user@host:~$ makepkg xmppy
+```
 
 ## Usage
 
 ### Sending and receiving messages
 
 #### example 1
 
@@ -115,15 +121,17 @@
 recipient = rece@examp.le
 ```
 
 and change function call from `.Client("jid@examp.le", "password", "recipient@examp.le", ...)`  to `.Client("file", "<.ini file>", <None or recipient@examp.le>, ...)`. Feature works with all calls from examples (1,2,3).
 
 ### Console script
 
-`xmppy -j <Jabber ID> -p <password> -t <recipient> -m <message>`
+```console
+user@host:~$ xmppy -j <Jabber ID> -p <password> -t <recipient> -m <message>
+```
 
 ---
 
 ### Encryption
 
 #### GPG
```

### Comparing `xmppy-0.11/xmppy/Messenger.py` & `xmppy-0.2/xmppy/Messenger.py`

 * *Files identical despite different names*

### Comparing `xmppy-0.11/xmppy/gpg_holder.py` & `xmppy-0.2/xmppy/gpg_holder.py`

 * *Files identical despite different names*

