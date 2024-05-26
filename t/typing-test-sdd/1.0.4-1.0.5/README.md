# Comparing `tmp/typing_test_sdd-1.0.4.tar.gz` & `tmp/typing_test_sdd-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_test_sdd-1.0.4.tar", last modified: Thu May 23 14:05:42 2024, max compression
+gzip compressed data, was "typing_test_sdd-1.0.5.tar", last modified: Sun May 26 07:59:08 2024, max compression
```

## Comparing `typing_test_sdd-1.0.4.tar` & `typing_test_sdd-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.063609 typing_test_sdd-1.0.4/typing_test_sdd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/typing_test_sdd/Assets/
--rw-r--r--   0 runner    (1001) docker     (127)    78455 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/Assets/main_image.png
--rw-r--r--   0 runner    (1001) docker     (127)    41028 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/Assets/polka.png
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-23 14:05:36.000000 typing_test_sdd-1.0.4/typing_test_sdd/words.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:05:42.067608 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 14:05:42.000000 typing_test_sdd-1.0.4/typing_test_sdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:59:08.341906 typing_test_sdd-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-26 07:59:08.337906 typing_test_sdd-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 07:59:08.341906 typing_test_sdd-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:59:08.337906 typing_test_sdd-1.0.5/typing_test_sdd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:59:08.337906 typing_test_sdd-1.0.5/typing_test_sdd/Assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    78455 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/typing_test_sdd/Assets/main_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41028 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/typing_test_sdd/Assets/polka.png
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/typing_test_sdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13735 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/typing_test_sdd/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21222 2024-05-26 07:59:00.000000 typing_test_sdd-1.0.5/typing_test_sdd/words.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 07:59:08.337906 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-26 07:59:08.000000 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-26 07:59:08.000000 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 07:59:08.000000 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-26 07:59:08.000000 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-26 07:59:08.000000 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-26 07:59:08.000000 typing_test_sdd-1.0.5/typing_test_sdd.egg-info/top_level.txt
```

### Comparing `typing_test_sdd-1.0.4/PKG-INFO` & `typing_test_sdd-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_test_sdd
-Version: 1.0.4
+Version: 1.0.5
 Summary: TKinter GUI Typing Test - Gaurav Surve 122SDD2
 Home-page: https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test
 Author: Gaurav Surve
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
@@ -41,14 +41,14 @@
     https://www.w3schools.com/python/python_json.asp
 - Stack Overflow --> Helped to get general assistance for any bugs or issues I encountered. 
     https://stackoverflow.com/
 - Github --> Repository
     https://github.com/
 - CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task.
 
-SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: https://github.com/GauravS2507/typing_test_sdd.wiki.git
+SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: [https://github.com/GauravS2507/typing_test_sdd.wiki.git](https://github.com/GauravS2507/typing_test_sdd/wiki)
 
 
 
 
 Thanks, 
 - Gaurav
```

### Comparing `typing_test_sdd-1.0.4/README.md` & `typing_test_sdd-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     https://www.w3schools.com/python/python_json.asp
 - Stack Overflow --> Helped to get general assistance for any bugs or issues I encountered. 
     https://stackoverflow.com/
 - Github --> Repository
     https://github.com/
 - CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task.
 
-SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: https://github.com/GauravS2507/typing_test_sdd.wiki.git
+SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: [https://github.com/GauravS2507/typing_test_sdd.wiki.git](https://github.com/GauravS2507/typing_test_sdd/wiki)
 
 
 
 
 Thanks, 
 - Gaurav
```

### Comparing `typing_test_sdd-1.0.4/setup.py` & `typing_test_sdd-1.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="typing_test_sdd",
-    version="1.0.4",
+    version="1.0.5",
     author="Gaurav Surve",
     url="https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test",
     description="TKinter GUI Typing Test - Gaurav Surve 122SDD2",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     platforms="any",
```

### Comparing `typing_test_sdd-1.0.4/typing_test_sdd/Assets/main_image.png` & `typing_test_sdd-1.0.5/typing_test_sdd/Assets/main_image.png`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.4/typing_test_sdd/Assets/polka.png` & `typing_test_sdd-1.0.5/typing_test_sdd/Assets/polka.png`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.4/typing_test_sdd/main.py` & `typing_test_sdd-1.0.5/typing_test_sdd/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Basic Import Functions
-import tkinter as tk
-import customtkinter as ctk
-import PIL.Image
-import random
-from pathlib import Path
-import json
-from os import path
+import tkinter as tk  # Importing tkinter library for GUI
+import customtkinter as ctk  # Importing customtkinter library for custom UI elements
+import PIL.Image  # Importing PIL library for image processing
+import random  # Importing random module for random sampling
+from pathlib import Path  # Importing Path class from pathlib module for working with file paths
+import json  # Importing json module for working with JSON files
+from os import path  # Importing path module from os for working with file paths
 
 
 # Initialize a variable to store the ID of the scheduled update
 timer_update_id = None #Boolean Variable to set whether the timer is meant to update or not
 
 
 # Defining Commands - Making Main Frame, All Widgets in 2nd Window, Each widget placed here will be represened in the main window
@@ -62,22 +62,22 @@
         container,
         text="← Go Back (Esc)",
         command=go_back,
         corner_radius=100,
         fg_color="white",
         text_color="black",
     )
-    Back.place(relx=0.1)
+    Back.place(relx=0.1) #places back button
 
     current_word_label = ctk.CTkLabel( #Current word that the user has to type
         text_container,
         text=" ".join(sampled_words[0:3]),
         font=ctk.CTkFont(size=40),
     )
-    current_word_label.place(relx=0.5, rely=0.5, anchor="c")
+    current_word_label.place(relx=0.5, rely=0.5, anchor="c") #places current word onto text container
 
     timer_label = ctk.CTkLabel( #Timer label
         text_container, text=f"Time left: {timer_seconds} seconds"
     )
     timer_label.place(relx=0.5, rely=0.7, anchor="c")
 
     current_text = "" #This variable stores what the user has typed into the entrybox and then later on checks whether the word is spelt correctly
@@ -96,60 +96,60 @@
     len_time = ctk.CTkOptionMenu( 
         settings_container,
         values=["10", "30", "60"],
         command=test_time,
         button_color="black",
         fg_color="grey",
     )
-    len_time.grid(column=0, row=1, pady=6, padx=10)
+    len_time.grid(column=0, row=1, pady=6, padx=10)#places time button
     len_time.configure(state="disable")
     len_time_label = ctk.CTkLabel(
         settings_container,
         text="Seconds",
         corner_radius=100,
         fg_color="grey",
         text_color="black",
     )
-    len_time_label.grid(column=0, row=0, pady=8, padx=10)
+    len_time_label.grid(column=0, row=0, pady=8, padx=10)#places time button
 
     modes = ctk.CTkOptionMenu( #Options for mode the user wants, system, dark or light
         settings_container,
         values=["dark", "light", "system"],
         command= ctk.set_appearance_mode,
         button_color="black",
         fg_color="grey",
     )
-    modes.grid(column=0, row=3, pady=6, padx=10)
+    modes.grid(column=0, row=3, pady=6, padx=10) #places modes button
     modes_label = ctk.CTkLabel(
         settings_container,
         text="Modes",
         corner_radius=100,
         fg_color="grey",
         text_color="black",
     )
-    modes_label.grid(column=0, row=2, pady=6, padx=10)
+    modes_label.grid(column=0, row=2, pady=6, padx=10) #places modes button
     modes.set("system")
     modes.set(ctk.get_appearance_mode())
 
     scale = ctk.CTkOptionMenu( #Options for the scale the user wants to use
         settings_container,
         values=["0.75", "1.0", "1.25"],
         command=scaling,
         button_color="black",
         fg_color="grey",
     )
-    scale.grid(column=0, row=5, pady=8, padx=10)
+    scale.grid(column=0, row=5, pady=8, padx=10)#places scale button
     scale_label = ctk.CTkLabel(
         settings_container,
         text="UI Scale",
         corner_radius=100,
         fg_color="grey",
         text_color="black",
     )
-    scale_label.grid(column=0, row=4, pady=6, padx=10)
+    scale_label.grid(column=0, row=4, pady=6, padx=10)#places scale button
     scale.set(current_scaling)
   
     Restart_button = ctk.CTkButton( #To restart the test
         typing_container,
         text="Restart (Enter)",
         command=restart,
         fg_color="grey",
@@ -250,18 +250,14 @@
         elif value == 30:
             wpm_label.configure(text=f"WPM: {score * 2} ")
         else:
             wpm_label.configure(text=f"WPM: {score} ")
         typing_box.configure(state="disable")
 
 
-def invoke_begin():
-    Begin_TTH.invoke()
-
-
 # Starts timer
 def start_timer(duration):
     global timer_seconds
     timer_seconds = duration
     update_timer()
 
 
@@ -288,91 +284,92 @@
     is_on_typing_window = False
     
     # main_window
     main_window = ctk.CTkFrame(
         root, width=400, height=500, border_width=10
     )  # border_color = "#13141F") )
 
-    dummy_widget = ctk.CTkLabel(
+    dummy_widget = ctk.CTkLabel( #holds main window's image 
         main_window,
         text="",
         image=ctk.CTkImage(
             PIL.Image.open(
                 Path(__file__).resolve().parents[0] / path.join("Assets", "polka.png")
             ),
             size=(1400, 700),
         ),
     )
 
-    # Labels Used
+    # Labels Used in main window
     Welcome_TTH = ctk.CTkLabel(
         main_window,
         text="Welcome to the Touch Type Helper",
         font=("Work Sans", 24),
         fg_color="#272626",
         text_color= "white",
         corner_radius=1,
     )
 
-    # Buttons
-    Begin_TTH = ctk.CTkButton(
+    # Buttons in main window
+    Begin_TTH = ctk.CTkButton( #Begin button
         main_window,
         text="Begin (⇧ + ↵)",
         font=("Arial", 16),
         fg_color="#272626",
         command=create_typing,
     )
 
-    EndProgram = ctk.CTkButton(
+    EndProgram = ctk.CTkButton( #End program button
         main_window,
         text="End Program (⇧ + Esc)",
         font=("Arial", 16),
         fg_color="#272626",
         command=root.destroy,
     )
 
-    Credits = ctk.CTkButton(
+    Credits = ctk.CTkButton( #Credits buttton
         main_window,
         text="Credits",
         font=("Arial", 16),
         fg_color="#272626",
         command=credits,
     )
 
 
 
-def keybind(button, action):
+def keybind(button, action): #Function to make sure that keybinds only work when the correct window is opened. 
     global is_on_main_window, is_on_typing_window
-    if action in actions[0:2] and is_on_main_window:
+    if action in actions[0:2] and is_on_main_window: #if the user is on the main window only the begin and end program keybinds work
         button.invoke()
-    elif action in actions[2:4] and is_on_typing_window:
+    elif action in actions[2:4] and is_on_typing_window: #If users is on the typing window only the back and restart button work
         button.invoke()
 
-def start_app():
+def start_app(): #Function to begin app when it is called through the temrinal
     try:
         global current_scaling, timer_seconds, score, root, timer_choice, is_on_main_window, is_on_typing_window, scale, actions 
         get_words()
         timer_seconds = 10
         score = 0  # Keeps score on how many words are right
-        is_on_main_window = False
-        is_on_typing_window = False
+        is_on_main_window = False #Sets variabel to false when program is intially run
+        is_on_typing_window = False#Sets variabel to false when program is intially run
         actions = ["to_typing_window", "do_exit", "do_restart", "to_main_window"]
         current_scaling = "1.0"
-
+#Basic UI 
         root = ctk.CTk()
         root.geometry("1400x700")
         root.title("Touch Typing Helper - Gaurav Surve")
         make_main_window()
         place_main_window_content()
-        root.bind("<Shift-Return>", lambda e: keybind(Begin_TTH, actions[0]))
+        #Assigning values to keybinds to make sure that they only work when called
+        root.bind("<Shift-Return>", lambda e: keybind(Begin_TTH, actions[0])) 
         root.bind("<Shift-Escape>", lambda e: keybind(EndProgram, actions[1]))
         root.bind("<Return>", lambda e: keybind(Restart_button, actions[2]))
         root.bind("<Escape>", lambda e: keybind(Back, actions[3]))
         root.mainloop()
 
     except Exception as ex:
         with open ("test.txt", "x") as f:
-            f.write(f"{type(ex).__name__} {ex}")
+            f.write(f"{type(ex).__name__} {ex}") #pypi package
 
 # Main variables for when program is started
 if __name__ == "__main__":
     start_app()
```

### Comparing `typing_test_sdd-1.0.4/typing_test_sdd/words.json` & `typing_test_sdd-1.0.5/typing_test_sdd/words.json`

 * *Files identical despite different names*

### Comparing `typing_test_sdd-1.0.4/typing_test_sdd.egg-info/PKG-INFO` & `typing_test_sdd-1.0.5/typing_test_sdd.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_test_sdd
-Version: 1.0.4
+Version: 1.0.5
 Summary: TKinter GUI Typing Test - Gaurav Surve 122SDD2
 Home-page: https://github.com/GauravS2507/Gaurav-Surve-SDD2-Project---Typing-Test
 Author: Gaurav Surve
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Education
@@ -41,14 +41,14 @@
     https://www.w3schools.com/python/python_json.asp
 - Stack Overflow --> Helped to get general assistance for any bugs or issues I encountered. 
     https://stackoverflow.com/
 - Github --> Repository
     https://github.com/
 - CHATGPT was used to source words for my words.json list. This was the fastest way to source words for this project, and the only time any AI was used in the making of this task.
 
-SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: https://github.com/GauravS2507/typing_test_sdd.wiki.git
+SEE WIKI FOR ADDITIONAL INFORMATION/ASSISTANCE: [https://github.com/GauravS2507/typing_test_sdd.wiki.git](https://github.com/GauravS2507/typing_test_sdd/wiki)
 
 
 
 
 Thanks, 
 - Gaurav
```

