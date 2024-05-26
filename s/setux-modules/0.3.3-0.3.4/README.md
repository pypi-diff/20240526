# Comparing `tmp/setux_modules-0.3.3.tar.gz` & `tmp/setux_modules-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/setux_modules-0.3.3.tar", last modified: Sun Aug 30 07:07:30 2020, max compression
+gzip compressed data, was "dist/setux_modules-0.3.4.tar", last modified: Sun Aug 30 18:33:10 2020, max compression
```

## Comparing `setux_modules-0.3.3.tar` & `setux_modules-0.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 07:07:30.000000 setux_modules-0.3.3/
--rw-r--r--   0 louis     (4444) louis     (4444)     1012 2020-08-30 07:07:30.000000 setux_modules-0.3.3/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      141 2020-08-09 08:26:44.000000 setux_modules-0.3.3/README.rst
--rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setup.cfg
--rw-r--r--   0 louis     (4444) louis     (4444)     1231 2020-08-30 07:06:28.000000 setux_modules-0.3.3/setup.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux/
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux/modules/
--rw-r--r--   0 louis     (4444) louis     (4444)      566 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/admin.py
--rw-r--r--   0 louis     (4444) louis     (4444)      687 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/copy_id.py
--rwxr-xr-x   0 louis     (4444) louis     (4444)     1185 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/download.py
--rwxr-xr-x   0 louis     (4444) louis     (4444)      834 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/infos.py
--rwxr-xr-x   0 louis     (4444) louis     (4444)      895 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/ping.py
--rw-r--r--   0 louis     (4444) louis     (4444)      525 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/ssh_init.py
--rw-r--r--   0 louis     (4444) louis     (4444)      520 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/ssh_prod.py
--rw-r--r--   0 louis     (4444) louis     (4444)      614 2020-08-30 07:04:47.000000 setux_modules-0.3.3/setux/modules/sudoers.py
-drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux_modules.egg-info/
--rw-r--r--   0 louis     (4444) louis     (4444)     1012 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux_modules.egg-info/PKG-INFO
--rw-r--r--   0 louis     (4444) louis     (4444)      409 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux_modules.egg-info/SOURCES.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux_modules.egg-info/dependency_links.txt
--rw-r--r--   0 louis     (4444) louis     (4444)       18 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux_modules.egg-info/requires.txt
--rw-r--r--   0 louis     (4444) louis     (4444)        6 2020-08-30 07:07:30.000000 setux_modules-0.3.3/setux_modules.egg-info/top_level.txt
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:33:10.000000 setux_modules-0.3.4/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1012 2020-08-30 18:33:10.000000 setux_modules-0.3.4/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      141 2020-08-09 08:26:44.000000 setux_modules-0.3.4/README.rst
+-rw-r--r--   0 louis     (4444) louis     (4444)       80 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setup.cfg
+-rw-r--r--   0 louis     (4444) louis     (4444)     1231 2020-08-30 17:54:24.000000 setux_modules-0.3.4/setup.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux/
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux/modules/
+-rw-r--r--   0 louis     (4444) louis     (4444)      566 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/admin.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      687 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/copy_id.py
+-rwxr-xr-x   0 louis     (4444) louis     (4444)     1185 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/download.py
+-rwxr-xr-x   0 louis     (4444) louis     (4444)      834 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/infos.py
+-rwxr-xr-x   0 louis     (4444) louis     (4444)      881 2020-08-30 17:54:24.000000 setux_modules-0.3.4/setux/modules/ping.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      525 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/ssh_init.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      520 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/ssh_prod.py
+-rw-r--r--   0 louis     (4444) louis     (4444)      614 2020-08-30 07:07:40.000000 setux_modules-0.3.4/setux/modules/sudoers.py
+drwxr-xr-x   0 louis     (4444) louis     (4444)        0 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux_modules.egg-info/
+-rw-r--r--   0 louis     (4444) louis     (4444)     1012 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux_modules.egg-info/PKG-INFO
+-rw-r--r--   0 louis     (4444) louis     (4444)      409 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        1 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)       18 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux_modules.egg-info/requires.txt
+-rw-r--r--   0 louis     (4444) louis     (4444)        6 2020-08-30 18:33:10.000000 setux_modules-0.3.4/setux_modules.egg-info/top_level.txt
```

### Comparing `setux_modules-0.3.3/PKG-INFO` & `setux_modules-0.3.4/setux_modules.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: setux_modules
-Version: 0.3.3
+Name: setux-modules
+Version: 0.3.4
 Summary: System deployment
 Home-page: https://gitlab.com/dugres/setux_modules
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

### Comparing `setux_modules-0.3.3/setup.py` & `setux_modules-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_namespace_packages
 
 curdir = abspath(dirname(__file__))
 readme = open(join(curdir, 'README.rst')).read()
 
 setup(
     name             = 'setux_modules',
-    version          = '0.3.3',
+    version          = '0.3.4',
     description      = 'System deployment',
     long_description = readme,
     keywords         = ['utility', ],
     url              = 'https://gitlab.com/dugres/setux_modules',
     author           = 'Louis RIVIERE',
     author_email     = 'louis@riviere.xyz',
     license          = 'MIT',
```

### Comparing `setux_modules-0.3.3/setux/modules/admin.py` & `setux_modules-0.3.4/setux/modules/admin.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux/modules/copy_id.py` & `setux_modules-0.3.4/setux/modules/copy_id.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux/modules/download.py` & `setux_modules-0.3.4/setux/modules/download.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux/modules/infos.py` & `setux_modules-0.3.4/setux/modules/infos.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux/modules/ping.py` & `setux_modules-0.3.4/setux/modules/ping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from setux.core.module import Module
 
 
-def ping(target, pong='pong'):
-    ret, out, err = target.run('echo', pong)
-    response = out[0]
-    return response==pong
-
-
 class Distro(Module):
     '''Check Target Reachability
     '''
     def deploy(self, target, **kw):
-        return ping(target, pong=kw.get('pong'))
+        pong = kw.get('pong', 'pong')
+        ret, out, err = target.run('echo', pong, report='verbose')
+        response = out[0]
+        return response==pong
 
 
 class debian_9(Distro):
     def deploy(self, target, **kw):
         return super().deploy(target, pong='Debian 9')
```

### Comparing `setux_modules-0.3.3/setux/modules/ssh_init.py` & `setux_modules-0.3.4/setux/modules/ssh_init.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux/modules/ssh_prod.py` & `setux_modules-0.3.4/setux/modules/ssh_prod.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux/modules/sudoers.py` & `setux_modules-0.3.4/setux/modules/sudoers.py`

 * *Files identical despite different names*

### Comparing `setux_modules-0.3.3/setux_modules.egg-info/PKG-INFO` & `setux_modules-0.3.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
-Name: setux-modules
-Version: 0.3.3
+Name: setux_modules
+Version: 0.3.4
 Summary: System deployment
 Home-page: https://gitlab.com/dugres/setux_modules
 Author: Louis RIVIERE
 Author-email: louis@riviere.xyz
 License: MIT
 Description: ########
          setux
```

