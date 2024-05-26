# Comparing `tmp/btgitserver-1.0.5.tar.gz` & `tmp/btgitserver-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btgitserver-1.0.5.tar", last modified: Wed Jul 12 13:56:54 2023, max compression
+gzip compressed data, was "btgitserver-2.0.tar", last modified: Sun May 26 18:54:55 2024, max compression
```

## Comparing `btgitserver-1.0.5.tar` & `btgitserver-2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.325730 btgitserver-1.0.5/
--rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-1.0.5/.gitignore
--rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-1.0.5/Dockerfile
--rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-07-12 13:56:54.325963 btgitserver-1.0.5/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1730 2023-06-27 12:45:34.000000 btgitserver-1.0.5/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-07-12 13:56:33.000000 btgitserver-1.0.5/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.321282 btgitserver-1.0.5/btgitserver/
--rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-1.0.5/btgitserver/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     6117 2023-07-12 13:56:09.000000 btgitserver-1.0.5/btgitserver/app.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2206 2023-06-27 12:46:04.000000 btgitserver-1.0.5/btgitserver/args.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-1.0.5/btgitserver/config.py
--rw-r--r--   0 etejeda    (501) staff       (20)      595 2023-06-27 12:39:08.000000 btgitserver-1.0.5/btgitserver/defaults.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-1.0.5/btgitserver/logger.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.324490 btgitserver-1.0.5/btgitserver.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     2363 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)      455 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       52 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-1.0.5/btgitserver.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      173 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       12 2023-07-12 13:56:54.000000 btgitserver-1.0.5/btgitserver.egg-info/top_level.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-12 13:56:54.325016 btgitserver-1.0.5/etc/
--rwx------   0 etejeda    (501) staff       (20)      162 2023-06-27 17:44:31.000000 btgitserver-1.0.5/etc/config.yaml
--rw-r--r--   0 etejeda    (501) staff       (20)     1236 2023-07-12 13:56:54.326897 btgitserver-1.0.5/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-1.0.5/setup.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:54:55.280184 btgitserver-2.0/
+-rwx------   0 etejeda    (501) staff       (20)     1442 2023-06-25 15:47:07.000000 btgitserver-2.0/.gitignore
+-rwx------   0 etejeda    (501) staff       (20)      445 2019-11-19 14:59:57.000000 btgitserver-2.0/Dockerfile
+-rw-r--r--   0 etejeda    (501) staff       (20)     2891 2024-05-26 18:54:55.280534 btgitserver-2.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     2259 2024-05-26 06:26:27.000000 btgitserver-2.0/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        3 2024-05-26 06:22:32.000000 btgitserver-2.0/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:54:55.274318 btgitserver-2.0/btgitserver/
+-rw-r--r--   0 etejeda    (501) staff       (20)      214 2023-06-25 19:24:10.000000 btgitserver-2.0/btgitserver/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     8177 2024-05-26 06:20:33.000000 btgitserver-2.0/btgitserver/app.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2464 2024-05-26 06:22:14.000000 btgitserver-2.0/btgitserver/args.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1004 2023-06-25 15:50:24.000000 btgitserver-2.0/btgitserver/config.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      757 2024-05-26 06:05:54.000000 btgitserver-2.0/btgitserver/defaults.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1444 2023-06-25 19:36:10.000000 btgitserver-2.0/btgitserver/logger.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:54:55.278895 btgitserver-2.0/btgitserver.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2891 2024-05-26 18:54:54.000000 btgitserver-2.0/btgitserver.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)      455 2024-05-26 18:54:55.000000 btgitserver-2.0/btgitserver.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2024-05-26 18:54:54.000000 btgitserver-2.0/btgitserver.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       55 2024-05-26 18:54:54.000000 btgitserver-2.0/btgitserver.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-06-25 19:26:41.000000 btgitserver-2.0/btgitserver.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      173 2024-05-26 18:54:54.000000 btgitserver-2.0/btgitserver.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       12 2024-05-26 18:54:54.000000 btgitserver-2.0/btgitserver.egg-info/top_level.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2024-05-26 18:54:55.279413 btgitserver-2.0/etc/
+-rwx------   0 etejeda    (501) staff       (20)      197 2024-05-25 21:39:11.000000 btgitserver-2.0/etc/config.yaml
+-rw-r--r--   0 etejeda    (501) staff       (20)     1239 2024-05-26 18:54:55.282318 btgitserver-2.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)      780 2023-06-26 00:48:02.000000 btgitserver-2.0/setup.py
```

### Comparing `btgitserver-1.0.5/.gitignore` & `btgitserver-2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.5/PKG-INFO` & `btgitserver-2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.5
+Version: 2.0
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,74 +18,95 @@
 
 ## Overview
 
 A git server implementation written in python.
 
 Based off the amazing work by Stewart Park in this gist: [https://gist.github.com/stewartpark/1b079dc0481c6213def9](https://gist.github.com/stewartpark/1b079dc0481c6213def9).
 
-The app makes any git repository lying below the _search\_paths_ 
-available for `git clone` via HTTP using basic authentication.
+Features:
 
-Application defaults can be overridden by specifying a configuration file.
-
-Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
+- Makes any git repository lying below the _search\_paths_ setting
+  available for `git clone` and `git push` via HTTP using basic authentication
+- Application defaults can be overridden by specifying a configuration file<br />
+  Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
+- On-demand repos: If you attempt to push a non-existing repo to the server, it will be created 
 
 ## Installation
 
 - Install from pypi.org: `pip install btgitserver`
 - Install directly from git repo: `pip install git+http://www.github.com/berttejeda/bert.gt-server.git`
 
 ## Usage
 
-To get usage information and help: `git-server -h`
+To get usage information and help: `bt.git-server -h`
 
 ### Clone paths
 
-There are two routes accepted by the script:
+These are the routes accepted by the script:
+
+- '/<org_name>/<project_name>'
 
-- '/example/<project name>'
-- '/<project name>'
+These routes mirror the directory structure under the git search path(s).
 
-All resolve to the same underlying repository path.
+### Authentication
+  
+For now, the only authentication available is HTTP AUTH BASIC
 
-This effectively allows you to mock organizational structures.
+As such, the default credentials are:
 
-TODO: Define additional routes dynamically as opposed to hard-coding.
+Username: `git-user`
+Password: `git-password`
 
 ### Usage Examples
 
-Quick test:
+#### Clone a repo
 
-* Create a test repo:
+* Create a test org and repo:
 
 ```
-mkdir -p /tmp/repos/test
-cd /tmp/repos/test
+cd ~
+mkdir -p /tmp/repos/contoso/test
+cd /tmp/repos/contoso/test
 git init .
+git checkout -b main
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
-git-server -r /tmp/repos
+cd ~
+bt.git-server -r /tmp/repos
 ```
 
 **Note**: The `--repo-search-paths/-r` cli option allows specifying 
-multiple, space-delimitted search paths, e.g. `git-server -r /tmp/repos /tmp/repos2`
+multiple, space-delimitted search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
 
 * Launch the standalone git server
 
-`git-server`
+`bt.git-server`
 
 You should see output similar to:
 ```
 Running on http://0.0.0.0:5000/	
 ```
 
 * On client-side:
 
 Try cloning the repo you just created via the supported routes:
 
 e.g.
 	
 ```bash
-git clone http://127.0.0.1:5000/test.git
-git clone http://127.0.0.1:5000/example/test.git
+git clone http://git-user:git-password@127.0.0.1:5000/contoso/test
+```
+
+#### Push an on-demand repo
+
+```
+mkdir -p foo-bar
+cd foo-bar
+git init .
+git remote add origin http://git-user:git-password@127.0.0.1:5000/contoso/foo-bar
+git checkout -b main
+touch test_file.txt
+git add .
+git commit -m 'Initial Commit'
+git push --set-upstream origin $(git rev-parse --abbrev-ref HEAD)
 ```
```

### Comparing `btgitserver-1.0.5/README.md` & `btgitserver-2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,94 @@
 ## Overview
 
 A git server implementation written in python.
 
 Based off the amazing work by Stewart Park in this gist: [https://gist.github.com/stewartpark/1b079dc0481c6213def9](https://gist.github.com/stewartpark/1b079dc0481c6213def9).
 
-The app makes any git repository lying below the _search\_paths_ 
-available for `git clone` via HTTP using basic authentication.
+Features:
 
-Application defaults can be overridden by specifying a configuration file.
-
-Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
+- Makes any git repository lying below the _search\_paths_ setting
+  available for `git clone` and `git push` via HTTP using basic authentication
+- Application defaults can be overridden by specifying a configuration file<br />
+  Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
+- On-demand repos: If you attempt to push a non-existing repo to the server, it will be created 
 
 ## Installation
 
 - Install from pypi.org: `pip install btgitserver`
 - Install directly from git repo: `pip install git+http://www.github.com/berttejeda/bert.gt-server.git`
 
 ## Usage
 
-To get usage information and help: `git-server -h`
+To get usage information and help: `bt.git-server -h`
 
 ### Clone paths
 
-There are two routes accepted by the script:
+These are the routes accepted by the script:
+
+- '/<org_name>/<project_name>'
 
-- '/example/<project name>'
-- '/<project name>'
+These routes mirror the directory structure under the git search path(s).
 
-All resolve to the same underlying repository path.
+### Authentication
+  
+For now, the only authentication available is HTTP AUTH BASIC
 
-This effectively allows you to mock organizational structures.
+As such, the default credentials are:
 
-TODO: Define additional routes dynamically as opposed to hard-coding.
+Username: `git-user`
+Password: `git-password`
 
 ### Usage Examples
 
-Quick test:
+#### Clone a repo
 
-* Create a test repo:
+* Create a test org and repo:
 
 ```
-mkdir -p /tmp/repos/test
-cd /tmp/repos/test
+cd ~
+mkdir -p /tmp/repos/contoso/test
+cd /tmp/repos/contoso/test
 git init .
+git checkout -b main
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
-git-server -r /tmp/repos
+cd ~
+bt.git-server -r /tmp/repos
 ```
 
 **Note**: The `--repo-search-paths/-r` cli option allows specifying 
-multiple, space-delimitted search paths, e.g. `git-server -r /tmp/repos /tmp/repos2`
+multiple, space-delimitted search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
 
 * Launch the standalone git server
 
-`git-server`
+`bt.git-server`
 
 You should see output similar to:
 ```
 Running on http://0.0.0.0:5000/	
 ```
 
 * On client-side:
 
 Try cloning the repo you just created via the supported routes:
 
 e.g.
 	
 ```bash
-git clone http://127.0.0.1:5000/test.git
-git clone http://127.0.0.1:5000/example/test.git
+git clone http://git-user:git-password@127.0.0.1:5000/contoso/test
+```
+
+#### Push an on-demand repo
+
 ```
+mkdir -p foo-bar
+cd foo-bar
+git init .
+git remote add origin http://git-user:git-password@127.0.0.1:5000/contoso/foo-bar
+git checkout -b main
+touch test_file.txt
+git add .
+git commit -m 'Initial Commit'
+git push --set-upstream origin $(git rev-parse --abbrev-ref HEAD)
+```
```

### Comparing `btgitserver-1.0.5/btgitserver/args.py` & `btgitserver-2.0/btgitserver/args.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 from argparse import RawTextHelpFormatter
+from btgitserver import __version__
 from btgitserver.defaults import app_name
 
 def parse_args(**kwargs):
     parser = argparse.ArgumentParser(
         description="Standalone git server written in python",
         formatter_class=RawTextHelpFormatter,
         epilog="""
@@ -43,17 +44,19 @@
         "-w",
         "--workers",
         help="Override number of gunicorn workers",
         metavar="ARG", required=False)    
     parser.add_argument('--no-verify-tls', '-notls',action='store_true', help='Verify SSL cert when downloading web content')
     parser.add_argument('--config-file', '-f', help="Path to config file override")
     parser.add_argument('--repo-search-paths', '-r', nargs='+', help="List of directories containing git repositories")
+    parser.add_argument('--ondemand-repo-search-paths', '-odr', nargs='+', help="List of directories containing on-demand git repositories")
     parser.add_argument('--logfile-path', '-L', help="Path to logfile")
     parser.add_argument('--logfile-write-mode', '-Lw', default='w', choices=['a', 'w'], help="File mode when writing to log file, 'a' to append, 'w' to overwrite")    
     parser.add_argument('--debug', action='store_true')
+    parser.add_argument('--version', action='version', version=f'{__version__}')
     parser.add_argument(
         "-v",
         "--verbose",
         help="increase output verbosity",
         action="store_true")
     
     return parser.parse_args()
```

### Comparing `btgitserver-1.0.5/btgitserver/config.py` & `btgitserver-2.0/btgitserver/config.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.5/btgitserver/defaults.py` & `btgitserver-2.0/btgitserver/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 # Flask app settings
 debug = False
 app_name = "Python Git Server"
 default_app_port = 5000
 default_config_file_name = 'config.yaml'
 default_app_host_address = '0.0.0.0'
 default_repo_search_paths = ['~/repos']
-default_num_workers = 4
+default_ondemand_repo_search_paths = ['~/repos.ondemand']
+default_num_workers = 4 # not yet implemented
 default_settings = {
   "auth": {
     "users": {
       "git-user": {
         "password": "git-password"
       }
     }
   },
   "app": {
     "debug": debug,
     "listen": default_app_host_address,
     "port": default_app_port,
     "search_paths": default_repo_search_paths,
+    "ondemand": {
+      "search_paths": default_ondemand_repo_search_paths
+    },
     "workers": default_num_workers
   }
 }
```

### Comparing `btgitserver-1.0.5/btgitserver/logger.py` & `btgitserver-2.0/btgitserver/logger.py`

 * *Files identical despite different names*

### Comparing `btgitserver-1.0.5/btgitserver.egg-info/PKG-INFO` & `btgitserver-2.0/btgitserver.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btgitserver
-Version: 1.0.5
+Version: 2.0
 Summary: Python-based Git Server
 Home-page: https://github.com/berttejeda/bert.git-server
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: yaml,configuration,config,file,python,settings
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,74 +18,95 @@
 
 ## Overview
 
 A git server implementation written in python.
 
 Based off the amazing work by Stewart Park in this gist: [https://gist.github.com/stewartpark/1b079dc0481c6213def9](https://gist.github.com/stewartpark/1b079dc0481c6213def9).
 
-The app makes any git repository lying below the _search\_paths_ 
-available for `git clone` via HTTP using basic authentication.
+Features:
 
-Application defaults can be overridden by specifying a configuration file.
-
-Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
+- Makes any git repository lying below the _search\_paths_ setting
+  available for `git clone` and `git push` via HTTP using basic authentication
+- Application defaults can be overridden by specifying a configuration file<br />
+  Review [etc/config.yaml](etc/config.yaml) for a sample data structure.
+- On-demand repos: If you attempt to push a non-existing repo to the server, it will be created 
 
 ## Installation
 
 - Install from pypi.org: `pip install btgitserver`
 - Install directly from git repo: `pip install git+http://www.github.com/berttejeda/bert.gt-server.git`
 
 ## Usage
 
-To get usage information and help: `git-server -h`
+To get usage information and help: `bt.git-server -h`
 
 ### Clone paths
 
-There are two routes accepted by the script:
+These are the routes accepted by the script:
+
+- '/<org_name>/<project_name>'
 
-- '/example/<project name>'
-- '/<project name>'
+These routes mirror the directory structure under the git search path(s).
 
-All resolve to the same underlying repository path.
+### Authentication
+  
+For now, the only authentication available is HTTP AUTH BASIC
 
-This effectively allows you to mock organizational structures.
+As such, the default credentials are:
 
-TODO: Define additional routes dynamically as opposed to hard-coding.
+Username: `git-user`
+Password: `git-password`
 
 ### Usage Examples
 
-Quick test:
+#### Clone a repo
 
-* Create a test repo:
+* Create a test org and repo:
 
 ```
-mkdir -p /tmp/repos/test
-cd /tmp/repos/test
+cd ~
+mkdir -p /tmp/repos/contoso/test
+cd /tmp/repos/contoso/test
 git init .
+git checkout -b main
 touch test_file.txt
 git add .
 git commit -m 'Initial Commit'
-git-server -r /tmp/repos
+cd ~
+bt.git-server -r /tmp/repos
 ```
 
 **Note**: The `--repo-search-paths/-r` cli option allows specifying 
-multiple, space-delimitted search paths, e.g. `git-server -r /tmp/repos /tmp/repos2`
+multiple, space-delimitted search paths, e.g. `bt.git-server -r /tmp/repos /tmp/repos2`
 
 * Launch the standalone git server
 
-`git-server`
+`bt.git-server`
 
 You should see output similar to:
 ```
 Running on http://0.0.0.0:5000/	
 ```
 
 * On client-side:
 
 Try cloning the repo you just created via the supported routes:
 
 e.g.
 	
 ```bash
-git clone http://127.0.0.1:5000/test.git
-git clone http://127.0.0.1:5000/example/test.git
+git clone http://git-user:git-password@127.0.0.1:5000/contoso/test
+```
+
+#### Push an on-demand repo
+
+```
+mkdir -p foo-bar
+cd foo-bar
+git init .
+git remote add origin http://git-user:git-password@127.0.0.1:5000/contoso/foo-bar
+git checkout -b main
+touch test_file.txt
+git add .
+git commit -m 'Initial Commit'
+git push --set-upstream origin $(git rev-parse --abbrev-ref HEAD)
 ```
```

### Comparing `btgitserver-1.0.5/setup.cfg` & `btgitserver-2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 	pytest-cov
 	coveralls
 	flake8
 	mypy
 
 [options.entry_points]
 console_scripts = 
-	git-server=btgitserver.app:main
+	bt.git-server=btgitserver.app:main
 
 [options.data_files]
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `btgitserver-1.0.5/setup.py` & `btgitserver-2.0/setup.py`

 * *Files identical despite different names*

