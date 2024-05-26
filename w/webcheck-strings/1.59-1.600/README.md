# Comparing `tmp/webcheck_strings-1.59.tar.gz` & `tmp/webcheck_strings-1.600.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcheck_strings-1.59.tar", last modified: Thu May 16 20:36:05 2024, max compression
+gzip compressed data, was "webcheck_strings-1.600.tar", last modified: Sun May 26 07:44:55 2024, max compression
```

## Comparing `webcheck_strings-1.59.tar` & `webcheck_strings-1.600.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 20:36:05.045188 webcheck_strings-1.59/
--rw-r--r--   0 silbrown   (501) staff       (20)    11357 2024-05-16 20:11:27.000000 webcheck_strings-1.59/LICENSE
--rw-r--r--   0 silbrown   (501) staff       (20)    14055 2024-05-16 20:36:05.044232 webcheck_strings-1.59/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-16 20:36:05.045355 webcheck_strings-1.59/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)    14166 2024-05-16 20:36:04.000000 webcheck_strings-1.59/setup.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 20:36:05.041311 webcheck_strings-1.59/webcheck/
--rw-r--r--   0 silbrown   (501) staff       (20)    45800 2024-05-16 20:36:04.000000 webcheck_strings-1.59/webcheck/__init__.py
--rw-r--r--   0 silbrown   (501) staff       (20)       32 2024-05-16 20:36:04.000000 webcheck_strings-1.59/webcheck/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 20:36:05.043569 webcheck_strings-1.59/webcheck_strings.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)    14055 2024-05-16 20:36:05.000000 webcheck_strings-1.59/webcheck_strings.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      261 2024-05-16 20:36:05.000000 webcheck_strings-1.59/webcheck_strings.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-16 20:36:05.000000 webcheck_strings-1.59/webcheck_strings.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       53 2024-05-16 20:36:05.000000 webcheck_strings-1.59/webcheck_strings.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        9 2024-05-16 20:36:05.000000 webcheck_strings-1.59/webcheck_strings.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-26 07:44:55.461076 webcheck_strings-1.600/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-26 07:44:52.000000 webcheck_strings-1.600/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    14044 2024-05-26 07:44:55.461076 webcheck_strings-1.600/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-26 07:44:55.461076 webcheck_strings-1.600/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    14155 2024-05-26 07:44:55.000000 webcheck_strings-1.600/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-26 07:44:55.461076 webcheck_strings-1.600/webcheck/
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)    46130 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       32 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-26 07:44:55.461076 webcheck_strings-1.600/webcheck_strings.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    14044 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck_strings.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      261 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck_strings.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck_strings.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       53 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck_strings.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2024-05-26 07:44:55.000000 webcheck_strings-1.600/webcheck_strings.egg-info/top_level.txt
```

### Comparing `webcheck_strings-1.59/LICENSE` & `webcheck_strings-1.600/LICENSE`

 * *Files identical despite different names*

### Comparing `webcheck_strings-1.59/PKG-INFO` & `webcheck_strings-1.600/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: webcheck_strings
-Version: 1.59
+Version: 1.600
 Summary: Monitor text strings on websites
 Home-page: http://ssb22.user.srcf.net/setup/webcheck.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 WebCheck
 ========
 
 From http://ssb22.user.srcf.net/setup/webcheck.html 
 
-webcheck.py requires Python, and is compatible with both Python 2 and Python 3.
-It is a program to check Web pages for changes to specific phrases of text. I currently use it to:
+WebCheck is a Python program (compatible with both Python 2 and Python 3) to check Web pages for changes to specific phrases (strings) of text. I currently use it to:
 
 * check that external links from my website still lead to the information that was there when I added them (I might need to update my links otherwise), and check whether or not I need to warn Lynx users about misguided blocking,
 * check the websites of companies, organisations or governments for changes to a specific rule to which I'd be interested in changes (for example because it applies to myself or someone I know, or because I've commented on it somewhere and my comment might need updating),
 * follow a couple of sites' "what's new" RSS feeds in my email,
 * check for new versions of software programs, data files, EPUB publications etc,
 * check if servers hosting my own projects are still serving them,
 * alert me if a private page has somehow been set to public when it shouldn't,
```

### Comparing `webcheck_strings-1.59/setup.py` & `webcheck_strings-1.600/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from setuptools import setup, find_packages;setup(name='webcheck_strings',version='1.59',entry_points={'console_scripts':['webcheck=webcheck.__init__:main']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/setup/webcheck.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Monitor text strings on websites',long_description=r'''WebCheck
+from setuptools import setup, find_packages;setup(name='webcheck_strings',version='1.600',entry_points={'console_scripts':['webcheck=webcheck.__init__:main']},license='Apache 2',platforms='any',url='http://ssb22.user.srcf.net/setup/webcheck.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Monitor text strings on websites',long_description=r'''WebCheck
 ========
 
 From http://ssb22.user.srcf.net/setup/webcheck.html 
 
-webcheck.py requires Python, and is compatible with both Python 2 and Python 3.
-It is a program to check Web pages for changes to specific phrases of text. I currently use it to:
+WebCheck is a Python program (compatible with both Python 2 and Python 3) to check Web pages for changes to specific phrases (strings) of text. I currently use it to:
 
 * check that external links from my website still lead to the information that was there when I added them (I might need to update my links otherwise), and check whether or not I need to warn Lynx users about misguided blocking,
 * check the websites of companies, organisations or governments for changes to a specific rule to which I'd be interested in changes (for example because it applies to myself or someone I know, or because I've commented on it somewhere and my comment might need updating),
 * follow a couple of sites' "what's new" RSS feeds in my email,
 * check for new versions of software programs, data files, EPUB publications etc,
 * check if servers hosting my own projects are still serving them,
 * alert me if a private page has somehow been set to public when it shouldn't,
```

### Comparing `webcheck_strings-1.59/webcheck/__init__.py` & `webcheck_strings-1.600/webcheck/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # (compatible with both Python 2 and Python 3)
 
-# webcheck.py v1.59 (c) 2014-24 Silas S. Brown.
+# webcheck.py v1.6 (c) 2014-24 Silas S. Brown.
 # See webcheck.html for description and usage instructions
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # 
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -25,15 +25,14 @@
 # and on GitHub at https://github.com/ssb22/web-imap-etc
 # and on GitLab at https://gitlab.com/ssb22/web-imap-etc
 # and on Bitbucket https://bitbucket.org/ssb22/web-imap-etc
 # and at https://gitlab.developers.cam.ac.uk/ssb22/web-imap-etc
 # and in China: https://gitee.com/ssb22/web-imap-etc
 
 max_threads = 10
-delay = 80 # seconds between fetches on same domain-set
 keep_etags = False # if True, will also keep any ETag headers as well as Last-Modified
 verify_SSL_certificates = False # webcheck's non-Webdriver URLs are for monitoring public services and there's not a lot of point in SSL authentication; failures due to server/client certificate misconfigurations are more trouble than they're worth
 
 import traceback, time, pickle, gzip, re, os, sys, socket, hashlib
 try: import htmlentitydefs # Python 2
 except ImportError: import html.entities as htmlentitydefs # Python 3
 try: from HTMLParser import HTMLParser # Python 2
@@ -233,15 +232,16 @@
         else: return parser.text().encode("latin1"), ""
     except: return html, "\n- problem extracting strings from HTML at line %d offset %d\n%s" % (parser.getpos()+(traceback.format_exc(),)) # returning html might still work for 'was that text still there' queries; error message is displayed only if it doesn't
 
 def main():
 
     # 1 job per domain:
     global jobs ; jobs = Queue.Queue()
-    for v in read_input().values(): jobs.put(v)
+    for mainDomain,jobItems in read_input().items():
+      jobs.put((mainDomain,jobItems))
     
     global previous_timestamps
     try: previous_timestamps = pickle.Unpickler(open(".webcheck-last","rb")).load()
     except: previous_timestamps = {}
     old_previous_timestamps = previous_timestamps.copy()
 
     for i in xrange(1,max_threads):
@@ -264,27 +264,32 @@
 # you can override this on a per-site basis with "User-Agent: whatever"
 # and undo again with "User-Agent:" on a line by itself.
 # Please override sparingly or with webmaster permission.
 # Let's not even mention it in the readme: we don't want to encourage
 # people to hide their tools from webmasters unnecessarily.
 
 class Delayer:
-  def __init__(self): self.last_fetch_finished = 0
+  def __init__(self,mainDomain):
+    self.last_fetch_finished = 0
+    if mainDomain=="stackoverflow.com":
+      # (or other Stack Exchange sites)
+      self.delay = 80 # seconds between fetches to these sites
+    else: self.delay = 3 # (want small if checking many pages and the server doesn't mind, but still non-0)
   def wait(self):
-    time.sleep(max(0,self.last_fetch_finished+delay-time.time()))
+    time.sleep(max(0,self.last_fetch_finished+self.delay-time.time()))
     if sys.stderr.isatty(): sys.stderr.write('.'),sys.stderr.flush()
   def done(self): self.last_fetch_finished = time.time()
 
 def worker_thread(*args):
     opener = [None]
     while True:
-      try: job = jobs.get(False)
+      try: mainDomain,job = jobs.get(False)
       except: return # no more jobs left
       try:
-        delayer = Delayer()
+        delayer = Delayer(mainDomain)
         items = sorted(job.items()) # sorted will group http and https together
         items.reverse()
         while items:
           url,checklist = items.pop()
           if '\n' in url:
               url = url.split('\n')
               extraHeaders = url[1:] ; url = url[0]
@@ -302,14 +307,15 @@
             r.reverse() ; items += r # try to keep pop() sequence in order
       except Exception as e:
         print ("Unhandled exception processing job "+repr(job))
         print (traceback.format_exc())
       jobs.task_done()
 class CDNBackoff(Exception): pass
 
+import threading ; lock = threading.Lock() # webcheck-debug
 def doJob(opener,delayer,url,checklist,extraHeaders):
   failRet = [c[2] for c in checklist if c[2]]
   delayer.wait()
   if url.startswith("dns://"): # DNS lookup
       try: u,content = None, B(' '.join(sorted(set('('+x[-1][0]+')' for x in socket.getaddrinfo(url[6:],1))))) # TODO this 'sorted' is lexicographical not numeric; it should be OK for most simple cases though (keeping things in a defined order so can check 2 or 3 IPs on same line if the numbers are consecutive and hold same number of digits).  Might be better if parse and numeric sort
       except: u,content=None,B("DNS lookup failed")
       textContent = content
@@ -498,15 +504,15 @@
     snippets = []
     for a in actionList:
         if a.startswith('http'): browser.get(a)
         elif a.startswith('"') and a.endswith('"'):
             # wait for "string" to appear in the source
             tries = 30
             while tries and not myFind(a[1:-1],getSrc()):
-              time.sleep(delay) ; tries -= 1
+              time.sleep(2) ; tries -= 1
             if not tries:
               try: current_url = browser.current_url
               except: current_url = "(unable to obtain)"
               raise NoTracebackException("webdriver timeout while waiting for %s, current URL is %s content \"%s\"\n" % (repr(a[1:-1]),current_url,repr(getSrc()))) # don't quote current URL: if the resulting email is viewed in (at least some versions of) MHonArc, a bug can result in &quot being added to the href
         elif a.startswith('[') and a.endswith(']'): # click
             findElem(a[1:-1]).click()
         elif a.startswith('/') and '/' in a[1:]: # click through items in a list to reveal each one (assume w/out Back)
@@ -582,15 +588,15 @@
         elif '=' in a: # put text in an input box
             spec, val = a.split('=',1)
             if val.startswith('"') and val.endswith('"'): val=val[1:-1]
             findElem(spec).send_keys(val)
         elif re.match("[0-9]+$",a): time.sleep(int(a))
         else: sys.stdout.write("Ignoring webdriver unknown action "+repr(a)+'\n')
         if sys.stderr.isatty(): sys.stderr.write(':'),sys.stderr.flush() # webdriver's '.'
-        time.sleep(delay)
+        time.sleep(2)
     snippets.append(getSrc())
     return B('\n').join(snippets)
 
 def get_gemini(url,nestLevel=0):
     if nestLevel > 9: return B("Too many redirects"),B("Too many redirects")
     url = B(url)
     host0 = host = re.match(B("gemini://([^/?#]*)"),url).groups(1)[0]
```

### Comparing `webcheck_strings-1.59/webcheck_strings.egg-info/PKG-INFO` & `webcheck_strings-1.600/webcheck_strings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: webcheck-strings
-Version: 1.59
+Version: 1.600
 Summary: Monitor text strings on websites
 Home-page: http://ssb22.user.srcf.net/setup/webcheck.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 WebCheck
 ========
 
 From http://ssb22.user.srcf.net/setup/webcheck.html 
 
-webcheck.py requires Python, and is compatible with both Python 2 and Python 3.
-It is a program to check Web pages for changes to specific phrases of text. I currently use it to:
+WebCheck is a Python program (compatible with both Python 2 and Python 3) to check Web pages for changes to specific phrases (strings) of text. I currently use it to:
 
 * check that external links from my website still lead to the information that was there when I added them (I might need to update my links otherwise), and check whether or not I need to warn Lynx users about misguided blocking,
 * check the websites of companies, organisations or governments for changes to a specific rule to which I'd be interested in changes (for example because it applies to myself or someone I know, or because I've commented on it somewhere and my comment might need updating),
 * follow a couple of sites' "what's new" RSS feeds in my email,
 * check for new versions of software programs, data files, EPUB publications etc,
 * check if servers hosting my own projects are still serving them,
 * alert me if a private page has somehow been set to public when it shouldn't,
```

