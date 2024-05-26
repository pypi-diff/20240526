# Comparing `tmp/direnumerate-4.0a5.tar.gz` & `tmp/direnumerate-4.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-4.0a5.tar", last modified: Thu May 23 16:55:55 2024, max compression
+gzip compressed data, was "direnumerate-4.0a6.tar", last modified: Sun May 26 15:50:14 2024, max compression
```

## Comparing `direnumerate-4.0a5.tar` & `direnumerate-4.0a6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-23 16:55:55.331773 direnumerate-4.0a5/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-23 14:34:30.000000 direnumerate-4.0a5/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3286 2024-05-23 16:55:55.331773 direnumerate-4.0a5/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1861 2024-05-23 16:36:50.000000 direnumerate-4.0a5/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-23 16:55:55.327773 direnumerate-4.0a5/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      421 2024-05-23 16:36:50.000000 direnumerate-4.0a5/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     7927 2024-05-23 16:51:23.000000 direnumerate-4.0a5/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-23 14:34:30.000000 direnumerate-4.0a5/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2619 2024-05-23 16:52:22.000000 direnumerate-4.0a5/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-23 14:34:30.000000 direnumerate-4.0a5/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-23 14:34:30.000000 direnumerate-4.0a5/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-23 14:34:30.000000 direnumerate-4.0a5/direnumerate/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-23 14:34:30.000000 direnumerate-4.0a5/direnumerate/help.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2021 2024-05-23 16:36:50.000000 direnumerate-4.0a5/direnumerate/port_scan.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       73 2024-05-23 16:52:52.000000 direnumerate-4.0a5/direnumerate/version.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-23 14:34:30.000000 direnumerate-4.0a5/direnumerate/warning.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-23 16:55:55.331773 direnumerate-4.0a5/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3286 2024-05-23 16:55:55.000000 direnumerate-4.0a5/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-23 16:55:55.000000 direnumerate-4.0a5/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-23 16:55:55.000000 direnumerate-4.0a5/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-23 16:55:55.000000 direnumerate-4.0a5/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-23 16:55:55.000000 direnumerate-4.0a5/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-23 16:55:55.000000 direnumerate-4.0a5/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1567 2024-05-23 16:52:28.000000 direnumerate-4.0a5/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-23 16:55:55.331773 direnumerate-4.0a5/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-26 15:50:14.919219 direnumerate-4.0a6/
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-26 15:20:14.000000 direnumerate-4.0a6/LICENSE
+-rw-r--r--   0 juan      (1000) juan      (1000)     3281 2024-05-26 15:50:14.919219 direnumerate-4.0a6/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1856 2024-05-26 15:45:06.000000 direnumerate-4.0a6/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-26 15:50:14.919219 direnumerate-4.0a6/direnumerate/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      421 2024-05-26 15:22:27.000000 direnumerate-4.0a6/direnumerate/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     7889 2024-05-26 15:46:43.000000 direnumerate-4.0a6/direnumerate/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      125 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/banner.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2605 2024-05-26 15:47:09.000000 direnumerate-4.0a6/direnumerate/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      394 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/colors.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    23461 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/createlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      229 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      981 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/help.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2021 2024-05-26 15:22:27.000000 direnumerate-4.0a6/direnumerate/port_scan.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       73 2024-05-26 15:24:55.000000 direnumerate-4.0a6/direnumerate/version.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      334 2024-05-26 15:20:14.000000 direnumerate-4.0a6/direnumerate/warning.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-26 15:50:14.919219 direnumerate-4.0a6/direnumerate.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     3281 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      515 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       55 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       13 2024-05-26 15:50:14.000000 direnumerate-4.0a6/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1567 2024-05-26 15:25:02.000000 direnumerate-4.0a6/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-26 15:50:14.919219 direnumerate-4.0a6/setup.cfg
```

### Comparing `direnumerate-4.0a5/LICENSE` & `direnumerate-4.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a5/PKG-INFO` & `direnumerate-4.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a5
+Version: 4.0a6
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -84,22 +84,24 @@
 
 from direnumerate import Scan
 
 url = "testphp.vulnweb.com"
 wordlist = "wordlist.txt"
 
 enum = Scan(url)
-print(enum.show_dirs(wordlist))
+print(enum.dirs(wordlist))
 ```
 ----------
 
 ### Port Scan:
 
 ```python
 
 from direnumerate import Scan
 
-enum = Scan()
-print(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25]))
+ip = '44.228.249.3'
+
+enum = Scan(ip)
+print(enum.ports(ports=[22, 443, 8080, 8280, 80, 25]))
 
 ```
 ----------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a5 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a6 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -34,11 +34,10 @@
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
 t 44.228.249.3 -p 22 80 443 ## Scripts usage: ### Directory Scan in Websites:
 ```python from direnumerate import Scan url = "testphp.vulnweb.com" wordlist =
-"wordlist.txt" enum = Scan(url) print(enum.show_dirs(wordlist)) ``` ---------
-- ### Port Scan: ```python from direnumerate import Scan enum = Scan() print
-(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25])) ``` --
---------
+"wordlist.txt" enum = Scan(url) print(enum.dirs(wordlist)) ``` ---------- ###
+Port Scan: ```python from direnumerate import Scan ip = '44.228.249.3' enum =
+Scan(ip) print(enum.ports(ports=[22, 443, 8080, 8280, 80, 25])) ``` ----------
```

### Comparing `direnumerate-4.0a5/README.md` & `direnumerate-4.0a6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,22 +51,24 @@
 
 from direnumerate import Scan
 
 url = "testphp.vulnweb.com"
 wordlist = "wordlist.txt"
 
 enum = Scan(url)
-print(enum.show_dirs(wordlist))
+print(enum.dirs(wordlist))
 ```
 ----------
 
 ### Port Scan:
 
 ```python
 
 from direnumerate import Scan
 
-enum = Scan()
-print(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25]))
+ip = '44.228.249.3'
+
+enum = Scan(ip)
+print(enum.ports(ports=[22, 443, 8080, 8280, 80, 25]))
 
 ```
 ----------
```

#### html2text {}

```diff
@@ -14,11 +14,10 @@
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
 t 44.228.249.3 -p 22 80 443 ## Scripts usage: ### Directory Scan in Websites:
 ```python from direnumerate import Scan url = "testphp.vulnweb.com" wordlist =
-"wordlist.txt" enum = Scan(url) print(enum.show_dirs(wordlist)) ``` ---------
-- ### Port Scan: ```python from direnumerate import Scan enum = Scan() print
-(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25])) ``` --
---------
+"wordlist.txt" enum = Scan(url) print(enum.dirs(wordlist)) ``` ---------- ###
+Port Scan: ```python from direnumerate import Scan ip = '44.228.249.3' enum =
+Scan(ip) print(enum.ports(ports=[22, 443, 8080, 8280, 80, 25])) ``` ----------
```

### Comparing `direnumerate-4.0a5/direnumerate/__main__.py` & `direnumerate-4.0a6/direnumerate/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 self.url = url
             else:
                 self.url = "https://" + url
                 
         except IndexError:
             raise exception.DirenumerateError("[error] expected an argument")
 
-    def show_dirs(self, 
+    def dirs(self, 
                  wordlist_file, 
                  verbose_only_found: bool = False,
                  verbose: bool = False
                  ) -> list:
         """
         Perform directory enumeration.
 
@@ -93,15 +93,14 @@
                         path = line.strip()
                         full_url = f"{self.url}/{path}"
                         response = requests.get(full_url)
                         
                         if response.status_code == 200:
                             results_list.append(f'[Found] {full_url}')
                             print(f"{Color.GREEN}[Found]:{Color.RESET} {full_url}")
-                            
                         elif response.status_code == 204:
                             results_list.append(f'[No Content] {full_url}')
                             print(f"{Color.BLUE}[No Content]:{Color.RESET} {full_url}")
                         elif response.status_code == 400:
                             results_list.append(f'[Bad Request] {full_url}')
                             print(f"{Color.YELLOW}[Bad Request]:{Color.RESET} {full_url}")
                         elif response.status_code == 401:
@@ -170,10 +169,10 @@
             except KeyboardInterrupt:
                 print(f"{Color.GREEN}Attempt interrupted by user.{Color.RESET}")
             except requests.exceptions.ConnectionError as rec:
                 print(f"{Color.RED}[Error] {rec}{Color.RESET}")
             
         return results_list
     
-    def port_scan(self, ports) -> list:
+    def ports(self, ports) -> list:
         scan = PortScan(self.url)
         return scan.scan_ports(ports)
```

### Comparing `direnumerate-4.0a5/direnumerate/cli.py` & `direnumerate-4.0a6/direnumerate/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
     if args.verbose:
             try:
                 url = args.target
                 wordlist_file = args.wordlist
 
                 enum = Scan(url)
-                enum.show_dirs(wordlist_file, verbose=True)
+                enum.dirs(wordlist_file, verbose=True)
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
             except KeyboardInterrupt:
                 print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
     else:
         pass
 
     try:
         url = args.target
         wordlist_file = args.wordlist
 
         enum = Scan(url)
-        enum.show_dirs(wordlist_file=wordlist_file)
+        enum.dirs(wordlist_file=wordlist_file)
     except TypeError:
         print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
     except KeyboardInterrupt:
         print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
 
 
 def port_scan(args):
@@ -49,15 +49,15 @@
     """
     show_banner()
     try:
         host = args.target
         ports = args.ports
 
         scanner = Scan(host)
-        scanner.port_scan(ports=ports)
+        scanner.ports(ports=ports)
     except KeyboardInterrupt:
         print(Color.GREEN + "-------------- Port scan interrupted by user ------------" + Color.RESET)
 
 
 def main():
     """
     The main function for the Direnumerate application.
```

### Comparing `direnumerate-4.0a5/direnumerate/createlist.py` & `direnumerate-4.0a6/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a5/direnumerate/help.py` & `direnumerate-4.0a6/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a5/direnumerate/port_scan.py` & `direnumerate-4.0a6/direnumerate/port_scan.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a5/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0a6/direnumerate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a5
+Version: 4.0a6
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
@@ -84,22 +84,24 @@
 
 from direnumerate import Scan
 
 url = "testphp.vulnweb.com"
 wordlist = "wordlist.txt"
 
 enum = Scan(url)
-print(enum.show_dirs(wordlist))
+print(enum.dirs(wordlist))
 ```
 ----------
 
 ### Port Scan:
 
 ```python
 
 from direnumerate import Scan
 
-enum = Scan()
-print(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25]))
+ip = '44.228.249.3'
+
+enum = Scan(ip)
+print(enum.ports(ports=[22, 443, 8080, 8280, 80, 25]))
 
 ```
 ----------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a5 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a6 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -34,11 +34,10 @@
 Wordlist customization. - Detailed output of findings. - Support for multiple
 URL schemes (http, https, etc.). ## install: pip install direnumerate ---------
 -------- ## install in ubuntu: pip install direnumerate --break-system-packages
 ---------- ## Command line usage: ### Directory Scan: direnumerate -
 t testphp.vulnweb.com -w wordlist.txt ### Post Scan: direnumerate -
 t 44.228.249.3 -p 22 80 443 ## Scripts usage: ### Directory Scan in Websites:
 ```python from direnumerate import Scan url = "testphp.vulnweb.com" wordlist =
-"wordlist.txt" enum = Scan(url) print(enum.show_dirs(wordlist)) ``` ---------
-- ### Port Scan: ```python from direnumerate import Scan enum = Scan() print
-(enum.port_scan(ip='44.228.249.3', ports=[22, 443, 8080, 8280, 80, 25])) ``` --
---------
+"wordlist.txt" enum = Scan(url) print(enum.dirs(wordlist)) ``` ---------- ###
+Port Scan: ```python from direnumerate import Scan ip = '44.228.249.3' enum =
+Scan(ip) print(enum.ports(ports=[22, 443, 8080, 8280, 80, 25])) ``` ----------
```

### Comparing `direnumerate-4.0a5/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0a6/direnumerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a5/pyproject.toml` & `direnumerate-4.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "4.0a5"
+version = "4.0a6"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

