# Comparing `tmp/cae_cli-0.2.9.7.tar.gz` & `tmp/cae_cli-0.2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.9.7.tar", last modified: Sat May 25 22:02:44 2024, max compression
+gzip compressed data, was "cae_cli-0.2.9.8.tar", last modified: Sat May 25 22:43:13 2024, max compression
```

## Comparing `cae_cli-0.2.9.7.tar` & `cae_cli-0.2.9.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.201925 cae_cli-0.2.9.7/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9.7/LICENSE
--rw-rw-rw-   0        0        0      419 2024-05-25 22:02:44.200930 cae_cli-0.2.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.158844 cae_cli-0.2.9.7/cae/
--rw-rw-rw-   0        0        0     9578 2024-05-25 22:02:34.000000 cae_cli-0.2.9.7/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      537 2024-05-25 05:03:15.000000 cae_cli-0.2.9.7/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9.7/cae/__init__.py
--rw-rw-rw-   0        0        0    10237 2024-05-25 21:59:54.000000 cae_cli-0.2.9.7/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.182879 cae_cli-0.2.9.7/cae/templates/
--rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9.7/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9.7/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9.7/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9.7/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9.7/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9.7/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9.7/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9.7/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9.7/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9.7/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.7/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.7/cae/templates/pom.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9.7/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9.7/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9.7/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9.7/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9.7/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9.7/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9.7/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9.7/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-25 22:02:44.199924 cae_cli-0.2.9.7/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      419 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      891 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-25 22:02:44.000000 cae_cli-0.2.9.7/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 22:02:44.202925 cae_cli-0.2.9.7/setup.cfg
--rw-rw-rw-   0        0        0      614 2024-05-25 22:02:34.000000 cae_cli-0.2.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:43:13.490808 cae_cli-0.2.9.8/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9.8/LICENSE
+-rw-rw-rw-   0        0        0      419 2024-05-25 22:43:13.489807 cae_cli-0.2.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 22:43:13.446290 cae_cli-0.2.9.8/cae/
+-rw-rw-rw-   0        0        0     9578 2024-05-25 22:02:34.000000 cae_cli-0.2.9.8/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      537 2024-05-25 05:03:15.000000 cae_cli-0.2.9.8/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9.8/cae/__init__.py
+-rw-rw-rw-   0        0        0    10237 2024-05-25 21:59:54.000000 cae_cli-0.2.9.8/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-25 22:43:13.469781 cae_cli-0.2.9.8/cae/templates/
+-rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9.8/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9.8/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9.8/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9.8/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9.8/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9.8/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9.8/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9.8/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9.8/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9.8/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.8/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9.8/cae/templates/pom.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9.8/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9.8/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9.8/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9.8/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9.8/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9.8/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9.8/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9.8/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 22:43:13.489807 cae_cli-0.2.9.8/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      419 2024-05-25 22:43:13.000000 cae_cli-0.2.9.8/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      891 2024-05-25 22:43:13.000000 cae_cli-0.2.9.8/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 22:43:13.000000 cae_cli-0.2.9.8/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-25 22:43:13.000000 cae_cli-0.2.9.8/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-25 22:43:13.000000 cae_cli-0.2.9.8/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 22:43:13.491812 cae_cli-0.2.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-05-25 22:43:06.000000 cae_cli-0.2.9.8/setup.py
```

### Comparing `cae_cli-0.2.9.7/LICENSE` & `cae_cli-0.2.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/README.md` & `cae_cli-0.2.9.8/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.9.8/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/Run.py` & `cae_cli-0.2.9.8/cae/Run.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/db.json` & `cae_cli-0.2.9.8/cae/db.json`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/assembler.txt` & `cae_cli-0.2.9.8/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/entityFactory.txt` & `cae_cli-0.2.9.8/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.9.8/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/implementation_ruc.txt` & `cae_cli-0.2.9.8/cae/templates/implementation_ruc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/implementation_suc.txt` & `cae_cli-0.2.9.8/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/pom-adapters.txt` & `cae_cli-0.2.9.8/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.9.8/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/pom-core.txt` & `cae_cli-0.2.9.8/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/pom.txt` & `cae_cli-0.2.9.8/cae/templates/pom.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/use_case.txt` & `cae_cli-0.2.9.8/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/use_case_factory.txt` & `cae_cli-0.2.9.8/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.9.8/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.9.8/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.9.7/setup.py` & `cae_cli-0.2.9.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.9.7',
+    version='0.2.9.8',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
     packages=['cae'],
     package_data={
           'cae': ['templates/*.txt', '*.json']
     },
     install_requires=[
-        'arch-flow>=0.1.8.5',
+        'arch-flow>=0.1.8.6',
         'colorama'
       ],
 )
```

