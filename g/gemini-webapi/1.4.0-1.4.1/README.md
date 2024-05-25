# Comparing `tmp/gemini_webapi-1.4.0.tar.gz` & `tmp/gemini_webapi-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_webapi-1.4.0.tar", last modified: Thu May 23 21:36:03 2024, max compression
+gzip compressed data, was "gemini_webapi-1.4.1.tar", last modified: Sat May 25 23:13:31 2024, max compression
```

## Comparing `gemini_webapi-1.4.0.tar` & `gemini_webapi-1.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.361659 gemini_webapi-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.361659 gemini_webapi-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55231 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/assets/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.361659 gemini_webapi-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.365659 gemini_webapi-1.4.0/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55231 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:36:03.000000 gemini_webapi-1.4.0/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:36:03.369659 gemini_webapi-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 21:35:58.000000 gemini_webapi-1.4.0/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.522483 gemini_webapi-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17780 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/assets/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:13:31.522483 gemini_webapi-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.514484 gemini_webapi-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55249 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-25 23:13:31.000000 gemini_webapi-1.4.1/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:13:31.518483 gemini_webapi-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-25 23:13:27.000000 gemini_webapi-1.4.1/tests/test_save_image.py
```

### Comparing `gemini_webapi-1.4.0/.github/workflows/pypi-publish.yml` & `gemini_webapi-1.4.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/.gitignore` & `gemini_webapi-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/LICENSE` & `gemini_webapi-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/PKG-INFO` & `gemini_webapi-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.4.0
+Version: 1.4.1
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -815,15 +815,15 @@
 
 > [!TIP]
 >
 > Simply use `print(response)` to get the same output if you just want to see the response text
 
 ### Generate contents from image
 
-Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` to `GeminiClient.generate_content` together with text prompt.
+Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` or `pathlib.Path` to `GeminiClient.generate_content` together with text prompt.
 
 ```python
 async def main():
     response = await client.generate_content(
             "Describe each of these images",
             images=["assets/banner.png", "assets/favicon.png"],
         )
```

### Comparing `gemini_webapi-1.4.0/README.md` & `gemini_webapi-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 > [!TIP]
 >
 > Simply use `print(response)` to get the same output if you just want to see the response text
 
 ### Generate contents from image
 
-Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` to `GeminiClient.generate_content` together with text prompt.
+Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` or `pathlib.Path` to `GeminiClient.generate_content` together with text prompt.
 
 ```python
 async def main():
     response = await client.generate_content(
             "Describe each of these images",
             images=["assets/banner.png", "assets/favicon.png"],
         )
```

#### html2text {}

```diff
@@ -62,41 +62,41 @@
 `close_delay` for better resource management. ### Generate contents from text
 Ask a one-turn quick question by calling `GeminiClient.generate_content`.
 ```python async def main(): response = await client.generate_content("Hello
 World!") print(response.text) asyncio.run(main()) ``` > [!TIP] > > Simply use
 `print(response)` to get the same output if you just want to see the response
 text ### Generate contents from image Gemini supports image recognition and
 generating contents from images. Optionally, you can pass images in a list of
-file data in `bytes` or their paths in `str` to `GeminiClient.generate_content`
-together with text prompt. ```python async def main(): response = await
-client.generate_content( "Describe each of these images", images=["assets/
-banner.png", "assets/favicon.png"], ) print(response.text) asyncio.run(main())
-``` ### Conversations across multiple turns If you want to keep conversation
-continuous, please use `GeminiClient.start_chat` to create a `ChatSession`
-object and send messages through it. The conversation history will be
-automatically handled and get updated after each turn. ```python async def main
-(): chat = client.start_chat() response1 = await chat.send_message("Briefly
-introduce Europe") response2 = await chat.send_message("What's the population
-there?") print(response1.text, response2.text, sep="\n\n-----------------------
------------\n\n") asyncio.run(main()) ``` > [!TIP] > > Same as
-`GeminiClient.generate_content`, `ChatSession.send_message` also accepts
-`image` as an optional argument. ### Continue previous conversations To
-manually retrieve previous conversations, you can pass previous `ChatSession`'s
-metadata to `GeminiClient.start_chat` when creating a new `ChatSession`.
-Alternatively, you can persist previous metadata to a file or db if you need to
-access them after the current Python process has exited. ```python async def
-main(): # Start a new chat session chat = client.start_chat() response = await
-chat.send_message("Fine weather today") # Save chat's metadata previous_session
-= chat.metadata # Load the previous conversation previous_chat =
-client.start_chat(metadata=previous_session) response = await
-previous_chat.send_message("What was my previous message?") print(response)
-asyncio.run(main()) ``` ### Retrieve images in response Images in the API's
-output are stored as a list of `Image` objects. You can access the image title,
-URL, and description by calling `image.title`, `image.url` and `image.alt`
-respectively. ```python async def main(): response = await
+file data in `bytes` or their paths in `str` or `pathlib.Path` to
+`GeminiClient.generate_content` together with text prompt. ```python async def
+main(): response = await client.generate_content( "Describe each of these
+images", images=["assets/banner.png", "assets/favicon.png"], ) print
+(response.text) asyncio.run(main()) ``` ### Conversations across multiple turns
+If you want to keep conversation continuous, please use
+`GeminiClient.start_chat` to create a `ChatSession` object and send messages
+through it. The conversation history will be automatically handled and get
+updated after each turn. ```python async def main(): chat = client.start_chat()
+response1 = await chat.send_message("Briefly introduce Europe") response2 =
+await chat.send_message("What's the population there?") print(response1.text,
+response2.text, sep="\n\n----------------------------------\n\n") asyncio.run
+(main()) ``` > [!TIP] > > Same as `GeminiClient.generate_content`,
+`ChatSession.send_message` also accepts `image` as an optional argument. ###
+Continue previous conversations To manually retrieve previous conversations,
+you can pass previous `ChatSession`'s metadata to `GeminiClient.start_chat`
+when creating a new `ChatSession`. Alternatively, you can persist previous
+metadata to a file or db if you need to access them after the current Python
+process has exited. ```python async def main(): # Start a new chat session chat
+= client.start_chat() response = await chat.send_message("Fine weather today")
+# Save chat's metadata previous_session = chat.metadata # Load the previous
+conversation previous_chat = client.start_chat(metadata=previous_session)
+response = await previous_chat.send_message("What was my previous message?")
+print(response) asyncio.run(main()) ``` ### Retrieve images in response Images
+in the API's output are stored as a list of `Image` objects. You can access the
+image title, URL, and description by calling `image.title`, `image.url` and
+`image.alt` respectively. ```python async def main(): response = await
 client.generate_content("Send me some pictures of cats") for image in
 response.images: print(image, "\n\n----------------------------------\n")
 asyncio.run(main()) ``` ### Generate images with ImageFx In February 2022,
 Google introduced a new AI image generator called ImageFx and integrated it
 into Gemini. You can ask Gemini to generate images with ImageFx simply by
 natural language. > [!IMPORTANT] > > Google has some limitations on the image
 generation feature in Gemini, so its availability could be different per
```

### Comparing `gemini_webapi-1.4.0/assets/banner.png` & `gemini_webapi-1.4.1/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/assets/favicon.png` & `gemini_webapi-1.4.1/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/assets/logo.svg` & `gemini_webapi-1.4.1/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/pyproject.toml` & `gemini_webapi-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/client.py` & `gemini_webapi-1.4.1/src/gemini_webapi/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import functools
 import asyncio
 from asyncio import Task
+from pathlib import Path
 from typing import Any, Optional
 
 from httpx import AsyncClient, ReadTimeout
 
 from .types import WebImage, GeneratedImage, Candidate, ModelOutput
 from .exceptions import AuthError, APIError, TimeoutError, GeminiError
 from .constants import Endpoint, Headers
@@ -248,26 +249,26 @@
                 self.cookies["__Secure-1PSIDTS"] = new_1psidts
             await asyncio.sleep(self.refresh_interval)
 
     @running(retry=1)
     async def generate_content(
         self,
         prompt: str,
-        images: list[bytes | str] | None = None,
+        images: list[bytes | str | Path] | None = None,
         chat: Optional["ChatSession"] = None,
     ) -> ModelOutput:
         """
         Generates contents with prompt.
 
         Parameters
         ----------
         prompt: `str`
             Prompt provided by user.
-        images: `list[bytes | str]`, optional
-            List of image file data in bytes or file paths in string.
+        images: `list[bytes | str | Path]`, optional
+            List of image file paths or file data in bytes.
         chat: `ChatSession`, optional
             Chat data to retrieve conversation history. If None, will automatically generate a new chat id when sending post request.
 
         Returns
         -------
         :class:`ModelOutput`
             Output data from gemini.google.com, use `ModelOutput.text` to get the default text reply, `ModelOutput.images` to get a list
@@ -481,26 +482,26 @@
         super().__setattr__(name, value)
         # update conversation history when last output is updated
         if name == "last_output" and isinstance(value, ModelOutput):
             self.metadata = value.metadata
             self.rcid = value.rcid
 
     async def send_message(
-        self, prompt: str, images: list[bytes | str] | None = None,
+        self, prompt: str, images: list[bytes | str | Path] | None = None,
     ) -> ModelOutput:
         """
         Generates contents with prompt.
         Use as a shortcut for `GeminiClient.generate_content(prompt, image, self)`.
 
         Parameters
         ----------
         prompt: `str`
             Prompt provided by user.
-        images: `list[bytes | str]`, optional
-            List of image file data in bytes or file paths in string.
+        images: `list[bytes | str | Path]`, optional
+            List of image file paths or file data in bytes.
 
         Returns
         -------
         :class:`ModelOutput`
             Output data from gemini.google.com, use `ModelOutput.text` to get the default text reply, `ModelOutput.images` to get a list
             of images in the default reply, `ModelOutput.candidates` to get a list of all answer candidates in the output.
```

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/constants.py` & `gemini_webapi-1.4.1/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/exceptions.py` & `gemini_webapi-1.4.1/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/types/candidate.py` & `gemini_webapi-1.4.1/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/types/image.py` & `gemini_webapi-1.4.1/src/gemini_webapi/types/image.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/types/modeloutput.py` & `gemini_webapi-1.4.1/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/utils/get_access_token.py` & `gemini_webapi-1.4.1/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini_webapi-1.4.1/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/utils/logger.py` & `gemini_webapi-1.4.1/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini_webapi-1.4.1/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi/utils/upload_file.py` & `gemini_webapi-1.4.1/src/gemini_webapi/utils/upload_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from pathlib import Path
+
 from httpx import AsyncClient
 from pydantic import validate_call
 
 from ..constants import Endpoint, Headers
 
 
 @validate_call
-async def upload_file(file: bytes | str, proxies: dict | None = None) -> str:
+async def upload_file(file: bytes | str | Path, proxies: dict | None = None) -> str:
     """
     Upload a file to Google's server and return its identifier.
 
     Parameters
     ----------
-    file : `bytes` | `str`
+    file : `bytes` | `str` | `Path`
         File data in bytes, or path to the file to be uploaded.
     proxies: `dict`, optional
         Dict of proxies.
 
     Returns
     -------
     `str`
@@ -24,15 +26,15 @@
 
     Raises
     ------
     `httpx.HTTPStatusError`
         If the upload request failed.
     """
 
-    if isinstance(file, str):
+    if not isinstance(file, bytes):
         with open(file, "rb") as f:
             file = f.read()
 
     async with AsyncClient(proxies=proxies) as client:
         response = await client.post(
             url=Endpoint.UPLOAD.value,
             headers=Headers.UPLOAD.value,
```

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi.egg-info/PKG-INFO` & `gemini_webapi-1.4.1/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.4.0
+Version: 1.4.1
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -815,15 +815,15 @@
 
 > [!TIP]
 >
 > Simply use `print(response)` to get the same output if you just want to see the response text
 
 ### Generate contents from image
 
-Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` to `GeminiClient.generate_content` together with text prompt.
+Gemini supports image recognition and generating contents from images. Optionally, you can pass images in a list of file data in `bytes` or their paths in `str` or `pathlib.Path` to `GeminiClient.generate_content` together with text prompt.
 
 ```python
 async def main():
     response = await client.generate_content(
             "Describe each of these images",
             images=["assets/banner.png", "assets/favicon.png"],
         )
```

### Comparing `gemini_webapi-1.4.0/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini_webapi-1.4.1/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/tests/test_client_features.py` & `gemini_webapi-1.4.1/tests/test_client_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import unittest
 import logging
+from pathlib import Path
 
 from loguru import logger
 
 from gemini_webapi import GeminiClient, AuthError, set_log_level
 
 logging.getLogger("asyncio").setLevel(logging.ERROR)
 set_log_level("DEBUG")
@@ -25,15 +26,15 @@
     async def test_successful_request(self):
         response = await self.geminiclient.generate_content("Hello World!")
         self.assertTrue(response.text)
 
     @logger.catch(reraise=True)
     async def test_upload_image(self):
         response = await self.geminiclient.generate_content(
-            "Describe the image", images=["assets/banner.png"]
+            "Describe these images", images=[Path("assets/banner.png"), "assets/favicon.png"]
         )
         self.assertTrue(response.text)
         logger.debug(response.text)
 
     @logger.catch(reraise=True)
     async def test_continuous_conversation(self):
         chat = self.geminiclient.start_chat()
```

### Comparing `gemini_webapi-1.4.0/tests/test_rotate_cookies.py` & `gemini_webapi-1.4.1/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.4.0/tests/test_save_image.py` & `gemini_webapi-1.4.1/tests/test_save_image.py`

 * *Files identical despite different names*

