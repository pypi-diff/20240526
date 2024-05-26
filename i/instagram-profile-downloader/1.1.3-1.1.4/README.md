# Comparing `tmp/instagram_profile_downloader-1.1.3.tar.gz` & `tmp/instagram_profile_downloader-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram_profile_downloader-1.1.3.tar", last modified: Sat May 25 06:22:55 2024, max compression
+gzip compressed data, was "instagram_profile_downloader-1.1.4.tar", last modified: Sun May 26 08:34:23 2024, max compression
```

## Comparing `instagram_profile_downloader-1.1.3.tar` & `instagram_profile_downloader-1.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-25 06:22:55.024137 instagram_profile_downloader-1.1.3/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.1.3/LICENSE
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4391 2024-05-25 06:22:55.023871 instagram_profile_downloader-1.1.3/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 23:34:58.000000 instagram_profile_downloader-1.1.3/README.md
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-25 06:22:55.022204 instagram_profile_downloader-1.1.3/instagram_profile_downloader/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)    12829 2024-05-25 06:21:46.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader/instagram_profile_downloader.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)     1168 2024-05-25 01:29:17.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader/private.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-25 06:22:55.023558 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4391 2024-05-25 06:22:54.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      482 2024-05-25 06:22:54.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-25 06:22:54.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-25 06:22:54.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       93 2024-05-25 06:22:54.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-25 06:22:54.000000 instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-25 06:22:55.024175 instagram_profile_downloader-1.1.3/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)     1092 2024-05-25 06:22:04.000000 instagram_profile_downloader-1.1.3/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-26 08:34:23.801682 instagram_profile_downloader-1.1.4/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:29:25.000000 instagram_profile_downloader-1.1.4/LICENSE
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4391 2024-05-26 08:34:23.801431 instagram_profile_downloader-1.1.4/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     3623 2024-05-24 23:34:58.000000 instagram_profile_downloader-1.1.4/README.md
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-26 08:34:23.800164 instagram_profile_downloader-1.1.4/instagram_profile_downloader/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-24 18:23:50.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)    13742 2024-05-26 08:33:50.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader/instagram_profile_downloader.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     1168 2024-05-25 01:29:17.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader/private.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-26 08:34:23.801144 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4391 2024-05-26 08:34:23.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      482 2024-05-26 08:34:23.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-26 08:34:23.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      112 2024-05-26 08:34:23.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       93 2024-05-26 08:34:23.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       29 2024-05-26 08:34:23.000000 instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-26 08:34:23.801726 instagram_profile_downloader-1.1.4/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     1092 2024-05-26 08:34:09.000000 instagram_profile_downloader-1.1.4/setup.py
```

### Comparing `instagram_profile_downloader-1.1.3/PKG-INFO` & `instagram_profile_downloader-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram_profile_downloader
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.1.3/README.md` & `instagram_profile_downloader-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.1.3/instagram_profile_downloader/instagram_profile_downloader.py` & `instagram_profile_downloader-1.1.4/instagram_profile_downloader/instagram_profile_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,27 +71,29 @@
 @click.command()
 @click.argument("profile_names", required=False)
 @click.option("--media-root", required=False, help="Base directory for media output.")
 @click.option("--no-highlights", is_flag=True, help="Do not download highlights.")
 @click.option("--no-posts", is_flag=True, help="Do not download posts.")
 @click.option("--user", required=False, help="Instagram username.")
 @click.option("--password", required=False, help="Instagram password.")
-def main(profile_names, media_root, no_highlights, no_posts, user, password):
+@click.option("--two-factor", is_flag=True, help="Use two-factor authentication.")
+def main(
+    profile_names, media_root, no_highlights, no_posts, user, password, two_factor
+):
     config = load_config()
 
     profile_names = profile_names or config.get("profile_names")
     if not profile_names:
         console.print(
             "[bold magenta]Please enter the Instagram profile names separated by commas[/bold magenta]"
         )
         profile_names = click.prompt("", type=str)
 
     profile_names = [name.strip() for name in profile_names.split(",")]
 
-    # instead of this: console.print(f"[green]Profile names set to:[/green] [bold]{profile_names}[/bold]") i would like to get multiple lines of console output -> one line per profile name
     for profile_name in profile_names:
         console.print(
             f"[green]Profile name set to:[/green] [bold]{profile_name}[/bold]"
         )
 
     media_root = media_root or config.get("download_directory")
     if not media_root:
@@ -108,15 +110,40 @@
         console.print("[bold cyan]Username:[/bold cyan]", end=" ")
         user = click.prompt("", type=str)
         console.print("[bold cyan]Password:[/bold cyan]", end=" ")
         password = click.prompt("", type=str, hide_input=True)
 
     # Create an instance of Instaloader
     L = instaloader.Instaloader()
-    L.login(user, password)
+
+    # Initial Login Attempt
+    try:
+        L.login(user, password)
+    except instaloader.TwoFactorAuthRequiredException:
+        if two_factor:
+            while True:
+                console.print(
+                    "[bold yellow]2FA is required. Please enter the 2FA code:[/bold yellow]",
+                    end=" ",
+                )
+                two_factor_code = click.prompt("", type=str)
+                try:
+                    L.two_factor_login(two_factor_code)
+                    console.print("[green]2FA login successful![/green]")
+                    break
+                except instaloader.exceptions.BadCredentialsException as e:
+                    console.print(f"[red]2FA error: {e}. Please try again.[/red]")
+        else:
+            console.print(
+                "[red]2FA is required but --two-factor flag not provided.[/red]"
+            )
+            return
+    except instaloader.exceptions.BadCredentialsException as e:
+        console.print(f"[red]Login error: {e}[/red]")
+        return
 
     def download_media(url, output_dir):
         try:
             # Ensure the output directory exists
             os.makedirs(output_dir, exist_ok=True)
 
             # Extract filename from URL
```

### Comparing `instagram_profile_downloader-1.1.3/instagram_profile_downloader/private.py` & `instagram_profile_downloader-1.1.4/instagram_profile_downloader/private.py`

 * *Files identical despite different names*

### Comparing `instagram_profile_downloader-1.1.3/instagram_profile_downloader.egg-info/PKG-INFO` & `instagram_profile_downloader-1.1.4/instagram_profile_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instagram-profile-downloader
-Version: 1.1.3
+Version: 1.1.4
 Summary: A tool to download all images and videos and story highlights from an Instagram profile.
 Home-page: https://github.com/tadeasf/instagram_profile_downloader
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `instagram_profile_downloader-1.1.3/setup.py` & `instagram_profile_downloader-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="instagram_profile_downloader",
-    version="1.1.3",
+    version="1.1.4",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to download all images and videos and story highlights from an Instagram profile.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/instagram_profile_downloader",
     packages=find_packages(),
```

