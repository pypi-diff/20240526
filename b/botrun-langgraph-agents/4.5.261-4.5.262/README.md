# Comparing `tmp/botrun_langgraph_agents-4.5.261.tar.gz` & `tmp/botrun_langgraph_agents-4.5.262.tar.gz`

## Comparing `botrun_langgraph_agents-4.5.261.tar` & `botrun_langgraph_agents-4.5.262.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/agents_config.json
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/botrun_langgraph_agents.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/requirements.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/docker_python.sh
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/go.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/install.sh
--rwxr-xr-x   0        0        0      165 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/install.sh~
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/pull.sh
--rwxr-xr-x   0        0        0       47 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/push.sh
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/sh/pypi.sh
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/.gitignore
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/README.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/pyproject.toml
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.261/PKG-INFO
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/agents_config.json
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/botrun_langgraph_agents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/requirements.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/docker_python.sh
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/go.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/install.sh
+-rwxr-xr-x   0        0        0      165 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/install.sh~
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/pull.sh
+-rwxr-xr-x   0        0        0       47 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/push.sh
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/sh/pypi.sh
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/.gitignore
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/README.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 botrun_langgraph_agents-4.5.262/PKG-INFO
```

### Comparing `botrun_langgraph_agents-4.5.261/agents_config.json` & `botrun_langgraph_agents-4.5.262/agents_config.json`

 * *Files identical despite different names*

### Comparing `botrun_langgraph_agents-4.5.261/botrun_langgraph_agents.py` & `botrun_langgraph_agents-4.5.262/botrun_langgraph_agents.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 import asyncio
 import functools
+import json
 import operator
 import sys
-import json
-from typing import Annotated, Sequence, TypedDict
+from typing import Annotated, Sequence, TypedDict, Any, Dict, List
 
+from botrun_google_docs_reader import botrun_google_docs_reader
 from dotenv import load_dotenv
 from langchain.agents import AgentExecutor, create_openai_tools_agent
 from langchain_community.tools.tavily_search import TavilySearchResults
 from langchain_core.messages import BaseMessage, HumanMessage
 from langchain_core.output_parsers.openai_functions import JsonOutputFunctionsParser
 from langchain_core.prompts import ChatPromptTemplate, MessagesPlaceholder
 from langchain_openai import ChatOpenAI
@@ -22,45 +23,43 @@
 # 定義代理人的狀態類別
 class AgentState(TypedDict):
     messages: Annotated[Sequence[BaseMessage], operator.add]
     next: str
 
 
 # 創建代理人的函數
-def create_agent(llm: ChatOpenAI, tools: list, system_prompt: str):
+def create_agent(llm: ChatOpenAI, tools: List[Any], system_prompt: str) -> AgentExecutor:
     prompt = ChatPromptTemplate.from_messages(
         [
             ("system", system_prompt),
             MessagesPlaceholder(variable_name="messages"),
             MessagesPlaceholder(variable_name="agent_scratchpad"),
         ]
     )
     agent = create_openai_tools_agent(llm, tools, prompt)
     executor = AgentExecutor(agent=agent, tools=tools)
     return executor
 
 
 # 代理人節點執行函數
-def agent_node(state, agent, name):
+def agent_node(state: AgentState, agent: AgentExecutor, name: str) -> Dict[str, List[HumanMessage]]:
     print(f"\n\n😊Starting node: {name}")
     result = agent.invoke(state)
     return {"messages": [HumanMessage(content=result["output"], name=name)]}
 
 
 # 主函數
-def main(user_input_prompt: str, agent_config_path: str):
+def botrun_langgraph_agents(user_input_prompt: str, agent_config_path: str) -> None:
     # 初始化 OpenAI 模型
     llm = ChatOpenAI(model="gpt-4o")
 
     # 初始化工具
     tavily_tool = TavilySearchResults(max_results=3)
 
-    # 讀取代理人配置
-    with open(agent_config_path, 'r', encoding='utf-8') as f:
-        agents_config = json.load(f)
+    agents_config = read_agents_config(agent_config_path)
 
     agents = {}
     for agent_info in agents_config:
         agent_name = agent_info["name"]
         agent_prompt = agent_info["prompt"]
         agents[agent_name] = create_agent(llm, [tavily_tool], agent_prompt)
 
@@ -122,15 +121,15 @@
     conditional_map["FINISH"] = END
     workflow.add_conditional_edges(AGENT_SUPERVISOR, lambda x: x["next"], conditional_map)
     workflow.set_entry_point(AGENT_SUPERVISOR)
 
     graph = workflow.compile()
 
     # 執行工作流並串流輸出
-    async def run_graph_with_stream():
+    async def run_graph_with_stream() -> None:
         async for event in graph.astream_events({"messages": [HumanMessage(content=user_input_prompt)]}, version="v2"):
             kind = event["event"]
             if kind == "on_chain_start":
                 if event["name"] == "Agent":
                     print(f"Starting agent: {event['name']} with input: {event['data'].get('input')}")
             elif kind == "on_chain_end":
                 if event["name"] == "Agent":
@@ -149,14 +148,26 @@
                 print(f"Tool output was: {event['data'].get('output')}")
                 print("--")
             sys.stdout.flush()
 
     asyncio.run(run_graph_with_stream())
 
 
+def read_agents_config(agent_config_path: str) -> List[Dict[str, Any]]:
+    if agent_config_path.startswith("https://docs.google.com/document/d/"):
+        doc_id = agent_config_path.split('/')[5]
+        content = botrun_google_docs_reader(doc_id)
+        agents_config = json.loads(content)
+    else:
+        # 讀取本地文件內容
+        with open(agent_config_path, 'r', encoding='utf-8') as f:
+            agents_config = json.load(f)
+    return agents_config
+
+
 # 解析命令行參數並執行主函數
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="LangGraph Multi-Agent CLI")
     parser.add_argument(
         "--user_input_prompt",
         type=str,
         default="請幫我寫一篇一百字的 RAG for AI LLM介紹，極短的，不要太長。",
@@ -165,8 +176,8 @@
     parser.add_argument(
         "--agent_config_path",
         type=str,
         default="agents_config.json",
         help="代理人配置文件的路徑"
     )
     args = parser.parse_args()
-    main(args.user_input_prompt, args.agent_config_path)
+    botrun_langgraph_agents(args.user_input_prompt, args.agent_config_path)
```

### Comparing `botrun_langgraph_agents-4.5.261/README.md` & `botrun_langgraph_agents-4.5.262/README.md`

 * *Files identical despite different names*

### Comparing `botrun_langgraph_agents-4.5.261/PKG-INFO` & `botrun_langgraph_agents-4.5.262/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.3
 Name: botrun_langgraph_agents
-Version: 4.5.261
+Version: 4.5.262
 Requires-Dist: argparse
+Requires-Dist: botrun-google-docs-reader
 Requires-Dist: langchain
 Requires-Dist: langchain-community
 Requires-Dist: langchain-openai
 Requires-Dist: langgraph
 Requires-Dist: litellm
 Requires-Dist: python-dotenv
 Requires-Dist: tavily-python
```

