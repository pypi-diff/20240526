# Comparing `tmp/mutt_html_reply-0.1.0.tar.gz` & `tmp/mutt_html_reply-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutt_html_reply-0.1.0.tar", last modified: Wed May 22 16:51:30 2024, max compression
+gzip compressed data, was "mutt_html_reply-0.2.0.tar", last modified: Sun May 26 02:13:44 2024, max compression
```

## Comparing `mutt_html_reply-0.1.0.tar` & `mutt_html_reply-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-22 16:51:30.052893 mutt_html_reply-0.1.0/
--rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.1.0/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)      126 2024-05-22 16:51:30.052893 mutt_html_reply-0.1.0/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      728 2024-05-22 16:51:01.000000 mutt_html_reply-0.1.0/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      252 2024-05-22 16:48:35.000000 mutt_html_reply-0.1.0/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-22 16:51:30.052893 mutt_html_reply-0.1.0/setup.cfg
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-22 16:51:30.052893 mutt_html_reply-0.1.0/src/
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-22 16:51:30.052893 mutt_html_reply-0.1.0/src/mutt_html_reply/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.1.0/src/mutt_html_reply/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1868 2024-05-22 16:50:50.000000 mutt_html_reply-0.1.0/src/mutt_html_reply/mutt_html_reply.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-22 16:51:30.052893 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)      126 2024-05-22 16:51:30.000000 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-22 16:51:30.000000 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-22 16:51:30.000000 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-22 16:51:30.000000 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-22 16:51:30.000000 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-22 16:51:30.000000 mutt_html_reply-0.1.0/src/mutt_html_reply.egg-info/top_level.txt
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-26 02:13:44.547094 mutt_html_reply-0.2.0/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1062 2024-05-22 16:41:30.000000 mutt_html_reply-0.2.0/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)     2275 2024-05-26 02:13:44.543761 mutt_html_reply-0.2.0/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      728 2024-05-22 16:51:01.000000 mutt_html_reply-0.2.0/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)      623 2024-05-26 02:13:36.000000 mutt_html_reply-0.2.0/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)       38 2024-05-26 02:13:44.547094 mutt_html_reply-0.2.0/setup.cfg
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-26 02:13:44.543761 mutt_html_reply-0.2.0/src/
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-26 02:13:44.543761 mutt_html_reply-0.2.0/src/mutt_html_reply/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2024-05-22 16:37:47.000000 mutt_html_reply-0.2.0/src/mutt_html_reply/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2208 2024-05-26 02:05:12.000000 mutt_html_reply-0.2.0/src/mutt_html_reply/mutt_html_reply.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-26 02:13:44.543761 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2275 2024-05-26 02:13:44.000000 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      363 2024-05-26 02:13:44.000000 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-26 02:13:44.000000 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       73 2024-05-26 02:13:44.000000 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       15 2024-05-26 02:13:44.000000 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       16 2024-05-26 02:13:44.000000 mutt_html_reply-0.2.0/src/mutt_html_reply.egg-info/top_level.txt
```

### Comparing `mutt_html_reply-0.1.0/LICENSE` & `mutt_html_reply-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.1.0/README.md` & `mutt_html_reply-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mutt_html_reply-0.1.0/src/mutt_html_reply/mutt_html_reply.py` & `mutt_html_reply-0.2.0/src/mutt_html_reply/mutt_html_reply.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import html
 import sys
-from bs4 import BeautifulSoup
+from bs4 import BeautifulSoup, Doctype
 import css_inline
 
-HEADER_FIRST_SORT_LIST_COMPARISON = ['F','D','T','C']
+HEADER_FIRST_SORT_LIST_COMPARISON = ['F','D','T','C','S']
 
 def main():
     """
     Create an Outlook-style HTML reply
     
     mutt-html-reply [html reply] [html original message] [headers to include in quote] [output path]
     """
@@ -22,39 +23,47 @@
         html_reply = file.read()
     with open(filepath_original_msg, 'r') as file:
         html_original_msg = file.read()
     with open(filepath_original_headers, 'r') as file:
         text_original_headers = file.read().splitlines()
 
     # Convert HTML text to BeautifulSoup object and inline all CSS
+
     bs4_msg = BeautifulSoup(css_inline.inline(html_reply),'html.parser')
+
     bs4_original_msg = BeautifulSoup(css_inline.inline(html_original_msg), 'html.parser')
+    bs4_original_msg.html.unwrap() #type: ignore
+    bs4_original_msg.body.unwrap() #type: ignore
+    bs4_original_msg.head.extract() #type: ignore
+    for element in bs4_original_msg.contents:
+        if isinstance(element, Doctype):
+            element.extract()
+
     bs4_original_headers = BeautifulSoup(_get_header_html(text_original_headers), 'html.parser')
 
     # Combine HTML together
-    bs4_final = BeautifulSoup()
-    bs4_final.append(bs4_msg)
-    bs4_final.append(BeautifulSoup('<hr>', 'html.parser'))
-    bs4_final.append(bs4_original_headers)
-    bs4_final.append(bs4_original_msg)
+    bs4_final = bs4_msg
+    bs4_final.body.append(BeautifulSoup('<hr></hr>', 'html.parser')) #type: ignore
+    bs4_final.body.append(bs4_original_headers) #type: ignore
+    bs4_final.body.append(bs4_original_msg) #type: ignore
 
     # Write output
     with open(filepath_output, 'w') as file:
         file.write(str(bs4_final))
 
 
-def _get_header_html(text):
+def _get_header_html(header_list):
     resorted_text = []
     for first in HEADER_FIRST_SORT_LIST_COMPARISON:
-        for header in text:
+        for header in header_list:
             if header[0] == first:
-                resorted_text.append(header)
-    html_headers = "<p>\n"
+                resorted_text.append(html.escape(header))
+    html_headers = "<p>"
     for header in resorted_text:
         html_headers = html_headers + '<br>' + header
-    html_headers = html_headers + "\n</p>\n"
+    html_headers = html_headers + "</p>\n"
     return html_headers
 
 
 
 if __name__ == "__main__":
     main()
```

