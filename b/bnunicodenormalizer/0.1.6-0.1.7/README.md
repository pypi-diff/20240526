# Comparing `tmp/bnunicodenormalizer-0.1.6.tar.gz` & `tmp/bnunicodenormalizer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnunicodenormalizer-0.1.6.tar", last modified: Sat Apr 15 15:18:24 2023, max compression
+gzip compressed data, was "bnunicodenormalizer-0.1.7.tar", last modified: Sun May 26 16:54:30 2024, max compression
```

## Comparing `bnunicodenormalizer-0.1.6.tar` & `bnunicodenormalizer-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     2793 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/CHANGELOG.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1067 2022-02-15 05:44:06.000000 bnunicodenormalizer-0.1.6/LICENSE
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2022-02-12 04:15:33.000000 bnunicodenormalizer-0.1.6/MANIFEST.in
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    20541 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    17137 2022-12-31 19:51:24.000000 bnunicodenormalizer-0.1.6/README.md
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.617163 bnunicodenormalizer-0.1.6/bnunicodenormalizer/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      190 2022-10-21 00:24:37.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/__init__.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    13947 2022-10-21 03:53:23.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/base.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1923 2022-12-31 19:53:42.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/indic.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    43487 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/langs.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    20883 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer/normalizer.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.617163 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    20541 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/PKG-INFO
--rw-rw-r--   0 ansary    (1000) ansary    (1000)      438 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/SOURCES.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/dependency_links.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       20 2023-04-15 15:18:24.000000 bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/top_level.txt
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/extra/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)    57070 2022-10-21 02:59:20.000000 bnunicodenormalizer-0.1.6/extra/conjuncts.py
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     3002 2022-06-15 05:35:07.000000 bnunicodenormalizer-0.1.6/extra/missing.txt
--rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/setup.cfg
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     1044 2023-04-15 15:16:57.000000 bnunicodenormalizer-0.1.6/setup.py
-drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2023-04-15 15:18:24.621163 bnunicodenormalizer-0.1.6/tests/
--rw-rw-r--   0 ansary    (1000) ansary    (1000)     5521 2022-09-10 17:59:24.000000 bnunicodenormalizer-0.1.6/tests/test_normalizer.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 16:54:30.923528 bnunicodenormalizer-0.1.7/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     2854 2024-05-26 16:52:00.000000 bnunicodenormalizer-0.1.7/CHANGELOG.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1067 2023-04-15 06:54:42.000000 bnunicodenormalizer-0.1.7/LICENSE
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       25 2023-04-15 06:54:42.000000 bnunicodenormalizer-0.1.7/MANIFEST.in
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    22535 2024-05-26 16:54:30.923528 bnunicodenormalizer-0.1.7/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    19089 2024-05-26 16:53:32.000000 bnunicodenormalizer-0.1.7/README.md
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 16:54:30.923528 bnunicodenormalizer-0.1.7/bnunicodenormalizer/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      190 2023-04-15 06:54:42.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer/__init__.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    13947 2023-04-15 06:54:42.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer/base.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1923 2023-04-15 06:54:42.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer/indic.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    43487 2023-04-15 07:06:59.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer/langs.py
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    20883 2023-04-15 07:09:45.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer/normalizer.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 16:54:30.923528 bnunicodenormalizer-0.1.7/bnunicodenormalizer.egg-info/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)    22535 2024-05-26 16:54:30.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer.egg-info/PKG-INFO
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)      401 2024-05-26 16:54:30.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)        1 2024-05-26 16:54:30.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       20 2024-05-26 16:54:30.000000 bnunicodenormalizer-0.1.7/bnunicodenormalizer.egg-info/top_level.txt
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)       38 2024-05-26 16:54:30.923528 bnunicodenormalizer-0.1.7/setup.cfg
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     1044 2024-05-26 16:52:10.000000 bnunicodenormalizer-0.1.7/setup.py
+drwxrwxr-x   0 ansary    (1000) ansary    (1000)        0 2024-05-26 16:54:30.923528 bnunicodenormalizer-0.1.7/tests/
+-rw-rw-r--   0 ansary    (1000) ansary    (1000)     5521 2023-04-15 06:54:42.000000 bnunicodenormalizer-0.1.7/tests/test_normalizer.py
```

### Comparing `bnunicodenormalizer-0.1.6/CHANGELOG.txt` & `bnunicodenormalizer-0.1.7/CHANGELOG.txt`

 * *Files 5% similar despite different names*

```diff
@@ -135,8 +135,12 @@
 
 0.1.5 (01/01/23)
 -------------------
 - cleaned panjabi double quotes in diac map 
 
 0.1.6 (15/04/23)
 -------------------
-- added bangla punctuations 
+- added bangla punctuations 
+
+0.1.7 (26/05/24)
+-------------------
+- added proper bibtex
```

### Comparing `bnunicodenormalizer-0.1.6/LICENSE` & `bnunicodenormalizer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.6/PKG-INFO` & `bnunicodenormalizer-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: bnunicodenormalizer
-Version: 0.1.6
+Version: 0.1.7
 Summary: Bangla Unicode Normalization Toolkit
 Home-page: https://github.com/mnansary/bnUnicodeNormalizer
 Author: Bengali.AI
 Author-email: research.bengaliai@gmail.com
 License: MIT
 Keywords: bangla,unicode,text normalization,indic
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -394,26 +393,45 @@
 '''        
         
 ```
 
 
 # ABOUT US
 * Authors: [Bengali.AI](https://bengali.ai/) in association with OCR Team , [APSIS Solutions Limited](https://apsissolutions.com/) 
-* **Cite Bengali.AI multipurpose grapheme dataset paper**
+* **Cite Our Work**
 ```bibtext
-@inproceedings{alam2021large,
-  title={A large multi-target dataset of common bengali handwritten graphemes},
-  author={Alam, Samiul and Reasat, Tahsin and Sushmit, Asif Shahriyar and Siddique, Sadi Mohammad and Rahman, Fuad and Hasan, Mahady and Humayun, Ahmed Imtiaz},
-  booktitle={International Conference on Document Analysis and Recognition},
-  pages={383--398},
-  year={2021},
-  organization={Springer}
+@inproceedings{ansary-etal-2024-unicode-normalization,
+    title = "{U}nicode Normalization and Grapheme Parsing of {I}ndic Languages",
+    author = "Ansary, Nazmuddoha  and
+      Adib, Quazi Adibur Rahman  and
+      Reasat, Tahsin  and
+      Sushmit, Asif Shahriyar  and
+      Humayun, Ahmed Imtiaz  and
+      Mehnaz, Sazia  and
+      Fatema, Kanij  and
+      Rashid, Mohammad Mamun Or  and
+      Sadeque, Farig",
+    editor = "Calzolari, Nicoletta  and
+      Kan, Min-Yen  and
+      Hoste, Veronique  and
+      Lenci, Alessandro  and
+      Sakti, Sakriani  and
+      Xue, Nianwen",
+    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
+    month = may,
+    year = "2024",
+    address = "Torino, Italia",
+    publisher = "ELRA and ICCL",
+    url = "https://aclanthology.org/2024.lrec-main.1479",
+    pages = "17019--17030",
+    abstract = "Writing systems of Indic languages have orthographic syllables, also known as complex graphemes, as unique horizontal units. A prominent feature of these languages is these complex grapheme units that comprise consonants/consonant conjuncts, vowel diacritics, and consonant diacritics, which, together make a unique Language. Unicode-based writing schemes of these languages often disregard this feature of these languages and encode words as linear sequences of Unicode characters using an intricate scheme of connector characters and font interpreters. Due to this way of using a few dozen Unicode glyphs to write thousands of different unique glyphs (complex graphemes), there are serious ambiguities that lead to malformed words. In this paper, we are proposing two libraries: i) a normalizer for normalizing inconsistencies caused by a Unicode-based encoding scheme for Indic languages and ii) a grapheme parser for Abugida text. It deconstructs words into visually distinct orthographic syllables or complex graphemes and their constituents. Our proposed normalizer is a more efficient and effective tool than the previously used IndicNLP normalizer. Moreover, our parser and normalizer are also suitable tools for general Abugida text processing as they performed well in our robust word-based and NLP experiments. We report the pipeline for the scripts of 7 languages in this work and develop the framework for the integration of more scripts.",
 }
 ```
 
+
 Change Log
 ===========
 
 0.0.5 (9/03/2022)
 -------------------
 - added details for execution map
 - checkop typo correction
@@ -549,7 +567,10 @@
 -------------------
 - cleaned panjabi double quotes in diac map 
 
 0.1.6 (15/04/23)
 -------------------
 - added bangla punctuations 
 
+0.1.7 (26/05/24)
+-------------------
+- added proper bibtex
```

### Comparing `bnunicodenormalizer-0.1.6/README.md` & `bnunicodenormalizer-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -376,18 +376,36 @@
 '''        
         
 ```
 
 
 # ABOUT US
 * Authors: [Bengali.AI](https://bengali.ai/) in association with OCR Team , [APSIS Solutions Limited](https://apsissolutions.com/) 
-* **Cite Bengali.AI multipurpose grapheme dataset paper**
+* **Cite Our Work**
 ```bibtext
-@inproceedings{alam2021large,
-  title={A large multi-target dataset of common bengali handwritten graphemes},
-  author={Alam, Samiul and Reasat, Tahsin and Sushmit, Asif Shahriyar and Siddique, Sadi Mohammad and Rahman, Fuad and Hasan, Mahady and Humayun, Ahmed Imtiaz},
-  booktitle={International Conference on Document Analysis and Recognition},
-  pages={383--398},
-  year={2021},
-  organization={Springer}
+@inproceedings{ansary-etal-2024-unicode-normalization,
+    title = "{U}nicode Normalization and Grapheme Parsing of {I}ndic Languages",
+    author = "Ansary, Nazmuddoha  and
+      Adib, Quazi Adibur Rahman  and
+      Reasat, Tahsin  and
+      Sushmit, Asif Shahriyar  and
+      Humayun, Ahmed Imtiaz  and
+      Mehnaz, Sazia  and
+      Fatema, Kanij  and
+      Rashid, Mohammad Mamun Or  and
+      Sadeque, Farig",
+    editor = "Calzolari, Nicoletta  and
+      Kan, Min-Yen  and
+      Hoste, Veronique  and
+      Lenci, Alessandro  and
+      Sakti, Sakriani  and
+      Xue, Nianwen",
+    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
+    month = may,
+    year = "2024",
+    address = "Torino, Italia",
+    publisher = "ELRA and ICCL",
+    url = "https://aclanthology.org/2024.lrec-main.1479",
+    pages = "17019--17030",
+    abstract = "Writing systems of Indic languages have orthographic syllables, also known as complex graphemes, as unique horizontal units. A prominent feature of these languages is these complex grapheme units that comprise consonants/consonant conjuncts, vowel diacritics, and consonant diacritics, which, together make a unique Language. Unicode-based writing schemes of these languages often disregard this feature of these languages and encode words as linear sequences of Unicode characters using an intricate scheme of connector characters and font interpreters. Due to this way of using a few dozen Unicode glyphs to write thousands of different unique glyphs (complex graphemes), there are serious ambiguities that lead to malformed words. In this paper, we are proposing two libraries: i) a normalizer for normalizing inconsistencies caused by a Unicode-based encoding scheme for Indic languages and ii) a grapheme parser for Abugida text. It deconstructs words into visually distinct orthographic syllables or complex graphemes and their constituents. Our proposed normalizer is a more efficient and effective tool than the previously used IndicNLP normalizer. Moreover, our parser and normalizer are also suitable tools for general Abugida text processing as they performed well in our robust word-based and NLP experiments. We report the pipeline for the scripts of 7 languages in this work and develop the framework for the integration of more scripts.",
 }
-```
+```
```

### Comparing `bnunicodenormalizer-0.1.6/bnunicodenormalizer/base.py` & `bnunicodenormalizer-0.1.7/bnunicodenormalizer/base.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.6/bnunicodenormalizer/indic.py` & `bnunicodenormalizer-0.1.7/bnunicodenormalizer/indic.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.6/bnunicodenormalizer/langs.py` & `bnunicodenormalizer-0.1.7/bnunicodenormalizer/langs.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.6/bnunicodenormalizer/normalizer.py` & `bnunicodenormalizer-0.1.7/bnunicodenormalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `bnunicodenormalizer-0.1.6/bnunicodenormalizer.egg-info/PKG-INFO` & `bnunicodenormalizer-0.1.7/bnunicodenormalizer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: bnunicodenormalizer
-Version: 0.1.6
+Version: 0.1.7
 Summary: Bangla Unicode Normalization Toolkit
 Home-page: https://github.com/mnansary/bnUnicodeNormalizer
 Author: Bengali.AI
 Author-email: research.bengaliai@gmail.com
 License: MIT
 Keywords: bangla,unicode,text normalization,indic
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -394,26 +393,45 @@
 '''        
         
 ```
 
 
 # ABOUT US
 * Authors: [Bengali.AI](https://bengali.ai/) in association with OCR Team , [APSIS Solutions Limited](https://apsissolutions.com/) 
-* **Cite Bengali.AI multipurpose grapheme dataset paper**
+* **Cite Our Work**
 ```bibtext
-@inproceedings{alam2021large,
-  title={A large multi-target dataset of common bengali handwritten graphemes},
-  author={Alam, Samiul and Reasat, Tahsin and Sushmit, Asif Shahriyar and Siddique, Sadi Mohammad and Rahman, Fuad and Hasan, Mahady and Humayun, Ahmed Imtiaz},
-  booktitle={International Conference on Document Analysis and Recognition},
-  pages={383--398},
-  year={2021},
-  organization={Springer}
+@inproceedings{ansary-etal-2024-unicode-normalization,
+    title = "{U}nicode Normalization and Grapheme Parsing of {I}ndic Languages",
+    author = "Ansary, Nazmuddoha  and
+      Adib, Quazi Adibur Rahman  and
+      Reasat, Tahsin  and
+      Sushmit, Asif Shahriyar  and
+      Humayun, Ahmed Imtiaz  and
+      Mehnaz, Sazia  and
+      Fatema, Kanij  and
+      Rashid, Mohammad Mamun Or  and
+      Sadeque, Farig",
+    editor = "Calzolari, Nicoletta  and
+      Kan, Min-Yen  and
+      Hoste, Veronique  and
+      Lenci, Alessandro  and
+      Sakti, Sakriani  and
+      Xue, Nianwen",
+    booktitle = "Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)",
+    month = may,
+    year = "2024",
+    address = "Torino, Italia",
+    publisher = "ELRA and ICCL",
+    url = "https://aclanthology.org/2024.lrec-main.1479",
+    pages = "17019--17030",
+    abstract = "Writing systems of Indic languages have orthographic syllables, also known as complex graphemes, as unique horizontal units. A prominent feature of these languages is these complex grapheme units that comprise consonants/consonant conjuncts, vowel diacritics, and consonant diacritics, which, together make a unique Language. Unicode-based writing schemes of these languages often disregard this feature of these languages and encode words as linear sequences of Unicode characters using an intricate scheme of connector characters and font interpreters. Due to this way of using a few dozen Unicode glyphs to write thousands of different unique glyphs (complex graphemes), there are serious ambiguities that lead to malformed words. In this paper, we are proposing two libraries: i) a normalizer for normalizing inconsistencies caused by a Unicode-based encoding scheme for Indic languages and ii) a grapheme parser for Abugida text. It deconstructs words into visually distinct orthographic syllables or complex graphemes and their constituents. Our proposed normalizer is a more efficient and effective tool than the previously used IndicNLP normalizer. Moreover, our parser and normalizer are also suitable tools for general Abugida text processing as they performed well in our robust word-based and NLP experiments. We report the pipeline for the scripts of 7 languages in this work and develop the framework for the integration of more scripts.",
 }
 ```
 
+
 Change Log
 ===========
 
 0.0.5 (9/03/2022)
 -------------------
 - added details for execution map
 - checkop typo correction
@@ -549,7 +567,10 @@
 -------------------
 - cleaned panjabi double quotes in diac map 
 
 0.1.6 (15/04/23)
 -------------------
 - added bangla punctuations 
 
+0.1.7 (26/05/24)
+-------------------
+- added proper bibtex
```

### Comparing `bnunicodenormalizer-0.1.6/setup.py` & `bnunicodenormalizer-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='bnunicodenormalizer',
-  version='0.1.6',
+  version='0.1.7',
   description='Bangla Unicode Normalization Toolkit',
   long_description=open('README.md',encoding='utf-8').read() + '\n\n' + open('CHANGELOG.txt',encoding='utf-8').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/mnansary/bnUnicodeNormalizer',  
   author='Bengali.AI',
   author_email='research.bengaliai@gmail.com',
   license='MIT',
```

### Comparing `bnunicodenormalizer-0.1.6/tests/test_normalizer.py` & `bnunicodenormalizer-0.1.7/tests/test_normalizer.py`

 * *Files identical despite different names*

