# Comparing `tmp/neurocaps-0.9.2.tar.gz` & `tmp/neurocaps-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.2.tar", last modified: Sat May 25 00:49:59 2024, max compression
+gzip compressed data, was "neurocaps-0.9.3.tar", last modified: Sun May 26 10:35:13 2024, max compression
```

## Comparing `neurocaps-0.9.2.tar` & `neurocaps-0.9.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.144962 neurocaps-0.9.2/
--rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.2/LICENSE.md
--rw-rw-rw-   0        0        0    16232 2024-05-25 00:49:59.134579 neurocaps-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    14914 2024-05-24 23:48:48.000000 neurocaps-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.038452 neurocaps-0.9.2/neurocaps/
--rw-rw-rw-   0        0        0       78 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.095996 neurocaps-0.9.2/neurocaps/_utils/
--rw-rw-rw-   0        0        0      369 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.102977 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/
--rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/__init__.py
--rw-rw-rw-   0        0        0     2591 2024-05-09 19:38:42.000000 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-rw-rw-   0        0        0      186 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.114978 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/
--rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-rw-rw-   0        0        0     2863 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
--rw-rw-rw-   0        0        0     5777 2024-05-23 03:16:17.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-rw-rw-   0        0        0     2701 2024-05-22 00:17:25.000000 neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.118327 neurocaps-0.9.2/neurocaps/analysis/
--rw-rw-rw-   0        0        0      143 2024-05-14 02:35:32.000000 neurocaps-0.9.2/neurocaps/analysis/__init__.py
--rw-rw-rw-   0        0        0    68833 2024-05-24 23:48:48.000000 neurocaps-0.9.2/neurocaps/analysis/cap.py
--rw-rw-rw-   0        0        0     4811 2024-05-14 02:35:32.000000 neurocaps-0.9.2/neurocaps/analysis/merge.py
--rw-rw-rw-   0        0        0     1598 2024-05-14 02:35:32.000000 neurocaps-0.9.2/neurocaps/analysis/standardize.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.128526 neurocaps-0.9.2/neurocaps/extraction/
--rw-rw-rw-   0        0        0       89 2024-04-28 16:38:21.000000 neurocaps-0.9.2/neurocaps/extraction/__init__.py
--rw-rw-rw-   0        0        0    30437 2024-05-24 23:48:48.000000 neurocaps-0.9.2/neurocaps/extraction/timeseriesextractor.py
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.134579 neurocaps-0.9.2/neurocaps.egg-info/
--rw-rw-rw-   0        0        0    16232 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-25 00:49:58.000000 neurocaps-0.9.2/neurocaps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1491 2024-05-25 00:49:27.000000 neurocaps-0.9.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-25 00:49:59.145975 neurocaps-0.9.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-25 00:49:59.134579 neurocaps-0.9.2/tests/
--rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.2/tests/test_CAP.py
--rw-rw-rw-   0        0        0     3767 2024-05-09 19:38:42.000000 neurocaps-0.9.2/tests/test_TimeseriesExtractor.py
--rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.2/tests/test_TimeseriesExtractor_additional.py
--rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.2/tests/test_merge_dicts.py
--rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.2/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.069695 neurocaps-0.9.3/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.3/LICENSE.md
+-rw-rw-rw-   0        0        0    16348 2024-05-26 10:35:13.064699 neurocaps-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    15021 2024-05-26 10:30:02.000000 neurocaps-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.858389 neurocaps-0.9.3/neurocaps/
+-rw-rw-rw-   0        0        0       72 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.942511 neurocaps-0.9.3/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      363 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.959177 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      184 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:12.994591 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-23 03:16:17.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2847 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-23 03:16:16.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2680 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.016421 neurocaps-0.9.3/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      139 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    69880 2024-05-26 10:33:29.000000 neurocaps-0.9.3/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4803 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1595 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.027554 neurocaps-0.9.3/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       87 2024-05-26 10:24:45.000000 neurocaps-0.9.3/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    31128 2024-05-26 10:33:29.000000 neurocaps-0.9.3/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.060701 neurocaps-0.9.3/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    16348 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-26 10:35:12.000000 neurocaps-0.9.3/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1499 2024-05-26 10:24:45.000000 neurocaps-0.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:35:13.070444 neurocaps-0.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 10:35:13.049929 neurocaps-0.9.3/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.3/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     4687 2024-05-25 04:47:35.000000 neurocaps-0.9.3/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-23 03:16:16.000000 neurocaps-0.9.3/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.3/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.3/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.2/LICENSE.md` & `neurocaps-0.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.2/PKG-INFO` & `neurocaps-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.2
+Version: 0.9.3
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -22,15 +22,15 @@
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: kneed
 Requires-Dist: nibabel
-Requires-Dist: nilearn==0.10.2
+Requires-Dist: nilearn!=0.10.3,>=0.10.1
 Requires-Dist: surfplot
 Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
@@ -65,24 +65,24 @@
 pip install -e .
 
 ```
 
 # Usage
 **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes)**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
 
 If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
 
 Custom Key Structure:
 - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
 - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
 visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
 Example 
 The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
 ```Python
 parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
@@ -93,27 +93,28 @@
  ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
 - Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+- Ability to use parallel processing by specifying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
 
 **Main features for `CAP` includes:**
 
 - Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
 - Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
-- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
-- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Visualizing the CAPs identified as an outer product or heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `caps2plot()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
+- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
+- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
 - Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
 different CAPs across the entire run.
 
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+**Additionally, the `neurocaps.analysis` submodule contains two additional functions**:
+- The `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
 Quick code example:
 
 ```python
 # Examples use randomized data
@@ -155,25 +156,25 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True)
 
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
 
 ```
-**Graph Outputs:**
+**Plot Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
@@ -194,25 +195,27 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
-# Create surface plots of CAPs
+# Create surface plots of CAPs; there will be as many plots as CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
+**Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
 ```python
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+**Plot Output:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
```

### Comparing `neurocaps-0.9.2/README.md` & `neurocaps-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 pip install -e .
 
 ```
 
 # Usage
 **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes)**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
 
 If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
 
 Custom Key Structure:
 - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
 - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
 visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
 Example 
 The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
 ```Python
 parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
@@ -60,27 +60,28 @@
  ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
 - Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+- Ability to use parallel processing by specifying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
 
 **Main features for `CAP` includes:**
 
 - Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
 - Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
-- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
-- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Visualizing the CAPs identified as an outer product or heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `caps2plot()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
+- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
+- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
 - Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
 different CAPs across the entire run.
 
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+**Additionally, the `neurocaps.analysis` submodule contains two additional functions**:
+- The `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
 Quick code example:
 
 ```python
 # Examples use randomized data
@@ -122,25 +123,25 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True)
 
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
 
 ```
-**Graph Outputs:**
+**Plot Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
@@ -161,25 +162,27 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
-# Create surface plots of CAPs
+# Create surface plots of CAPs; there will be as many plots as CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
+**Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
 ```python
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+**Plot Output:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
```

### Comparing `neurocaps-0.9.2/neurocaps/_utils/_cap_internals/_capgetter.py` & `neurocaps-0.9.3/neurocaps/_utils/_cap_internals/_capgetter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .._timeseriesextractor_internals._check_parcel_approach import _check_parcel_approach
 
-# A class which is responsible for accessing all CAPMetadata and to keep track of all attributes in CAP
+# A class which is responsible for accessing all CAP metadata and to keep track of all attributes in CAP
 class _CAPGetter:
     def __init__(self):
         pass
     
     ### Attributes exist when CAP initialized
     @property
     def n_clusters(self):
@@ -81,19 +81,8 @@
     def means(self):
         if hasattr(self, "_mean_vec"): return self._mean_vec
         else: return None
 
     @property
     def stdev(self):
         if hasattr(self, "_stdev_vec"): return self._stdev_vec
-        else: return None
-
-
-    
-
-
-    
-     
-     
-     
-     
-         
+        else: return None
```

### Comparing `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py` & `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
 def _check_confound_names(high_pass, specified_confound_names, n_acompcor_separate):
     if specified_confound_names == None:
         if high_pass:
-            # Do not use cosine or acompcor regressor if high pass filtering is not None. Acompcor regressors are estimated on high pass filtered version 
-            # of data form fmriprep
+            # Do not use cosine or acompcor regressor if high pass filtering is not None. Acompcor regressors are estimated on high pass filtered version of data form fmriprep
             confound_names = [
                 "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
                 "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
                 "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
                 "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
                 "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
                 "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2"
```

### Comparing `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,19 @@
     
     if "Custom" in parcel_approach.keys():
         if call  == "TimeseriesExtractor" and "maps" not in parcel_approach["Custom"].keys():
             raise ValueError(f"For `Custom` parcel_approach, a nested key-value pair containing the key 'maps' with the value being a string specifying the location of the parcellation is needed.\nExample: {{'Custom' : valid_parcel_dict['Custom']}}")
         check_subkeys = ["nodes" in parcel_approach["Custom"].keys(), "regions" in parcel_approach["Custom"].keys()]
         if not all(check_subkeys):
             missing_subkeys = [["nodes", "regions"][x] for x,y in enumerate(check_subkeys) if y == False]
-            error_message = f"The following subkeys haven't been detected {missing_subkeys}."
-            if call == "TimeseriesExtractor": warnings.warn(error_message + " These labels are not needed for timeseries extraction but are needed for future timeseries or CAPs plotting.")
+            error_message = f"The following subkeys haven't been detected {missing_subkeys}"
+            if call == "TimeseriesExtractor": warnings.warn(f"{error_message}. These labels are not needed for timeseries extraction but are needed for future timeseries or CAPs plotting.")
             else: 
                 custom_example = {"Custom": {"nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
                                              "regions": {"Vis" : {"lh": [0,1],
                                                                    "rh": [3,4]}},
                                                                    "Hippocampus": {"lh": [2],"rh": [5]}}}
-                raise ValueError(error_message + f" These subkeys are needed for plotting. Please reassign `parcel_approach` using `self.parcel_approach` amd refer to the example structure: {custom_example}")
+                raise ValueError(f"{error_message}. These subkeys are needed for plotting. Please reassign `parcel_approach` using `self.parcel_approach` amd refer to the example structure: {custom_example}")
         if call  == "TimeseriesExtractor" and not os.path.isfile(parcel_approach["Custom"]["maps"]):
             raise ValueError("Please specify the location to the custom parcellation to be used.")
 
     return parcel_approach
```

### Comparing `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.2/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.3/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from ._check_parcel_approach import _check_parcel_approach
-# A class which is responsible for acessing all TimeseriesExtractorGetter and to keep track of all attributes in TimeSeriesExtractor
+# A class which is responsible for accessing all TimeseriesExtractorGetter and to keep track of all attributes in TimeSeriesExtractor
 class _TimeseriesExtractorGetter:
     def __init__(self):
         pass
     
     #### Exists upon initialization of TimeseriesExtractor
     @property
     def space(self):
@@ -55,11 +55,8 @@
             first_level_indx = list(subject_dict.keys())[0]
             if isinstance(subject_dict[first_level_indx], dict) and len(subject_dict[first_level_indx].keys()) != 0 and "run" in list(subject_dict[first_level_indx].keys())[0]: 
                 run = list(subject_dict[first_level_indx].keys())[0]
                 if isinstance(subject_dict[first_level_indx][run],np.ndarray): 
                     self._subject_timeseries = subject_dict
                 else: raise TypeError(error_message) 
             else: raise TypeError(error_message) 
-        else: raise TypeError(error_message)
-    
-    
-        
+        else: raise TypeError(error_message)
```

### Comparing `neurocaps-0.9.2/neurocaps/analysis/cap.py` & `neurocaps-0.9.3/neurocaps/analysis/cap.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,40 +3,30 @@
 from sklearn.cluster import KMeans
 from typing import Union, Literal
 from .._utils import _CAPGetter, _convert_pickle_to_dict, _check_parcel_approach
 
 
 class CAP(_CAPGetter):
     def __init__(self, parcel_approach: dict[dict], n_clusters: Union[int, list[int]]=5, cluster_selection_method: str=None, groups: dict=None):
-        """
-        Initialize the CAP (Co-activation Patterns) analysis class.
+        """CAP class
+
+        Initializes the CAPs (Co-activation Patterns) class.
 
         Parameters
         ----------
-        node_labels : list[str]
+        node_labels: list[str]
             Decoded or non-decoded Schaefer Atlas labels for the nodes.
-        n_clusters : int or list[int], default=5
+        n_clusters: int or list[int], default=5
             The number of clusters to use. Can be a single integer or a list of integers.
         cluster_selection_method: str, default=None
             Method to find the optimal number of clusters. Options are "silhouette" or "elbow".
-        groups : dict, default=None
+        groups: dict, default=None
             A mapping of group names to subject IDs. Each group contains subject IDs for
             separate CAP analysis. If None, CAPs are not separated by group.
 
-        Raises
-        ------
-        ValueError
-            If `cluster_selection_method` is none when `n_clusters` is a list.
-        ValueError
-            If `cluster_selection_method` is used when `n_clusters` is a single integer.
-        TypeError
-            If `groups` is provided but is not a dictionary.
-        AssertionError
-            If any group in `groups` has zero subject IDs.
-
         Notes
         -----
         The initialization ensures unique values if `n_clusters` is a list and checks for 
         valid input types and values.
         """
         # Ensure all unique values if n_clusters is a list
         self._n_clusters = n_clusters if type(n_clusters) == int else sorted(list(set(n_clusters)))
@@ -72,15 +62,15 @@
         
         self._parcel_approach = parcel_approach 
 
     def get_caps(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], runs: Union[int, list[int]]=None, random_state: int=None, 
                  init: Union[np.array, Literal["k-means++", "random"]]="k-means++", n_init: Union[Literal["auto"],int]='auto', 
                  max_iter: int=300, tol: float=0.0001, algorithm: Literal["lloyd", "elkan"]="lloyd", show_figs: bool=False, 
                  output_dir: str=None, standardize: bool=True, epsilon: Union[int,float]=0, **kwargs) -> None:
-        """"" Create CAPs
+        """""Generate CAPs
 
         The purpose of this function is to concatenate the timeseries of each subject and perform kmeans clustering on the concatenated data.
         
         Parameters
         ----------
         subject_timeseries: dict or str
             A pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
@@ -101,24 +91,23 @@
         tol: float, default=1e-4,
             Stopping criteria if the change of inertia is below value assuming `max_iter` has not been reached.
         algorithm: "lloyd or "elkan", default="lloyd"
             The type of algorithm to use. Please refer to scikit's KMeans documentation for more information.
         show_figs: bool, default=False
             Display the plots of inertia scores for all groups if `cluster_selection_method`="elbow".
         output_dir: str, default=None
-            Directory to save plot in if `cluster_selection_method`="elbow".
+            Directory to save plot in if `cluster_selection_method`="elbow". Will create the directory if it does not exist.
         standardize: bool, default=True
             To z-score the features of the concatonated timeseries array.
         epsilon: int or float, default=0
             Small number to add to the denominator when z-scoring for numerical stabilty.
         kwargs: dict
             Dictionary to adjust certain parameters related to `cluster_selection_method`="elbow". Additional parameters includes "S", which adjust the sensitivity of finding the elbow 
             (Larger values of `S` are more conservative and less sensitive to small fluctuations; this package uses KneeLocator from the kneed package to identify the elbow), defaults to 1, 
             "dpi", to adjust the dpi of the elbow plot, defaults to 300, and "figsize", which adjust the size of the elbow plots.
-            
         """
         
         if runs:
             if isinstance(runs,int): runs = list(runs)
     
         self._runs = runs if runs else "all"
         self._standardize = standardize
@@ -157,15 +146,14 @@
                 cluster_labels = self._kmeans[group].labels_
                 self._silhouette_scores[group].update({n_cluster: silhouette_score(self._concatenated_timeseries[group], cluster_labels)})
             self._optimal_n_clusters[group] = max(self._silhouette_scores[group], key=self._silhouette_scores[group].get)
             if self._optimal_n_clusters[group] != self._n_clusters[-1]:
                 self._kmeans[group] = KMeans(n_clusters=self._optimal_n_clusters[group], random_state=random_state, init=init, n_init=n_init, max_iter=max_iter, tol=tol, algorithm=algorithm).fit(self._concatenated_timeseries[group]) 
             print(f"Optimal cluster size for {group} is {self._optimal_n_clusters[group]}.")
         
-    
     def _perform_elbow_method(self, random_state, show_figs, output_dir, init, n_init, max_iter, tol, algorithm, **kwargs):
         # Initialize attribute
         self._inertia = {}
         self._optimal_n_clusters = {}
         self._kmeans = {}
 
         knee_dict = dict(S = kwargs["S"] if "S" in kwargs.keys() else 1)
@@ -203,14 +191,15 @@
                                linestyles="--", label="elbow")
                     plt.legend(loc="best")
                     plt.xlabel("K")
                     plt.ylabel("Inertia")
                     plt.title(group)
 
                     if output_dir:
+                        if not os.path.exists(output_dir): os.makedirs(output_dir)
                         plt.savefig(os.path.join(output_dir,f"{group.replace(' ','_')}_elbow.png"), dpi=plot_dict["dpi"])
                     
                     if show_figs == False:
                         plt.close()
                     else:
                         plt.show()
 
@@ -256,24 +245,24 @@
         for group in self._groups:
             for subj_id in self._groups[group]:
                 if subj_id in self._subject_table.keys():
                     warnings.warn(f"Subject: {subj_id} appears more than once, only including the first instance of this subject in the analysis.") 
                 else:
                     self._subject_table.update({subj_id : group})
 
-    def visualize_caps(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="regions", 
+    def caps2plot(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="regions", 
                        task_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
-        """ Plotting CAPs
+        """Generate heatmaps and outer product plots of CAPs
 
         This function produces seaborn heatmaps for each CAP. If groups were given when the CAP class was initialized, plotting will be done for all CAPs for all groups.
 
         Parameters
         ----------
         output_dir: str, default=None
-            Directory to save plots in. If None, plots will not be saved.
+            Directory to save plots in. Will create the directory if it does not exist. If None, plots will not be saved.
         plot_options: str or list[str], default="outer product"
             Type of plots to create. Options are "outer product" or "heatmap".
         visual_scope: str or list[str], default="regions"
             Determines whether plotting is done at the region level or node level. 
             For region level, the value of each nodes in the same regions are averaged together them plotted.
             Options are "regions" or "nodes".
         task_title: str, default=None
@@ -344,29 +333,29 @@
                              "regions": {"Vis" : {"lh": [0,1],
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
         """
         import itertools, os
 
-        # Check parcel approach
-
+        if not hasattr(self,"_caps"):
+            raise AttributeError("Cannot plot caps since `self._caps` attribute does not exist. Run `self.get_caps()` first.")
+        
         # Check if parcellation_approach is custom
         if "Custom" in self.parcel_approach.keys() and ("nodes" not in self.parcel_approach["Custom"].keys() or "regions" not in self.parcel_approach["Custom"].keys()):
-            _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_caps")
+            _check_parcel_approach(parcel_approach=self._parcel_approach, call="caps2plot")
 
         # Check labels
         check_caps = self._caps[list(self._caps.keys())[0]]
         check_caps = check_caps[list(check_caps.keys())[0]]
         if check_caps.shape[0] != len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]): 
                 raise ValueError("Number of rois/nodes used for CAPs does not equal the number of rois/nodes specified in `parcel_approach`.")
 
         if output_dir:
-            if not os.path.exists(output_dir):
-                os.makedirs(output_dir)
+            if not os.path.exists(output_dir): os.makedirs(output_dir)
 
         # Convert to list
         if type(plot_options) == str: plot_options = [plot_options]
         if type(visual_scope) == str: visual_scope = [visual_scope]
 
         # Check inputs for plot_options and visual_scope
         if not any(["heatmap" in plot_options, "outer product" in plot_options]):
@@ -428,14 +417,15 @@
                 #  Generate plot for each group
                 if plot_option == "outer product": self._generate_outer_product_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns, subplots=subplots,
                                                                                     output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
                 elif plot_option == "heatmap": self._generate_heatmap_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns,
                                                                             output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
             
     def _create_regions(self):
+        # Internal function to create an attribute called `region_caps`. Purpose is to average the vales of all nodes in a corresponding region to create region heatmaps or outer product plots
         self._region_caps = {group: {} for group in self._groups.keys()}
         for group in self._groups.keys():
             for cap in self._caps[group].keys():
                 region_caps = {}
                 if list(self._parcel_approach.keys())[0] != "Custom":
                     for region in self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]:
                         if len(region_caps) == 0:
@@ -561,34 +551,32 @@
                     ticks = [i for i, label in enumerate(labels) if label]  
 
                     display.set_xticks(ticks)  
                     display.set_xticklabels([label for label in labels if label]) 
                     display.set_yticks(ticks)  
                     display.set_yticklabels([label for label in labels if label]) 
                 
-                # Set title
                 display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
-                # Modify label sizes
                 display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
                 display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
                 # Save individual plots
                 if output_dir:
                     partial_filename = f"{group}_{cap}_{task_title}" if task_title else f"{group}_{cap}"
-                    full_filename = f"{partial_filename}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.png"
+                    full_filename = f"{partial_filename.replace(' ','_')}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename.replace(' ','_')}_outer_product_heatmap-nodes.png"
                     display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
         
         # Remove subplots with no data
         if subplots: [fig.delaxes(ax) for ax in axes.flatten() if not ax.has_data()]
 
         # Save subplot
         if subplots and output_dir: 
-            partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.png"
+            partial_filename = f"{group}_CAPs_{task_title}" if task_title else f"{group}_CAPs"
+            full_filename = f"{partial_filename.replace(' ','_')}_outer_product_heatmap-regions.png" if scope == "regions" else f"{partial_filename.replace(' ','_')}_outer_product_heatmap-nodes.png"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
         
         # Display figures
         if not show_figs: plt.close()
 
     def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
         import matplotlib.pyplot as plt, os, pandas as pd
@@ -626,37 +614,38 @@
                     starting_value += frequency_dict[names_list[num-1]] 
                     labels[starting_value] = name
 
             display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]})
 
             plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list)  
 
-        # Modify label sizes
         display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
         display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
 
-        # Set plot name
-        plot_title = f"{group} CAPS {task_title}" if task_title else f"{group} CAPS" 
+        plot_title = f"{group} CAPs {task_title}" if task_title else f"{group} CAPs" 
         display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
         # Save plots
         if output_dir:
-            partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_heatmap-regions.png" if scope == "regions" else f"{partial_filename}_heatmap-nodes.png"
+            partial_filename = f"{group}_CAPs_{task_title}" if task_title else f"{group}_CAPs"
+            full_filename = f"{partial_filename.replace(' ','_')}_heatmap-regions.png" if scope == "regions" else f"{partial_filename.replace(' ','_')}_heatmap-nodes.png"
             display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
    
         # Display figures
         if not show_figs: plt.close()
 
-    def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, output_dir: str=None, file_name: str=None) -> dict:
-        """Get CAP metrics
-
-        Creates a single pandas Dataframe containing all participants containing CAP metrics as described in Liu et al., 2018 and Yang et al., 2021, where `temporal fraction` is the proportion of total volumes spent in a single CAP over all volumes in a run,
-        `persistence` is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and `counts` is the frequency of each CAP observed in a run, and `transition frequency` is the number of switches between
-        different CAPs across the entire run.
+    def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, 
+                          metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, 
+                          output_dir: str=None, file_name: str=None) -> dict:
+        """Get CAPs metrics
+
+        Creates a single pandas Dataframe containing all participants containing CAP metrics as described in Liu et al., 2018 and Yang et al., 2021, 
+        where `temporal fraction` is the proportion of total volumes spent in a single CAP over all volumes in a run, `persistence` is the average 
+        time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and `counts` is the frequency 
+        of each CAP observed in a run, and `transition frequency` is the number of switches between different CAPs across the entire run.
 
         Parameters
         ----------
         subject_timeseries: dict or str
             The absolute path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
             the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
             ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
@@ -664,32 +653,27 @@
         tr: float, default=None
             The repetition time. If given, persistence will be calculate as the average uninterrupted time spent in each CAP. If not give, persistence will be calculate
             as the average uninterrupted volumes (TRs) spent in each state.
         runs: int or list[int], default=None
             The run numbers to calculate cap metrics for. If None, cap metrics will be calculated for each run.
         continuous_runs: bool, default=False
             If True, all runs will be treated as a single, uninterrupted run.
-        metrics : str or list[str], default=["temporal fraction", "persistence", "counts", "transition frequency"]
+        metrics: str or list[str], default=["temporal fraction", "persistence", "counts", "transition frequency"]
             The metrics to calculate. Available options include `temporal fraction`, `persistence`, `counts`, and `transition frequency`.
         return_df: str, default=True
             If True, dataframe will be returned.
         output_dir: str, default=None
-            Directory to save dataframe in. If None, dataframe will not be saved.
+            Directory to save dataframe in. Will create the directory if it does not exist. If None, dataframe will not be saved.
         file_name: str, default=None
             Name to save dataframe as if output_dir is not None.
 
         Returns
         -------
         Dictionary containing pandas dataframes - one for each metric requested.
 
-        Raises
-        ------
-        ValueError
-            No valid metrics are detected in `metrics` parameter.
-
         Notes
         -----
         The presence of 0 for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes, indicates that the participant had zero instances of 
         a specific CAP.
 
         References
         -----
@@ -697,14 +681,19 @@
 
         Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. 
         NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
 
         """
         import collections, os, pandas as pd
 
+        if not hasattr(self,"_kmeans"):
+            raise AttributeError("Cannot calculate metrics since `self._kmeans` attribute does not exist. Run `self.get_caps()` first.")
+        
+        if file_name != None and output_dir == None: warnings.warn("`file_name` supplied but no `output_dir` specified. Files will not be saved.")
+
         metrics = [metrics] if isinstance(metrics, str) else metrics
 
         valid_metrics = ["temporal fraction", "persistence", "counts", "transition frequency"]
 
         boolean_list = [element in valid_metrics for element in metrics]
 
         if any(boolean_list):
@@ -742,15 +731,14 @@
                 subject_runs = "Continuous Runs"
                 timeseries = {subject_runs: {}}
                 for curr_run in subject_timeseries[subj_id].keys():
                     timeseries[subject_runs] = np.vstack([timeseries[subject_runs], subject_timeseries[subj_id][curr_run]]) if len(timeseries[subject_runs]) != 0 else subject_timeseries[subj_id][curr_run]
                 timeseries = (timeseries[subject_runs] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon) if self._standardize else timeseries[subject_runs]
                 predicted_subject_timeseries[subj_id].update({subject_runs: self._kmeans[group].predict(timeseries) + 1})
 
-        # Create pd.dataframe
         df_dict = {}
 
         for metric in metrics: 
             if metric in valid_metrics:
                 if metric != "transition frequency":
                     df_dict.update({metric: pd.DataFrame(columns=["Subject_ID", "Group","Run"] + list(cap_names))})
                 else:
@@ -815,30 +803,31 @@
                     if index != 0:
                         # If the subsequent element does not equal the previous element, this is considered a transition
                         if predicted_subject_timeseries[subj_id][curr_run][index-1] != predicted_subject_timeseries[subj_id][curr_run][index]:
                             count +=1
                 df_dict["transition frequency"].loc[len(df_dict["transition frequency"])] = [subj_id, group, curr_run, count]
 
         if output_dir:
+            if not os.path.exists(output_dir): os.makedirs(output_dir)
             for metric in df_dict.keys():
-                filename = file_name + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
+                filename = os.path.splitext(file_name.rstrip())[0].rstrip() + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
                 df_dict[f"{metric}"].to_csv(path_or_buf=os.path.join(output_dir,filename + ".csv"), sep=",", index=False)
 
         if return_df:
             return df_dict
 
     def caps2corr(self, output_dir: str=None, show_figs: bool=True, **kwargs):
-        """ Generate Correlation Matrix
+        """Generate Correlation Matrix
 
         This function produces the correlation matrix of all CAPs. If groups were given when the CAP class was initialized, a correlation matrix will be generated for each group. 
 
         Parameters
         ----------
         output_dir: str, default=None
-            Directory to save plots in. If None, plots will not be saved.
+            Directory to save plots in. Will create the directory if it does not exist. If None, plots will not be saved.
         show_figs: bool, default=True
             Display figures or not to display figures.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
 
             - "dpi": int, default=300
                 Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
@@ -861,16 +850,17 @@
             - "linewidths": float, default=0
                 Padding between each cell in the plot.
             - "cmap": str, default="coolwarm"
                 Color map for the cells in the plot.
         """
         import matplotlib.pyplot as plt, os, pandas as pd
         from seaborn import heatmap
-        
-        # Initialize new grid
+
+        if not hasattr(self,"_caps"):
+            raise AttributeError("Cannot plot caps since `self._caps` attribute does not exist. Run `self.get_caps()` first.")
         
         # Create plot dictionary
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6),
                         fontsize = kwargs["fontsize"] if kwargs and "fontsize" in kwargs.keys() else 14,
                         xticklabels_size = kwargs["xticklabels_size"] if kwargs and "xticklabels_size" in kwargs.keys() else 8,
                         yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
@@ -894,47 +884,46 @@
             df = pd.DataFrame(self.caps[group])
             display = heatmap(df.corr(), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], 
                               cbar_kws={'shrink': plot_dict["shrink"]}, annot=plot_dict["annot"]) 
             # Modify label sizes
             display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
             display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
             # Set plot name
-            plot_title = f"{group} - CAPS Correlation Matrix" 
+            plot_title = f"{group} - CAPs Correlation Matrix" 
             display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
 
             # Display figures
             if not show_figs: plt.close()
             # Save figure
             if output_dir:
+                if not os.path.exists(output_dir): os.makedirs(output_dir)
                 full_filename = f"{group.replace(' ', '_')}_correlation_matrix.png"
                 display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
 
     def caps2surf(self, output_dir: str=None, show_figs: bool = True, fwhm: float=None, 
-                  fslr_density: str="32k", method: str="linear", return_stat_map: bool = False, **kwargs):
-        """Project CAPs back onto atlas used for spatial dimensionality reduction for visualization
+                  fslr_density: str="32k", save_stat_map: bool=False, method: str="linear",  **kwargs):
+        """Project CAPs onto 
         
         Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
         This function uses surfplot for surface plotting.
 
         Parameters
         ----------
         output_dir: str, default=None
-            Directory to save plots in. If None, plots will not be saved.
+            Directory to save plots in. Will create the directory if it does not exist. If None, plots will not be saved. 
         show_figs: bool, default=True
             Display figures or not to display figures.
         fwhm: float, defualt=None
             Strength of spatial smoothing to apply in millimeters.
         fslr_density: str, default="32k"
             Density of the fslr surface when converting from mni 152 space to fslr surface. Options are 
             "32k" or "164k".
         method: str, default="linear"
             Interpolation method to use when converting from mni152 space to fslr surface. Options are "linear"
             or "nearest".
-        return_stat_map: bool, default=FAlse
-            Returns the atlas as a stat map.
         **kwargs : dict
             Additional parameters to pass to modify certain plot parameters. Options include:
 
             - "dpi": int, default=300
                 Dots per inch for the plot.
             - "title_pad": int, default=-3
                 Padding for the plot title.
@@ -958,15 +947,15 @@
                 Number of ticks on the colorbar.
             - "cbar_fontsize": int, default=10
                 Font size for the colorbar labels.
             - "cbar_alpha": float, default=1
                 Transparency level of the colorbar.
             - "size": tuple, default=(500, 400)
                 Size of the plot in pixels.
-            - "layout": str, default="grid";
+            - "layout": str, default="grid"
                 Layout of the plot.
             - "zoom": float, default=1.5
                 Zoom level for the plot.
             - "views": list of str, default=["lateral", "medial"]
                 Views to be displayed in the plot.
             - "brightness": float, default=0.5
                 Brightness level of the plot.
@@ -984,25 +973,31 @@
 
         Notes
         -----
         Assumes that atlas background label is zero and atlas is in MNI space. Also assumes that the indices from the cluster centroids are related
         to the atlas by an offset of one. For instance, index 0 of the cluster centroid vector is the first nonzero label, which is assumed to be at the 
         first index of the array in sorted(np.unique(atlas_fdata)).
 
-        Using fwhm to adjust smooting may help coverage issues.
+        Using fwhm to adjust smoothing may help coverage issues.
 
         """
 
         import nibabel as nib, numpy as np, os
         from nilearn import image
         from nilearn.plotting.cm import _cmap_d 
         from neuromaps.transforms import mni152_to_fslr
         from neuromaps.datasets import fetch_fslr
         from surfplot import Plot
 
+        if not hasattr(self,"_caps"):
+            raise AttributeError("Cannot plot caps since `self._caps` attribute does not exist. Run `self.get_caps()` first.")
+
+        if output_dir:
+            if not os.path.exists(output_dir): os.makedirs(output_dir)
+
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
                          title_pad = kwargs["title_pad"] if kwargs and "title_pad" in kwargs.keys() else -3,
                          cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "cold_hot",
                          cbar_location = kwargs["cbar_location"] if kwargs and "cbar_location" in kwargs.keys() else "bottom",
                          cbar_draw_border = kwargs["cbar_draw_border"] if kwargs and "cbar_draw_border" in kwargs.keys() else False,
                          cbar_aspect = kwargs["cbar_aspect"] if kwargs and "cbar_aspect" in kwargs.keys() else 20,
                          cbar_shrink = kwargs["cbar_shrink"] if kwargs and "cbar_shrink" in kwargs.keys() else 0.2,
@@ -1072,10 +1067,11 @@
                 
                 if show_figs:
                     fig.show()
                 
                 if output_dir:
                     save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}.png"
                     fig.savefig(os.path.join(output_dir, save_name), dpi=plot_dict["dpi"])
-
-        if return_stat_map:
-            return stat_map
+                    # Save stat map
+                    if save_stat_map: 
+                        stat_map_name = save_name.replace(".png", ".nii.gz")
+                        nib.save(stat_map, stat_map_name)
```

### Comparing `neurocaps-0.9.2/neurocaps/analysis/merge.py` & `neurocaps-0.9.3/neurocaps/analysis/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
     Merge subject timeseries dictionaries or pickle files to the first dictionary or pickle file in the list.
     Repetition times from the same subject and run are merged together. The combined dicitonary will only include subjects
     that are present in all dictionaries.
 
     Parameters
     ----------
-
     subject_timeseries_list: list[dict] or list[str]
         The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
         the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
         ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
         must consist of the timeseries associated with that run.
     return_combined_dict: bool, default=True,
         Returns the merged dictionaries if True
@@ -31,15 +30,14 @@
     ------
     AssertionError
         If the length of `subject_timeseries_list` is less than two.
 
     Returns
     -------
     dict
-    
     """
     assert len(subject_timeseries_list) > 1, "Merging cannot be done with less than two dictionaries or files."
 
     if isinstance(subject_timeseries_list[0],dict): subject_timeseries_combined = subject_timeseries_list[0] 
     else: subject_timeseries_combined = _convert_pickle_to_dict(pickle_file=subject_timeseries_list[0])
 
     # Get common subject ids
```

### Comparing `neurocaps-0.9.2/neurocaps/analysis/standardize.py` & `neurocaps-0.9.3/neurocaps/analysis/standardize.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 def standardize(subject_timeseries: Union[dict,str]) -> dict:
     """Standardize subject timeseries 
     
     Standardizes each run independently for all subjects in the subject timeseries.
 
     Parameters
     ----------
-
     subject_timeseries_list: dict or str
         The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
         the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
         ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
         must consist of the timeseries associated with that run.
 
-     Returns
+    Returns
     -------
     dict
     """
 
     if ".pkl" in subject_timeseries:
         with open(subject_timeseries, "rb") as foo:
             subject_timeseries = pickle.load(foo)
```

### Comparing `neurocaps-0.9.2/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.3/neurocaps/extraction/timeseriesextractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,52 +4,52 @@
 
 class TimeseriesExtractor(_TimeseriesExtractorGetter):
     def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
                  parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}, use_confounds: bool=True, confound_names: list[str]=None, 
                  fwhm: float=None, fd_threshold: float=None, n_acompcor_separate: int=None, dummy_scans: int=None):
         """Timeseries Extractor Class
         
-        Initializes a TimeseriesExtractor to prepare for Co-activation Patterns (CAPs) analysis.
+        Initializes the TimeseriesExtractor class to prepare for Co-activation Patterns (CAPs) analysis.
 
         Parameters
         ----------
-        space : str, default="MNI152NLin2009cAsym"
+        space: str, default="MNI152NLin2009cAsym"
             The brain template space data is in. 
-        standardize : bool, default=True
+        standardize: bool, default=True
             Determines whether to standardize the timeseries. Refer to Nilearn's NiftiLabelsMasker for available options. 
-        detrend : bool, default=True
+        detrend: bool, default=True
             Detrends timeseries during extraction.
-        low_pass : bool, default=None
+        low_pass: bool, default=None
             Signals above cutoff frequency will be filtered out.
-        high_pass : float, default=None
+        high_pass: float, default=None
             Signals below cutoff frequency will be filtered out.
-        parcel_approach : dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
+        parcel_approach: dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
             Approach to use to parcellate bold images. Should be in the form of a nested dictionary where the first key is the atlas.
             Currently only "Schaefer", "AAL", and "Custom" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois", "yeo_networks", and "resolution_mm".
             Please refer to the documentation for Nilearn's `datasets.fetch_atlas_schaefer_2018` for valid inputs. For the subdictionary for "AAL" only "version"
             is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs. As of version 0.8.9, you can replace "Schaefer"
             and "AAL" with "Custom". At minimum, if "Custom" is specified, a subkey, called "maps" specifying the directory location of the parcellation as a Nifti (e.g .nii or .nii.gz)
             - {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}.
-        use_confounds : bool, default=True
+        use_confounds: bool, default=True
             To use confounds when extracting timeseries.
-        confound_names : List[str], default=None
+        confound_names: List[str], default=None
             Names of confounds to use in confound files. If None, default confounds are used.
-        fwhm : float, default=None
+        fwhm: float, default=None
             Parameter for spatial smoothing.
-        fd_threshold : float, default=None
+        fd_threshold: float, default=None
             Threshold criteria to remove frames after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
             in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
-        n_acompcor_separate : int, default = None
-            The number of seperate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
+        n_acompcor_separate: int, default = None
+            The number of separate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
             then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
             used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
             masks. To use the acompcor components derived from the combined masks (WM & CSF) leave this parameter as 'None' and list the specific acompcors of interest in the 
             `confound_names` parameter.
-        dummy_scans : float, default=None
-            Removes the first `n` number of volumes before extracting timeseries.
+        dummy_scans: float, default=None
+            Removes the first `n` number of volumes before extracting the timeseries.
         
         Notes for `confounds_names`
         --------------------------
         For the `confound_names` parameter, an asterisk ("*") can be used to find the name of confounds that starts with the term preceding the asterisk.
         For instance, "cosine*" will find all confound names in the confound files starting with "cosine".
 
         Notes for `parcel_approach`
@@ -92,29 +92,29 @@
                  exclude_niftis: list[str]=None) -> None: 
         """Get Bold Data
 
         Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
 
         Parameters
         ----------
-        bids_dir : str
+        bids_dir: str
             Path to a BIDS compliant directory. 
-        task : str, default="rest"
-            Task name.
-        session : int, default=None
+        task: str
+            Name of task to process.
+        session: int, default=None
             Session to extract timeseries from. Only a single session can be extracted at a time. 
-        runs : list[int], default=None
+        runs: list[int], default=None
             Run number to extract timeseries data from. Extracts all runs if unspecified.
-        condition : str, default=None
+        condition: str, default=None
             Specific condition in the task to extract from. Only a single condition can be extracted at a time.
-        tr : int or float, default=None
-            Repetition time.
-        run_subjects : list[str], default=None
+        tr: int or float, default=None
+            Repetition time for task.
+        run_subjects: list[str], default=None
             List of subject IDs to process. Processes all subjects if None.
-        exclude_subjects : list[str], default=None
+        exclude_subjects: list[str], default=None
             List of subject IDs to exclude.  
         pipeline_name: str, default=None
             The name of the pipeline folder in the derivatives folder containing the preprocessed data. If None, BIDSLayout will use the name of dset_dir with derivatives=True. This parameter
             should be used if their are multiple pipelines in the derivatives folder.
         n_cores: bool or int, default=None
             The number of CPU cores to use for multiprocessing. If true, all available cores will be used.
         verbose: bool, default=True
@@ -245,15 +245,15 @@
                 warnings.warn(f"Subject: {subj_id} is missing mask file but timeseries extraction will continue.")
                 
             if self._signal_clean_info["use_confounds"]:
                 if len(confound_files) == 0:
                     warnings.warn(f"Skipping subject: {subj_id} due to missing confound files.")
                     continue
                 if len(confound_metadata_files) == 0 and self._signal_clean_info["n_acompcor_separate"]:
-                    warnings.warn(f"Skipping subject: {subj_id} due to missing confound metadata to locate the first six components of the white-matter and cerobrospinal fluid masks seperately.")
+                    warnings.warn(f"Skipping subject: {subj_id} due to missing confound metadata to locate the first six components of the white-matter and cerobrospinal fluid masks separately.")
                     continue
             
             if self._task_info["condition"] and len(event_files) == 0:
                 warnings.warn(f"Skipping subject: {subj_id} due to having no event files.")
                 continue
                 
             if len(check_runs) != 0:
@@ -286,33 +286,38 @@
             # Get repetition time for the subject
             tr = self._task_info["tr"] if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
 
             # Store subject specific information
             self._subject_info[subj_id] = {"nifti_files": nifti_files, "event_files": event_files, "confound_files": confound_files, "confound_metadata_files": confound_metadata_files, "mask_files": mask_files,
                                            "tr": tr, "run_list": run_list}
 
-    def timeseries_to_pickle(self, output_dir: str, file_name: str):
+    def timeseries_to_pickle(self, output_dir: str, file_name: str=None):
         """Save Bold Data
 
-        Saves the timeseries dictionary as a pickle file where columns are the subject ID and indices are the runs. Each cell contains the timeseries array.
+        Saves the timeseries dictionary obtained from running `get_bold()` as a pickle file.
 
         Parameters
         ----------
-        output_dir : str
-            Directory to save the file to.
-        file_name : str
-            Name of the file without the "pkl" extension.
+        output_dir: str
+            Directory to save the file to. Will create the directory if it does not exist.
+        file_name: str, default=None
+            Name of the file without or without the "pkl" extension.
         """
         import pickle
 
+        if not hasattr(self, "_subject_timeseries"):
+            raise AttributeError("Cannot save pickle file since `self._subject_timeseries` does not exist, either run `self.get_bold()` or assign a valid timeseries dictionary to `self.subject_timeseries`.")
+
         if output_dir:
-            if not os.path.exists(output_dir):
-                os.makedirs(output_dir)
+            if not os.path.exists(output_dir): os.makedirs(output_dir)
         
-        with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
+        if file_name == None: save_file_name = "subject_timeseries.pkl"
+        else: save_file_name = f"{os.path.splitext(file_name.rstrip())[0].rstrip()}.pkl" 
+
+        with open(os.path.join(output_dir,save_file_name), "wb") as f:
             pickle.dump(self._subject_timeseries,f)
 
     def visualize_bold(self, subj_id: Union[int,str], run: int, roi_indx: Union[int, list[int]]=None, region: str=None, show_figs: bool=True, output_dir: str=None, file_name: str=None, **kwargs):
         """Plot Bold Data
 
         Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
 
@@ -323,36 +328,28 @@
         run: int
             The run to plot.
         roi_indx: int or list[int], default=None
             The indices of the Schaefer nodes to plot. See self.node_indices for valid node names and indices.
         region: str, default=None
             The region of the parcellation to plot. If not None, all nodes in the specified region will be averaged then plotted. See `regions` in self.parcel_approach 
             for valid regions names.
-        show_figs: bool, defaults=True
+        show_figs: bool, default=True
             Whether to show figires or not to show figures
-        output_dir : str
-            Directory to save the file to.
-        file_name : str
-            Name of the file with the extension to signify the file type.
+        output_dir: str, default=None
+            Directory to save the file to. Will create the directory if it does not exist.
+        file_name: str, default=None
+            Name of the file without the extension.
         **kwargs: dict
             Keyword arguments used when saving figures. Valid keywords include:
         
             - "dpi": int, default=300
                 Dots per inch for the figure. Default is 300 if `output_dir` is provided and `dpi` is not specified.
             - "figsize": tuple, default=(11, 5)
                 Size of the figure in inches. Default is (11, 5) if "figsize" is not specified.
 
-
-        Raises
-        ------
-        ValueError
-            If both `roi_indx` and `region` are specified.
-        AssertionError
-            If `file_name` does not contain an extension to signify the file type.
-
         Notes
         -----
         If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
         the zero index should correspond the first id that is not zero.
 
         Custom Key Structure:
         - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
@@ -370,23 +367,27 @@
                                                   "rh": [3,4]},
                                          "Hippocampus": {"lh": [2],
                                                          "rh": [5]}}}}
         """
     
         import matplotlib.pyplot as plt, numpy as np
 
+        if not hasattr(self, "_subject_timeseries"):
+            raise AttributeError("Cannot plot bold data since `self._subject_timeseries` does not exist, either run `self.get_bold()` or assign a valid timeseries structure to self.subject_timeseries.")
+
         if isinstance(subj_id,int): subj_id = str(subj_id)
 
         if roi_indx !=None and region != None:
             raise ValueError("`roi_indx` and `region` can not be used simultaneously.")
         
+        if file_name != None and output_dir == None: warnings.warn("`file_name` supplied but no `output_dir` specified. Files will not be saved.")
+        
         if output_dir:
             if not os.path.exists(output_dir):
                 os.makedirs(output_dir)
-            assert "." in file_name, "`file_name` must be specified if `output_dir` is specified and it must contain an extension to signify the file type."
 
         plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
                          figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (11, 5))
         
         if kwargs:
             invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
             if len(invalid_kwargs.keys()) > 0:
@@ -415,33 +416,29 @@
                     raise ValueError("All elements in `roi_indx` need to be all strings or all integers.")
                 
         elif region:
             if "Custom" in self.parcel_approach.keys():
                 if "regions" not in self.parcel_approach["Custom"].keys():
                     _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
                 else:
-                    plot_indxs =  np.array(self.parcel_approach["Custom"]["regions"][region]["lh"] + self.parcel_approach["Custom"]["regions"][region]["rh"])
+                    plot_indxs =  np.array(self._parcel_approach["Custom"]["regions"][region]["lh"] + self._parcel_approach["Custom"]["regions"][region]["rh"])
             else:
                 plot_indxs = np.array([index for index, label in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in label])
         
         plt.figure(figsize=plot_dict["figsize"])
 
         if roi_indx or roi_indx == 0: 
             plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs])
         elif region:  
             plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), np.mean(self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs], axis=1))
             plt.title(region)
         plt.xlabel("TR")
 
         if output_dir:
+            if not os.path.exists(output_dir): os.makedirs(output_dir)
+            file_name = f"{os.path.splitext(file_name.rstrip())[0].rstrip()}.png" if file_name else f'subject-{subj_id}_run-{run}_timeseries.png'
             plt.savefig(os.path.join(output_dir,file_name), dpi=plot_dict["dpi"])
 
         if show_figs == False:
             plt.close()
         else:
-            plt.show()
-
-
-
-        
-        
-        
+            plt.show()
```

### Comparing `neurocaps-0.9.2/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.3/neurocaps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurocaps
-Version: 0.9.2
+Version: 0.9.3
 Summary: Co-activation patterns Python package
 Author-email: Donisha Smith <donishasmith@outlook.com>
 Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
 Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -22,15 +22,15 @@
 License-File: LICENSE.md
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: kneed
 Requires-Dist: nibabel
-Requires-Dist: nilearn==0.10.2
+Requires-Dist: nilearn!=0.10.3,>=0.10.1
 Requires-Dist: surfplot
 Requires-Dist: neuromaps
 Requires-Dist: pybids; platform_system != "Windows"
 
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
@@ -65,24 +65,24 @@
 pip install -e .
 
 ```
 
 # Usage
 **This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
 
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes have a left and right version (bilateral nodes)**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
 
 If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
 
 Custom Key Structure:
 - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
 - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
 Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
 visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
         
 Example 
 The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
 
 ```Python
 parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
                              "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
@@ -93,27 +93,28 @@
  ```
 
 **Main features for `TimeseriesExtractor` includes:**
 
 - Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
 - Saving the nested dictionary containing timeseries as a pickle file.
 - Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+- Ability to use parallel processing by specifying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
 
 **Main features for `CAP` includes:**
 
 - Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
 - Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
-- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
-- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available kwargs arguments and parameters to modify plots.
+- Visualizing the CAPs identified as an outer product or heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `caps2plot()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
+- Visualizing CAPs as surface plots by converting the atlas used for parcellation to a stat map that gets projected onto a surface plot. Please refer to the docstring for the `caps2surf()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
+- Creating a correlation matrix from CAPs. Please refer to the docstring for the `caps2corr()` method in the `CAP` class to see the list of available `**kwargs` arguments and parameters to modify plots.
 - Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
 different CAPs across the entire run.
 
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+**Additionally, the `neurocaps.analysis` submodule contains two additional functions**:
+- The `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
 
 Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
 
 Quick code example:
 
 ```python
 # Examples use randomized data
@@ -155,25 +156,25 @@
 cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
                     n_clusters=6)
 
 cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
                       standardize = True)
 
 # Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+cap_analysis.caps2plot(visual_scope="regions", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3, sharey=True, 
                             subplots=True)
 
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+cap_analysis.caps2plot(visual_scope="nodes", plot_options="outer product", 
                             task_title="- Positive Valence", ncol=3,sharey=True, 
                             subplots=True, xlabel_rotation=90, tight_layout=False, 
                             hspace = 0.4)
 
 ```
-**Graph Outputs:**
+**Plot Outputs:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
 
 ```python
 
 # Get CAP metrics
 outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
@@ -194,25 +195,27 @@
 | 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
 | 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
 | 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
 | 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
 | 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
 
 ```python
-# Create surface plots of CAPs
+# Create surface plots of CAPs; there will be as many plots as CAPs
 # If you experience coverage issues, usually smoothing helps to mitigate these issues
 cap_analysis.caps2surf(fwhm=2)
 ```
+**Plot Output:**
 ![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
 
 ```python
 # Create correlation matrix
 cap_analysis.caps2corr(annot=True)
 ```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/83d20109-432f-41ca-8a8f-999fb6482e39)
+**Plot Output:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/81620b36-55b0-4c83-be51-95d3f5280fa9)
 
 # Testing 
 This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slightly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
 
 Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
```

### Comparing `neurocaps-0.9.2/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.3/neurocaps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.2/pyproject.toml` & `neurocaps-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6e65 7572 6f63 6170 7322 0d0a 7665   "neurocaps"..ve
-00000080: 7273 696f 6e20 3d20 2230 2e39 2e32 220d  rsion = "0.9.2".
+00000080: 7273 696f 6e20 3d20 2230 2e39 2e33 220d  rsion = "0.9.3".
 00000090: 0a61 7574 686f 7273 203d 205b 7b6e 616d  .authors = [{nam
 000000a0: 6520 3d20 2244 6f6e 6973 6861 2053 6d69  e = "Donisha Smi
 000000b0: 7468 222c 2065 6d61 696c 203d 2022 646f  th", email = "do
 000000c0: 6e69 7368 6173 6d69 7468 406f 7574 6c6f  nishasmith@outlo
 000000d0: 6f6b 2e63 6f6d 227d 5d0d 0a64 6573 6372  ok.com"}]..descr
 000000e0: 6970 7469 6f6e 203d 2022 436f 2d61 6374  iption = "Co-act
 000000f0: 6976 6174 696f 6e20 7061 7474 6572 6e73  ivation patterns
@@ -70,25 +70,25 @@
 00000450: 746c 6962 222c 0d0a 2020 2020 2020 2020  tlib",..        
 00000460: 2020 2020 2020 2020 2273 6561 626f 726e          "seaborn
 00000470: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
 00000480: 2020 2020 226b 6e65 6564 222c 0d0a 2020      "kneed",..  
 00000490: 2020 2020 2020 2020 2020 2020 2020 226e                "n
 000004a0: 6962 6162 656c 222c 0d0a 2020 2020 2020  ibabel",..      
 000004b0: 2020 2020 2020 2020 2020 226e 696c 6561            "nilea
-000004c0: 726e 203d 3d20 302e 3130 2e32 222c 0d0a  rn == 0.10.2",..
-000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004e0: 2273 7572 6670 6c6f 7422 2c0d 0a20 2020  "surfplot",..   
-000004f0: 2020 2020 2020 2020 2020 2020 2022 6e65               "ne
-00000500: 7572 6f6d 6170 7322 2c0d 0a20 2020 2020  uromaps",..     
-00000510: 2020 2020 2020 2020 2020 2022 7079 6269             "pybi
-00000520: 6473 3b20 706c 6174 666f 726d 5f73 7973  ds; platform_sys
-00000530: 7465 6d20 213d 2027 5769 6e64 6f77 7327  tem != 'Windows'
-00000540: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00000550: 2020 205d 0d0a 0d0a 5b70 726f 6a65 6374     ]....[project
-00000560: 2e75 726c 735d 0d0a 486f 6d65 7061 6765  .urls]..Homepage
-00000570: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-00000580: 7562 2e63 6f6d 2f64 6f6e 6973 6861 6473  ub.com/donishads
-00000590: 6d69 7468 2f6e 6575 726f 6361 7073 2220  mith/neurocaps" 
-000005a0: 200d 0a0d 0a5b 746f 6f6c 2e64 6973 7475   ....[tool.distu
-000005b0: 7469 6c73 2e62 6469 7374 5f77 6865 656c  tils.bdist_wheel
-000005c0: 5d0d 0a75 6e69 7665 7273 616c 203d 2074  ]..universal = t
-000005d0: 7275 65                                  rue
+000004c0: 726e 3e3d 302e 3130 2e31 2c20 213d 302e  rn>=0.10.1, !=0.
+000004d0: 3130 2e33 222c 0d0a 2020 2020 2020 2020  10.3",..        
+000004e0: 2020 2020 2020 2020 2273 7572 6670 6c6f          "surfplo
+000004f0: 7422 2c0d 0a20 2020 2020 2020 2020 2020  t",..           
+00000500: 2020 2020 2022 6e65 7572 6f6d 6170 7322       "neuromaps"
+00000510: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000520: 2020 2022 7079 6269 6473 3b20 706c 6174     "pybids; plat
+00000530: 666f 726d 5f73 7973 7465 6d20 213d 2027  form_system != '
+00000540: 5769 6e64 6f77 7327 220d 0a20 2020 2020  Windows'"..     
+00000550: 2020 2020 2020 2020 2020 205d 0d0a 0d0a             ]....
+00000560: 5b70 726f 6a65 6374 2e75 726c 735d 0d0a  [project.urls]..
+00000570: 486f 6d65 7061 6765 203d 2022 6874 7470  Homepage = "http
+00000580: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00000590: 6f6e 6973 6861 6473 6d69 7468 2f6e 6575  onishadsmith/neu
+000005a0: 726f 6361 7073 2220 200d 0a0d 0a5b 746f  rocaps"  ....[to
+000005b0: 6f6c 2e64 6973 7475 7469 6c73 2e62 6469  ol.distutils.bdi
+000005c0: 7374 5f77 6865 656c 5d0d 0a75 6e69 7665  st_wheel]..unive
+000005d0: 7273 616c 203d 2074 7275 65              rsal = true
```

### Comparing `neurocaps-0.9.2/tests/test_CAP.py` & `neurocaps-0.9.3/tests/test_CAP.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.2/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.3/tests/test_TimeseriesExtractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,35 @@
     extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
     
     print(extractor.subject_timeseries, flush=True)
 
     assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 426
     assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 39
 
+def test_TimeseriesExtractor_dummy():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds, dummy_scans=5)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
+    
+    print(extractor.subject_timeseries, flush=True)
+
+    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 426
+    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 35
+
 def test_TimeseriesExtractor_check_exclusion():
     dir = os.path.dirname(__file__)
 
     confounds=["Cosine*", "aComp*", "Rot*"]
 
     parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
```

### Comparing `neurocaps-0.9.2/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.3/tests/test_TimeseriesExtractor_additional.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.2/tests/test_merge_dicts.py` & `neurocaps-0.9.3/tests/test_merge_dicts.py`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.2/tests/test_standardize.py` & `neurocaps-0.9.3/tests/test_standardize.py`

 * *Files identical despite different names*

