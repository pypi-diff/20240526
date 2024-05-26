# Comparing `tmp/pipackager-0.3.0.tar.gz` & `tmp/pipackager-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipackager-0.3.0.tar", last modified: Sat May 25 21:03:34 2024, max compression
+gzip compressed data, was "pipackager-0.3.1.tar", last modified: Sun May 26 02:11:07 2024, max compression
```

## Comparing `pipackager-0.3.0.tar` & `pipackager-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:03:34.404252 pipackager-0.3.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.3.0/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-25 21:03:34.404252 pipackager-0.3.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.3.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:03:34.400252 pipackager-0.3.0/pipackager/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.3.0/pipackager/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11401 2024-05-25 21:02:24.000000 pipackager-0.3.0/pipackager/cli.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:03:34.400252 pipackager-0.3.0/pipackager.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-25 21:03:34.000000 pipackager-0.3.0/pipackager.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-25 21:03:34.000000 pipackager-0.3.0/pipackager.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 21:03:34.000000 pipackager-0.3.0/pipackager.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-25 21:03:34.000000 pipackager-0.3.0/pipackager.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-25 21:03:34.000000 pipackager-0.3.0/pipackager.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-25 21:03:34.000000 pipackager-0.3.0/pipackager.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 21:03:34.404252 pipackager-0.3.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1511 2024-05-25 21:03:28.000000 pipackager-0.3.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 21:03:34.404252 pipackager-0.3.0/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.3.0/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.3.0/tests/test_pipackager.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:11:07.476693 pipackager-0.3.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1060 2024-05-25 20:25:24.000000 pipackager-0.3.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:11:07.476693 pipackager-0.3.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-05-25 20:55:56.000000 pipackager-0.3.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:11:07.476693 pipackager-0.3.1/pipackager/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-25 20:26:07.000000 pipackager-0.3.1/pipackager/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14144 2024-05-26 02:08:12.000000 pipackager-0.3.1/pipackager/cli.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:11:07.476693 pipackager-0.3.1/pipackager.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4562 2024-05-26 02:11:07.000000 pipackager-0.3.1/pipackager.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      316 2024-05-26 02:11:07.000000 pipackager-0.3.1/pipackager.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-26 02:11:07.000000 pipackager-0.3.1/pipackager.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2024-05-26 02:11:07.000000 pipackager-0.3.1/pipackager.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       56 2024-05-26 02:11:07.000000 pipackager-0.3.1/pipackager.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2024-05-26 02:11:07.000000 pipackager-0.3.1/pipackager.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-26 02:11:07.476693 pipackager-0.3.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1511 2024-05-26 02:10:37.000000 pipackager-0.3.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-26 02:11:07.476693 pipackager-0.3.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       31 2024-05-25 20:26:07.000000 pipackager-0.3.1/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       76 2024-05-25 20:47:17.000000 pipackager-0.3.1/tests/test_pipackager.py
```

### Comparing `pipackager-0.3.0/LICENSE` & `pipackager-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipackager-0.3.0/PKG-INFO` & `pipackager-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/yourusername/pipackager
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.3.0/README.md` & `pipackager-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pipackager-0.3.0/pipackager/cli.py` & `pipackager-0.3.1/pipackager/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 import sys
 
 def show_menu():
     clear()
     print("***********************************")
     print("*        PyPI Package Manager     *")
     print("***********************************")
-    print("1. Clean old distributions")
-    print("2. Build new distributions")
-    print("3. Upload distributions to PyPI")
-    print("4. Increment version number (patch)")
-    print("5. Increment version number (minor)")
-    print("6. Increment version number (major)")
-    print("7. Advanced options")
-    print("8. Help")
-    print("9. Exit")
-
+    print("1. Initial Setup")
+    print("2. Clean old distributions")
+    print("3. Build new distributions")
+    print("4. Upload distributions to PyPI")
+    print("5. Increment version number (patch)")
+    print("6. Increment version number (minor)")
+    print("7. Increment version number (major)")
+    print("8. Advanced options")
+    print("9. Help")
+    print("10. Exit")
 
 def show_advanced_menu():
     clear()
     print("***********************************")
     print("*        Advanced Options         *")
     print("***********************************")
     print("1. Create/update .github workflow")
     print("2. Run tests using Pytest")
     print("3. Lint and format code")
     print("4. Check and update dependencies")
     print("5. Generate start command")
-    print("6. Back to main menu")
+    print("6. Reconfigure setup.py")
+    print("7. Back to main menu")
 
 
 def show_help():
     clear()
     print("***********************************")
     print("*           Help Overview         *")
     print("***********************************")
@@ -60,14 +61,98 @@
     print("3. Lint and format code: Lints and formats code using flake8 and black.")
     print("4. Check and update dependencies: Checks and updates package dependencies.")
     print("5. Generate start command: Generates a start command for your library.")
     print("6. Back to main menu: Returns to the main menu.")
     print("")
     input("Press any key to return to the main menu...")
 
+def initial_setup():
+    check_github_workflow()
+    check_setup_py()
+
+def check_github_workflow():
+    workflow_path = '.github/workflows/python-package.yml'
+    if not os.path.exists(workflow_path):
+        print(f"⚠️  GitHub workflow not found at {workflow_path}. Creating...")
+        create_update_workflow()
+    else:
+        print(f"✅ GitHub workflow already exists at {workflow_path}")
+
+def check_setup_py():
+    setup_path = 'setup.py'
+    if not os.path.exists(setup_path):
+        print(f"⚠️  setup.py not found. Creating...")
+        create_setup_py()
+    else:
+        print(f"✅ setup.py already exists")
+
+def create_setup_py():
+    name = input("Enter the package name: ")
+    version = input("Enter the package version (e.g., 0.1.0): ")
+    author = input("Enter the author's name: ")
+    author_email = input("Enter the author's email: ")
+    description = input("Enter the package description: ")
+    url = input("Enter the package URL: ")
+
+    setup_contents = f"""
+from setuptools import setup, find_packages
+from pathlib import Path
+
+# Read the contents of README.md
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+setup(
+    name='{name}',
+    version='{version}',
+    packages=find_packages(),
+    install_requires=[
+        'twine',
+        'setuptools',
+        'wheel',
+        'flake8',
+        'black',
+        'pytest',
+        'pip-upgrader',
+    ],
+    entry_points={{
+        'console_scripts': [
+            '{name}={name}.cli:main',
+        ],
+    }},
+    author='{author}',
+    author_email='{author_email}',
+    description='{description}',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='{url}',
+    license='Apache License 2.0',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Libraries :: Application Frameworks',
+        'License :: OSI Approved :: Apache Software License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+    ],
+)
+"""
+    with open('setup.py', 'w') as file:
+        file.write(setup_contents)
+    print(f"✅ setup.py created")
+
+def reconfigure_setup_py():
+    if os.path.exists('setup.py'):
+        os.remove('setup.py')
+    create_setup_py()
+    print(f"✅ setup.py reconfigured")
+
 
 def clear():
     os.system("cls" if os.name == "nt" else "clear")
 
 
 def clean_dists():
     dist_dir = 'dist'
@@ -295,55 +380,58 @@
 
 
 def main_menu():
     while True:
         show_menu()
         choice = input("Select an option: ")
 
-        if choice == "1":
+        if choice == '1':
+            initial_setup()
+        elif choice == '2':
             clean_dists()
-        elif choice == "2":
+        elif choice == '3':
             build_dists()
-        elif choice == "3":
+        elif choice == '4':
             upload_dists()
-        elif choice == "4":
-            increment_version("patch")
-        elif choice == "5":
-            increment_version("minor")
-        elif choice == "6":
-            increment_version("major")
-        elif choice == "7":
+        elif choice == '5':
+            increment_version('patch')
+        elif choice == '6':
+            increment_version('minor')
+        elif choice == '7':
+            increment_version('major')
+        elif choice == '8':
             advanced_menu()
-        elif choice == "8":
+        elif choice == '9':
             show_help()
-        elif choice == "9":
+        elif choice == '10':
             print("Goodbye! 👋")
             break
         else:
             print("❌ Invalid option, please try again.")
 
         input("\nPress any key to continue...")
 
-
 def advanced_menu():
     while True:
         show_advanced_menu()
         adv_choice = input("Select an advanced option: ")
 
-        if adv_choice == "1":
+        if adv_choice == '1':
             create_update_workflow()
-        elif adv_choice == "2":
+        elif adv_choice == '2':
             run_tests()
-        elif adv_choice == "3":
+        elif adv_choice == '3':
             lint_format_code()
-        elif adv_choice == "4":
+        elif adv_choice == '4':
             check_update_dependencies()
-        elif adv_choice == "5":
+        elif adv_choice == '5':
             generate_start_command()
-        elif adv_choice == "6":
+        elif adv_choice == '6':
+            reconfigure_setup_py()
+        elif adv_choice == '7':
             break
         else:
             print("❌ Invalid option, please try again.")
 
         input("\nPress any key to continue...")
```

### Comparing `pipackager-0.3.0/pipackager.egg-info/PKG-INFO` & `pipackager-0.3.1/pipackager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipackager
-Version: 0.3.0
+Version: 0.3.1
 Summary: A tool to manage your PyPI package.
 Home-page: https://github.com/yourusername/pipackager
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pipackager-0.3.0/setup.py` & `pipackager-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pipackager",
-    version="0.3.0",
+    version="0.3.1",
     packages=find_packages(),
     install_requires=[
         "twine",
         "setuptools",
         "wheel",
         "flake8",
         "black",
```

