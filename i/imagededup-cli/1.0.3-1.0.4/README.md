# Comparing `tmp/imagededup-cli-1.0.3.tar.gz` & `tmp/imagededup-cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagededup-cli-1.0.3.tar", last modified: Tue May 21 04:20:27 2024, max compression
+gzip compressed data, was "imagededup-cli-1.0.4.tar", last modified: Sun May 26 04:22:49 2024, max compression
```

## Comparing `imagededup-cli-1.0.3.tar` & `imagededup-cli-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 04:20:27.097091 imagededup-cli-1.0.3/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:29.000000 imagededup-cli-1.0.3/LICENSE
--rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-21 04:20:27.096938 imagededup-cli-1.0.3/PKG-INFO
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 04:20:27.096094 imagededup-cli-1.0.3/imagededup_cli/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:11.000000 imagededup-cli-1.0.3/imagededup_cli/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4835 2024-05-21 04:20:17.000000 imagededup-cli-1.0.3/imagededup_cli/imagededup_cli.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-21 04:20:27.096777 imagededup-cli-1.0.3/imagededup_cli.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-21 04:20:27.000000 imagededup-cli-1.0.3/imagededup_cli.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      306 2024-05-21 04:20:27.000000 imagededup-cli-1.0.3/imagededup_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-21 04:20:27.000000 imagededup-cli-1.0.3/imagededup_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       70 2024-05-21 04:20:27.000000 imagededup-cli-1.0.3/imagededup_cli.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       32 2024-05-21 04:20:27.000000 imagededup-cli-1.0.3/imagededup_cli.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       15 2024-05-21 04:20:27.000000 imagededup-cli-1.0.3/imagededup_cli.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-21 04:20:27.097130 imagededup-cli-1.0.3/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)      904 2024-05-21 04:19:55.000000 imagededup-cli-1.0.3/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-26 04:22:49.161907 imagededup-cli-1.0.4/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:29.000000 imagededup-cli-1.0.4/LICENSE
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-26 04:22:49.161772 imagededup-cli-1.0.4/PKG-INFO
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-26 04:22:49.160627 imagededup-cli-1.0.4/imagededup_cli/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-21 02:18:11.000000 imagededup-cli-1.0.4/imagededup_cli/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4943 2024-05-26 04:21:42.000000 imagededup-cli-1.0.4/imagededup_cli/imagededup_cli.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-26 04:22:49.161528 imagededup-cli-1.0.4/imagededup_cli.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      480 2024-05-26 04:22:49.000000 imagededup-cli-1.0.4/imagededup_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      306 2024-05-26 04:22:49.000000 imagededup-cli-1.0.4/imagededup_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-26 04:22:49.000000 imagededup-cli-1.0.4/imagededup_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       70 2024-05-26 04:22:49.000000 imagededup-cli-1.0.4/imagededup_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       37 2024-05-26 04:22:49.000000 imagededup-cli-1.0.4/imagededup_cli.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       15 2024-05-26 04:22:49.000000 imagededup-cli-1.0.4/imagededup_cli.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-26 04:22:49.162009 imagededup-cli-1.0.4/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      909 2024-05-26 04:22:35.000000 imagededup-cli-1.0.4/setup.py
```

### Comparing `imagededup-cli-1.0.3/imagededup_cli/imagededup_cli.py` & `imagededup-cli-1.0.4/imagededup_cli/imagededup_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import shutil
-import click
+import rich_click as click
 from tqdm import tqdm
 import tkinter as tk
 from tkinter import filedialog
 from imagededup.methods import DHash, CNN
 from loguru import logger
 from time import time
 import sys
@@ -18,20 +18,22 @@
     colorize=True,
     format="<green>{time}</green> <level>{message}</level>",
 )
 logger.add(
     sys.stderr, format="<green>{time}</green> <level>{message}</level>", colorize=True
 )
 
+
 def select_directory():
     root = tk.Tk()
     root.withdraw()  # Hide the main window
     folder_selected = filedialog.askdirectory()
     return folder_selected
 
+
 def find_and_move_duplicates_dhash(input_dir, threshold):
     dhash = DHash()
     duplicates_dir = os.path.join(input_dir, "duplicates")
     if not os.path.exists(duplicates_dir):
         os.makedirs(duplicates_dir)
 
     # Find all JPG files recursively
@@ -61,14 +63,15 @@
         src_file = os.path.join(input_dir, file)
         dest_file = os.path.join(duplicates_dir, os.path.basename(file))
         if os.path.exists(src_file):
             shutil.move(src_file, dest_file)
 
     return total_images, total_duplicates
 
+
 def find_and_move_duplicates_cnn(input_dir, threshold):
     cnn = CNN()
     duplicates_dir = os.path.join(input_dir, "duplicates")
     if not os.path.exists(duplicates_dir):
         os.makedirs(duplicates_dir)
 
     # Find all JPG files recursively
@@ -95,14 +98,15 @@
         src_file = os.path.join(input_dir, file)
         dest_file = os.path.join(duplicates_dir, os.path.basename(file))
         if os.path.exists(src_file):
             shutil.move(src_file, dest_file)
 
     return total_images, total_duplicates
 
+
 @click.command()
 @click.option(
     "--threshold",
     default=10,  # Default threshold for DHash method
     type=float,
     help="Threshold for duplicate detection. For DHash (default: 10, min: 0, max: 64). For CNN (default: 0.99, range: 0.5-0.99)",
 )
@@ -115,30 +119,39 @@
 def main(threshold, algo):
     start_time = time()
 
     if algo == "cnn":
         if threshold == 10:
             threshold = 0.99  # Default threshold for CNN
         else:
-            threshold = max(0.5, min(0.99, threshold))  # Ensure threshold is within valid range
+            threshold = max(
+                0.5, min(0.99, threshold)
+            )  # Ensure threshold is within valid range
     else:
         threshold = int(threshold)  # Convert to integer for DHash
 
     input_dir = select_directory()
     if not input_dir:
         logger.info("No directory selected. Exiting.")
         return
     logger.info(f"Selected directory: {input_dir}")
-    logger.info(f"Finding duplicates with threshold: {threshold} using {algo.upper()} algorithm")
+    logger.info(
+        f"Finding duplicates with threshold: {threshold} using {algo.upper()} algorithm"
+    )
 
     if algo == "dhash":
-        total_images, total_duplicates = find_and_move_duplicates_dhash(input_dir, threshold)
+        total_images, total_duplicates = find_and_move_duplicates_dhash(
+            input_dir, threshold
+        )
     else:
-        total_images, total_duplicates = find_and_move_duplicates_cnn(input_dir, threshold)
+        total_images, total_duplicates = find_and_move_duplicates_cnn(
+            input_dir, threshold
+        )
 
     end_time = time()
     total_time = end_time - start_time
 
     logger.info(f"Total runtime: {total_time:.2f} seconds")
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `imagededup-cli-1.0.3/setup.py` & `imagededup-cli-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="imagededup-cli",  # Package name
-    version="1.0.3",  # Initial version
+    version="1.0.4",  # Initial version
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to remove duplicate jpg images",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/imagededup-cli",  # Project URL
     packages=find_packages(),
     install_requires=[
-        "click",
+        "rich-click",
         "tk",
         "tqdm",
         "loguru",
         "imagededup",
     ],
     entry_points={
         "console_scripts": [
```

