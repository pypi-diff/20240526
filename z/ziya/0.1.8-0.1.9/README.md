# Comparing `tmp/ziya-0.1.8.tar.gz` & `tmp/ziya-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziya-0.1.8.tar", max compression
+gzip compressed data, was "ziya-0.1.9.tar", max compression
```

## Comparing `ziya-0.1.8.tar` & `ziya-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,35 @@
--rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.8/LICENSE
--rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.8/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.8/app/agents/__init__.py
--rw-r--r--   0        0        0     4382 2024-04-27 20:53:42.937406 ziya-0.1.8/app/agents/agent.py
--rw-r--r--   0        0        0     1674 2024-04-22 03:14:43.793776 ziya-0.1.8/app/agents/prompts.py
--rw-r--r--   0        0        0     3146 2024-04-27 20:21:37.939016 ziya-0.1.8/app/main.py
--rw-r--r--   0        0        0      676 2024-04-22 03:14:43.793985 ziya-0.1.8/app/server.py
--rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.8/app/utils/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-27 03:12:25.454451 ziya-0.1.8/app/utils/directory_util.py
--rw-r--r--   0        0        0     7496 2024-04-22 03:14:43.794305 ziya-0.1.8/app/utils/gitignore_parser.py
--rw-r--r--   0        0        0      527 2024-04-27 20:33:01.898238 ziya-0.1.8/app/utils/langchain_validation_util.py
--rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.8/app/utils/logging_utils.py
--rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.8/app/utils/print_tree_util.py
--rw-r--r--   0        0        0      631 2024-04-27 19:40:53.572399 ziya-0.1.8/app/utils/version_util.py
--rw-r--r--   0        0        0      716 2024-04-28 01:54:07.699255 ziya-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5513 2024-04-28 01:53:16.706202 ziya-0.1.8/static/app.js
--rw-r--r--   0        0        0    15086 2024-04-22 03:14:43.795783 ziya-0.1.8/static/favicon.ico
--rw-r--r--   0        0        0     1956 2024-04-22 03:14:43.795889 ziya-0.1.8/static/sendPayload.js
--rw-r--r--   0        0        0     1395 2024-04-28 01:21:44.865881 ziya-0.1.8/static/ziya.css
--rw-r--r--   0        0        0      800 2024-04-28 01:20:35.489775 ziya-0.1.8/templates/index.html
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 ziya-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 03:14:32.272276 ziya-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2072 2024-04-26 01:28:16.357186 ziya-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793375 ziya-0.1.9/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.793453 ziya-0.1.9/app/agents/__init__.py
+-rw-r--r--   0        0        0     5363 2024-05-18 17:16:27.553846 ziya-0.1.9/app/agents/agent.py
+-rw-r--r--   0        0        0     1747 2024-05-18 17:16:26.715212 ziya-0.1.9/app/agents/prompts.py
+-rw-r--r--   0        0        0     2819 2024-05-18 17:16:27.554141 ziya-0.1.9/app/main.py
+-rw-r--r--   0        0        0     3199 2024-05-18 20:41:15.047537 ziya-0.1.9/app/server.py
+-rw-r--r--   0        0        0        0 2024-04-22 03:14:43.794018 ziya-0.1.9/app/utils/__init__.py
+-rw-r--r--   0        0        0     2762 2024-05-18 17:16:27.554809 ziya-0.1.9/app/utils/directory_util.py
+-rw-r--r--   0        0        0     7425 2024-05-18 17:16:27.555102 ziya-0.1.9/app/utils/gitignore_parser.py
+-rw-r--r--   0        0        0      527 2024-04-27 20:33:01.898238 ziya-0.1.9/app/utils/langchain_validation_util.py
+-rw-r--r--   0        0        0      280 2024-04-22 03:14:43.794403 ziya-0.1.9/app/utils/logging_utils.py
+-rw-r--r--   0        0        0     1419 2024-04-22 03:14:43.794504 ziya-0.1.9/app/utils/print_tree_util.py
+-rw-r--r--   0        0        0      631 2024-04-27 19:40:53.572399 ziya-0.1.9/app/utils/version_util.py
+-rw-r--r--   0        0        0      803 2024-05-18 20:39:25.230814 ziya-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      809 2024-05-18 20:42:29.812232 ziya-0.1.9/scripts.py
+-rw-r--r--   0        0        0     6148 2024-05-05 15:45:58.377644 ziya-0.1.9/templates/.DS_Store
+-rw-r--r--   0        0        0     1157 2024-05-18 20:44:21.935759 ziya-0.1.9/templates/asset-manifest.json
+-rw-r--r--   0        0        0    15086 2024-05-18 20:44:21.936040 ziya-0.1.9/templates/favicon.ico
+-rw-r--r--   0        0        0      465 2024-05-18 20:44:21.936180 ziya-0.1.9/templates/index.html
+-rw-r--r--   0        0        0   103690 2024-05-18 20:44:21.936662 ziya-0.1.9/templates/static/css/main.85c755f1.css
+-rw-r--r--   0        0        0   151536 2024-05-18 20:44:21.936873 ziya-0.1.9/templates/static/css/main.85c755f1.css.map
+-rw-r--r--   0        0        0   191420 2024-05-18 20:44:21.937212 ziya-0.1.9/templates/static/js/main.d47d0f10.js
+-rw-r--r--   0        0        0      971 2024-05-18 20:44:21.940800 ziya-0.1.9/templates/static/js/main.d47d0f10.js.LICENSE.txt
+-rw-r--r--   0        0        0   481332 2024-05-18 20:44:21.940643 ziya-0.1.9/templates/static/js/main.d47d0f10.js.map
+-rw-r--r--   0        0        0   117852 2024-05-18 20:44:21.943024 ziya-0.1.9/templates/static/media/fa-brands-400.455ea818179b4def0c43.woff2
+-rw-r--r--   0        0        0   209128 2024-05-18 20:44:21.941245 ziya-0.1.9/templates/static/media/fa-brands-400.60127e352b7a11f7f1bc.ttf
+-rw-r--r--   0        0        0    25392 2024-05-18 20:44:21.943739 ziya-0.1.9/templates/static/media/fa-regular-400.21cb8f55d8e0c5b89751.woff2
+-rw-r--r--   0        0        0    67860 2024-05-18 20:44:21.942008 ziya-0.1.9/templates/static/media/fa-regular-400.eb91f7b948a42799f678.ttf
+-rw-r--r--   0        0        0   156400 2024-05-18 20:44:21.942674 ziya-0.1.9/templates/static/media/fa-solid-900.4d986b00ff9ca3828fbd.woff2
+-rw-r--r--   0        0        0   420332 2024-05-18 20:44:21.941814 ziya-0.1.9/templates/static/media/fa-solid-900.bacd5de623fb563b961a.ttf
+-rw-r--r--   0        0        0    10832 2024-05-18 20:44:21.943921 ziya-0.1.9/templates/static/media/fa-v4compatibility.c8e090db312b0bea2aa2.ttf
+-rw-r--r--   0        0        0     4792 2024-05-18 20:44:21.942853 ziya-0.1.9/templates/static/media/fa-v4compatibility.cf7f5903d06b79ad60f1.woff2
+-rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 ziya-0.1.9/PKG-INFO
```

### Comparing `ziya-0.1.8/LICENSE` & `ziya-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ziya-0.1.8/README.md` & `ziya-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ziya-0.1.8/app/agents/agent.py` & `ziya-0.1.9/app/agents/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
-import botocore
-
-from typing import Generator, List, Tuple, Set, Union
+from typing import List, Tuple, Set, Union
 
+import botocore
 import tiktoken
 from langchain.agents import AgentExecutor
 from langchain.agents.format_scratchpad import format_xml
 from langchain_aws import ChatBedrock
 from langchain_community.document_loaders import TextLoader
 from langchain_core.messages import AIMessage, HumanMessage
 from langchain_core.pydantic_v1 import BaseModel, Field
 
 from app.agents.prompts import conversational_prompt, parse_output
-from app.utils.directory_util import get_ignored_patterns, get_complete_file_list
 from app.utils.logging_utils import logger
 from app.utils.print_tree_util import print_file_tree
 
 
 def _format_chat_history(chat_history: List[Tuple[str, str]]) -> List[Union[HumanMessage, AIMessage]]:
+    logger.info("Formatting chat history")
     buffer = []
     for human, ai in chat_history:
         buffer.append(HumanMessage(content=human))
         buffer.append(AIMessage(content=ai))
     return buffer
 
 aws_profile = os.environ.get("ZIYA_AWS_PROFILE")
@@ -42,72 +41,94 @@
     credentials_profile_name=aws_profile if aws_profile else None,
     config=botocore.config.Config(
         read_timeout=900
     )
 )
 
 
-def get_combined_document_contents() -> str:
-    user_codebase_dir: str = os.environ["ZIYA_USER_CODEBASE_DIR"]
-    print(f"Reading user's current codebase: {user_codebase_dir}")
-
+def get_combined_docs_from_files(files) -> str:
     combined_contents: str = ""
-    ignored_patterns: List[str] = get_ignored_patterns(user_codebase_dir)
-    included_relative_dirs = [pattern.strip() for pattern in os.environ.get("ZIYA_ADDITIONAL_INCLUDE_DIRS", "").split(',')]
-    all_files: List[str] = get_complete_file_list(user_codebase_dir, ignored_patterns, included_relative_dirs)
-
-    print_file_tree(all_files)
-
-    seen_dirs: Set[str] = set()
-    for file_path in all_files:
+    print_file_tree(files)
+    user_codebase_dir: str = os.environ["ZIYA_USER_CODEBASE_DIR"]
+    for file_path in files:
         try:
-            docs = TextLoader(file_path).load()
+            full_file_path = os.path.join(user_codebase_dir, file_path)
+            docs = TextLoader(full_file_path).load()
             for doc in docs:
                 combined_contents += f"File: {file_path}\n{doc.page_content}\n\n"
-            dir_path = os.path.dirname(file_path)
-            if dir_path not in seen_dirs:
-                seen_dirs.add(dir_path)
+
         except Exception as e:
-            print(f"Skipping file {file_path} due to error: {e}")
+            print(f"Skipping file {full_file_path} due to error: {e}")
 
-    print("--------------------------------------------------------")
-    print(f"Ignoring following paths based on gitIgnore and other defaults: {ignored_patterns}")
-    print("--------------------------------------------------------")
     print(f"Codebase word count: {len(combined_contents.split()):,}")
     token_count = len(tiktoken.get_encoding("cl100k_base").encode(combined_contents))
     print(f"Codebase token count: {token_count:,}")
     print(f"Max Claude Token limit: 200,000")
     print("--------------------------------------------------------")
     return combined_contents
 
-def get_child_paths(directory: str) -> Generator[str, None, None]:
-    for entry in os.listdir(directory):
-        child_path = os.path.join(directory, entry)
-        yield child_path
-
-
-prompt = conversational_prompt.partial(
-    codebase=get_combined_document_contents,
-)
+# def get_combined_document_contents_from_included_dirs(included_relative_dirs) -> str:
+#     user_codebase_dir: str = os.environ["ZIYA_USER_CODEBASE_DIR"]
+#     print(f"Reading user's current codebase: {user_codebase_dir}")
+#
+#     combined_contents: str = ""
+#     ignored_patterns: List[str] = get_ignored_patterns(user_codebase_dir)
+#     all_files: List[str] = get_complete_file_list(user_codebase_dir, ignored_patterns, included_relative_dirs)
+#     print("all_files")
+#     print(all_files)
+#
+#     print_file_tree(all_files)
+#
+#     seen_dirs: Set[str] = set()
+#     for file_path in all_files:
+#         try:
+#             docs = TextLoader(file_path).load()
+#             for doc in docs:
+#                 combined_contents += f"File: {file_path}\n{doc.page_content}\n\n"
+#             dir_path = os.path.dirname(file_path)
+#             if dir_path not in seen_dirs:
+#                 seen_dirs.add(dir_path)
+#         except Exception as e:
+#             print(f"Skipping file {file_path} due to error: {e}")
+#
+#     print("--------------------------------------------------------")
+#     print(f"Ignoring following paths based on gitIgnore and other defaults: {ignored_patterns}")
+#     print("--------------------------------------------------------")
+#     print(f"Codebase word count: {len(combined_contents.split()):,}")
+#     token_count = len(tiktoken.get_encoding("cl100k_base").encode(combined_contents))
+#     print(f"Codebase token count: {token_count:,}")
+#     print(f"Max Claude Token limit: 200,000")
+#     print("--------------------------------------------------------")
+#     return combined_contents
+
+# prompt = conversational_prompt.partial(
+#     # codebase=get_combined_document_contents()
+# )
 llm_with_stop = model.bind(stop=["</tool_input>"])
 
+def extract_codebase(x):
+    # return get_combined_docs_from_files(x["config"].get("include_dirs", ['./']))
+    return get_combined_docs_from_files(x["config"].get("files", []))
+
 agent = (
         {
+            "codebase": lambda x: extract_codebase(x),
             "question": lambda x: x["question"],
             "agent_scratchpad": lambda x: format_xml(x["intermediate_steps"]),
             "chat_history": lambda x: _format_chat_history(x["chat_history"]),
         }
-        | prompt
+        | conversational_prompt
         | llm_with_stop
         | parse_output
 )
 
 
 class AgentInput(BaseModel):
     question: str
+    config: dict = Field({})
     chat_history: List[Tuple[str, str]] = Field(..., extra={"widget": {"type": "chat"}})
 
 
 agent_executor = AgentExecutor(
     agent=agent, tools=[], verbose=True, handle_parsing_errors=True
 ).with_types(input_type=AgentInput)
```

### Comparing `ziya-0.1.8/app/agents/prompts.py` & `ziya-0.1.9/app/agents/prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from langchain_core.agents import AgentFinish
 from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
 # import pydevd_pycharm
 
-template = """You are an excellent coder. Help the user with their coding tasks. You are given the entire codebase
+template = """
+You are an excellent coder. Help the user with their coding tasks. You are given the entire codebase
  of the user in your context. It is in the format like below where first line has the File path and then the content follows. 
 
 File: <filepath>
 <Content of the file>. 
 
 Now below is the current codebase of the user: 
  
 {codebase}
 """
 
 conversational_prompt = ChatPromptTemplate.from_messages(
     [
         ("system", template),
+        # ("system", "You are a helpful AI bot. Your name is {name}."),
         MessagesPlaceholder(variable_name="chat_history"),
         ("user", "{question}"),
         ("ai", "{agent_scratchpad}"),
     ]
 )
```

### Comparing `ziya-0.1.8/app/main.py` & `ziya-0.1.9/app/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 from app.utils.version_util import get_current_version, get_latest_version
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description="Run with custom options")
     parser.add_argument("--exclude", default=[], type=lambda x: x.split(','),
                         help="List of files or directories to exclude (e.g., --exclude 'tst,build,*.py')")
-    parser.add_argument("--include", default=[], type=lambda x: x.split(','),
-                        help="List of directories to include (e.g., --include 'src,static'). Only directories for now")
     parser.add_argument("--profile", type=str, default=None,
                         help="AWS profile to use (e.g., --profile ziya)")
     parser.add_argument("--model", type=str, choices=["sonnet", "haiku", "opus"], default="sonnet",
                         help="AWS Bedrock Model to use (e.g., --model sonnet)")
     parser.add_argument("--port", type=int, default=6969,
                         help="Port number to run Ziya frontend on (e.g., --port 8080)")
     parser.add_argument("--version", action="store_true",
@@ -30,17 +28,14 @@
 
 def setup_environment(args):
     os.environ["ZIYA_USER_CODEBASE_DIR"] = os.getcwd()
 
     additional_excluded_dirs = ','.join(args.exclude)
     os.environ["ZIYA_ADDITIONAL_EXCLUDE_DIRS"] = additional_excluded_dirs
 
-    additional_included_dirs = ','.join(args.include)
-    os.environ["ZIYA_ADDITIONAL_INCLUDE_DIRS"] = additional_included_dirs
-
     if args.profile:
         os.environ["ZIYA_AWS_PROFILE"] = args.profile
     if args.model:
         os.environ["ZIYA_AWS_MODEL"] = args.model
 
 
 def check_version_and_upgrade():
```

### Comparing `ziya-0.1.8/app/utils/directory_util.py` & `ziya-0.1.9/app/utils/directory_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import glob
 import os
-from typing import List, Set, Tuple
+from typing import List, Set, Tuple, Dict
 
 from app.utils.gitignore_parser import parse_gitignore_patterns
 
 
 def get_ignored_patterns(directory: str) -> List[Tuple[str, str]]:
     ignored_patterns: List[Tuple[str, str]] = [
         ("poetry.lock", os.environ["ZIYA_USER_CODEBASE_DIR"]),
@@ -37,25 +37,30 @@
 
         return patterns
 
     ignored_patterns.extend(get_patterns_recursive(directory))
     return ignored_patterns
 
 
-def get_complete_file_list(user_codebase_dir: str, ignored_patterns: List[str], included_relative_dirs: List[str]) -> List[str]:
-    should_ignore = parse_gitignore_patterns(ignored_patterns, base_dir=user_codebase_dir)
-    file_set: Set[str] = set()
+def get_complete_file_list(user_codebase_dir: str, ignored_patterns: List[str], included_relative_dirs: List[str]) -> Dict[str, Dict]:
+    should_ignore_fn = parse_gitignore_patterns(ignored_patterns)
+    file_dict: Dict[str, Dict] = {}
     for pattern in included_relative_dirs:
         for root, dirs, files in os.walk(os.path.normpath(os.path.join(user_codebase_dir, pattern))):
-            # Filter out ignored directories
-            dirs[:] = [d for d in dirs if not should_ignore(os.path.join(root, d))]
+            # Filter out ignored directories and hidden directories
+            dirs[:] = [d for d in dirs if not should_ignore_fn(os.path.join(root, d)) and not d.startswith('.')]
 
             for file in files:
                 file_path = os.path.join(root, file)
-                if not should_ignore(file_path) and not is_image_file(file_path):
-                    file_set.add(file_path)
+                if not should_ignore_fn(file_path) and not is_image_file(file_path) and not file.startswith('.'):
+                    file_dict[file_path] = {}
 
-    return list(file_set)
+            for dir in dirs:
+                dir_path = os.path.join(root, dir)
+                if not should_ignore_fn(dir_path):
+                    file_dict[dir_path] = {}
+
+    return file_dict
 
 def is_image_file(file_path: str) -> bool:
     image_extensions = ['.jpg', '.jpeg', '.png', '.gif', '.bmp', '.svg', '.ico']
     return any(file_path.lower().endswith(ext) for ext in image_extensions)
```

### Comparing `ziya-0.1.8/app/utils/gitignore_parser.py` & `ziya-0.1.9/app/utils/gitignore_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 def handle_negation(file_path, rules: Reversible["IgnoreRule"]):
     for rule in reversed(rules):
         if rule.match(file_path):
             return not rule.negation
     return False
 
 
-def parse_gitignore_patterns(patterns: List[Tuple[str, str]], base_dir=None):
-    if base_dir is None:
-        base_dir = os.getcwd()
+def parse_gitignore_patterns(patterns: List[Tuple[str, str]]):
     rules = []
     for counter, (pattern, directory) in enumerate(patterns, start=1):
         rule = rule_from_pattern(pattern, base_path=_normalize_path(directory),
                                  source=('in-memory', counter))
         if rule:
             rules.append(rule)
     if not any(r.negation for r in rules):
```

### Comparing `ziya-0.1.8/app/utils/langchain_validation_util.py` & `ziya-0.1.9/app/utils/langchain_validation_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.8/app/utils/print_tree_util.py` & `ziya-0.1.9/app/utils/print_tree_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.8/app/utils/version_util.py` & `ziya-0.1.9/app/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `ziya-0.1.8/pyproject.toml` & `ziya-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "ziya"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Vishnu Krishnaprasad <vishnukool@gmail.com>"]
 readme = "README.md"
-include = ["static/**/*", "templates/**/*", "pyproject.toml"]
+include = ["templates/**/*", "pyproject.toml" ,"scripts.py"]
 packages = [
     { include = "app" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 uvicorn = "^0.23.2"
@@ -17,17 +17,19 @@
 tiktoken = "^0.6.0"
 boto3 = "^1.34.88"
 langchain-aws = "^0.1.0"
 langchain = "^0.1"
 langchainhub = ">=0.1.15"
 langchain-anthropic = "^0.1.4"
 langchain-cli = ">=0.0.15"
-
-[tool.poetry.group.dev.dependencies]
 pydevd-pycharm = "^241.15989.57"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-ziya = 'app.main:main'
+ziya = 'scripts:ziya'
+dev = 'scripts:dev'
+finstall = "scripts:frontend_install"
+fstart = "scripts:frontend_start"
+fbuild = "scripts:frontend_build"
```

### Comparing `ziya-0.1.8/static/favicon.ico` & `ziya-0.1.9/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `ziya-0.1.8/PKG-INFO` & `ziya-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ziya
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Vishnu Krishnaprasad
 Author-email: vishnukool@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,15 @@
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: langchain (>=0.1,<0.2)
 Requires-Dist: langchain-anthropic (>=0.1.4,<0.2.0)
 Requires-Dist: langchain-aws (>=0.1.0,<0.2.0)
 Requires-Dist: langchain-cli (>=0.0.15)
 Requires-Dist: langchainhub (>=0.1.15)
 Requires-Dist: pydantic (<2)
+Requires-Dist: pydevd-pycharm (>=241.15989.57,<242.0.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: uvicorn (>=0.23.2,<0.24.0)
 Description-Content-Type: text/markdown
 
 # Ziya
 
 ## Documentation
```

