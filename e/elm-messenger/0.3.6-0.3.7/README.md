# Comparing `tmp/elm_messenger-0.3.6.tar.gz` & `tmp/elm_messenger-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm_messenger-0.3.6.tar", last modified: Thu May 23 02:26:18 2024, max compression
+gzip compressed data, was "elm_messenger-0.3.7.tar", last modified: Sun May 26 14:42:15 2024, max compression
```

## Comparing `elm_messenger-0.3.6.tar` & `elm_messenger-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      888 2024-05-15 03:21:04.000000 elm_messenger-0.3.6/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1159 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-23 02:26:18.000000 elm_messenger-0.3.6/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-23 02:26:18.946915 elm_messenger-0.3.6/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    16639 2024-05-23 02:21:06.000000 elm_messenger-0.3.6/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1090 2024-05-15 18:35:42.000000 elm_messenger-0.3.6/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2024-05-23 02:26:18.950249 elm_messenger-0.3.6/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.6/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-26 14:42:15.898825 elm_messenger-0.3.7/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2024-05-04 14:47:23.000000 elm_messenger-0.3.7/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1052 2024-05-26 14:42:15.898825 elm_messenger-0.3.7/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      781 2024-05-24 23:29:13.000000 elm_messenger-0.3.7/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-26 14:42:15.898825 elm_messenger-0.3.7/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1052 2024-05-26 14:42:15.000000 elm_messenger-0.3.7/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2024-05-26 14:42:15.000000 elm_messenger-0.3.7/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2024-05-26 14:42:15.000000 elm_messenger-0.3.7/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2024-05-26 14:42:15.000000 elm_messenger-0.3.7/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2024-05-26 14:42:15.000000 elm_messenger-0.3.7/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2024-05-26 14:42:15.000000 elm_messenger-0.3.7/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-26 14:42:15.898825 elm_messenger-0.3.7/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2024-05-04 14:47:23.000000 elm_messenger-0.3.7/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2024-05-04 14:47:23.000000 elm_messenger-0.3.7/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    16736 2024-05-26 13:45:33.000000 elm_messenger-0.3.7/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1090 2024-05-15 18:35:42.000000 elm_messenger-0.3.7/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      392 2024-05-26 14:42:15.898825 elm_messenger-0.3.7/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2024-05-04 14:47:23.000000 elm_messenger-0.3.7/setup.py
```

### Comparing `elm_messenger-0.3.6/PKG-INFO` & `elm_messenger-0.3.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.6
+Version: 0.3.7
 Summary: The Messenger toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -23,15 +23,12 @@
 
 - Engine in a library. Messenger core is built in a library.
 - Message (or event) based. Faster development cycle, easier to divide work.
 - Functional, but OOP styled. Take advantages of both functional programming and OOP.
 
 ## Conceptual Picture
 
-![](docs/imgs/concept.png)
-
-- Red arrow: messages that are sent positively
-- Orange arrow: messages that are triggered passively
+![](docs/concept.png)
 
 ## Tutorial/Guide
 
 [Full documentation](https://typst.app/project/rytMGqODAPcw9-39Fec_aB) is hosted on Typst.
```

### Comparing `elm_messenger-0.3.6/Readme.md` & `elm_messenger-0.3.7/Readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,12 @@
 
 - Engine in a library. Messenger core is built in a library.
 - Message (or event) based. Faster development cycle, easier to divide work.
 - Functional, but OOP styled. Take advantages of both functional programming and OOP.
 
 ## Conceptual Picture
 
-![](docs/imgs/concept.png)
-
-- Red arrow: messages that are sent positively
-- Orange arrow: messages that are triggered passively
+![](docs/concept.png)
 
 ## Tutorial/Guide
 
 [Full documentation](https://typst.app/project/rytMGqODAPcw9-39Fec_aB) is hosted on Typst.
```

### Comparing `elm_messenger-0.3.6/elm_messenger.egg-info/PKG-INFO` & `elm_messenger-0.3.7/elm_messenger.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-messenger
-Version: 0.3.6
+Version: 0.3.7
 Summary: The Messenger toolkit for Elm
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -23,15 +23,12 @@
 
 - Engine in a library. Messenger core is built in a library.
 - Message (or event) based. Faster development cycle, easier to divide work.
 - Functional, but OOP styled. Take advantages of both functional programming and OOP.
 
 ## Conceptual Picture
 
-![](docs/imgs/concept.png)
-
-- Red arrow: messages that are sent positively
-- Orange arrow: messages that are triggered passively
+![](docs/concept.png)
 
 ## Tutorial/Guide
 
 [Full documentation](https://typst.app/project/rytMGqODAPcw9-39Fec_aB) is hosted on Typst.
```

### Comparing `elm_messenger-0.3.6/messengercli/messenger.py` & `elm_messenger-0.3.7/messengercli/messenger.py`

 * *Files 4% similar despite different names*

```diff
@@ -230,15 +230,18 @@
             if scene not in self.config["sceneprotos"]:
                 raise Exception("Scene doesn't exist.")
             if layer in self.config["sceneprotos"][scene]["layers"]:
                 raise Exception("Layer already exists.")
             if has_component and not os.path.exists(
                 f"src/SceneProtos/{scene}/{dir}/ComponentBase.elm"
             ):
-                raise Exception("Please first create a component.")
+                Updater(
+                    [".messenger/component/ComponentBase.elm"],
+                    [f"src/SceneProtos/{scene}/{dir}/ComponentBase.elm"],
+                ).rep("SceneProtos").rep(scene).rep(dir)
 
             if not os.path.exists(f"src/SceneProtos/{scene}/SceneBase.elm"):
                 Updater(
                     [".messenger/sceneproto/SceneBase.elm"],
                     [f"src/SceneProtos/{scene}/SceneBase.elm"],
                 ).rep(scene)
             self.config["sceneprotos"][scene]["layers"].append(layer)
@@ -271,15 +274,18 @@
             if scene not in self.config["scenes"]:
                 raise Exception("Scene doesn't exist.")
             if layer in self.config["scenes"][scene]["layers"]:
                 raise Exception("Layer already exists.")
             if has_component and not os.path.exists(
                 f"src/Scenes/{scene}/{dir}/ComponentBase.elm"
             ):
-                raise Exception("Please first create a component.")
+                Updater(
+                    [".messenger/component/ComponentBase.elm"],
+                    [f"src/Scenes/{scene}/{dir}/ComponentBase.elm"],
+                ).rep("Scenes").rep(scene).rep(dir)
 
             if not os.path.exists(f"src/Scenes/{scene}/SceneBase.elm"):
                 Updater(
                     [".messenger/scene/SceneBase.elm"],
                     [f"src/Scenes/{scene}/SceneBase.elm"],
                 ).rep(scene)
             self.config["scenes"][scene]["layers"].append(layer)
@@ -329,15 +335,15 @@
         "-t",
         help="Use customized repository for cloning templates.",
     ),
     template_tag=typer.Option(
         None,
         "--template-tag",
         "-b",
-        help="Use the tag or branch of the repository to clone",
+        help="Use the tag or branch of the repository to clone.",
     ),
 ):
     input(
         f"""Thanks for using Messenger.
 See https://github.com/linsyking/Messenger.git for more information.
 Here is my plan:
 
@@ -379,50 +385,39 @@
 
 
 @app.command()
 def component(
     scene: str,
     name: str,
     compdir: str = typer.Option(
-        "Components", "--cdir", "-cd", help="Directory to store components"
+        "Components", "--cdir", "-cd", help="Directory to store components."
     ),
     is_proto: bool = typer.Option(
-        False, "--proto", "-p", help="Create a component in sceneproto"
+        False, "--proto", "-p", help="Create a component in sceneproto."
     ),
-    init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file"),
+    init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file."),
 ):
     name = check_name(name)
     scene = check_name(scene)
     compdir = check_name(compdir)
     msg = Messenger()
     input(
         f"You are going to create a component named {name} in {'SceneProtos' if is_proto else 'Scenes'}/{scene}/{compdir}, continue?"
     )
     msg.add_component(name, scene, compdir, is_proto, init)
     msg.format()
     print("Done!")
 
 
 @app.command()
-def update():
-    msg = Messenger()
-    input(f"You are going to regenerate elm files based on settings, continue?")
-    msg.update_scenes()
-    msg.format()
-    print("Done!")
-
-
-@app.command()
 def scene(
     name: str,
-    raw: bool = typer.Option(False, "--raw", help="Use raw scene without layers"),
-    is_proto: bool = typer.Option(
-        False, "--proto", "-p", help="Create a sceneproto"
-    ),
-    init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file"),
+    raw: bool = typer.Option(False, "--raw", help="Use raw scene without layers."),
+    is_proto: bool = typer.Option(False, "--proto", "-p", help="Create a sceneproto."),
+    init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file."),
 ):
     name = check_name(name)
     msg = Messenger()
     input(
         f"You are going to create a {'raw ' if raw else ''}{'sceneproto' if is_proto else 'scene'} named {name}, continue?"
     )
     msg.add_scene(name, raw, is_proto, init)
@@ -446,23 +441,23 @@
 
 
 @app.command()
 def layer(
     scene: str,
     layer: str,
     has_component: bool = typer.Option(
-        False, "--with-component", "-c", help="Use components in this layer"
+        False, "--with-component", "-c", help="Use components in this layer."
     ),
     compdir: str = typer.Option(
-        "Components", "--cdir", "-cd", help="Directory of components in the scene"
+        "Components", "--cdir", "-cd", help="Directory of components in the scene."
     ),
     is_proto: bool = typer.Option(
-        False, "--proto", "-p", help="Create a layer in sceneproto"
+        False, "--proto", "-p", help="Create a layer in sceneproto."
     ),
-    init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file"),
+    init: bool = typer.Option(False, "--init", "-i", help="Create a `Init.elm` file."),
 ):
     scene = check_name(scene)
     layer = check_name(layer)
     msg = Messenger()
     input(
         f"You are going to create a layer named {layer} under {'sceneproto' if is_proto else 'scene'} {scene}, continue?"
     )
```

### Comparing `elm_messenger-0.3.6/messengercli/updater.py` & `elm_messenger-0.3.7/messengercli/updater.py`

 * *Files identical despite different names*

