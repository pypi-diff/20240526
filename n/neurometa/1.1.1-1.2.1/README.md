# Comparing `tmp/neurometa-1.1.1.tar.gz` & `tmp/neurometa-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurometa-1.1.1.tar", max compression
+gzip compressed data, was "neurometa-1.2.1.tar", max compression
```

## Comparing `neurometa-1.1.1.tar` & `neurometa-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      748 2023-05-19 06:47:12.696689 neurometa-1.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-19 06:47:12.696689 neurometa-1.1.1/neurometa/__init__.py
--rw-r--r--   0        0        0    23589 2023-11-12 08:08:53.684475 neurometa-1.1.1/neurometa/constant.py
--rw-r--r--   0        0        0    12022 2023-10-26 11:15:00.054908 neurometa-1.1.1/neurometa/scrape.py
--rw-r--r--   0        0        0    17077 2023-05-19 06:47:12.697689 neurometa-1.1.1/neurometa/static/wikipedia_table.ods
--rw-r--r--   0        0        0      949 2023-11-12 08:12:25.869961 neurometa-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 neurometa-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      748 2023-05-19 06:47:12.000000 neurometa-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 06:47:12.000000 neurometa-1.2.1/neurometa/__init__.py
+-rw-r--r--   0        0        0    25218 2023-12-03 21:16:23.000000 neurometa-1.2.1/neurometa/constant.py
+-rw-r--r--   0        0        0    11532 2023-12-03 21:18:28.000000 neurometa-1.2.1/neurometa/scrape.py
+-rw-r--r--   0        0        0    17077 2023-05-19 06:47:12.000000 neurometa-1.2.1/neurometa/static/wikipedia_table.ods
+-rw-r--r--   0        0        0     1155 2024-05-26 18:57:09.598883 neurometa-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1799 1970-01-01 00:00:00.000000 neurometa-1.2.1/PKG-INFO
```

### Comparing `neurometa-1.1.1/README.md` & `neurometa-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `neurometa-1.1.1/neurometa/constant.py` & `neurometa-1.2.1/neurometa/constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     BOMBESIN = "bombesin"
     BRADYKININ = "bradykinin"
     CALCITONIN = "calcitonin"
     CALCITONIN_GENE_RELATED_PEPTIDE = "calcitonin gene related peptide"
     CARBON_MONOXIDE = "carbon monoxide"
     CHOLECYSTOKININ = "cholecystokinin"
     CHROMOGRANIN_A = "chromogranin a"
-    COCAINE_AND_AMPHETAMINE_REGULATED_TRANSCRIPT = (
-        "cocaine and amphetamine regulated transcript"
-    )
+    COCAINE_AND_AMPHETAMINE_REGULATED_TRANSCRIPT = "cocaine and amphetamine regulated transcript"
     COPEPTIN = "copeptin"
     CORTICOTROPIN_RELEASING_HORMONE = "corticotropin releasing hormone"
     DOPAMINE = "dopamine"
     DYNORPHINS = "dynorphins"
     D_SERINE = "d serine"
     ENDOMORPHINS = "endomorphins"
     ENDORPHINS = "endorphins"
@@ -79,17 +77,15 @@
     OREXIN_A = "orexin a"
     OREXIN_B = "orexin b"
     OXYTOCIN = "oxytocin"
     PANCREATIC_POLYPEPTIDE = "pancreatic polypeptide"
     PARATHYROID_HORMONE_RELATED_PROTEIN = "parathyroid hormone related protein"
     PEPTIDE_YY = "peptide yy"
     PHENETHYLAMINE = "phenethylamine"
-    PITUITARY_ADENYLATE_CYCLASE_ACTIVATING_PEPTIDE = (
-        "pituitary adenylate cyclase activating peptide"
-    )
+    PITUITARY_ADENYLATE_CYCLASE_ACTIVATING_PEPTIDE = "pituitary adenylate cyclase activating peptide"
     PROLACTIN_RELEASING_PEPTIDE = "prolactin releasing peptide"
     PROOPIOMELANOCORTIN = "proopiomelanocortin"
     PYROGLUTAMYLATED_RFAMIDE_PEPTIDE = "pyroglutamylated rfamide peptide"
     SECRETIN = "secretin"
     SEROTONIN = "serotonin"
     SOMATOSTATIN = "somatostatin"
     SUBSTANCE_P = "substance p"
@@ -578,7 +574,35 @@
 
 class GeneExpression(Enum):
     KNOCK_OUT = "knock-out"
     KNOCK_IN = "knock-in"
     KNOCK_DOWN = "knock-down"
     KNOCK_SIDEWAYS = "knock-sideways"
     OVEREXPRESSION = "overexpression"
+
+
+class NeuronPolarity(Enum):
+    UNIPOLAR = "unipolar"  # Neurons with a single process
+    BIPOLAR = "bipolar"  # Neurons with two processes (one axon, one dendrite)
+    ANAXONIC = "anaxonic"  # Neurons without a clear axon
+    PSEUDOUNIPOLAR = "pseudounipolar"  # Neurons with a single process that divides into two branches
+    MULTIPOLAR = "multipolar"  # Neurons with one axon and multiple dendrites
+
+
+class NeuronType(Enum):
+    BASKET = "basket"  # Inhibitory interneurons in the brain
+    BETZ = "betz"  # Large pyramidal neurons in the primary motor cortex
+    LUGARO = "lugaro"  # Neurons in the cerebellar cortex
+    MEDIUM_SPINY = "medium spiny"  # Principal neurons of the striatum
+    PURKINJE = "purkinje"  # Large neurons in the cerebellar cortex
+    PYRAMIDAL = "pyramidal"  # Neurons with pyramid-shaped cell bodies in the cerebral cortex
+    RENSHAW = "renshaw"  # Interneurons in the spinal cord
+    UNIPOLAR_BRUSH = "unipolar brush"  # Neurons found in the cerebellum
+    GRANULE = "granule"  # Small neurons in the cerebellum and olfactory bulb
+    MOTOR = "motor"  # Neurons that send impulses to muscles
+    SPINDLE = "spindle"  # Sensory neurons in muscles
+    FAN = "fan"  # A type of neuron (need more specific context)
+    STELLATE = "stellate"  # Star-shaped interneurons in the cerebral cortex
+    CHANDELIER = "chandelier"  # A type of inhibitory interneuron in the cerebral cortex
+    GOLGI = "golgi"  # Inhibitory interneurons in the cerebellum
+    MARTINOTTI = "martinotti"  # Interneurons found throughout the cerebral cortex
+    CAJAL_RETZIUS = "cajal_retzius"  # Early-developing neurons in the marginal zone of the cortex
```

### Comparing `neurometa-1.1.1/neurometa/scrape.py` & `neurometa-1.2.1/neurometa/scrape.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import pkgutil
 import re
 from copy import copy
 from datetime import date
 from pathlib import Path
 from pprint import pprint
 from typing import Optional
 
@@ -18,27 +19,23 @@
             deeper_section.title: _scrape_sessions_from_wiki_class(deeper_section)
             for deeper_section in root_section.sections
         }
     else:
         return root_section.title
 
 
-def _define_depth_for_every_subfield(
-    rem_section, rem_section_data, previous_subsection
-):
+def _define_depth_for_every_subfield(rem_section, rem_section_data, previous_subsection):
     current_subsections = previous_subsection[rem_section]
 
     subsections, substructures = {}, []
     for i, data in enumerate(rem_section_data, start=1):
         if isinstance(data, dict):
             subsections.update(data)
         elif data in current_subsections:
-            subsections[data] = _define_depth_for_every_subfield(
-                data, rem_section_data[i:], current_subsections
-            )
+            subsections[data] = _define_depth_for_every_subfield(data, rem_section_data[i:], current_subsections)
         else:
             substructures.append(data)
 
     if subsections:
         subsections["Substructures"] = substructures
         return subsections
     return substructures
@@ -46,59 +43,52 @@
 
 def scrape_human_brain_tree() -> dict:
     def recursive_set_adder(data_to_add):
         if isinstance(data_to_add, str):
             flattened_structure_dataset.add(data_to_add.capitalize())
         elif isinstance(data_to_add, dict):
             for subsection_name, recursive_subsection in data_to_add.items():
-                if any(
-                    recursive_data.isdigit() for recursive_data in recursive_subsection
-                ):
+                if any(recursive_data.isdigit() for recursive_data in recursive_subsection):
                     for daughter_tag in recursive_subsection:
-                        flattened_structure_dataset.add(
-                            f"{subsection_name} {daughter_tag}"
-                        )
+                        flattened_structure_dataset.add(f"{subsection_name} {daughter_tag}")
                 else:
                     recursive_set_adder(recursive_subsection)
         else:
             for recursive_data in data_to_add:
                 recursive_set_adder(recursive_data)
 
     deli = re.compile(r"[,;]")
     parenthesis_exp = re.compile(r"\([\w,; ]*\)")
     id_followed_by_numbering = re.compile(r"^[\w ]* \d+")
 
-    wiki_api = wikipediaapi.Wikipedia(
-        language="en", extract_format=wikipediaapi.ExtractFormat.WIKI
-    )
+    wiki_api = wikipediaapi.Wikipedia(language="en", extract_format=wikipediaapi.ExtractFormat.WIKI)
 
     wiki_page = wiki_api.page("List_of_regions_in_the_human_brain")
 
     section_titles = {}
     for section in wiki_page.sections:
         section_titles[section.title] = _scrape_sessions_from_wiki_class(section)
 
-    data, section_data = {}, []
-    section, deeper_section, current_section_field = None, None, None
+    data = {}
+    section_data = []
+    section = None
     for line in wiki_page.text.splitlines():
         if "Related topics" in line:
             break
 
         if not line or (":" not in line and len(line.split(" ")) >= 15):
             continue
         elif line in section_titles:
             if section:
                 data[section] = copy(section_data)
                 section_data = []
             section = line
         else:
             assert section
-            if (parenthesis_exp_findings := re.findall(parenthesis_exp, line)) and len(
-                parenthesis_exp_findings
-            ) == 1:
+            if (parenthesis_exp_findings := re.findall(parenthesis_exp, line)) and len(parenthesis_exp_findings) == 1:
                 split_line = re.split(parenthesis_exp, line)
                 if len(split_line) == 2:
                     if not split_line[1]:
                         section_data.append(line.strip())
                         continue
 
             if " and " in line.lower():
@@ -135,36 +125,28 @@
                 # section_data.append({parent: [daughter for daughter in daughters if daughter.lower() == "other"]})
                 section_data.append({parent: daughters})
             else:
                 section_data.append(line)
 
     data_with_depth = {}
     for section, section_data in data.items():
-        data_with_depth[section] = _define_depth_for_every_subfield(
-            section, section_data, section_titles
-        )
+        data_with_depth[section] = _define_depth_for_every_subfield(section, section_data, section_titles)
 
     organized_data = {"neuronal_structure": {}}
     for section_name, data in data_with_depth.items():
         if "Neurotransmitter pathways" == section_name:
             organized_data["neurotransmitter"] = data
         elif "Neural pathways" == section_name:
             organized_data["neuronal_pathway"] = data
         else:
             organized_data["neuronal_structure"][section_name] = data
 
-    organized_data["neuro_endocrine_system"] = organized_data["neuronal_structure"].pop(
-        "Neuro endocrine systems"
-    )
-    organized_data["neuro_vascular_system"] = organized_data["neuronal_structure"].pop(
-        "Neuro vascular systems"
-    )
-    organized_data["dural_meningeal_system"] = organized_data["neuronal_structure"].pop(
-        "Dural meningeal system"
-    )
+    organized_data["neuro_endocrine_system"] = organized_data["neuronal_structure"].pop("Neuro endocrine systems")
+    organized_data["neuro_vascular_system"] = organized_data["neuronal_structure"].pop("Neuro vascular systems")
+    organized_data["dural_meningeal_system"] = organized_data["neuronal_structure"].pop("Dural meningeal system")
 
     flattened_structure_dataset = set()
 
     for subsection in organized_data["neuronal_structure"].values():
         recursive_set_adder(subsection)
 
     flattened_structure_dataset.remove("Surface")  # Absurd brain structure.
@@ -184,27 +166,23 @@
             iterable = sorted(parenthesis_content.split("and"))
         else:
             iterable = (parenthesis_content,)
         [name.replace("also", "").strip().lower() for name in iterable if len(name) > 3]
         standard_name_to_names[names] = (standard_name, *iterable)
 
     organized_data["neuronal_structure_flat"] = flattened_structure_dataset
-    organized_data["standard_name_to_names"] = dict(
-        sorted(standard_name_to_names.items())
-    )
+    organized_data["standard_name_to_names"] = dict(sorted(standard_name_to_names.items()))
     organized_data = dict(sorted(organized_data.items()))
 
     return organized_data
 
 
 def scrape_neurotransmitter() -> dict:
     standard_neurotransmitter_names, neurotransmitter_with_alternative_names = [], []
-    for row in pd.read_excel(
-        pkgutil.get_data(__name__, "wikipedia_table.ods")
-    ).iterrows():
+    for row in pd.read_excel(pkgutil.get_data(__name__, "wikipedia_table.ods")).iterrows():
         row = row[1]
         name, abbreviation = row[1:3]
 
         name = name.strip().replace("\xa0", " ")
         if "(" in name:
             name, alternative_name = name.split("(")
             name = name.strip()
@@ -220,55 +198,45 @@
             abbreviation = abbreviation.strip().replace("\xa0", " ")
             names = f"{name}; {abbreviation}"
         if alternative_name:
             names += f"; {alternative_name}"
 
         neurotransmitter_with_alternative_names.append(names)
 
-    return dict(
-        zip(standard_neurotransmitter_names, neurotransmitter_with_alternative_names)
-    )
+    return dict(zip(standard_neurotransmitter_names, neurotransmitter_with_alternative_names))
 
 
 def scrape_model_organism() -> dict:
     def section_unpacker(recursive_section, current_dict: Optional[dict] = None):
         unpacked_data = current_dict or {}
         if recursive_section.text:
             for line in recursive_section.text.split("\n"):
                 processed_line = line.split(",")[0].strip()
 
-                if (
-                    not processed_line
-                    or "References" in processed_line
-                    or ":" in processed_line
-                ):
+                if not processed_line or "References" in processed_line or ":" in processed_line:
                     continue
 
                 parenthesis_split = processed_line.split(" (")
                 scientific_names = parenthesis_split[0].strip()
                 try:
-                    cultural_name = (
-                        parenthesis_split[1].replace(")", "").strip().capitalize()
-                    )
+                    cultural_name = parenthesis_split[1].replace(")", "").strip().capitalize()
                 except IndexError:
                     # No cultural name defined
                     cultural_name = ""
 
                 for species_name in scientific_names.split(" and "):
                     unpacked_data[species_name.capitalize()] = cultural_name
 
         else:
             for sub_section in recursive_section.sections:
                 unpacked_data = section_unpacker(sub_section, unpacked_data)
 
         return unpacked_data
 
-    wiki_api = wikipediaapi.Wikipedia(
-        language="en", extract_format=wikipediaapi.ExtractFormat.WIKI
-    )
+    wiki_api = wikipediaapi.Wikipedia(language="en", extract_format=wikipediaapi.ExtractFormat.WIKI)
     wiki_page = wiki_api.page("List_of_model_organisms")
 
     result = {}
     for section in wiki_page.sections:
         if "Eukaryotes" == section.title:
             for eu_section in section.sections:
                 result[eu_section.title] = section_unpacker(section)
@@ -302,17 +270,15 @@
 
             with open(dataset_dir / latest_dataset_filename, "rb") as in_json:
                 latest_dataset = json.load(in_json)
 
             difference = DeepDiff(dataset, latest_dataset, ignore_order=True)
             difference.pop("type_changes", None)
             if not difference:
-                return print(
-                    "Done: No change in data since last save, nothing new to store"
-                )
+                return print("Done: No change in data since last save, nothing new to store")
 
             print("Difference:")
             pprint(difference, indent=2, width=200)
 
         new_dataset_filename = dataset_dir / f"{dataset_label}_{date.today()}.json"
         with open(new_dataset_filename, "w") as out_json:
             json.dump(dataset, out_json)
```

### Comparing `neurometa-1.1.1/neurometa/static/wikipedia_table.ods` & `neurometa-1.2.1/neurometa/static/wikipedia_table.ods`

 * *Files identical despite different names*

### Comparing `neurometa-1.1.1/PKG-INFO` & `neurometa-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurometa
-Version: 1.1.1
+Version: 1.2.1
 Summary: Package for generating metadata related to neuroscience
 Home-page: https://github.com/memorycircuits/neurometa
 License: BSD-3-Clause
 Author: Can H. Tartanoglu
 Author-email: canhtart@gmail.com
 Maintainer: Can H. Tartanoglu
 Maintainer-email: canhtart@gmail.com
@@ -12,18 +12,19 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: gen
 Requires-Dist: Wikipedia-API (>=0.5.4,<0.6.0) ; extra == "gen"
 Requires-Dist: deepdiff (>=5.8.0,<6.0.0) ; extra == "gen"
-Requires-Dist: pandas[excel,performance]
+Requires-Dist: pandas[excel,performance] ; extra == "gen"
 Project-URL: Repository, https://github.com/memorycircuits/neurometa
 Description-Content-Type: text/markdown
 
 # Neurometa
 
 ## Installation
```

