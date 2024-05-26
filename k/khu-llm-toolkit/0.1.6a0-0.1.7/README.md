# Comparing `tmp/khu_llm_toolkit-0.1.6a0.tar.gz` & `tmp/khu_llm_toolkit-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khu_llm_toolkit-0.1.6a0.tar", max compression
+gzip compressed data, was "khu_llm_toolkit-0.1.7.tar", max compression
```

## Comparing `khu_llm_toolkit-0.1.6a0.tar` & `khu_llm_toolkit-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-09-22 05:27:45.226670 khu_llm_toolkit-0.1.6a0/LICENSE
--rw-r--r--   0        0        0     1063 2023-09-22 05:27:45.226670 khu_llm_toolkit-0.1.6a0/LICENSE.txt
--rw-r--r--   0        0        0     7469 2024-02-19 07:18:09.718936 khu_llm_toolkit-0.1.6a0/README.md
--rw-r--r--   0        0        0       61 2024-02-19 07:02:56.715927 khu_llm_toolkit-0.1.6a0/khu_llm_toolkit/__init__.py
--rw-r--r--   0        0        0       92 2024-02-01 02:04:07.123996 khu_llm_toolkit-0.1.6a0/khu_llm_toolkit/commons.py
--rw-r--r--   0        0        0      354 2024-02-01 02:04:07.123996 khu_llm_toolkit-0.1.6a0/khu_llm_toolkit/config.ini
--rw-r--r--   0        0        0     3038 2024-02-19 07:03:47.185873 khu_llm_toolkit-0.1.6a0/khu_llm_toolkit/model_definition.py
--rw-r--r--   0        0        0      417 2024-02-19 07:19:15.296282 khu_llm_toolkit-0.1.6a0/pyproject.toml
--rw-r--r--   0        0        0     8041 1970-01-01 00:00:00.000000 khu_llm_toolkit-0.1.6a0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-01-05 11:30:51.182033 khu_llm_toolkit-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1063 2024-01-05 11:30:51.182033 khu_llm_toolkit-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     7411 2024-05-26 08:20:56.782806 khu_llm_toolkit-0.1.7/README.md
+-rw-r--r--   0        0        0       61 2024-05-25 03:57:28.662960 khu_llm_toolkit-0.1.7/khu_llm_toolkit/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-25 07:43:36.908081 khu_llm_toolkit-0.1.7/khu_llm_toolkit/commons.py
+-rw-r--r--   0        0        0      692 2024-05-25 11:00:57.427394 khu_llm_toolkit-0.1.7/khu_llm_toolkit/config.ini.sample
+-rw-r--r--   0        0        0     5000 2024-05-25 10:56:43.745945 khu_llm_toolkit-0.1.7/khu_llm_toolkit/model_definition.py
+-rw-r--r--   0        0        0      449 2024-05-25 08:47:53.202276 khu_llm_toolkit-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     8085 1970-01-01 00:00:00.000000 khu_llm_toolkit-0.1.7/PKG-INFO
```

### Comparing `khu_llm_toolkit-0.1.6a0/LICENSE` & `khu_llm_toolkit-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `khu_llm_toolkit-0.1.6a0/LICENSE.txt` & `khu_llm_toolkit-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `khu_llm_toolkit-0.1.6a0/README.md` & `khu_llm_toolkit-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -70,97 +70,89 @@
   ```shell
   curl -sSL https://install.python-poetry.org | python3 -
   ```
 
 * Virtual environment
 
   ```
-  python3 -m venv .venv
-  source .venv/bin/activate
-  pip install -r requirements.txt
-  ```  
-
-  或 使用 poetry:
-
-  ```
   poetry install
   poetry shell
   ```
 
 ### Development
 
 see [How to upload your python package to PyPi](https://medium.com/@joel.barmettler/how-to-upload-your-python-package-to-pypi-65edc5fe9c56)
 
-#### Without Poetry
+#### 使用 Poetry
 
 * Virtual environment
 
   ```
-  source .venv/bin/activate
+  poetry shell
   ```
 
 * Test
 
     ```
     pytest 
     ```
 
-* Github Release
-
-  建立並發布git tag
-
-  ```
-  git tag -a 0.1.1 -m "adjust config file content layout"
-  git push origin 0.1.1
-  ```
-
-  然後到Github倉庫頁面建立一個新的release
-
-  複製Assets中Source code(.tar.gz)的URL, 把它貼到setup.py裡的download_url中
-
 * Build
 
   ```
-  python3 setup.py sdist
-  python3 setup.py clean --all
+  poetry build
   ```
 
 * Upload
 
-  PyPi不再允許在上傳過程中用個人帳號密碼做為身份驗證方式, 參考[Hackmd記錄](https://hackmd.io/4zug-RFaS362quf2Qfj2CA#2023-09-21)。
-  在上傳過程中要求認證的時候, 以"__token__"做為username, 以該檔案中的token值做為密碼 
-
   ```
-  twine upload dist/*
+  poetry publish --username=__token__ --password=pypi token值
   ```
 
-#### With Poetry
+#### 手動執行 setuptools
 
 * Virtual environment
 
   ```
-  poetry shell
+  source .venv/bin/activate
   ```
 
 * Test
 
     ```
     pytest 
     ```
 
+* Github Release
+
+  建立並發布git tag
+
+  ```
+  git tag -a 0.1.1 -m "adjust config file content layout"
+  git push origin 0.1.1
+  ```
+
+  然後到Github倉庫頁面建立一個新的release
+
+  複製Assets中Source code(.tar.gz)的URL, 把它貼到setup.py裡的download_url中
+
 * Build
 
   ```
-  poetry build
+  python3 setup.py sdist
+  python3 setup.py clean --all
   ```
 
 * Upload
 
+  PyPi不再允許在上傳過程中用個人帳號密碼做為身份驗證方式, 參考[Hackmd記錄](https://hackmd.io/4zug-RFaS362quf2Qfj2CA#2023-09-21)。
+  在上傳過程中要求認證的時候, 以"__token__"做為username, 以該檔案中的token值做為密碼 
+
   ```
-  poetry publish --username=__token__ --password=上述檔案中的token值
+  twine upload dist/*
   ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 完成建置並推送到PyPi server後, 就可以在其它專案中將它設為相依套件, 並在程式碼中使用.
 
@@ -208,15 +200,16 @@
 COMPLETIONS_MODEL = gpt-35-turbo
 EMBEDDINGS_MODEL = text-embedding-ada-002
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] 支援 Gemini
+- [x] 支援 Gemini (0.1.7 2024-04-25)
+- [x] 一設定檔,多模型 (0.1.7 2024-04-25)
 - [ ] 支援 Huggingface上的開源模型
 
 See the [open issues](https://github.com/kenhutaiwan/MyLlmUtils/issues) for a full list of proposed features (and known issues).
 
 <!-- LICENSE -->
 ## License
```

### Comparing `khu_llm_toolkit-0.1.6a0/PKG-INFO` & `khu_llm_toolkit-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: khu-llm-toolkit
-Version: 0.1.6a0
+Version: 0.1.7
 Summary: 
 Author: Ken Hu
 Author-email: ken.hu@hwacom.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.1.4,<0.2.0)
-Requires-Dist: langchain-community (>=0.0.16,<0.0.17)
-Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: langchain (>=0.2.1,<0.3.0)
+Requires-Dist: langchain-community (>=0.2.1,<0.3.0)
+Requires-Dist: langchain-google-genai (>=1.0.5,<2.0.0)
+Requires-Dist: langchain-openai (>=0.1.7,<0.2.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Description-Content-Type: text/markdown
 
 <!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
 <a name="readme-top"></a>
 <!--
 *** Thanks for checking out the Best-README-Template. If you have a suggestion
@@ -87,97 +89,89 @@
   ```shell
   curl -sSL https://install.python-poetry.org | python3 -
   ```
 
 * Virtual environment
 
   ```
-  python3 -m venv .venv
-  source .venv/bin/activate
-  pip install -r requirements.txt
-  ```  
-
-  或 使用 poetry:
-
-  ```
   poetry install
   poetry shell
   ```
 
 ### Development
 
 see [How to upload your python package to PyPi](https://medium.com/@joel.barmettler/how-to-upload-your-python-package-to-pypi-65edc5fe9c56)
 
-#### Without Poetry
+#### 使用 Poetry
 
 * Virtual environment
 
   ```
-  source .venv/bin/activate
+  poetry shell
   ```
 
 * Test
 
     ```
     pytest 
     ```
 
-* Github Release
-
-  建立並發布git tag
-
-  ```
-  git tag -a 0.1.1 -m "adjust config file content layout"
-  git push origin 0.1.1
-  ```
-
-  然後到Github倉庫頁面建立一個新的release
-
-  複製Assets中Source code(.tar.gz)的URL, 把它貼到setup.py裡的download_url中
-
 * Build
 
   ```
-  python3 setup.py sdist
-  python3 setup.py clean --all
+  poetry build
   ```
 
 * Upload
 
-  PyPi不再允許在上傳過程中用個人帳號密碼做為身份驗證方式, 參考[Hackmd記錄](https://hackmd.io/4zug-RFaS362quf2Qfj2CA#2023-09-21)。
-  在上傳過程中要求認證的時候, 以"__token__"做為username, 以該檔案中的token值做為密碼 
-
   ```
-  twine upload dist/*
+  poetry publish --username=__token__ --password=pypi token值
   ```
 
-#### With Poetry
+#### 手動執行 setuptools
 
 * Virtual environment
 
   ```
-  poetry shell
+  source .venv/bin/activate
   ```
 
 * Test
 
     ```
     pytest 
     ```
 
+* Github Release
+
+  建立並發布git tag
+
+  ```
+  git tag -a 0.1.1 -m "adjust config file content layout"
+  git push origin 0.1.1
+  ```
+
+  然後到Github倉庫頁面建立一個新的release
+
+  複製Assets中Source code(.tar.gz)的URL, 把它貼到setup.py裡的download_url中
+
 * Build
 
   ```
-  poetry build
+  python3 setup.py sdist
+  python3 setup.py clean --all
   ```
 
 * Upload
 
+  PyPi不再允許在上傳過程中用個人帳號密碼做為身份驗證方式, 參考[Hackmd記錄](https://hackmd.io/4zug-RFaS362quf2Qfj2CA#2023-09-21)。
+  在上傳過程中要求認證的時候, 以"__token__"做為username, 以該檔案中的token值做為密碼 
+
   ```
-  poetry publish --username=__token__ --password=上述檔案中的token值
+  twine upload dist/*
   ```
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 完成建置並推送到PyPi server後, 就可以在其它專案中將它設為相依套件, 並在程式碼中使用.
 
@@ -225,15 +219,16 @@
 COMPLETIONS_MODEL = gpt-35-turbo
 EMBEDDINGS_MODEL = text-embedding-ada-002
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
-- [ ] 支援 Gemini
+- [x] 支援 Gemini (0.1.7 2024-04-25)
+- [x] 一設定檔,多模型 (0.1.7 2024-04-25)
 - [ ] 支援 Huggingface上的開源模型
 
 See the [open issues](https://github.com/kenhutaiwan/MyLlmUtils/issues) for a full list of proposed features (and known issues).
 
 <!-- LICENSE -->
 ## License
```

