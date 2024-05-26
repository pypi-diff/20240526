# Comparing `tmp/auto-coder-0.1.8.tar.gz` & `tmp/auto-coder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-coder-0.1.8.tar", last modified: Sun Mar 17 15:26:35 2024, max compression
+gzip compressed data, was "auto-coder-0.1.9.tar", last modified: Mon Mar 18 12:40:02 2024, max compression
```

## Comparing `auto-coder-0.1.8.tar` & `auto-coder-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/
--rw-r--r--   0 winubuntu  (1000) winubuntu  (1000)    16255 2024-03-17 15:26:35.950064 auto-coder-0.1.8/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15938 2024-03-17 15:25:53.000000 auto-coder-0.1.8/README.md
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       38 2024-03-17 15:26:35.950064 auto-coder-0.1.8/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1346 2024-03-13 14:17:55.000000 auto-coder-0.1.8/setup.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.946064 auto-coder-0.1.8/src/
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/auto_coder.egg-info/
--rw-r--r--   0 winubuntu  (1000) winubuntu  (1000)    16255 2024-03-17 15:26:35.000000 auto-coder-0.1.8/src/auto_coder.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      888 2024-03-17 15:26:35.000000 auto-coder-0.1.8/src/auto_coder.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2024-03-17 15:26:35.000000 auto-coder-0.1.8/src/auto_coder.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       57 2024-03-17 15:26:35.000000 auto-coder-0.1.8/src/auto_coder.egg-info/entry_points.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       10 2024-03-17 15:26:35.000000 auto-coder-0.1.8/src/auto_coder.egg-info/top_level.txt
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-13 06:35:22.000000 auto-coder-0.1.8/src/autocoder/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8585 2024-03-17 04:49:23.000000 auto-coder-0.1.8/src/autocoder/auto_coder.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/common/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2816 2024-03-17 05:05:58.000000 auto-coder-0.1.8/src/autocoder/common/JupyterClient.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2063 2024-03-17 15:23:01.000000 auto-coder-0.1.8/src/autocoder/common/ShellClient.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     9201 2024-03-17 05:10:05.000000 auto-coder-0.1.8/src/autocoder/common/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1089 2024-03-13 23:48:44.000000 auto-coder-0.1.8/src/autocoder/common/cleaner.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2911 2024-03-13 23:48:44.000000 auto-coder-0.1.8/src/autocoder/common/const.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15806 2024-03-17 04:42:22.000000 auto-coder-0.1.8/src/autocoder/common/search.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/dispacher/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1006 2024-03-15 02:56:30.000000 auto-coder-0.1.8/src/autocoder/dispacher/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/dispacher/actions/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-13 23:59:37.000000 auto-coder-0.1.8/src/autocoder/dispacher/actions/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10478 2024-03-15 12:47:45.000000 auto-coder-0.1.8/src/autocoder/dispacher/actions/action.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11038 2024-03-17 15:13:08.000000 auto-coder-0.1.8/src/autocoder/dispacher/actions/copilot.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/index/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-15 02:21:37.000000 auto-coder-0.1.8/src/autocoder/index/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6699 2024-03-15 02:48:14.000000 auto-coder-0.1.8/src/autocoder/index/index.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/pyproject/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7387 2024-03-15 08:25:34.000000 auto-coder-0.1.8/src/autocoder/pyproject/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/suffixproject/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3877 2024-03-17 05:05:02.000000 auto-coder-0.1.8/src/autocoder/suffixproject/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/tsproject/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4815 2024-03-15 12:47:28.000000 auto-coder-0.1.8/src/autocoder/tsproject/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-17 15:26:35.950064 auto-coder-0.1.8/src/autocoder/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-15 12:40:25.000000 auto-coder-0.1.8/src/autocoder/utils/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2229 2024-03-17 02:55:06.000000 auto-coder-0.1.8/src/autocoder/utils/rest.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       21 2024-03-17 15:26:14.000000 auto-coder-0.1.8/src/autocoder/version.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/
+-rw-r--r--   0 winubuntu  (1000) winubuntu  (1000)    17185 2024-03-18 12:40:02.020278 auto-coder-0.1.9/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16868 2024-03-18 12:39:22.000000 auto-coder-0.1.9/README.md
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       38 2024-03-18 12:40:02.020278 auto-coder-0.1.9/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1346 2024-03-13 14:17:55.000000 auto-coder-0.1.9/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.016278 auto-coder-0.1.9/src/
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.016278 auto-coder-0.1.9/src/auto_coder.egg-info/
+-rw-r--r--   0 winubuntu  (1000) winubuntu  (1000)    17185 2024-03-18 12:40:01.000000 auto-coder-0.1.9/src/auto_coder.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      888 2024-03-18 12:40:01.000000 auto-coder-0.1.9/src/auto_coder.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2024-03-18 12:40:01.000000 auto-coder-0.1.9/src/auto_coder.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       57 2024-03-18 12:40:01.000000 auto-coder-0.1.9/src/auto_coder.egg-info/entry_points.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       10 2024-03-18 12:40:01.000000 auto-coder-0.1.9/src/auto_coder.egg-info/top_level.txt
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-13 06:35:22.000000 auto-coder-0.1.9/src/autocoder/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8935 2024-03-18 11:23:13.000000 auto-coder-0.1.9/src/autocoder/auto_coder.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/common/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2816 2024-03-17 05:05:58.000000 auto-coder-0.1.9/src/autocoder/common/JupyterClient.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2063 2024-03-17 15:23:01.000000 auto-coder-0.1.9/src/autocoder/common/ShellClient.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     9209 2024-03-18 11:35:56.000000 auto-coder-0.1.9/src/autocoder/common/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1089 2024-03-13 23:48:44.000000 auto-coder-0.1.9/src/autocoder/common/cleaner.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2911 2024-03-13 23:48:44.000000 auto-coder-0.1.9/src/autocoder/common/const.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15806 2024-03-17 04:42:22.000000 auto-coder-0.1.9/src/autocoder/common/search.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/dispacher/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1006 2024-03-15 02:56:30.000000 auto-coder-0.1.9/src/autocoder/dispacher/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/dispacher/actions/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-13 23:59:37.000000 auto-coder-0.1.9/src/autocoder/dispacher/actions/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10478 2024-03-15 12:47:45.000000 auto-coder-0.1.9/src/autocoder/dispacher/actions/action.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11038 2024-03-18 02:39:55.000000 auto-coder-0.1.9/src/autocoder/dispacher/actions/copilot.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/index/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-15 02:21:37.000000 auto-coder-0.1.9/src/autocoder/index/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6699 2024-03-15 02:48:14.000000 auto-coder-0.1.9/src/autocoder/index/index.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/pyproject/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7395 2024-03-18 11:58:59.000000 auto-coder-0.1.9/src/autocoder/pyproject/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/suffixproject/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3877 2024-03-17 05:05:02.000000 auto-coder-0.1.9/src/autocoder/suffixproject/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/tsproject/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4815 2024-03-15 12:47:28.000000 auto-coder-0.1.9/src/autocoder/tsproject/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-18 12:40:02.020278 auto-coder-0.1.9/src/autocoder/utils/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2024-03-15 12:40:25.000000 auto-coder-0.1.9/src/autocoder/utils/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2229 2024-03-17 02:55:06.000000 auto-coder-0.1.9/src/autocoder/utils/rest.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       21 2024-03-18 12:39:13.000000 auto-coder-0.1.9/src/autocoder/version.py
```

### Comparing `auto-coder-0.1.8/PKG-INFO` & `auto-coder-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: auto-coder
-Version: 0.1.8
-Summary: AutoCoder: AutoCoder
-Author: allwefantasy
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>    
     <img alt="auto-coder" src="https://github.com/allwefantasy/byzer-llm/blob/master/docs/source/assets/logos/logo.jpg" width=55%>
   </picture>
 </p>
 
@@ -23,15 +14,15 @@
 
 </p>
 
 ---
 
 *Latest News* 🔥
 
-- [2024/03] Release Auto-Coder 0.1.7
+- [2024/03] Release Auto-Coder 0.1.9
 
 ---
 
 
 
 🚀 Attention developers! 🚨 The game-changing Auto-Coder has arrived, and it's about to take your AI programming to a whole new level! 🌟
 
@@ -51,57 +42,85 @@
 
 🌟 Don't wait another second! Experience the raw power of Auto-Coder today and let AI be your ultimate coding companion! https://github.com/allwefantasy/auto-coder 🔥
 
 #AutoCoder #AIProgramming #GameChanger #ByzerLLM #DevTools
 
 ## Table of Contents
 
+- [Installation](#installation)
 - [Brand new Installation](#brand-new-installation)
-- [Existing Installation](#existing-installation)
 - [Usage](#usage)
   - [Basic](#basic)
   - [Advanced](#advanced)
   - [Python Project Only Features](#python-project-only-features)
   - [TypeScript Project](#typescript-project)
   - [Real-Auto](#real-auto)
     - [Real-Auto with Search Engine](#real-auto-with-search-engine)
 
 
 
+## Existing Installation
+
+```shell
+# or https://gitcode.com/allwefantasy11/auto-coder.git
+git clone https://github.com/allwefantasy/auto-coder.git
+pip install -r requirements.txt
+## if you want to use private/open-source models, uncomment this line.
+# pip install -U vllm
+pip install -U byzerllm
+pip install -U auto-coder
+
+ray start --head
+```
 
 ## Brand new Installation
 
 You can use the script provided by Byzer-LLM to setup the nvidia-driver/cuda environment:
 
 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04](https://docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy)
 
 After the nvidia-driver/cuda environment is set up, you can install auto_coder like this:
 
 ```shell
 pip install -U auto-coder
 ```
 
-## Existing Installation
 
+## Usage 
+
+### LLM Model
+
+> Recommend to use 千义通问Max/Qwen-Max-longcontext SaaS model
+
+Try to use the following command to deploy Qwen-Max:
 
 ```shell
-# or https://gitcode.com/allwefantasy11/auto-coder.git
-git clone https://github.com/allwefantasy/auto-coder.git
-pip install -r requirements.txt
-## if you want to use private/open-source models, uncomment this line.
-# pip install -U vllm
-pip install -U byzerllm
-pip install -U auto-coder
+byzerllm deploy  --pretrained_model_type saas/qianwen \
+--cpus_per_worker 0.01 \
+--gpus_per_worker 0 \
+--num_workers 1 \
+--infer_params saas.api_key="sk-33cbd1e4a45f477e860035a57b39efa8" saas.model="qwen-max" \
+--model qianwen_short_chat 
 ```
 
-## Usage 
+Then you can use the following command to test the model:
+
+```shell
+byzerllm query --model qianwen_short_chat --query "你好"
+```
+
+If you want to undeploy the model:
+
+```shell
+byzerllm undeploy --model qianwen_short_chat
+```
+
+If you want to deploy you private/open source model, please try to this [link](https://github.com/allwefantasy/byzer-llm)
 
 ### Basic 
-> Recommend to use 千义通问Max/Qwen-Max-longcontext SaaS model
-> You should deploy the model by [Byzer-LLM](https://github.com/allwefantasy/byzer-llm)
 
 
 The auto-coder provide two ways:
 
 1. Generate context for the query and you can copy&&Paste to Web UI of ChatGPT/Claud3/Kimi.
 2. Use the model from Byzer-LLM to generate the result directly.
 
@@ -157,18 +176,21 @@
 2. model
 
 For example:
 
 ```yaml
 source_dir: /home/winubuntu/projects/ByzerRawCopilot 
 target_file: /home/winubuntu/projects/ByzerRawCopilot/output.txt 
+
 model: qianwen_chat
 model_max_length: 2000
 anti_quota_limit: 13
+
 skip_build_index: false
+
 project_type: "copilot/.py"
 query: |
   优化 copilot 里的 get_suffix_from_project_type 函数并更新原文件
 ```
 
 Here we add a new parameter `skip_build_index`, by default, this value is true. 
 If you set it to false and a model provide at the same time, then the auto-coder will generate index for the source code using the model(This may cost a lot of tokens), and the index file will be stored in a directory called `.auto-coder` in source directory. 
@@ -314,14 +336,23 @@
   帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project
 ```
 
 Here we add  new parameters  `search_engine` and `search_engine_token`, the search engine will provide more context for the model, and the model will use the context to generate the result.
 
 For now, we support bing/google.  If you use bing, try to get the token from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api).
 
+The basic workflow is:
+
+1. search the query 
+2. reranking the search result by snippets
+3. fetch the first search result and answer the question based on the full content.
+4. generate the result based on the query and the full content.
+5. get execute steps based on the result.
+5. execute the steps by ShellClient/PythonClient in auto-coder.
+
 Here is the output:
 
 ```text
 用户尝试: UserIntent.CREATE_NEW_PROJECT
 search SearchEngine.BING for 帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project...
 reraking the search result by snippets...
 fetch https://blog.csdn.net/weixin_42429718/article/details/117402097 and answer the quesion (帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project) based on the full content...
```

#### html2text {}

```diff
@@ -1,16 +1,11 @@
-Metadata-Version: 2.1 Name: auto-coder Version: 0.1.8 Summary: AutoCoder:
-AutoCoder Author: allwefantasy Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
-text/markdown
                                  [auto-coder]
                   ******** AAuuttoo--CCooddeerr ((ppoowweerreedd bbyy BByyzzeerr--LLLLMM)) ********
                              | _EE_nn_gg_ll_ii_ss_hh | _?ä_?¸_?­_?æ_?_? |
---- *Latest News* ð¥ - [2024/03] Release Auto-Coder 0.1.7 --- ð Attention
+--- *Latest News* ð¥ - [2024/03] Release Auto-Coder 0.1.9 --- ð Attention
 developers! ð¨ The game-changing Auto-Coder has arrived, and it's about to
 take your AI programming to a whole new level! ð Fueled by the incredible
 power of Byzer-LLM, this command-line tool is packed with features that will
 blow your mind: ð Say goodbye to manual context gathering! Auto-Coder
 intelligently generates code based on the context of your source directory.
 It's like having a genius assistant that knows exactly what you need! ð¡ Two
 modes, endless possibilities! Generate perfect prompts to paste into web-based
@@ -24,91 +19,98 @@
 and even modifies code for you. It's like having a super-smart sidekick that
 never sleeps! ð§âð» Developers, prepare to have your minds blown! Auto-
 Coder integrates seamlessly with the hottest AI models like ChatGPT,
 turbocharging your development process to lightning speeds! ð ð Don't
 wait another second! Experience the raw power of Auto-Coder today and let AI be
 your ultimate coding companion! https://github.com/allwefantasy/auto-coder ð¥
 #AutoCoder #AIProgramming #GameChanger #ByzerLLM #DevTools ## Table of Contents
-- [Brand new Installation](#brand-new-installation) - [Existing Installation]
-(#existing-installation) - [Usage](#usage) - [Basic](#basic) - [Advanced]
-(#advanced) - [Python Project Only Features](#python-project-only-features) -
-[TypeScript Project](#typescript-project) - [Real-Auto](#real-auto) - [Real-
-Auto with Search Engine](#real-auto-with-search-engine) ## Brand new
-Installation You can use the script provided by Byzer-LLM to setup the nvidia-
-driver/cuda environment: 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04](https://
-docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy) After the nvidia-driver/
-cuda environment is set up, you can install auto_coder like this: ```shell pip
-install -U auto-coder ``` ## Existing Installation ```shell # or https://
-gitcode.com/allwefantasy11/auto-coder.git git clone https://github.com/
-allwefantasy/auto-coder.git pip install -r requirements.txt ## if you want to
-use private/open-source models, uncomment this line. # pip install -U vllm pip
-install -U byzerllm pip install -U auto-coder ``` ## Usage ### Basic >
-Recommend to use åä¹éé®Max/Qwen-Max-longcontext SaaS model > You should
-deploy the model by [Byzer-LLM](https://github.com/allwefantasy/byzer-llm) The
-auto-coder provide two ways: 1. Generate context for the query and you can
-copy&&Paste to Web UI of ChatGPT/Claud3/Kimi. 2. Use the model from Byzer-LLM
-to generate the result directly. >> Note: You should make sure the model has a
-long context length support, e.g. >32k. The auto-coder will collect the source
-code from the source directory, and then generate context into the target file
-based on the query. Then you can copy the content of `output.txt` and paste it
-to Web UI of ChatGPT/Claud3/Kimi: For example: ```shell auto-coder --source_dir
-/home/winubuntu/projects/ByzerRawCopilot --target_file /home/winubuntu/
-projects/ByzerRawCopilot/output.txt --query "å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿
-auto-coder å½ä»¤æ§è¡ï¼" ``` You can also put all arguments into a yaml
-file: ```yaml # /home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml
-source_dir: /home/winubuntu/projects/ByzerRawCopilot target_file: /home/
-winubuntu/projects/ByzerRawCopilot/output.txt query: |
-å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-coder å½ä»¤æ§è¡ï¼ ``` Then use the
-following command: ```shell auto-coder --file /home/winubuntu/projects/
-ByzerRawCopilot/auto-coder.yaml ``` If you want to use the model from Byzer-
-LLM, you can use the following command: ```shell auto-coder --source_dir /home/
+- [Installation](#installation) - [Brand new Installation](#brand-new-
+installation) - [Usage](#usage) - [Basic](#basic) - [Advanced](#advanced) -
+[Python Project Only Features](#python-project-only-features) - [TypeScript
+Project](#typescript-project) - [Real-Auto](#real-auto) - [Real-Auto with
+Search Engine](#real-auto-with-search-engine) ## Existing Installation ```shell
+# or https://gitcode.com/allwefantasy11/auto-coder.git git clone https://
+github.com/allwefantasy/auto-coder.git pip install -r requirements.txt ## if
+you want to use private/open-source models, uncomment this line. # pip install
+-U vllm pip install -U byzerllm pip install -U auto-coder ray start --head ```
+## Brand new Installation You can use the script provided by Byzer-LLM to setup
+the nvidia-driver/cuda environment: 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04]
+(https://docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy) After the nvidia-
+driver/cuda environment is set up, you can install auto_coder like this:
+```shell pip install -U auto-coder ``` ## Usage ### LLM Model > Recommend to
+use åä¹éé®Max/Qwen-Max-longcontext SaaS model Try to use the following
+command to deploy Qwen-Max: ```shell byzerllm deploy --pretrained_model_type
+saas/qianwen \ --cpus_per_worker 0.01 \ --gpus_per_worker 0 \ --num_workers 1 \
+--infer_params saas.api_key="sk-33cbd1e4a45f477e860035a57b39efa8"
+saas.model="qwen-max" \ --model qianwen_short_chat ``` Then you can use the
+following command to test the model: ```shell byzerllm query --model
+qianwen_short_chat --query "ä½ å¥½" ``` If you want to undeploy the model:
+```shell byzerllm undeploy --model qianwen_short_chat ``` If you want to deploy
+you private/open source model, please try to this [link](https://github.com/
+allwefantasy/byzer-llm) ### Basic The auto-coder provide two ways: 1. Generate
+context for the query and you can copy&&Paste to Web UI of ChatGPT/Claud3/Kimi.
+2. Use the model from Byzer-LLM to generate the result directly. >> Note: You
+should make sure the model has a long context length support, e.g. >32k. The
+auto-coder will collect the source code from the source directory, and then
+generate context into the target file based on the query. Then you can copy the
+content of `output.txt` and paste it to Web UI of ChatGPT/Claud3/Kimi: For
+example: ```shell auto-coder --source_dir /home/winubuntu/projects/
+ByzerRawCopilot --target_file /home/winubuntu/projects/ByzerRawCopilot/
+output.txt --query "å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-coder
+å½ä»¤æ§è¡ï¼" ``` You can also put all arguments into a yaml file: ```yaml #
+/home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml source_dir: /home/
+winubuntu/projects/ByzerRawCopilot target_file: /home/winubuntu/projects/
+ByzerRawCopilot/output.txt query: | å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-
+coder å½ä»¤æ§è¡ï¼ ``` Then use the following command: ```shell auto-coder -
+-file /home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml ``` If you want
+to use the model from Byzer-LLM, you can use the following command: ```shell
+auto-coder --source_dir /home/winubuntu/projects/ByzerRawCopilot --target_file
+/home/winubuntu/projects/ByzerRawCopilot/output.txt --model qianwen_chat --
+execute --query "éæ°çæä¸ä¸ª is_likely_useful_file
+æ¹æ³ï¼æ»¡è¶³reactjs+typescript ç»åçé¡¹ç®ã" ``` In the above command,
+we provide a model and enable the execute mode, the auto-coder will collect the
+source code from the source directory, and then generate context for the query,
+and then use the model to generate the result, then put the result into the
+target file. ### How to reduce the context length? As you may know, auto-coder
+will collect the source code from the source directory, and then generate
+context for the query, if the source directory is too large, the context will
+be too long, and the model may not be able to handle it. There are two ways to
+reduce the context length: 1. Change the source_dir to sub directory of
+project. 2. Enable aut-coder's index feature. In order to use the index
+feature, you should configure some extra parameters: 1. skip_build_index: false
+2. model For example: ```yaml source_dir: /home/winubuntu/projects/
+ByzerRawCopilot target_file: /home/winubuntu/projects/ByzerRawCopilot/
+output.txt model: qianwen_chat model_max_length: 2000 anti_quota_limit: 13
+skip_build_index: false project_type: "copilot/.py" query: | ä¼å copilot
+éç get_suffix_from_project_type å½æ°å¹¶æ´æ°åæä»¶ ``` Here we add a
+new parameter `skip_build_index`, by default, this value is true. If you set it
+to false and a model provide at the same time, then the auto-coder will
+generate index for the source code using the model(This may cost a lot of
+tokens), and the index file will be stored in a directory called `.auto-coder`
+in source directory. Once the index is created, the auto-coder will use the
+index to filter files and reduce the context length. notice that the filter
+action also use model, and it may cost tokens, so you should use it carefully.
+### Advanced > This feature only works with the model from Byzer-LLM. Translate
+the markdown file in the project: ```shell auto-coder --source_dir /home/
 winubuntu/projects/ByzerRawCopilot --target_file /home/winubuntu/projects/
-ByzerRawCopilot/output.txt --model qianwen_chat --execute --query
-"éæ°çæä¸ä¸ª is_likely_useful_file æ¹æ³ï¼æ»¡è¶³reactjs+typescript
-ç»åçé¡¹ç®ã" ``` In the above command, we provide a model and enable the
-execute mode, the auto-coder will collect the source code from the source
-directory, and then generate context for the query, and then use the model to
-generate the result, then put the result into the target file. ### How to
-reduce the context length? As you may know, auto-coder will collect the source
-code from the source directory, and then generate context for the query, if the
-source directory is too large, the context will be too long, and the model may
-not be able to handle it. There are two ways to reduce the context length: 1.
-Change the source_dir to sub directory of project. 2. Enable aut-coder's index
-feature. In order to use the index feature, you should configure some extra
-parameters: 1. skip_build_index: false 2. model For example: ```yaml
-source_dir: /home/winubuntu/projects/ByzerRawCopilot target_file: /home/
-winubuntu/projects/ByzerRawCopilot/output.txt model: qianwen_chat
-model_max_length: 2000 anti_quota_limit: 13 skip_build_index: false
-project_type: "copilot/.py" query: | ä¼å copilot éç
-get_suffix_from_project_type å½æ°å¹¶æ´æ°åæä»¶ ``` Here we add a new
-parameter `skip_build_index`, by default, this value is true. If you set it to
-false and a model provide at the same time, then the auto-coder will generate
-index for the source code using the model(This may cost a lot of tokens), and
-the index file will be stored in a directory called `.auto-coder` in source
-directory. Once the index is created, the auto-coder will use the index to
-filter files and reduce the context length. notice that the filter action also
-use model, and it may cost tokens, so you should use it carefully. ### Advanced
-> This feature only works with the model from Byzer-LLM. Translate the markdown
-file in the project: ```shell auto-coder --source_dir /home/winubuntu/projects/
+ByzerRawCopilot/output.txt --project_type "translate/ä¸­æ/.md/cn" --
+model_max_length 2000 --model qianwen_chat ``` When you want to translate some
+files, you must specify the model parameter. And the project_type is a litle
+bit complex, it's a combination of the following parameters: - translate: the
+project type - ä¸­æ: the target language you want to translate to - .md: the
+file extension you want to translate - cn: the new file suffix created with the
+translated content. for example, if the original file is README.md, the new
+file will be README-cn.md So the final project_type is "translate/ä¸­æ/.md/
+cn" If your model is powerful enough, you can use the following command to do
+the same task: ```shell auto-coder --source_dir /home/winubuntu/projects/
 ByzerRawCopilot --target_file /home/winubuntu/projects/ByzerRawCopilot/
-output.txt --project_type "translate/ä¸­æ/.md/cn" --model_max_length 2000 --
-model qianwen_chat ``` When you want to translate some files, you must specify
-the model parameter. And the project_type is a litle bit complex, it's a
-combination of the following parameters: - translate: the project type -
-ä¸­æ: the target language you want to translate to - .md: the file extension
-you want to translate - cn: the new file suffix created with the translated
-content. for example, if the original file is README.md, the new file will be
-README-cn.md So the final project_type is "translate/ä¸­æ/.md/cn" If your
-model is powerful enough, you can use the following command to do the same
-task: ```shell auto-coder --source_dir /home/winubuntu/projects/ByzerRawCopilot
---target_file /home/winubuntu/projects/ByzerRawCopilot/output.txt --model
-qianwen_chat --project_type translate --model_max_length 2000 --query
-"æé¡¹ç®ä¸­çmarkdownææ¡£ç¿»è¯æä¸­æ" ``` The model will extract
-"translate/ä¸­æ/.md/cn" from the query and then do the same thing as the
-previous command. Note: The model_max_length is used to control the model's
+output.txt --model qianwen_chat --project_type translate --model_max_length
+2000 --query "æé¡¹ç®ä¸­çmarkdownææ¡£ç¿»è¯æä¸­æ" ``` The model will
+extract "translate/ä¸­æ/.md/cn" from the query and then do the same thing as
+the previous command. Note: The model_max_length is used to control the model's
 generation length, if the model_max_length is not set, the default value is
 1024. You should change the value based on your esitmating on the length of the
 translation. ### Python Project Only Features In order to reduce the context
 length collected by the auto-coder, if you are dealing with a python project,
 you can use the following command: ```shell auto-coder --target_file /home/
 winubuntu/projects/ByzerRawCopilot/output.txt --script_path /home/winubuntu/
 projects/ByzerRawCopilot/xxx --package_name byzer_copilot --project_type py-
@@ -155,22 +157,26 @@
 output.txt model: qianwen_short_chat model_max_length: 2000 anti_quota_limit: 5
 search_engine: bing search_engine_token: xxxxxx project_type: "copilot" query:
 | å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
 ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project ``` Here we add new parameters
 `search_engine` and `search_engine_token`, the search engine will provide more
 context for the model, and the model will use the context to generate the
 result. For now, we support bing/google. If you use bing, try to get the token
-from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api).
-Here is the output: ```text ç¨æ·å°è¯: UserIntent.CREATE_NEW_PROJECT search
-SearchEngine.BING for å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
-ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project... reraking the search result by
-snippets... fetch https://blog.csdn.net/weixin_42429718/article/details/
-117402097 and answer the quesion (å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª
-typescript + reactjs ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project) based on the
-full content... user:
+from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api). The
+basic workflow is: 1. search the query 2. reranking the search result by
+snippets 3. fetch the first search result and answer the question based on the
+full content. 4. generate the result based on the query and the full content.
+5. get execute steps based on the result. 5. execute the steps by ShellClient/
+PythonClient in auto-coder. Here is the output: ```text ç¨æ·å°è¯:
+UserIntent.CREATE_NEW_PROJECT search SearchEngine.BING for å¸®æå¨/tmp/
+ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-
+project... reraking the search result by snippets... fetch https://
+blog.csdn.net/weixin_42429718/article/details/117402097 and answer the quesion
+(å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
+ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project) based on the full content... user:
 ä½ çæåç§ç¼ç¨è¯­è¨ä»¥åç¸å³æ¡æ¶å¯¹åºçé¡¹ç®ç»æãç°å¨ï¼ä½ éè¦
 æ ¹æ®ç¨æ·çé®é¢ï¼æ ¹æ®æä¾çä¿¡æ¯ï¼å¯¹é®é¢è¿è¡æè§£ï¼ç¶åçææ§è¡æ­¥éª¤ï¼å½æ§è¡å®æææ­¥éª¤ï¼æç»å¸®çæä¸ä¸ªç¬¦åå¯¹åºç¼ç¨è¯­è¨è§èä»¥åç¸å³æ¡æ¶çé¡¹ç®ç»æã
 æ´ä¸ªè¿ç¨åªè½ä½¿ç¨ python/shellã ç¯å¢ä¿¡æ¯å¦ä¸: æä½ç³»ç»:
 linux 5.15.0-48-generic Pythonçæ¬: 3.10.11 Condaç¯å¢: byzerllm-dev
 æ¯æBash ç°å¨è¯·åèä¸é¢åå®¹ï¼
 ç±äºæä¾çä¸ä¸æä¿¡æ¯ä¸å¨Linuxç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åå»ºä¸ä¸ªTypeScriptåReactJSé¡¹ç®æ å³ï¼æå°åºäºä¸è¬æä½æ­¥éª¤ç»åºè§£ç­ã
 è¦å¨Linuxç³»ç»ç `/tmp/
```

### Comparing `auto-coder-0.1.8/README.md` & `auto-coder-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: auto-coder
+Version: 0.1.9
+Summary: AutoCoder: AutoCoder
+Author: allwefantasy
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>    
     <img alt="auto-coder" src="https://github.com/allwefantasy/byzer-llm/blob/master/docs/source/assets/logos/logo.jpg" width=55%>
   </picture>
 </p>
 
@@ -14,15 +23,15 @@
 
 </p>
 
 ---
 
 *Latest News* 🔥
 
-- [2024/03] Release Auto-Coder 0.1.7
+- [2024/03] Release Auto-Coder 0.1.9
 
 ---
 
 
 
 🚀 Attention developers! 🚨 The game-changing Auto-Coder has arrived, and it's about to take your AI programming to a whole new level! 🌟
 
@@ -42,57 +51,85 @@
 
 🌟 Don't wait another second! Experience the raw power of Auto-Coder today and let AI be your ultimate coding companion! https://github.com/allwefantasy/auto-coder 🔥
 
 #AutoCoder #AIProgramming #GameChanger #ByzerLLM #DevTools
 
 ## Table of Contents
 
+- [Installation](#installation)
 - [Brand new Installation](#brand-new-installation)
-- [Existing Installation](#existing-installation)
 - [Usage](#usage)
   - [Basic](#basic)
   - [Advanced](#advanced)
   - [Python Project Only Features](#python-project-only-features)
   - [TypeScript Project](#typescript-project)
   - [Real-Auto](#real-auto)
     - [Real-Auto with Search Engine](#real-auto-with-search-engine)
 
 
 
+## Existing Installation
+
+```shell
+# or https://gitcode.com/allwefantasy11/auto-coder.git
+git clone https://github.com/allwefantasy/auto-coder.git
+pip install -r requirements.txt
+## if you want to use private/open-source models, uncomment this line.
+# pip install -U vllm
+pip install -U byzerllm
+pip install -U auto-coder
+
+ray start --head
+```
 
 ## Brand new Installation
 
 You can use the script provided by Byzer-LLM to setup the nvidia-driver/cuda environment:
 
 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04](https://docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy)
 
 After the nvidia-driver/cuda environment is set up, you can install auto_coder like this:
 
 ```shell
 pip install -U auto-coder
 ```
 
-## Existing Installation
 
+## Usage 
+
+### LLM Model
+
+> Recommend to use 千义通问Max/Qwen-Max-longcontext SaaS model
+
+Try to use the following command to deploy Qwen-Max:
 
 ```shell
-# or https://gitcode.com/allwefantasy11/auto-coder.git
-git clone https://github.com/allwefantasy/auto-coder.git
-pip install -r requirements.txt
-## if you want to use private/open-source models, uncomment this line.
-# pip install -U vllm
-pip install -U byzerllm
-pip install -U auto-coder
+byzerllm deploy  --pretrained_model_type saas/qianwen \
+--cpus_per_worker 0.01 \
+--gpus_per_worker 0 \
+--num_workers 1 \
+--infer_params saas.api_key="sk-33cbd1e4a45f477e860035a57b39efa8" saas.model="qwen-max" \
+--model qianwen_short_chat 
 ```
 
-## Usage 
+Then you can use the following command to test the model:
+
+```shell
+byzerllm query --model qianwen_short_chat --query "你好"
+```
+
+If you want to undeploy the model:
+
+```shell
+byzerllm undeploy --model qianwen_short_chat
+```
+
+If you want to deploy you private/open source model, please try to this [link](https://github.com/allwefantasy/byzer-llm)
 
 ### Basic 
-> Recommend to use 千义通问Max/Qwen-Max-longcontext SaaS model
-> You should deploy the model by [Byzer-LLM](https://github.com/allwefantasy/byzer-llm)
 
 
 The auto-coder provide two ways:
 
 1. Generate context for the query and you can copy&&Paste to Web UI of ChatGPT/Claud3/Kimi.
 2. Use the model from Byzer-LLM to generate the result directly.
 
@@ -148,18 +185,21 @@
 2. model
 
 For example:
 
 ```yaml
 source_dir: /home/winubuntu/projects/ByzerRawCopilot 
 target_file: /home/winubuntu/projects/ByzerRawCopilot/output.txt 
+
 model: qianwen_chat
 model_max_length: 2000
 anti_quota_limit: 13
+
 skip_build_index: false
+
 project_type: "copilot/.py"
 query: |
   优化 copilot 里的 get_suffix_from_project_type 函数并更新原文件
 ```
 
 Here we add a new parameter `skip_build_index`, by default, this value is true. 
 If you set it to false and a model provide at the same time, then the auto-coder will generate index for the source code using the model(This may cost a lot of tokens), and the index file will be stored in a directory called `.auto-coder` in source directory. 
@@ -305,14 +345,23 @@
   帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project
 ```
 
 Here we add  new parameters  `search_engine` and `search_engine_token`, the search engine will provide more context for the model, and the model will use the context to generate the result.
 
 For now, we support bing/google.  If you use bing, try to get the token from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api).
 
+The basic workflow is:
+
+1. search the query 
+2. reranking the search result by snippets
+3. fetch the first search result and answer the question based on the full content.
+4. generate the result based on the query and the full content.
+5. get execute steps based on the result.
+5. execute the steps by ShellClient/PythonClient in auto-coder.
+
 Here is the output:
 
 ```text
 用户尝试: UserIntent.CREATE_NEW_PROJECT
 search SearchEngine.BING for 帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project...
 reraking the search result by snippets...
 fetch https://blog.csdn.net/weixin_42429718/article/details/117402097 and answer the quesion (帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project) based on the full content...
```

#### html2text {}

```diff
@@ -1,11 +1,16 @@
+Metadata-Version: 2.1 Name: auto-coder Version: 0.1.9 Summary: AutoCoder:
+AutoCoder Author: allwefantasy Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
+text/markdown
                                  [auto-coder]
                   ******** AAuuttoo--CCooddeerr ((ppoowweerreedd bbyy BByyzzeerr--LLLLMM)) ********
                              | _EE_nn_gg_ll_ii_ss_hh | _?ä_?¸_?­_?æ_?_? |
---- *Latest News* ð¥ - [2024/03] Release Auto-Coder 0.1.7 --- ð Attention
+--- *Latest News* ð¥ - [2024/03] Release Auto-Coder 0.1.9 --- ð Attention
 developers! ð¨ The game-changing Auto-Coder has arrived, and it's about to
 take your AI programming to a whole new level! ð Fueled by the incredible
 power of Byzer-LLM, this command-line tool is packed with features that will
 blow your mind: ð Say goodbye to manual context gathering! Auto-Coder
 intelligently generates code based on the context of your source directory.
 It's like having a genius assistant that knows exactly what you need! ð¡ Two
 modes, endless possibilities! Generate perfect prompts to paste into web-based
@@ -19,91 +24,98 @@
 and even modifies code for you. It's like having a super-smart sidekick that
 never sleeps! ð§âð» Developers, prepare to have your minds blown! Auto-
 Coder integrates seamlessly with the hottest AI models like ChatGPT,
 turbocharging your development process to lightning speeds! ð ð Don't
 wait another second! Experience the raw power of Auto-Coder today and let AI be
 your ultimate coding companion! https://github.com/allwefantasy/auto-coder ð¥
 #AutoCoder #AIProgramming #GameChanger #ByzerLLM #DevTools ## Table of Contents
-- [Brand new Installation](#brand-new-installation) - [Existing Installation]
-(#existing-installation) - [Usage](#usage) - [Basic](#basic) - [Advanced]
-(#advanced) - [Python Project Only Features](#python-project-only-features) -
-[TypeScript Project](#typescript-project) - [Real-Auto](#real-auto) - [Real-
-Auto with Search Engine](#real-auto-with-search-engine) ## Brand new
-Installation You can use the script provided by Byzer-LLM to setup the nvidia-
-driver/cuda environment: 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04](https://
-docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy) After the nvidia-driver/
-cuda environment is set up, you can install auto_coder like this: ```shell pip
-install -U auto-coder ``` ## Existing Installation ```shell # or https://
-gitcode.com/allwefantasy11/auto-coder.git git clone https://github.com/
-allwefantasy/auto-coder.git pip install -r requirements.txt ## if you want to
-use private/open-source models, uncomment this line. # pip install -U vllm pip
-install -U byzerllm pip install -U auto-coder ``` ## Usage ### Basic >
-Recommend to use åä¹éé®Max/Qwen-Max-longcontext SaaS model > You should
-deploy the model by [Byzer-LLM](https://github.com/allwefantasy/byzer-llm) The
-auto-coder provide two ways: 1. Generate context for the query and you can
-copy&&Paste to Web UI of ChatGPT/Claud3/Kimi. 2. Use the model from Byzer-LLM
-to generate the result directly. >> Note: You should make sure the model has a
-long context length support, e.g. >32k. The auto-coder will collect the source
-code from the source directory, and then generate context into the target file
-based on the query. Then you can copy the content of `output.txt` and paste it
-to Web UI of ChatGPT/Claud3/Kimi: For example: ```shell auto-coder --source_dir
-/home/winubuntu/projects/ByzerRawCopilot --target_file /home/winubuntu/
-projects/ByzerRawCopilot/output.txt --query "å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿
-auto-coder å½ä»¤æ§è¡ï¼" ``` You can also put all arguments into a yaml
-file: ```yaml # /home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml
-source_dir: /home/winubuntu/projects/ByzerRawCopilot target_file: /home/
-winubuntu/projects/ByzerRawCopilot/output.txt query: |
-å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-coder å½ä»¤æ§è¡ï¼ ``` Then use the
-following command: ```shell auto-coder --file /home/winubuntu/projects/
-ByzerRawCopilot/auto-coder.yaml ``` If you want to use the model from Byzer-
-LLM, you can use the following command: ```shell auto-coder --source_dir /home/
+- [Installation](#installation) - [Brand new Installation](#brand-new-
+installation) - [Usage](#usage) - [Basic](#basic) - [Advanced](#advanced) -
+[Python Project Only Features](#python-project-only-features) - [TypeScript
+Project](#typescript-project) - [Real-Auto](#real-auto) - [Real-Auto with
+Search Engine](#real-auto-with-search-engine) ## Existing Installation ```shell
+# or https://gitcode.com/allwefantasy11/auto-coder.git git clone https://
+github.com/allwefantasy/auto-coder.git pip install -r requirements.txt ## if
+you want to use private/open-source models, uncomment this line. # pip install
+-U vllm pip install -U byzerllm pip install -U auto-coder ray start --head ```
+## Brand new Installation You can use the script provided by Byzer-LLM to setup
+the nvidia-driver/cuda environment: 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04]
+(https://docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy) After the nvidia-
+driver/cuda environment is set up, you can install auto_coder like this:
+```shell pip install -U auto-coder ``` ## Usage ### LLM Model > Recommend to
+use åä¹éé®Max/Qwen-Max-longcontext SaaS model Try to use the following
+command to deploy Qwen-Max: ```shell byzerllm deploy --pretrained_model_type
+saas/qianwen \ --cpus_per_worker 0.01 \ --gpus_per_worker 0 \ --num_workers 1 \
+--infer_params saas.api_key="sk-33cbd1e4a45f477e860035a57b39efa8"
+saas.model="qwen-max" \ --model qianwen_short_chat ``` Then you can use the
+following command to test the model: ```shell byzerllm query --model
+qianwen_short_chat --query "ä½ å¥½" ``` If you want to undeploy the model:
+```shell byzerllm undeploy --model qianwen_short_chat ``` If you want to deploy
+you private/open source model, please try to this [link](https://github.com/
+allwefantasy/byzer-llm) ### Basic The auto-coder provide two ways: 1. Generate
+context for the query and you can copy&&Paste to Web UI of ChatGPT/Claud3/Kimi.
+2. Use the model from Byzer-LLM to generate the result directly. >> Note: You
+should make sure the model has a long context length support, e.g. >32k. The
+auto-coder will collect the source code from the source directory, and then
+generate context into the target file based on the query. Then you can copy the
+content of `output.txt` and paste it to Web UI of ChatGPT/Claud3/Kimi: For
+example: ```shell auto-coder --source_dir /home/winubuntu/projects/
+ByzerRawCopilot --target_file /home/winubuntu/projects/ByzerRawCopilot/
+output.txt --query "å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-coder
+å½ä»¤æ§è¡ï¼" ``` You can also put all arguments into a yaml file: ```yaml #
+/home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml source_dir: /home/
+winubuntu/projects/ByzerRawCopilot target_file: /home/winubuntu/projects/
+ByzerRawCopilot/output.txt query: | å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-
+coder å½ä»¤æ§è¡ï¼ ``` Then use the following command: ```shell auto-coder -
+-file /home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml ``` If you want
+to use the model from Byzer-LLM, you can use the following command: ```shell
+auto-coder --source_dir /home/winubuntu/projects/ByzerRawCopilot --target_file
+/home/winubuntu/projects/ByzerRawCopilot/output.txt --model qianwen_chat --
+execute --query "éæ°çæä¸ä¸ª is_likely_useful_file
+æ¹æ³ï¼æ»¡è¶³reactjs+typescript ç»åçé¡¹ç®ã" ``` In the above command,
+we provide a model and enable the execute mode, the auto-coder will collect the
+source code from the source directory, and then generate context for the query,
+and then use the model to generate the result, then put the result into the
+target file. ### How to reduce the context length? As you may know, auto-coder
+will collect the source code from the source directory, and then generate
+context for the query, if the source directory is too large, the context will
+be too long, and the model may not be able to handle it. There are two ways to
+reduce the context length: 1. Change the source_dir to sub directory of
+project. 2. Enable aut-coder's index feature. In order to use the index
+feature, you should configure some extra parameters: 1. skip_build_index: false
+2. model For example: ```yaml source_dir: /home/winubuntu/projects/
+ByzerRawCopilot target_file: /home/winubuntu/projects/ByzerRawCopilot/
+output.txt model: qianwen_chat model_max_length: 2000 anti_quota_limit: 13
+skip_build_index: false project_type: "copilot/.py" query: | ä¼å copilot
+éç get_suffix_from_project_type å½æ°å¹¶æ´æ°åæä»¶ ``` Here we add a
+new parameter `skip_build_index`, by default, this value is true. If you set it
+to false and a model provide at the same time, then the auto-coder will
+generate index for the source code using the model(This may cost a lot of
+tokens), and the index file will be stored in a directory called `.auto-coder`
+in source directory. Once the index is created, the auto-coder will use the
+index to filter files and reduce the context length. notice that the filter
+action also use model, and it may cost tokens, so you should use it carefully.
+### Advanced > This feature only works with the model from Byzer-LLM. Translate
+the markdown file in the project: ```shell auto-coder --source_dir /home/
 winubuntu/projects/ByzerRawCopilot --target_file /home/winubuntu/projects/
-ByzerRawCopilot/output.txt --model qianwen_chat --execute --query
-"éæ°çæä¸ä¸ª is_likely_useful_file æ¹æ³ï¼æ»¡è¶³reactjs+typescript
-ç»åçé¡¹ç®ã" ``` In the above command, we provide a model and enable the
-execute mode, the auto-coder will collect the source code from the source
-directory, and then generate context for the query, and then use the model to
-generate the result, then put the result into the target file. ### How to
-reduce the context length? As you may know, auto-coder will collect the source
-code from the source directory, and then generate context for the query, if the
-source directory is too large, the context will be too long, and the model may
-not be able to handle it. There are two ways to reduce the context length: 1.
-Change the source_dir to sub directory of project. 2. Enable aut-coder's index
-feature. In order to use the index feature, you should configure some extra
-parameters: 1. skip_build_index: false 2. model For example: ```yaml
-source_dir: /home/winubuntu/projects/ByzerRawCopilot target_file: /home/
-winubuntu/projects/ByzerRawCopilot/output.txt model: qianwen_chat
-model_max_length: 2000 anti_quota_limit: 13 skip_build_index: false
-project_type: "copilot/.py" query: | ä¼å copilot éç
-get_suffix_from_project_type å½æ°å¹¶æ´æ°åæä»¶ ``` Here we add a new
-parameter `skip_build_index`, by default, this value is true. If you set it to
-false and a model provide at the same time, then the auto-coder will generate
-index for the source code using the model(This may cost a lot of tokens), and
-the index file will be stored in a directory called `.auto-coder` in source
-directory. Once the index is created, the auto-coder will use the index to
-filter files and reduce the context length. notice that the filter action also
-use model, and it may cost tokens, so you should use it carefully. ### Advanced
-> This feature only works with the model from Byzer-LLM. Translate the markdown
-file in the project: ```shell auto-coder --source_dir /home/winubuntu/projects/
+ByzerRawCopilot/output.txt --project_type "translate/ä¸­æ/.md/cn" --
+model_max_length 2000 --model qianwen_chat ``` When you want to translate some
+files, you must specify the model parameter. And the project_type is a litle
+bit complex, it's a combination of the following parameters: - translate: the
+project type - ä¸­æ: the target language you want to translate to - .md: the
+file extension you want to translate - cn: the new file suffix created with the
+translated content. for example, if the original file is README.md, the new
+file will be README-cn.md So the final project_type is "translate/ä¸­æ/.md/
+cn" If your model is powerful enough, you can use the following command to do
+the same task: ```shell auto-coder --source_dir /home/winubuntu/projects/
 ByzerRawCopilot --target_file /home/winubuntu/projects/ByzerRawCopilot/
-output.txt --project_type "translate/ä¸­æ/.md/cn" --model_max_length 2000 --
-model qianwen_chat ``` When you want to translate some files, you must specify
-the model parameter. And the project_type is a litle bit complex, it's a
-combination of the following parameters: - translate: the project type -
-ä¸­æ: the target language you want to translate to - .md: the file extension
-you want to translate - cn: the new file suffix created with the translated
-content. for example, if the original file is README.md, the new file will be
-README-cn.md So the final project_type is "translate/ä¸­æ/.md/cn" If your
-model is powerful enough, you can use the following command to do the same
-task: ```shell auto-coder --source_dir /home/winubuntu/projects/ByzerRawCopilot
---target_file /home/winubuntu/projects/ByzerRawCopilot/output.txt --model
-qianwen_chat --project_type translate --model_max_length 2000 --query
-"æé¡¹ç®ä¸­çmarkdownææ¡£ç¿»è¯æä¸­æ" ``` The model will extract
-"translate/ä¸­æ/.md/cn" from the query and then do the same thing as the
-previous command. Note: The model_max_length is used to control the model's
+output.txt --model qianwen_chat --project_type translate --model_max_length
+2000 --query "æé¡¹ç®ä¸­çmarkdownææ¡£ç¿»è¯æä¸­æ" ``` The model will
+extract "translate/ä¸­æ/.md/cn" from the query and then do the same thing as
+the previous command. Note: The model_max_length is used to control the model's
 generation length, if the model_max_length is not set, the default value is
 1024. You should change the value based on your esitmating on the length of the
 translation. ### Python Project Only Features In order to reduce the context
 length collected by the auto-coder, if you are dealing with a python project,
 you can use the following command: ```shell auto-coder --target_file /home/
 winubuntu/projects/ByzerRawCopilot/output.txt --script_path /home/winubuntu/
 projects/ByzerRawCopilot/xxx --package_name byzer_copilot --project_type py-
@@ -150,22 +162,26 @@
 output.txt model: qianwen_short_chat model_max_length: 2000 anti_quota_limit: 5
 search_engine: bing search_engine_token: xxxxxx project_type: "copilot" query:
 | å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
 ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project ``` Here we add new parameters
 `search_engine` and `search_engine_token`, the search engine will provide more
 context for the model, and the model will use the context to generate the
 result. For now, we support bing/google. If you use bing, try to get the token
-from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api).
-Here is the output: ```text ç¨æ·å°è¯: UserIntent.CREATE_NEW_PROJECT search
-SearchEngine.BING for å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
-ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project... reraking the search result by
-snippets... fetch https://blog.csdn.net/weixin_42429718/article/details/
-117402097 and answer the quesion (å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª
-typescript + reactjs ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project) based on the
-full content... user:
+from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api). The
+basic workflow is: 1. search the query 2. reranking the search result by
+snippets 3. fetch the first search result and answer the question based on the
+full content. 4. generate the result based on the query and the full content.
+5. get execute steps based on the result. 5. execute the steps by ShellClient/
+PythonClient in auto-coder. Here is the output: ```text ç¨æ·å°è¯:
+UserIntent.CREATE_NEW_PROJECT search SearchEngine.BING for å¸®æå¨/tmp/
+ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-
+project... reraking the search result by snippets... fetch https://
+blog.csdn.net/weixin_42429718/article/details/117402097 and answer the quesion
+(å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
+ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project) based on the full content... user:
 ä½ çæåç§ç¼ç¨è¯­è¨ä»¥åç¸å³æ¡æ¶å¯¹åºçé¡¹ç®ç»æãç°å¨ï¼ä½ éè¦
 æ ¹æ®ç¨æ·çé®é¢ï¼æ ¹æ®æä¾çä¿¡æ¯ï¼å¯¹é®é¢è¿è¡æè§£ï¼ç¶åçææ§è¡æ­¥éª¤ï¼å½æ§è¡å®æææ­¥éª¤ï¼æç»å¸®çæä¸ä¸ªç¬¦åå¯¹åºç¼ç¨è¯­è¨è§èä»¥åç¸å³æ¡æ¶çé¡¹ç®ç»æã
 æ´ä¸ªè¿ç¨åªè½ä½¿ç¨ python/shellã ç¯å¢ä¿¡æ¯å¦ä¸: æä½ç³»ç»:
 linux 5.15.0-48-generic Pythonçæ¬: 3.10.11 Condaç¯å¢: byzerllm-dev
 æ¯æBash ç°å¨è¯·åèä¸é¢åå®¹ï¼
 ç±äºæä¾çä¸ä¸æä¿¡æ¯ä¸å¨Linuxç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åå»ºä¸ä¸ªTypeScriptåReactJSé¡¹ç®æ å³ï¼æå°åºäºä¸è¬æä½æ­¥éª¤ç»åºè§£ç­ã
 è¦å¨Linuxç³»ç»ç `/tmp/
```

### Comparing `auto-coder-0.1.8/setup.py` & `auto-coder-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/auto_coder.egg-info/PKG-INFO` & `auto-coder-0.1.9/src/auto_coder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-coder
-Version: 0.1.8
+Version: 0.1.9
 Summary: AutoCoder: AutoCoder
 Author: allwefantasy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 
@@ -23,15 +23,15 @@
 
 </p>
 
 ---
 
 *Latest News* 🔥
 
-- [2024/03] Release Auto-Coder 0.1.7
+- [2024/03] Release Auto-Coder 0.1.9
 
 ---
 
 
 
 🚀 Attention developers! 🚨 The game-changing Auto-Coder has arrived, and it's about to take your AI programming to a whole new level! 🌟
 
@@ -51,57 +51,85 @@
 
 🌟 Don't wait another second! Experience the raw power of Auto-Coder today and let AI be your ultimate coding companion! https://github.com/allwefantasy/auto-coder 🔥
 
 #AutoCoder #AIProgramming #GameChanger #ByzerLLM #DevTools
 
 ## Table of Contents
 
+- [Installation](#installation)
 - [Brand new Installation](#brand-new-installation)
-- [Existing Installation](#existing-installation)
 - [Usage](#usage)
   - [Basic](#basic)
   - [Advanced](#advanced)
   - [Python Project Only Features](#python-project-only-features)
   - [TypeScript Project](#typescript-project)
   - [Real-Auto](#real-auto)
     - [Real-Auto with Search Engine](#real-auto-with-search-engine)
 
 
 
+## Existing Installation
+
+```shell
+# or https://gitcode.com/allwefantasy11/auto-coder.git
+git clone https://github.com/allwefantasy/auto-coder.git
+pip install -r requirements.txt
+## if you want to use private/open-source models, uncomment this line.
+# pip install -U vllm
+pip install -U byzerllm
+pip install -U auto-coder
+
+ray start --head
+```
 
 ## Brand new Installation
 
 You can use the script provided by Byzer-LLM to setup the nvidia-driver/cuda environment:
 
 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04](https://docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy)
 
 After the nvidia-driver/cuda environment is set up, you can install auto_coder like this:
 
 ```shell
 pip install -U auto-coder
 ```
 
-## Existing Installation
 
+## Usage 
+
+### LLM Model
+
+> Recommend to use 千义通问Max/Qwen-Max-longcontext SaaS model
+
+Try to use the following command to deploy Qwen-Max:
 
 ```shell
-# or https://gitcode.com/allwefantasy11/auto-coder.git
-git clone https://github.com/allwefantasy/auto-coder.git
-pip install -r requirements.txt
-## if you want to use private/open-source models, uncomment this line.
-# pip install -U vllm
-pip install -U byzerllm
-pip install -U auto-coder
+byzerllm deploy  --pretrained_model_type saas/qianwen \
+--cpus_per_worker 0.01 \
+--gpus_per_worker 0 \
+--num_workers 1 \
+--infer_params saas.api_key="sk-33cbd1e4a45f477e860035a57b39efa8" saas.model="qwen-max" \
+--model qianwen_short_chat 
 ```
 
-## Usage 
+Then you can use the following command to test the model:
+
+```shell
+byzerllm query --model qianwen_short_chat --query "你好"
+```
+
+If you want to undeploy the model:
+
+```shell
+byzerllm undeploy --model qianwen_short_chat
+```
+
+If you want to deploy you private/open source model, please try to this [link](https://github.com/allwefantasy/byzer-llm)
 
 ### Basic 
-> Recommend to use 千义通问Max/Qwen-Max-longcontext SaaS model
-> You should deploy the model by [Byzer-LLM](https://github.com/allwefantasy/byzer-llm)
 
 
 The auto-coder provide two ways:
 
 1. Generate context for the query and you can copy&&Paste to Web UI of ChatGPT/Claud3/Kimi.
 2. Use the model from Byzer-LLM to generate the result directly.
 
@@ -157,18 +185,21 @@
 2. model
 
 For example:
 
 ```yaml
 source_dir: /home/winubuntu/projects/ByzerRawCopilot 
 target_file: /home/winubuntu/projects/ByzerRawCopilot/output.txt 
+
 model: qianwen_chat
 model_max_length: 2000
 anti_quota_limit: 13
+
 skip_build_index: false
+
 project_type: "copilot/.py"
 query: |
   优化 copilot 里的 get_suffix_from_project_type 函数并更新原文件
 ```
 
 Here we add a new parameter `skip_build_index`, by default, this value is true. 
 If you set it to false and a model provide at the same time, then the auto-coder will generate index for the source code using the model(This may cost a lot of tokens), and the index file will be stored in a directory called `.auto-coder` in source directory. 
@@ -314,14 +345,23 @@
   帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project
 ```
 
 Here we add  new parameters  `search_engine` and `search_engine_token`, the search engine will provide more context for the model, and the model will use the context to generate the result.
 
 For now, we support bing/google.  If you use bing, try to get the token from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api).
 
+The basic workflow is:
+
+1. search the query 
+2. reranking the search result by snippets
+3. fetch the first search result and answer the question based on the full content.
+4. generate the result based on the query and the full content.
+5. get execute steps based on the result.
+5. execute the steps by ShellClient/PythonClient in auto-coder.
+
 Here is the output:
 
 ```text
 用户尝试: UserIntent.CREATE_NEW_PROJECT
 search SearchEngine.BING for 帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project...
 reraking the search result by snippets...
 fetch https://blog.csdn.net/weixin_42429718/article/details/117402097 and answer the quesion (帮我在/tmp/目录下创建一个 typescript + reactjs 组成的项目，项目名字叫 t-project) based on the full content...
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: auto-coder Version: 0.1.8 Summary: AutoCoder:
+Metadata-Version: 2.1 Name: auto-coder Version: 0.1.9 Summary: AutoCoder:
 AutoCoder Author: allwefantasy Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Description-Content-Type:
 text/markdown
                                  [auto-coder]
                   ******** AAuuttoo--CCooddeerr ((ppoowweerreedd bbyy BByyzzeerr--LLLLMM)) ********
                              | _EE_nn_gg_ll_ii_ss_hh | _?ä_?¸_?­_?æ_?_? |
---- *Latest News* ð¥ - [2024/03] Release Auto-Coder 0.1.7 --- ð Attention
+--- *Latest News* ð¥ - [2024/03] Release Auto-Coder 0.1.9 --- ð Attention
 developers! ð¨ The game-changing Auto-Coder has arrived, and it's about to
 take your AI programming to a whole new level! ð Fueled by the incredible
 power of Byzer-LLM, this command-line tool is packed with features that will
 blow your mind: ð Say goodbye to manual context gathering! Auto-Coder
 intelligently generates code based on the context of your source directory.
 It's like having a genius assistant that knows exactly what you need! ð¡ Two
 modes, endless possibilities! Generate perfect prompts to paste into web-based
@@ -24,91 +24,98 @@
 and even modifies code for you. It's like having a super-smart sidekick that
 never sleeps! ð§âð» Developers, prepare to have your minds blown! Auto-
 Coder integrates seamlessly with the hottest AI models like ChatGPT,
 turbocharging your development process to lightning speeds! ð ð Don't
 wait another second! Experience the raw power of Auto-Coder today and let AI be
 your ultimate coding companion! https://github.com/allwefantasy/auto-coder ð¥
 #AutoCoder #AIProgramming #GameChanger #ByzerLLM #DevTools ## Table of Contents
-- [Brand new Installation](#brand-new-installation) - [Existing Installation]
-(#existing-installation) - [Usage](#usage) - [Basic](#basic) - [Advanced]
-(#advanced) - [Python Project Only Features](#python-project-only-features) -
-[TypeScript Project](#typescript-project) - [Real-Auto](#real-auto) - [Real-
-Auto with Search Engine](#real-auto-with-search-engine) ## Brand new
-Installation You can use the script provided by Byzer-LLM to setup the nvidia-
-driver/cuda environment: 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04](https://
-docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy) After the nvidia-driver/
-cuda environment is set up, you can install auto_coder like this: ```shell pip
-install -U auto-coder ``` ## Existing Installation ```shell # or https://
-gitcode.com/allwefantasy11/auto-coder.git git clone https://github.com/
-allwefantasy/auto-coder.git pip install -r requirements.txt ## if you want to
-use private/open-source models, uncomment this line. # pip install -U vllm pip
-install -U byzerllm pip install -U auto-coder ``` ## Usage ### Basic >
-Recommend to use åä¹éé®Max/Qwen-Max-longcontext SaaS model > You should
-deploy the model by [Byzer-LLM](https://github.com/allwefantasy/byzer-llm) The
-auto-coder provide two ways: 1. Generate context for the query and you can
-copy&&Paste to Web UI of ChatGPT/Claud3/Kimi. 2. Use the model from Byzer-LLM
-to generate the result directly. >> Note: You should make sure the model has a
-long context length support, e.g. >32k. The auto-coder will collect the source
-code from the source directory, and then generate context into the target file
-based on the query. Then you can copy the content of `output.txt` and paste it
-to Web UI of ChatGPT/Claud3/Kimi: For example: ```shell auto-coder --source_dir
-/home/winubuntu/projects/ByzerRawCopilot --target_file /home/winubuntu/
-projects/ByzerRawCopilot/output.txt --query "å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿
-auto-coder å½ä»¤æ§è¡ï¼" ``` You can also put all arguments into a yaml
-file: ```yaml # /home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml
-source_dir: /home/winubuntu/projects/ByzerRawCopilot target_file: /home/
-winubuntu/projects/ByzerRawCopilot/output.txt query: |
-å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-coder å½ä»¤æ§è¡ï¼ ``` Then use the
-following command: ```shell auto-coder --file /home/winubuntu/projects/
-ByzerRawCopilot/auto-coder.yaml ``` If you want to use the model from Byzer-
-LLM, you can use the following command: ```shell auto-coder --source_dir /home/
+- [Installation](#installation) - [Brand new Installation](#brand-new-
+installation) - [Usage](#usage) - [Basic](#basic) - [Advanced](#advanced) -
+[Python Project Only Features](#python-project-only-features) - [TypeScript
+Project](#typescript-project) - [Real-Auto](#real-auto) - [Real-Auto with
+Search Engine](#real-auto-with-search-engine) ## Existing Installation ```shell
+# or https://gitcode.com/allwefantasy11/auto-coder.git git clone https://
+github.com/allwefantasy/auto-coder.git pip install -r requirements.txt ## if
+you want to use private/open-source models, uncomment this line. # pip install
+-U vllm pip install -U byzerllm pip install -U auto-coder ray start --head ```
+## Brand new Installation You can use the script provided by Byzer-LLM to setup
+the nvidia-driver/cuda environment: 1. [CentOS 8 / Ubuntu 20.04 / Ubuntu 22.04]
+(https://docs.byzer.org/#/byzer-lang/zh-cn/byzer-llm/deploy) After the nvidia-
+driver/cuda environment is set up, you can install auto_coder like this:
+```shell pip install -U auto-coder ``` ## Usage ### LLM Model > Recommend to
+use åä¹éé®Max/Qwen-Max-longcontext SaaS model Try to use the following
+command to deploy Qwen-Max: ```shell byzerllm deploy --pretrained_model_type
+saas/qianwen \ --cpus_per_worker 0.01 \ --gpus_per_worker 0 \ --num_workers 1 \
+--infer_params saas.api_key="sk-33cbd1e4a45f477e860035a57b39efa8"
+saas.model="qwen-max" \ --model qianwen_short_chat ``` Then you can use the
+following command to test the model: ```shell byzerllm query --model
+qianwen_short_chat --query "ä½ å¥½" ``` If you want to undeploy the model:
+```shell byzerllm undeploy --model qianwen_short_chat ``` If you want to deploy
+you private/open source model, please try to this [link](https://github.com/
+allwefantasy/byzer-llm) ### Basic The auto-coder provide two ways: 1. Generate
+context for the query and you can copy&&Paste to Web UI of ChatGPT/Claud3/Kimi.
+2. Use the model from Byzer-LLM to generate the result directly. >> Note: You
+should make sure the model has a long context length support, e.g. >32k. The
+auto-coder will collect the source code from the source directory, and then
+generate context into the target file based on the query. Then you can copy the
+content of `output.txt` and paste it to Web UI of ChatGPT/Claud3/Kimi: For
+example: ```shell auto-coder --source_dir /home/winubuntu/projects/
+ByzerRawCopilot --target_file /home/winubuntu/projects/ByzerRawCopilot/
+output.txt --query "å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-coder
+å½ä»¤æ§è¡ï¼" ``` You can also put all arguments into a yaml file: ```yaml #
+/home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml source_dir: /home/
+winubuntu/projects/ByzerRawCopilot target_file: /home/winubuntu/projects/
+ByzerRawCopilot/output.txt query: | å¦ä½è®©è¿ä¸ªç³»ç»å¯ä»¥éè¿ auto-
+coder å½ä»¤æ§è¡ï¼ ``` Then use the following command: ```shell auto-coder -
+-file /home/winubuntu/projects/ByzerRawCopilot/auto-coder.yaml ``` If you want
+to use the model from Byzer-LLM, you can use the following command: ```shell
+auto-coder --source_dir /home/winubuntu/projects/ByzerRawCopilot --target_file
+/home/winubuntu/projects/ByzerRawCopilot/output.txt --model qianwen_chat --
+execute --query "éæ°çæä¸ä¸ª is_likely_useful_file
+æ¹æ³ï¼æ»¡è¶³reactjs+typescript ç»åçé¡¹ç®ã" ``` In the above command,
+we provide a model and enable the execute mode, the auto-coder will collect the
+source code from the source directory, and then generate context for the query,
+and then use the model to generate the result, then put the result into the
+target file. ### How to reduce the context length? As you may know, auto-coder
+will collect the source code from the source directory, and then generate
+context for the query, if the source directory is too large, the context will
+be too long, and the model may not be able to handle it. There are two ways to
+reduce the context length: 1. Change the source_dir to sub directory of
+project. 2. Enable aut-coder's index feature. In order to use the index
+feature, you should configure some extra parameters: 1. skip_build_index: false
+2. model For example: ```yaml source_dir: /home/winubuntu/projects/
+ByzerRawCopilot target_file: /home/winubuntu/projects/ByzerRawCopilot/
+output.txt model: qianwen_chat model_max_length: 2000 anti_quota_limit: 13
+skip_build_index: false project_type: "copilot/.py" query: | ä¼å copilot
+éç get_suffix_from_project_type å½æ°å¹¶æ´æ°åæä»¶ ``` Here we add a
+new parameter `skip_build_index`, by default, this value is true. If you set it
+to false and a model provide at the same time, then the auto-coder will
+generate index for the source code using the model(This may cost a lot of
+tokens), and the index file will be stored in a directory called `.auto-coder`
+in source directory. Once the index is created, the auto-coder will use the
+index to filter files and reduce the context length. notice that the filter
+action also use model, and it may cost tokens, so you should use it carefully.
+### Advanced > This feature only works with the model from Byzer-LLM. Translate
+the markdown file in the project: ```shell auto-coder --source_dir /home/
 winubuntu/projects/ByzerRawCopilot --target_file /home/winubuntu/projects/
-ByzerRawCopilot/output.txt --model qianwen_chat --execute --query
-"éæ°çæä¸ä¸ª is_likely_useful_file æ¹æ³ï¼æ»¡è¶³reactjs+typescript
-ç»åçé¡¹ç®ã" ``` In the above command, we provide a model and enable the
-execute mode, the auto-coder will collect the source code from the source
-directory, and then generate context for the query, and then use the model to
-generate the result, then put the result into the target file. ### How to
-reduce the context length? As you may know, auto-coder will collect the source
-code from the source directory, and then generate context for the query, if the
-source directory is too large, the context will be too long, and the model may
-not be able to handle it. There are two ways to reduce the context length: 1.
-Change the source_dir to sub directory of project. 2. Enable aut-coder's index
-feature. In order to use the index feature, you should configure some extra
-parameters: 1. skip_build_index: false 2. model For example: ```yaml
-source_dir: /home/winubuntu/projects/ByzerRawCopilot target_file: /home/
-winubuntu/projects/ByzerRawCopilot/output.txt model: qianwen_chat
-model_max_length: 2000 anti_quota_limit: 13 skip_build_index: false
-project_type: "copilot/.py" query: | ä¼å copilot éç
-get_suffix_from_project_type å½æ°å¹¶æ´æ°åæä»¶ ``` Here we add a new
-parameter `skip_build_index`, by default, this value is true. If you set it to
-false and a model provide at the same time, then the auto-coder will generate
-index for the source code using the model(This may cost a lot of tokens), and
-the index file will be stored in a directory called `.auto-coder` in source
-directory. Once the index is created, the auto-coder will use the index to
-filter files and reduce the context length. notice that the filter action also
-use model, and it may cost tokens, so you should use it carefully. ### Advanced
-> This feature only works with the model from Byzer-LLM. Translate the markdown
-file in the project: ```shell auto-coder --source_dir /home/winubuntu/projects/
+ByzerRawCopilot/output.txt --project_type "translate/ä¸­æ/.md/cn" --
+model_max_length 2000 --model qianwen_chat ``` When you want to translate some
+files, you must specify the model parameter. And the project_type is a litle
+bit complex, it's a combination of the following parameters: - translate: the
+project type - ä¸­æ: the target language you want to translate to - .md: the
+file extension you want to translate - cn: the new file suffix created with the
+translated content. for example, if the original file is README.md, the new
+file will be README-cn.md So the final project_type is "translate/ä¸­æ/.md/
+cn" If your model is powerful enough, you can use the following command to do
+the same task: ```shell auto-coder --source_dir /home/winubuntu/projects/
 ByzerRawCopilot --target_file /home/winubuntu/projects/ByzerRawCopilot/
-output.txt --project_type "translate/ä¸­æ/.md/cn" --model_max_length 2000 --
-model qianwen_chat ``` When you want to translate some files, you must specify
-the model parameter. And the project_type is a litle bit complex, it's a
-combination of the following parameters: - translate: the project type -
-ä¸­æ: the target language you want to translate to - .md: the file extension
-you want to translate - cn: the new file suffix created with the translated
-content. for example, if the original file is README.md, the new file will be
-README-cn.md So the final project_type is "translate/ä¸­æ/.md/cn" If your
-model is powerful enough, you can use the following command to do the same
-task: ```shell auto-coder --source_dir /home/winubuntu/projects/ByzerRawCopilot
---target_file /home/winubuntu/projects/ByzerRawCopilot/output.txt --model
-qianwen_chat --project_type translate --model_max_length 2000 --query
-"æé¡¹ç®ä¸­çmarkdownææ¡£ç¿»è¯æä¸­æ" ``` The model will extract
-"translate/ä¸­æ/.md/cn" from the query and then do the same thing as the
-previous command. Note: The model_max_length is used to control the model's
+output.txt --model qianwen_chat --project_type translate --model_max_length
+2000 --query "æé¡¹ç®ä¸­çmarkdownææ¡£ç¿»è¯æä¸­æ" ``` The model will
+extract "translate/ä¸­æ/.md/cn" from the query and then do the same thing as
+the previous command. Note: The model_max_length is used to control the model's
 generation length, if the model_max_length is not set, the default value is
 1024. You should change the value based on your esitmating on the length of the
 translation. ### Python Project Only Features In order to reduce the context
 length collected by the auto-coder, if you are dealing with a python project,
 you can use the following command: ```shell auto-coder --target_file /home/
 winubuntu/projects/ByzerRawCopilot/output.txt --script_path /home/winubuntu/
 projects/ByzerRawCopilot/xxx --package_name byzer_copilot --project_type py-
@@ -155,22 +162,26 @@
 output.txt model: qianwen_short_chat model_max_length: 2000 anti_quota_limit: 5
 search_engine: bing search_engine_token: xxxxxx project_type: "copilot" query:
 | å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
 ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project ``` Here we add new parameters
 `search_engine` and `search_engine_token`, the search engine will provide more
 context for the model, and the model will use the context to generate the
 result. For now, we support bing/google. If you use bing, try to get the token
-from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api).
-Here is the output: ```text ç¨æ·å°è¯: UserIntent.CREATE_NEW_PROJECT search
-SearchEngine.BING for å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
-ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project... reraking the search result by
-snippets... fetch https://blog.csdn.net/weixin_42429718/article/details/
-117402097 and answer the quesion (å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª
-typescript + reactjs ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project) based on the
-full content... user:
+from [here](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api). The
+basic workflow is: 1. search the query 2. reranking the search result by
+snippets 3. fetch the first search result and answer the question based on the
+full content. 4. generate the result based on the query and the full content.
+5. get execute steps based on the result. 5. execute the steps by ShellClient/
+PythonClient in auto-coder. Here is the output: ```text ç¨æ·å°è¯:
+UserIntent.CREATE_NEW_PROJECT search SearchEngine.BING for å¸®æå¨/tmp/
+ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-
+project... reraking the search result by snippets... fetch https://
+blog.csdn.net/weixin_42429718/article/details/117402097 and answer the quesion
+(å¸®æå¨/tmp/ç®å½ä¸åå»ºä¸ä¸ª typescript + reactjs
+ç»æçé¡¹ç®ï¼é¡¹ç®åå­å« t-project) based on the full content... user:
 ä½ çæåç§ç¼ç¨è¯­è¨ä»¥åç¸å³æ¡æ¶å¯¹åºçé¡¹ç®ç»æãç°å¨ï¼ä½ éè¦
 æ ¹æ®ç¨æ·çé®é¢ï¼æ ¹æ®æä¾çä¿¡æ¯ï¼å¯¹é®é¢è¿è¡æè§£ï¼ç¶åçææ§è¡æ­¥éª¤ï¼å½æ§è¡å®æææ­¥éª¤ï¼æç»å¸®çæä¸ä¸ªç¬¦åå¯¹åºç¼ç¨è¯­è¨è§èä»¥åç¸å³æ¡æ¶çé¡¹ç®ç»æã
 æ´ä¸ªè¿ç¨åªè½ä½¿ç¨ python/shellã ç¯å¢ä¿¡æ¯å¦ä¸: æä½ç³»ç»:
 linux 5.15.0-48-generic Pythonçæ¬: 3.10.11 Condaç¯å¢: byzerllm-dev
 æ¯æBash ç°å¨è¯·åèä¸é¢åå®¹ï¼
 ç±äºæä¾çä¸ä¸æä¿¡æ¯ä¸å¨Linuxç¯å¢ä¸ä½¿ç¨å½ä»¤è¡åå»ºä¸ä¸ªTypeScriptåReactJSé¡¹ç®æ å³ï¼æå°åºäºä¸è¬æä½æ­¥éª¤ç»åºè§£ç­ã
 è¦å¨Linuxç³»ç»ç `/tmp/
```

### Comparing `auto-coder-0.1.8/src/auto_coder.egg-info/SOURCES.txt` & `auto-coder-0.1.9/src/auto_coder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/auto_coder.py` & `auto-coder-0.1.9/src/autocoder/auto_coder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import byzerllm
 from typing import List,Dict,Any,Optional
 import argparse 
 from autocoder.common import AutoCoderArgs
 from autocoder.dispacher import Dispacher 
 import yaml   
 import locale
+import os
+from jinja2 import Template
+
 lang_desc = {
     "en": {
         "parser_desc": "Auto-implement missing methods in a Python script.",
         "source_dir": "Path to the project source code directory",
         "git_url": "URL of the git repository to clone the source code from",
         "target_file": "The file path to write the generated source code to",
         "query": "The user query or instruction to handle the source code",
@@ -91,15 +94,19 @@
 
 def main():
     args = parse_args()
     if args.file:
         with open(args.file, "r") as f:
             config = yaml.safe_load(f)
             for key, value in config.items():
-                if key != "file":  # 排除 --file 参数本身
+                if key != "file":  # 排除 --file 参数本身   
+                    ## key: ENV {{VARIABLE_NAME}}
+                    if isinstance(value, str) and value.startswith("ENV"):  
+                        template = Template(value.removeprefix("ENV").strip())                  
+                        value = template.render(os.environ)                        
                     setattr(args, key, value)
     
     print("Command Line Arguments:")
     print("-" * 50)
     for arg, value in vars(args).items():
         print(f"{arg:20}: {value}")
     print("-" * 50)
```

### Comparing `auto-coder-0.1.8/src/autocoder/common/JupyterClient.py` & `auto-coder-0.1.9/src/autocoder/common/JupyterClient.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/common/ShellClient.py` & `auto-coder-0.1.9/src/autocoder/common/ShellClient.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/common/__init__.py` & `auto-coder-0.1.9/src/autocoder/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     urls: str = pydantic.Field("", description="The urls to crawl and extract text from, separated by comma")
     search_engine: str = ""
     search_engine_token: str = ""
 
 
 def is_likely_useful_file(file_path):
     """Determine if the file is likely to be useful by excluding certain directories and specific file types."""
-    excluded_dirs = ["docs", "examples", "tests", "test", "__pycache__", "scripts", "benchmarks"]
+    excluded_dirs = ["docs", "examples", "tests", "test", "__pycache__", "scripts", "benchmarks","build"]
     utility_or_config_files = ["hubconf.py", "setup.py"]
     github_workflow_or_docs = ["stale.py", "gen-card-", "write_model_card"]
     
     if any(part.startswith('.') for part in file_path.split('/')):
         return False
     if 'test' in file_path.lower():
         return False
```

### Comparing `auto-coder-0.1.8/src/autocoder/common/cleaner.py` & `auto-coder-0.1.9/src/autocoder/common/cleaner.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/common/const.py` & `auto-coder-0.1.9/src/autocoder/common/const.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/common/search.py` & `auto-coder-0.1.9/src/autocoder/common/search.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/dispacher/__init__.py` & `auto-coder-0.1.9/src/autocoder/dispacher/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/dispacher/actions/action.py` & `auto-coder-0.1.9/src/autocoder/dispacher/actions/action.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/dispacher/actions/copilot.py` & `auto-coder-0.1.9/src/autocoder/dispacher/actions/copilot.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/index/index.py` & `auto-coder-0.1.9/src/autocoder/index/index.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/pyproject/__init__.py` & `auto-coder-0.1.9/src/autocoder/pyproject/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     def get_rest_source_codes(self) -> Generator[SourceCode, None, None]:
         if self.args.urls:
             http_doc = HttpDoc(urls=self.args.urls.split(","), llm=self.llm)
             sources = http_doc.crawl_urls()         
             return sources
         return []    
 
-    def get_source_codes(self)->Generator[SourceCode,None,None]:
+    def get_source_codes(self)->Generator[SourceCode,None,None]:        
         for root, dirs, files in os.walk(self.directory):
             for file in files:
                 file_path = os.path.join(root, file)
                 if self.is_python_file(file_path):
                     source_code = self.convert_to_source_code(file_path)
                     if source_code is not None:
                         yield source_code
```

### Comparing `auto-coder-0.1.8/src/autocoder/suffixproject/__init__.py` & `auto-coder-0.1.9/src/autocoder/suffixproject/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/tsproject/__init__.py` & `auto-coder-0.1.9/src/autocoder/tsproject/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-coder-0.1.8/src/autocoder/utils/rest.py` & `auto-coder-0.1.9/src/autocoder/utils/rest.py`

 * *Files identical despite different names*

