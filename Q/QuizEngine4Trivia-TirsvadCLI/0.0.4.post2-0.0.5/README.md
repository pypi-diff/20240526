# Comparing `tmp/quizengine4trivia_tirsvadcli-0.0.4.post2.tar.gz` & `tmp/quizengine4trivia_tirsvadcli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quizengine4trivia_tirsvadcli-0.0.4.post2.tar", last modified: Wed May 22 15:46:53 2024, max compression
+gzip compressed data, was "quizengine4trivia_tirsvadcli-0.0.5.tar", last modified: Sun May 26 03:28:30 2024, max compression
```

## Comparing `quizengine4trivia_tirsvadcli-0.0.4.post2.tar` & `quizengine4trivia_tirsvadcli-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.251620 quizengine4trivia_tirsvadcli-0.0.4.post2/
--rw-rw-rw-   0        0        0    35823 2024-05-20 12:50:09.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/LICENSE
--rw-rw-rw-   0        0        0       62 2024-05-21 10:57:47.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/MANIFEST.in
--rw-rw-rw-   0        0        0    46503 2024-05-22 15:46:53.251620 quizengine4trivia_tirsvadcli-0.0.4.post2/PKG-INFO
--rw-rw-rw-   0        0        0     4504 2024-05-21 16:51:16.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/README.md
--rw-rw-rw-   0        0        0     1034 2024-05-22 15:46:34.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/pyproject.toml
--rw-rw-rw-   0        0        0       17 2024-05-22 15:43:49.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 15:46:53.251620 quizengine4trivia_tirsvadcli-0.0.4.post2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.126655 quizengine4trivia_tirsvadcli-0.0.4.post2/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.157894 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/
--rw-rw-rw-   0        0        0     1648 2024-05-22 14:35:07.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.157894 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/models/
--rw-rw-rw-   0        0        0     3553 2024-05-22 14:35:07.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.173517 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/
--rw-rw-rw-   0        0        0     4972 2024-05-21 11:35:07.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-21 11:10:25.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 11:35:07.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 11:35:07.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-21 11:35:07.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.235994 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/
--rw-rw-rw-   0        0        0    46503 2024-05-22 15:46:53.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1113 2024-05-22 15:46:53.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 15:46:53.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-22 15:46:53.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-22 15:46:53.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.235994 quizengine4trivia_tirsvadcli-0.0.4.post2/src/tirsvadCLI_quiz_engine_4_trivia.egg-info/
--rw-rw-rw-   0        0        0     4956 2024-05-21 12:14:06.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/tirsvadCLI_quiz_engine_4_trivia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      967 2024-05-21 12:14:06.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/tirsvadCLI_quiz_engine_4_trivia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:14:06.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/tirsvadCLI_quiz_engine_4_trivia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 12:14:06.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/tirsvadCLI_quiz_engine_4_trivia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-21 12:14:06.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/src/tirsvadCLI_quiz_engine_4_trivia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 15:46:53.235994 quizengine4trivia_tirsvadcli-0.0.4.post2/tests/
--rw-rw-rw-   0        0        0      534 2024-05-22 14:41:22.000000 quizengine4trivia_tirsvadcli-0.0.4.post2/tests/test_class.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.870794 quizengine4trivia_tirsvadcli-0.0.5/
+-rw-rw-rw-   0        0        0    35823 2024-05-20 12:50:09.000000 quizengine4trivia_tirsvadcli-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       62 2024-05-21 10:57:47.000000 quizengine4trivia_tirsvadcli-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    46992 2024-05-26 03:28:30.855168 quizengine4trivia_tirsvadcli-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4999 2024-05-26 03:24:55.000000 quizengine4trivia_tirsvadcli-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1771 2024-05-25 16:30:27.000000 quizengine4trivia_tirsvadcli-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2024-05-22 15:43:49.000000 quizengine4trivia_tirsvadcli-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 03:28:30.870794 quizengine4trivia_tirsvadcli-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.823926 quizengine4trivia_tirsvadcli-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.823926 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/
+-rw-rw-rw-   0        0        0     2011 2024-05-25 15:22:04.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.823926 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/models/
+-rw-rw-rw-   0        0        0     3401 2024-05-25 15:37:25.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.855168 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/
+-rw-rw-rw-   0        0        0    46992 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-26 03:28:30.000000 quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 03:28:30.855168 quizengine4trivia_tirsvadcli-0.0.5/tests/
+-rw-rw-rw-   0        0        0     2698 2024-05-26 02:30:55.000000 quizengine4trivia_tirsvadcli-0.0.5/tests/test_quiz_engine.py
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.4.post2/LICENSE` & `quizengine4trivia_tirsvadcli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quizengine4trivia_tirsvadcli-0.0.4.post2/PKG-INFO` & `quizengine4trivia_tirsvadcli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuizEngine4Trivia-TirsvadCLI
-Version: 0.0.4.post2
+Version: 0.0.5
 Summary: Question Engine for Trivia Queston DB
 Author: Jens Tirsvad Nielsen
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,17 +694,21 @@
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
-<a href='https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia'>
-    <img src='https://coveralls.io/repos/github/TirsvadCLI/Python.QuizEngine4Trivia/badge.svg' alt='Coverage Status' height="28"/>
-</a>
+
+[![PyPi][pypi-shield]][pypi-url]
+[![Coveralls][coveralls-shield]][coverall-url]
+![PyPiPythonVer][pypipyver-shield]
+
+
+
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
     <br />
     <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/">
         <img src="images/logo.png" alt="Logo" width="80" height="80">
     </a>
@@ -748,26 +752,38 @@
 
 In a terminal do following
 ```commandline
 pip install tirsvadCLI-quiz_engine_4_trivia
 ```
 
 ```python
-from main import QuizEngine
+from QuizEngine4Trivia import QuizEngine
+import html
 
 quiz = QuizEngine()
 
 while quiz.still_has_questions():
-    print(f"Your score : {quiz.score}")
-    q_text = quiz.next_question()
-    user_answer = input(f"Q.{quiz.question_number}: {q_text}")
-    if quiz.check_answer(user_answer):
-        print("You are right")
-    else:
-        print("You are wrong")
+    print(f"Your score : {quiz.score}\n\n")
+    current = quiz.next_question()
+    print({html.unescape(current.question)})
+
+    count = 0
+    for possible_answer in current.possible_answers:
+        print(f"{count}: {html.unescape(possible_answer)}")
+        count += 1
+
+    user_answer = int(input("Answer .:"))
+    if 0 <= user_answer <= count:
+        if quiz.check_answer(current.possible_answers[user_answer]):
+            print("You are right")
+        else:
+            print("You are wrong")
+
+print("You've completed the quiz")
+print(f"Your final score was: {quiz.score}/{quiz.question_number}")
 ```
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are greatly appreciated.
 
@@ -791,30 +807,32 @@
 git commit -m 'Add my feature enhance to project'
 git push origin feature
 ```
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
-[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [contributors-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors
 
-[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/members
 
-[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
+[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/stargazers
 
-[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
+[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [issues-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues
 
-[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
+[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [license-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE
 
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
 
+[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia
+
+[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypi-url]: https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/
 
-[coveralls-shield]: https://coveralls.io/repos/github/TirsvadCLI/Python.QuizEngine4Trivia/badge.svg?branch=main
-[coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia?branch=main
+[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia/tirsvadCLI_quiz_engine_4_trivia.egg-info/PKG-INFO` & `quizengine4trivia_tirsvadcli-0.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,24 @@
-Metadata-Version: 2.1
-Name: tirsvadCLI-quiz-engine-4-trivia
-Version: 0.0.2.post11
-Home-page: https://github.com/TirsvadCLI
-Download-URL: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/releases/download/v0.0.1a2/tirsvadcli_quiz_engine_4_trivia-0.0.1a2.tar.gz
-Author: Jens Tirsvad Nielsen
-Author-email: jenstirsvad@gmail.com
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Environment :: Console
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
-<!-- REPLACE -->
+
+[![PyPi][pypi-shield]][pypi-url]
+[![Coveralls][coveralls-shield]][coverall-url]
+![PyPiPythonVer][pypipyver-shield]
+
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
+    <br />
     <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/">
         <img src="images/logo.png" alt="Logo" width="80" height="80">
     </a>
     <h3 align="center">Quiz Engine for Trivia</h3>
     <p align="center">
     <!-- PROJECT DESCRIPTION -->
     <br />
@@ -40,19 +26,19 @@
     <!-- PROJECT SCREENSHOTS -->
     <!--
     <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/main/images/screenshot01.png">
         <img src="images/screenshot01.png" alt="screenshot" width="120" height="120">
     </a>
     -->
     <br />
-    <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia"><strong>Explore the docs Â»</strong></a>
+    <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia"><strong>Explore the docs »</strong></a>
     <br />
     <br />
     <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
-    Â·
+    ·
     <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
 
   </p>
 </div>
 
 # Quiz Engine for Trivia
 
@@ -71,28 +57,39 @@
 ## Use
 
 In a terminal do following
 ```commandline
 pip install tirsvadCLI-quiz_engine_4_trivia
 ```
 
-
 ```python
-from quiz_engine import QuizEngine
+from QuizEngine4Trivia import QuizEngine
+import html
 
 quiz = QuizEngine()
 
 while quiz.still_has_questions():
-    print(f"Your score : {quiz.score}")
-    q_text = quiz.next_question()
-    user_answer = input(f"Q.{quiz.question_number}: {q_text}")
-    if quiz.check_answer(user_answer):
-        print("You are right")
-    else:
-        print("You are wrong")
+    print(f"Your score : {quiz.score}\n\n")
+    current = quiz.next_question()
+    print({html.unescape(current.question)})
+
+    count = 0
+    for possible_answer in current.possible_answers:
+        print(f"{count}: {html.unescape(possible_answer)}")
+        count += 1
+
+    user_answer = int(input("Answer .:"))
+    if 0 <= user_answer <= count:
+        if quiz.check_answer(current.possible_answers[user_answer]):
+            print("You are right")
+        else:
+            print("You are wrong")
+
+print("You've completed the quiz")
+print(f"Your final score was: {quiz.score}/{quiz.question_number}")
 ```
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are greatly appreciated.
 
@@ -116,30 +113,32 @@
 git commit -m 'Add my feature enhance to project'
 git push origin feature
 ```
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
-[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [contributors-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors
 
-[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/members
 
-[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/stargazers
 
-[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [issues-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues
 
-[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [license-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE
 
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
-
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
+
+[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia
+
+[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypi-url]: https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/
+
+[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
```

#### html2text {}

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.1 Name: tirsvadCLI-quiz-engine-4-trivia Version:
-0.0.2.post11 Home-page: https://github.com/TirsvadCLI Download-URL: https://
-github.com/TirsvadCLI/Python.QuizEngine4Trivia/releases/download/v0.0.1a2/
-tirsvadcli_quiz_engine_4_trivia-0.0.1a2.tar.gz Author: Jens Tirsvad Nielsen
-Author-email: jenstirsvad@gmail.com Classifier: License :: OSI Approved :: GNU
-Affero General Public License v3 or later (AGPLv3+) Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Environment ::
-Console Classifier: Operating System :: POSIX :: Linux Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests [![Contributors][contributors-shield]][contributors-url] [![Forks]
-[forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues]
-[issues-shield]][issues-url] [![MIT License][license-shield]][license-url] [!
-[LinkedIn][linkedin-shield]][linkedin-url]
+[![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
+shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [![Issues][issues-
+shield]][issues-url] [![MIT License][license-shield]][license-url] [![LinkedIn]
+[linkedin-shield]][linkedin-url] [![PyPi][pypi-shield]][pypi-url] [![Coveralls]
+[coveralls-shield]][coverall-url] ![PyPiPythonVer][pypipyver-shield]
+
                                     _[_L_o_g_o_]
                        ******** QQuuiizz EEnnggiinnee ffoorr TTrriivviiaa ********
 
 
 
-                            _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Ã_?_?Â_?»
+                             _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
-                        _R_e_p_o_r_t_ _B_u_g ÃÂ· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
+                         _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # Quiz Engine for Trivia # Getting Started Quiz Engine for Trivia module Easy
 to create a quiz game by using this module. ## Prerequisites You have python 3
 installed. ## Use In a terminal do following ```commandline pip install
-tirsvadCLI-quiz_engine_4_trivia ``` ```python from quiz_engine import
-QuizEngine quiz = QuizEngine() while quiz.still_has_questions(): print(f"Your
-score : {quiz.score}") q_text = quiz.next_question() user_answer = input(f"Q.
-{quiz.question_number}: {q_text}") if quiz.check_answer(user_answer): print
-("You are right") else: print("You are wrong") ``` ## Contributing
-Contributions are what make the open source community such an amazing place to
-learn, inspire, and create. Any contributions you make are greatly appreciated.
-If you have a suggestion that would make this better, please fork the repo and
-create a pull request. You can also simply open an issue with the tag
-"enhancement". Don't forget to give the project a star! Thanks again! Fork the
-Project
+tirsvadCLI-quiz_engine_4_trivia ``` ```python from QuizEngine4Trivia import
+QuizEngine import html quiz = QuizEngine() while quiz.still_has_questions():
+print(f"Your score : {quiz.score}\n\n") current = quiz.next_question() print(
+{html.unescape(current.question)}) count = 0 for possible_answer in
+current.possible_answers: print(f"{count}: {html.unescape(possible_answer)}")
+count += 1 user_answer = int(input("Answer .:")) if 0 <= user_answer <= count:
+if quiz.check_answer(current.possible_answers[user_answer]): print("You are
+right") else: print("You are wrong") print("You've completed the quiz") print
+(f"Your final score was: {quiz.score}/{quiz.question_number}") ``` ##
+Contributing Contributions are what make the open source community such an
+amazing place to learn, inspire, and create. Any contributions you make are
+greatly appreciated. If you have a suggestion that would make this better,
+please fork the repo and create a pull request. You can also simply open an
+issue with the tag "enhancement". Don't forget to give the project a star!
+Thanks again! Fork the Project
    1. Fork the Project
    2. Create your Feature Branch
    3. Commit your Changes
    4. Push to the Branch
    5. Open a Pull Request
 Example ```commandline git checkout -b feature git commit -m 'Add my feature
 enhance to project' git push origin feature ``` [contributors-shield]: https://
 img.shields.io/github/contributors/TirsvadCLI/
-Python.QuizEngine4Trivia?style=for-the-badge [contributors-url]: https://
-github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors [forks-
-shield]: https://img.shields.io/github/forks/TirsvadCLI/
-Python.QuizEngine4Trivia?style=for-the-badge [forks-url]: https://github.com/
-TirsvadCLI/Python.QuizEngine4Trivia/network/members [stars-shield]: https://
-img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-
-badge [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/
-stargazers [issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/
-Python.QuizEngine4Trivia?style=for-the-badge [issues-url]: https://github.com/
-TirsvadCLI/Python.QuizEngine4Trivia/issues [license-shield]: https://
-img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-
-the-badge [license-url]: https://github.com/TirsvadCLI/
-Python.QuizEngine4Trivia/blob/master/LICENSE [linkedin-shield]: https://
-img.shields.io/badge/-LinkedIn-black.svg?style=for-the-
-badge&logo=linkedin&colorB=555 [linkedin-url]: https://www.linkedin.com/in/
-jens-tirsvad-nielsen-13b795b9/
+Python.QuizEngine4Trivia?style=flat [contributors-url]: https://github.com/
+TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors [forks-shield]: https:/
+/img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/
+members [stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/
+Python.QuizEngine4Trivia?style=flat [stars-url]: https://github.com/TirsvadCLI/
+Python.QuizEngine4Trivia/stargazers [issues-shield]: https://img.shields.io/
+github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat [issues-url]:
+https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues [license-shield]:
+https://img.shields.io/github/license/TirsvadCLI/
+Python.QuizEngine4Trivia?style=flat [license-url]: https://github.com/
+TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE [linkedin-shield]:
+https://img.shields.io/badge/-LinkedIn-
+black.svg?style=flat&logo=linkedin&colorB=555 [linkedin-url]: https://
+www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/ [coveralls-shield]: https://
+img.shields.io/coverallsCoverage/github/TirsvadCLI/
+Python.QuizEngine4Trivia?style=flat [coverall-url]: https://coveralls.io/
+github/TirsvadCLI/Python.QuizEngine4Trivia [pypi-shield]: https://
+img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat [pypi-url]:
+https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/ [pypipyver-shield]:
+https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
```

### Comparing `quizengine4trivia_tirsvadcli-0.0.4.post2/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO` & `quizengine4trivia_tirsvadcli-0.0.5/src/QuizEngine4Trivia_TirsvadCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuizEngine4Trivia-TirsvadCLI
-Version: 0.0.4.post2
+Version: 0.0.5
 Summary: Question Engine for Trivia Queston DB
 Author: Jens Tirsvad Nielsen
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,17 +694,21 @@
 
 [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url]
 [![Stargazers][stars-shield]][stars-url]
 [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
 [![LinkedIn][linkedin-shield]][linkedin-url]
-<a href='https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia'>
-    <img src='https://coveralls.io/repos/github/TirsvadCLI/Python.QuizEngine4Trivia/badge.svg' alt='Coverage Status' height="28"/>
-</a>
+
+[![PyPi][pypi-shield]][pypi-url]
+[![Coveralls][coveralls-shield]][coverall-url]
+![PyPiPythonVer][pypipyver-shield]
+
+
+
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
     <br />
     <a href="https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/">
         <img src="images/logo.png" alt="Logo" width="80" height="80">
     </a>
@@ -748,26 +752,38 @@
 
 In a terminal do following
 ```commandline
 pip install tirsvadCLI-quiz_engine_4_trivia
 ```
 
 ```python
-from main import QuizEngine
+from QuizEngine4Trivia import QuizEngine
+import html
 
 quiz = QuizEngine()
 
 while quiz.still_has_questions():
-    print(f"Your score : {quiz.score}")
-    q_text = quiz.next_question()
-    user_answer = input(f"Q.{quiz.question_number}: {q_text}")
-    if quiz.check_answer(user_answer):
-        print("You are right")
-    else:
-        print("You are wrong")
+    print(f"Your score : {quiz.score}\n\n")
+    current = quiz.next_question()
+    print({html.unescape(current.question)})
+
+    count = 0
+    for possible_answer in current.possible_answers:
+        print(f"{count}: {html.unescape(possible_answer)}")
+        count += 1
+
+    user_answer = int(input("Answer .:"))
+    if 0 <= user_answer <= count:
+        if quiz.check_answer(current.possible_answers[user_answer]):
+            print("You are right")
+        else:
+            print("You are wrong")
+
+print("You've completed the quiz")
+print(f"Your final score was: {quiz.score}/{quiz.question_number}")
 ```
 
 ## Contributing
 
 Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any
 contributions you make are greatly appreciated.
 
@@ -791,30 +807,32 @@
 git commit -m 'Add my feature enhance to project'
 git push origin feature
 ```
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 
-[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[contributors-shield]: https://img.shields.io/github/contributors/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [contributors-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/graphs/contributors
 
-[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
-
+[forks-shield]: https://img.shields.io/github/forks/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [forks-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/network/members
 
-[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
+[stars-shield]: https://img.shields.io/github/stars/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [stars-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/stargazers
 
-[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
+[issues-shield]: https://img.shields.io/github/issues/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [issues-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/issues
 
-[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=for-the-badge
+[license-shield]: https://img.shields.io/github/license/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
 [license-url]: https://github.com/TirsvadCLI/Python.QuizEngine4Trivia/blob/master/LICENSE
 
-[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
+[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat&logo=linkedin&colorB=555
 [linkedin-url]: https://www.linkedin.com/in/jens-tirsvad-nielsen-13b795b9/
 
+[coveralls-shield]: https://img.shields.io/coverallsCoverage/github/TirsvadCLI/Python.QuizEngine4Trivia?style=flat
+[coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia
+
+[pypi-shield]: https://img.shields.io/pypi/v/QuizEngine4Trivia-TirsvadCLI?style=flat
+[pypi-url]: https://pypi.org/project/QuizEngine4Trivia-TirsvadCLI/
 
-[coveralls-shield]: https://coveralls.io/repos/github/TirsvadCLI/Python.QuizEngine4Trivia/badge.svg?branch=main
-[coverall-url]: https://coveralls.io/github/TirsvadCLI/Python.QuizEngine4Trivia?branch=main
+[pypipyver-shield]: https://img.shields.io/pypi/pyversions/QuizEngine4Trivia-TirsvadCLI?style=flat
```

