# Comparing `tmp/linkinglines-2.1.1.tar.gz` & `tmp/linkinglines-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkinglines-2.1.1.tar", max compression
+gzip compressed data, was "linkinglines-2.1.2.tar", max compression
```

## Comparing `linkinglines-2.1.1.tar` & `linkinglines-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       88 2023-10-27 17:49:22.627589 linkinglines-2.1.1/AUTHORS
--rw-r--r--   0        0        0     1069 2023-10-27 17:49:22.627589 linkinglines-2.1.1/LICENSE
--rw-r--r--   0        0        0     4713 2024-03-14 00:27:03.195267 linkinglines-2.1.1/README.md
--rw-r--r--   0        0        0     1439 2024-03-19 18:07:07.424547 linkinglines-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4085 2024-03-18 02:36:06.359435 linkinglines-2.1.1/src/linkinglines/ClusterLines.py
--rw-r--r--   0        0        0    11947 2024-03-19 18:06:25.224385 linkinglines-2.1.1/src/linkinglines/DilationCalculations.py
--rw-r--r--   0        0        0    43937 2024-03-19 18:06:25.224385 linkinglines-2.1.1/src/linkinglines/ExamineClusters.py
--rw-r--r--   0        0        0    17421 2024-03-19 18:06:25.224385 linkinglines-2.1.1/src/linkinglines/FitRadialCenters.py
--rw-r--r--   0        0        0    13613 2024-03-19 18:06:22.288373 linkinglines-2.1.1/src/linkinglines/FitRectangle.py
--rw-r--r--   0        0        0    10617 2024-03-19 18:06:25.224385 linkinglines-2.1.1/src/linkinglines/HT.py
--rw-r--r--   0        0        0    63715 2024-03-19 18:06:25.224385 linkinglines-2.1.1/src/linkinglines/PlotUtils.py
--rw-r--r--   0        0        0    18809 2024-03-19 18:06:25.200384 linkinglines-2.1.1/src/linkinglines/PrePostProcess.py
--rw-r--r--   0        0        0    12469 2024-03-19 18:06:25.216385 linkinglines-2.1.1/src/linkinglines/SyntheticLines.py
--rw-r--r--   0        0        0      449 2024-03-19 18:06:49.684479 linkinglines-2.1.1/src/linkinglines/__init__.py
--rw-r--r--   0        0        0     1730 2024-03-19 18:06:25.224385 linkinglines-2.1.1/src/linkinglines/__main__.py
--rw-r--r--   0        0        0     5899 1970-01-01 00:00:00.000000 linkinglines-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-13 19:03:53.385841 linkinglines-2.1.2/AUTHORS
+-rw-r--r--   0        0        0     1069 2023-10-27 17:49:22.627589 linkinglines-2.1.2/LICENSE
+-rw-r--r--   0        0        0     4256 2024-05-17 00:28:20.080050 linkinglines-2.1.2/README.md
+-rw-r--r--   0        0        0     1478 2024-05-26 21:05:58.642639 linkinglines-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4085 2024-05-13 19:03:53.417841 linkinglines-2.1.2/src/linkinglines/ClusterLines.py
+-rw-r--r--   0        0        0    11947 2024-05-13 19:03:53.417841 linkinglines-2.1.2/src/linkinglines/DilationCalculations.py
+-rw-r--r--   0        0        0    43937 2024-05-13 19:03:53.417841 linkinglines-2.1.2/src/linkinglines/ExamineClusters.py
+-rw-r--r--   0        0        0    17421 2024-05-13 19:03:53.421841 linkinglines-2.1.2/src/linkinglines/FitRadialCenters.py
+-rw-r--r--   0        0        0    13613 2024-05-13 19:03:53.421841 linkinglines-2.1.2/src/linkinglines/FitRectangle.py
+-rw-r--r--   0        0        0    10617 2024-05-13 19:03:53.421841 linkinglines-2.1.2/src/linkinglines/HT.py
+-rw-r--r--   0        0        0    63715 2024-05-13 19:03:53.421841 linkinglines-2.1.2/src/linkinglines/PlotUtils.py
+-rw-r--r--   0        0        0    18805 2024-05-13 19:24:13.996314 linkinglines-2.1.2/src/linkinglines/PrePostProcess.py
+-rw-r--r--   0        0        0    12469 2024-05-13 19:03:53.421841 linkinglines-2.1.2/src/linkinglines/SyntheticLines.py
+-rw-r--r--   0        0        0      449 2024-05-26 21:05:58.662639 linkinglines-2.1.2/src/linkinglines/__init__.py
+-rw-r--r--   0        0        0     1730 2024-05-13 19:03:53.421841 linkinglines-2.1.2/src/linkinglines/__main__.py
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 linkinglines-2.1.2/PKG-INFO
```

### Comparing `linkinglines-2.1.1/LICENSE` & `linkinglines-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/README.md` & `linkinglines-2.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 # Welcome to LinkingLines!
  [![status](https://joss.theoj.org/papers/64eeef828a1100bfba74052d89314758/status.svg)](https://joss.theoj.org/papers/64eeef828a1100bfba74052d89314758) [![DOI](https://zenodo.org/badge/272334230.svg)](https://zenodo.org/badge/latestdoi/272334230) [![PyPI](https://img.shields.io/pypi/v/LinkingLines.svg)](https://pypi.org/project/LinkingLines/) [![ReadtheDocs](https://readthedocs.org/projects/linkinglines/badge/)](https://linkinglines.readthedocs.io/) [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Read the Full documentation on [ReadtheDocs!](https://linkinglines.readthedocs.io/en/latest/)
 
 ## 1. Introduction
 Welcome to the documentation for our Python module that performs the Hough
-Transform on line data from a CSV, clusters it using Agglomerative Clustering,
-and provides functionality to export the results into a CSV file.
+Transform on lines from geospatial data, clusters it using Agglomerative Clustering.
 This module also includes custom plotting scripts and feature extraction
 methods to help you analyze and visualize your data effectively.
 
 This code was used to create the results published in
 [Kubo Hutchison et al., 2023](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022GC010842).
 Initially, it was designed to link together mapped dike segments in Cartesian space
 to find their true lengths. This code can be applied to any linear features including
 roads, fractures, and other types of linear data.
 
 - **Data Clustering**: Apply Agglomerative Clustering to group similar data points, this
-can be used for data reduction, analysis, and mapping .
+can be used for data reduction, analysis, and mapping.
 
 - **Data Visualization**: Custom plotting scripts help you visualize and analyze
 your data, making it easier to identify patterns and anomalies.
 
 - **Feature Extraction**: Extract meaningful features from clustered data to
 perform further analysis, such as linear or radial type features.
 
@@ -53,61 +52,56 @@
 dikeset, Z=ll.AggCluster(data)
 lines,evaluation=examineCluster(data)
 fig,ax=DotsLines(lines, ColorBy='AvgTheta')
 
 ```
 
 We have three examples:
-1. Indepth tutorial with hough transform, clustering, and feature extraction using Spanish Peaks Data CSV file.
+1. In-depth tutorial with Hough transform, clustering, and feature extraction using Spanish Peaks Data CSV file.
 2. Hough Transform and feature extraction on Venus lineament data shape file.
-3. Hough transform on fracture data geoJSON.
+3. Hough Transform on fracture data geoJSON.
 
-Data from: 
+Data from:
 1. https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022GC010842
 2. https://pubs.usgs.gov/sim/3121/
 3. https://doi.org/10.5281/zenodo.7919843
 
-You are now ready to utilize the power of Hough Line Transform, Agglomerative Clustering, and custom plotting in your data analysis projects. If you have any questions or need further assistance, please refer to the detailed documentation or contact our support team.
-
 
 ## 4. Contributing Guidelines
-Thank you for your interest in contributing to `linkinglines`. Please feel free to open up issues with bugs or requested features. Any contributions you make will benefit everybody else and are greatly appreciated.
 
-We recommend using a virutal environment to manage packages `virtualenv`, see [here](https://virtualenv.pypa.io/en/latest/). 
+If you find bugs or issues please open up an [issues](). We also welcome requests for additional features.
 
-```
-# Install virtualenv if you haven't already
-pip install virtualenv
+If you would like to contribute code please do so in a separate branch and open up an issue describing your contribution.
 
-# Navigate to the project directory
-cd path/to/LinkingLines
+```
+git clone git@github.com:USER/LinkingLines.git
+git checkout my-development-branch
+```
 
-# Create a virtual environment
-virtualenv venv
+We recommend using a virtual environment to manage packages. We use `poetry` to manage dependencies and building.
+See more about [poetry](https://python-poetry.org/).
 
-# Activate the virtual environment
-# On Windows
-venv\Scripts\activate
-# On Unix or MacOS
-source venv/bin/activate
 
-# Install dependencies
-pip install -r requirements.txt
 ```
+pipx install poetry # you may need to install pipx first
 
-If you would like to contribute code please do so in a seperate branch and open up an issue describing your contribution.
+cd linkinglines # go to the repo
+
+poetry install --with test,dev # install in editable mode
+
+# add your code
+
+poetry run pytest  # test code locally
 
 ```
-git clone git@github.com:aikubo/LinkingLines.git
-git checkout my-development-branch
-```
+
 
 Before submitting your pull request please verify the following:
 
 1. Code is documented in [NumPy Docstring Style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html)
-2. Code is tested and passes test 
-    - To run the tests please go to "/tests" and run `pytest`
+2. Code is tested and passes test
+    - To run the tests please go to "/tests" and run `poetry run pytest` or `pytest`
     - Add your test code to any file with the name `test`
     - More here on [pytest and testing practices](https://docs.pytest.org/en/8.0.x/)
-3. Open an issue and pull request 
-
-After your pull request the code will be reviewed by maintainers. After the sucessful merge the documentation will be regenerated.
+3. Open an issue and pull request
+4. After your pull request the code will be reviewed by maintainer (namely @aikubo).
+5. After passing review and automated tests it will be added to the next release and published to pypi.
```

### Comparing `linkinglines-2.1.1/pyproject.toml` & `linkinglines-2.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkinglines"
-version = "2.1.1"
+version = "2.1.2"
 description = "Process linear geospatial data and link them using the Hough Transform and Agglomerative Clustering"
 authors = ["aikubo <alli.i.kubo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/aikubo/LinkingLines"
 repository = "https://github.com/aikubo/LinkingLines"
 documentation = "https://linkinglines.readthedocs.io/en/latest/"
@@ -38,14 +38,16 @@
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.2.6"
 nbsphinx = "^0.9.3"
 jupyterlab = "^4.1.5"
+rtds-action = "^1.1.0"
+pandoc = "^2.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 pytest-datafiles = "^3.0.0"
 pytest-datadir = "^1.5.0"
 
 [tool.poetry_bumpversion.file."src/linkinglines/__init__.py"]
```

### Comparing `linkinglines-2.1.1/src/linkinglines/ClusterLines.py` & `linkinglines-2.1.2/src/linkinglines/ClusterLines.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/DilationCalculations.py` & `linkinglines-2.1.2/src/linkinglines/DilationCalculations.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/ExamineClusters.py` & `linkinglines-2.1.2/src/linkinglines/ExamineClusters.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/FitRadialCenters.py` & `linkinglines-2.1.2/src/linkinglines/FitRadialCenters.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/FitRectangle.py` & `linkinglines-2.1.2/src/linkinglines/FitRectangle.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/HT.py` & `linkinglines-2.1.2/src/linkinglines/HT.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/PlotUtils.py` & `linkinglines-2.1.2/src/linkinglines/PlotUtils.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/PrePostProcess.py` & `linkinglines-2.1.2/src/linkinglines/PrePostProcess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # LinkingLines Package
  # Written by aikubo
- 
+
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Thu Jul  1 11:04:53 2021
 
 @author: akh
 
@@ -64,28 +64,30 @@
     if not os.path.exists(name):
         raise ValueError("Invalid path")
     # if file is not .csv, .txt, or .shp, return error
     valid_extensions = ['.csv', '.txt', '.shp', '.geojson', '.json']
 
     if not any(name.endswith(ext) for ext in valid_extensions):
         raise ValueError("Invalid file type")
-    
+
     # identify the type of file
-    # read in .csv 
+    # read in .csv
     if name.endswith('.csv'):
         data=pd.read_csv(name)
     elif name.endswith('.txt'):
         data=pd.read_csv(name, delimiter='\t')
     else:
         data=geopandas.read_file(name)
         data=data.to_wkt()
-    
+
+    if 'Xstart' not in data.columns:
+        data = WKTtoArray(data)
+
     # if preprocess is True, preprocess the data
     if preprocess:
-        data = WKTtoArray(data)
         data = preProcess(data)
 
     return data
 
 
 def midPoint(df):
     """
@@ -185,15 +187,15 @@
 
     """
     if not isinstance(df, pd.DataFrame):
         raise ValueError("Input 'data' must be a pandas DataFrame.")
 
     if len(df) < 1:
         raise ValueError("DataFrame is empty")
-    
+
     #     # if neither is in columns raise value error
     if not ("WKT" in df.columns ):
         if not ("geometry" in df.columns):
          raise ValueError("No geometry present")
 
     xstart=[]
     ystart=[]
@@ -201,15 +203,15 @@
     xend=[]
     yend=[]
     drop=[]
 
     if plot:
         fig,ax=plt.subplots()
 
-    # check for either "WKT" or "geometry" columns 
+    # check for either "WKT" or "geometry" columns
     if "geometry" in df.columns:
         tag = "geometry"
     else:
         tag = "WKT"
 
     for i in range(len(df)):
         temp=df[tag].iloc[i]
@@ -217,27 +219,27 @@
         # Using regex to find all numbers in the string
         temp = re.findall(r"[-+]?\d*\.\d+|\d+", temp)
 
 
         if len(temp)<1:
             drop.append(i)
             continue
-       
+
         if "Z" in t1:
             tempx=np.array(temp[::3]).astype(float)
             tempy=np.array(temp[1::3]).astype(float)
         else:
             tempx=np.array(temp[::2]).astype(float)
             tempy=np.array(temp[1::2]).astype(float)
 
         if np.unique(tempx).shape[0]==1 or np.unique(tempy).shape[0]==1:
             drop.append(i)
             continue
 
-    
+
         slope, intercept, r_value, p_value, std_err = stats.linregress(tempx, tempy)
 
         #for x,y in zip(tempx, tempy):
         if any(np.isnan( [slope, intercept])):
             drop.append(i)
             continue
 
@@ -495,15 +497,15 @@
         2. Transform Xstart, so Xstart < Xend
         3. calculate segment lengths
         4. assign unique hash IDs
         5. calculate midpoints
         6. calculate Hough Transform attributes (theta, rho, xc, yc)
         7. calculate perpendicular offset distances
         8. assign the processing date
-        9. remove duplicate entries and report any found duplicates    
+        9. remove duplicate entries and report any found duplicates
 
     Parameters
     ----------
     data : pandas.DataFrame
         The input dataframe containing line data.
 
     Returns
@@ -513,14 +515,15 @@
     """
     df = data.copy()
 
     # Convert WKT column to array format if present
     if "WKT" in df.columns:
         df = WKTtoArray(df)
 
+
     # Transform 'Xstart', calculate segment lengths, and assign unique hash IDs
     df = transformXstart(df)
     df = segLength(df)
     df = giveHashID(df)
 
     # Calculate midpoints
     df = midPoint(df)
@@ -659,26 +662,26 @@
     myProj : str, optional
         The projection of the dataframe, if applicable. Default is None.
 
     Returns
     -------
     pandas.DataFrame
         The input dataframe.
-    """    
+    """
    # if ends with .csv or .txt, write as csv
     if name.endswith('.csv') or name.endswith('.txt'):
         df = writeToWKT(df, name, myProj=myProj)
     # if ends with .shp, write as shapefile
-    else: 
+    else:
         if name.endswith('.shp'):
             driver = 'ESRI Shapefile'
         elif name.endswith('.geojson') or name.endswith('.json'):
             driver = 'GeoJSON'
         elif name.endswith('.gpkg'):
             driver = 'GPKG'
         else:
             driver = 'GeoJSON'
-        
+
         df = writetoGeoData(df, name, driver, myProj=myProj)
 
 
     return df
```

### Comparing `linkinglines-2.1.1/src/linkinglines/SyntheticLines.py` & `linkinglines-2.1.2/src/linkinglines/SyntheticLines.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/src/linkinglines/__main__.py` & `linkinglines-2.1.2/src/linkinglines/__main__.py`

 * *Files identical despite different names*

### Comparing `linkinglines-2.1.1/PKG-INFO` & `linkinglines-2.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkinglines
-Version: 2.1.1
+Version: 2.1.2
 Summary: Process linear geospatial data and link them using the Hough Transform and Agglomerative Clustering
 Home-page: https://github.com/aikubo/LinkingLines
 License: MIT
 Keywords: geospatial,houghtransform,clustering
 Author: aikubo
 Author-email: alli.i.kubo@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -30,27 +30,26 @@
 # Welcome to LinkingLines!
  [![status](https://joss.theoj.org/papers/64eeef828a1100bfba74052d89314758/status.svg)](https://joss.theoj.org/papers/64eeef828a1100bfba74052d89314758) [![DOI](https://zenodo.org/badge/272334230.svg)](https://zenodo.org/badge/latestdoi/272334230) [![PyPI](https://img.shields.io/pypi/v/LinkingLines.svg)](https://pypi.org/project/LinkingLines/) [![ReadtheDocs](https://readthedocs.org/projects/linkinglines/badge/)](https://linkinglines.readthedocs.io/) [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 # Read the Full documentation on [ReadtheDocs!](https://linkinglines.readthedocs.io/en/latest/)
 
 ## 1. Introduction
 Welcome to the documentation for our Python module that performs the Hough
-Transform on line data from a CSV, clusters it using Agglomerative Clustering,
-and provides functionality to export the results into a CSV file.
+Transform on lines from geospatial data, clusters it using Agglomerative Clustering.
 This module also includes custom plotting scripts and feature extraction
 methods to help you analyze and visualize your data effectively.
 
 This code was used to create the results published in
 [Kubo Hutchison et al., 2023](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022GC010842).
 Initially, it was designed to link together mapped dike segments in Cartesian space
 to find their true lengths. This code can be applied to any linear features including
 roads, fractures, and other types of linear data.
 
 - **Data Clustering**: Apply Agglomerative Clustering to group similar data points, this
-can be used for data reduction, analysis, and mapping .
+can be used for data reduction, analysis, and mapping.
 
 - **Data Visualization**: Custom plotting scripts help you visualize and analyze
 your data, making it easier to identify patterns and anomalies.
 
 - **Feature Extraction**: Extract meaningful features from clustered data to
 perform further analysis, such as linear or radial type features.
 
@@ -81,62 +80,57 @@
 dikeset, Z=ll.AggCluster(data)
 lines,evaluation=examineCluster(data)
 fig,ax=DotsLines(lines, ColorBy='AvgTheta')
 
 ```
 
 We have three examples:
-1. Indepth tutorial with hough transform, clustering, and feature extraction using Spanish Peaks Data CSV file.
+1. In-depth tutorial with Hough transform, clustering, and feature extraction using Spanish Peaks Data CSV file.
 2. Hough Transform and feature extraction on Venus lineament data shape file.
-3. Hough transform on fracture data geoJSON.
+3. Hough Transform on fracture data geoJSON.
 
-Data from: 
+Data from:
 1. https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2022GC010842
 2. https://pubs.usgs.gov/sim/3121/
 3. https://doi.org/10.5281/zenodo.7919843
 
-You are now ready to utilize the power of Hough Line Transform, Agglomerative Clustering, and custom plotting in your data analysis projects. If you have any questions or need further assistance, please refer to the detailed documentation or contact our support team.
-
 
 ## 4. Contributing Guidelines
-Thank you for your interest in contributing to `linkinglines`. Please feel free to open up issues with bugs or requested features. Any contributions you make will benefit everybody else and are greatly appreciated.
 
-We recommend using a virutal environment to manage packages `virtualenv`, see [here](https://virtualenv.pypa.io/en/latest/). 
+If you find bugs or issues please open up an [issues](). We also welcome requests for additional features.
 
-```
-# Install virtualenv if you haven't already
-pip install virtualenv
+If you would like to contribute code please do so in a separate branch and open up an issue describing your contribution.
 
-# Navigate to the project directory
-cd path/to/LinkingLines
+```
+git clone git@github.com:USER/LinkingLines.git
+git checkout my-development-branch
+```
 
-# Create a virtual environment
-virtualenv venv
+We recommend using a virtual environment to manage packages. We use `poetry` to manage dependencies and building.
+See more about [poetry](https://python-poetry.org/).
 
-# Activate the virtual environment
-# On Windows
-venv\Scripts\activate
-# On Unix or MacOS
-source venv/bin/activate
 
-# Install dependencies
-pip install -r requirements.txt
 ```
+pipx install poetry # you may need to install pipx first
 
-If you would like to contribute code please do so in a seperate branch and open up an issue describing your contribution.
+cd linkinglines # go to the repo
+
+poetry install --with test,dev # install in editable mode
+
+# add your code
+
+poetry run pytest  # test code locally
 
 ```
-git clone git@github.com:aikubo/LinkingLines.git
-git checkout my-development-branch
-```
+
 
 Before submitting your pull request please verify the following:
 
 1. Code is documented in [NumPy Docstring Style](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_numpy.html)
-2. Code is tested and passes test 
-    - To run the tests please go to "/tests" and run `pytest`
+2. Code is tested and passes test
+    - To run the tests please go to "/tests" and run `poetry run pytest` or `pytest`
     - Add your test code to any file with the name `test`
     - More here on [pytest and testing practices](https://docs.pytest.org/en/8.0.x/)
-3. Open an issue and pull request 
-
-After your pull request the code will be reviewed by maintainers. After the sucessful merge the documentation will be regenerated.
+3. Open an issue and pull request
+4. After your pull request the code will be reviewed by maintainer (namely @aikubo).
+5. After passing review and automated tests it will be added to the next release and published to pypi.
```

