# Comparing `tmp/klldFN-2.0.0.tar.gz` & `tmp/klldFN-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-2.0.0.tar", last modified: Sun May 26 21:30:14 2024, max compression
+gzip compressed data, was "klldFN-2.0.0b1.tar", last modified: Sat May 18 16:01:32 2024, max compression
```

## Comparing `klldFN-2.0.0.tar` & `klldFN-2.0.0b1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-26 21:30:14.822440 klldFN-2.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)     1086 2024-05-26 21:30:14.822440 klldFN-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       62 2024-05-25 10:49:24.000000 klldFN-2.0.0/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-26 21:30:14.810439 klldFN-2.0.0/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)   134588 2024-05-26 18:28:13.000000 klldFN-2.0.0/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-26 21:30:14.818440 klldFN-2.0.0/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1086 2024-05-26 21:30:14.000000 klldFN-2.0.0/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-05-26 21:30:14.000000 klldFN-2.0.0/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-26 21:30:14.000000 klldFN-2.0.0/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      109 2024-05-26 21:30:14.000000 klldFN-2.0.0/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-26 21:30:14.000000 klldFN-2.0.0/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-26 21:30:14.822440 klldFN-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1282 2024-05-26 21:28:57.000000 klldFN-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1052 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       64 2024-05-18 12:28:14.000000 klldFN-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.425220 klldFN-2.0.0b1/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)   134565 2024-05-18 13:15:51.000000 klldFN-2.0.0b1/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-18 16:01:32.429221 klldFN-2.0.0b1/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1052 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      102 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2024-05-18 16:01:32.000000 klldFN-2.0.0b1/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      494 2024-04-12 16:24:13.000000 klldFN-2.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-18 16:01:32.433221 klldFN-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1248 2024-05-18 15:56:57.000000 klldFN-2.0.0b1/setup.py
```

### Comparing `klldFN-2.0.0/PKG-INFO` & `klldFN-2.0.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 2.0.0
+Version: 2.0.0b1
 Summary: klldFN
-Home-page: https://github.com/klldtest/klldFN
+Home-page: https://klldfn.xyz
 Author: klld
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: crayons
 Requires-Dist: fortnitepy-edit
 Requires-Dist: FortniteAPIAsync==0.1.6
 Requires-Dist: sanic==20.12.0
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
-Requires-Dist: jinja2
 
-# klldFN 2.0.0
+# klldFN 2.0.0b1
 **pip install klldFN**
 
 **pip3 install klldFN**
```

### Comparing `klldFN-2.0.0/klldFN/__init__.py` & `klldFN-2.0.0b1/klldFN/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,14 @@
         """
         response = requests.get(url)
 
         if response.status_code == 200:
             new_content = response.content
 
             try:
-                os.makedirs(os.path.dirname(file_name), exist_ok=True)
-              
                 with open(file_name, 'rb') as f:
                     existing_content = f.read()
 
                 if new_content != existing_content:
                     with open(file_name, 'wb') as f:
                         f.write(new_content)
                     pass
@@ -133,15 +131,15 @@
                 TextColumn("[bold blue]{task.description}", justify="right"),
                 BarColumn(bar_width=None),
                 SpinnerColumn(spinner_name="clock", style="bright_yellow", speed=1.0),
                 TimeElapsedColumn(),
             )        
     task1 = None
     with progress:
-                task1 = progress.add_task("[bold green]Starting klldFN v2.0.0...", total=3)
+                task1 = progress.add_task("[bold green]Starting klldFN 2.0.0b1...", total=3)
                 await asyncio.sleep(2)
                 progress.update(task1, advance=2, description="[bold green]Checking and updating package...")
                 await check_and_update_package()
                 await asyncio.sleep(1)
                 progress.update(task1, advance=1, description="[bold green]Updating translations...")
                 await UpdateTranslations()
 
@@ -221,15 +219,14 @@
     @client.event  
     async def event_ready() -> None:
 
         await edit_and_keep_client_member()
         await add_list()
         client_ready = translations.read()["translations"]["Client-ready"][get_Language]
         print(f'{client_ready} {client.user.display_name}')
-      
 
 
     async def set_crowns():
         meta = client.party.me.meta
         data = (meta.get_prop('Default:AthenaCosmeticLoadout_j'))['AthenaCosmeticLoadout']
         try:
             data['cosmeticStats'][1]['statValue'] = 1942
@@ -257,27 +254,27 @@
                         icon=configuration.read()['banner']['bannerName'],
                         color=configuration.read()['banner']['bannerColor'],
                         season_level=configuration.read()['banner']['level']),
                 partial(client.party.me.set_backpack, asset=configuration.read()['cosmetics']['backpack']),
                 partial(client.party.me.set_pickaxe, asset=configuration.read()['cosmetics']['pickaxe']),
             )
         except Exception as e:
-            error_klldfn = translations.read()["translations"]["error-klldfn"][get_Language]
+            error_klldfn = translations.read()["translations"]["error-klldfn"][f"{get_Language}"]
             print(error_klldfn, e)
 
 
     @client.event
     async def event_party_member_promote(old_leader: fortnitepy.PartyMember, new_leader: fortnitepy.PartyMember):
      if new_leader.id == client.user.id:
         try:
             if old_leader is not None:
-                promote_thanks_old = translations.read()["translations"]["promote-thanks_old"][get_Language]
+                promote_thanks_old = translations.read()["translations"]["promote-thanks_old"][f"{get_Language}"]
                 await client.party.send(promote_thanks_old.format(old_leader.display_name))
             else:
-                promote_thanks = translations.read()["translations"]["promote-thanks"][get_Language]
+                promote_thanks = translations.read()["translations"]["promote-thanks"][f"{get_Language}"]
                 await client.party.send(promote_thanks)
         finally:
             try:
                 await client.party.me.set_emote("EID_TrueLove")
             except:
                 pass
 
@@ -297,15 +294,15 @@
           except fortnitepy.Forbidden:
             pass
           except fortnitepy.PartyIsFull: 
             pass
         else:
           try:
             await invite.decline()
-            party_invite = translations.read()["translations"]["party-invite"][get_Language]
+            party_invite = translations.read()["translations"]["party-invite"][f"{get_Language}"]
             await invite.sender.send(party_invite)
             await invite.sender.invite()
           except fortnitepy.HTTPException:
             pass
           except AttributeError:
             pass
           except fortnitepy.PartyError:
@@ -331,36 +328,36 @@
             await friend.send("Hi {DISPLAY_NAME} u add me now \n join me for more and fun thing ! \n klldfn.xyz".replace('{DISPLAY_NAME}', friend.display_name))
             await friend.invite()
         except: pass 
 
     @client.event 
     async def event_command_error(ctx: fortnitepy.ext.commands.Context, error):
         if isinstance(error, fcommands.CommandNotFound):
-            notfound = translations.read()["translations"]["command-error-notfound"][get_Language]
+            notfound = translations.read()["translations"]["command-error-notfound"][f"{get_Language}"]
             await ctx.send(notfound)
         elif isinstance(error, IndexError):
             pass
         elif isinstance(error, fortnitepy.HTTPException):
             pass
         elif isinstance(error, fcommands.CheckFailure):
-            checfFailure = translations.read()["translations"]["command-error-checkfailure"][get_Language]
+            checfFailure = translations.read()["translations"]["command-error-checkfailure"][f"{get_Language}"]
             await ctx.send(checfFailure)
         elif isinstance(error, TimeoutError):
-            timeout = translations.read()["translations"]["command-error-timeouterror"][get_Language]
+            timeout = translations.read()["translations"]["command-error-timeouterror"][f"{get_Language}"]
             await ctx.send(timeout)
         else:
             print(error)
 
 
 
     @client.event
     async def event_party_member_join(member: fortnitepy.PartyMember) -> None:
         await set_crowns()
         #await edit_and_keep_client_member()
-        member_join = translations.read()["translations"]["member-join"][get_Language]
+        member_join = translations.read()["translations"]["member-join"][f"{get_Language}"]
         await member.party.send(member_join.format(member.display_name))
 
 
     @client.command(
     name="skin",
     aliases=[
         'outfit',
@@ -888,16 +885,16 @@
       <div class="row mt-4">
         <div class="col-lg-7 mb-lg-0 mb-4">
           <div class="card">
             <div class="card-body p-3">
               <div class="row">
                 <div class="col-lg-6">
                   <div class="d-flex flex-column h-100">
-                    <h5 class="font-weight-bolder">klldFN 2.0.0</h5>
-                    <p class="mb-5">Launch version 2.0.0</p>
+                    <h5 class="font-weight-bolder">klldFN 2.0.0b1</h5>
+                    <p class="mb-5">Available now with enhancements and fixes</p>
                     <!--
                     <a class="text-body text-sm font-weight-bold mb-0 icon-move-right mt-auto" href="javascript:;">
                       Read More
                       <i class="fas fa-arrow-right text-sm ms-1" aria-hidden="true"></i>
                     </a>
                   -->
                   </div>
@@ -926,15 +923,15 @@
           </div>
         </div>
       </div>
 
       <div class="col-12 mt-4">
         <div class="card mb-4">
           <div class="card-header pb-0 p-3">
-            <h6 class="mb-1"></h6>
+            <h6 class="mb-1">Locker</h6>
           </div>
           <div class="card-body p-3">
             <div class="row">
               <div class="col-xl-3 col-md-6 mb-xl-0 mb-4">
                 <div class="card card-blog card-plain">
                   <div class="position-relative">
                     <a class="d-block shadow-xl border-radius-xl">
```

### Comparing `klldFN-2.0.0/klldFN.egg-info/PKG-INFO` & `klldFN-2.0.0b1/klldFN.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: klldFN
-Version: 2.0.0
+Version: 2.0.0b1
 Summary: klldFN
-Home-page: https://github.com/klldtest/klldFN
+Home-page: https://klldfn.xyz
 Author: klld
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: crayons
 Requires-Dist: fortnitepy-edit
 Requires-Dist: FortniteAPIAsync==0.1.6
 Requires-Dist: sanic==20.12.0
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: aiohttp
 Requires-Dist: asyncio
 Requires-Dist: requests
-Requires-Dist: jinja2
 
-# klldFN 2.0.0
+# klldFN 2.0.0b1
 **pip install klldFN**
 
 **pip3 install klldFN**
```

### Comparing `klldFN-2.0.0/setup.py` & `klldFN-2.0.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="klldFN",
-    version="2.0.0",
+    version="2.0.0b1",
     author="klld",
     description="klldFN",
     long_description=long_description,
-    python_requires='>=3.6.0',
+    python_requires='>=3.8.0',
     long_description_content_type="text/markdown",
-    url="https://github.com/klldtest/klldFN",
+    url="https://klldfn.xyz",
     packages=setuptools.find_packages(),
     classifiers=[
           'License :: OSI Approved :: MIT License',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Programming Language :: Python :: 3.8',
@@ -32,11 +32,10 @@
           'fortnitepy-edit',
           'FortniteAPIAsync==0.1.6',
           'sanic==20.12.0',
           'requests',
           'rich',
           'aiohttp',
           'asyncio',
-          'requests',
-          'jinja2'
+          'requests'
       ],
 )
```

