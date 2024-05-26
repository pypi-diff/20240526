# Comparing `tmp/chemfunc-1.0.5.tar.gz` & `tmp/chemfunc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemfunc-1.0.5.tar", last modified: Fri Dec 29 16:37:16 2023, max compression
+gzip compressed data, was "chemfunc-1.0.6.tar", last modified: Sun May 26 03:31:36 2024, max compression
```

## Comparing `chemfunc-1.0.5.tar` & `chemfunc-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-12-29 16:37:16.198438 chemfunc-1.0.5/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.5/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6747 2023-12-29 16:37:16.198712 chemfunc-1.0.5/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5954 2023-07-14 01:56:12.000000 chemfunc-1.0.5/README.md
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-12-29 16:37:16.193700 chemfunc-1.0.5/chemfunc/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2037 2023-07-13 23:01:21.000000 chemfunc-1.0.5/chemfunc/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-12-29 16:29:19.000000 chemfunc-1.0.5/chemfunc/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/canonicalize_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/chemical_diversity.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/cluster_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/compute_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.5/chemfunc/constants.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/deduplicate_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.5/chemfunc/filter_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1222 2023-07-13 23:01:21.000000 chemfunc-1.0.5/chemfunc/main.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.5/chemfunc/measure_experimental_reproducibility.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5736 2023-07-13 23:19:10.000000 chemfunc-1.0.5/chemfunc/molecular_fingerprints.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.5/chemfunc/molecular_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/molecular_similarities.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3274 2023-06-02 15:22:59.000000 chemfunc-1.0.5/chemfunc/nearest_neighbor.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.5/chemfunc/plot_property_distribution.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6393 2023-12-29 16:34:03.000000 chemfunc-1.0.5/chemfunc/plot_tsne.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.5/chemfunc/regression_to_classification.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.5/chemfunc/sample_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/sdf_to_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.5/chemfunc/select_from_clusters.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.5/chemfunc/smiles_to_svg.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.5/chemfunc/utils.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-06-24 07:43:27.000000 chemfunc-1.0.5/chemfunc/visualize_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.5/chemfunc/visualize_reactions.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-12-29 16:37:16.197951 chemfunc-1.0.5/chemfunc.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6747 2023-12-29 16:37:16.000000 chemfunc-1.0.5/chemfunc.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-12-29 16:37:16.000000 chemfunc-1.0.5/chemfunc.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-12-29 16:37:16.000000 chemfunc-1.0.5/chemfunc.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-12-29 16:37:16.000000 chemfunc-1.0.5/chemfunc.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-12-29 16:37:16.000000 chemfunc-1.0.5/chemfunc.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-12-29 16:37:16.000000 chemfunc-1.0.5/chemfunc.egg-info/top_level.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-12-29 16:37:16.199523 chemfunc-1.0.5/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1662 2023-11-13 20:29:19.000000 chemfunc-1.0.5/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 03:31:36.820650 chemfunc-1.0.6/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.6/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     7174 2024-05-26 03:31:36.820926 chemfunc-1.0.6/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6381 2024-05-26 03:30:25.000000 chemfunc-1.0.6/README.md
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 03:31:36.816657 chemfunc-1.0.6/chemfunc/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2037 2023-07-13 23:01:21.000000 chemfunc-1.0.6/chemfunc/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2024-05-26 03:17:45.000000 chemfunc-1.0.6/chemfunc/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/canonicalize_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/chemical_diversity.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/cluster_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/compute_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.6/chemfunc/constants.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/deduplicate_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/filter_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1222 2023-07-13 23:01:21.000000 chemfunc-1.0.6/chemfunc/main.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.6/chemfunc/measure_experimental_reproducibility.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5727 2024-05-24 19:57:04.000000 chemfunc-1.0.6/chemfunc/molecular_fingerprints.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.6/chemfunc/molecular_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/molecular_similarities.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3274 2023-06-02 15:22:59.000000 chemfunc-1.0.6/chemfunc/nearest_neighbor.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.6/chemfunc/plot_property_distribution.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6393 2023-12-29 16:34:03.000000 chemfunc-1.0.6/chemfunc/plot_tsne.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/regression_to_classification.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/sample_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3279 2024-05-26 03:26:04.000000 chemfunc-1.0.6/chemfunc/sdf_to_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/select_from_clusters.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.6/chemfunc/smiles_to_svg.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/utils.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-06-24 07:43:27.000000 chemfunc-1.0.6/chemfunc/visualize_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.6/chemfunc/visualize_reactions.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 03:31:36.820177 chemfunc-1.0.6/chemfunc.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     7174 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/top_level.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2024-05-26 03:31:36.821806 chemfunc-1.0.6/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1662 2023-11-13 20:29:19.000000 chemfunc-1.0.6/setup.py
```

### Comparing `chemfunc-1.0.5/LICENSE` & `chemfunc-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/PKG-INFO` & `chemfunc-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.5.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.6.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,19 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chem Func
 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chemfunc)](https://badge.fury.io/py/chemfunc)
+[![PyPI version](https://badge.fury.io/py/chemfunc.svg)](https://badge.fury.io/py/chemfunc)
+[![Downloads](https://pepy.tech/badge/chemfunc)](https://pepy.tech/project/chemfunc)
+[![license](https://img.shields.io/github/license/swansonk14/chemfunc.svg)](https://github.com/swansonk14/chemfunc/blob/main/LICENSE.txt)
+
 Useful functions and scripts for working with small molecules.
 
 ## Installation
 
 Optionally, create a conda environment.
 ```bash
 conda create -y -n chemfunc python=3.10
```

### Comparing `chemfunc-1.0.5/README.md` & `chemfunc-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Chem Func
 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chemfunc)](https://badge.fury.io/py/chemfunc)
+[![PyPI version](https://badge.fury.io/py/chemfunc.svg)](https://badge.fury.io/py/chemfunc)
+[![Downloads](https://pepy.tech/badge/chemfunc)](https://pepy.tech/project/chemfunc)
+[![license](https://img.shields.io/github/license/swansonk14/chemfunc.svg)](https://github.com/swansonk14/chemfunc/blob/main/LICENSE.txt)
+
 Useful functions and scripts for working with small molecules.
 
 ## Installation
 
 Optionally, create a conda environment.
 ```bash
 conda create -y -n chemfunc python=3.10
```

### Comparing `chemfunc-1.0.5/chemfunc/__init__.py` & `chemfunc-1.0.6/chemfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/canonicalize_smiles.py` & `chemfunc-1.0.6/chemfunc/canonicalize_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/chemical_diversity.py` & `chemfunc-1.0.6/chemfunc/chemical_diversity.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/cluster_molecules.py` & `chemfunc-1.0.6/chemfunc/cluster_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/compute_properties.py` & `chemfunc-1.0.6/chemfunc/compute_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/deduplicate_smiles.py` & `chemfunc-1.0.6/chemfunc/deduplicate_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/filter_molecules.py` & `chemfunc-1.0.6/chemfunc/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/main.py` & `chemfunc-1.0.6/chemfunc/main.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/measure_experimental_reproducibility.py` & `chemfunc-1.0.6/chemfunc/measure_experimental_reproducibility.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/molecular_fingerprints.py` & `chemfunc-1.0.6/chemfunc/molecular_fingerprints.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,21 +67,21 @@
         num_bits: int = MORGAN_NUM_BITS
 ) -> np.ndarray:
     """Generates a binary Morgan fingerprint for a molecule.
 
     :param mol: A molecule (i.e., either a SMILES string or an RDKit molecule).
     :param radius: Morgan fingerprint radius.
     :param num_bits: Number of bits in Morgan fingerprint.
-    :return: A 1D boolean numpy array (num_bits,) containing the binary Morgan fingerprint.
+    :return: A 1D numpy array (num_bits,) containing the Morgan fingerprint.
     """
     mol = Chem.MolFromSmiles(mol) if type(mol) == str else mol
     morgan_vec = AllChem.GetMorganFingerprintAsBitVect(mol, radius, nBits=num_bits)
     morgan_fp = np.zeros((1,))
     ConvertToNumpyArray(morgan_vec, morgan_fp)
-    morgan_fp = morgan_fp.astype(bool)
+    morgan_fp = morgan_fp.astype(np.float32)
 
     return morgan_fp
 
 
 @register_fingerprint_generator('rdkit')
 def compute_rdkit_fingerprint(mol: Molecule) -> np.ndarray:
     """Generates RDKit 2D normalized features for a molecule.
```

### Comparing `chemfunc-1.0.5/chemfunc/molecular_properties.py` & `chemfunc-1.0.6/chemfunc/molecular_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/molecular_similarities.py` & `chemfunc-1.0.6/chemfunc/molecular_similarities.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/nearest_neighbor.py` & `chemfunc-1.0.6/chemfunc/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/plot_property_distribution.py` & `chemfunc-1.0.6/chemfunc/plot_property_distribution.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/plot_tsne.py` & `chemfunc-1.0.6/chemfunc/plot_tsne.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/regression_to_classification.py` & `chemfunc-1.0.6/chemfunc/regression_to_classification.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/sample_molecules.py` & `chemfunc-1.0.6/chemfunc/sample_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/sdf_to_smiles.py` & `chemfunc-1.0.6/chemfunc/sdf_to_smiles.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,30 +4,62 @@
 import pandas as pd
 from rdkit import Chem
 from tqdm import tqdm
 
 from chemfunc.constants import SMILES_COLUMN
 
 
+def mol_to_smiles_with_properties(
+        mol: Chem.Mol,
+        smiles_column: str = SMILES_COLUMN,
+        all_properties: bool = False,
+        properties: list[str] | None = None,
+) -> dict:
+    """Converts an RDKit molecule to a dictionary containing SMILES and optionally properties.
+
+    :param mol: RDKit molecule.
+    :param smiles_column: The name of the column where SMILES will be saved.
+    :param all_properties: Whether to extract all properties from the SDF.
+    :param properties: List of properties to extract from the SDF for each molecule.
+    :return: Dictionary containing SMILES and optionally properties.
+    """
+    # Get properties
+    if all_properties:
+        props = mol.GetPropsAsDict()
+    elif properties is not None:
+        props = {prop: mol.GetProp(prop) for prop in properties}
+    else:
+        props = {}
+
+    return {
+        smiles_column: Chem.MolToSmiles(mol),
+        **props
+    }
+
+
 def sdf_to_smiles(
         data_path: Path,
         save_path: Path,
+        smiles_column: str = SMILES_COLUMN,
+        all_properties: bool = False,
         properties: list[str] | None = None,
         deduplicate: bool = False
 ) -> None:
     """Converts molecules in SDF format to a CSV with SMILES.
 
     :param data_path: Path to an SDF file.
+    :param smiles_column: The name of the column where SMILES will be saved.
+    :param all_properties: Whether to extract all properties from the SDF.
     :param properties: List of properties to extract from the SDF for each molecule.
     :param save_path: Path to a CSV file where SMILES strings will be saved.
     :param deduplicate: Whether to deduplicate SMILES.
     """
-    # Default to empty set for properties
-    if properties is None:
-        properties = []
+    # Validate arguments
+    if all_properties and properties is not None:
+        raise ValueError('Cannot specify both all_properties and properties')
 
     # Load SDF file
     num_skipped = 0
     mols = []
 
     with Chem.SDMolSupplier(str(data_path)) as suppl:
         for mol in tqdm(suppl, desc='Loading SDF'):
@@ -35,33 +67,32 @@
                 num_skipped += 1
             else:
                 mols.append(mol)
 
     print(f'Number of molecules = {len(mols):,}')
     print(f'Number skipped = {num_skipped:,}')
 
-    # Put data in Pandas DataFrame
-    data = pd.DataFrame(data=[
-        {
-            SMILES_COLUMN: Chem.MolToSmiles(mol),
-            **{
-                prop: mol.GetProp(prop)
-                for prop in properties
-            }
-        } for mol in tqdm(mols, desc='Mol to SMILES')
+    # Covert mols to SMILES and optionally extract properties
+    data = pd.DataFrame([
+        mol_to_smiles_with_properties(
+            mol=mol,
+            smiles_column=smiles_column,
+            all_properties=all_properties,
+            properties=properties
+        ) for mol in tqdm(mols, desc='Mol to SMILES')
     ])
 
     # Optionally deduplicate
     if deduplicate:
         print('Deduplicating SMILES')
-        data.drop_duplicates(subset=SMILES_COLUMN, inplace=True)
+        data.drop_duplicates(subset=smiles_column, inplace=True)
 
     # Print stats
     print(f'Data size = {len(data):,}')
-    print(f'Number of unique smiles = {data[SMILES_COLUMN].nunique():,}')
+    print(f'Number of unique smiles = {data[smiles_column].nunique():,}')
 
-    for prop in properties:
-        print(f'Number of unique {prop} = {data[prop].nunique():,}')
+    for prop in sorted(set(data.columns) - {smiles_column}):
+        print(f'Number of {prop} (# unique) = {data[prop].notna().sum():,} ({data[prop].nunique():,})')
 
     # Save data as CSV
     save_path.parent.mkdir(parents=True, exist_ok=True)
     data.to_csv(save_path, index=False)
```

### Comparing `chemfunc-1.0.5/chemfunc/select_from_clusters.py` & `chemfunc-1.0.6/chemfunc/select_from_clusters.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/smiles_to_svg.py` & `chemfunc-1.0.6/chemfunc/smiles_to_svg.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/utils.py` & `chemfunc-1.0.6/chemfunc/utils.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/visualize_molecules.py` & `chemfunc-1.0.6/chemfunc/visualize_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc/visualize_reactions.py` & `chemfunc-1.0.6/chemfunc/visualize_reactions.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/chemfunc.egg-info/PKG-INFO` & `chemfunc-1.0.6/chemfunc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.5
+Version: 1.0.6
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.5.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.6.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,19 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Chem Func
 
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chemfunc)](https://badge.fury.io/py/chemfunc)
+[![PyPI version](https://badge.fury.io/py/chemfunc.svg)](https://badge.fury.io/py/chemfunc)
+[![Downloads](https://pepy.tech/badge/chemfunc)](https://pepy.tech/project/chemfunc)
+[![license](https://img.shields.io/github/license/swansonk14/chemfunc.svg)](https://github.com/swansonk14/chemfunc/blob/main/LICENSE.txt)
+
 Useful functions and scripts for working with small molecules.
 
 ## Installation
 
 Optionally, create a conda environment.
 ```bash
 conda create -y -n chemfunc python=3.10
```

### Comparing `chemfunc-1.0.5/chemfunc.egg-info/SOURCES.txt` & `chemfunc-1.0.6/chemfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.5/setup.py` & `chemfunc-1.0.6/setup.py`

 * *Files identical despite different names*

