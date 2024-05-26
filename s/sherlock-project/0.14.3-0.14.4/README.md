# Comparing `tmp/sherlock_project-0.14.3.tar.gz` & `tmp/sherlock_project-0.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherlock_project-0.14.3.tar", last modified: Mon May 13 04:19:57 2024, max compression
+gzip compressed data, was "sherlock_project-0.14.4.tar", last modified: Sun May 26 08:46:12 2024, max compression
```

## Comparing `sherlock_project-0.14.3.tar` & `sherlock_project-0.14.4.tar`

### file list

```diff
@@ -1,33 +1,32 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.839317 sherlock_project-0.14.3/
--rw-r--r--   0 paul      (1000) paul      (1000)     1073 2024-04-07 22:08:31.000000 sherlock_project-0.14.3/LICENSE
--rw-r--r--   0 paul      (1000) paul      (1000)     3099 2024-05-13 04:19:57.839317 sherlock_project-0.14.3/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7132 2024-05-13 03:45:16.000000 sherlock_project-0.14.3/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.834317 sherlock_project-0.14.3/docs/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.836317 sherlock_project-0.14.3/docs/pyproj/
--rw-r--r--   0 paul      (1000) paul      (1000)     1801 2024-05-13 04:15:27.000000 sherlock_project-0.14.3/docs/pyproj/README.md
--rw-r--r--   0 paul      (1000) paul      (1000)     1430 2024-05-13 04:14:56.000000 sherlock_project-0.14.3/pyproject.toml
--rw-r--r--   0 paul      (1000) paul      (1000)      167 2024-05-13 03:45:16.000000 sherlock_project-0.14.3/requirements.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      133 2024-05-13 04:19:57.839317 sherlock_project-0.14.3/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)      136 2024-05-13 03:45:16.000000 sherlock_project-0.14.3/setup.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.837317 sherlock_project-0.14.3/sherlock/
--rw-r--r--   0 paul      (1000) paul      (1000)      106 2024-04-07 22:08:31.000000 sherlock_project-0.14.3/sherlock/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)      537 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/__main__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9034 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/notify.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.837317 sherlock_project-0.14.3/sherlock/resources/
--rw-r--r--   0 paul      (1000) paul      (1000)    87973 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/resources/data.json
--rw-r--r--   0 paul      (1000) paul      (1000)     3228 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/resources/data.schema.json
--rw-r--r--   0 paul      (1000) paul      (1000)     3184 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/result.py
--rw-r--r--   0 paul      (1000) paul      (1000)    32322 2024-05-13 04:19:40.000000 sherlock_project-0.14.3/sherlock/sherlock.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.839317 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     3099 2024-05-13 04:19:57.000000 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)      684 2024-05-13 04:19:57.000000 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-05-13 04:19:57.000000 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       43 2024-05-13 04:19:57.000000 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/entry_points.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-13 04:19:57.000000 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       63 2024-05-13 04:19:57.000000 sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/top_level.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     9370 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/sites.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-13 04:19:57.839317 sherlock_project-0.14.3/sherlock/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)       87 2024-04-07 22:08:31.000000 sherlock_project-0.14.3/sherlock/tests/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7164 2024-05-12 04:25:04.000000 sherlock_project-0.14.3/sherlock/tests/all.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8588 2024-04-07 22:08:31.000000 sherlock_project-0.14.3/sherlock/tests/base.py
--rw-r--r--   0 paul      (1000) paul      (1000)      930 2024-04-07 22:08:31.000000 sherlock_project-0.14.3/sherlock/tests/test_multiple_usernames.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.725094 sherlock_project-0.14.4/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1073 2024-04-07 22:08:31.000000 sherlock_project-0.14.4/LICENSE
+-rw-r--r--   0 paul      (1000) paul      (1000)     3157 2024-05-26 08:46:12.725094 sherlock_project-0.14.4/PKG-INFO
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.720094 sherlock_project-0.14.4/docs/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.721094 sherlock_project-0.14.4/docs/pyproj/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1801 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/docs/pyproj/README.md
+-rw-r--r--   0 paul      (1000) paul      (1000)     1435 2024-05-26 08:45:47.000000 sherlock_project-0.14.4/pyproject.toml
+-rw-r--r--   0 paul      (1000) paul      (1000)      167 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/requirements.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      133 2024-05-26 08:46:12.725094 sherlock_project-0.14.4/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)      136 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.722094 sherlock_project-0.14.4/sherlock/
+-rw-r--r--   0 paul      (1000) paul      (1000)      106 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      537 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/__main__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9034 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/notify.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.723094 sherlock_project-0.14.4/sherlock/resources/
+-rw-r--r--   0 paul      (1000) paul      (1000)    88033 2024-05-20 20:19:35.000000 sherlock_project-0.14.4/sherlock/resources/data.json
+-rw-r--r--   0 paul      (1000) paul      (1000)     3228 2024-05-16 03:28:52.000000 sherlock_project-0.14.4/sherlock/resources/data.schema.json
+-rw-r--r--   0 paul      (1000) paul      (1000)     3184 2024-05-16 03:28:52.000000 sherlock_project-0.14.4/sherlock/result.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    32360 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/sherlock.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.725094 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3157 2024-05-26 08:46:12.000000 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)      674 2024-05-26 08:46:12.000000 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-05-26 08:46:12.000000 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       43 2024-05-26 08:46:12.000000 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/entry_points.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-26 08:46:12.000000 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       63 2024-05-26 08:46:12.000000 sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/top_level.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     9370 2024-05-22 19:31:16.000000 sherlock_project-0.14.4/sherlock/sites.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-26 08:46:12.724094 sherlock_project-0.14.4/sherlock/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)       87 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/tests/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7164 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/tests/all.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8588 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/tests/base.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      930 2024-05-25 08:36:12.000000 sherlock_project-0.14.4/sherlock/tests/test_multiple_usernames.py
```

### Comparing `sherlock_project-0.14.3/LICENSE` & `sherlock_project-0.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/PKG-INFO` & `sherlock_project-0.14.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sherlock-project
-Version: 0.14.3
+Version: 0.14.4
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/
-Author: Siddharth Dushantha
-Maintainer: Matheus Felipe, Sondre Karlsen Dyrnes, Paul Pfeister
+Author: Sherlock Project
+Author-email: Siddharth Dushantha <siddharth.dushantha@gmail.com>
+Maintainer-email: Paul Pfeister <pypi-contact@pfeister.dev>
 License: MIT
 Project-URL: Homepage, http://sherlock-project.github.io/
 Project-URL: Repository, https://github.com/sherlock-project/sherlock.git
 Project-URL: Issues, https://github.com/sherlock-project/sherlock/issues
 Keywords: osint,reconnaissance,information gathering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: sherlock-project Version: 0.14.3 Summary: Hunt down
+Metadata-Version: 2.1 Name: sherlock-project Version: 0.14.4 Summary: Hunt down
 social media accounts by username across social networks Home-page: http://
-sherlock-project.github.io/ Author: Siddharth Dushantha Maintainer: Matheus
-Felipe, Sondre Karlsen Dyrnes, Paul Pfeister License: MIT Project-URL:
-Homepage, http://sherlock-project.github.io/ Project-URL: Repository, https://
-github.com/sherlock-project/sherlock.git Project-URL: Issues, https://
-github.com/sherlock-project/sherlock/issues Keywords:
-osint,reconnaissance,information gathering Classifier: Development Status :: 5
-- Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Information Technology Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Security Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1
-Requires-Dist: PySocks>=1.7.0 Requires-Dist: requests>=2.22.0 Requires-Dist:
-requests-futures>=1.0.0 Requires-Dist: stem>=1.8.0 Requires-Dist:
-torrequest>=0.1.0 Requires-Dist: pandas>=1.0.0 Requires-Dist: openpyxl>=3.0.10
-Requires-Dist: exrex>=0.11.0
+sherlock-project.github.io/ Author: Sherlock Project Author-email: Siddharth
+Dushantha
+gmail.com> Maintainer-email: Paul Pfeister
+pfeister.dev> License: MIT Project-URL: Homepage, http://sherlock-
+project.github.io/ Project-URL: Repository, https://github.com/sherlock-
+project/sherlock.git Project-URL: Issues, https://github.com/sherlock-project/
+sherlock/issues Keywords: osint,reconnaissance,information gathering
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Security Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1 Requires-Dist: PySocks>=1.7.0
+Requires-Dist: requests>=2.22.0 Requires-Dist: requests-futures>=1.0.0
+Requires-Dist: stem>=1.8.0 Requires-Dist: torrequest>=0.1.0 Requires-Dist:
+pandas>=1.0.0 Requires-Dist: openpyxl>=3.0.10 Requires-Dist: exrex>=0.11.0
 
   _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_2_7_0_6_5_6_4_6_/_5_3_5_5_1_9_6_0_-_a_e_4_d_f_f_8_0_-_3_b_3_a_-
                           _1_1_e_9_-_9_0_7_5_-_c_e_f_7_8_6_c_6_9_3_6_4_._p_n_g_]
       Hunt down social media accounts by username across _s_o_c_i_a_l_ _n_e_t_w_o_r_k_s
         Additional documentation can be found on our _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y
  [https://user-images.githubusercontent.com/27065646/219638267-a5e11090-aa6e-
                           4e77-87f7-0e95f6ad5978.png]
```

### Comparing `sherlock_project-0.14.3/docs/pyproj/README.md` & `sherlock_project-0.14.4/docs/pyproj/README.md`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/pyproject.toml` & `sherlock_project-0.14.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 Homepage = "http://sherlock-project.github.io/"
 Repository = "https://github.com/sherlock-project/sherlock.git"
 Issues = "https://github.com/sherlock-project/sherlock/issues"
 
 [project]
 name = "sherlock-project"
 authors = [
-    { name = "Siddharth Dushantha" }
+    { name = "Siddharth Dushantha", email = "siddharth.dushantha@gmail.com" }
 ]
 maintainers = [
-    { name = "Matheus Felipe" },
-    { name = "Sondre Karlsen Dyrnes" },
-    { name = "Paul Pfeister" }
+    { name = "Paul Pfeister", email = "pypi-contact@pfeister.dev" }
 ]
 description = "Hunt down social media accounts by username across social networks"
 readme = "docs/pyproj/README.md"
 # Do not set license to file. Causes issues with rpm packaging for some reason.
 license = {text = "MIT"}
 dynamic = ["dependencies", "version"]
 keywords = [ "osint", "reconnaissance", "information gathering" ]
```

### Comparing `sherlock_project-0.14.3/sherlock/__main__.py` & `sherlock_project-0.14.4/sherlock/__main__.py`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/notify.py` & `sherlock_project-0.14.4/sherlock/notify.py`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/resources/data.json` & `sherlock_project-0.14.4/sherlock/resources/data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998249299719888%*

 * *Differences: {"'Kick'": "{'__comment__': 'Cloudflare. Only viable when proxied.'}"}*

```diff
@@ -1209,14 +1209,15 @@
     "Keybase": {
         "errorType": "status_code",
         "url": "https://keybase.io/{}",
         "urlMain": "https://keybase.io/",
         "username_claimed": "blue"
     },
     "Kick": {
+        "__comment__": "Cloudflare. Only viable when proxied.",
         "errorMsg": "Not Found",
         "errorType": "message",
         "url": "https://kick.com/{}",
         "urlMain": "https://kick.com/",
         "urlProbe": "https://kick.com/api/v2/channels/{}",
         "username_claimed": "blue"
     },
```

### Comparing `sherlock_project-0.14.3/sherlock/resources/data.schema.json` & `sherlock_project-0.14.4/sherlock/resources/data.schema.json`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/result.py` & `sherlock_project-0.14.4/sherlock/result.py`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/sherlock.py` & `sherlock_project-0.14.4/sherlock/sherlock.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from result import QueryResult
 from notify import QueryNotifyPrint
 from sites import SitesInformation
 from colorama import init
 from argparse import ArgumentTypeError
 
 module_name = "Sherlock: Find Usernames Across Social Networks"
-__version__ = "0.14.3"
+__version__ = "0.14.4"
 
 
 class SherlockFuturesSession(FuturesSession):
     def request(self, method, url, hooks=None, *args, **kwargs):
         """Request URL.
 
         This extends the FuturesSession request method to calculate a response
@@ -196,15 +196,20 @@
     """
 
     # Notify caller that we are starting the query.
     query_notify.start(username)
     # Create session based on request methodology
     if tor or unique_tor:
         # Requests using Tor obfuscation
-        underlying_request = TorRequest()
+        try:
+            underlying_request = TorRequest()
+        except OSError:
+            print("Tor not found in system path. Unable to continue.\n")
+            sys.exit(query_notify.finish())
+
         underlying_session = underlying_request.session
     else:
         # Normal requests
         underlying_session = requests.session()
         underlying_request = requests.Request()
 
     # Limit number of workers to 20.
@@ -373,19 +378,21 @@
             response_text = r.text.encode(r.encoding or "UTF-8")
         except Exception:
             response_text = ""
 
         query_status = QueryStatus.UNKNOWN
         error_context = None
 
-        # As WAFs advance and evolve, they will occasionally block Sherlock and lead to false positives
-        # and negatives. Fingerprints should be added here to filter results that fail to bypass WAFs.
-        # Fingerprints should be highly targetted. Comment at the end of each fingerprint to indicate target and date.
+        # As WAFs advance and evolve, they will occasionally block Sherlock and
+        # lead to false positives and negatives. Fingerprints should be added
+        # here to filter results that fail to bypass WAFs. Fingerprints should
+        # be highly targetted. Comment at the end of each fingerprint to
+        # indicate target and date fingerprinted.
         WAFHitMsgs = [
-            '.loading-spinner{visibility:hidden}body.no-js .challenge-running{display:none}body.dark{background-color:#222;color:#d9d9d9}body.dark a{color:#fff}body.dark a:hover{color:#ee730a;text-decoration:underline}body.dark .lds-ring div{border-color:#999 transparent transparent}body.dark .font-red{color:#b20f03}body.dark .big-button,body.dark .pow-button{background-color:#4693ff;color:#1d1d1d}body.dark #challenge-success-text{background-image:url(data:image/svg+xml;base64,', # 2024-04-08 Cloudflare
+            '.loading-spinner{visibility:hidden}body.no-js .challenge-running{display:none}body.dark{background-color:#222;color:#d9d9d9}body.dark a{color:#fff}body.dark a:hover{color:#ee730a;text-decoration:underline}body.dark .lds-ring div{border-color:#999 transparent transparent}body.dark .font-red{color:#b20f03}body.dark', # 2024-05-13 Cloudflare
             '{return l.onPageView}}),Object.defineProperty(r,"perimeterxIdentifiers",{enumerable:' # 2024-04-09 PerimeterX / Human Security
         ]
 
         if error_text is not None:
             error_context = error_text
 
         elif any(hitMsg in r.text for hitMsg in WAFHitMsgs):
```

### Comparing `sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/PKG-INFO` & `sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sherlock-project
-Version: 0.14.3
+Version: 0.14.4
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/
-Author: Siddharth Dushantha
-Maintainer: Matheus Felipe, Sondre Karlsen Dyrnes, Paul Pfeister
+Author: Sherlock Project
+Author-email: Siddharth Dushantha <siddharth.dushantha@gmail.com>
+Maintainer-email: Paul Pfeister <pypi-contact@pfeister.dev>
 License: MIT
 Project-URL: Homepage, http://sherlock-project.github.io/
 Project-URL: Repository, https://github.com/sherlock-project/sherlock.git
 Project-URL: Issues, https://github.com/sherlock-project/sherlock/issues
 Keywords: osint,reconnaissance,information gathering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: sherlock-project Version: 0.14.3 Summary: Hunt down
+Metadata-Version: 2.1 Name: sherlock-project Version: 0.14.4 Summary: Hunt down
 social media accounts by username across social networks Home-page: http://
-sherlock-project.github.io/ Author: Siddharth Dushantha Maintainer: Matheus
-Felipe, Sondre Karlsen Dyrnes, Paul Pfeister License: MIT Project-URL:
-Homepage, http://sherlock-project.github.io/ Project-URL: Repository, https://
-github.com/sherlock-project/sherlock.git Project-URL: Issues, https://
-github.com/sherlock-project/sherlock/issues Keywords:
-osint,reconnaissance,information gathering Classifier: Development Status :: 5
-- Production/Stable Classifier: Intended Audience :: Developers Classifier:
-Intended Audience :: Information Technology Classifier: License :: OSI Approved
-:: MIT License Classifier: Natural Language :: English Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Security Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1
-Requires-Dist: PySocks>=1.7.0 Requires-Dist: requests>=2.22.0 Requires-Dist:
-requests-futures>=1.0.0 Requires-Dist: stem>=1.8.0 Requires-Dist:
-torrequest>=0.1.0 Requires-Dist: pandas>=1.0.0 Requires-Dist: openpyxl>=3.0.10
-Requires-Dist: exrex>=0.11.0
+sherlock-project.github.io/ Author: Sherlock Project Author-email: Siddharth
+Dushantha
+gmail.com> Maintainer-email: Paul Pfeister
+pfeister.dev> License: MIT Project-URL: Homepage, http://sherlock-
+project.github.io/ Project-URL: Repository, https://github.com/sherlock-
+project/sherlock.git Project-URL: Issues, https://github.com/sherlock-project/
+sherlock/issues Keywords: osint,reconnaissance,information gathering
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Security Description-
+Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1 Requires-Dist: PySocks>=1.7.0
+Requires-Dist: requests>=2.22.0 Requires-Dist: requests-futures>=1.0.0
+Requires-Dist: stem>=1.8.0 Requires-Dist: torrequest>=0.1.0 Requires-Dist:
+pandas>=1.0.0 Requires-Dist: openpyxl>=3.0.10 Requires-Dist: exrex>=0.11.0
 
   _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_2_7_0_6_5_6_4_6_/_5_3_5_5_1_9_6_0_-_a_e_4_d_f_f_8_0_-_3_b_3_a_-
                           _1_1_e_9_-_9_0_7_5_-_c_e_f_7_8_6_c_6_9_3_6_4_._p_n_g_]
       Hunt down social media accounts by username across _s_o_c_i_a_l_ _n_e_t_w_o_r_k_s
         Additional documentation can be found on our _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y
  [https://user-images.githubusercontent.com/27065646/219638267-a5e11090-aa6e-
                           4e77-87f7-0e95f6ad5978.png]
```

### Comparing `sherlock_project-0.14.3/sherlock/sherlock_project.egg-info/SOURCES.txt` & `sherlock_project-0.14.4/sherlock/sherlock_project.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 docs/pyproj/README.md
 sherlock/__init__.py
 sherlock/__main__.py
```

### Comparing `sherlock_project-0.14.3/sherlock/sites.py` & `sherlock_project-0.14.4/sherlock/sites.py`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/tests/all.py` & `sherlock_project-0.14.4/sherlock/tests/all.py`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/tests/base.py` & `sherlock_project-0.14.4/sherlock/tests/base.py`

 * *Files identical despite different names*

### Comparing `sherlock_project-0.14.3/sherlock/tests/test_multiple_usernames.py` & `sherlock_project-0.14.4/sherlock/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

