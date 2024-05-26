# Comparing `tmp/openvoicechat-0.1.4.tar.gz` & `tmp/openvoicechat-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openvoicechat-0.1.4.tar", last modified: Sun May  5 20:59:08 2024, max compression
+gzip compressed data, was "openvoicechat-0.1.5.tar", last modified: Sun May 26 09:44:31 2024, max compression
```

## Comparing `openvoicechat-0.1.4.tar` & `openvoicechat-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:59:08.720551 openvoicechat-0.1.4/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)    11357 2024-05-01 20:34:23.000000 openvoicechat-0.1.4/LICENSE
--rw-r--r--   0 fakhir    (1000) fakhir    (1000)     1198 2024-05-05 20:59:08.720551 openvoicechat-0.1.4/PKG-INFO
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1189 2024-05-04 20:22:11.000000 openvoicechat-0.1.4/README.md
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:59:08.716551 openvoicechat-0.1.4/openvoicechat/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/__init__.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:59:08.716551 openvoicechat-0.1.4/openvoicechat/llm/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      188 2024-05-04 20:22:11.000000 openvoicechat-0.1.4/openvoicechat/llm/__init__.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1884 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/llm/base.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1403 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/llm/llm_gpt.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3090 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/llm/llm_hf.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1723 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/llm/llm_llama.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)    14665 2024-05-05 20:33:56.000000 openvoicechat-0.1.4/openvoicechat/llm/prompts.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:59:08.716551 openvoicechat-0.1.4/openvoicechat/stt/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      171 2024-05-05 08:35:31.000000 openvoicechat-0.1.4/openvoicechat/stt/__init__.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3524 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/stt/base.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     2175 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/stt/stt_deepgram.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1025 2024-05-05 20:57:04.000000 openvoicechat-0.1.4/openvoicechat/stt/stt_hf.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1453 2024-05-05 20:58:18.000000 openvoicechat-0.1.4/openvoicechat/stt/stt_vosk.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3079 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/stt/utils.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1144 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/stt/vad.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:59:08.720551 openvoicechat-0.1.4/openvoicechat/tts/
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      347 2024-05-05 20:46:40.000000 openvoicechat-0.1.4/openvoicechat/tts/__init__.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     5760 2024-05-05 20:34:42.000000 openvoicechat-0.1.4/openvoicechat/tts/base.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1827 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/tts/tts_elevenlabs.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1526 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/tts/tts_hf.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     2823 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/tts/tts_parler.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1505 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/tts/tts_piper.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     3106 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/tts/tts_tortoise.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1086 2024-05-04 19:47:47.000000 openvoicechat-0.1.4/openvoicechat/tts/tts_xtts.py
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      974 2024-05-05 20:45:48.000000 openvoicechat-0.1.4/openvoicechat/utils.py
-drwxrwxr-x   0 fakhir    (1000) fakhir    (1000)        0 2024-05-05 20:59:08.720551 openvoicechat-0.1.4/openvoicechat.egg-info/
--rw-r--r--   0 fakhir    (1000) fakhir    (1000)     1198 2024-05-05 20:59:08.000000 openvoicechat-0.1.4/openvoicechat.egg-info/PKG-INFO
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      879 2024-05-05 20:59:08.000000 openvoicechat-0.1.4/openvoicechat.egg-info/SOURCES.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)        1 2024-05-05 20:59:08.000000 openvoicechat-0.1.4/openvoicechat.egg-info/dependency_links.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)      198 2024-05-05 20:59:08.000000 openvoicechat-0.1.4/openvoicechat.egg-info/requires.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)       14 2024-05-05 20:59:08.000000 openvoicechat-0.1.4/openvoicechat.egg-info/top_level.txt
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)       38 2024-05-05 20:59:08.720551 openvoicechat-0.1.4/setup.cfg
--rw-rw-r--   0 fakhir    (1000) fakhir    (1000)     1178 2024-05-05 20:59:03.000000 openvoicechat-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:31.934240 openvoicechat-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-26 09:44:31.934240 openvoicechat-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:31.930240 openvoicechat-0.1.5/openvoicechat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:31.930240 openvoicechat-0.1.5/openvoicechat/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/llm/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/llm/llm_gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/llm/llm_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/llm/llm_llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/llm/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:31.930240 openvoicechat-0.1.5/openvoicechat/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/stt_deepgram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/stt_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/stt_vosk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/stt/vad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:31.934240 openvoicechat-0.1.5/openvoicechat/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/tts_elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/tts_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/tts_parler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/tts_piper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/tts_tortoise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/tts/tts_xtts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/openvoicechat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 09:44:31.934240 openvoicechat-0.1.5/openvoicechat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-26 09:44:31.000000 openvoicechat-0.1.5/openvoicechat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-26 09:44:31.000000 openvoicechat-0.1.5/openvoicechat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 09:44:31.000000 openvoicechat-0.1.5/openvoicechat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-26 09:44:31.000000 openvoicechat-0.1.5/openvoicechat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 09:44:31.000000 openvoicechat-0.1.5/openvoicechat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 09:44:31.934240 openvoicechat-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-26 09:44:27.000000 openvoicechat-0.1.5/setup.py
```

### Comparing `openvoicechat-0.1.4/LICENSE` & `openvoicechat-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/README.md` & `openvoicechat-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,17 @@
 ### To install only the base packages
 ```shell
 pip install openvoicechat
 ```
 
 ### To install base and functionality specific packages
 ```shell
-pip install openvoicechat[piper,xtts]
+pip install openvoicechat[piper,openai,transformers]
 ```
 
 similarly "piper" and "xtts" can be replaced by any of the following
 - piper
 - vosk
-- llama
-- open_ai
+- openai
 - tortoise
 - xtts
 - transformers
```

### Comparing `openvoicechat-0.1.4/openvoicechat/llm/base.py` & `openvoicechat-0.1.5/openvoicechat/llm/base.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/openvoicechat/llm/llm_gpt.py` & `openvoicechat-0.1.5/openvoicechat/llm/llm_gpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .base import BaseChatbot
 import os
 
 class Chatbot_gpt(BaseChatbot):
-    def __init__(self, sys_prompt='', Model='gpt-3.5-turbo'):
+    def __init__(self, sys_prompt='',
+                 Model='gpt-3.5-turbo',
+                 api_key=''):
         from openai import OpenAI
         from dotenv import load_dotenv
-        load_dotenv()
-        OPENAI_API_KEY = os.getenv("OPENAI_API_KEY")
         self.MODEL = Model
-        self.client = OpenAI(api_key=OPENAI_API_KEY)
+        self.client = OpenAI(api_key=api_key)
         self.messages = []
         self.messages.append({"role": "system", "content": sys_prompt})
 
     def run(self, input_text):
         self.messages.append({"role": "user", "content": input_text})
         stream = self.client.chat.completions.create(
             model=self.MODEL,
```

### Comparing `openvoicechat-0.1.4/openvoicechat/llm/llm_hf.py` & `openvoicechat-0.1.5/openvoicechat/llm/llm_hf.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/openvoicechat/llm/llm_llama.py` & `openvoicechat-0.1.5/openvoicechat/llm/llm_llama.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/openvoicechat/llm/prompts.py` & `openvoicechat-0.1.5/openvoicechat/llm/prompts.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/openvoicechat/stt/base.py` & `openvoicechat-0.1.5/openvoicechat/stt/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 import re
 from time import monotonic
 import numpy as np
 from threading import Thread
 from queue import Queue
 
 class BaseEar:
-    def __init__(self, silence_seconds=3, not_interrupt_words=None):
+    def __init__(self, silence_seconds=3,
+                 not_interrupt_words=None,
+                 listener=None):
         if not_interrupt_words is None:
             not_interrupt_words = ['you', 'yes', 'yeah', 'hmm']  # you because whisper says "you" in silence
         self.silence_seconds = silence_seconds
         self.not_interrupt_words = not_interrupt_words
         self.vad = VoiceActivityDetection()
+        self.listener = listener
 
     @torch.no_grad()
     def transcribe(self, input: np.ndarray) -> str:
         '''
         :param input: fp32 numpy array of the audio
         :return: transcription
         '''
@@ -31,15 +34,15 @@
         raise NotImplementedError("This method should be implemented by the subclass")
 
     def listen(self) -> str:
         '''
         :return: transcription
         records audio using record_user and returns its transcription
         '''
-        audio = record_user(self.silence_seconds, self.vad)
+        audio = record_user(self.silence_seconds, self.vad, self.listener)
         text = self.transcribe(audio)
         return text
 
     def listen_stream(self) -> str:
         '''
         :return: transcription
         records audio using record_user and returns its transcription
@@ -76,15 +79,15 @@
         :param record_seconds: Max seconds to record for
         :return: boolean indicating the if an interruption occured
         Records audio with interruption. Transcribes audio if
         voice activity detected and returns True if transcription indicates
         interruption.
         '''
         while record_seconds > 0:
-            interruption_audio = record_interruption(self.vad, record_seconds)
+            interruption_audio = record_interruption(self.vad, record_seconds, streamer=self.listener)
             # duration of interruption audio
             if interruption_audio is None:
                 return ''
             else:
                 duration = len(interruption_audio) / 16_000
                 text = self.transcribe(interruption_audio)
                 # remove any punctuation using re
```

### Comparing `openvoicechat-0.1.4/openvoicechat/stt/stt_deepgram.py` & `openvoicechat-0.1.5/openvoicechat/stt/stt_deepgram.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from dotenv import load_dotenv
 import websockets
 import json
 import asyncio
 
 
 class Ear_deepgram(BaseEar):
-    def __init__(self, silence_seconds=2):
+    def __init__(self, silence_seconds=2, api_key=''):
         super().__init__(silence_seconds)
-        load_dotenv()
-        self.api_key = os.getenv('DEEPGRAM_API_KEY')
+        self.api_key = api_key
 
     def transcribe_stream(self, audio_queue, transcription_queue):
         extra_headers = {
            'Authorization': 'token ' + self.api_key
         }
         async def f():
-            async with websockets.connect('wss://api.deepgram.com/v1/listen?encoding=linear16&sample_rate=16000&channels=1&model=nova-2',
+            async with websockets.connect('wss://api.deepgram.com/v1/listen?encoding=linear16&sample_rate=16000'
+                                          '&channels=1&model=nova-2',
                                           extra_headers=extra_headers) as ws:
                 async def sender(ws):  # sends audio to websocket
                     try:
                         while True:
                             data = audio_queue.get()
                             if data is None:
                                 await ws.send(json.dumps({"type": "CloseStream"}))
```

### Comparing `openvoicechat-0.1.4/openvoicechat/stt/stt_hf.py` & `openvoicechat-0.1.5/openvoicechat/stt/stt_hf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import torch
 from .base import BaseEar
 import numpy as np
 
+
 class Ear_hf(BaseEar):
     def __init__(self, model_id='openai/whisper-base.en', device='cpu',
-                 silence_seconds=2, generate_kwargs=None):
-        super().__init__(silence_seconds)
+                 silence_seconds=2, generate_kwargs=None, listener=None):
+        super().__init__(silence_seconds, listener=listener)
         from transformers import pipeline
         self.pipe = pipeline('automatic-speech-recognition', model=model_id, device=device)
         self.device = device
         self.generate_kwargs = generate_kwargs
 
     @torch.no_grad()
     def transcribe(self, audio):
```

### Comparing `openvoicechat-0.1.4/openvoicechat/stt/stt_vosk.py` & `openvoicechat-0.1.5/openvoicechat/stt/stt_vosk.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/openvoicechat/stt/utils.py` & `openvoicechat-0.1.5/openvoicechat/stt/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 
 CHUNK = int(1024 * 2)
 FORMAT = pyaudio.paInt16
 CHANNELS = 1
 RATE = 16000
 
 
+
 def make_stream():
     p = pyaudio.PyAudio()
     return p.open(format=FORMAT,
                   channels=CHANNELS,
                   rate=RATE,
                   input=True,
                   frames_per_buffer=CHUNK)
 
 
-
-
 def record_interruption_parallel(vad, listen_queue):
     #listen for interruption untill the queue is not empty
     frames = []
     stream = make_stream()
     while True:
         a = listen_queue.get()
         if a is None:
@@ -36,41 +35,58 @@
             frames = np.frombuffer(b''.join(frames), dtype=np.int16)
             frames = frames / (1 << 15)
             return frames.astype(np.float32)
     stream.close()
     return None
 
 
-def record_interruption(vad, recond_seconds=100):
+def record_interruption(vad, record_seconds=100, streamer=None):
     print("* recording for interruption")
     frames = []
-    stream = make_stream()
-    for _ in range(0, int(RATE / CHUNK * recond_seconds)):
+    if streamer is None:
+        stream = make_stream()
+        global CHUNK
+        global RATE
+    else:
+        stream = streamer.make_stream()
+        CHUNK = streamer.CHUNK
+        RATE = streamer.RATE
+
+    for _ in range(0, int(RATE / CHUNK * record_seconds)):
         data = stream.read(CHUNK)
+        assert len(data) == CHUNK * 2, 'chunk size does not match 2 bytes per sample'
         frames.append(data)
         contains_speech = vad.contains_speech(frames[int(RATE / CHUNK) * -2:])
         if contains_speech:
             stream.close()
             frames = np.frombuffer(b''.join(frames), dtype=np.int16)
             frames = frames / (1 << 15)
             return frames.astype(np.float32)
     stream.close()
     return None
 
 
-def record_user(silence_seconds, vad):
+def record_user(silence_seconds, vad, streamer=None):
     frames = []
 
     started = False
+    if streamer is None:
+        stream = make_stream()
+        global CHUNK
+        global RATE
+    else:
+        stream = streamer.make_stream()
+        CHUNK = streamer.CHUNK
+        RATE = streamer.RATE
     one_second_iters = int(RATE / CHUNK)
-    stream = make_stream()
     print("* recording")
 
     while True:
         data = stream.read(CHUNK)
+        assert len(data) == CHUNK * 2, 'chunk size does not match 2 bytes per sample'
         frames.append(data)
         contains_speech = vad.contains_speech(frames[int(-one_second_iters * silence_seconds):])
         if not started and contains_speech:
             started = True
             print("*listening to speech*")
         if started and contains_speech is False:
             break
```

### Comparing `openvoicechat-0.1.4/openvoicechat/stt/vad.py` & `openvoicechat-0.1.5/openvoicechat/stt/vad.py`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/openvoicechat/tts/base.py` & `openvoicechat-0.1.5/openvoicechat/tts/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,72 +1,73 @@
 import sounddevice as sd
-import torch
 import re
 from time import monotonic
 import queue
 import threading
 from typing import Callable
 import numpy as np
+import inspect
+import asyncio
 
 
 def remove_words_in_brackets_and_spaces(text):
     '''
     :param text: input text
     :return: input text with the extra spaces and words in brackets removed. (e.g. [USER])
     '''
     pattern = r'\s*\[.*?\]\s*'
     cleaned_text = re.sub(pattern, ' ', text)
     cleaned_text = cleaned_text.strip()
     return cleaned_text
 
 
 class BaseMouth:
-    def __init__(self, sample_rate: int):
+    def __init__(self, sample_rate: int, player=sd):
         self.sample_rate = sample_rate
         self.sentence_stop_pattern = r'[.?](?=\s+\S)'
         self.interrupted = ''
+        self.player = player
 
-    @torch.no_grad()
     def run_tts(self, text: str) -> np.ndarray:
         '''
         :param text: The text to synthesize speech for
         :return: audio numpy array for sounddevice
         '''
         raise NotImplementedError('This method should be implemented by the subclass')
 
     def say_text(self, text: str):
         '''
         :param text: The text to synthesize speech for
         calls run_tts and plays the audio using sounddevice.
         '''
         output = self.run_tts(text)
-        sd.play(output, samplerate=self.sample_rate)
-        sd.wait()
+        self.player.play(output, samplerate=self.sample_rate)
+        self.player.wait()
 
     def say(self, audio_queue: queue.Queue, listen_interruption_func: Callable):
         '''
         :param audio_queue: The queue where the audio is stored for it to be played
         :param listen_interruption_func: callable function from the ear class.
         Plays the audios in the queue using sounddevice. Stops if interruption occurred.
         '''
         self.interrupted = ''
         while True:
             output, text = audio_queue.get()
             if output is None:
                 break
             # get the duration of audio
             duration = len(output) / self.sample_rate
-            sd.play(output, samplerate=self.sample_rate)
+            self.player.play(output, samplerate=self.sample_rate)
             interruption = listen_interruption_func(duration)
             if interruption:
-                sd.stop()
+                self.player.stop()
                 self.interrupted = (interruption, text)
                 break
             else:
-                sd.wait()
+                self.player.wait()
 
     def say_multiple(self, text: str, listen_interruption_func: Callable):
         '''
         :param text: Intput text to synthesize
         :param listen_interruption_func: callable function from the ear class
         Splits the text into sentences separated by ['.', '?', '!']. Then plays the sentences one by one
         using run_tts and say
@@ -104,42 +105,43 @@
         :param interrupt_queue: The queue where True is put when interruption occurred.
         :param audio_queue: The queue where the audio to be played is placed
         Receives text from the text_queue. As soon as a sentence is made run_tts is called to
         synthesize its speech.
         '''
         response = ''
         all_response = []
+        interrupt_text_list = []
         if audio_queue is None:
             audio_queue = queue.Queue()
         say_thread = threading.Thread(target=self.say, args=(audio_queue, listen_interruption_func))
         say_thread.start()
         while True:
             text = text_queue.get()
             if text is None:
-                sentence = remove_words_in_brackets_and_spaces(response).strip()
+                sentence = response
             else:
                 response += text
                 if bool(re.search(self.sentence_stop_pattern, response)):
                     sentences = re.split(self.sentence_stop_pattern, response, maxsplit=1)
                     sentence = sentences[0]
                     response = sentences[1]
                 else:
                     continue
             if sentence.strip() == '':
                 break
-            sentence = remove_words_in_brackets_and_spaces(sentence).strip()
-            output = self.run_tts(sentence)
-            audio_queue.put((output, sentence))
+            clean_sentence = remove_words_in_brackets_and_spaces(sentence).strip()
+            output = self.run_tts(clean_sentence)
+            audio_queue.put((output, clean_sentence))
             all_response.append(sentence)
+            interrupt_text_list.append(clean_sentence)
             if self.interrupted:
-                all_response = self._handle_interruption(all_response, interrupt_queue)
+                all_response = self._handle_interruption(interrupt_text_list, interrupt_queue)
                 self.interrupted = ''
                 break
             if text is None:
                 break
         audio_queue.put((None, ''))
         say_thread.join()
         if self.interrupted:
-            all_response = self._handle_interruption(all_response, interrupt_queue)
+            all_response = self._handle_interruption(interrupt_text_list, interrupt_queue)
         text_queue.queue.clear()
         text_queue.put('. '.join(all_response))
-
```

### Comparing `openvoicechat-0.1.4/openvoicechat/tts/tts_elevenlabs.py` & `openvoicechat-0.1.5/openvoicechat/tts/tts_elevenlabs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 import numpy as np
 import sounddevice as sd
 import requests
 import os
 
 
 class Mouth_elevenlabs(BaseMouth):
-    def __init__(self, model_id='eleven_turbo_v2', voice_id='IKne3meq5aSn9XLyUdCD'):
+    def __init__(self, model_id='eleven_turbo_v2',
+                 voice_id='IKne3meq5aSn9XLyUdCD',
+                 player=sd):
         self.model_id = model_id
         self.voice_id = voice_id
         load_dotenv()
         self.api_key = os.getenv('ELEVENLABS_API_KEY')
-        super().__init__(sample_rate=44100)
+        super().__init__(sample_rate=44100, player=player)
 
     def run_tts(self, text):
         url = f"https://api.elevenlabs.io/v1/text-to-speech/{self.voice_id}?optimize_streaming_latency=4"
         headers = {
             "Accept": "audio/mpeg",
             "Content-Type": "application/json",
             "xi-api-key": f"{self.api_key}"
```

### Comparing `openvoicechat-0.1.4/openvoicechat/tts/tts_hf.py` & `openvoicechat-0.1.5/openvoicechat/tts/tts_hf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sounddevice as sd
 import torch
 from .base import BaseMouth
 
 
 class Mouth_hf(BaseMouth):
     def __init__(self, model_id='kakao-enterprise/vits-vctk', device='cpu',
-                 forward_params=None):
+                 forward_params=None, player=sd):
         from transformers import pipeline
         self.pipe = pipeline('text-to-speech', model=model_id, device=device)
         self.device = device
         self.forward_params = forward_params
-        super().__init__(sample_rate=self.pipe.sampling_rate)
+        super().__init__(sample_rate=self.pipe.sampling_rate, player=player)
 
     @torch.no_grad()
     def run_tts(self, text):
         # inputs = self.tokenizer(text, return_tensors="pt")
         # inputs = inputs.to(self.device)
         # output = self.model(**inputs, speaker_id=self.speaker_id).waveform[0].to('cpu')
         output = self.pipe(text, forward_params=self.forward_params)
```

### Comparing `openvoicechat-0.1.4/openvoicechat/tts/tts_parler.py` & `openvoicechat-0.1.5/openvoicechat/tts/tts_parler.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 etc ....
 '''
 
 class Mouth_parler(BaseMouth):
     def __init__(self, model_id='parler-tts/parler_tts_mini_v0.1',
                  tts_description=None,
                  device='cuda:0' if torch.cuda.is_available() else 'cpu',
-                 temperature=1.0):
+                 temperature=1.0, player=sd):
         from parler_tts import ParlerTTSForConditionalGeneration
         if tts_description is None:
             tts_description = ('A female speaker with a slightly low-pitched voice delivers her words quite '
                                'expressively, in a very confined sounding environment with clear audio quality.')
         self.model = ParlerTTSForConditionalGeneration.from_pretrained(model_id).to(device)
         self.tokenizer = AutoTokenizer.from_pretrained(model_id)
         self.device = device
         self.tts_description = tts_description
         input_ids = self.tokenizer(tts_description, return_tensors="pt").input_ids.to(device)
         self.desc_tensor = BaseModelOutput(last_hidden_state=self.model.text_encoder(input_ids=input_ids).last_hidden_state)
         self.temperature = temperature
-        super().__init__(sample_rate=self.model.config.sampling_rate)
+        super().__init__(sample_rate=self.model.config.sampling_rate, player=player)
 
     def run_tts(self, text):
         prompt_input_ids = self.tokenizer(text, return_tensors="pt").input_ids.to(self.device)
         generation = self.model.generate(encoder_outputs=self.desc_tensor,
                                          prompt_input_ids=prompt_input_ids,
                                          temperature=self.temperature
                                          )
```

### Comparing `openvoicechat-0.1.4/openvoicechat/tts/tts_tortoise.py` & `openvoicechat-0.1.5/openvoicechat/tts/tts_tortoise.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         chunk = chunk.cpu().numpy()
         # wait if already playing
         sd.play(chunk, samplerate=sample_rate)
         sd.wait()
 
 
 class Mouth:
-    def __init__(self, device='cpu'):
+    def __init__(self, device='cpu', player=sd):
         from tortoise.api_fast import TextToSpeech
         from tortoise.utils.audio import load_voice
         self.model = TextToSpeech(use_deepspeed=False, kv_cache=True, half=True)
         self.sample_rate = 24000
         self.voice_samples, self.conditioning_latents = load_voice('tom')
 
     @torch.no_grad()
```

### Comparing `openvoicechat-0.1.4/openvoicechat/tts/tts_xtts.py` & `openvoicechat-0.1.5/openvoicechat/tts/tts_xtts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import sounddevice as sd
 import torch
 from .base import BaseMouth
 
+
 class Mouth_xtts(BaseMouth):
-    def __init__(self, model_id='tts_models/en/jenny/jenny', device='cpu'):
+    def __init__(self, model_id='tts_models/en/jenny/jenny', device='cpu', player=sd):
         from TTS.api import TTS
         self.model = TTS(model_id)
         self.device = device
         self.model.to(device)
-        super().__init__(sample_rate=self.model.synthesizer.output_sample_rate)
+        super().__init__(sample_rate=self.model.synthesizer.output_sample_rate, player=player)
 
     def run_tts(self, text):
         output = self.model.tts(text=text, split_sentences=False)
         return output
 
+
 if __name__ == '__main__':
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     mouth = Mouth_xtts(device=device)
 
     text = ("If there's one thing that makes me nervous about the future of self-driving cars, it's that they'll "
             "replace human drivers.\nI think there's a huge opportunity to make human-driven cars safer and more "
             "efficient. There's no reason why we can't combine the benefits of self-driving cars with the ease of use "
```

### Comparing `openvoicechat-0.1.4/openvoicechat.egg-info/SOURCES.txt` & `openvoicechat-0.1.5/openvoicechat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openvoicechat-0.1.4/setup.py` & `openvoicechat-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,28 +6,29 @@
     description='OpenVoiceChat is an opensource library that allows you to have a natural voice conversation with '
                 'your LLM agent.',
     long_description='If you plan on making an LLM agent and want to have your users be able to talk to it like a '
                      'person (low latency, handles interruptions), this library is for you. It aims to be the '
                      'opensource, highly extensible and easy to use alternative to the proprietary solutions.',
     url='http://www.fakhirali.pk/OpenVoiceChat/',
     name='openvoicechat',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'sounddevice',
         'pygame',
         'pyaudio',
         'librosa',
         'pydub',
         'python-dotenv',
-        'websockets'
+        'websockets',
+        'fastapi'
     ],
     extras_require={
         'transformers': ['transformers'],
         'piper': ['piper-tts', 'piper-phonemize'],
         'vosk': ['vosk'],
-        'open_ai': ['openai'],
+        'openai': ['openai'],
         'tortoise': ['tortoise-tts'],
         'xtts': ['TTS'],
     },
     dependency_links=[],
 )
```

