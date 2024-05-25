# Comparing `tmp/cae_cli-0.2.9.6.tar.gz` & `tmp/cae_cli-0.2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.9.6.tar", last modified: Sat May 25 21:28:47 2024, max compression
+gzip compressed data, was "cae_cli-0.2.9.7.tar", last modified: Sat May 25 22:02:44 2024, max compression
```

## Comparing `cae_cli-0.2.9.6.tar` & `cae_cli-0.2.9.7.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 21:28:47.772754 cae_cli-0.2.9.6/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9.6/LICENSE
--rw-rw-rw-   0        0        0      419 2024-05-25 21:28:47.770751 cae_cli-0.2.9.6/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 21:28:47.721565 cae_cli-0.2.9.6/cae/
--rw-rw-rw-   0        0        0     9506 2024-05-09 22:42:15.000000 cae_cli-0.2.9.6/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      537 2024-05-25 05:03:15.000000 cae_cli-0.2.9.6/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9.6/cae/__init__.py
--rw-rw-rw-   0        0        0    10247 2024-05-09 22:46:38.000000 cae_cli-0.2.9.6/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-25 21:28:47.748497 cae_cli-0.2.9.6/cae/templates/
--rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9.6/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9.6/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9.6/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9.6/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9.6/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9.6/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9.6/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9.6/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9.6/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9.6/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.6/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9.6/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9.6/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9.6/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9.6/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9.6/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9.6/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9.6/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9.6/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 21:28:47.769750 cae_cli-0.2.9.6/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      419 2024-05-25 21:28:47.000000 cae_cli-0.2.9.6/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-25 21:28:47.000000 cae_cli-0.2.9.6/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 21:28:47.000000 cae_cli-0.2.9.6/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-25 21:28:47.000000 cae_cli-0.2.9.6/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-25 21:28:47.000000 cae_cli-0.2.9.6/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 21:28:47.772754 cae_cli-0.2.9.6/setup.cfg
--rw-rw-rw-   0        0        0      614 2024-05-25 21:28:45.000000 cae_cli-0.2.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.201925 cae_cli-0.2.9.7/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9.7/LICENSE
+-rw-rw-rw-   0        0        0      419 2024-05-25 22:02:44.200930 cae_cli-0.2.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.158844 cae_cli-0.2.9.7/cae/
+-rw-rw-rw-   0        0        0     9578 2024-05-25 22:02:34.000000 cae_cli-0.2.9.7/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      537 2024-05-25 05:03:15.000000 cae_cli-0.2.9.7/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9.7/cae/__init__.py
+-rw-rw-rw-   0        0        0    10237 2024-05-25 21:59:54.000000 cae_cli-0.2.9.7/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.182879 cae_cli-0.2.9.7/cae/templates/
+-rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9.7/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9.7/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9.7/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9.7/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9.7/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9.7/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9.7/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9.7/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9.7/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9.7/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.7/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.7/cae/templates/pom.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9.7/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9.7/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9.7/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9.7/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9.7/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9.7/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9.7/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9.7/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.199924 cae_cli-0.2.9.7/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      419 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      891 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 22:02:44.202925 cae_cli-0.2.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-05-25 22:02:34.000000 cae_cli-0.2.9.7/setup.py
```

### Comparing `cae_cli-0.2.9.6/LICENSE` & `cae_cli-0.2.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/README.md` & `cae_cli-0.2.9.7/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.9.7/cae/ArchFlowJavaWeb.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
         print("⚡️ Cae Version 0.0.3 ⚡️")
         print("⚡️ ArchFlow Version 0.1.4 ⚡️")
         print("ArchFlow is evolving... slowly. But hey, we still love him! ⚡️")
 
     def read_content_pom(self):
         poms = self.DirectoryExplorer.list_files(self.POM_FILE)
         core_pom_path = self.filter.find_one_obj_by_key(poms, "core")
+        if core_pom_path is None:
+            core_pom_path = poms[0]
         content = self.DirectoryExplorer.read_file(core_pom_path)
         return self.extract_content_pom(content)
 
     def get_artifact_id(self, input_string):
         _, artifact = self.read_content_pom()
         return artifact
```

### Comparing `cae_cli-0.2.9.6/cae/Run.py` & `cae_cli-0.2.9.7/cae/Run.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/db.json` & `cae_cli-0.2.9.7/cae/db.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995039682539683%*

 * *Differences: {"'functions'": "{'new_project': {'steps': {0: {'new_layer': {insert: [(3, '')], delete: [3]}}}}, "*

 * *                "'new_project_ignore_ssl': {'steps': {0: {'new_layer_ignore_ssl': {insert: [(3, "*

 * *                "'')], delete: [3]}}}}}"}*

```diff
@@ -526,15 +526,15 @@
         "new_project": {
             "steps": [
                 {
                     "new_layer": [
                         "args[1]",
                         "args[2]",
                         "core",
-                        "-core",
+                        "",
                         "<pk>args[1].args[2].core</pk>.use_cases"
                     ]
                 },
                 {
                     "new_layer": [
                         "args[1]",
                         "args[2]",
@@ -557,15 +557,15 @@
         "new_project_ignore_ssl": {
             "steps": [
                 {
                     "new_layer_ignore_ssl": [
                         "args[1]",
                         "args[2]",
                         "core",
-                        "-core",
+                        "",
                         "<pk>args[1].args[2].core</pk>.use_cases"
                     ]
                 },
                 {
                     "new_layer_ignore_ssl": [
                         "args[1]",
                         "args[2]",
```

### Comparing `cae_cli-0.2.9.6/cae/templates/assembler.txt` & `cae_cli-0.2.9.7/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/entityFactory.txt` & `cae_cli-0.2.9.7/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.9.7/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/implementation_ruc.txt` & `cae_cli-0.2.9.7/cae/templates/implementation_ruc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/implementation_suc.txt` & `cae_cli-0.2.9.7/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/pom-adapters.txt` & `cae_cli-0.2.9.7/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.9.7/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/pom-core.txt` & `cae_cli-0.2.9.7/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/use_case.txt` & `cae_cli-0.2.9.7/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/use_case_factory.txt` & `cae_cli-0.2.9.7/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.9.7/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.6/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.9.7/cae_cli.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 cae/templates/entityImplementation.txt
 cae/templates/implementation_cuc.txt
 cae/templates/implementation_ruc.txt
 cae/templates/implementation_suc.txt
 cae/templates/pom-adapters.txt
 cae/templates/pom-assemblers.txt
 cae/templates/pom-core.txt
+cae/templates/pom.txt
 cae/templates/use_case.txt
 cae/templates/use_case_cuc.txt
 cae/templates/use_case_factory.txt
 cae/templates/use_case_implementation.txt
 cae/templates/use_case_input.txt
 cae/templates/use_case_output.txt
 cae/templates/use_case_ruc.txt
```

### Comparing `cae_cli-0.2.9.6/setup.py` & `cae_cli-0.2.9.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.9.6',
+    version='0.2.9.7',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

