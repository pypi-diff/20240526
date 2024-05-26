# Comparing `tmp/tenshitranslator-1.0.4.tar.gz` & `tmp/tenshitranslator-2.0.0.tar.gz`

## Comparing `tenshitranslator-1.0.4.tar` & `tenshitranslator-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/__init__.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/CSVGlossary.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/Glossary.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/PassthroughGlossary.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Glossary/__init__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/LineByLineFormat.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/OutputFormat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/__init__.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/BatchTranslator.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/OfflineTranslator.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/OnlineTranslator.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/Translator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Translator/__init__.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Util/TextProcessor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/TenshiTranslator/Util/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/LICENSE
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/README.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    46305 2020-02-02 00:00:00.000000 tenshitranslator-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/__init__.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Glossary/CSVGlossary.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Glossary/Glossary.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Glossary/PassthroughGlossary.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Glossary/__init__.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/LineByLineFormat.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/OutputFormat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/__init__.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Translator/BatchTranslator.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Translator/OfflineTranslator.py
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Translator/OnlineTranslator.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Translator/Translator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Translator/__init__.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Util/TextProcessor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/TenshiTranslator/Util/__init__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/README.md
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    46793 2020-02-02 00:00:00.000000 tenshitranslator-2.0.0/PKG-INFO
```

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Glossary/CSVGlossary.py` & `tenshitranslator-2.0.0/TenshiTranslator/Glossary/CSVGlossary.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Glossary/Glossary.py` & `tenshitranslator-2.0.0/TenshiTranslator/Glossary/Glossary.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py` & `tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/EnglishOnlyFormat.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/LineByLineFormat.py` & `tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/LineByLineFormat.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/OutputFormat/OutputFormat.py` & `tenshitranslator-2.0.0/TenshiTranslator/OutputFormat/OutputFormat.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Translator/BatchTranslator.py` & `tenshitranslator-2.0.0/TenshiTranslator/Translator/BatchTranslator.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Translator/OfflineTranslator.py` & `tenshitranslator-2.0.0/TenshiTranslator/Translator/OfflineTranslator.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Translator/OnlineTranslator.py` & `tenshitranslator-2.0.0/TenshiTranslator/Translator/OnlineTranslator.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Translator/Translator.py` & `tenshitranslator-2.0.0/TenshiTranslator/Translator/Translator.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/TenshiTranslator/Util/TextProcessor.py` & `tenshitranslator-2.0.0/TenshiTranslator/Util/TextProcessor.py`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/LICENSE` & `tenshitranslator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tenshitranslator-1.0.4/README.md` & `tenshitranslator-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 [![Unit Test](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml/badge.svg)](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/Ryan4253/TenshiTranslator/graph/badge.svg?token=G04BIXZ45E)](https://codecov.io/gh/Ryan4253/TenshiTranslator)
 [![PyPI version](https://badge.fury.io/py/TenshiTranslator.svg)](https://badge.fury.io/py/TenshiTranslator)
 
 # TenshiTranslator
 Sugoi Toolkit's [Sugoi Translator](https://sugoitoolkit.com/) is very effective for ACG (Anime, Comit, Games) media translation as the model is trained with data from the same medium. However, the project lacks automation support as all the features require manual control, which makes large file translation incredibly daunting. This project implements automation utility that interfaces with the translator to both automate the translation process and increase the translation accuracy. This project has since then been adopted by over 10 novel series to generate preliminary machine translations for new novels.  
 
+## Demos
+### GUI App (Click For Video)
+[![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/674100e7-1b61-4a23-9e72-5284a69a4091)](https://www.youtube.com/watch?v=CoYnrSkI5Q0&ab_channel=RyanLiao)
+
+### CLI App
 ![project](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/263efe3b-5062-4ec2-961e-943658f54ec7)  
 
 
 ## Getting Started
-You can install the project using ```pip install TenshiTranslator```  
+You can download both the CLI and GUI application from the [latest release](https://github.com/Ryan4253/TenshiTranslator/releases/latest) page
+To use the code as a Python package, run ```pip install TenshiTranslator```  
 For more information, visit the documentation [here](https://ryan4253.github.io/TenshiTranslator/)
 
 ## Translator Options
 
 ### Online Translator
 This translator automates Sugoi Toolkit's [web translator](sugoitranslator.com) with zero extra setup required. However, it is both the slowest and the least accurate due to an older model, api limits, and a character limit.  
 ![online](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/ee3a442d-a03e-4e27-9075-d0d9a8c627d7)
@@ -39,17 +45,18 @@
 You can specify translations for specific phrases and also apply corrections to the translated text to improve translation accuracy. This is commonly used for names and other jargons that may not be translated correctly.  
 <br>
 ![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/2be406f1-ed6a-4eef-979f-24940f342ab3)
 ![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/04264b62-1be2-4506-9889-7bb048533723)  
 Example replacement & correction with regex
 
 ## Requirements
-To run the program, you need Python >= 3.10  
-To use the offline and batch translator, you need Windows, and download Sugoi Toolkit from [here](https://www.patreon.com/mingshiba/about)  
-To use the batch translator, you need a computer with a Nvidia GPU and [CUDA](https://developer.nvidia.com/cuda-downloads)
+The applications are tested on Windows and are available directly for use
+The Python package version requires Python >= 3.10
+To use the offline and batch translator, you need to download Sugoi Toolkit from [here](https://www.patreon.com/mingshiba/about)  
+To use the batch translator, you need a computer with a Nvidia GPU and [CUDA](https://developer.nvidia.com/cuda-downloads), then run the install script
 
 ## Benchmarks
 ![benchmark](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/e12ce131-ec07-4de8-a3bb-46bac0a13f41)  
 Benchmark is done by measuring the time taken to translate 125 lines. Benchmark is run with an Intel i7-13700k and a Nvidia RTX 3060ti 8G
 
 ## Credits
 CUDA Installation script is adapted from the work by Tenerezza from the Sugoi Toolkit Discord
```

### Comparing `tenshitranslator-1.0.4/pyproject.toml` & `tenshitranslator-2.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "TenshiTranslator"
-version = "1.0.4"
+version = "2.0.0"
 requires-python = ">=3.10"
 authors = [{ name="Ryan4253", email="ryan.liao0305@gmail.com" }]
 description = "Novel Translation utility using Sugoi Translator"
 readme = "README.md"
 license = {file="LICENSE"}
 
 dependencies = [
@@ -17,15 +17,15 @@
   "chromedriver-autoinstaller",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: Microsoft :: Windows",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Framework :: Pytest",
     "Framework :: Sphinx",
     "Topic :: Text Processing :: Linguistic"
 ]
 
 [project.urls]
 Homepage = "https://github.com/Ryan4253/TenshiTranslator"
@@ -34,9 +34,11 @@
 
 [tool.hatch.build]
 include = [
   "TenshiTranslator/*",
 ]
 
 exclude = [
-  "TenshiTranslator/Backend.py"
+  "TenshiTranslator/TenshiTranslatorCLI.py",
+  "TenshiTranslator/TenshiTranslatorGUI.py",
+  "TenshiTranslator/UI/*",
 ]
```

### Comparing `tenshitranslator-1.0.4/PKG-INFO` & `tenshitranslator-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: TenshiTranslator
-Version: 1.0.4
+Version: 2.0.0
 Summary: Novel Translation utility using Sugoi Translator
 Project-URL: Homepage, https://github.com/Ryan4253/TenshiTranslator
 Project-URL: Issues, https://github.com/Ryan4253/TenshiTranslator/issues
 Project-URL: documentation, https://ryan4253.github.io/TenshiTranslator/
 Author-email: Ryan4253 <ryan.liao0305@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -677,15 +677,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Framework :: Sphinx
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.10
@@ -698,19 +698,25 @@
 [![Unit Test](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml/badge.svg)](https://github.com/Ryan4253/TenshiTranslator/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/Ryan4253/TenshiTranslator/graph/badge.svg?token=G04BIXZ45E)](https://codecov.io/gh/Ryan4253/TenshiTranslator)
 [![PyPI version](https://badge.fury.io/py/TenshiTranslator.svg)](https://badge.fury.io/py/TenshiTranslator)
 
 # TenshiTranslator
 Sugoi Toolkit's [Sugoi Translator](https://sugoitoolkit.com/) is very effective for ACG (Anime, Comit, Games) media translation as the model is trained with data from the same medium. However, the project lacks automation support as all the features require manual control, which makes large file translation incredibly daunting. This project implements automation utility that interfaces with the translator to both automate the translation process and increase the translation accuracy. This project has since then been adopted by over 10 novel series to generate preliminary machine translations for new novels.  
 
+## Demos
+### GUI App (Click For Video)
+[![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/674100e7-1b61-4a23-9e72-5284a69a4091)](https://www.youtube.com/watch?v=CoYnrSkI5Q0&ab_channel=RyanLiao)
+
+### CLI App
 ![project](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/263efe3b-5062-4ec2-961e-943658f54ec7)  
 
 
 ## Getting Started
-You can install the project using ```pip install TenshiTranslator```  
+You can download both the CLI and GUI application from the [latest release](https://github.com/Ryan4253/TenshiTranslator/releases/latest) page
+To use the code as a Python package, run ```pip install TenshiTranslator```  
 For more information, visit the documentation [here](https://ryan4253.github.io/TenshiTranslator/)
 
 ## Translator Options
 
 ### Online Translator
 This translator automates Sugoi Toolkit's [web translator](sugoitranslator.com) with zero extra setup required. However, it is both the slowest and the least accurate due to an older model, api limits, and a character limit.  
 ![online](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/ee3a442d-a03e-4e27-9075-d0d9a8c627d7)
@@ -735,17 +741,18 @@
 You can specify translations for specific phrases and also apply corrections to the translated text to improve translation accuracy. This is commonly used for names and other jargons that may not be translated correctly.  
 <br>
 ![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/2be406f1-ed6a-4eef-979f-24940f342ab3)
 ![image](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/04264b62-1be2-4506-9889-7bb048533723)  
 Example replacement & correction with regex
 
 ## Requirements
-To run the program, you need Python >= 3.10  
-To use the offline and batch translator, you need Windows, and download Sugoi Toolkit from [here](https://www.patreon.com/mingshiba/about)  
-To use the batch translator, you need a computer with a Nvidia GPU and [CUDA](https://developer.nvidia.com/cuda-downloads)
+The applications are tested on Windows and are available directly for use
+The Python package version requires Python >= 3.10
+To use the offline and batch translator, you need to download Sugoi Toolkit from [here](https://www.patreon.com/mingshiba/about)  
+To use the batch translator, you need a computer with a Nvidia GPU and [CUDA](https://developer.nvidia.com/cuda-downloads), then run the install script
 
 ## Benchmarks
 ![benchmark](https://github.com/Ryan4253/TenshiTranslator/assets/71594512/e12ce131-ec07-4de8-a3bb-46bac0a13f41)  
 Benchmark is done by measuring the time taken to translate 125 lines. Benchmark is run with an Intel i7-13700k and a Nvidia RTX 3060ti 8G
 
 ## Credits
 CUDA Installation script is adapted from the work by Tenerezza from the Sugoi Toolkit Discord
```

