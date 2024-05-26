# Comparing `tmp/aiy_worker-0.0.6.tar.gz` & `tmp/aiy_worker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiy_worker-0.0.6.tar", last modified: Sat May 25 11:37:10 2024, max compression
+gzip compressed data, was "aiy_worker-0.0.7.tar", last modified: Sun May 26 07:29:39 2024, max compression
```

## Comparing `aiy_worker-0.0.6.tar` & `aiy_worker-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-25 11:37:10.456444 aiy_worker-0.0.6/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-25 11:37:10.455837 aiy_worker-0.0.6/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.6/README.md
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-25 11:37:10.452938 aiy_worker-0.0.6/aiy_worker/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.6/aiy_worker/__init__.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1594 2024-05-25 08:02:04.000000 aiy_worker-0.0.6/aiy_worker/types.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.6/aiy_worker/utils.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     6315 2024-05-25 11:20:52.000000 aiy_worker-0.0.6/aiy_worker/worker.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)    10768 2024-05-25 11:19:01.000000 aiy_worker-0.0.6/aiy_worker/ws_client.py
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-25 11:37:10.454923 aiy_worker-0.0.6/aiy_worker.egg-info/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/SOURCES.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/dependency_links.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/requires.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-05-25 11:37:10.000000 aiy_worker-0.0.6/aiy_worker.egg-info/top_level.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-05-25 11:37:10.456595 aiy_worker-0.0.6/setup.cfg
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-05-25 11:36:59.000000 aiy_worker-0.0.6/setup.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 07:29:39.040728 aiy_worker-0.0.7/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-26 07:29:39.040296 aiy_worker-0.0.7/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.7/README.md
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 07:29:39.036883 aiy_worker-0.0.7/aiy_worker/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.7/aiy_worker/__init__.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     2205 2024-05-26 07:24:56.000000 aiy_worker-0.0.7/aiy_worker/types.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.7/aiy_worker/utils.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     6872 2024-05-26 07:26:56.000000 aiy_worker-0.0.7/aiy_worker/worker.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)    10768 2024-05-25 11:19:01.000000 aiy_worker-0.0.7/aiy_worker/ws_client.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-05-26 07:29:39.039701 aiy_worker-0.0.7/aiy_worker.egg-info/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-05-26 07:29:38.000000 aiy_worker-0.0.7/aiy_worker.egg-info/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-05-26 07:29:38.000000 aiy_worker-0.0.7/aiy_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-05-26 07:29:38.000000 aiy_worker-0.0.7/aiy_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-05-26 07:29:38.000000 aiy_worker-0.0.7/aiy_worker.egg-info/requires.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-05-26 07:29:38.000000 aiy_worker-0.0.7/aiy_worker.egg-info/top_level.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-05-26 07:29:39.040818 aiy_worker-0.0.7/setup.cfg
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-05-26 07:28:39.000000 aiy_worker-0.0.7/setup.py
```

### Comparing `aiy_worker-0.0.6/aiy_worker/types.py` & `aiy_worker-0.0.7/aiy_worker/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from enum import Enum
 from typing import List
 
 class PayloadErrorLocation:
     line: int
     column: int
     def __init__(self, location: dict):
         self.line = location['line']
@@ -24,22 +25,43 @@
         self.negative_prompt = props.get('negativePrompt')
         self.seed = props.get('seed')
         self.width = props.get('width')
         self.height = props.get('height')
         self.n_steps = props.get('nSteps')
         self.ip_adapter_image_url = props.get('ipAdapterImageUrl')
 
+class CannyProps:
+    def __init__(self, props: dict) -> None:
+        self.image_url = props.get('imageUrl')
+
+class TaskKind(Enum):
+    TEXT_TO_IMAGE = 1
+    CANNY = 2
+
 class Task:
     def __init__(self, data: dict):
         if data is None:
             return
         subscribe_task: dict = data.get('subscribeTasks')
         if subscribe_task:
             self.id = subscribe_task.get('id')
-            self.text2Image = Text2ImageProps(subscribe_task.get('text2Image'))
+            self.text2Image = None
+            if subscribe_task.get('text2Image'):
+                Text2ImageProps(subscribe_task.get('text2Image'))
+            self.canny = None
+            if subscribe_task.get('canny'):
+                self.canny = CannyProps(subscribe_task.get('canny'))
+
+    @property
+    def kind(self):
+        if self.text2Image is not None:
+            return TaskKind.TEXT_TO_IMAGE
+        if self.canny is not None:
+            return TaskKind.CANNY
+        return None
 
 class Payload:
     def __init__(self, payload: dict) -> None:
         self.errors = [PayloadError(i) for i in payload.get('errors', [])]
         self.task = Task(payload.get('data', {}))
```

### Comparing `aiy_worker-0.0.6/aiy_worker/utils.py` & `aiy_worker-0.0.7/aiy_worker/utils.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.6/aiy_worker/worker.py` & `aiy_worker-0.0.7/aiy_worker/worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from enum import Enum
 from typing import Callable, List
 import requests
 from .ws_client import GraphQLClient
-from .types import WsData, Task, PayloadError
+from .types import TaskKind, WsData, Task, PayloadError
 from .utils import encode_image, png2webp, png2avif, make_thumbnail, check_pngquant_bin, timer, handle_image
 import logging
 from PIL import Image
 
 logger = logging.getLogger(__name__)
 
 sub_task_query = """
@@ -19,14 +19,17 @@
             negativePrompt
             seed
             width
             height
             nSteps,
             ipAdapterImageUrl
         }
+        canny {
+            imageUrl
+        }
     }
   }
 """
 
 
 def wait_shutdown(fn: Callable):
     import signal
@@ -77,24 +80,29 @@
                         self.__submit_task_result(task, TaskState.RECEIVED)
                 def _set_progress(progress: float):
                     self.set_progress(task, progress)
                 import threading
                 t = threading.Thread(target=received, args=(task,))
                 t.start()
                 logger.info("Start to generate image")
-                images = self.on_task(task, _set_progress)
+                if task.kind == TaskKind.TEXT_TO_IMAGE:
+                    images = self.on_task(task, _set_progress)
+                if task.kind == TaskKind.CANNY:
+                    images = self.on_canny_task(task, _set_progress)
+                else:
+                    raise Exception('Task kind is NONE')
                 # 等待 submit 成功
                 t.join()
-                logger.info("text2images successfully")       
+                logger.info(f"Execute task successfully")       
                 with timer('handle image[0]'):
                     result, suffix, thumbnail = handle_image(images[0])
                 with timer('set worker state to SUCCESSFUL'):
                     self.__submit_task_result(task, TaskState.SUCCESSFUL, None, result, suffix, thumbnail)
             except Exception as e:
-                logger.info(e)
+                logger.error(e)
                 self.__submit_task_result(task, TaskState.FAILED)
 
     def __submit_task_result(self, task: Task, state: TaskState, progress: float = None,
                              result: str = None, suffix: str = None, thumbnail_base64: str=None):
         logger.info(f"set worker's state to {state}")
         query = """
 mutation ($task_id: Int!, $worker_token: String!, $progress: Float, $result: String, $suffix: String, $thumbnail_base64: String) {{
@@ -147,14 +155,18 @@
             if len(errors) > 0:
                 logger.info('Error: %s' % errors[0].message)
 
     def on_task(self, task: Task, progress_callback: Callable[[float], None]) -> List[Image.Image]:
         """ 接收到任务，并进行处理，返回处理结果（生成的图片的路径） """
         raise NotImplementedError
 
+    def on_canny_task(self, task: Task, progress_callback: Callable[[float], None]) -> List[Image.Image]:
+        """ 处理生成 Canny 图片的任务 """
+        logger.exception('This worker not support canny task, but still received')
+
     def set_progress(self, task: Task, progress: float):
         """ 设置进度条 """
         logger.info(f'progress: {progress}')
         self.__submit_task_result(task, TaskState.GENERATING, progress)
 
     def run(self):
         logger.info("Starting...")
```

### Comparing `aiy_worker-0.0.6/aiy_worker/ws_client.py` & `aiy_worker-0.0.7/aiy_worker/ws_client.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.6/setup.py` & `aiy_worker-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if os.path.exists("requirements.txt"):
     install_requires = [i for i in io.open("requirements.txt").read().split("\n") if i]
 else:
     install_requires = []
 print(install_requires)
 setuptools.setup(
     name="aiy_worker",
-    version="0.0.6",
+    version="0.0.7",
     author="zgljl2012",
     # license = 'MIT License',
     # author_email="pengshiyuyx@gmail.com",
     description="aiy worker",
     long_description=long_description,
     # long_description_content_type="text/x-rst",
     # url="https://github.com/mouday/chinesename",
```

