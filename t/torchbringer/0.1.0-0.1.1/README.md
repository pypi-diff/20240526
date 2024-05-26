# Comparing `tmp/torchbringer-0.1.0.tar.gz` & `tmp/torchbringer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbringer-0.1.0.tar", last modified: Sun May 26 16:06:20 2024, max compression
+gzip compressed data, was "torchbringer-0.1.1.tar", last modified: Sun May 26 16:29:47 2024, max compression
```

## Comparing `torchbringer-0.1.0.tar` & `torchbringer-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.786769 torchbringer-0.1.0/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-25 23:44:21.000000 torchbringer-0.1.0/LICENSE
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      727 2024-05-26 16:06:20.786769 torchbringer-0.1.0/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5008 2024-05-26 15:39:27.000000 torchbringer-0.1.0/README.md
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-26 16:06:20.786769 torchbringer-0.1.0/setup.cfg
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      913 2024-05-26 16:05:54.000000 torchbringer-0.1.0/setup.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.776769 torchbringer-0.1.0/torchbringer/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-26 16:06:18.000000 torchbringer-0.1.0/torchbringer/__init__.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.776769 torchbringer-0.1.0/torchbringer/components/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2757 2024-05-26 15:48:03.000000 torchbringer-0.1.0/torchbringer/components/builders.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      610 2024-05-25 16:10:22.000000 torchbringer-0.1.0/torchbringer/components/epsilon.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-25 17:27:12.000000 torchbringer-0.1.0/torchbringer/components/replay_memory.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.776769 torchbringer-0.1.0/torchbringer/examples/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-26 15:39:23.000000 torchbringer-0.1.0/torchbringer/examples/cartpole_grpc_dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-26 15:39:22.000000 torchbringer-0.1.0/torchbringer/examples/cartpole_local_dqn.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.776769 torchbringer-0.1.0/torchbringer/learners/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4941 2024-05-26 15:47:32.000000 torchbringer-0.1.0/torchbringer/learners/dqn.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-25 15:17:44.000000 torchbringer-0.1.0/torchbringer/learners/learner_utils.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.776769 torchbringer-0.1.0/torchbringer/servers/
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.776769 torchbringer-0.1.0/torchbringer/servers/grpc/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-26 15:38:36.000000 torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_grpc_client.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-26 15:41:48.000000 torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_grpc_server.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-26 15:50:10.000000 torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_pb2.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-26 15:50:10.000000 torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_pb2.pyi
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-26 15:52:44.000000 torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-26 15:38:36.000000 torchbringer-0.1.0/torchbringer/servers/torchbringer_agent.py
-drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:06:20.786769 torchbringer-0.1.0/torchbringer.egg-info/
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      727 2024-05-26 16:06:20.000000 torchbringer-0.1.0/torchbringer.egg-info/PKG-INFO
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)      792 2024-05-26 16:06:20.000000 torchbringer-0.1.0/torchbringer.egg-info/SOURCES.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-26 16:06:20.000000 torchbringer-0.1.0/torchbringer.egg-info/dependency_links.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       84 2024-05-26 16:06:20.000000 torchbringer-0.1.0/torchbringer.egg-info/requires.txt
--rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-26 16:06:20.000000 torchbringer-0.1.0/torchbringer.egg-info/top_level.txt
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1058 2024-05-25 23:44:21.000000 torchbringer-0.1.1/LICENSE
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7056 2024-05-26 16:29:47.686786 torchbringer-0.1.1/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     6287 2024-05-26 16:19:58.000000 torchbringer-0.1.1/README.md
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       38 2024-05-26 16:29:47.686786 torchbringer-0.1.1/setup.cfg
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1130 2024-05-26 16:29:29.000000 torchbringer-0.1.1/setup.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      137 2024-05-26 16:29:37.000000 torchbringer-0.1.1/torchbringer/__init__.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/components/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2757 2024-05-26 15:48:03.000000 torchbringer-0.1.1/torchbringer/components/builders.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      610 2024-05-25 16:10:22.000000 torchbringer-0.1.1/torchbringer/components/epsilon.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      547 2024-05-25 17:27:12.000000 torchbringer-0.1.1/torchbringer/components/replay_memory.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/examples/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2547 2024-05-26 15:39:23.000000 torchbringer-0.1.1/torchbringer/examples/cartpole_grpc_dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2517 2024-05-26 15:39:22.000000 torchbringer-0.1.1/torchbringer/examples/cartpole_local_dqn.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/learners/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     4941 2024-05-26 15:47:32.000000 torchbringer-0.1.1/torchbringer/learners/dqn.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      330 2024-05-25 15:17:44.000000 torchbringer-0.1.1/torchbringer/learners/learner_utils.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/servers/
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer/servers/grpc/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      957 2024-05-26 15:38:36.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_client.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1882 2024-05-26 15:41:48.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_server.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     2022 2024-05-26 15:50:10.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     1536 2024-05-26 15:50:10.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.pyi
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     5450 2024-05-26 15:52:44.000000 torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      583 2024-05-26 15:38:36.000000 torchbringer-0.1.1/torchbringer/servers/torchbringer_agent.py
+drwxr-xr-x   0 moraguma  (1000) moraguma  (1000)        0 2024-05-26 16:29:47.686786 torchbringer-0.1.1/torchbringer.egg-info/
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)     7056 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/PKG-INFO
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)      792 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/SOURCES.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)        1 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/dependency_links.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       84 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/requires.txt
+-rw-r--r--   0 moraguma  (1000) moraguma  (1000)       32 2024-05-26 16:29:47.000000 torchbringer-0.1.1/torchbringer.egg-info/top_level.txt
```

### Comparing `torchbringer-0.1.0/LICENSE` & `torchbringer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/README.md` & `torchbringer-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,58 @@
 TorchBringer is an open-source framework that provides a simple interface for operating with pre-implemented deep reinforcement learning algorithms built on top of PyTorch. The interfaces provided can be used to operate deep RL agents either locally or remotely via gRPC. Currently, TorchBringer supports the following algorithms
 
 - [x] DQN
 
+## Quickstart
+
+To install TorchBringer, run
+
+```bash
+pip install --upgrade pip
+pip install torchbringer
+```
+
+Here's a simple project for running a TorchBringer agent on gymnasium's Cartpole environment.
+
+```python
+import gymnasium as gym
+from itertools import count
+import torch
+from torchbringer.servers.torchbringer_agent import TorchBringerAgent
+
+env = gym.make("CartPole-v1")
+state, info = env.reset()
+
+config = {
+    # Check the reference section to understand config formatting
+}
+
+dqn = TorchBringerAgent()
+dqn.initialize(config)
+steps_done = 0
+
+num_episodes = 600
+for i_episode in range(num_episodes):
+    # Initialize the environment and get its state
+    state, info = env.reset()
+    reward = torch.tensor([0.0], device=device)
+    terminal = False
+    
+    state = torch.tensor(state, dtype=torch.float32, device=device).unsqueeze(0)
+    for t in count():
+        observation, reward, terminated, truncated, _ = env.step(dqn.step(state, reward, terminal).item())
+        state = None if terminated else torch.tensor(observation, dtype=torch.float32, device=device).unsqueeze(0) 
+        reward = torch.tensor([reward], device=device)
+        terminal = terminated or truncated
+
+        if terminal:
+            dqn.step(state, reward, terminal)
+            break
+```
+
 ## Reference
 
 `cartpole_local_dqn.py` provides a simple example of TorchBringer being used on gymnasium's CartPole-v1 envinronment. `cartpole_grpc_dqn.py` provides an example of how to use the gRPC interface to learn remotely.
 
 The main class that is used in this framework is `TorchBringerAgent`, implemented in `servers/`. The gRPC server has an interface very similar to it.
 
 ### TorchBringerAgent
```

### Comparing `torchbringer-0.1.0/setup.py` & `torchbringer-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from setuptools import setup, find_namespace_packages
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name='torchbringer',
-    version='0.1.0',    
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    version='0.1.1',    
     description='A PyTorch library for deep reinforcement learning ',
     url='https://github.com/moraguma/TorchBringer',
     author='Moraguma',
     author_email='g170603@dac.unicamp.br',
     license='MIT',
     packages=find_namespace_packages(),
     install_requires=[
```

### Comparing `torchbringer-0.1.0/torchbringer/components/builders.py` & `torchbringer-0.1.1/torchbringer/components/builders.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/components/epsilon.py` & `torchbringer-0.1.1/torchbringer/components/epsilon.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/components/replay_memory.py` & `torchbringer-0.1.1/torchbringer/components/replay_memory.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/examples/cartpole_grpc_dqn.py` & `torchbringer-0.1.1/torchbringer/examples/cartpole_grpc_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/examples/cartpole_local_dqn.py` & `torchbringer-0.1.1/torchbringer/examples/cartpole_local_dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/learners/dqn.py` & `torchbringer-0.1.1/torchbringer/learners/dqn.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_grpc_client.py` & `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_client.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_grpc_server.py` & `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_grpc_server.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_pb2.py` & `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_pb2.pyi` & `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/servers/grpc/torchbringer_pb2_grpc.py` & `torchbringer-0.1.1/torchbringer/servers/grpc/torchbringer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer/servers/torchbringer_agent.py` & `torchbringer-0.1.1/torchbringer/servers/torchbringer_agent.py`

 * *Files identical despite different names*

### Comparing `torchbringer-0.1.0/torchbringer.egg-info/SOURCES.txt` & `torchbringer-0.1.1/torchbringer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

