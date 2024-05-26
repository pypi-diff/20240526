# Comparing `tmp/optframe-5.0.8rc0.tar.gz` & `tmp/optframe-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optframe-5.0.8rc0.tar", last modified: Tue Sep 27 01:39:16 2022, max compression
+gzip compressed data, was "optframe-5.1.0.tar", last modified: Sun May 26 14:39:17 2024, max compression
```

## Comparing `optframe-5.0.8rc0.tar` & `optframe-5.1.0.tar`

### file list

```diff
@@ -1,26 +1,35 @@
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       80 2021-08-20 01:21:08.000000 optframe-5.0.8rc0/.clang-format
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      162 2021-08-20 01:21:03.000000 optframe-5.0.8rc0/CPPLINT.cfg
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     1926 2022-09-26 19:09:24.000000 optframe-5.0.8rc0/LICENSE
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      150 2022-09-26 20:02:27.000000 optframe-5.0.8rc0/MANIFEST.in
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     7406 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/PKG-INFO
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4722 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/README.md
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      530 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/bumpver.toml
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/demo/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    13188 2022-09-26 18:41:40.000000 optframe-5.0.8rc0/demo/demo_kp.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    35796 2022-09-24 02:38:22.000000 optframe-5.0.8rc0/demo/draft_pyfcore.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      958 2022-09-26 23:03:20.000000 optframe-5.0.8rc0/makefile
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/optframe/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      216 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/optframe/__init__.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    23000 2022-09-26 23:53:01.000000 optframe-5.0.8rc0/optframe/engine.py
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)    52712 2022-09-26 23:47:58.000000 optframe-5.0.8rc0/optframe/optframe_lib.cpp
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4882 2022-09-26 23:46:59.000000 optframe-5.0.8rc0/optframe/optframe_lib.h
-drwxrwsr-x   0 imcoelho  (1000) imcoelho  (1000)        0 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/optframe.egg-info/
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     7406 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/PKG-INFO
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      388 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/SOURCES.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)        1 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/dependency_links.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       44 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/requires.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)        9 2022-09-27 01:39:16.000000 optframe-5.0.8rc0/optframe.egg-info/top_level.txt
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)      852 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/pyproject.toml
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)       38 2022-09-27 01:39:16.784005 optframe-5.0.8rc0/setup.cfg
--rw-rw-r--   0 imcoelho  (1000) imcoelho  (1000)     4618 2022-09-27 01:38:40.000000 optframe-5.0.8rc0/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-26 14:39:17.741406 optframe-5.1.0/
+-rw-rw-r--   0 root         (0) root         (0)       80 2022-12-07 00:43:54.000000 optframe-5.1.0/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-11-11 20:53:35.000000 optframe-5.1.0/COPYING.LESSERv3
+-rw-rw-r--   0 root         (0) root         (0)      162 2022-12-07 00:43:54.000000 optframe-5.1.0/CPPLINT.cfg
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-11-11 20:53:32.000000 optframe-5.1.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      150 2022-12-07 00:43:54.000000 optframe-5.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7130 2024-05-26 14:39:17.741406 optframe-5.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5170 2024-05-26 14:38:10.000000 optframe-5.1.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)      489 2024-05-26 14:38:10.000000 optframe-5.1.0/bumpver.toml
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-26 14:39:17.733406 optframe-5.1.0/demo/
+-rw-rw-r--   0 root         (0) root         (0)    22759 2023-06-22 18:22:25.000000 optframe-5.1.0/demo/demo_kp.py
+-rw-rw-r--   0 root         (0) root         (0)    16201 2023-06-13 21:52:35.000000 optframe-5.1.0/demo/demo_kp_tiny.py
+-rw-rw-r--   0 root         (0) root         (0)     3953 2023-06-13 21:46:27.000000 optframe-5.1.0/demo/demo_kp_tiny_sa.py
+-rw-rw-r--   0 root         (0) root         (0)    35796 2022-12-07 00:43:54.000000 optframe-5.1.0/demo/draft_pyfcore.py
+-rw-rw-r--   0 root         (0) root         (0)     3526 2023-12-07 19:30:46.000000 optframe-5.1.0/makefile
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-26 14:39:17.737406 optframe-5.1.0/optframe/
+-rw-rw-r--   0 root         (0) root         (0)      198 2024-05-26 14:38:10.000000 optframe-5.1.0/optframe/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5280 2023-06-14 23:14:54.000000 optframe-5.1.0/optframe/components.py
+-rw-rw-r--   0 root         (0) root         (0)     2799 2023-06-14 21:40:42.000000 optframe-5.1.0/optframe/core.py
+-rw-rw-r--   0 root         (0) root         (0)    44378 2023-12-07 19:35:57.000000 optframe-5.1.0/optframe/engine.py
+-rw-rw-r--   0 root         (0) root         (0)     9407 2024-05-26 14:34:33.000000 optframe-5.1.0/optframe/heuristics.py
+-rw-rw-r--   0 root         (0) root         (0)      179 2023-11-12 23:39:54.000000 optframe-5.1.0/optframe/optframe_lib.cpp
+-rw-rw-r--   0 root         (0) root         (0)      299 2023-11-12 23:38:55.000000 optframe-5.1.0/optframe/optframe_lib.h
+-rw-rw-r--   0 root         (0) root         (0)     3473 2023-12-07 18:27:39.000000 optframe-5.1.0/optframe/protocols.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-26 14:39:17.741406 optframe-5.1.0/optframe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7130 2024-05-26 14:39:17.000000 optframe-5.1.0/optframe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-26 14:39:17.000000 optframe-5.1.0/optframe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 14:39:17.000000 optframe-5.1.0/optframe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-26 14:39:17.000000 optframe-5.1.0/optframe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-26 14:39:17.000000 optframe-5.1.0/optframe.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      841 2024-05-26 14:38:10.000000 optframe-5.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 14:39:17.741406 optframe-5.1.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2781 2024-05-26 14:38:10.000000 optframe-5.1.0/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-26 14:39:17.741406 optframe-5.1.0/tests/
+-rw-rw-r--   0 root         (0) root         (0)     9005 2023-06-14 19:03:56.000000 optframe-5.1.0/tests/test_pkg_engine_kp.py
```

### Comparing `optframe-5.0.8rc0/PKG-INFO` & `optframe-5.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,118 @@
 Metadata-Version: 2.1
 Name: optframe
-Version: 5.0.8rc0
+Version: 5.1.0
 Summary: Python bindings for OptFrame Functional Core
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
-License: OptFrame Python - Optimization Framework
-        Copyright (C) 2009-2022 - MIT LICENSE
-        https://github.com/optframe/pyoptframe
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-        Or, at your choice...
-        
-        Copyright (C) 2009-2022 - LICENSE LGPLv3
-        
-        This file is part of the OptFrame optimization framework. This framework
-        is free software; you can redistribute it and/or modify it under the
-        terms of the GNU Lesser General Public License v3 as published by the
-        Free Software Foundation.
-        
-        This framework is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU Lesser General Public License v3 for more details.
-        
-        You should have received a copy of the GNU Lesser General Public License v3
-        along with this library; see the file COPYING.  If not, write to the Free
-        Software Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301,
-        USA.
+License: Copyright (c) 2023 OptFrame Developers
         
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 Project-URL: Homepage, https://github.com/optframe/pyoptframe
 Keywords: optframe,optimization,metaheuristics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+License-File: COPYING.LESSERv3
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
+# pyoptframe-dev
+
+[![Documentation Status](https://readthedocs.org/projects/optframe/badge/?version=latest)](https://pyoptframe.readthedocs.io/en/latest/?badge=latest)
+
+Development repo for draft versions of Python bindings for OptFrame Functional Core C++.
 
-# pyoptframe
-Python bindings for OptFrame Functional Core
 
 Install: `python -m pip install optframe`
 
-Version: `pyoptframe v5.0.8rc0`
+Version: `pyoptframe v5.1.0`
+
+Play on Jupyter Notebook: [BRKGA Traveling Salesman Problem Example](demo/OptFrame_BRKGA_Official.ipynb)
 
 Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
 
+Beware that, after officially launched, this project may be migrated into [Official Optframe C++](https://github.com/optframe/optframe) repo (and same strategy applies to other future external language bindings).
+
+### About OptFrame C++
+
 [OptFrame](https://github.com/optframe/optframe) is a C++ framework for optimization problems, including techniques such as classic metaheuristics Simulated Annealing, Genetic Algorithm, 
 Variable Neighborhood Search, Iterated Local Search, Tabu Search, Particle Swarm Optimization, NSGA-II, and other single and multi-objective methods.
-This is a 10-year project with several practical applications in industry and academia, so feel free to use it.
+This is a 10+ year project with several practical applications in industry and academia, so feel free to use it.
+
+## For Developers
 
-## How to test
+If you want to help, please see instructions on [Development.md](./Development.md).
 
-### With Package Manager
 
-`make install` or `pip install .`
+### Advice for online environments
 
-`make test`
+OptFrame now supports both `c++17` and `c++20`.
 
-### Without Package Manager (local only)
+Before installing optframe online (such as google colab), check C++ compiler (typically GCC) version:
 
+`x86_64-linux-gnu-gcc -v`
+
+At least gcc-10 is required for C++20... if not enough, try to install g++-10 and make it default.
+*Considering Jupyter notebook syntax*:
 ```
-make optframe_lib
-make demo_local
+!apt install -y g++-10
+!g++-10 --version
+!update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-10 10
+!update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-10 10
+!update-alternatives --install /usr/bin/x86_64-linux-gnu-gcc gcc /usr/bin/gcc-10 10
 ```
 
-
 ## Tutorials
 
-Please read the official tutorials for OptFrame C++: https://optframe.readthedocs.io/
+### Demos
+
+Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
+
+Please see the demos on demo/ folder.
 
-Tutorials specific for OptFrame Python is coming!
+We also include some jupyter notebooks for playing.
 
-### Example with 0-1 Knapsack Problem
 
-Please see file `tests/test_engine_kp.py` for an example with 0-1 Knapsack Problem.
+### Example with 0-1 Knapsack Problem (tests)
 
-## Technical discussions
+Also see file `tests/test_engine_kp.py` for an example with 0-1 Knapsack Problem,
+used on internal tests.
+
+### More tutorials
+
+Please read the official tutorials for OptFrame C++, 
+as they may give ideas for python too: https://optframe.readthedocs.io/
+
+Also see the Examples and demo folders on C++ project: [github.com/optframe/optframe](https://github.com/optframe/optframe).
+
+
+## Technical discussions and Roadmap
 ### C++ Standard and Compiler Support
 
 We love Concepts and Optionals, so we require `C++20` as default. 
 However, it is possible to adapt `setup.py` in order to allow for `C++17` with `-fconcepts` on GCC. 
 If necessary (only C++17 is available), add this line on `setup.py`:
 
 ```
@@ -118,84 +145,28 @@
 ### Versioning Strategy
 
 Versioning should follow OptFrame C++ project on MAJOR and MINOR, leaving PATCH field to be different, if necessary. Examples: 
 
 - v 5 dot 1 dot 3 should include OptFrame C++ 5 dot 1.
 - v 5 dot 4 dot 5 could include OptFrame C++ 5 dot 4 dot 8 OR 5 dot 4 dot 1, but NOT 5 dot 6 dot x.
 
-### Packaging instructions
-
-Edit `setup.py`.
-
-Edit `pyproject.toml`.
-
-`virtualenv venv`
-
-`source venv/bin/activate`
-
-`python -m pip install pip-tools`
-
-`pip-compile pyproject.toml`
-
-`pip-sync`
-
-For versioning:
-
-`python -m pip install bumpver`
-
-`bumpver init`
-
-**To increase PATCH number:**
-
-`bumpver update --patch`
-
-Test locally:
-
-`python -m pip install -e .`
-
-Build:
-
-`python -m pip install build twine`
-
-`python -m build`
-
-`twine check dist/*`
-
-`twine upload -r testpypi dist/* --verbose`
-
-Error: Binary wheel 'optframe-5.0.8rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
-
-Solution: `rm -f dist/*.whl`
-
-`twine upload -r testpypi dist/* --verbose`
-
-Test if OK on test package website:
-
-`python -m pip install -i https://test.pypi.org/simple optframe --upgrade`
-
-Finally:
-
-`twine upload dist/*`
-
-`python -m pip install optframe --upgrade`
-
-Thanks again to: https://realpython.com/pypi-publish-python-package/
-
-
 ## Known Issues
 
 All known issues fixed :)
 
 ## Thanks
 
 Thanks to the general help from Internet posts, this project could be packaged on Python (there are many links all around the source code mentioning the respective authors).
 
 Also thanks for the encouragement and fruitful discussions with my students, specially, Rafael Albuquerque, Marcos Souza, Victor Silva and Fellipe Pessanha.
 
 ## License
 
-MIT License || LGPLv3 License  (at your choice)
+At your choice:
+
+- [LICENSE-MIT](./LICENSE-MIT.txt)
+- [LICENSE-LGPLv3+](./LICENSE-LGPL-3.0-or-later.txt)
 
-Copyleft 2022
+Copyleft 2023
 
 Igor Machado Coelho
```

### Comparing `optframe-5.0.8rc0/README.md` & `optframe-5.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,78 @@
-# pyoptframe
-Python bindings for OptFrame Functional Core
+# pyoptframe-dev
+
+[![Documentation Status](https://readthedocs.org/projects/optframe/badge/?version=latest)](https://pyoptframe.readthedocs.io/en/latest/?badge=latest)
+
+Development repo for draft versions of Python bindings for OptFrame Functional Core C++.
+
 
 Install: `python -m pip install optframe`
 
-Version: `pyoptframe v5.0.8rc0`
+Version: `pyoptframe v5.1.0`
+
+Play on Jupyter Notebook: [BRKGA Traveling Salesman Problem Example](demo/OptFrame_BRKGA_Official.ipynb)
 
 Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
 
+Beware that, after officially launched, this project may be migrated into [Official Optframe C++](https://github.com/optframe/optframe) repo (and same strategy applies to other future external language bindings).
+
+### About OptFrame C++
+
 [OptFrame](https://github.com/optframe/optframe) is a C++ framework for optimization problems, including techniques such as classic metaheuristics Simulated Annealing, Genetic Algorithm, 
 Variable Neighborhood Search, Iterated Local Search, Tabu Search, Particle Swarm Optimization, NSGA-II, and other single and multi-objective methods.
-This is a 10-year project with several practical applications in industry and academia, so feel free to use it.
+This is a 10+ year project with several practical applications in industry and academia, so feel free to use it.
 
-## How to test
+## For Developers
 
-### With Package Manager
+If you want to help, please see instructions on [Development.md](./Development.md).
 
-`make install` or `pip install .`
 
-`make test`
+### Advice for online environments
 
-### Without Package Manager (local only)
+OptFrame now supports both `c++17` and `c++20`.
 
+Before installing optframe online (such as google colab), check C++ compiler (typically GCC) version:
+
+`x86_64-linux-gnu-gcc -v`
+
+At least gcc-10 is required for C++20... if not enough, try to install g++-10 and make it default.
+*Considering Jupyter notebook syntax*:
 ```
-make optframe_lib
-make demo_local
+!apt install -y g++-10
+!g++-10 --version
+!update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-10 10
+!update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-10 10
+!update-alternatives --install /usr/bin/x86_64-linux-gnu-gcc gcc /usr/bin/gcc-10 10
 ```
 
-
 ## Tutorials
 
-Please read the official tutorials for OptFrame C++: https://optframe.readthedocs.io/
+### Demos
+
+Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
+
+Please see the demos on demo/ folder.
 
-Tutorials specific for OptFrame Python is coming!
+We also include some jupyter notebooks for playing.
 
-### Example with 0-1 Knapsack Problem
 
-Please see file `tests/test_engine_kp.py` for an example with 0-1 Knapsack Problem.
+### Example with 0-1 Knapsack Problem (tests)
 
-## Technical discussions
+Also see file `tests/test_engine_kp.py` for an example with 0-1 Knapsack Problem,
+used on internal tests.
+
+### More tutorials
+
+Please read the official tutorials for OptFrame C++, 
+as they may give ideas for python too: https://optframe.readthedocs.io/
+
+Also see the Examples and demo folders on C++ project: [github.com/optframe/optframe](https://github.com/optframe/optframe).
+
+
+## Technical discussions and Roadmap
 ### C++ Standard and Compiler Support
 
 We love Concepts and Optionals, so we require `C++20` as default. 
 However, it is possible to adapt `setup.py` in order to allow for `C++17` with `-fconcepts` on GCC. 
 If necessary (only C++17 is available), add this line on `setup.py`:
 
 ```
@@ -74,84 +105,28 @@
 ### Versioning Strategy
 
 Versioning should follow OptFrame C++ project on MAJOR and MINOR, leaving PATCH field to be different, if necessary. Examples: 
 
 - v 5 dot 1 dot 3 should include OptFrame C++ 5 dot 1.
 - v 5 dot 4 dot 5 could include OptFrame C++ 5 dot 4 dot 8 OR 5 dot 4 dot 1, but NOT 5 dot 6 dot x.
 
-### Packaging instructions
-
-Edit `setup.py`.
-
-Edit `pyproject.toml`.
-
-`virtualenv venv`
-
-`source venv/bin/activate`
-
-`python -m pip install pip-tools`
-
-`pip-compile pyproject.toml`
-
-`pip-sync`
-
-For versioning:
-
-`python -m pip install bumpver`
-
-`bumpver init`
-
-**To increase PATCH number:**
-
-`bumpver update --patch`
-
-Test locally:
-
-`python -m pip install -e .`
-
-Build:
-
-`python -m pip install build twine`
-
-`python -m build`
-
-`twine check dist/*`
-
-`twine upload -r testpypi dist/* --verbose`
-
-Error: Binary wheel 'optframe-5.0.8rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
-
-Solution: `rm -f dist/*.whl`
-
-`twine upload -r testpypi dist/* --verbose`
-
-Test if OK on test package website:
-
-`python -m pip install -i https://test.pypi.org/simple optframe --upgrade`
-
-Finally:
-
-`twine upload dist/*`
-
-`python -m pip install optframe --upgrade`
-
-Thanks again to: https://realpython.com/pypi-publish-python-package/
-
-
 ## Known Issues
 
 All known issues fixed :)
 
 ## Thanks
 
 Thanks to the general help from Internet posts, this project could be packaged on Python (there are many links all around the source code mentioning the respective authors).
 
 Also thanks for the encouragement and fruitful discussions with my students, specially, Rafael Albuquerque, Marcos Souza, Victor Silva and Fellipe Pessanha.
 
 ## License
 
-MIT License || LGPLv3 License  (at your choice)
+At your choice:
+
+- [LICENSE-MIT](./LICENSE-MIT.txt)
+- [LICENSE-LGPLv3+](./LICENSE-LGPL-3.0-or-later.txt)
 
-Copyleft 2022
+Copyleft 2023
 
 Igor Machado Coelho
```

### Comparing `optframe-5.0.8rc0/demo/draft_pyfcore.py` & `optframe-5.1.0/demo/draft_pyfcore.py`

 * *Files identical despite different names*

### Comparing `optframe-5.0.8rc0/optframe.egg-info/PKG-INFO` & `optframe-5.1.0/optframe.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,118 @@
 Metadata-Version: 2.1
 Name: optframe
-Version: 5.0.8rc0
+Version: 5.1.0
 Summary: Python bindings for OptFrame Functional Core
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
-License: OptFrame Python - Optimization Framework
-        Copyright (C) 2009-2022 - MIT LICENSE
-        https://github.com/optframe/pyoptframe
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-        Or, at your choice...
-        
-        Copyright (C) 2009-2022 - LICENSE LGPLv3
-        
-        This file is part of the OptFrame optimization framework. This framework
-        is free software; you can redistribute it and/or modify it under the
-        terms of the GNU Lesser General Public License v3 as published by the
-        Free Software Foundation.
-        
-        This framework is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU Lesser General Public License v3 for more details.
-        
-        You should have received a copy of the GNU Lesser General Public License v3
-        along with this library; see the file COPYING.  If not, write to the Free
-        Software Foundation, 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301,
-        USA.
+License: Copyright (c) 2023 OptFrame Developers
         
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 Project-URL: Homepage, https://github.com/optframe/pyoptframe
 Keywords: optframe,optimization,metaheuristics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+License-File: COPYING.LESSERv3
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
+# pyoptframe-dev
+
+[![Documentation Status](https://readthedocs.org/projects/optframe/badge/?version=latest)](https://pyoptframe.readthedocs.io/en/latest/?badge=latest)
+
+Development repo for draft versions of Python bindings for OptFrame Functional Core C++.
 
-# pyoptframe
-Python bindings for OptFrame Functional Core
 
 Install: `python -m pip install optframe`
 
-Version: `pyoptframe v5.0.8rc0`
+Version: `pyoptframe v5.1.0`
+
+Play on Jupyter Notebook: [BRKGA Traveling Salesman Problem Example](demo/OptFrame_BRKGA_Official.ipynb)
 
 Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
 
+Beware that, after officially launched, this project may be migrated into [Official Optframe C++](https://github.com/optframe/optframe) repo (and same strategy applies to other future external language bindings).
+
+### About OptFrame C++
+
 [OptFrame](https://github.com/optframe/optframe) is a C++ framework for optimization problems, including techniques such as classic metaheuristics Simulated Annealing, Genetic Algorithm, 
 Variable Neighborhood Search, Iterated Local Search, Tabu Search, Particle Swarm Optimization, NSGA-II, and other single and multi-objective methods.
-This is a 10-year project with several practical applications in industry and academia, so feel free to use it.
+This is a 10+ year project with several practical applications in industry and academia, so feel free to use it.
+
+## For Developers
 
-## How to test
+If you want to help, please see instructions on [Development.md](./Development.md).
 
-### With Package Manager
 
-`make install` or `pip install .`
+### Advice for online environments
 
-`make test`
+OptFrame now supports both `c++17` and `c++20`.
 
-### Without Package Manager (local only)
+Before installing optframe online (such as google colab), check C++ compiler (typically GCC) version:
 
+`x86_64-linux-gnu-gcc -v`
+
+At least gcc-10 is required for C++20... if not enough, try to install g++-10 and make it default.
+*Considering Jupyter notebook syntax*:
 ```
-make optframe_lib
-make demo_local
+!apt install -y g++-10
+!g++-10 --version
+!update-alternatives --install /usr/bin/g++ g++ /usr/bin/g++-10 10
+!update-alternatives --install /usr/bin/gcc gcc /usr/bin/gcc-10 10
+!update-alternatives --install /usr/bin/x86_64-linux-gnu-gcc gcc /usr/bin/gcc-10 10
 ```
 
-
 ## Tutorials
 
-Please read the official tutorials for OptFrame C++: https://optframe.readthedocs.io/
+### Demos
+
+Documentation and Tutorials: see [PyOptFrame Quickstart](https://pyoptframe.readthedocs.io/en/latest/quickstart.html)
+
+Please see the demos on demo/ folder.
 
-Tutorials specific for OptFrame Python is coming!
+We also include some jupyter notebooks for playing.
 
-### Example with 0-1 Knapsack Problem
 
-Please see file `tests/test_engine_kp.py` for an example with 0-1 Knapsack Problem.
+### Example with 0-1 Knapsack Problem (tests)
 
-## Technical discussions
+Also see file `tests/test_engine_kp.py` for an example with 0-1 Knapsack Problem,
+used on internal tests.
+
+### More tutorials
+
+Please read the official tutorials for OptFrame C++, 
+as they may give ideas for python too: https://optframe.readthedocs.io/
+
+Also see the Examples and demo folders on C++ project: [github.com/optframe/optframe](https://github.com/optframe/optframe).
+
+
+## Technical discussions and Roadmap
 ### C++ Standard and Compiler Support
 
 We love Concepts and Optionals, so we require `C++20` as default. 
 However, it is possible to adapt `setup.py` in order to allow for `C++17` with `-fconcepts` on GCC. 
 If necessary (only C++17 is available), add this line on `setup.py`:
 
 ```
@@ -118,84 +145,28 @@
 ### Versioning Strategy
 
 Versioning should follow OptFrame C++ project on MAJOR and MINOR, leaving PATCH field to be different, if necessary. Examples: 
 
 - v 5 dot 1 dot 3 should include OptFrame C++ 5 dot 1.
 - v 5 dot 4 dot 5 could include OptFrame C++ 5 dot 4 dot 8 OR 5 dot 4 dot 1, but NOT 5 dot 6 dot x.
 
-### Packaging instructions
-
-Edit `setup.py`.
-
-Edit `pyproject.toml`.
-
-`virtualenv venv`
-
-`source venv/bin/activate`
-
-`python -m pip install pip-tools`
-
-`pip-compile pyproject.toml`
-
-`pip-sync`
-
-For versioning:
-
-`python -m pip install bumpver`
-
-`bumpver init`
-
-**To increase PATCH number:**
-
-`bumpver update --patch`
-
-Test locally:
-
-`python -m pip install -e .`
-
-Build:
-
-`python -m pip install build twine`
-
-`python -m build`
-
-`twine check dist/*`
-
-`twine upload -r testpypi dist/* --verbose`
-
-Error: Binary wheel 'optframe-5.0.8rc0-cp39-cp39-linux_x86_64.whl' has an unsupported platform tag 'linux_x86_64'. See [1](https://stackoverflow.com/questions/59451069/binary-wheel-cant-be-uploaded-on-pypi-using-twine) and [2](https://peps.python.org/pep-0513/#rationale).
-
-Solution: `rm -f dist/*.whl`
-
-`twine upload -r testpypi dist/* --verbose`
-
-Test if OK on test package website:
-
-`python -m pip install -i https://test.pypi.org/simple optframe --upgrade`
-
-Finally:
-
-`twine upload dist/*`
-
-`python -m pip install optframe --upgrade`
-
-Thanks again to: https://realpython.com/pypi-publish-python-package/
-
-
 ## Known Issues
 
 All known issues fixed :)
 
 ## Thanks
 
 Thanks to the general help from Internet posts, this project could be packaged on Python (there are many links all around the source code mentioning the respective authors).
 
 Also thanks for the encouragement and fruitful discussions with my students, specially, Rafael Albuquerque, Marcos Souza, Victor Silva and Fellipe Pessanha.
 
 ## License
 
-MIT License || LGPLv3 License  (at your choice)
+At your choice:
+
+- [LICENSE-MIT](./LICENSE-MIT.txt)
+- [LICENSE-LGPLv3+](./LICENSE-LGPL-3.0-or-later.txt)
 
-Copyleft 2022
+Copyleft 2023
 
 Igor Machado Coelho
```

### Comparing `optframe-5.0.8rc0/pyproject.toml` & `optframe-5.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # pyproject.toml
 # some advices from: https://realpython.com/pypi-publish-python-package/
 
 [build-system]
-requires = ["setuptools>=53.0.0", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optframe"
-version = "5.0.8rc0"
+version = "5.1.0"
 description = "Python bindings for OptFrame Functional Core"
 readme = "README.md"
 authors = [{ name = "Igor Machado Coelho", email = "igormcoelho@proton.me" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

