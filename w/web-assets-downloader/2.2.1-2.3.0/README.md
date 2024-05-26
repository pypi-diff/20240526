# Comparing `tmp/web_assets_downloader-2.2.1.tar.gz` & `tmp/web_assets_downloader-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_assets_downloader-2.2.1.tar", last modified: Sat May 18 13:40:11 2024, max compression
+gzip compressed data, was "web_assets_downloader-2.3.0.tar", last modified: Sun May 26 17:19:38 2024, max compression
```

## Comparing `web_assets_downloader-2.2.1.tar` & `web_assets_downloader-2.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-18 13:40:11.511816 web_assets_downloader-2.2.1/
--rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-18 13:40:11.511816 web_assets_downloader-2.2.1/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-18 13:40:11.511816 web_assets_downloader-2.2.1/setup.cfg
--rw-rw-r--   0 arif      (1000) arif      (1000)     1543 2024-05-18 13:40:00.000000 web_assets_downloader-2.2.1/setup.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-18 13:40:11.511816 web_assets_downloader-2.2.1/web_assets_downloader/
--rw-rw-r--   0 arif      (1000) arif      (1000)      141 2024-03-03 10:53:55.000000 web_assets_downloader-2.2.1/web_assets_downloader/__init__.py
--rw-rw-r--   0 arif      (1000) arif      (1000)     4985 2024-05-18 13:36:01.000000 web_assets_downloader-2.2.1/web_assets_downloader/web_assets_downloader.py
-drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-18 13:40:11.511816 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/
--rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-18 13:40:11.000000 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/PKG-INFO
--rw-rw-r--   0 arif      (1000) arif      (1000)      361 2024-05-18 13:40:11.000000 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/SOURCES.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       88 2024-05-18 13:40:11.000000 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/dependency_links.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       81 2024-05-18 13:40:11.000000 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/entry_points.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       59 2024-05-18 13:40:11.000000 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/requires.txt
--rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-18 13:40:11.000000 web_assets_downloader-2.2.1/web_assets_downloader.egg-info/top_level.txt
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 17:19:38.606554 web_assets_downloader-2.3.0/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-26 17:19:38.606554 web_assets_downloader-2.3.0/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)       38 2024-05-26 17:19:38.606554 web_assets_downloader-2.3.0/setup.cfg
+-rw-rw-r--   0 arif      (1000) arif      (1000)     1543 2024-05-26 17:19:37.000000 web_assets_downloader-2.3.0/setup.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 17:19:38.602554 web_assets_downloader-2.3.0/web_assets_downloader/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      141 2024-03-03 10:53:55.000000 web_assets_downloader-2.3.0/web_assets_downloader/__init__.py
+-rw-rw-r--   0 arif      (1000) arif      (1000)     5573 2024-05-26 17:19:15.000000 web_assets_downloader-2.3.0/web_assets_downloader/web_assets_downloader.py
+drwxrwxr-x   0 arif      (1000) arif      (1000)        0 2024-05-26 17:19:38.602554 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/
+-rw-rw-r--   0 arif      (1000) arif      (1000)      957 2024-05-26 17:19:38.000000 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/PKG-INFO
+-rw-rw-r--   0 arif      (1000) arif      (1000)      361 2024-05-26 17:19:38.000000 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/SOURCES.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       88 2024-05-26 17:19:38.000000 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/dependency_links.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       81 2024-05-26 17:19:38.000000 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/entry_points.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       59 2024-05-26 17:19:38.000000 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/requires.txt
+-rw-rw-r--   0 arif      (1000) arif      (1000)       22 2024-05-26 17:19:38.000000 web_assets_downloader-2.3.0/web_assets_downloader.egg-info/top_level.txt
```

### Comparing `web_assets_downloader-2.2.1/PKG-INFO` & `web_assets_downloader-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web_assets_downloader
-Version: 2.2.1
+Version: 2.3.0
 Summary: A package for downloading web content and assets
 Home-page: https://github.com/arif-x/web-assets-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@email.com
 License: MIT
 Project-URL: Source, https://github.com/arif-x/web-assets-downloader
 Project-URL: Source Code, https://github.com/arif-x/web-assets-downloader
```

### Comparing `web_assets_downloader-2.2.1/setup.py` & `web_assets_downloader-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='web_assets_downloader',
-    version='2.2.1',
+    version='2.3.0',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
         'pillow',
         'PyPDF2',
         'python-docx',
```

### Comparing `web_assets_downloader-2.2.1/web_assets_downloader/web_assets_downloader.py` & `web_assets_downloader-2.3.0/web_assets_downloader/web_assets_downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,72 @@
 import os
 from urllib.parse import urlparse
 import requests
 from bs4 import BeautifulSoup
 from urllib.parse import urljoin, unquote
-from PIL import Image
 import PyPDF2
 from docx import Document
 from openpyxl import load_workbook
 
-def download_asset(asset_urls, save_folder, headers, img=True, pdf=True, doc=True, xlx=True):
+def download_asset(asset_urls, save_folder, headers, img=True, pdf=True, doc=True, xlx=True, html=True):
     for url in asset_urls:
         print(url)
         response = requests.get(url, headers=headers)
         if response.status_code == 200:
             # Parse the asset URL to extract the path
             parsed_url = urlparse(url)
             asset_path = unquote(parsed_url.path)
 
+            # Check if the file is an HTML, JS, or CSS file
+            if not html and asset_path.lower().endswith(('.html', '.htm', '.js', '.css')):
+                print(f"Skipping HTML/CSS/JS file: {asset_path}")
+                continue
+
+            # Check if the file is a PDF file
+            if not pdf and asset_path.lower().endswith('.pdf'):
+                print(f"Skipping PDF file: {asset_path}")
+                continue
+
+            # Check if the file is a DOCX file
+            if not doc and asset_path.lower().endswith('.docx'):
+                print(f"Skipping DOCX file: {asset_path}")
+                continue
+
+            # Check if the file is an XLSX file
+            if not xlx and asset_path.lower().endswith('.xlsx'):
+                print(f"Skipping XLSX file: {asset_path}")
+                continue
+
+            # Check if the file is an image file
+            if not img and asset_path.lower().endswith(('.png', '.jpg', '.jpeg', '.gif')):
+                print(f"Skipping image file: {asset_path}")
+                continue
+
             # Construct the filepath within the assets directory
             asset_filepath = os.path.join(save_folder, asset_path.lstrip('/'))
 
             # Create the directory if it doesn't exist
             os.makedirs(os.path.dirname(asset_filepath), exist_ok=True)
 
             # Download the asset
             with open(asset_filepath, 'wb') as f:
                 f.write(response.content)
                 print(f"Downloaded {asset_path}.")
 
-            if img:
-                # Resize images if it's an image file
-                if asset_path.lower().endswith(('.png', '.jpg', '.jpeg', '.gif')):
-                    resize_image(asset_filepath, (100, 100))  # Specify desired dimensions
-
-            if pdf:
+            if pdf and asset_path.lower().endswith('.pdf'):
                 # Extract text from PDF files
-                if asset_path.lower().endswith('.pdf'):
-                    extract_text_from_pdf(asset_filepath)
+                extract_text_from_pdf(asset_filepath)
 
-            if doc:
+            if doc and asset_path.lower().endswith('.docx'):
                 # Extract text from Word files
-                if asset_path.lower().endswith('.docx'):
-                    extract_text_from_docx(asset_filepath)
+                extract_text_from_docx(asset_filepath)
 
-            if xlx:
+            if xlx and asset_path.lower().endswith('.xlsx'):
                 # Extract text from Excel files
-                if asset_path.lower().endswith('.xlsx'):
-                    extract_text_from_excel(asset_filepath)
-
-def resize_image(image_path, dimensions):
-    img = Image.open(image_path)
-    img_resized = img.resize(dimensions, Image.ANTIALIAS)
-    img_resized.save(image_path)
+                extract_text_from_excel(asset_filepath)
 
 def extract_text_from_pdf(pdf_path):
     with open(pdf_path, 'rb') as pdf_file:
         pdf_reader = PyPDF2.PdfFileReader(pdf_file)
         text = ''
         for page_num in range(pdf_reader.numPages):
             page = pdf_reader.getPage(page_num)
@@ -74,15 +85,15 @@
         ws = wb[sheet]
         for row in ws.iter_rows():
             for cell in row:
                 text += str(cell.value) + ' '
             text += '\n'
     print(f"Text extracted from {excel_path}: {text}")
 
-def download_html_and_asset(url_list, save_folder, max_depth=None, img=True, pdf=True, doc=True, xlx=True):
+def download_html_and_asset(url_list, save_folder, max_depth=None, img=True, pdf=True, doc=True, xlx=True, html=True):
     # Standard User-Agent header for a common web browser
     headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3'}
 
     for url in url_list:
         response = requests.get(url, headers=headers)
         print(response.status_code)
         if response.status_code == 200:
@@ -122,10 +133,10 @@
 
                 absolute_url = urljoin(base_url, asset_url)
 
                 print(absolute_url)
                 asset_urls.add(absolute_url)
 
             # Download assets
-            download_asset(asset_urls, save_folder, headers, img, pdf, doc, xlx)
+            download_asset(asset_urls, save_folder, headers, img, pdf, doc, xlx, html)
 
     return True
```

### Comparing `web_assets_downloader-2.2.1/web_assets_downloader.egg-info/PKG-INFO` & `web_assets_downloader-2.3.0/web_assets_downloader.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-assets-downloader
-Version: 2.2.1
+Version: 2.3.0
 Summary: A package for downloading web content and assets
 Home-page: https://github.com/arif-x/web-assets-downloader
 Author: Ariffudin
 Author-email: sudo.ariffudin@email.com
 License: MIT
 Project-URL: Source, https://github.com/arif-x/web-assets-downloader
 Project-URL: Source Code, https://github.com/arif-x/web-assets-downloader
```

