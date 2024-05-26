# Comparing `tmp/chemfunc-1.0.6.tar.gz` & `tmp/chemfunc-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemfunc-1.0.6.tar", last modified: Sun May 26 03:31:36 2024, max compression
+gzip compressed data, was "chemfunc-1.0.7.tar", last modified: Sun May 26 21:27:10 2024, max compression
```

## Comparing `chemfunc-1.0.6.tar` & `chemfunc-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 03:31:36.820650 chemfunc-1.0.6/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.6/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     7174 2024-05-26 03:31:36.820926 chemfunc-1.0.6/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6381 2024-05-26 03:30:25.000000 chemfunc-1.0.6/README.md
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 03:31:36.816657 chemfunc-1.0.6/chemfunc/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2037 2023-07-13 23:01:21.000000 chemfunc-1.0.6/chemfunc/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2024-05-26 03:17:45.000000 chemfunc-1.0.6/chemfunc/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/canonicalize_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/chemical_diversity.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/cluster_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/compute_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.6/chemfunc/constants.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/deduplicate_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/filter_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1222 2023-07-13 23:01:21.000000 chemfunc-1.0.6/chemfunc/main.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.6/chemfunc/measure_experimental_reproducibility.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5727 2024-05-24 19:57:04.000000 chemfunc-1.0.6/chemfunc/molecular_fingerprints.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.6/chemfunc/molecular_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/molecular_similarities.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3274 2023-06-02 15:22:59.000000 chemfunc-1.0.6/chemfunc/nearest_neighbor.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.6/chemfunc/plot_property_distribution.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6393 2023-12-29 16:34:03.000000 chemfunc-1.0.6/chemfunc/plot_tsne.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/regression_to_classification.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/sample_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3279 2024-05-26 03:26:04.000000 chemfunc-1.0.6/chemfunc/sdf_to_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.6/chemfunc/select_from_clusters.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.6/chemfunc/smiles_to_svg.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.6/chemfunc/utils.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-06-24 07:43:27.000000 chemfunc-1.0.6/chemfunc/visualize_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.6/chemfunc/visualize_reactions.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 03:31:36.820177 chemfunc-1.0.6/chemfunc.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     7174 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2024-05-26 03:31:36.000000 chemfunc-1.0.6/chemfunc.egg-info/top_level.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2024-05-26 03:31:36.821806 chemfunc-1.0.6/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1662 2023-11-13 20:29:19.000000 chemfunc-1.0.6/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 21:27:10.885115 chemfunc-1.0.7/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.7/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     7174 2024-05-26 21:27:10.885277 chemfunc-1.0.7/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6381 2024-05-26 03:30:25.000000 chemfunc-1.0.7/README.md
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 21:27:10.882362 chemfunc-1.0.7/chemfunc/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2037 2023-07-13 23:01:21.000000 chemfunc-1.0.7/chemfunc/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2024-05-26 21:16:32.000000 chemfunc-1.0.7/chemfunc/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.7/chemfunc/canonicalize_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.7/chemfunc/chemical_diversity.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.7/chemfunc/cluster_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.7/chemfunc/compute_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.7/chemfunc/constants.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.7/chemfunc/deduplicate_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.7/chemfunc/filter_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1222 2023-07-13 23:01:21.000000 chemfunc-1.0.7/chemfunc/main.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.7/chemfunc/measure_experimental_reproducibility.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5727 2024-05-24 19:57:04.000000 chemfunc-1.0.7/chemfunc/molecular_fingerprints.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.7/chemfunc/molecular_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     9772 2024-05-26 20:42:37.000000 chemfunc-1.0.7/chemfunc/molecular_similarities.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4016 2024-05-26 20:42:37.000000 chemfunc-1.0.7/chemfunc/nearest_neighbor.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.7/chemfunc/plot_property_distribution.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6393 2023-12-29 16:34:03.000000 chemfunc-1.0.7/chemfunc/plot_tsne.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2948 2024-05-26 21:21:24.000000 chemfunc-1.0.7/chemfunc/regression_to_classification.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.7/chemfunc/sample_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3279 2024-05-26 03:26:04.000000 chemfunc-1.0.7/chemfunc/sdf_to_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.7/chemfunc/select_from_clusters.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.7/chemfunc/smiles_to_svg.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.7/chemfunc/utils.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-06-24 07:43:27.000000 chemfunc-1.0.7/chemfunc/visualize_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.7/chemfunc/visualize_reactions.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2024-05-26 21:27:10.884839 chemfunc-1.0.7/chemfunc.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     7174 2024-05-26 21:27:10.000000 chemfunc-1.0.7/chemfunc.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2024-05-26 21:27:10.000000 chemfunc-1.0.7/chemfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2024-05-26 21:27:10.000000 chemfunc-1.0.7/chemfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2024-05-26 21:27:10.000000 chemfunc-1.0.7/chemfunc.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      101 2024-05-26 21:27:10.000000 chemfunc-1.0.7/chemfunc.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2024-05-26 21:27:10.000000 chemfunc-1.0.7/chemfunc.egg-info/top_level.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2024-05-26 21:27:10.885786 chemfunc-1.0.7/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1670 2024-05-26 21:12:23.000000 chemfunc-1.0.7/setup.py
```

### Comparing `chemfunc-1.0.6/LICENSE` & `chemfunc-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/PKG-INFO` & `chemfunc-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.6
+Version: 1.0.7
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.6.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.7.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chemfunc-1.0.6/README.md` & `chemfunc-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/__init__.py` & `chemfunc-1.0.7/chemfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/canonicalize_smiles.py` & `chemfunc-1.0.7/chemfunc/canonicalize_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/chemical_diversity.py` & `chemfunc-1.0.7/chemfunc/chemical_diversity.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/cluster_molecules.py` & `chemfunc-1.0.7/chemfunc/cluster_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/compute_properties.py` & `chemfunc-1.0.7/chemfunc/compute_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/deduplicate_smiles.py` & `chemfunc-1.0.7/chemfunc/deduplicate_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/filter_molecules.py` & `chemfunc-1.0.7/chemfunc/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/main.py` & `chemfunc-1.0.7/chemfunc/main.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/measure_experimental_reproducibility.py` & `chemfunc-1.0.7/chemfunc/measure_experimental_reproducibility.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/molecular_fingerprints.py` & `chemfunc-1.0.7/chemfunc/molecular_fingerprints.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/molecular_properties.py` & `chemfunc-1.0.7/chemfunc/molecular_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/molecular_similarities.py` & `chemfunc-1.0.7/chemfunc/molecular_similarities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions to compute the similarities between molecules."""
+from functools import partial
 from itertools import product
 from multiprocessing import Pool
 from typing import Callable, Iterable
 
 import numpy as np
 from rdkit import Chem
 from rdkit.Chem.rdFMCS import FindMCS
@@ -18,14 +19,15 @@
 
 def register_similarity_function(similarity_type: str) -> Callable[[SimilarityFunction], SimilarityFunction]:
     """Creates a decorator which registers a similarity function in a global dictionary to enable access by name.
 
     :param similarity_type: The name to use to access the similarity function.
     :return: A decorator which will add a similarity function to the registry using the specified name.
     """
+
     def decorator(similarity_function: SimilarityFunction) -> SimilarityFunction:
         SIMILARITY_FUNCTION_REGISTRY[similarity_type] = similarity_function
         return similarity_function
 
     return decorator
 
 
@@ -72,35 +74,50 @@
     # Compute pairwise Tanimoto similarities
     tanimoto_distances = pairwise_distances(fps_1, fps_2, metric='jaccard', n_jobs=-1)
     tanimoto_similarities = 1 - tanimoto_distances
 
     return tanimoto_similarities
 
 
-def compute_mcs_size(mols: Iterable[Chem.Mol]) -> int:
+def compute_mcs_size(
+        mols: Iterable[Chem.Mol],
+        match_valences: bool = False,
+        ring_matches_ring_only: bool = False,
+        complete_rings_only: bool = False,
+) -> int:
     """
     Computes the size (number of atoms) of the maximum common substructure between molecules.
 
     :param mols: An iterable of molecules.
+    :param match_valences: Whether to match valences when computing the MCS.
+    :param ring_matches_ring_only: Whether to only match rings to rings when computing the MCS.
+    :param complete_rings_only: Whether to only match complete rings when computing the MCS.
     :return: The size (number of atoms) of the maximum common substructure between molecules.
     """
-    return FindMCS(mols).numAtoms
+    return FindMCS(mols, matchValences=match_valences, ringMatchesRingOnly=ring_matches_ring_only,
+                   completeRingsOnly=complete_rings_only).numAtoms
 
 
 @register_similarity_function('mcs')
 def compute_pairwise_mcs_similarities(
         mols_1: list[Molecule],
-        mols_2: list[Molecule] | None = None
+        mols_2: list[Molecule] | None = None,
+        match_valences: bool = False,
+        ring_matches_ring_only: bool = False,
+        complete_rings_only: bool = False,
 ) -> np.ndarray:
     """
     Computes pairwise maximum common substructure (MCS) similarities between the molecules in mols_1 and mols_2.
 
     :param mols_1: A list of molecules, either SMILES strings or RDKit molecules.
     :param mols_2: A list of molecules, either SMILES strings or RDKit molecules.
                    If None, copies mols_1 list.
+    :param match_valences: Whether to match valences when computing the MCS.
+    :param ring_matches_ring_only: Whether to only match rings to rings when computing the MCS.
+    :param complete_rings_only: Whether to only match complete rings when computing the MCS.
     :return: A 2D numpy array of pairwise similarities.
     """
     # Convert SMILES to RDKit molecules if needed
     mols_1 = [
         Chem.MolFromSmiles(mol) if isinstance(mol, str) else mol
         for mol in mols_1
     ]
@@ -109,18 +126,26 @@
         mols_2 = [
             Chem.MolFromSmiles(mol) if isinstance(mol, str) else mol
             for mol in mols_2
         ]
     else:
         mols_2 = mols_1
 
+    # Set up MCS function
+    compute_mcs_size_fn = partial(
+        compute_mcs_size,
+        match_valences=match_valences,
+        ring_matches_ring_only=ring_matches_ring_only,
+        complete_rings_only=complete_rings_only
+    )
+
     # Compute pairwise MCS similarities
     with Pool() as pool:
         pairwise_mcs = np.array(
-            list(tqdm(pool.imap(compute_mcs_size, product(mols_1, mols_2)),
+            list(tqdm(pool.imap(compute_mcs_size_fn, product(mols_1, mols_2)),
                       total=len(mols_1) * len(mols_2)))
         )
 
     pairwise_mcs = pairwise_mcs.reshape(len(mols_1), len(mols_2))
 
     num_atoms_2 = np.array([mol.GetNumAtoms() for mol in mols_2])
     mcs_similarities = pairwise_mcs / num_atoms_2
@@ -142,15 +167,16 @@
     :param mols_1: A list of molecules, either SMILES strings or RDKit molecules.
     :param mols_2: A list of molecules, either SMILES strings or RDKit molecules.
                    If None, copies mols_1 list.
     :return: A 2D numpy array of pairwise similarities.
     """
     # Compute Morgan fingerprints
     fps_1 = np.array(compute_fingerprints(mols_1, fingerprint_type='morgan'), dtype=int)
-    fps_2 = np.array(compute_fingerprints(mols_2, fingerprint_type='morgan'), dtype=int) if mols_2 is not None else fps_1
+    fps_2 = np.array(compute_fingerprints(mols_2, fingerprint_type='morgan'),
+                     dtype=int) if mols_2 is not None else fps_1
 
     # Compute pairwise Tversky similarities
     intersection = fps_1 @ fps_2.transpose()
     size_2 = fps_2.sum(axis=1)
     tversky_similarities = intersection / size_2
 
     return tversky_similarities
```

### Comparing `chemfunc-1.0.6/chemfunc/nearest_neighbor.py` & `chemfunc-1.0.7/chemfunc/nearest_neighbor.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 def nearest_neighbor(
         data_path: Path,
         reference_data_path: Path,
         metric: Literal['tanimoto', 'mcs', 'tversky'] = 'tanimoto',
         save_path: Path | None = None,
         smiles_column: str = SMILES_COLUMN,
         reference_smiles_column: str | None = None,
-        reference_name: str | None = None
+        reference_name: str | None = None,
+        match_valences: bool = False,
+        ring_matches_ring_only: bool = False,
+        complete_rings_only: bool = False,
 ) -> None:
     """Given a dataset, computes the nearest neighbor molecule by Tanimoto similarity in a second dataset.
 
     :param data_path: Path to CSV file containing data with SMILES whose neighbors are to be computed.
     :param reference_data_path: Path to CSV file containing reference SMILES which will be the neighbors of data_path.
     :param metric: Metric to use when computing similarity.
                    tanimoto: Tanimoto similarity using Morgan fingerprint.
@@ -28,14 +31,17 @@
                    tversky: Tversky index with alpha = 0 and beta = 1, i.e., the proportion of reference substructures
                    in the molecule.
     :param save_path: Where the data with the neighbor info should be saved (defaults to data_path).
     :param smiles_column: Name of the column in data_path containing SMILES.
     :param reference_smiles_column: Name of the column in reference_data_path containing SMILES.
                                     If None, then smiles_column is used.
     :param reference_name: Name of the reference data when naming the new columns with neighbor info.
+    :param match_valences: For MCS only, whether to match valences when computing the MCS.
+    :param ring_matches_ring_only: For MCS only, whether to only match rings to rings when computing the MCS.
+    :param complete_rings_only: For MCS only, whether to only match complete rings when computing the MCS.
     """
     # Set save path
     if save_path is None:
         save_path = data_path
 
     # Set reference smiles column
     if reference_smiles_column is None:
@@ -45,18 +51,29 @@
     data = pd.read_csv(data_path)
     reference_data = pd.read_csv(reference_data_path)
 
     # Sort reference data and drop duplicates
     reference_data.drop_duplicates(subset=reference_smiles_column, inplace=True)
     reference_data.sort_values(by=reference_smiles_column, ignore_index=True, inplace=True)
 
+    # Set up similarity function kwargs
+    if metric == 'mcs':
+        kwargs = {
+            'match_valences': match_valences,
+            'ring_matches_ring_only': ring_matches_ring_only,
+            'complete_rings_only': complete_rings_only,
+        }
+    else:
+        kwargs = {}
+
     print(f'Computing similarities using {metric} metric')
     similarities = get_similarity_function(metric)(
         data[smiles_column],
-        reference_data[reference_smiles_column]
+        reference_data[reference_smiles_column],
+        **kwargs
     )
 
     print('Finding minimum distance SMILES')
     prefix = f'{f"{reference_name}_" if reference_name is not None else ""}{metric}_'
 
     max_similarity_indices = np.argmax(similarities, axis=1)
```

### Comparing `chemfunc-1.0.6/chemfunc/plot_property_distribution.py` & `chemfunc-1.0.7/chemfunc/plot_property_distribution.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/plot_tsne.py` & `chemfunc-1.0.7/chemfunc/plot_tsne.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/sample_molecules.py` & `chemfunc-1.0.7/chemfunc/sample_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/sdf_to_smiles.py` & `chemfunc-1.0.7/chemfunc/sdf_to_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/select_from_clusters.py` & `chemfunc-1.0.7/chemfunc/select_from_clusters.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/smiles_to_svg.py` & `chemfunc-1.0.7/chemfunc/smiles_to_svg.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/utils.py` & `chemfunc-1.0.7/chemfunc/utils.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/visualize_molecules.py` & `chemfunc-1.0.7/chemfunc/visualize_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc/visualize_reactions.py` & `chemfunc-1.0.7/chemfunc/visualize_reactions.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/chemfunc.egg-info/PKG-INFO` & `chemfunc-1.0.7/chemfunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.6
+Version: 1.0.7
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.6.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.7.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chemfunc-1.0.6/chemfunc.egg-info/SOURCES.txt` & `chemfunc-1.0.7/chemfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.6/setup.py` & `chemfunc-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     install_requires=[
         'descriptastorus',
         'matplotlib',
         'numpy',
         'pandas',
         'rdkit',
         'scikit-learn',
-        'tqdm',
+        'tqdm>=4.66.3',
         'typed-argument-parser>=1.9.0'
     ],
     python_requires='>=3.10',
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

