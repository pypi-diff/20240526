# Comparing `tmp/manim_speech-0.1.0.tar.gz` & `tmp/manim_speech-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_speech-0.1.0.tar", last modified: Thu May 23 03:13:48 2024, max compression
+gzip compressed data, was "manim_speech-0.2.0.tar", last modified: Sun May 26 11:14:38 2024, max compression
```

## Comparing `manim_speech-0.1.0.tar` & `manim_speech-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:13:48.903602 manim_speech-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 03:13:44.000000 manim_speech-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-23 03:13:48.903602 manim_speech-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-23 03:13:44.000000 manim_speech-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-23 03:13:44.000000 manim_speech-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 03:13:48.903602 manim_speech-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:13:48.899602 manim_speech-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:13:48.899602 manim_speech-0.1.0/src/manim_speech/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:13:48.903602 manim_speech-0.1.0/src/manim_speech/services/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/assemblyai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/deepl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/services/whisper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/speech.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-23 03:13:44.000000 manim_speech-0.1.0/src/manim_speech/translation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 03:13:48.903602 manim_speech-0.1.0/src/manim_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-23 03:13:48.000000 manim_speech-0.1.0/src/manim_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-23 03:13:48.000000 manim_speech-0.1.0/src/manim_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 03:13:48.000000 manim_speech-0.1.0/src/manim_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-23 03:13:48.000000 manim_speech-0.1.0/src/manim_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 03:13:48.000000 manim_speech-0.1.0/src/manim_speech.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:14:38.703861 manim_speech-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-26 11:14:30.000000 manim_speech-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-26 11:14:38.703861 manim_speech-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-26 11:14:30.000000 manim_speech-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-26 11:14:30.000000 manim_speech-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:14:38.703861 manim_speech-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:14:38.699861 manim_speech-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:14:38.699861 manim_speech-0.2.0/src/manim_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:14:38.703861 manim_speech-0.2.0/src/manim_speech/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/assemblyai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/deepl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/services/whisper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/speech.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-26 11:14:30.000000 manim_speech-0.2.0/src/manim_speech/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:14:38.703861 manim_speech-0.2.0/src/manim_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-26 11:14:38.000000 manim_speech-0.2.0/src/manim_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-26 11:14:38.000000 manim_speech-0.2.0/src/manim_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 11:14:38.000000 manim_speech-0.2.0/src/manim_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-26 11:14:38.000000 manim_speech-0.2.0/src/manim_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-26 11:14:38.000000 manim_speech-0.2.0/src/manim_speech.egg-info/top_level.txt
```

### Comparing `manim_speech-0.1.0/LICENSE` & `manim_speech-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_speech-0.1.0/PKG-INFO` & `manim_speech-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_speech
-Version: 0.1.0
+Version: 0.2.0
 Summary: Manim plugin for adding speech to videos.
 Author-email: Celeste Ma <mtcelestema@proton.me>
 License: MIT License
         
         Copyright (c) 2024 Celeste Ma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,20 +22,21 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/MtCelesteMa/manim-speech
+Project-URL: Repository, https://github.com/MtCelesteMa/manim-speech
 Project-URL: Bug Tracker, https://github.com/MtCelesteMa/manim-speech/issues
 Keywords: manim,speech,voiceover,tts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: manim
 Requires-Dist: pydantic
 Requires-Dist: mutagen
@@ -66,61 +67,69 @@
 pip install "manim_speech[*optional_dependency_sets*]"
 ```
 
 Where `*optional_dependency_sets*` is a list of optional dependency sets for Manim Speech.
 
 ## Features
 
-* Adding AI-generated voiceovers to Manim animations.
-* Translating text between languages.
+* Integrate voiceovers into Manim animations.
+
+    * Utilize bookmarks to pause for key moments in the voiceover (identical to Manim Voiceover functionality).
+
+* Easily translate text within Manim animations to various languages with minimal code.
+
+* Leverage AI-driven services for text-to-speech, speech-to-text, and translation.
 
 ### Services
 
 | Service Name | Optional Dependency Set | Is Local | Text-To-Speech | Speech-To-Text | Translation |
 |--------------|-------------------------|----------|----------------|----------------|-------------|
-| OpenAI       | `openai`                | No       | Yes            | Yes            | No          |
+| OpenAI       | `openai`                | No       | Yes            | Yes            | Yes         |
 | ElevenLabs   | `elevenlabs`            | No       | Yes            | No             | No          |
 | Whisper      | `whisper`               | Yes      | No             | Yes            | No          |
 | AssemblyAI   | `assemblyai`            | No       | No             | Yes            | No          |
 | DeepL        | `deepl`                 | No       | No             | No             | Yes         |
 
-**Note:** Translating to Traditional Chinese (`zh_tw`) using the DeepL service requires the `chinese` optional dependency set to be installed.
+#### Notes on Chinese Translations
+
+**OpenAI Translator:** Please specify Traditional (`zh_tw`) or Simplified (`zh_cn`) when using the OpenAI translator. Only specifying `zh` has no guarantee on the script used, although tests have indicated that GPT-4o strongly prefers Simplified Chinese in such cases.
+
+**DeepL Translator:** The DeepL translator does not natively support translating to Traditional Chinese, so translating to Traditional Chinese requires the `chinese` optional dependency set to be installed. Only specifying `zh` has the same effect as specifying `zh_cn`.
 
 ## Usage Examples
 
 Creating a basic scene with a voiceover with Manim Speech:
 ```python
 import manim
 import manim_speech
 from manim_speech.services import openai as openai_service
 
 class MeaningOfLife(manim_speech.VoiceoverScene):
     def construct(self) -> None:
-        self.set_tts_service(openai_service.OpenAITTSService())
-        self.set_stt_service(openai_service.OpenAISTTService())
+        self.set_tts_service(openai_service.OpenAITTSService()) # Remove this line if you want to manually record voiceovers.
+        self.set_stt_service(openai_service.OpenAISTTService()) # Only required if you use bookmarks.
 
         with self.voiceover("What is the meaning of life?") as speech_data:
             txt = manim.Text("The meaning of life is 42.")
             self.play(manim.Write(txt), run_time=speech_data.duration)
             self.wait_for_voiceover()
             self.play(manim.FadeOut(txt))
 ```
 
 The same scene, but translated into Traditional Chinese:
 ```python
 import manim
 import manim_speech
 from manim_speech.services import openai as openai_service
-from manim_speech.services import deepl as deepl_service
 
 class MeaningOfLife(manim_speech.VoiceoverScene, manim_speech.TranslationScene):
     def construct(self) -> None:
-        self.set_tts_service(openai_service.OpenAITTSService())
-        self.set_stt_service(openai_service.OpenAISTTService())
-        self.set_translation_service(deepl_service.DeepLTranslationService())
+        self.set_tts_service(openai_service.OpenAITTSService()) # Remove this line if you want to manually record voiceovers.
+        self.set_stt_service(openai_service.OpenAISTTService()) # Only required if you use bookmarks.
+        self.set_translation_service(openai_service.OpenAITranslationService()) # Remove this line if you want to manually translate text.
 
         self.translate(__file__, "meaning_of_life", "en", "zh_tw")
         _ = self._
 
         with self.voiceover(_("What is the meaning of life?")) as speech_data:
             txt = manim.Text(_("The meaning of life is 42."))
             self.play(manim.Write(txt), run_time=speech_data.duration)
```

### Comparing `manim_speech-0.1.0/pyproject.toml` & `manim_speech-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "manim_speech"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
     "manim",
     "pydantic",
     "mutagen",
     "polib"
 ]
 requires-python = ">=3.12"
@@ -19,22 +19,23 @@
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["manim", "speech", "voiceover", "tts"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Topic :: Multimedia :: Sound/Audio :: Speech",
-    "License :: OSI Approved :: Apache Software License",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.12"
 ]
 
 [project.optional-dependencies]
 openai = ["openai"]
 elevenlabs = ["elevenlabs"]
 whisper = ["openai-whisper"]
 assemblyai = ["assemblyai"]
 deepl = ["deepl"]
 chinese = ["opencc"]
 
 [project.urls]
 Homepage = "https://github.com/MtCelesteMa/manim-speech"
+Repository = "https://github.com/MtCelesteMa/manim-speech"
 "Bug Tracker" = "https://github.com/MtCelesteMa/manim-speech/issues"
```

### Comparing `manim_speech-0.1.0/src/manim_speech/scene.py` & `manim_speech-0.2.0/src/manim_speech/scene.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import pathlib
 import gettext
 
 import manim
 
 
 class VoiceoverScene(manim.Scene):
-    tts_service: services.base.TTSService
-    stt_service: services.base.STTService
+    tts_service: services.base.TTSService | None = None
+    stt_service: services.base.STTService | None = None
     current_speech_data: speech.SpeechData | None = None
     current_speech_start_time: float | None = None
 
     def set_tts_service(self, service: services.base.TTSService) -> None:
         self.tts_service = service
     
     def set_stt_service(self, service: services.base.STTService) -> None:
@@ -34,36 +34,32 @@
     
     def wait_until_bookmark(self, key: str) -> None:
         if not isinstance(self.current_speech_data, type(None)) and not isinstance(self.current_speech_start_time, type(None)):
             self.safe_wait(self.current_speech_data.bookmark_times[key] - (self.renderer.time - self.current_speech_start_time))
     
     @contextlib.contextmanager
     def voiceover(self, text: str) -> abc.Generator[speech.SpeechData, None, None]:
-        if not hasattr(self, "tts_service"):
-            raise AttributeError("TTS service not set")
-        if not hasattr(self, "stt_service"):
-            raise AttributeError("STT service not set")
+        if not isinstance(self.stt_service, services.base.STTService):
+            manim.logger.warning("No STT service is set. Bookmark locations will be inaccurate.")
         try:
             self.current_speech_data = speech.create(text, self.tts_service, self.stt_service)
             self.current_speech_start_time = self.renderer.time
             self.add_sound(str(pathlib.Path(manim.config.media_dir) / "manim_speech" / self.current_speech_data.tts_data.output.audio_path))
             yield self.current_speech_data
         finally:
             self.wait_for_voiceover()
             self.current_speech_data = None
             self.current_speech_start_time = None
 
 
 class TranslationScene(manim.Scene):
-    translation_service: services.base.TranslationService
+    translation_service: services.base.TranslationService | None = None
     _ = staticmethod(gettext.gettext)
 
     def set_translation_service(self, service: services.base.TranslationService) -> None:
         self.translation_service = service
     
     def translate(self, file: pathlib.Path | str, domain: str, source_language: str, target_language: str,) -> None:
-        if not hasattr(self, "translation_service"):
-            raise AttributeError("Translation service not set")
         translation.init_translation_env(file, domain)
         translation.translate_po_file(domain, source_language, target_language, service=self.translation_service)
         trans = gettext.translation(domain, languages=[target_language], localedir="locales")
         self._ = trans.gettext
```

### Comparing `manim_speech-0.1.0/src/manim_speech/services/assemblyai.py` & `manim_speech-0.2.0/src/manim_speech/services/assemblyai.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,27 +67,27 @@
 
         aai.settings.api_key = self.api_key
         transcriber = aai.Transcriber(config=self.config)
         response = transcriber.transcribe(str(self.cache_dir / input.audio_path))
         if response.error:
             raise ValueError(response.error)
 
-        word_boundaries: list[base.WordBoundary] = []
+        word_boundaries: list[base.Boundary] = []
         text_offset = 0
         for word in response.words:
             word_boundaries.append(
-                base.WordBoundary(
-                    word=word.text,
+                base.Boundary(
+                    text=word.text,
                     start=word.start / 1000,
                     end=word.end / 1000,
                     text_offset=text_offset
                 )
             )
             if text_offset != 0 and response.text[text_offset] == " ":
                 text_offset += 1
             text_offset += len(word.text)
     
         return base.STTData(
             info=info,
             input=input,
-            output=base.STTOutput(text=response.text, word_boundaries=word_boundaries)
+            output=base.STTOutput(text=response.text, boundaries=word_boundaries)
         )
```

### Comparing `manim_speech-0.1.0/src/manim_speech/services/base.py` & `manim_speech-0.2.0/src/manim_speech/services/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,54 +41,55 @@
 
 
 class TTSOutput(pydantic.BaseModel):
     audio_path: pathlib.Path
 
 
 class TTSData(pydantic.BaseModel):
-    info: ServiceInfo
+    info: ServiceInfo | None
     input: TTSInput
     output: TTSOutput
 
 
 class TTSService(Service, ABC):
     @property
     def service_type(self) -> str:
         return "TTS"
     
-    def get_file_name(self, input: TTSInput) -> pathlib.Path:
+    @staticmethod
+    def get_file_name(input: TTSInput) -> pathlib.Path:
         return pathlib.Path(f"{hashlib.sha256(input.text.encode()).hexdigest()}.mp3")
     
     @abstractmethod
     def tts(self, input: TTSInput) -> TTSData:
         raise NotImplementedError
 
 
-class WordBoundary(pydantic.BaseModel):
-    word: str
+class Boundary(pydantic.BaseModel):
+    text: str
     start: float
     end: float
     text_offset: int
 
     @property
-    def word_length(self) -> int:
-        return len(self.word)
+    def length(self) -> int:
+        return len(self.text)
 
 
 class STTInput(pydantic.BaseModel):
     audio_path: pathlib.Path
 
 
 class STTOutput(pydantic.BaseModel):
     text: str
-    word_boundaries: list[WordBoundary]
+    boundaries: list[Boundary]
 
 
 class STTData(pydantic.BaseModel):
-    info: ServiceInfo
+    info: ServiceInfo | None
     input: STTInput
     output: STTOutput
 
 
 class STTService(Service, ABC):
     @property
     def service_type(self) -> str:
@@ -106,15 +107,15 @@
 
 
 class TranslationOutput(pydantic.BaseModel):
     translated_text: str
 
 
 class TranslationData(pydantic.BaseModel):
-    info: ServiceInfo
+    info: ServiceInfo | None
     input: TranslationInput
     output: TranslationOutput
 
 
 class TranslationService(Service, ABC):
     @property
     def service_type(self) -> str:
```

### Comparing `manim_speech-0.1.0/src/manim_speech/services/deepl.py` & `manim_speech-0.2.0/src/manim_speech/services/deepl.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,9 +40,12 @@
         if input.target_language == "zh_tw":
             try:
                 import opencc
             except ImportError:
                 raise ImportError("Please install opencc with `pip install opencc`")
             result = self.client.translate_text(input.text, source_lang=input.source_language, target_lang="zh", tag_handling="xml")
             return base.TranslationData(info=info, input=input, output=base.TranslationOutput(translated_text=opencc.OpenCC("s2t.json").convert(result.text)))
-        result = self.client.translate_text(input.text, source_lang=input.source_language, target_lang=input.target_language, tag_handling="xml")
+        target_language = input.target_language
+        if target_language == "zh_cn":
+            target_language = "zh"
+        result = self.client.translate_text(input.text, source_lang=input.source_language, target_lang=target_language, tag_handling="xml")
         return base.TranslationData(info=info, input=input, output=base.TranslationOutput(translated_text=result.text))
```

### Comparing `manim_speech-0.1.0/src/manim_speech/services/elevenlabs.py` & `manim_speech-0.2.0/src/manim_speech/services/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `manim_speech-0.1.0/src/manim_speech/services/whisper.py` & `manim_speech-0.2.0/src/manim_speech/services/whisper.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,25 +36,25 @@
             service_name=self.service_name,
             service_type=self.service_type,
             config={"model": self.model, "device": self.device}
         )
 
         transcript = self.model_obj.transcribe(str(self.cache_dir / input.audio_path), word_timestamps=True)
 
-        word_boundaries: list[base.WordBoundary] = []
+        word_boundaries: list[base.Boundary] = []
         text_offset = 0
         for segment in transcript["segments"]:
             for word in segment["words"]:
                 word_boundaries.append(
-                    base.WordBoundary(
-                        word=word["word"],
+                    base.Boundary(
+                        text=word["word"],
                         start=word["start"],
                         end=word["end"],
                         text_offset=text_offset
                     )
                 )
                 if text_offset != 0 and response.text[text_offset] == " ":
                     text_offset += 1
                 text_offset += len(word["word"])
         
-        return base.STTData(info=info, input=input, output=base.STTOutput(text=transcript["text"], word_boundaries=word_boundaries))
+        return base.STTData(info=info, input=input, output=base.STTOutput(text=transcript["text"], boundaries=word_boundaries))
```

### Comparing `manim_speech-0.1.0/src/manim_speech/speech.py` & `manim_speech-0.2.0/src/manim_speech/speech.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 def remove_bookmarks(s: str) -> str:
     return re.sub(r"<bookmark\s*mark\s*=['\"]\w*[\"']\s*/>", "", s)
 
 
 def get_bookmark_times(text: str, tts_data: services.base.TTSData, stt_data: services.base.STTData) -> dict[str, float]:
     interpolator = interpolate.interp1d(
-        [wb.text_offset for wb in stt_data.output.word_boundaries],
-        [wb.start for wb in stt_data.output.word_boundaries],
+        [wb.text_offset for wb in stt_data.output.boundaries] + [len(stt_data.output.text)],
+        [wb.start for wb in stt_data.output.boundaries] + [stt_data.output.boundaries[-1].end],
         fill_value="extrapolate"
     )
 
     text_len = len(tts_data.input.text)
     transcribed_text_len = len(stt_data.output.text.strip())
 
     bookmark_dist: dict[str, int] = {}
@@ -59,16 +59,16 @@
         cache_dir.mkdir(parents=True)
     with (cache_dir / "cache.json").open("w") as f:
         f.write(pydantic.TypeAdapter(list[SpeechData]).dump_json(data, indent=4).decode("utf-8"))
 
 
 def create(
         text: str,
-        tts_service: services.base.TTSService,
-        stt_service: services.base.STTService,
+        tts_service: services.base.TTSService | None = None,
+        stt_service: services.base.STTService | None = None,
         *,
         cache_dir: pathlib.Path | str | None = None
 ) -> SpeechData:
     if isinstance(cache_dir, type(None)):
         cache_dir = pathlib.Path(manim.config.media_dir) / "manim_speech"
     elif isinstance(cache_dir, str):
         cache_dir = pathlib.Path(cache_dir)
@@ -81,16 +81,46 @@
         for data in cache:
             if data.text == text:
                 return data
     else:
         cache = []
 
     input_text = remove_bookmarks(text)
-    tts_data = tts_service.tts(services.base.TTSInput(text=input_text))
-    stt_data = stt_service.stt(services.base.STTInput(audio_path=tts_data.output.audio_path))
+    if isinstance(tts_service, services.base.TTSService):
+        tts_data = tts_service.tts(services.base.TTSInput(text=input_text))
+    else:
+        input_data = services.base.TTSInput(text=input_text)
+        tts_data = services.base.TTSData(
+            info=None,
+            input=input_data,
+            output=services.base.TTSOutput(audio_path=services.base.TTSService.get_file_name(input_data))
+        )
+        if not (cache_dir / tts_data.output.audio_path).exists():
+            manim.console.print(f"Please record the following text manually and save it to {cache_dir / tts_data.output.audio_path}.")
+            manim.console.print(f"[green]{input_text}[/green]")
+            manim.console.print("Rerun `manim` after you're done recording.")
+            exit(1)
+    if isinstance(stt_service, services.base.STTService):
+        stt_data = stt_service.stt(services.base.STTInput(audio_path=tts_data.output.audio_path))
+    else:
+        stt_data = services.base.STTData(
+            info=None,
+            input=services.base.STTInput(audio_path=tts_data.output.audio_path),
+            output=services.base.STTOutput(
+                text=input_text,
+                boundaries=[
+                    services.base.Boundary(
+                        text=input_text,
+                        start=0.0,
+                        end=MP3(cache_dir / tts_data.output.audio_path).info.length,
+                        text_offset=0
+                    )
+                ]
+            )
+        )
     bookmark_times = get_bookmark_times(text, tts_data, stt_data)
 
     data = SpeechData(
         text=text,
         tts_data=tts_data,
         stt_data=stt_data,
         duration=MP3(cache_dir / tts_data.output.audio_path).info.length,
```

### Comparing `manim_speech-0.1.0/src/manim_speech/translation.py` & `manim_speech-0.2.0/src/manim_speech/translation.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,32 +2,42 @@
 
 from . import services
 
 import subprocess
 import pathlib
 
 import polib
+import manim
 
 
 def init_translation_env(file: pathlib.Path | str, domain: str) -> None:
     if not pathlib.Path("locales").exists():
         pathlib.Path("locales").mkdir()
     result = subprocess.run(["xgettext", "-d", domain, "-o", str(pathlib.Path("locales") / f"{domain}.pot"), str(file)])
     if result.returncode != 0:
         raise RuntimeError(f"xgettext failed with return code {result.returncode}")
 
 
-def translate_po_file(domain: str, src_lang: str, target_lang: str, *, service: services.base.TranslationService) -> None:
+def translate_po_file(domain: str, src_lang: str, target_lang: str, *, service: services.base.TranslationService | None = None) -> None:
     src_path = pathlib.Path("locales") / f"{domain}.pot"
     target_path = pathlib.Path("locales") / target_lang / "LC_MESSAGES" / f"{domain}"
     if not target_path.parent.exists():
         target_path.parent.mkdir(parents=True)
+    manim.logger.info(f"Translating to {target_lang}...")
     if not target_path.with_suffix(".po").exists():
         pofile = polib.pofile(str(src_path))
         pofile.metadata["Content-Type"] = "text/plain; charset=UTF-8"
-        for entry in pofile.untranslated_entries():
-            translation = service.translate(services.base.TranslationInput(text=entry.msgid, source_language=src_lang, target_language=target_lang)).output.translated_text
-            entry.msgstr = translation
+        if isinstance(service, services.base.TranslationService):
+            manim.logger.info(f"Using {service.service_name} translation service.")
+            for entry in pofile.untranslated_entries():
+                translation = service.translate(services.base.TranslationInput(text=entry.msgid, source_language=src_lang, target_language=target_lang)).output.translated_text
+                entry.msgstr = translation
+        else:
+            manim.logger.info("No translation service specified.")
         pofile.save(str(target_path.with_suffix(".po")))
+        if not isinstance(service, services.base.TranslationService):
+            manim.console.print(f"An empty translation file has been created at {target_path.with_suffix(".po")}. Please fill it in and then rerun `manim`.")
+            exit(1)
     else:
+        manim.logger.info(f"Translation file for {target_lang} found.")
         pofile = polib.pofile(str(target_path.with_suffix(".po")))
     pofile.save_as_mofile(str(target_path.with_suffix(".mo")))
```

### Comparing `manim_speech-0.1.0/src/manim_speech.egg-info/PKG-INFO` & `manim_speech-0.2.0/src/manim_speech.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manim_speech
-Version: 0.1.0
+Version: 0.2.0
 Summary: Manim plugin for adding speech to videos.
 Author-email: Celeste Ma <mtcelestema@proton.me>
 License: MIT License
         
         Copyright (c) 2024 Celeste Ma
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,20 +22,21 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/MtCelesteMa/manim-speech
+Project-URL: Repository, https://github.com/MtCelesteMa/manim-speech
 Project-URL: Bug Tracker, https://github.com/MtCelesteMa/manim-speech/issues
 Keywords: manim,speech,voiceover,tts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: manim
 Requires-Dist: pydantic
 Requires-Dist: mutagen
@@ -66,61 +67,69 @@
 pip install "manim_speech[*optional_dependency_sets*]"
 ```
 
 Where `*optional_dependency_sets*` is a list of optional dependency sets for Manim Speech.
 
 ## Features
 
-* Adding AI-generated voiceovers to Manim animations.
-* Translating text between languages.
+* Integrate voiceovers into Manim animations.
+
+    * Utilize bookmarks to pause for key moments in the voiceover (identical to Manim Voiceover functionality).
+
+* Easily translate text within Manim animations to various languages with minimal code.
+
+* Leverage AI-driven services for text-to-speech, speech-to-text, and translation.
 
 ### Services
 
 | Service Name | Optional Dependency Set | Is Local | Text-To-Speech | Speech-To-Text | Translation |
 |--------------|-------------------------|----------|----------------|----------------|-------------|
-| OpenAI       | `openai`                | No       | Yes            | Yes            | No          |
+| OpenAI       | `openai`                | No       | Yes            | Yes            | Yes         |
 | ElevenLabs   | `elevenlabs`            | No       | Yes            | No             | No          |
 | Whisper      | `whisper`               | Yes      | No             | Yes            | No          |
 | AssemblyAI   | `assemblyai`            | No       | No             | Yes            | No          |
 | DeepL        | `deepl`                 | No       | No             | No             | Yes         |
 
-**Note:** Translating to Traditional Chinese (`zh_tw`) using the DeepL service requires the `chinese` optional dependency set to be installed.
+#### Notes on Chinese Translations
+
+**OpenAI Translator:** Please specify Traditional (`zh_tw`) or Simplified (`zh_cn`) when using the OpenAI translator. Only specifying `zh` has no guarantee on the script used, although tests have indicated that GPT-4o strongly prefers Simplified Chinese in such cases.
+
+**DeepL Translator:** The DeepL translator does not natively support translating to Traditional Chinese, so translating to Traditional Chinese requires the `chinese` optional dependency set to be installed. Only specifying `zh` has the same effect as specifying `zh_cn`.
 
 ## Usage Examples
 
 Creating a basic scene with a voiceover with Manim Speech:
 ```python
 import manim
 import manim_speech
 from manim_speech.services import openai as openai_service
 
 class MeaningOfLife(manim_speech.VoiceoverScene):
     def construct(self) -> None:
-        self.set_tts_service(openai_service.OpenAITTSService())
-        self.set_stt_service(openai_service.OpenAISTTService())
+        self.set_tts_service(openai_service.OpenAITTSService()) # Remove this line if you want to manually record voiceovers.
+        self.set_stt_service(openai_service.OpenAISTTService()) # Only required if you use bookmarks.
 
         with self.voiceover("What is the meaning of life?") as speech_data:
             txt = manim.Text("The meaning of life is 42.")
             self.play(manim.Write(txt), run_time=speech_data.duration)
             self.wait_for_voiceover()
             self.play(manim.FadeOut(txt))
 ```
 
 The same scene, but translated into Traditional Chinese:
 ```python
 import manim
 import manim_speech
 from manim_speech.services import openai as openai_service
-from manim_speech.services import deepl as deepl_service
 
 class MeaningOfLife(manim_speech.VoiceoverScene, manim_speech.TranslationScene):
     def construct(self) -> None:
-        self.set_tts_service(openai_service.OpenAITTSService())
-        self.set_stt_service(openai_service.OpenAISTTService())
-        self.set_translation_service(deepl_service.DeepLTranslationService())
+        self.set_tts_service(openai_service.OpenAITTSService()) # Remove this line if you want to manually record voiceovers.
+        self.set_stt_service(openai_service.OpenAISTTService()) # Only required if you use bookmarks.
+        self.set_translation_service(openai_service.OpenAITranslationService()) # Remove this line if you want to manually translate text.
 
         self.translate(__file__, "meaning_of_life", "en", "zh_tw")
         _ = self._
 
         with self.voiceover(_("What is the meaning of life?")) as speech_data:
             txt = manim.Text(_("The meaning of life is 42."))
             self.play(manim.Write(txt), run_time=speech_data.duration)
```

### Comparing `manim_speech-0.1.0/src/manim_speech.egg-info/SOURCES.txt` & `manim_speech-0.2.0/src/manim_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

