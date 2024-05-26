# Comparing `tmp/bia-bob-0.8.1.tar.gz` & `tmp/bia-bob-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bia-bob-0.8.1.tar", last modified: Tue Dec 26 12:01:54 2023, max compression
+gzip compressed data, was "bia-bob-0.9.0.tar", last modified: Tue Jan 16 15:51:55 2024, max compression
```

## Comparing `bia-bob-0.8.1.tar` & `bia-bob-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-12-26 12:01:54.024965 bia-bob-0.8.1/
--rw-rw-rw-   0        0        0     1546 2023-12-26 08:20:37.000000 bia-bob-0.8.1/LICENSE
--rw-rw-rw-   0        0        0      101 2023-08-07 14:03:50.000000 bia-bob-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8336 2023-12-26 12:01:54.024965 bia-bob-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     6910 2023-12-26 11:43:13.000000 bia-bob-0.8.1/README.md
--rw-rw-rw-   0        0        0     1233 2023-08-07 14:03:50.000000 bia-bob-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0     1561 2023-12-26 12:01:54.030968 bia-bob-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0       89 2023-08-07 14:03:50.000000 bia-bob-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-26 12:01:53.998982 bia-bob-0.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-12-26 12:01:54.006882 bia-bob-0.8.1/src/bia_bob/
--rw-rw-rw-   0        0        0      307 2023-12-26 11:59:56.000000 bia-bob-0.8.1/src/bia_bob/__init__.py
--rw-rw-rw-   0        0        0     1208 2023-12-26 08:20:37.000000 bia-bob-0.8.1/src/bia_bob/_bug_fixing.py
--rw-rw-rw-   0        0        0      922 2023-12-26 08:20:37.000000 bia-bob-0.8.1/src/bia_bob/_document.py
--rw-rw-rw-   0        0        0     4027 2023-12-26 11:43:13.000000 bia-bob-0.8.1/src/bia_bob/_machinery.py
-drwxrwxrwx   0        0        0        0 2023-12-26 12:01:54.022963 bia-bob-0.8.1/src/bia_bob/_tests/
--rw-rw-rw-   0        0        0       31 2023-08-07 14:03:50.000000 bia-bob-0.8.1/src/bia_bob/_tests/__init__.py
--rw-rw-rw-   0        0        0    13378 2023-12-26 11:59:56.000000 bia-bob-0.8.1/src/bia_bob/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-12-26 12:01:54.023964 bia-bob-0.8.1/src/bia_bob.egg-info/
--rw-rw-rw-   0        0        0     8336 2023-12-26 12:01:53.000000 bia-bob-0.8.1/src/bia_bob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-12-26 12:01:53.000000 bia-bob-0.8.1/src/bia_bob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-26 12:01:53.000000 bia-bob-0.8.1/src/bia_bob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-12-26 12:01:53.000000 bia-bob-0.8.1/src/bia_bob.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-12-26 12:01:53.000000 bia-bob-0.8.1/src/bia_bob.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-16 15:51:55.739603 bia-bob-0.9.0/
+-rw-rw-rw-   0        0        0     1546 2023-12-26 08:20:37.000000 bia-bob-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      131 2024-01-16 09:27:30.000000 bia-bob-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9708 2024-01-16 15:51:55.738603 bia-bob-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8224 2024-01-16 15:43:30.000000 bia-bob-0.9.0/README.md
+-rw-rw-rw-   0        0        0     1233 2023-08-07 14:03:50.000000 bia-bob-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1591 2024-01-16 15:51:55.744603 bia-bob-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0       89 2023-08-07 14:03:50.000000 bia-bob-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-16 15:51:55.709598 bia-bob-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2024-01-16 15:51:55.722603 bia-bob-0.9.0/src/bia_bob/
+-rw-rw-rw-   0        0        0      307 2024-01-16 15:29:07.000000 bia-bob-0.9.0/src/bia_bob/__init__.py
+-rw-rw-rw-   0        0        0       97 2024-01-16 09:27:30.000000 bia-bob-0.9.0/src/bia_bob/__main__.py
+-rw-rw-rw-   0        0        0     1259 2024-01-16 09:27:30.000000 bia-bob-0.9.0/src/bia_bob/_bug_fixing.py
+-rw-rw-rw-   0        0        0     1061 2024-01-16 15:29:07.000000 bia-bob-0.9.0/src/bia_bob/_document.py
+-rw-rw-rw-   0        0        0     5380 2024-01-16 15:29:07.000000 bia-bob-0.9.0/src/bia_bob/_kernel.py
+-rw-rw-rw-   0        0        0     4190 2024-01-16 15:29:07.000000 bia-bob-0.9.0/src/bia_bob/_machinery.py
+drwxrwxrwx   0        0        0        0 2024-01-16 15:51:55.737610 bia-bob-0.9.0/src/bia_bob/_tests/
+-rw-rw-rw-   0        0        0       31 2023-08-07 14:03:50.000000 bia-bob-0.9.0/src/bia_bob/_tests/__init__.py
+-rw-rw-rw-   0        0        0    15739 2024-01-16 15:29:07.000000 bia-bob-0.9.0/src/bia_bob/_utilities.py
+drwxrwxrwx   0        0        0        0 2024-01-16 15:51:55.737610 bia-bob-0.9.0/src/bia_bob.egg-info/
+-rw-rw-rw-   0        0        0     9708 2024-01-16 15:51:55.000000 bia-bob-0.9.0/src/bia_bob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2024-01-16 15:51:55.000000 bia-bob-0.9.0/src/bia_bob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-16 15:51:55.000000 bia-bob-0.9.0/src/bia_bob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-01-16 15:51:55.000000 bia-bob-0.9.0/src/bia_bob.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-01-16 15:51:55.000000 bia-bob-0.9.0/src/bia_bob.egg-info/top_level.txt
```

### Comparing `bia-bob-0.8.1/LICENSE` & `bia-bob-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bia-bob-0.8.1/PKG-INFO` & `bia-bob-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Jupyter-based assistant for data analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase, Christian Tischer
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
@@ -22,27 +22,34 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipython
+Requires-Dist: jupyter_client
+Requires-Dist: metakernel
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 # bia-bob
 
 BIA `bob` is a Jupyter-based assistant for interacting with data using large language models which generate python code. 
 It can make use of [OpenAI's chatGPT API](https://openai.com/blog/openai-api) or [Google's Vertex AI API](https://cloud.google.com/vertex-ai?hl=en) and [Gemini](https://blog.google/technology/ai/google-gemini-ai/). 
 You need an OpenAI API account or a Google Cloud account to use it.
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/screencast.gif)
 
+> [!CAUTION]
+> When using the OpenAI or Google Gemini API via BiA-Bob, you are bound to the terms of service of these companies.
+> The prompts you enter are transferred to the servers of these companies and may be processed and stored there. 
+> Make sure to not submit any sensitive, confidential or personal data. Also using these services may cost money.
+
 ## Usage
 
 You can initialize `bob` like this:
 ```
 from bia_bob import bob
 ```
 
@@ -65,14 +72,24 @@
 
 ### Code documentation
 
 Using the `%%doc` magic, you can generate documentation for a given code cell.
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/documenting_mini.gif)
 
+### No-code custom Jupyter Kernel
+
+If installed, you can also choose the BiA-Bob from the Launcher in Jupyter lab:
+
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia-bob-custom-kernel.png)
+
+This will give you a Jupyter kernel that allows you to type in English language instead of code:
+
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia-bob-custom-kernel2.png)
+
 ### Example notebooks
 
 * [Basic demo](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
 * [Bio-image analysis workflow](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/analysis_workflow.ipynb)
 * [Choosing a model](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/choose_model.ipynb)
 * [Using Gemini and chatGPT altenating](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/gemini.ipynb)
 * [Interpreting images](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/vision.ipynb)
@@ -130,14 +147,34 @@
 ```
 gcloud auth application-default login
 ```
 Follow the instructions in the browser. Enter your Project ID (not the name). If it worked the terminal should approximately look like this:
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/gcloud_auth.png)
 
+### BiA-Bob Jupyter kernel (optional)
+
+If you want to use the BiA-Bob Jupyter kernel, please run additionally this command:
+
+```
+python -m bia_bob install
+```
+
+You can check if it's installed by printing out the list of installed kernels:
+
+```
+jupyter kernelspec list
+```
+
+And you can uninstall them using this command:
+
+```
+jupyter kernelspec uninstall bia-bob
+```
+
 ## Development
 
 If you want to contribute to `bia-bob`, you can install it in development mode like this:
 
 ```
 git clone https://github.com/haesleinhuepf/bia-bob.git
 cd bia-bob
@@ -180,14 +217,16 @@
 (Feel free to extend this list by sending a pull-request)
 
 
 ## Similar projects
 
 There are similar projects:
 * [jupyter-ai](https://github.com/jupyterlab/jupyter-ai)
+* [chatGPT-jupyter-extension](https://github.com/jflam/chat-gpt-jupyter-extension)
+* [chapyter](https://github.com/chapyter/chapyter/)
 * [napari-chatGPT](https://github.com/royerlab/napari-chatgpt)
 * [bioimageio-chatbot](https://github.com/bioimage-io/bioimageio-chatbot)
 
 ## Issues
 
 If you encounter any problems or want to provide feedback or suggestions, please create a thread on [image.sc](https://image.sc) along with a detailed description and tag @haesleinhuepf .
```

### Comparing `bia-bob-0.8.1/README.md` & `bia-bob-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 
 BIA `bob` is a Jupyter-based assistant for interacting with data using large language models which generate python code. 
 It can make use of [OpenAI's chatGPT API](https://openai.com/blog/openai-api) or [Google's Vertex AI API](https://cloud.google.com/vertex-ai?hl=en) and [Gemini](https://blog.google/technology/ai/google-gemini-ai/). 
 You need an OpenAI API account or a Google Cloud account to use it.
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/screencast.gif)
 
+> [!CAUTION]
+> When using the OpenAI or Google Gemini API via BiA-Bob, you are bound to the terms of service of these companies.
+> The prompts you enter are transferred to the servers of these companies and may be processed and stored there. 
+> Make sure to not submit any sensitive, confidential or personal data. Also using these services may cost money.
+
 ## Usage
 
 You can initialize `bob` like this:
 ```
 from bia_bob import bob
 ```
 
@@ -32,14 +37,24 @@
 
 ### Code documentation
 
 Using the `%%doc` magic, you can generate documentation for a given code cell.
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/documenting_mini.gif)
 
+### No-code custom Jupyter Kernel
+
+If installed, you can also choose the BiA-Bob from the Launcher in Jupyter lab:
+
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia-bob-custom-kernel.png)
+
+This will give you a Jupyter kernel that allows you to type in English language instead of code:
+
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia-bob-custom-kernel2.png)
+
 ### Example notebooks
 
 * [Basic demo](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
 * [Bio-image analysis workflow](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/analysis_workflow.ipynb)
 * [Choosing a model](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/choose_model.ipynb)
 * [Using Gemini and chatGPT altenating](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/gemini.ipynb)
 * [Interpreting images](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/vision.ipynb)
@@ -97,14 +112,34 @@
 ```
 gcloud auth application-default login
 ```
 Follow the instructions in the browser. Enter your Project ID (not the name). If it worked the terminal should approximately look like this:
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/gcloud_auth.png)
 
+### BiA-Bob Jupyter kernel (optional)
+
+If you want to use the BiA-Bob Jupyter kernel, please run additionally this command:
+
+```
+python -m bia_bob install
+```
+
+You can check if it's installed by printing out the list of installed kernels:
+
+```
+jupyter kernelspec list
+```
+
+And you can uninstall them using this command:
+
+```
+jupyter kernelspec uninstall bia-bob
+```
+
 ## Development
 
 If you want to contribute to `bia-bob`, you can install it in development mode like this:
 
 ```
 git clone https://github.com/haesleinhuepf/bia-bob.git
 cd bia-bob
@@ -147,14 +182,16 @@
 (Feel free to extend this list by sending a pull-request)
 
 
 ## Similar projects
 
 There are similar projects:
 * [jupyter-ai](https://github.com/jupyterlab/jupyter-ai)
+* [chatGPT-jupyter-extension](https://github.com/jflam/chat-gpt-jupyter-extension)
+* [chapyter](https://github.com/chapyter/chapyter/)
 * [napari-chatGPT](https://github.com/royerlab/napari-chatgpt)
 * [bioimageio-chatbot](https://github.com/bioimage-io/bioimageio-chatbot)
 
 ## Issues
 
 If you encounter any problems or want to provide feedback or suggestions, please create a thread on [image.sc](https://image.sc) along with a detailed description and tag @haesleinhuepf .
```

### Comparing `bia-bob-0.8.1/pyproject.toml` & `bia-bob-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bia-bob-0.8.1/setup.cfg` & `bia-bob-0.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -68,31 +68,33 @@
 00000430: 7420 3d20 6874 7470 733a 2f2f 6769 7468  t = https://gith
 00000440: 7562 2e63 6f6d 2f68 6165 736c 6569 6e68  ub.com/haesleinh
 00000450: 7565 7066 2f62 6961 2d62 6f62 2f69 7373  uepf/bia-bob/iss
 00000460: 7565 730d 0a0d 0a5b 6f70 7469 6f6e 735d  ues....[options]
 00000470: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
 00000480: 643a 0d0a 696e 7374 616c 6c5f 7265 7175  d:..install_requ
 00000490: 6972 6573 203d 200d 0a09 6e75 6d70 790d  ires = ...numpy.
-000004a0: 0a09 6970 7974 686f 6e0d 0a70 7974 686f  ..ipython..pytho
-000004b0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000004c0: 2e38 0d0a 696e 636c 7564 655f 7061 636b  .8..include_pack
-000004d0: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-000004e0: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-000004f0: 0a09 3d73 7263 0d0a 0d0a 5b6f 7074 696f  ..=src....[optio
-00000500: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000510: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-00000520: 0d0a 5b6f 7074 696f 6e73 2e65 7874 7261  ..[options.extra
-00000530: 735f 7265 7175 6972 655d 0d0a 7465 7374  s_require]..test
-00000540: 696e 6720 3d20 0d0a 0974 6f78 0d0a 0970  ing = ...tox...p
-00000550: 7974 6573 7420 2023 2068 7474 7073 3a2f  ytest  # https:/
-00000560: 2f64 6f63 732e 7079 7465 7374 2e6f 7267  /docs.pytest.org
-00000570: 2f65 6e2f 6c61 7465 7374 2f63 6f6e 7465  /en/latest/conte
-00000580: 6e74 732e 6874 6d6c 0d0a 0970 7974 6573  nts.html...pytes
-00000590: 742d 636f 7620 2023 2068 7474 7073 3a2f  t-cov  # https:/
-000005a0: 2f70 7974 6573 742d 636f 762e 7265 6164  /pytest-cov.read
-000005b0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000005c0: 7465 7374 2f0d 0a0d 0a5b 6f70 7469 6f6e  test/....[option
-000005d0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-000005e0: 0a2a 203d 202a 2e79 616d 6c0d 0a0d 0a5b  .* = *.yaml....[
-000005f0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000600: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000610: 6520 3d20 300d 0a0d 0a                   e = 0....
+000004a0: 0a09 6970 7974 686f 6e0d 0a09 6a75 7079  ..ipython...jupy
+000004b0: 7465 725f 636c 6965 6e74 0d0a 096d 6574  ter_client...met
+000004c0: 616b 6572 6e65 6c0d 0a70 7974 686f 6e5f  akernel..python_
+000004d0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+000004e0: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+000004f0: 655f 6461 7461 203d 2054 7275 650d 0a70  e_data = True..p
+00000500: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000510: 3d73 7263 0d0a 0d0a 5b6f 7074 696f 6e73  =src....[options
+00000520: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+00000530: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
+00000540: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+00000550: 7265 7175 6972 655d 0d0a 7465 7374 696e  require]..testin
+00000560: 6720 3d20 0d0a 0974 6f78 0d0a 0970 7974  g = ...tox...pyt
+00000570: 6573 7420 2023 2068 7474 7073 3a2f 2f64  est  # https://d
+00000580: 6f63 732e 7079 7465 7374 2e6f 7267 2f65  ocs.pytest.org/e
+00000590: 6e2f 6c61 7465 7374 2f63 6f6e 7465 6e74  n/latest/content
+000005a0: 732e 6874 6d6c 0d0a 0970 7974 6573 742d  s.html...pytest-
+000005b0: 636f 7620 2023 2068 7474 7073 3a2f 2f70  cov  # https://p
+000005c0: 7974 6573 742d 636f 762e 7265 6164 7468  ytest-cov.readth
+000005d0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000005e0: 7374 2f0d 0a0d 0a5b 6f70 7469 6f6e 732e  st/....[options.
+000005f0: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
+00000600: 203d 202a 2e79 616d 6c0d 0a0d 0a5b 6567   = *.yaml....[eg
+00000610: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000620: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000630: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `bia-bob-0.8.1/src/bia_bob/_bug_fixing.py` & `bia-bob-0.9.0/src/bia_bob/_bug_fixing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from IPython.core.magic import register_line_cell_magic
 
 
-@register_line_cell_magic
 def fix(line: str = None, cell: str = None):
     """This Jupyter Magic automatically fixes code when it's in the first line of a cell that caused an error that just
     happened.
     """
     from IPython.core.getipython import get_ipython
     from ._machinery import bob, combine_user_input, Context, init_assistant
     from ._utilities import generate_response_to_user
@@ -38,7 +37,15 @@
     if Context.model is None:
         init_assistant()
     p = get_ipython()
 
     code, text = generate_response_to_user(Context.model, prompt)
 
     p.set_next_input(code, replace=True)
+
+
+try:
+    register_line_cell_magic(fix)
+except NameError:
+    pass
+
+
```

### Comparing `bia-bob-0.8.1/src/bia_bob/_document.py` & `bia-bob-0.9.0/src/bia_bob/_document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from IPython.core.magic import register_line_cell_magic
 
 
-@register_line_cell_magic
 def doc(line:str=None, cell:str=None):
     """
     This Jupyter Magic automatically documents code when it's in the first line of a cell.
     """
     from ._machinery import Context, init_assistant, combine_user_input
     from ._utilities import generate_response_to_user
     from IPython.core.getipython import get_ipython
 
     code = combine_user_input(line, cell)
 
     prompt = f"""
-    Please write comments in the following code.
+    Summarize the following code. 
+    Provide a step-by-step plan for the code.
+    Please write comments in the code.
     Put comments on new lines before the code block you describe. 
-    If there are functions in the code, add numpy-style docstrings.
+    Only, if there are functions in the code, add numpy-style docstrings to these functions.
     
     ```python
-    {code}
+{code}
     ```
     """
 
     if Context.model is None:
         init_assistant()
     p = get_ipython()
 
     code, text = generate_response_to_user(Context.model, prompt)
 
     p.set_next_input(code, replace=True)
 
 
+try:
+    register_line_cell_magic(doc)
+except NameError:
+    pass
+
```

### Comparing `bia-bob-0.8.1/src/bia_bob/_machinery.py` & `bia-bob-0.9.0/src/bia_bob/_machinery.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     variables = None
     model = None
     verbose = False
     auto_execute = False
     chat = []
     client = None
     plugins_enabled = True
+    seed = None # openai only
+    temperature = None # openai only
+
     libraries = keep_available_packages([
         "scikit-image",
         "numpy",
         "scipy",
         "pandas",
         "matplotlib",
         "seaborn",
@@ -21,27 +24,27 @@
         "stackview",
         "torch",
         "pytorch-lightning",
         "cellpose",
         "stardist",
         "n2v",
         "pyclesperanto-prototype",
+        "pyclesperanto_prototype",
         "apoc",
         "napari-segment-blobs-and-things-with-membranes",
         "napari-simpleitk-image-processing",
         "napari-skimage-regionprops",
         "skan",
-        "aicsimageio"
+        "aicsimageio",
+        "os"
 
         # to add libraries here, add their pypi package names (not their import names)
     ])
 
 
-
-@register_line_cell_magic
 def bob(line: str = None, cell: str = None):
     """Sends a prompt to openAI
     and shows the text and code response
     and pastes the code into the next cell.
     """
     from IPython.core.getipython import get_ipython
     from IPython.display import display
@@ -50,15 +53,15 @@
     if Context.model is None:
         init_assistant()
 
     if line in Context.variables and is_image(Context.variables[line]):
         image = Context.variables[line]
     else:
         image = None
-    
+
     user_input = combine_user_input(line, cell)
 
     if user_input is None:
         display("Please ask a question!")
         return
 
     # generate the response
@@ -76,14 +79,20 @@
             # execute it
             p.run_cell(code)
         else:
             # put a new cell below the current cell
             p.set_next_input(code, replace=False)
 
 
+try:
+    register_line_cell_magic(bob)
+except NameError:
+    pass
+
+
 def combine_user_input(line, cell):
     if line and cell:
         user_input = line + "\n" + cell
     elif line:
         user_input = line
     elif cell:
         user_input = cell
```

### Comparing `bia-bob-0.8.1/src/bia_bob/_utilities.py` & `bia-bob-0.9.0/src/bia_bob/_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,90 @@
-def generate_response_to_user(model, user_prompt: str, image=None):
+def generate_response_to_user(model, user_prompt: str, image=None, additional_system_prompt: str = None, max_number_attempts:int = 3):
     """Generates code and text respond for a specific user input.
     To do so, it combines the user input with additional context such as
     current variables and a prompt template."""
+    from ._machinery import Context
 
-    system_prompt = create_system_prompt()
+    text, plan, code = None, None, None
 
-    # take the last n chat entries
-    from ._machinery import Context
-    n = 10
-    chat_history = Context.chat[-n:]
+    chat_backup = [c for c in Context.chat]
 
-    if Context.verbose:
-        print("\nUser prompt:", user_prompt)
-        print("\nSystem prompt:", system_prompt)
-        print_chat(chat_history)
-
-    if "gpt-" in model:
-        full_response = generate_response_from_openai(model, system_prompt, user_prompt, chat_history, image)
-    elif "gemini-" in model:
-        full_response = generate_response_from_vertex_ai(model, system_prompt, user_prompt, chat_history, image)
-    else:
-        raise RuntimeError(f"Unknown model API for {model}")
+    for attempt in range(1, max_number_attempts + 1):
+        system_prompt = create_system_prompt()
+        if additional_system_prompt is not None:
+            system_prompt += "\n" + additional_system_prompt
+
+        # take the last n chat entries
+        n = 10
+        chat_history = Context.chat[-n:]
+
+        if Context.verbose:
+            print("\nUser prompt:", user_prompt)
+            print("\nSystem prompt:", system_prompt)
+            print_chat(chat_history)
+
+        if "gpt-" in model:
+            full_response = generate_response_from_openai(model, system_prompt, user_prompt, chat_history, image)
+        elif "gemini-" in model:
+            full_response = generate_response_from_vertex_ai(model, system_prompt, user_prompt, chat_history, image)
+        else:
+            raise RuntimeError(f"Unknown model API for {model}")
 
-    if Context.verbose:
-        print("\n\nFull response:\n", full_response)
+        if Context.verbose:
+            print("\n\nFull response:\n", full_response)
 
-    full_response = full_response\
-                    .replace("```python", "```")\
-                    .replace("```nextflow", "```")\
-                    .replace("```java", "```")\
-                    .replace("```javascript", "```")\
-                    .replace("```macro", "```")\
-                    .replace("```groovy", "```")\
-                    .replace("```jython", "```")
-
-    # split response in text and code
-    parts = full_response.split("```")
-    if len(parts) == 1:
-        text = full_response
-        code = None
-    else:
-        text = ""
-        code = ""
-        for t, c in zip(parts[::2], parts[1::2]):
-            text = text + t
-            code = code + c
-        code = code.strip("\n")
+        full_response = full_response\
+                        .replace("```python", "```")\
+                        .replace("```nextflow", "```")\
+                        .replace("```java", "```")\
+                        .replace("```javascript", "```")\
+                        .replace("```macro", "```")\
+                        .replace("```groovy", "```")\
+                        .replace("```jython", "```")
+
+        # split response in text and code
+        text, plan, code = split_response(full_response)
+
+        if text is not None and plan is not None:
+            break
+
+        print(f"There was an issue. Retrying ({attempt}/{max_number_attempts})...")
+        Context.chat = chat_backup
 
     return code, text
 
+def split_response(text):
+    # Split the text based on three predefined Markdown headlines
+    import re
+    sections = re.split(r'### (Summary|Plan|Code)\s*', text)
+
+    # The first element is usually an empty string before the first headline
+    # The rest of the elements are alternating between section names and contents
+    summary, plan, code = None, None, None
+    for i in range(1, len(sections), 2):
+        if sections[i] == 'Summary':
+            summary = sections[i + 1]
+        elif sections[i] == 'Plan':
+            plan = sections[i + 1]
+        elif sections[i] == 'Code':
+            code = sections[i + 1]
+
+    if code is not None:
+        parts = code.split("```")
+        if len(parts) == 1:
+            code = None
+        else:
+            text = ""
+            code = ""
+            for t, c in zip(parts[::2], parts[1::2]):
+                code = code + c
+            code = code.strip("\n")
+
+    return summary, plan, code
+
 
 def create_system_prompt(reusable_variables_block=None):
     """Creates a system prompt that contains instructions of general interest, available functions and variables."""
     # determine useful variables and functions in context
 
     # if scikit-image is installed, give hints how to use it
     from ._machinery import Context
@@ -64,15 +96,19 @@
     image = imread(filename)
     ```
     * Expanding labels by a given radius in a label image works like this:
     ```
     from skimage.segmentation import expand_labels
     expanded_labels = expand_labels(label_image, distance=10)
     ```
-
+    * Measure properties of labels with respect to an image works like this:
+    ```
+    from skimage.measure import regionprops
+    properties = regionprops(label_image, image)
+    ```
     """
     if "scikit-image" not in Context.libraries:
         skimage_snippets = ""
 
     # if aicsimageio is installed, give hints how to use it
     aicsimageio_snippets = """
     * Loading files with endings other than `.tif`, `.png` or `.jpg` works like this:
@@ -101,48 +137,64 @@
         additional_instructions = []
         # Iterate over discovered entry points and load them
         for ep in bia_bob_plugins:
             func = ep.load()
 
             # load instructions from a plugin
             instructions = func()
-            additional_instructions.append(instructions)
+            # special treatment for code snippets from stackview, as it won't work with the custom kernel
+            if "stackview" not in instructions or "stackview" in Context.libraries:
+                additional_instructions.append(instructions)
+
         additional_snippets = "\n".join(additional_instructions)
     else:
         additional_snippets = ""
 
     system_prompt = f"""
+    You are a extremely talented bioimage analyst and you use Python to solve your tasks unless stated otherwise.
     If the request entails writing code, write concise professional bioimage analysis high-quality code.
-    If there are several ways to solve the task, chose the option with the least amount of code.
-    
+    If there are several ways to solve the task, chose the option with the least amount of code.    
     If there is no specific programming language required, write python code and follow the below instructions.
     
     {reusable_variables_block}
     
     ## Python specific code snippets
     
     If the user asks for those simple tasks, use these code snippets.
     {skimage_snippets}
     {aicsimageio_snippets}
     {additional_snippets}
     
-    ## Explanations and code
+    ## Todos
+    
+    Answer your response in three sections:
+    1. Summary: First provide a short summary of the task.
+    2. Plan: Provide a concise step-by-step plan without any code.
+    3. Code: Provide the code.
+    
+    Structure it with markdown headings like this:
     
-    Initially, provide a concise step-by-step plan without any code. 
-    Always provide the plan first.
+    ### Summary
+    I will do this and that.
     
-    After the complete plan, print the code.
-    There must be only one single code block.
-    Importantly, the code block must start with the line: 
+    ### Plan
+    1. Do this.
+    2. Do that.
+    
+    ### Code
     ```
-    and it must end with the line:
+    this()
+    that()
     ```
     
-    There must be no text after the code block.
-    If the request does not require to write code, simply answer in plain text.
+    ## Final remarks
+    
+    The following points have highest importance and may overwrite the instructions above.
+    Make sure to provide 1) summary, 2) plan and 3) code.
+    Make sure to keep your answer concise and to the point. Make sure the code you write is correct and can be executed.
     """
 
     return system_prompt
 
 
 def create_reusable_variables_block():
     """Creates a block of text that explains which variables, functions and libraries are
@@ -228,14 +280,19 @@
     if model == "gpt-4-vision-preview":
         # this seems necessary according to the docs:
         # https://platform.openai.com/docs/guides/vision
         # if it is not provided, the response will be
         # cropped to half a sentence
         kwargs['max_tokens'] = 3000
 
+    if Context.seed is not None:
+        kwargs['seed'] = Context.seed
+    if Context.temperature is not None:
+        kwargs['temperature'] = Context.temperature
+
     # init client
     if Context.client is None or not isinstance(Context.client, OpenAI):
         Context.client = OpenAI()
 
     # retrieve answer
     response = Context.client.chat.completions.create(
         messages=system_message + chat_history + image_message + user_message,
@@ -279,15 +336,15 @@
             prompt = f"""
                        {system_prompt}
                        
                        # Task
                        This is the task:
                        {user_prompt}
                        
-                       Remember: Your output should be 1) a step-by-step plan and 2) code.
+                       Remember: Your output should be 1) a summary, 2) a plan and 3) the code.
                        """
         if image is not None:
             from stackview._image_widget import _img_to_rgb
             from darth_d._utilities import numpy_to_bytestream
 
             rgb_image = _img_to_rgb(image)
             byte_stream = numpy_to_bytestream(rgb_image)
@@ -297,15 +354,15 @@
             prompt = f"""
                    {system_prompt}
 
                    # Task
                    This is the task:
                    {user_prompt}
 
-                   If the task is not explicitly about generating code, do not generated any code.
+                   If the task is not explicitly about generating code, do not generate any code.
                    """
 
             prompt = [image, prompt]
 
         response = Context.client.generate_content(prompt).text
 
     else:
@@ -382,11 +439,15 @@
         # Python 3.8+
         from importlib.metadata import distributions
     except ImportError:
         # Python < 3.8
         from importlib_metadata import distributions
 
     installed = [dist.metadata['Name'] for dist in distributions()]
+
+    # add always available packages
+    installed.append('os')
+
     result = [i for i in libraries if i in installed]
 
     return result
```

### Comparing `bia-bob-0.8.1/src/bia_bob.egg-info/PKG-INFO` & `bia-bob-0.9.0/src/bia_bob.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-bob
-Version: 0.8.1
+Version: 0.9.0
 Summary: A Jupyter-based assistant for data analysis tasks
 Home-page: https://github.com/haesleinhuepf/bia-bob
 Author: Robert Haase, Christian Tischer
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/haesleinhuepf/bia-bob/issues
 Project-URL: Documentation, https://github.com/haesleinhuepf/bia-bob#README.md
@@ -22,27 +22,34 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipython
+Requires-Dist: jupyter_client
+Requires-Dist: metakernel
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 # bia-bob
 
 BIA `bob` is a Jupyter-based assistant for interacting with data using large language models which generate python code. 
 It can make use of [OpenAI's chatGPT API](https://openai.com/blog/openai-api) or [Google's Vertex AI API](https://cloud.google.com/vertex-ai?hl=en) and [Gemini](https://blog.google/technology/ai/google-gemini-ai/). 
 You need an OpenAI API account or a Google Cloud account to use it.
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/screencast.gif)
 
+> [!CAUTION]
+> When using the OpenAI or Google Gemini API via BiA-Bob, you are bound to the terms of service of these companies.
+> The prompts you enter are transferred to the servers of these companies and may be processed and stored there. 
+> Make sure to not submit any sensitive, confidential or personal data. Also using these services may cost money.
+
 ## Usage
 
 You can initialize `bob` like this:
 ```
 from bia_bob import bob
 ```
 
@@ -65,14 +72,24 @@
 
 ### Code documentation
 
 Using the `%%doc` magic, you can generate documentation for a given code cell.
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/documenting_mini.gif)
 
+### No-code custom Jupyter Kernel
+
+If installed, you can also choose the BiA-Bob from the Launcher in Jupyter lab:
+
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia-bob-custom-kernel.png)
+
+This will give you a Jupyter kernel that allows you to type in English language instead of code:
+
+![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/bia-bob-custom-kernel2.png)
+
 ### Example notebooks
 
 * [Basic demo](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/basic_demo.ipynb)
 * [Bio-image analysis workflow](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/analysis_workflow.ipynb)
 * [Choosing a model](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/choose_model.ipynb)
 * [Using Gemini and chatGPT altenating](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/gemini.ipynb)
 * [Interpreting images](https://github.com/haesleinhuepf/bia-bob/blob/main/demo/vision.ipynb)
@@ -130,14 +147,34 @@
 ```
 gcloud auth application-default login
 ```
 Follow the instructions in the browser. Enter your Project ID (not the name). If it worked the terminal should approximately look like this:
 
 ![img.png](https://github.com/haesleinhuepf/bia-bob/raw/main/docs/images/gcloud_auth.png)
 
+### BiA-Bob Jupyter kernel (optional)
+
+If you want to use the BiA-Bob Jupyter kernel, please run additionally this command:
+
+```
+python -m bia_bob install
+```
+
+You can check if it's installed by printing out the list of installed kernels:
+
+```
+jupyter kernelspec list
+```
+
+And you can uninstall them using this command:
+
+```
+jupyter kernelspec uninstall bia-bob
+```
+
 ## Development
 
 If you want to contribute to `bia-bob`, you can install it in development mode like this:
 
 ```
 git clone https://github.com/haesleinhuepf/bia-bob.git
 cd bia-bob
@@ -180,14 +217,16 @@
 (Feel free to extend this list by sending a pull-request)
 
 
 ## Similar projects
 
 There are similar projects:
 * [jupyter-ai](https://github.com/jupyterlab/jupyter-ai)
+* [chatGPT-jupyter-extension](https://github.com/jflam/chat-gpt-jupyter-extension)
+* [chapyter](https://github.com/chapyter/chapyter/)
 * [napari-chatGPT](https://github.com/royerlab/napari-chatgpt)
 * [bioimageio-chatbot](https://github.com/bioimage-io/bioimageio-chatbot)
 
 ## Issues
 
 If you encounter any problems or want to provide feedback or suggestions, please create a thread on [image.sc](https://image.sc) along with a detailed description and tag @haesleinhuepf .
```

