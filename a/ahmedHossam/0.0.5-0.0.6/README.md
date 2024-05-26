# Comparing `tmp/ahmedhossam-0.0.5.tar.gz` & `tmp/ahmedHossam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahmedhossam-0.0.5.tar", last modified: Thu May 23 07:35:29 2024, max compression
+gzip compressed data, was "ahmedHossam-0.0.6.tar", last modified: Sun May 26 06:27:44 2024, max compression
```

## Comparing `ahmedhossam-0.0.5.tar` & `ahmedHossam-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:35:29.536662 ahmedhossam-0.0.5/
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:35:29.386705 ahmedhossam-0.0.5/AhmedHossam/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       23 2024-05-23 07:02:12.000000 ahmedhossam-0.0.5/AhmedHossam/__init__.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       49 2024-05-23 07:34:10.000000 ahmedhossam-0.0.5/AhmedHossam/main.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       78 2024-05-22 09:52:26.000000 ahmedhossam-0.0.5/CHANGELOG.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)     1051 2024-05-22 09:52:26.000000 ahmedhossam-0.0.5/LICENCE.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       26 2024-05-22 09:52:26.000000 ahmedhossam-0.0.5/MANIFEST.in
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 07:35:29.521542 ahmedhossam-0.0.5/PKG-INFO
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       20 2024-05-22 09:52:52.000000 ahmedhossam-0.0.5/README.txt
-drwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        0 2024-05-23 07:35:29.501042 ahmedhossam-0.0.5/ahmedHossam.egg-info/
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      544 2024-05-23 07:35:29.000000 ahmedhossam-0.0.5/ahmedHossam.egg-info/PKG-INFO
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      249 2024-05-23 07:35:29.000000 ahmedhossam-0.0.5/ahmedHossam.egg-info/SOURCES.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)        1 2024-05-23 07:35:29.000000 ahmedhossam-0.0.5/ahmedHossam.egg-info/dependency_links.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       12 2024-05-23 07:35:29.000000 ahmedhossam-0.0.5/ahmedHossam.egg-info/top_level.txt
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       38 2024-05-23 07:35:29.538661 ahmedhossam-0.0.5/setup.cfg
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)      633 2024-05-23 07:34:42.000000 ahmedhossam-0.0.5/setup.py
--rwxrwxrwx   0 ahossam   (6511) ahossam   (6500)       53 2024-05-23 07:33:44.000000 ahmedhossam-0.0.5/test.py
+drwxrwxrwx   0        0        0        0 2024-05-26 06:27:44.233169 ahmedHossam-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-26 06:27:44.222648 ahmedHossam-0.0.6/AhmedHossam/
+-rw-rw-rw-   0        0        0       39 2024-05-26 06:25:24.000000 ahmedHossam-0.0.6/AhmedHossam/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-05-26 06:25:18.000000 ahmedHossam-0.0.6/AhmedHossam/main.py
+-rw-rw-rw-   0        0        0       78 2024-05-22 09:52:26.000000 ahmedHossam-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1051 2024-05-22 09:52:26.000000 ahmedHossam-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       26 2024-05-22 09:52:26.000000 ahmedHossam-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      563 2024-05-26 06:27:44.231173 ahmedHossam-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2024-05-22 09:52:52.000000 ahmedHossam-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 06:27:44.230170 ahmedHossam-0.0.6/ahmedHossam.egg-info/
+-rw-rw-rw-   0        0        0      563 2024-05-26 06:27:44.000000 ahmedHossam-0.0.6/ahmedHossam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-26 06:27:44.000000 ahmedHossam-0.0.6/ahmedHossam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 06:27:44.000000 ahmedHossam-0.0.6/ahmedHossam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-26 06:27:44.000000 ahmedHossam-0.0.6/ahmedHossam.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 06:27:44.233169 ahmedHossam-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      628 2024-05-26 06:25:54.000000 ahmedHossam-0.0.6/setup.py
+-rw-rw-rw-   0        0        0       51 2024-05-23 07:38:02.000000 ahmedHossam-0.0.6/test.py
```

### Comparing `ahmedhossam-0.0.5/LICENCE.txt` & `ahmedHossam-0.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ahmedhossam-0.0.5/setup.py` & `ahmedHossam-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='ahmedHossam',
-  version='0.0.5',
+  version='0.0.6',
   description='SABA7',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Ahmed Hossam',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
-  keywords='calculator', 
+  keywords='ahmed', 
   packages=find_packages(),
   install_requires=[''] 
 )
```

