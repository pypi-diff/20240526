# Comparing `tmp/preprod-0.1.0.tar.gz` & `tmp/preprod-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprod-0.1.0.tar", max compression
+gzip compressed data, was "preprod-0.2.0.tar", max compression
```

## Comparing `preprod-0.1.0.tar` & `preprod-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2024-05-04 07:46:13.142433 preprod-0.1.0/LICENSE
--rw-r--r--   0        0        0      154 2024-05-21 19:06:48.611820 preprod-0.1.0/README.md
--rw-r--r--   0        0        0      143 2024-05-04 07:46:13.144433 preprod-0.1.0/preprod/__init__.py
--rw-r--r--   0        0        0     7833 2024-05-21 18:50:11.667872 preprod-0.1.0/preprod/commons.py
--rw-r--r--   0        0        0     3737 2024-05-20 19:01:26.434508 preprod-0.1.0/preprod/core.py
--rw-r--r--   0        0        0      424 2024-05-21 19:00:26.254891 preprod-0.1.0/preprod/locale/en/LC_MESSAGES/preprod.mo
--rw-r--r--   0        0        0      738 2024-05-04 07:46:13.144433 preprod-0.1.0/preprod/locale/en.po
--rw-r--r--   0        0        0     1227 2024-05-21 19:06:48.612820 preprod-0.1.0/preprod/locale/es/LC_MESSAGES/preprod.mo
--rw-r--r--   0        0        0     2452 2024-05-21 19:06:48.611820 preprod-0.1.0/preprod/locale/es.po
--rw-r--r--   0        0        0     1988 2024-05-21 19:06:48.612820 preprod-0.1.0/preprod/locale/preprod.pot
--rw-r--r--   0        0        0     1253 2024-05-21 19:06:48.612820 preprod-0.1.0/preprod/poethepoet.py
--rw-r--r--   0        0        0      167 2024-05-04 08:31:09.575065 preprod-0.1.0/preprod/tests/test_commons.py
--rw-r--r--   0        0        0      827 2024-05-20 19:01:57.745509 preprod-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 preprod-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-04 07:46:13.142433 preprod-0.2.0/LICENSE
+-rw-r--r--   0        0        0      313 2024-05-26 18:08:54.806898 preprod-0.2.0/README.md
+-rw-r--r--   0        0        0      144 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/__init__.py
+-rw-r--r--   0        0        0     9742 2024-05-26 18:03:08.573887 preprod-0.2.0/preprod/commons.py
+-rw-r--r--   0        0        0     4579 2024-05-26 17:09:10.902231 preprod-0.2.0/preprod/core.py
+-rw-r--r--   0        0        0      424 2024-05-26 18:06:43.770894 preprod-0.2.0/preprod/locale/en/LC_MESSAGES/preprod.mo
+-rw-r--r--   0        0        0      738 2024-05-04 07:46:13.144433 preprod-0.2.0/preprod/locale/en.po
+-rw-r--r--   0        0        0     1480 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/locale/es/LC_MESSAGES/preprod.mo
+-rw-r--r--   0        0        0     2662 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/locale/es.po
+-rw-r--r--   0        0        0     2026 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/locale/preprod.pot
+-rw-r--r--   0        0        0     1253 2024-05-21 19:06:48.612820 preprod-0.2.0/preprod/poethepoet.py
+-rw-r--r--   0        0        0      167 2024-05-04 08:31:09.575065 preprod-0.2.0/preprod/tests/test_commons.py
+-rw-r--r--   0        0        0      827 2024-05-26 18:08:54.807898 preprod-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 preprod-0.2.0/PKG-INFO
```

### Comparing `preprod-0.1.0/LICENSE` & `preprod-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preprod-0.1.0/preprod/commons.py` & `preprod-0.2.0/preprod/commons.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,85 +3,100 @@
 from importlib.resources import files
 from os import getuid, path, listdir, remove, chdir as os_chdir, system  as os_system
 from shutil import copyfile as shutil_copyfile, rmtree as shutil_rmtree
 from socket import create_connection
 from subprocess import run
 from sys import exit, stdout
 
+
+
 try:
     t=translation('preprod', files("preprod") / 'locale')
     _=t.gettext
 except:
     _=str
 
+
+
 def red(s):
         return Fore.RED + Style.BRIGHT + s + Style.RESET_ALL
         
 def green(s):
         return Fore.GREEN + Style.BRIGHT + s + Style.RESET_ALL
 
 def yellow(s):
         return Fore.YELLOW+ Style.BRIGHT + s + Style.RESET_ALL
 
 def white(s):
         return Style.BRIGHT + s + Style.RESET_ALL
 
 def press_a_key_to_continue():
-    system("read -p '{0}".format(_("Press a key to continue...")))
+    from preprod.core import concurrent_log
+    concurrent_log("Before press a key to continue...")
+    system("read -p '{0}'".format(_("Press a key to continue...")))
+    concurrent_log("After press a key to continue...")
 
 def nmcli_net_change(netname, check_host,  check_port, description=""):
     """
         Parameters:
             - netname with Networkmanager: str
             - ip to check: str or name
             - port to check: int
             - description="" Default description. None doesn't print anything
     """
     if description is not None:
         print_before(_("Changing net to {0}").format(netname) )
     
     retry=1
+    from preprod.core import concurrent_log
+    concurrent_log(f"Before changing net to {netname}")
     while True:
             run(f"nmcli connection up {netname}", shell=True,  capture_output=True)
             for i in range(3):
                 try:
                     with create_connection((check_host, check_port), timeout=1 ):
                         if description is not None:
                             print_after_ok()
+                        concurrent_log(f"After changing net to {netname}")
                         return
                 except:
                     if retry==1:
                         print(" " * 12, end="")
                         stdout.flush()
                     s=f"[Retrying {retry}]"
                     print("\b"*len(s)+ yellow(s),  end="")
                     stdout.flush()
                     retry+=1
 
+
 def replace_in_file(filename, s, r,description=""):
     if description is not None:
         print_before(_("Replacing values in {0}").format(filename))
     data=open(filename,"r").read()
     remove(filename)
     data=data.replace(s,r)
     with open(filename, "w") as f:
         f.write(data)
     
     if description is not None:
         print_after_ok()
+    from preprod.core import concurrent_log
+    concurrent_log(f"Replaced in file '{filename}', '{s}' by '{r}'")
 
 def lines_at_the_end_of_file(filename, s, description=""):
     if description is not None:
         print_before(_("Appending text at the end of {0}").format(filename))
     with open(filename, 'a') as f:
         f.write(s)
     if description is not None:
         print_after_ok()
+    from preprod.core import concurrent_log
+    concurrent_log(f"Added at the of file '{filename}'", s)
 
-def run_and_check(command,  description=None,  expected_returncode=0,  expected_stdout=None, verbose=True):
+def run_and_check(command,  description=None,  expected_returncode=0,  expected_stdout=None):
     """
         Executes a comand and returns a boolean if command was executed as expected
         
         Parameters:
             - verbose. If true shows stdout and stderr
             - description. None makes not output, "" print command, else prints else
     """
@@ -99,27 +114,26 @@
     if expected_stdout is not None:
         print(expected_stdout, )
         r= expected_stdout in p.stdout.decode('utf-8')
         r=True
     elif p.returncode==expected_returncode:
         r=True
     
-    if r is False and verbose is True:
-        print(f"Error en comando. {command}")
-        print("STDOUT:")
-        print(p.stdout.decode('utf-8'))
-        print("STDERR:")
-        print(p.stderr.decode('utf-8'))
-        print(_("Exiting propred..."))
         
     if description is not None:
         if r is True:
             print (f"[{green('OK')}]")
         else:
             print (f"[{red('ERROR')}]")
+            
+    from preprod.core import concurrent_log
+    stdout_=p.stdout.decode('utf-8')
+    stderr_=p.stderr.decode('utf-8')
+    concurrent_log(f"run_and_check('{command}')",  stdout_, stderr_)
+
     return r
 
 def print_before(s, show=True):
     if show:
         print (f"  - {s} ",  end="")
         stdout.flush()
 
@@ -128,23 +142,29 @@
         print (f"[{green('OK')}]")
 
 def print_after_error(show=True):
     if show:
         print (f"[{red('ERROR')}]")
 
 def system(command):
+    from preprod.core import concurrent_log
+    concurrent_log(f"system('{command}')")
     os_system(command)
 
 def rmtree(directory, show=True):
     print_before(_("Deleting directory {0}").format(directory),show)
     shutil_rmtree(directory, ignore_errors=True)
     print_after_ok(show)
+    from preprod.core import concurrent_log
+    concurrent_log(f"rmtree('{directory}')")
     
 def chdir(directory, show=True):
+    from preprod.core import concurrent_log
     print_before(_("Changing to directory {0}").format(directory),show)
+    concurrent_log(f"chdir('{directory}')")
     os_chdir(directory)
     print_after_ok(show)
 
 def git_clone(url):
     run_and_check(f"git clone {url}", description=f"Cloning git repository {url}")
 
 def git_pull():
@@ -173,39 +193,48 @@
     lines.insert(line_number, text + '\n')
 
     with open(file_path, 'w') as file:
         file.writelines(lines)
 
     if description is not None:
         print_after_ok()
+        
+    from preprod.core import concurrent_log
+    concurrent_log(f"insert_at_line('{file_path}', {line_number})", text)
 
 
 def copyfile(from_,  to_):
     shutil_copyfile(from_,  to_)
+    from preprod.core import concurrent_log
+    concurrent_log(f"copyfile('{from_}', '{to_}')")
 
 def delete_line_in_file(file_path, line_number, description=""):
     if description is not None:
         print_before(_("Deleting line {0} in {1}").format(line_number, file_path))
 
     with open(file_path, 'r') as file:
         lines = file.readlines()
 
     # Adjust line number to zero-based index
     line_number -= 1
 
     if line_number < 0 or line_number >= len(lines):
         raise IndexError(_("Line number is out of range"))
+        
+    to_delete=lines[line_number]
 
     del lines[line_number]
 
     with open(file_path, 'w') as file:
         file.writelines(lines)
 
     if description is not None:
         print_after_ok()
+    from preprod.core import concurrent_log
+    concurrent_log(f"delete_line_in_file('{file_path}', {line_number})", None,  to_delete)
 
 
 
 def is_root():
     """
         Returns if current user is root
     """
@@ -243,22 +272,34 @@
 
 def create_python_virtual_env(python_version_name="python3.11", system_site_packages=False):
     """
         Will create a python virtual env in .python_version_name with python_version_name executable
         Parameters:
            - python_version_name: str: python3.11
     """
-    str_sss=""
-    if system_site_packages:
-        str_sss="--system-site-packages"
-    
-    
+    str_sss="--system-site-packages" if system_site_packages else ""
     run_and_check(f"{python_version_name} -m venv {str_sss} .{python_version_name}", description= f"Creating virtual env at .{python_version_name}")
-    return ".python3.11/bin/python3", ".python3.11/bin/pip"
+    return path.abspath(".python3.11/bin/python3"), path.abspath(".python3.11/bin/pip")
 
 def apache_initd_restart():
     run_and_check("/etc/init.d/apache2 restart", "Restarting apache server")
     
+def chown_recursive(path,  user="root",  group="root"):
+    run_and_check(f"find {path} -type f -exec chown -R {user}:{group} {{}} +")
+
+def chmod_recursive(path,  directory_permissions="755",  file_permissions="644" ):
+    run_and_check(f"find {path} -type d -exec chmod -R {directory_permissions} {{}} +")
+    run_and_check(f"find {path} -type f -exec chmod -R {file_permissions} {{}} +")
 
 def npm_install():
     run_and_check("npm install")
     
+def rsync(from_,  to_,  delete_after=False):
+    str_delete_after="--delete-after" if delete_after else ""
+    run_and_check(f"rsync -avzPH {from_} {to_} {str_delete_after}")
+    
+def poetry_install():
+    run_and_check("poetry install")
+    
+def poetry_env_info():
+    p=run("poetry env info -e", shell=True, capture_output=True)
+    return p.stdout.decode('utf-8')
```

### Comparing `preprod-0.1.0/preprod/core.py` & `preprod-0.2.0/preprod/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,55 @@
 #!/usr/bin/python3
 from argparse import ArgumentParser
 from datetime import datetime
 from gettext import translation
 from importlib.resources import files
+from multiprocessing import Lock
 from os import path, makedirs
 from preprod import commons
 from sys import exit
 
 
 try:
     t=translation('preprod', files("preprod") / 'locale')
     _=t.gettext
 except:
     _=str
 
 
+def concurrent_log(title, stdout=None,  stderr=None):
+    def parse_std(std):
+        arr=std.split("\n")
+        r=""
+        for line in arr:
+            r+=f"      {line}\n"
+        return r
+    filename=f"/tmp/preprod_logs/{args.project}.log"
+    makedirs(path.dirname(filename), exist_ok=True)
+    with lock:
+        with open(filename, "a") as f:
+            f.write(commons.yellow(f"{datetime.now()} [{args.project}/{args.action}] {title}\n"))
+            if stdout!="" and stdout is not None:
+                f.write(commons.green("      STDOUT\n"))
+                f.write(parse_std(stdout))
+            if stderr!="" and stderr is not None:
+                f.write(commons.red("      STDERR\n"))
+                f.write(parse_std(stderr))
+            
 def main():
+    global lock
+    lock=Lock()
 
-    parser=ArgumentParser(description=_("ProPre manager"))
+    parser=ArgumentParser(description=_("ProPred manager"))
     parser.add_argument('--pretend', default=False, help=_("Prints action code without running it"),  action='store_true')
 
     parser.add_argument('project',nargs='?', default=None, help=_("Project identification"),  action='store')
-    parser.add_argument('action',nargs='?', default=None, help=_("Project identification"),  action='store')
-
+    parser.add_argument('action',nargs='?', default=None, help=_("Action identification"),  action='store')
 
+    global args
     args=parser.parse_args()
     
     commons.check_repository_path(verbose=True)
     repository_path=commons.repository_path()
     project_path=f"{repository_path}/{args.project}/"
     action_path=f"{project_path}/{args.action}"
```

### Comparing `preprod-0.1.0/preprod/locale/en.po` & `preprod-0.2.0/preprod/locale/en.po`

 * *Files identical despite different names*

### Comparing `preprod-0.1.0/preprod/locale/es.po` & `preprod-0.2.0/preprod/locale/es.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # root <turulomio@yahoo.es>, 2015, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: TooManyFiles\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-21 20:58+0200\n"
+"POT-Creation-Date: 2024-05-26 20:05+0200\n"
 "PO-Revision-Date: 2020-04-03 08:54+0200\n"
 "Last-Translator: trabajo <turulomio@yahoo.es>\n"
 "Language-Team: Spanish <kde-i18n-doc@kde.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -30,17 +30,14 @@
 msgid "Replacing values in {0}"
 msgstr "Remplazando valores en {0}"
 
 #, python-brace-format
 msgid "Appending text at the end of {0}"
 msgstr "Añadiendo texto al final de {0}"
 
-msgid "Exiting propred..."
-msgstr "Saliendo de propred..."
-
 #, python-brace-format
 msgid "Deleting directory {0}"
 msgstr "Borarando directorio {0}"
 
 #, python-brace-format
 msgid "Changing to directory {0}"
 msgstr "Cambiando a directorio {0}"
@@ -55,46 +52,54 @@
 #, python-brace-format
 msgid "Deleting line {0} in {1}"
 msgstr ""
 
 msgid "You must create repository path"
 msgstr "Debe crear el directory del repositorio"
 
-msgid "ProPre manager"
+msgid "ProPred manager"
 msgstr ""
 
 msgid "Prints action code without running it"
 msgstr "Muestra el código de la acción sin ejecutarlo"
 
 msgid "Project identification"
-msgstr ""
+msgstr "Identificación del proyecto"
+
+msgid "Action identification"
+msgstr "Identificación de la acción"
 
 #, python-brace-format
 msgid "Reading repository from {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Project wasn't found in {0}"
-msgstr ""
+msgstr "El proyecto no fue encontrado en {0}"
 
 #, python-brace-format
 msgid "Action wasn't found in {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Executing project '{0}' and action '{1}'"
 msgstr ""
 
 #, python-brace-format
 msgid "Executed project '{0}' and action '{1}' took {2}"
 msgstr ""
 
-msgid "Repository already created in {}"
+msgid "ProPre manager"
 msgstr ""
 
+msgid "Repository already created in {}"
+msgstr "El repositorio ya está creado en {}"
+
 msgid "Shows repository_commons.py file in repository pathh"
 msgstr ""
 
 #, python-brace-format
 msgid "Reading repository from {0} and listing available preprod scripts"
 msgstr ""
 
+#~ msgid "Exiting propred..."
+#~ msgstr "Saliendo de propred..."
```

### Comparing `preprod-0.1.0/preprod/locale/preprod.pot` & `preprod-0.2.0/preprod/locale/preprod.pot`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-21 21:00+0200\n"
+"POT-Creation-Date: 2024-05-26 20:06+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=CHARSET\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -28,17 +28,14 @@
 msgid "Replacing values in {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Appending text at the end of {0}"
 msgstr ""
 
-msgid "Exiting propred..."
-msgstr ""
-
 #, python-brace-format
 msgid "Deleting directory {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Changing to directory {0}"
 msgstr ""
@@ -53,23 +50,26 @@
 #, python-brace-format
 msgid "Deleting line {0} in {1}"
 msgstr ""
 
 msgid "You must create repository path"
 msgstr ""
 
-msgid "ProPre manager"
+msgid "ProPred manager"
 msgstr ""
 
 msgid "Prints action code without running it"
 msgstr ""
 
 msgid "Project identification"
 msgstr ""
 
+msgid "Action identification"
+msgstr ""
+
 #, python-brace-format
 msgid "Reading repository from {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Project wasn't found in {0}"
 msgstr ""
@@ -82,14 +82,17 @@
 msgid "Executing project '{0}' and action '{1}'"
 msgstr ""
 
 #, python-brace-format
 msgid "Executed project '{0}' and action '{1}' took {2}"
 msgstr ""
 
+msgid "ProPre manager"
+msgstr ""
+
 msgid "Repository already created in {}"
 msgstr ""
 
 msgid "Shows repository_commons.py file in repository pathh"
 msgstr ""
 
 #, python-brace-format
```

### Comparing `preprod-0.1.0/preprod/poethepoet.py` & `preprod-0.2.0/preprod/poethepoet.py`

 * *Files identical despite different names*

### Comparing `preprod-0.1.0/pyproject.toml` & `preprod-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preprod"
-version = "0.1.0"
+version = "0.2.0"
 description = "Easily creation of pre-production and production scripts to automete your deployment"
 authors = ["turulomio <turulomio@yahoo.es>"]
 license = "GPL-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

