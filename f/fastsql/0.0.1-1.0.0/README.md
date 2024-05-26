# Comparing `tmp/fastsql-0.0.1.tar.gz` & `tmp/fastsql-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsql-0.0.1.tar", last modified: Sun May 26 01:41:15 2024, max compression
+gzip compressed data, was "dist/fastsql-1.0.0.tar", last modified: Sat Sep  5 17:28:26 2020, max compression
```

## Comparing `fastsql-0.0.1.tar` & `fastsql-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-26 01:41:15.234724 fastsql-0.0.1/
--rw-rw-r--   0 jhoward    (501) staff       (20)    11337 2023-04-27 10:12:58.000000 fastsql-0.0.1/LICENSE
--rw-rw-r--   0 jhoward    (501) staff       (20)      111 2023-04-27 10:12:58.000000 fastsql-0.0.1/MANIFEST.in
--rw-r--r--   0 jhoward    (501) staff       (20)     2763 2024-05-26 01:41:15.234528 fastsql-0.0.1/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)     1917 2024-05-26 01:36:26.000000 fastsql-0.0.1/README.md
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-26 01:41:15.233039 fastsql-0.0.1/fastsql/
--rw-r--r--   0 jhoward    (501) staff       (20)       43 2024-05-26 01:21:51.000000 fastsql-0.0.1/fastsql/__init__.py
--rw-r--r--   0 jhoward    (501) staff       (20)     1355 2024-05-26 01:21:51.000000 fastsql-0.0.1/fastsql/_modidx.py
--rw-r--r--   0 jhoward    (501) staff       (20)     2293 2024-05-26 01:21:51.000000 fastsql-0.0.1/fastsql/core.py
-drwxr-xr-x   0 jhoward    (501) staff       (20)        0 2024-05-26 01:41:15.234282 fastsql-0.0.1/fastsql.egg-info/
--rw-r--r--   0 jhoward    (501) staff       (20)     2763 2024-05-26 01:41:15.000000 fastsql-0.0.1/fastsql.egg-info/PKG-INFO
--rw-r--r--   0 jhoward    (501) staff       (20)      324 2024-05-26 01:41:15.000000 fastsql-0.0.1/fastsql.egg-info/SOURCES.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-26 01:41:15.000000 fastsql-0.0.1/fastsql.egg-info/dependency_links.txt
--rw-r--r--   0 jhoward    (501) staff       (20)       36 2024-05-26 01:41:15.000000 fastsql-0.0.1/fastsql.egg-info/entry_points.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        1 2024-05-25 23:39:24.000000 fastsql-0.0.1/fastsql.egg-info/not-zip-safe
--rw-r--r--   0 jhoward    (501) staff       (20)       30 2024-05-26 01:41:15.000000 fastsql-0.0.1/fastsql.egg-info/requires.txt
--rw-r--r--   0 jhoward    (501) staff       (20)        8 2024-05-26 01:41:15.000000 fastsql-0.0.1/fastsql.egg-info/top_level.txt
--rw-r--r--   0 jhoward    (501) staff       (20)      879 2024-05-26 01:08:00.000000 fastsql-0.0.1/settings.ini
--rw-r--r--   0 jhoward    (501) staff       (20)       38 2024-05-26 01:41:15.234769 fastsql-0.0.1/setup.cfg
--rw-r--r--   0 jhoward    (501) staff       (20)     2606 2024-05-26 01:41:08.000000 fastsql-0.0.1/setup.py
+drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2020-09-05 17:28:26.000000 fastsql-1.0.0/
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2392 2020-09-05 17:28:26.000000 fastsql-1.0.0/PKG-INFO
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     1217 2019-11-15 20:17:59.000000 fastsql-1.0.0/README.md
+drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql/
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     1823 2020-09-05 17:08:49.000000 fastsql-1.0.0/fastsql/__init__.py
+drwxrwxr-x   0 jhoward   (1002) jhoward   (1002)        0 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2392 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/PKG-INFO
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)      256 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/SOURCES.txt
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        1 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/dependency_links.txt
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       20 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/entry_points.txt
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        1 2019-07-21 23:47:55.000000 fastsql-1.0.0/fastsql.egg-info/not-zip-safe
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       41 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/requires.txt
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)        8 2020-09-05 17:28:26.000000 fastsql-1.0.0/fastsql.egg-info/top_level.txt
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)       38 2020-09-05 17:28:26.000000 fastsql-1.0.0/setup.cfg
+-rw-rw-r--   0 jhoward   (1002) jhoward   (1002)     2516 2020-09-05 17:08:59.000000 fastsql-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `fastsql-0.0.1/setup.py` & `fastsql-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
-import setuptools, shlex
+import setuptools
+import re
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
-config.read('settings.ini', encoding='utf-8')
+config.read('settings.ini')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
-    'mit': ('MIT License', 'OSI Approved :: MIT License'),
-    'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
-    'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10 3.11 3.12'.split()
-
-requirements = shlex.split(cfg.get('requirements', ''))
-if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
+py_versions = '2.0 2.1 2.2 2.3 2.4 2.5 2.6 2.7 3.0 3.1 3.2 3.3 3.4 3.5 3.6 3.7 3.8'.split()
 min_python = cfg['min_python']
-lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
-dev_requirements = (cfg.get('dev_requirements') or '').split()
+lic = licenses[cfg['license']]
+
+requirements = ['pip', 'packaging']
+if cfg.get('requirements'): requirements += cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
+
+long_description = open('README.md').read()
+# ![png](docs/images/output_13_0.png)
+for ext in ['png', 'svg']:
+    long_description = re.sub(r'!\['+ext+'\]\((.*)\)', '!['+ext+']('+'https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1)', long_description)
+    long_description = re.sub(r'src=\"(.*)\.'+ext+'\"', 'src=\"https://raw.githubusercontent.com/{}/{}'.format(cfg['user'],cfg['lib_name'])+'/'+cfg['branch']+'/\\1.'+ext+'\"', long_description)
 
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
     classifiers = [
         'Development Status :: ' + statuses[int(cfg['status'])],
         'Intended Audience :: ' + cfg['audience'].title(),
+        'License :: ' + lic[1],
         'Natural Language :: ' + cfg['language'].title(),
-    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
-    url = cfg['git_url'],
+    ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]],
+    url = cfg['git_url'], 
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
-    extras_require={ 'dev': dev_requirements },
-    dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md', encoding='utf-8').read(),
+    long_description = long_description,
     long_description_content_type = 'text/markdown',
     zip_safe = False,
-    entry_points = {
-        'console_scripts': cfg.get('console_scripts','').split(),
-        'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
-    },
+    entry_points = { 'console_scripts': cfg.get('console_scripts','').split() },
     **setup_cfg)
 
-
```

