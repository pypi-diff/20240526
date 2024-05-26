# Comparing `tmp/surfkit-0.1.98.tar.gz` & `tmp/surfkit-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.98.tar", max compression
+gzip compressed data, was "surfkit-0.1.99.tar", max compression
```

## Comparing `surfkit-0.1.98.tar` & `surfkit-0.1.99.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.98/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.98/README.md
--rw-r--r--   0        0        0      756 2024-05-01 17:41:28.640573 surfkit-0.1.98/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 21:28:15.523878 surfkit-0.1.98/surfkit/__init__.py
--rw-r--r--   0        0        0     1921 2024-05-01 02:53:14.821990 surfkit-0.1.98/surfkit/agent.py
--rw-r--r--   0        0        0    16409 2024-05-01 14:51:16.439451 surfkit-0.1.98/surfkit/cli/main.py
--rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.98/surfkit/cli/new.py
--rw-r--r--   0        0        0    17058 2024-04-30 03:19:26.328281 surfkit-0.1.98/surfkit/cli/templates/agent.py
--rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.98/surfkit/cli/templates/device.py
--rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.98/surfkit/cli/util.py
--rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.98/surfkit/config.py
--rw-r--r--   0        0        0     2263 2024-04-30 02:59:37.720164 surfkit-0.1.98/surfkit/db/conn.py
--rw-r--r--   0        0        0     1216 2024-05-01 14:46:55.707656 surfkit-0.1.98/surfkit/db/models.py
--rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.98/surfkit/env.py
--rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.98/surfkit/hub.py
--rw-r--r--   0        0        0     2687 2024-05-01 17:42:12.432805 surfkit-0.1.98/surfkit/models.py
--rw-r--r--   0        0        0     3543 2024-05-01 02:03:25.109376 surfkit-0.1.98/surfkit/runtime/agent/base.py
--rw-r--r--   0        0        0     9356 2024-05-01 02:03:41.708645 surfkit-0.1.98/surfkit/runtime/agent/docker.py
--rw-r--r--   0        0        0    28578 2024-05-01 02:04:01.750740 surfkit-0.1.98/surfkit/runtime/agent/kube.py
--rw-r--r--   0        0        0     1187 2024-04-30 16:00:13.133177 surfkit-0.1.98/surfkit/runtime/agent/load.py
--rw-r--r--   0        0        0    11187 2024-05-01 02:04:40.092850 surfkit-0.1.98/surfkit/runtime/agent/process.py
--rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.98/surfkit/runtime/container/base.py
--rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.98/surfkit/runtime/container/docker.py
--rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.98/surfkit/runtime/container/kube.py
--rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.98/surfkit/runtime/container/load.py
--rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.98/surfkit/runtime/vm/base.py
--rw-r--r--   0        0        0     7230 2024-05-01 17:41:48.899239 surfkit-0.1.98/surfkit/server/routes.py
--rw-r--r--   0        0        0    14338 2024-04-30 17:45:57.825243 surfkit-0.1.98/surfkit/types.py
--rw-r--r--   0        0        0     1516 2024-04-30 17:09:57.207060 surfkit-0.1.98/surfkit/util.py
--rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 surfkit-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-09 16:39:37.152115 surfkit-0.1.99/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.99/README.md
+-rw-r--r--   0        0        0      756 2024-05-01 19:17:39.346022 surfkit-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 21:28:15.523878 surfkit-0.1.99/surfkit/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-01 02:53:14.821990 surfkit-0.1.99/surfkit/agent.py
+-rw-r--r--   0        0        0    19649 2024-05-01 18:42:32.989351 surfkit-0.1.99/surfkit/cli/main.py
+-rw-r--r--   0        0        0      926 2024-04-29 19:57:18.519637 surfkit-0.1.99/surfkit/cli/new.py
+-rw-r--r--   0        0        0    17058 2024-04-30 03:19:26.328281 surfkit-0.1.99/surfkit/cli/templates/agent.py
+-rw-r--r--   0        0        0        0 2024-04-09 16:39:37.166494 surfkit-0.1.99/surfkit/cli/templates/device.py
+-rw-r--r--   0        0        0      866 2024-04-29 19:58:42.750756 surfkit-0.1.99/surfkit/cli/util.py
+-rw-r--r--   0        0        0     2053 2024-04-17 19:36:14.985684 surfkit-0.1.99/surfkit/config.py
+-rw-r--r--   0        0        0     2263 2024-04-30 02:59:37.720164 surfkit-0.1.99/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1216 2024-05-01 14:46:55.707656 surfkit-0.1.99/surfkit/db/models.py
+-rw-r--r--   0        0        0      238 2024-04-17 19:35:04.174976 surfkit-0.1.99/surfkit/env.py
+-rw-r--r--   0        0        0      993 2024-04-03 16:40:15.124046 surfkit-0.1.99/surfkit/hub.py
+-rw-r--r--   0        0        0     2687 2024-05-01 17:42:12.432805 surfkit-0.1.99/surfkit/models.py
+-rw-r--r--   0        0        0     3514 2024-05-01 17:50:28.486968 surfkit-0.1.99/surfkit/runtime/agent/base.py
+-rw-r--r--   0        0        0     9332 2024-05-01 17:50:50.667830 surfkit-0.1.99/surfkit/runtime/agent/docker.py
+-rw-r--r--   0        0        0    28568 2024-05-01 17:51:17.788790 surfkit-0.1.99/surfkit/runtime/agent/kube.py
+-rw-r--r--   0        0        0     1187 2024-04-30 16:00:13.133177 surfkit-0.1.99/surfkit/runtime/agent/load.py
+-rw-r--r--   0        0        0    11177 2024-05-01 17:51:31.922375 surfkit-0.1.99/surfkit/runtime/agent/process.py
+-rw-r--r--   0        0        0     1425 2024-04-11 22:52:18.482166 surfkit-0.1.99/surfkit/runtime/container/base.py
+-rw-r--r--   0        0        0     5983 2024-04-16 16:34:59.842004 surfkit-0.1.99/surfkit/runtime/container/docker.py
+-rw-r--r--   0        0        0    16077 2024-04-11 22:50:31.352813 surfkit-0.1.99/surfkit/runtime/container/kube.py
+-rw-r--r--   0        0        0     1028 2024-04-11 16:49:49.850218 surfkit-0.1.99/surfkit/runtime/container/load.py
+-rw-r--r--   0        0        0      402 2024-04-11 18:32:09.170609 surfkit-0.1.99/surfkit/runtime/vm/base.py
+-rw-r--r--   0        0        0     7197 2024-05-01 18:54:50.300147 surfkit-0.1.99/surfkit/server/routes.py
+-rw-r--r--   0        0        0    14538 2024-05-01 18:35:19.133937 surfkit-0.1.99/surfkit/types.py
+-rw-r--r--   0        0        0     1516 2024-04-30 17:09:57.207060 surfkit-0.1.99/surfkit/util.py
+-rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 surfkit-0.1.99/PKG-INFO
```

### Comparing `surfkit-0.1.98/LICENSE` & `surfkit-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/pyproject.toml` & `surfkit-0.1.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surfkit"
-version = "0.1.98"
+version = "0.1.99"
 description = "A toolkit to build GUI surfing AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `surfkit-0.1.98/surfkit/agent.py` & `surfkit-0.1.99/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/cli/main.py` & `surfkit-0.1.99/surfkit/cli/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 import typer
 import webbrowser
 from namesgenerator import get_random_name
 import requests
 from tabulate import tabulate
 
+from surfkit import agent
+from surfkit.types import AgentType
+
 art = """
  _______                ___  __  __  __  __   
 |     __|.--.--..----..'  _||  |/  ||__||  |_ 
 |__     ||  |  ||   _||   _||     < |  ||   _|
 |_______||_____||__|  |__|  |__|\__||__||____|
 """
 
@@ -517,24 +520,36 @@
 
 
 @app.command(help="Use an agent to solve a task")
 def solve(
     description: str = typer.Option(..., help="Description of the task."),
     agent_name: Optional[str] = typer.Option(None, help="Name of the agent to use."),
     agent_type: Optional[str] = typer.Option(None, help="Type of agent to use."),
+    agent_file: Optional[str] = typer.Option(None, help="Path to agent config file."),
+    agent_version: Optional[str] = typer.Option(None, help="Version of agent to use."),
+    device: Optional[str] = typer.Option(
+        None, help="Name of device to use if applicable."
+    ),
+    device_type: Optional[str] = typer.Option(
+        None, help="Name of the type of device if using one."
+    ),
+    device_provider: Optional[str] = typer.Option(
+        None, help="The provider type for the device."
+    ),
     max_steps: int = typer.Option(20, help="Maximum steps for the task."),
     starting_url: Optional[str] = typer.Option(
         None, help="Starting URL if applicable."
     ),
     runtime: str = typer.Option("docker", help="Runtime environment for the agent."),
     kill: bool = typer.Option(False, help="Whether to kill the agent when done"),
+    view: bool = typer.Option(True, help="Whether to view the device"),
+    follow: bool = typer.Option(True, help="Whether to follow the agent logs"),
 ):
-    typer.echo(f"Solving task {description}...")
-    from taskara.server.models import V1SolveTask
     from taskara import Task
+    from agentdesk import Desktop
 
     if runtime == "docker":
         from surfkit.runtime.agent.docker import (
             DockerAgentRuntime,
             ConnectConfig as DockerConnectConfig,
         )
 
@@ -558,17 +573,91 @@
 
         pconf = ProcessConnectConfig()
         runt = ProcessAgentRuntime.connect(cfg=pconf)
 
     else:
         raise ValueError(f"Unknown runtime '{runtime}'")
 
-    task = Task(description=description, parameters={"site": starting_url})
-    mdl = V1SolveTask(
-        task=task.to_v1(),
+    v1device = None
+    _device = None
+    if device_type:
+        if device_type == "desktop":
+            from agentdesk.server.models import V1ProviderData
+            from agentdesk.vm.load import load_provider
+
+            data = V1ProviderData(type=device_provider)
+            _provider = load_provider(data)
+
+            typer.echo(
+                f"Creating desktop '{agent_name}' using '{device_provider}' provider"
+            )
+            try:
+                vm = _provider.create(
+                    name=agent_name,
+                )
+                _device = Desktop.from_vm(vm)
+                v1device = _device.to_v1()
+            except KeyboardInterrupt:
+                print("Keyboard interrupt received, exiting...")
+                return
+        else:
+            raise ValueError(f"unknown device type {device_type}")
+
+    if device:
+        typer.echo(f"finding device '{device}'...")
+        vms = Desktop.find(name=device)
+        if not vms:
+            raise ValueError(f"Device '{device}' not found")
+        vm = vms[0]
+        _device = Desktop.from_vm(vm)
+        v1device = _device.to_v1()
+        typer.echo(f"found device '{device}'...")
+
+    if _device and view:
+        typer.echo("viewing device...")
+        _device.view(True)
+
+    if agent_type:
+        from surfkit.config import HUB_API_URL
+
+        types = AgentType.find(remote=HUB_API_URL, name=agent_type)
+        if not types:
+            raise ValueError(f"Agent type '{agent_type}' not found")
+        typ = types[0]
+        if not agent_name:
+            agent_name = get_random_name("-")
+            if not agent_name:
+                raise ValueError("could not generate agent name")
+        typer.echo(f"creating agent {agent_name}...")
+        runt.run(agent_type=typ, name=agent_name, version=agent_version)
+
+    if agent_file:
+        typ = AgentType.from_file(agent_file)
+        if not agent_name:
+            agent_name = get_random_name("-")
+            if not agent_name:
+                raise ValueError("could not generate agent name")
+        typer.echo(f"creating agent {agent_name} from file {agent_file}...")
+        runt.run(agent_type=typ, name=agent_name, version=agent_version)
+
+    if not agent_name:
+        raise ValueError("Either agent_name or agent_type needs to be provided")
+
+    task = Task(
+        description=description,
+        parameters={"site": starting_url},
         max_steps=max_steps,
+        device=v1device,
+        assigned_to=agent_name,
+        assigned_type=agent_type,
     )
-    runt.solve_task(agent_name, mdl)
+
+    typer.echo(f"Solving task '{task.description}' with agent {agent_name}...")
+    runt.solve_task(agent_name, task.to_v1(), follow_logs=follow)
+
+    if kill:
+        typer.echo(f"Killing agent {agent_name}...")
+        runt.delete(agent_name)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `surfkit-0.1.98/surfkit/cli/new.py` & `surfkit-0.1.99/surfkit/cli/new.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/cli/templates/agent.py` & `surfkit-0.1.99/surfkit/cli/templates/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/cli/util.py` & `surfkit-0.1.99/surfkit/cli/util.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/config.py` & `surfkit-0.1.99/surfkit/config.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/db/conn.py` & `surfkit-0.1.99/surfkit/db/conn.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/db/models.py` & `surfkit-0.1.99/surfkit/db/models.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/hub.py` & `surfkit-0.1.99/surfkit/hub.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/models.py` & `surfkit-0.1.99/surfkit/models.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/runtime/agent/base.py` & `surfkit-0.1.99/surfkit/runtime/agent/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, TypeVar, Type, Generic, Union, Iterator, Optional
 from abc import ABC, abstractmethod
 
 from pydantic import BaseModel
-from taskara.server.models import V1SolveTask
+from taskara import V1Task
 
 from surfkit.types import AgentType
 from surfkit.models import V1AgentInstance
 
 R = TypeVar("R", bound="AgentRuntime")
 C = TypeVar("C", bound="BaseModel")
 
@@ -42,15 +42,15 @@
         self,
         local_port: Optional[int] = None,
         pod_port: int = 9090,
         background: bool = True,
     ) -> None:
         return self._runtime.proxy(self._name, local_port, pod_port, background)
 
-    def solve_task(self, task: V1SolveTask, follow_logs: bool = False) -> None:
+    def solve_task(self, task: V1Task, follow_logs: bool = False) -> None:
         return self._runtime.solve_task(self._name, task, follow_logs)
 
     def delete(self) -> None:
         return self._runtime.delete(self._name)
 
     def logs(self, follow: bool = False) -> Union[str, Iterator[str]]:
         """
@@ -100,15 +100,15 @@
         llm_providers_local: bool = False,
         owner_id: Optional[str] = None,
     ) -> AgentInstance:
         pass
 
     @abstractmethod
     def solve_task(
-        self, agent_name: str, task: V1SolveTask, follow_logs: bool = False
+        self, agent_name: str, task: V1Task, follow_logs: bool = False
     ) -> None:
         pass
 
     @abstractmethod
     def list(self) -> List[AgentInstance]:
         pass
```

### Comparing `surfkit-0.1.98/surfkit/runtime/agent/docker.py` & `surfkit-0.1.99/surfkit/runtime/agent/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Type, Union, Iterator
 import os
 
 import docker
 from docker.errors import NotFound
-from taskara.server.models import V1SolveTask
+from taskara import V1Task
 from agentdesk.util import find_open_port
 import requests
 from pydantic import BaseModel
 from mllm import Router
 
 from surfkit.models import V1AgentType
 
@@ -101,15 +101,15 @@
         )
         if container and type(container) != bytes:
             print(f"ran container '{container.id}'")  # type: ignore
 
         return AgentInstance(name, agent_type, self)
 
     def solve_task(
-        self, agent_name: str, task: V1SolveTask, follow_logs: bool = False
+        self, agent_name: str, task: V1Task, follow_logs: bool = False
     ) -> None:
         try:
             container = self.client.containers.get(agent_name)
             print(f"Container '{agent_name}' found.")
             response = requests.post(
                 f"http://localhost:{container.attrs['NetworkSettings']['Ports']['9090/tcp'][0]['HostPort']}/v1/tasks",  # type: ignore
                 json=task.model_dump(),
```

### Comparing `surfkit-0.1.98/surfkit/runtime/agent/kube.py` & `surfkit-0.1.99/surfkit/runtime/agent/kube.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from kubernetes.client.rest import ApiException
 from kubernetes.stream import portforward
 from kubernetes.client import Configuration
 from kubernetes.client.api import core_v1_api
 from namesgenerator import get_random_name
 from tenacity import retry
 from pydantic import BaseModel
-from taskara.server.models import V1SolveTask
+from taskara.server.models import V1Task
 from agentdesk.util import find_open_port
 from mllm import Router
 
 from .base import AgentRuntime, AgentInstance
 from surfkit.types import AgentType
 from surfkit.models import V1ResourceLimits, V1ResourceRequests, V1AgentType
 
@@ -703,15 +703,15 @@
             env_vars=env_vars,
             owner_id=owner_id,
         )
 
         return AgentInstance(name, agent_type, self)
 
     def solve_task(
-        self, agent_name: str, task: V1SolveTask, follow_logs: bool = False
+        self, agent_name: str, task: V1Task, follow_logs: bool = False
     ) -> None:
         try:
             # Making the call to the specified path to initiate the task
             status_code, response_text = self.call(
                 name=agent_name,
                 path="/v1/tasks",
                 method="POST",
```

### Comparing `surfkit-0.1.98/surfkit/runtime/agent/load.py` & `surfkit-0.1.99/surfkit/runtime/agent/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/runtime/agent/process.py` & `surfkit-0.1.99/surfkit/runtime/agent/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional, Type, Union, Iterator
 import os
 import subprocess
 import time
 import signal
 import json
 
-from taskara.server.models import V1SolveTask
+from taskara.server.models import V1Task
 from agentdesk.util import find_open_port
 import requests
 from pydantic import BaseModel
 from mllm import Router
 
 from .base import AgentRuntime, AgentInstance
 from surfkit.models import V1AgentType
@@ -112,15 +112,15 @@
             # Print the output from stdout
             print("Command output:")
             print(stdout)
 
         return AgentInstance(name, agent_type, self, port)
 
     def solve_task(
-        self, agent_name: str, task: V1SolveTask, follow_logs: bool = False
+        self, agent_name: str, task: V1Task, follow_logs: bool = False
     ) -> None:
         try:
             # Fetch the list of all processes to find the required agent
             process_list = subprocess.check_output(
                 f"ps ax -o pid,command | grep -v grep | grep SURFER={agent_name}",
                 shell=True,
                 text=True,
```

### Comparing `surfkit-0.1.98/surfkit/runtime/container/base.py` & `surfkit-0.1.99/surfkit/runtime/container/base.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/runtime/container/docker.py` & `surfkit-0.1.99/surfkit/runtime/container/docker.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/runtime/container/kube.py` & `surfkit-0.1.99/surfkit/runtime/container/kube.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/runtime/container/load.py` & `surfkit-0.1.99/surfkit/runtime/container/load.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/surfkit/server/routes.py` & `surfkit-0.1.99/surfkit/server/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # type: ignore
 import os
 from typing import List, Final
 import logging
 
-from taskara.server.models import V1SolveTask, V1Task, V1Tasks
+from taskara.server.models import V1Task, V1Tasks
 from taskara.task import Task
 from surfkit.hub import Hub
 from fastapi import FastAPI, BackgroundTasks
 from fastapi.middleware.cors import CORSMiddleware
 from contextlib import asynccontextmanager
 from tenacity import retry, stop_after_attempt, wait_fixed
 import uvicorn
@@ -41,15 +41,15 @@
 
 @app.get("/health")
 async def health():
     return {"status": "ok"}
 
 
 @app.post("/v1/tasks")
-async def solve_task(background_tasks: BackgroundTasks, task_model: V1SolveTask):
+async def solve_task(background_tasks: BackgroundTasks, task_model: V1Task):
     print(f"solving task: 
 {task_model.model_dump()}")
     try:
         # TODO: we need to find a way to do this earlier but get status back
         router.check_model()
     except Exception as e:
         print(f"Cannot connect to LLM providers: {e} -- did you provide a valid key?")
@@ -57,15 +57,15 @@
             "status": "failed",
             "message": f"failed to conect to LLM providers: {e} -- did you provide a valid key?",
         }
 
     background_tasks.add_task(_solve_task, task_model)
     print("created background task...")
 
-def _solve_task(task_model: V1SolveTask):
+def _solve_task(task_model: V1Task):
     task = Task.from_v1(task_model.task, owner_id="local")
     if task.remote:
         print("connecting to remote task...")
         HUB_SERVER = os.environ.get("SURF_HUB_SERVER", "https://surf.agentlabs.xyz")
         HUB_API_KEY = os.environ.get("HUB_API_KEY")
         if not HUB_API_KEY:
             raise Exception("$HUB_API_KEY not set")
@@ -135,15 +135,15 @@
     tasks = Task.find(id=id)
     if not tasks:
         raise Exception(f"Task {id} not found")
     return tasks[0].to_v1()
 
 
 @app.post("/v1/work")
-async def work(background_tasks: BackgroundTasks, work_model: V1SolveTask):
+async def work(background_tasks: BackgroundTasks, work_model: V1Task):
     print(f"solving task: {work_model.model_dump()}")
     try:
         # TODO: we need to find a way to do this earlier but get status back
         router.check_model()
     except Exception as e:
         print(f"Cannot connect to LLM providers: {e} -- did you provide a valid key?")
         return {
@@ -151,15 +151,15 @@
             "message": f"failed to conect to LLM providers: {e} -- did you provide a valid key?",
         }
 
     background_tasks.add_task(_work, work_model)
     print("created background task...")
 
 
-def _work(work_model: V1SolveTask):
+def _work(work_model: V1Task):
     while True:
         print("connecting to remote task...")
         HUB_SERVER = os.environ.get("SURF_HUB_SERVER", "https://surf.agentlabs.xyz")
         HUB_API_KEY = os.environ.get("HUB_API_KEY")
         if not HUB_API_KEY:
             raise Exception("$HUB_API_KEY not set")
```

### Comparing `surfkit-0.1.98/surfkit/types.py` & `surfkit-0.1.99/surfkit/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List, Optional, Dict, Any
 import uuid
 import time
 import json
 import os
 import logging
+import yaml
 
 from sqlalchemy import or_
 import requests
 
 from .db.models import AgentTypeRecord
 from .db.conn import WithDB
 from .models import (
@@ -71,14 +72,24 @@
         self.llm_providers: Optional[V1LLMProviders] = llm_providers
         self.devices = devices
         self.repo = repo
         self.meters = meters
         self.remote = remote
         self.save()
 
+    @classmethod
+    def from_file(
+        cls, path: str = "./agent.yaml", owner_id: Optional[str] = None
+    ) -> "AgentType":
+        with open(path) as f:
+            data = yaml.safe_load(f)
+
+        v1 = V1AgentType.model_validate(data)
+        return cls.from_v1(v1, owner_id)
+
     def to_v1(self) -> V1AgentType:
         return V1AgentType(
             id=self.id,
             name=self.name,
             description=self.description,
             kind=self.kind,
             cmd=self.cmd,
@@ -96,38 +107,36 @@
             devices=self.devices,
             owner_id=self.owner_id,
             repo=self.repo,
             meters=self.meters,
         )
 
     @classmethod
-    def from_v1(
-        cls, schema: V1AgentType, owner_id: Optional[str] = None
-    ) -> "AgentType":
+    def from_v1(cls, v1: V1AgentType, owner_id: Optional[str] = None) -> "AgentType":
         obj = cls.__new__(cls)
-        obj.id = schema.id
-        obj.name = schema.name
-        obj.kind = schema.kind
-        obj.owner_id = schema.owner_id
-        obj.description = schema.description
-        obj.cmd = schema.cmd
-        obj.image = schema.image
-        obj.env_opts = schema.env_opts
-        obj.runtimes = schema.runtimes
-        obj.created = schema.created
-        obj.updated = schema.updated
-        obj.public = schema.public
-        obj.icon = schema.icon
-        obj.resource_requests = schema.resource_requests
-        obj.resource_limits = schema.resource_limits
-        obj.versions = schema.versions
-        obj.llm_providers = schema.llm_providers
-        obj.devices = schema.devices
-        obj.repo = schema.repo
-        obj.meters = schema.meters
+        obj.id = v1.id
+        obj.name = v1.name
+        obj.kind = v1.kind
+        obj.owner_id = v1.owner_id
+        obj.description = v1.description
+        obj.cmd = v1.cmd
+        obj.image = v1.image
+        obj.env_opts = v1.env_opts
+        obj.runtimes = v1.runtimes
+        obj.created = v1.created
+        obj.updated = v1.updated
+        obj.public = v1.public
+        obj.icon = v1.icon
+        obj.resource_requests = v1.resource_requests
+        obj.resource_limits = v1.resource_limits
+        obj.versions = v1.versions
+        obj.llm_providers = v1.llm_providers
+        obj.devices = v1.devices
+        obj.repo = v1.repo
+        obj.meters = v1.meters
         obj.owner_id = owner_id
         return obj
 
     def to_record(self) -> AgentTypeRecord:
         versions = json.dumps(self.versions)
         llm_providers = None
         if self.llm_providers:
```

### Comparing `surfkit-0.1.98/surfkit/util.py` & `surfkit-0.1.99/surfkit/util.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.98/PKG-INFO` & `surfkit-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.98
+Version: 0.1.99
 Summary: A toolkit to build GUI surfing AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

