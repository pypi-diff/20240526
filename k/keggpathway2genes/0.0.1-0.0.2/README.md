# Comparing `tmp/keggpathway2genes-0.0.1.tar.gz` & `tmp/keggpathway2genes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keggpathway2genes-0.0.1.tar", last modified: Sun May 26 18:36:20 2024, max compression
+gzip compressed data, was "keggpathway2genes-0.0.2.tar", last modified: Sun May 26 18:48:05 2024, max compression
```

## Comparing `keggpathway2genes-0.0.1.tar` & `keggpathway2genes-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:36:20.436270 keggpathway2genes-0.0.1/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      636 2024-05-26 18:36:20.436270 keggpathway2genes-0.0.1/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      407 2024-05-26 18:31:08.000000 keggpathway2genes-0.0.1/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:36:20.436270 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      636 2024-05-26 18:36:20.000000 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      308 2024-05-26 18:36:20.000000 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 18:36:20.000000 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       61 2024-05-26 18:36:20.000000 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       27 2024-05-26 18:36:20.000000 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-26 18:36:20.000000 keggpathway2genes-0.0.1/keggpathway2genes.egg-info/top_level.txt
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:36:20.436270 keggpathway2genes-0.0.1/kp2genes/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 keggpathway2genes-0.0.1/kp2genes/__init__.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1721 2024-05-26 16:45:24.000000 keggpathway2genes-0.0.1/kp2genes/kp2genes.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-26 18:36:20.436270 keggpathway2genes-0.0.1/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      605 2024-05-26 18:35:51.000000 keggpathway2genes-0.0.1/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:48:05.483731 keggpathway2genes-0.0.2/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      636 2024-05-26 18:48:05.483731 keggpathway2genes-0.0.2/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      407 2024-05-26 18:47:21.000000 keggpathway2genes-0.0.2/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:48:05.479731 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      636 2024-05-26 18:48:05.000000 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      308 2024-05-26 18:48:05.000000 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-05-26 18:48:05.000000 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       65 2024-05-26 18:48:05.000000 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       27 2024-05-26 18:48:05.000000 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        9 2024-05-26 18:48:05.000000 keggpathway2genes-0.0.2/keggpathway2genes.egg-info/top_level.txt
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-05-26 18:48:05.483731 keggpathway2genes-0.0.2/kp2genes/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-17 19:50:34.000000 keggpathway2genes-0.0.2/kp2genes/__init__.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1774 2024-05-26 18:46:39.000000 keggpathway2genes-0.0.2/kp2genes/kp2genes.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-05-26 18:48:05.483731 keggpathway2genes-0.0.2/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      609 2024-05-26 18:47:14.000000 keggpathway2genes-0.0.2/setup.py
```

### Comparing `keggpathway2genes-0.0.1/PKG-INFO` & `keggpathway2genes-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keggpathway2genes
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to convert KEGG Pathway IDs to genes
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Description-Content-Type: text/markdown
 
 
 ## Installation
@@ -19,10 +19,10 @@
 
 ## Examples
 Extract gene entries for the KEGG pathway Apoptosis (hsa04210):
 `$ keggpathway2genes -kp hsa04210`
 
 A tab-separated file will be written out
 
-<i>current version='0.0.1'</i>
+<i>current version='0.0.2'</i>
```

### Comparing `keggpathway2genes-0.0.1/keggpathway2genes.egg-info/PKG-INFO` & `keggpathway2genes-0.0.2/keggpathway2genes.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keggpathway2genes
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to convert KEGG Pathway IDs to genes
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Description-Content-Type: text/markdown
 
 
 ## Installation
@@ -19,10 +19,10 @@
 
 ## Examples
 Extract gene entries for the KEGG pathway Apoptosis (hsa04210):
 `$ keggpathway2genes -kp hsa04210`
 
 A tab-separated file will be written out
 
-<i>current version='0.0.1'</i>
+<i>current version='0.0.2'</i>
```

### Comparing `keggpathway2genes-0.0.1/kp2genes/kp2genes.py` & `keggpathway2genes-0.0.2/kp2genes/kp2genes.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,13 +35,16 @@
     with open(f"{pathway_id}.txt", "w") as file:
         file.write("Entrez_ID\tGene\n")
         for gene_id, gene_name in gene_info:
             file.write(f"{gene_id}\t{gene_name}\n")
     
     print(f"Found {total_genes} genes for pathway {pathway_id}.")
 
-if __name__ == "__main__":
+def parse_arguments():
     parser = argparse.ArgumentParser(description="Fetch gene IDs and names for a given KEGG pathway")
     parser.add_argument("-kp", "--kegg_pathway", required=True, help="KEGG pathway ID")
-    args = parser.parse_args()
+    return parser.parse_args()
+
+if __name__ == "__main__":
+    args = parse_arguments()
     main(args.kegg_pathway)
```

### Comparing `keggpathway2genes-0.0.1/setup.py` & `keggpathway2genes-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='keggpathway2genes',
-    version='0.0.1',
+    version='0.0.2',
     author='Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email=' ',
     description='A package to convert KEGG Pathway IDs to genes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'keggpathway2genes=kp2genes.kp2genes:main',
+            'keggpathway2genes=kp2genes.kp2genes:main_cli',
         ],
     },
     install_requires=[
         'argparse',
         'requests',
         'bs4',
         'tqdm'
```

