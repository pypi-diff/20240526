# Comparing `tmp/pymkv2-2.0.2.tar.gz` & `tmp/pymkv2-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymkv2-2.0.2.tar", max compression
+gzip compressed data, was "pymkv2-2.0.3.tar", max compression
```

## Comparing `pymkv2-2.0.2.tar` & `pymkv2-2.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-05-12 01:21:08.052855 pymkv2-2.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2543 2024-05-12 01:21:08.052855 pymkv2-2.0.2/README.md
--rw-r--r--   0        0        0      521 2024-05-12 01:21:08.052855 pymkv2-2.0.2/pymkv/BCP47.py
--rw-r--r--   0        0        0      550 2024-05-12 01:21:08.052855 pymkv2-2.0.2/pymkv/ISO639_2.py
--rw-r--r--   0        0        0     2904 2024-05-12 01:21:08.052855 pymkv2-2.0.2/pymkv/MKVAttachment.py
--rw-r--r--   0        0        0    39513 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/MKVFile.py
--rw-r--r--   0        0        0    14332 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/MKVTrack.py
--rw-r--r--   0        0        0     8592 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/Timestamp.py
--rw-r--r--   0        0        0     1685 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/TypeTrack.py
--rw-r--r--   0        0        0     3653 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/Verifications.py
--rw-r--r--   0        0        0      560 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pymkv/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-12 01:21:08.056855 pymkv2-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     3670 1970-01-01 00:00:00.000000 pymkv2-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-26 21:51:08.140397 pymkv2-2.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2397 2024-05-26 21:51:08.140397 pymkv2-2.0.3/README.md
+-rw-r--r--   0        0        0      479 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/BCP47.py
+-rw-r--r--   0        0        0      480 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/ISO639_2.py
+-rw-r--r--   0        0        0     3692 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/MKVAttachment.py
+-rw-r--r--   0        0        0    41345 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/MKVFile.py
+-rw-r--r--   0        0        0    15711 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/MKVTrack.py
+-rw-r--r--   0        0        0    11593 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/Timestamp.py
+-rw-r--r--   0        0        0     1824 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/TypeTrack.py
+-rw-r--r--   0        0        0     5728 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/Verifications.py
+-rw-r--r--   0        0        0      784 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pymkv/utils.py
+-rw-r--r--   0        0        0     3239 2024-05-26 21:51:08.140397 pymkv2-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 pymkv2-2.0.3/PKG-INFO
```

### Comparing `pymkv2-2.0.2/LICENSE.txt` & `pymkv2-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymkv2-2.0.2/README.md` & `pymkv2-2.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 scriptable and easier to use. Please open new issues for any bugs you find, support is greatly appreciated!
 
 ## Installation
 mkvmerge must be installed on your computer, it is needed to process files when creating MKV objects. It is also
 recommended to add it to your $PATH variable but a different path can be manually specified. mkvmerge can be found
 and downloaded from [here](https://mkvtoolnix.download/downloads.html) or from most package managers.
 
+To install pymkv from PyPI, use the following command:
+
+    $ pip install pymkv2
+
 You can also clone the repo and run the following command in the project root to install the source code as editable:
 
     $ pip install -e .
 
 ## Documentation
 The documentation for pymkv can be found [here](https://gitbib.github.io/pymkv2/) or in the project's docstrings.
 
 ### Tests
-~~After completing documentation for the existing features, unit tests need to be written to "lock in" the existing
-functionality. Generating mkvmerge commands can be complex and it is easy to subtly modify an existing feature when
-adding a new one. Unit tests will ensure that features remain the same and help prevent bugs in the future.~~
+Added the first tests for the project. Still a lot to do, but it’s a start. Currently, 49% is covered by tests.
 
 ### Cleanup
 ~~The existing code base could use some tidying, better commenting, debugging, and a general styling overhaul. Setting up
 [pre-commit](https://pre-commit.com/) and the [Black code formatter](https://github.com/psf/black) will help keep the
 code base more readable and maintainable.~~
 
 ### Features
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymkv2-2.0.2/pymkv/MKVAttachment.py` & `pymkv2-2.0.3/pymkv/MKVAttachment.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+from __future__ import annotations
+
+from mimetypes import guess_type
+from pathlib import Path
+
 """:class:`~pymkv.MKVAttachment` classes are used to represent attachment files within an MKV or to be used in an
 MKV.
 
 Examples
 --------
 Below are some basic examples of how the :class:`~pymkv.MKVAttachment` objects can be used.
 
@@ -19,17 +24,14 @@
 
 Now, the MKV can be muxed with both attachments.
 
 >>> mkv.add_attachment(attachment)
 >>> mkv.mux('path/to/output.mkv')
 """
 
-from os.path import expanduser, isfile
-from mimetypes import guess_type
-
 
 class MKVAttachment:
     """A class that represents an MKV attachment for an :class:`~pymkv.MKVFile` object.
 
     Parameters
     ----------
     file_path : str
@@ -51,37 +53,68 @@
     description : str
         The description that will be given to the attachment when muxed into a file.
     attach_once : bool
         Determines if the attachment should be added to all split files or only the first. Default is False,
         which will attach to all files.
     """
 
-    def __init__(self, file_path, name=None, description=None, attach_once=False):
+    def __init__(
+        self,
+        file_path: str,
+        name: str | None = None,
+        description: str | None = None,
+        attach_once: bool | None = False,
+    ) -> None:
         self.mime_type = None
         self._file_path = None
         self.file_path = file_path
         self.name = name
         self.description = description
         self.attach_once = attach_once
 
-    def __repr__(self):
+    def __repr__(self) -> str:
+        """
+        Return a string representation of the object.
+
+        Parameters:
+            self (object): The object for which the string representation is generated.
+
+        Returns:
+            str: The string representation of the object. It is the representation of the object's __dict__ attribute.
+        """
         return repr(self.__dict__)
 
     @property
-    def file_path(self):
+    def file_path(self) -> str:
         """str: The path to the attachment file.
 
         Raises
         ------
         FileNotFoundError
             Raised if `file_path` does not exist.
         """
         return self._file_path
 
     @file_path.setter
-    def file_path(self, file_path):
-        file_path = expanduser(file_path)
-        if not isfile(file_path):
-            raise FileNotFoundError(f'"{file_path}" does not exist')
+    def file_path(self, file_path: str) -> None:
+        """
+        Parameters
+        ----------
+        file_path : str
+            The file path to be set.
+
+        Raises
+        ------
+        FileNotFoundError
+            If the specified file does not exist.
+
+        Returns
+        -------
+        None
+        """
+        file_path = Path(file_path).expanduser()
+        if not file_path.is_file():
+            msg = f'"{file_path}" does not exist'
+            raise FileNotFoundError(msg)
         self.mime_type = guess_type(file_path)[0]
         self.name = None
-        self._file_path = file_path
+        self._file_path = str(file_path)
```

### Comparing `pymkv2-2.0.2/pymkv/MKVFile.py` & `pymkv2-2.0.3/pymkv/MKVFile.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,26 +31,30 @@
 
 >>> mkv1 = MKVFile('/path/to/file1.mkv')
 >>> mkv2 = MKVFile('/path/to/file2.mkv')
 >>> mkv1.add_file(mkv2)
 >>> mkv1.mux('/path/to/output.mkv')
 """
 
+from __future__ import annotations
+
 import json
 import logging
-from os.path import expanduser, isfile
+import os
 import subprocess as sp
+from pathlib import Path
 
 import bitmath
 
-from pymkv.MKVTrack import MKVTrack
+from pymkv.ISO639_2 import is_iso639_2
 from pymkv.MKVAttachment import MKVAttachment
+from pymkv.MKVTrack import MKVTrack
 from pymkv.Timestamp import Timestamp
-from pymkv.ISO639_2 import is_iso639_2
-from pymkv.Verifications import verify_matroska, verify_mkvmerge
+from pymkv.utils import prepare_mkvtoolnix_path
+from pymkv.Verifications import checking_file_path, verify_mkvmerge
 
 
 class MKVFile:
     """A class that represents an MKV file.
 
     The :class:`~pymkv.MKVFile` class can either import a pre-existing MKV file or create a new one. After an
     :class:`~pymkv.MKVFile` object has been instantiated, :class:`~pymkv.MKVTrack` objects or other
@@ -79,84 +83,112 @@
 
     Raises
     ------
     FileNotFoundError
         Raised if the path to mkvmerge could not be verified.
     """
 
-    def __init__(self, file_path=None, title=None, mkvmerge_path='mkvmerge'):
-        self.mkvmerge_path = mkvmerge_path
+    def __init__(  # noqa: C901, PLR0912
+        self,
+        file_path: str | os.PathLike | None = None,
+        title: str | None = None,
+        mkvmerge_path: str | list | os.PathLike | None = "mkvmerge",
+    ) -> None:
+        self.mkvmerge_path: list[str] = prepare_mkvtoolnix_path(mkvmerge_path)
         self.title = title
         self._chapters_file = None
         self._chapter_language = None
         self._global_tags_file = None
         self._link_to_previous_file = None
         self._link_to_next_file = None
         self.tracks: list[MKVTrack] = []
         self.attachments = []
         self._number_file = 0
 
         if not verify_mkvmerge(mkvmerge_path=mkvmerge_path):
-            raise FileNotFoundError('mkvmerge is not at the specified path, add it there or change'
-                                    'the mkvmerge_path property')
+            msg = "mkvmerge is not at the specified path, add it there or changed mkvmerge_path property"
+            raise FileNotFoundError(msg)
 
         if file_path is not None:
             # add file title
-            file_path = expanduser(file_path)
-            info_json = json.loads(sp.check_output([self.mkvmerge_path, '-J', file_path]).decode())
-            if self.title is None and 'title' in info_json['container']['properties']:
-                self.title = info_json['container']['properties']['title']
+            file_path = checking_file_path(file_path)
+            try:
+                info_json = json.loads(sp.check_output([*self.mkvmerge_path, "-J", file_path]).decode())  # noqa: S603
+            except sp.CalledProcessError as e:
+                error_output = e.output.decode()
+                raise sp.CalledProcessError(e.returncode, e.cmd, output=error_output) from e
+            if self.title is None and "title" in info_json["container"]["properties"]:
+                self.title = info_json["container"]["properties"]["title"]
 
             # add tracks with info
-            for track in info_json['tracks']:
-                new_track = MKVTrack(file_path, track_id=track['id'], mkvmerge_path=self.mkvmerge_path)
-                if 'track_name' in track['properties']:
-                    new_track.track_name = track['properties']['track_name']
-                if 'language' in track['properties']:
-                    new_track.language = track['properties']['language']
-                if 'language_ietf' in track['properties']:
-                    new_track.language_ietf = track['properties']['language_ietf']
-                if 'default_track' in track['properties']:
-                    new_track.default_track = track['properties']['default_track']
-                if 'forced_track' in track['properties']:
-                    new_track.forced_track = track['properties']['forced_track']
-                if 'flag_commentary' in track['properties']:
-                    new_track.flag_commentary = track['properties']['flag_commentary']
-                if 'flag_hearing_impaired' in track['properties']:
-                    new_track.flag_hearing_impaired = track['properties']['flag_hearing_impaired']
-                if 'flag_visual_impaired' in track['properties']:
-                    new_track.flag_visual_impaired = track['properties']['flag_visual_impaired']
-                if 'flag_original' in track['properties']:
-                    new_track.flag_original = track['properties']['flag_original']
+            for track in info_json["tracks"]:
+                new_track = MKVTrack(file_path, track_id=track["id"], mkvmerge_path=self.mkvmerge_path)
+                if "track_name" in track["properties"]:
+                    new_track.track_name = track["properties"]["track_name"]
+                if "language" in track["properties"]:
+                    new_track.language = track["properties"]["language"]
+                if "language_ietf" in track["properties"]:
+                    new_track.language_ietf = track["properties"]["language_ietf"]
+                if "default_track" in track["properties"]:
+                    new_track.default_track = track["properties"]["default_track"]
+                if "forced_track" in track["properties"]:
+                    new_track.forced_track = track["properties"]["forced_track"]
+                if "flag_commentary" in track["properties"]:
+                    new_track.flag_commentary = track["properties"]["flag_commentary"]
+                if "flag_hearing_impaired" in track["properties"]:
+                    new_track.flag_hearing_impaired = track["properties"]["flag_hearing_impaired"]
+                if "flag_visual_impaired" in track["properties"]:
+                    new_track.flag_visual_impaired = track["properties"]["flag_visual_impaired"]
+                if "flag_original" in track["properties"]:
+                    new_track.flag_original = track["properties"]["flag_original"]
                 self.add_track(new_track, new_file=False)
 
         # split options
         self._split_options = []
 
-    def __repr__(self):
+    def __repr__(self) -> str:
+        """
+        Return a string representation of the object.
+
+        :returns: A string representation of the object.
+        :rtype: str
+        """
         return repr(self.__dict__)
 
     @property
-    def chapter_language(self):
+    def chapter_language(self) -> str:
         """str: The language code of the chapters in the :class:`~pymkv.MKVFile` object.
 
         Raises
         ------
         ValueError
             Raised if not a valid ISO 639-2 language code.
         """
         return self._chapter_language
 
     @chapter_language.setter
-    def chapter_language(self, language):
+    def chapter_language(self, language: str) -> None:
+        """
+        Parameters
+        ----------
+        language : str
+            The language code for the chapter.
+            Must be an ISO639-2 language code.
+
+        Raises
+        ------
+        ValueError
+            If the provided language code is not a valid ISO639-2 language code.
+        """
         if language is not None and not is_iso639_2(language):
-            raise ValueError('not an ISO639-2 language code')
+            msg = "not an ISO639-2 language code"
+            raise ValueError(msg)
         self._chapter_language = language
 
-    def command(self, output_path, subprocess=False):
+    def command(self, output_path: str, subprocess: bool = False) -> str | list:  # noqa: C901, PLR0912, PLR0915
         """Generates an mkvmerge command based on the configured :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         output_path : str
             The path to be used as the output file in the mkvmerge command.
         subprocess : bool
@@ -164,190 +196,193 @@
 
         Returns
         -------
         str, list of str
             The full command to mux the :class:`~pymkv.MKVFile` as a string containing spaces. Will be returned as a
             list of strings with no spaces if `subprocess` is True.
         """
-
-        output_path = expanduser(output_path)
-        command = [self.mkvmerge_path, '-o', output_path]
+        output_path = str(Path(output_path).expanduser())
+        command = [*self.mkvmerge_path, "-o", output_path]
         if self.title is not None:
-            command.extend(['--title', self.title])
+            command.extend(["--title", self.title])
         track_order = []
         for track in self.tracks:
             # for track_order
-            track_order.append(f'{track.file_id}:{track.track_id}')
+            track_order.append(f"{track.file_id}:{track.track_id}")
             # flags
             if track.track_name is not None:
-                command.extend(['--track-name', f'{str(track.track_id)}:{track.track_name}'])
+                command.extend(["--track-name", f"{track.track_id!s}:{track.track_name}"])
             if track.language_ietf is not None:
-                command.extend(['--language', f'{str(track.track_id)}:{track.language_ietf}'])
+                command.extend(["--language", f"{track.track_id!s}:{track.language_ietf}"])
             elif track.language is not None:
-                command.extend(['--language', f'{str(track.track_id)}:{track.language}'])
+                command.extend(["--language", f"{track.track_id!s}:{track.language}"])
             if track.sync is not None:
-                command.extend(['--sync', f'{str(track.track_id)}:{track.sync}'])
+                command.extend(["--sync", f"{track.track_id!s}:{track.sync}"])
             if track.tags is not None:
-                command.extend(['--tags', f'{str(track.track_id)}:{track.tags}'])
+                command.extend(["--tags", f"{track.track_id!s}:{track.tags}"])
             if track.default_track:
-                command.extend(['--default-track', f'{str(track.track_id)}:1'])
+                command.extend(["--default-track", f"{track.track_id!s}:1"])
             else:
-                command.extend(['--default-track', f'{str(track.track_id)}:0'])
+                command.extend(["--default-track", f"{track.track_id!s}:0"])
             if track.forced_track:
-                command.extend(['--forced-track', f'{str(track.track_id)}:1'])
+                command.extend(["--forced-track", f"{track.track_id!s}:1"])
             else:
-                command.extend(['--forced-track', f'{str(track.track_id)}:0'])
+                command.extend(["--forced-track", f"{track.track_id!s}:0"])
             if track.flag_hearing_impaired:
-                command.extend(['--hearing-impaired-flag', f'{str(track.track_id)}:1'])
+                command.extend(["--hearing-impaired-flag", f"{track.track_id!s}:1"])
             else:
-                command.extend(['--hearing-impaired-flag', f'{str(track.track_id)}:0'])
+                command.extend(["--hearing-impaired-flag", f"{track.track_id!s}:0"])
             if track.flag_visual_impaired:
-                command.extend(['--visual-impaired-flag', f'{str(track.track_id)}:1'])
+                command.extend(["--visual-impaired-flag", f"{track.track_id!s}:1"])
             else:
-                command.extend(['--visual-impaired-flag', f'{str(track.track_id)}:0'])
+                command.extend(["--visual-impaired-flag", f"{track.track_id!s}:0"])
             if track.flag_original:
-                command.extend(['--original-flag', f'{str(track.track_id)}:1'])
+                command.extend(["--original-flag", f"{track.track_id!s}:1"])
             else:
-                command.extend(['--original-flag', f'{str(track.track_id)}:0'])
+                command.extend(["--original-flag", f"{track.track_id!s}:0"])
             if track.flag_commentary:
-                command.extend(['--commentary-flag', f'{str(track.track_id)}:1'])
+                command.extend(["--commentary-flag", f"{track.track_id!s}:1"])
             else:
-                command.extend(['--commentary-flag', f'{str(track.track_id)}:0'])
+                command.extend(["--commentary-flag", f"{track.track_id!s}:0"])
 
             # remove extra tracks
-            if track.track_type == 'audio':
-                command.append('-D')
-                command.extend(['-a', str(track.track_id), '-S'])
-            elif track.track_type == 'subtitles':
-                command.extend(('-D', '-A', '-s', str(track.track_id)))
-            elif track.track_type == 'video':
-                command.extend(['-d', str(track.track_id), '-A', '-S'])
+            if track.track_type == "audio":
+                command.append("-D")
+                command.extend(["-a", str(track.track_id), "-S"])
+            elif track.track_type == "subtitles":
+                command.extend(("-D", "-A", "-s", str(track.track_id)))
+            elif track.track_type == "video":
+                command.extend(["-d", str(track.track_id), "-A", "-S"])
             else:
-                command.extend(('-D', '-A', '-S'))
+                command.extend(("-D", "-A", "-S"))
             # exclusions
             if track.no_chapters:
-                command.append('--no-chapters')
+                command.append("--no-chapters")
             if track.no_global_tags:
-                command.append('--no-global-tags')
+                command.append("--no-global-tags")
             if track.no_track_tags:
-                command.append('--no-track-tags')
+                command.append("--no-track-tags")
             if track.no_attachments:
-                command.append('--no-attachments')
+                command.append("--no-attachments")
 
-            # add path
             command.append(track.file_path)
 
         # add attachments
         for attachment in self.attachments:
             # info
             if attachment.name is not None:
-                command.extend(['--attachment-name', attachment.name])
+                command.extend(["--attachment-name", attachment.name])
             if attachment.description is not None:
-                command.extend(['--attachment-description', attachment.description])
+                command.extend(["--attachment-description", attachment.description])
             if attachment.mime_type is not None:
-                command.extend(['--attachment-mime-type', attachment.mime_type])
+                command.extend(["--attachment-mime-type", attachment.mime_type])
 
             # add path
             if not attachment.attach_once:
-                command.extend(['--attach-file', attachment.file_path])
+                command.extend(["--attach-file", attachment.file_path])
             else:
-                command.extend(['--attach-file-once', attachment.file_path])
+                command.extend(["--attach-file-once", attachment.file_path])
 
         # chapters
         if self._chapter_language is not None:
-            command.extend(['--chapter-language', self._chapter_language])
+            command.extend(["--chapter-language", self._chapter_language])
         if self._chapters_file is not None:
-            command.extend(['--chapters', self._chapters_file])
+            command.extend(["--chapters", self._chapters_file])
 
         # global tags
         if self._global_tags_file is not None:
-            command.extend(['--global-tags', self._global_tags_file])
+            command.extend(["--global-tags", self._global_tags_file])
 
         # linking
         if self._link_to_previous_file is not None:
-            command.extend(['--link-to-previous', f'={self._link_to_previous_file}'])
+            command.extend(["--link-to-previous", f"={self._link_to_previous_file}"])
         if self._link_to_next_file is not None:
-            command.extend(['--link-to-next', f'={self._link_to_next_file}'])
+            command.extend(["--link-to-next", f"={self._link_to_next_file}"])
 
         # tracks order
         if track_order:
-            command.extend(['--track-order', ','.join(track_order)])
+            command.extend(["--track-order", ",".join(track_order)])
 
         # split options
         command.extend(self._split_options)
 
         return command if subprocess else " ".join(command)
 
-    def mux(self, output_path, silent=False):
+    def mux(self, output_path: str | os.PathLike, silent: bool = False) -> int:
         """Mixes the specified :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         output_path : str
             The path to be used as the output file in the mkvmerge command.
         silent : bool, optional
             By default the mkvmerge output will be shown unless silent is True.
+        Returns
+        -------
+        int of Any
+            return code
 
         Raises
         ------
         ValueError
             Raised if the external mkvmerge command fails with a non-zero exit status.
             This includes scenarios such as invalid command arguments, errors in
             processing the :class:`~pymkv.MKVFile`, or issues with output file writing. The error
             message provides details about the failure based on the output of the command.
         """
-        output_path = expanduser(output_path)
+        output_path = str(Path(output_path).expanduser())
         args = self.command(output_path, subprocess=True)
 
         stdout = sp.DEVNULL if silent else None
         stderr = sp.PIPE
 
-        proc = sp.Popen(args, stdout=stdout, stderr=stderr)
+        proc = sp.Popen(args, stdout=stdout, stderr=stderr)  # noqa: S603
         _, err = proc.communicate()
 
         if proc.returncode:
             error_message = f"Command failed with non-zero exit status {proc.returncode}"
             if err:
                 error_details = err.decode()
                 error_message += f"\nError Output:\n{error_details}"
                 logging.error(error_details)
             logging.error("Non-zero exit status when running %s (%s)", args, proc.returncode)
             raise ValueError(error_message)
 
         return proc.returncode
 
-    def add_file(self, file):
+    def add_file(self, file: MKVFile | str | os.PathLike) -> None:
         """Add an MKV file into the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
-        file : str, :class:`~pymkv.MKVFile`
+        file : str, :class:`~pymkv.MKVFile`, os.PathLike
             The file to be combined with the :class:`~pymkv.MKVFile` object.
 
         Raises
         ------
         TypeError
             Raised if if `file` is not a string-like path to an MKV file or an :class:`~pymkv.MKVFile` object.
         """
-        if isinstance(file, str):
+        if isinstance(file, (str, os.PathLike)):
             self._number_file += 1
             new_tracks = MKVFile(file).tracks
             for track in new_tracks:
                 track.file_id = self._number_file
             self.tracks = self.tracks + new_tracks
         elif isinstance(file, MKVFile):
             self._number_file += 1
             for track in file.tracks:
                 track.file_id = self._number_file
             self.tracks = self.tracks + file.tracks
         else:
-            raise TypeError('track is not str or MKVFile')
+            msg = "track is not str or MKVFile"
+            raise TypeError(msg)
         self.order_tracks_by_file_id()
 
-    def add_track(self, track, new_file: bool = True):
+    def add_track(self, track: str | MKVTrack, new_file: bool = True) -> None:
         """Add a track to the :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         track : str, :class:`~pymkv.MKVTrack`
             The track to be added to the :class:`~pymkv.MKVFile` object.
         new_file : bool, optional
@@ -361,44 +396,47 @@
         """
         if isinstance(track, str):
             new_track = MKVTrack(track, mkvmerge_path=self.mkvmerge_path)
             self._extracted_from_add_track(new_track, new_file)
         elif isinstance(track, MKVTrack):
             self._extracted_from_add_track(track, new_file)
         else:
-            raise TypeError('track is not str or MKVTrack')
+            msg = "track is not str or MKVTrack"
+            raise TypeError(msg)
         self.order_tracks_by_file_id()
 
-    def _extracted_from_add_track(self, track: MKVTrack, new_file: bool = False):
+    def _extracted_from_add_track(self, track: MKVTrack, new_file: bool = False) -> None:
         if new_file:
             self._number_file += 1
         track.file_id = self._number_file
         self.tracks.append(track)
 
-    def add_attachment(self, attachment):
+    def add_attachment(self, attachment: str | MKVAttachment) -> None:
         """Add an attachment to the :class:`~pymkv.MKVFile`.
 
         Parameters
         ----------
         attachment : str, :class:`~pymkv.MKVAttachment`
             The attachment to be added to the :class:`~pymkv.MKVFile` object.
 
         Raises
         ------
         TypeError
-            Raised if if `attachment` is not a string-like path to an attachment file or an :class:`~pymkv.MKVAttachment`.
+            Raised if if `attachment` is not a string-like path to an attachment file
+            or an :class:`~pymkv.MKVAttachment`.
         """
         if isinstance(attachment, str):
             self.attachments.append(MKVAttachment(attachment))
         elif isinstance(attachment, MKVAttachment):
             self.attachments.append(attachment)
         else:
-            raise TypeError('attachment is not str of MKVAttachment')
+            msg = "Attachment is not str of MKVAttachment"
+            raise TypeError(msg)
 
-    def get_track(self, track_num=None):
+    def get_track(self, track_num: int | None = None) -> MKVTrack:
         """Get a :class:`~pymkv.MKVTrack` from the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int, optional
             Index of track to retrieve. Will return list of :class:`~pymkv.MKVTrack` objects if argument is not
             provided.
@@ -407,156 +445,158 @@
         -------
         :class:`~pymkv.MKVTrack`, list of :class:`~pymkv.MKVTrack`
             A list of all :class:`~pymkv.MKVTrack` objects in an :class:`~pymkv.MKVFile`. Returns a specific
             :class:`~pymkv.MKVTrack` if `track_num` is specified.
         """
         return self.tracks if track_num is None else self.tracks[track_num]
 
-    def move_track_front(self, track_num):
+    def move_track_front(self, track_num: int) -> None:
         """Set a track as the first in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move to the front.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if 0 <= track_num < len(self.tracks):
-            self.tracks.insert(0, self.tracks.pop(track_num))
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 <= track_num < len(self.tracks):
+            msg = "track index out of range"
+            raise IndexError(msg)
+        self.tracks.insert(0, self.tracks.pop(track_num))
+        self.order_tracks_by_file_id()
 
-    def move_track_end(self, track_num):
+    def move_track_end(self, track_num: int) -> None:
         """Set as track as the last in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move to the back.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if 0 <= track_num < len(self.tracks):
-            self.tracks.append(self.tracks.pop(track_num))
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 <= track_num < len(self.tracks):
+            msg = "track index out of range"
+            raise IndexError(msg)
+        self.tracks.append(self.tracks.pop(track_num))
+        self.order_tracks_by_file_id()
 
-    def move_track_forward(self, track_num):
+    def move_track_forward(self, track_num: int) -> None:
         """Move a track forward in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move forward.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if 0 <= track_num < len(self.tracks) - 1:
-            self.tracks[track_num], self.tracks[track_num + 1] = self.tracks[track_num + 1], self.tracks[track_num]
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 <= track_num < len(self.tracks) - 1:
+            msg = "Track index out of range"
+            raise IndexError(msg)
+        self.tracks[track_num], self.tracks[track_num + 1] = self.tracks[track_num + 1], self.tracks[track_num]
+        self.order_tracks_by_file_id()
 
-    def move_track_backward(self, track_num):
+    def move_track_backward(self, track_num: int) -> None:
         """Move a track backward in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to move backward.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if 0 < track_num < len(self.tracks):
-            self.tracks[track_num], self.tracks[track_num - 1] = self.tracks[track_num - 1], self.tracks[track_num]
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 < track_num < len(self.tracks):
+            msg = "Track index out of range"
+            raise IndexError(msg)
+        self.tracks[track_num], self.tracks[track_num - 1] = self.tracks[track_num - 1], self.tracks[track_num]
+        self.order_tracks_by_file_id()
 
-    def swap_tracks(self, track_num_1, track_num_2):
+    def swap_tracks(self, track_num_1: int, track_num_2: int) -> None:
         """Swap the position of two tracks in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num_1 : int
             The track number of one track to swap.
         track_num_2 : int
             The track number of the other track to swap
 
         Raises
         ------
         IndexError
             Raised if `track_num_1` or `track_num_2` are out of range of the track list.
         """
-        if 0 <= track_num_1 < len(self.tracks) and 0 <= track_num_2 < len(self.tracks):
-            self.tracks[track_num_1], self.tracks[track_num_2] = self.tracks[track_num_2], self.tracks[track_num_1]
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 <= track_num_1 < len(self.tracks) or not 0 <= track_num_2 < len(
+            self.tracks,
+        ):
+            msg = "Track index out of range"
+            raise IndexError(msg)
+        self.tracks[track_num_1], self.tracks[track_num_2] = self.tracks[track_num_2], self.tracks[track_num_1]
+        self.order_tracks_by_file_id()
 
-    def replace_track(self, track_num, track):
+    def replace_track(self, track_num: int, track: MKVTrack) -> None:
         """Replace a track with another track in the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to replace.
         track : :class:`~pymkv.MKVTrack`
             The :class:`~pymkv.MKVTrack` to be replaced into the file.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if 0 <= track_num < len(self.tracks):
-            self.tracks[track_num] = track
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 <= track_num < len(self.tracks):
+            msg = "track index out of range"
+            raise IndexError(msg)
+        self.tracks[track_num] = track
+        self.order_tracks_by_file_id()
 
-    def remove_track(self, track_num):
+    def remove_track(self, track_num: int) -> None:
         """Remove a track from the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         track_num : int
             The track number of the track to remove.
 
         Raises
         ------
         IndexError
             Raised if `track_num` is is out of range of the track list.
         """
-        if 0 <= track_num < len(self.tracks):
-            del self.tracks[track_num]
-            self.order_tracks_by_file_id()
-        else:
-            raise IndexError('track index out of range')
+        if not 0 <= track_num < len(self.tracks):
+            msg = "track index out of range"
+            raise IndexError(msg)
+        del self.tracks[track_num]
+        self.order_tracks_by_file_id()
 
-    def split_none(self):
+    def split_none(self) -> None:
         """Remove all splitting options."""
         self._split_options = []
 
-    def split_size(self, size, link=False):
+    def split_size(self, size: bitmath.Bitmath | int, link: bool | None = False) -> None:
         """Split the output file into parts by size.
 
         Parameters
         ----------
         size : :obj:`bitmath`, int
             The size of each split file. Takes either a :obj:`bitmath` size object or an integer representing the
             number of bytes.
@@ -564,38 +604,39 @@
             Determines if the split files should be linked together after splitting.
 
         Raises
         ------
         TypeError
             Raised if if `size` is not a bitmath object or an integer.
         """
-        if getattr(size, '__module__', None) == bitmath.__name__:
+        if getattr(size, "__module__", None) == bitmath.__name__:
             size = size.bytes
         elif not isinstance(size, int):
-            raise TypeError('size is not a bitmath object or integer')
-        self._split_options = ['--split', f'size:{size}']
+            msg = "size is not a bitmath object or integer"
+            raise TypeError(msg)
+        self._split_options = ["--split", f"size:{size}"]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def split_duration(self, duration, link=False):
+    def split_duration(self, duration: str | int, link: bool | None = False) -> None:
         """Split the output file into parts by duration.
 
         Parameters
         ----------
         duration : str, int
             The duration of each split file. Takes either a str formatted to HH:MM:SS.nnnnnnnnn or an integer
             representing the number of seconds. The duration string requires formatting of at least M:S.
         link : bool, optional
             Determines if the split files should be linked together after splitting.
         """
-        self._split_options = ['--split', f'duration:{str(Timestamp(duration))}']
+        self._split_options = ["--split", f"duration:{Timestamp(duration)!s}"]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def split_timestamps(self, *timestamps, link=False):
+    def split_timestamps(self, *timestamps: str | int | list | tuple, link: bool | None = False) -> None:
         """Split the output file into parts by timestamps.
 
         Parameters
         ----------
         *timestamps : str, int, list, tuple
             The timestamps to split the file by. Can be passed as any combination of strs and ints, inside or outside
             an :obj:`Iterable` object. Any lists will be flattened. Timestamps must be ints, representing seconds,
@@ -607,30 +648,33 @@
         ------
         ValueError
             Raised if invalid or improperly formatted timestamps are passed in for `*timestamps`.
         """
         # check if in timestamps form
         ts_flat = MKVFile.flatten(timestamps)
         if len(ts_flat) == 0:
-            raise ValueError(f'"{timestamps}" are not properly formatted timestamps')
+            msg = f'"{timestamps}" are not properly formatted timestamps'
+            raise ValueError(msg)
         if None in ts_flat:
-            raise ValueError(f'"{timestamps}" are not properly formatted timestamps')
-        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:]):
+            msg = f'"{timestamps}" are not properly formatted timestamps'
+            raise ValueError(msg)
+        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:], strict=False):
             if Timestamp(ts_1) >= Timestamp(ts_2):
-                raise ValueError(f'"{timestamps}" are not properly formatted timestamps')
+                msg = f'"{timestamps}" are not properly formatted timestamps'
+                raise ValueError(msg)
 
         # build ts_string from timestamps
-        ts_string = 'timestamps:'
+        ts_string = "timestamps:"
         for ts in ts_flat:
-            ts_string += f'{str(Timestamp(ts))},'
-        self._split_options = ['--split', ts_string[:-1]]
+            ts_string += f"{Timestamp(ts)!s},"
+        self._split_options = ["--split", ts_string[:-1]]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def split_frames(self, *frames, link=False):
+    def split_frames(self, *frames: int | list | tuple, link: bool | None = False) -> None:
         """Split the output file into parts by frames.
 
         Parameters
         ----------
         *frames : int, list, tuple
             The frames to split the file by. Can be passed as any combination of ints, inside or outside an
             :obj:`Iterable` object. Any lists will be flattened. Frames must be ints.
@@ -641,33 +685,36 @@
         ------
         TypeError
             Raised if non-int frames are passed in for `*frames` or within the `*frames` iterable.
         ValueError
             Raised if improperly formatted frames are passed in for `*frames`.
         """
         # check if in frames form
-        f_flat = MKVFile.flatten(frames)
-        if len(f_flat) == 0:
-            raise ValueError(f'"{frames}" are not properly formatted frames')
-        for f in f_flat:
+        frames_flat = MKVFile.flatten(frames)
+        if len(frames_flat) == 0:
+            msg = f'"{frames}" are not properly formatted frames'
+            raise ValueError(msg)
+        for f in frames_flat:
             if not isinstance(f, int):
-                raise TypeError(f'frame "{f}" not an int')
-        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:]):
+                msg = f'frame "{f}" not an int'
+                raise TypeError(msg)
+        for f_1, f_2 in zip(frames_flat[:-1], frames_flat[1:], strict=False):
             if f_1 >= f_2:
-                raise ValueError(f'"{frames}" are not properly formatted frames')
+                msg = f'"{frames}" are not properly formatted frames'
+                raise ValueError(msg)
 
         # build f_string from frames
-        f_string = 'frames:'
-        for f in f_flat:
-            f_string += f'{str(f)},'
-        self._split_options = ['--split', f_string[:-1]]
+        f_string = "frames:"
+        for f in frames_flat:
+            f_string += f"{f!s},"
+        self._split_options = ["--split", f_string[:-1]]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def split_timestamp_parts(self, timestamp_parts, link=False):
+    def split_timestamp_parts(self, timestamp_parts: list | tuple, link: bool | None = False) -> None:  # noqa: C901
         """Split the output in parts by time parts.
 
         Parameters
         ----------
         timestamp_parts : list, tuple
             An Iterable of timestamp sets. Each timestamp set should be an Iterable of an even number of timestamps
             or any number of timestamp pairs. The very first and last timestamps are permitted to be None. Timestamp
@@ -680,41 +727,46 @@
         TypeError
             Raised if any of the timestamp sets are not a list or tuple.
         ValueError
             Raised if `timestamp_parts` contains improperly formatted parts.
         """
         ts_flat = MKVFile.flatten(timestamp_parts)
         if len(timestamp_parts) == 0:
-            raise ValueError(f'"{timestamp_parts}" are not properly formatted parts')
+            msg = f'"{timestamp_parts}" are not properly formatted parts'
+            raise ValueError(msg)
 
         if None in ts_flat[1:-1]:
-            raise ValueError(f'"{timestamp_parts}" are not properly formatted parts')
+            msg = f'"{timestamp_parts}" are not properly formatted parts'
+            raise ValueError(msg)
 
-        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:]):
+        for ts_1, ts_2 in zip(ts_flat[:-1], ts_flat[1:], strict=False):
             if None not in (ts_1, ts_2) and Timestamp(ts_1) >= Timestamp(ts_2):
-                raise ValueError(f'"{timestamp_parts}" are not properly formatted parts')
+                msg = f'"{timestamp_parts}" are not properly formatted parts'
+                raise ValueError(msg)
 
-        ts_string = 'parts:'
+        ts_string = "parts:"
         for ts_set in timestamp_parts:
-            ts_set = MKVFile.flatten(ts_set)
+            ts_set = MKVFile.flatten(ts_set)  # noqa: PLW2901
             if not isinstance(ts_set, (list, tuple)):
-                raise TypeError('set is not of type list or tuple')
-            if len(ts_set) < 2 or len(ts_set) % 2 != 0:
-                raise ValueError(f'"{ts_set}" is not a properly formatted set')
+                msg = "set is not of type list or tuple"
+                raise TypeError(msg)
+            if len(ts_set) < 2 or len(ts_set) % 2 != 0:  # noqa: PLR2004
+                msg = f'"{ts_set}" is not a properly formatted set'
+                raise ValueError(msg)
             for index, ts in enumerate(ts_set):
                 if index % 2 == 0 and index > 0:
-                    ts_string += '+'
+                    ts_string += "+"
                 if ts is not None:
                     ts_string += str(Timestamp(ts))
-                ts_string += '-' if index % 2 == 0 else ','
-        self._split_options = ['--split', ts_string[:-1]]
+                ts_string += "-" if index % 2 == 0 else ","
+        self._split_options = ["--split", ts_string[:-1]]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def split_parts_frames(self, frame_parts, link=False):
+    def split_parts_frames(self, frame_parts: list | tuple, link: bool | None = False) -> None:  # noqa: C901
         """Split the output in parts by frames.
 
         Parameters
         ----------
         frame_parts : list, tuple
             An Iterable of frame sets. Each frame set should be an :obj:`Iterable` object of an even number of frames
             or any
@@ -728,40 +780,46 @@
         TypeError
             Raised if any of the frame sets are not a list or tuple.
         ValueError
             Raised if `frame_parts` contains improperly formatted parts.
         """
         f_flat = MKVFile.flatten(frame_parts)
         if len(frame_parts) == 0:
-            raise ValueError(f'"{frame_parts}" are not properly formatted parts')
+            msg = f'"{frame_parts}" are not properly formatted parts'
+            raise ValueError(msg)
         if None in f_flat[1:-1]:
-            raise ValueError(f'"{frame_parts}" are not properly formatted parts')
-        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:]):
+            msg = f'"{frame_parts}" are not properly formatted parts'
+            raise ValueError(msg)
+        for f_1, f_2 in zip(f_flat[:-1], f_flat[1:], strict=False):
             if None not in (f_1, f_2) and f_1 >= f_2:
-                raise ValueError(f'"{frame_parts}" are not properly formatted parts')
-        f_string = 'parts:'
+                msg = f'"{frame_parts}" are not properly formatted parts'
+                raise ValueError(msg)
+        f_string = "parts:"
         for f_set in frame_parts:
-            f_set = MKVFile.flatten(f_set)
+            f_set = MKVFile.flatten(f_set)  # noqa: PLW2901
             if not isinstance(f_set, (list, tuple)):
-                raise TypeError('set is not of type list or tuple')
-            if len(f_set) < 2 or len(f_set) % 2 != 0:
-                raise ValueError(f'"{f_set}" is not a properly formatted set')
+                msg = "set is not of type list or tuple"
+                raise TypeError(msg)
+            if len(f_set) < 2 or len(f_set) % 2 != 0:  # noqa: PLR2004
+                msg = f'"{f_set}" is not a properly formatted set'
+                raise ValueError(msg)
             for index, f in enumerate(f_set):
                 if not isinstance(f, int) and f is not None:
-                    raise TypeError(f'frame "{f}" not an int')
+                    msg = f'frame "{f}" not an int'
+                    raise TypeError(msg)
                 if index % 2 == 0 and index > 0:
-                    f_string += '+'
+                    f_string += "+"
                 if f is not None:
                     f_string += str(f)
-                f_string += '-' if index % 2 == 0 else ','
-        self._split_options = ['--split', f_string[:-1]]
+                f_string += "-" if index % 2 == 0 else ","
+        self._split_options = ["--split", f_string[:-1]]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def split_chapters(self, *chapters, link=False):
+    def split_chapters(self, *chapters: int | list | tuple, link: bool | None = False) -> None:
         """Split the output file into parts by chapters.
 
         Parameters
         ----------
         *chapters : int, list, tuple
            The chapters to split the file by. Can be passed as any combination of ints, inside or outside an
            :obj:`Iterable` object. Any lists will be flattened. Chapters must be ints.
@@ -770,84 +828,77 @@
 
         Raises
         ------
         TypeError
             Raised if any chapters in `*chapters` are not of type int.
         ValueError
             Raised if `*chapters` contains improperly formatted chapters.
-       """
+        """
         c_flat = MKVFile.flatten(chapters)
         if not chapters:
-            self._split_options = ['--split', 'chapters:all']
+            self._split_options = ["--split", "chapters:all"]
             return
         for c in c_flat:
             if not isinstance(c, int):
-                raise TypeError(f'chapter "{c}" not an int')
+                msg = f'chapter "{c}" not an int'
+                raise TypeError(msg)
             if c < 1:
-                raise ValueError(f'"{chapters}" are not properly formatted chapters')
-        for c_1, c_2 in zip(c_flat[:-1], c_flat[1:]):
+                msg = f'"{chapters}" are not properly formatted chapters'
+                raise ValueError(msg)
+        for c_1, c_2 in zip(c_flat[:-1], c_flat[1:], strict=False):
             if c_1 >= c_2:
-                raise ValueError(f'"{chapters}" are not properly formatted chapters')
-        c_string = 'chapters:'
+                msg = f'"{chapters}" are not properly formatted chapters'
+                raise ValueError(msg)
+        c_string = "chapters:"
         for c in c_flat:
-            c_string += f'{str(c)},'
-        self._split_options = ['--split', c_string[:-1]]
+            c_string += f"{c!s},"
+        self._split_options = ["--split", c_string[:-1]]
         if link:
-            self._split_options += '--link'
+            self._split_options += "--link"
 
-    def link_to_previous(self, file_path):
+    def link_to_previous(self, file_path: str) -> None:
         """Link the output file as the predecessor of the `file_path` file.
 
         Parameters
         ----------
         file_path : str
             Path of the file to be linked to.
 
         Raises
         ------
         TypeError
             Raised if `file_path` is not of type str.
         ValueError
             Raised if file at `file_path` cannot be verified as an MKV.
         """
-        if not isinstance(str, file_path):
-            raise TypeError(f'"{file_path}" is not of type str')
-        file_path = expanduser(file_path)
-        if not verify_matroska(file_path):
-            raise ValueError(f'"{file_path}" is not a matroska file')
-        self._link_to_previous_file = file_path
+        self._link_to_previous_file = checking_file_path(file_path)
 
-    def link_to_next(self, file_path):
+    def link_to_next(self, file_path: str) -> None:
         """Link the output file as the successor of the `file_path` file.
 
         Parameters
         ----------
         file_path : str
             Path of the file to be linked to.
 
         Raises
         ------
         TypeError
             Raised if `file_path` is not of type str.
         ValueError
             Raised if file at `file_path` cannot be verified as an MKV.
         """
-        if not isinstance(file_path, str):
-            raise TypeError(f'"{file_path}" is not of type str')
-        file_path = expanduser(file_path)
-        if not verify_matroska(file_path):
-            raise ValueError(f'"{file_path}" is not a matroska file')
-        self._link_to_next_file = file_path
+        self._link_to_next_file = checking_file_path(file_path)
 
-    def link_to_none(self):
+    def link_to_none(self) -> None:
         """Remove all linking to previous and next options."""
         self._link_to_previous_file = None
         self._link_to_next_file = None
 
-    def chapters(self, file_path, language=None):
+    def chapters(self, file_path: str, language: str | None = None) -> None:
         """Add a chapters file to the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         file_path : str
             The chapters file to be added to the :class:`~pymkv.MKVFile` object.
         language : str, optional
@@ -856,45 +907,35 @@
         Raises
         ------
         FileNotFoundError
             Raised if the file at `file_path` does not exist.
         TypeError
             Raised if `file_path` is not of type str.
         """
-        if not isinstance(file_path, str):
-            raise TypeError(f'"{file_path}" is not of type str')
-        file_path = expanduser(file_path)
-        if not isfile(file_path):
-            raise FileNotFoundError(f'"{file_path}" does not exist')
-        self._chapters_file = file_path
+        self._chapters_file = checking_file_path(file_path)
         self.chapter_language = language
 
-    def global_tags(self, file_path):
+    def global_tags(self, file_path: str) -> None:
         """Add global tags to the :class:`~pymkv.MKVFile` object.
 
         Parameters
         ----------
         file_path : str
             The tags file to be added to the :class:`~pymkv.MKVFile` object.
 
         Raises
         ------
         FileNotFoundError
             Raised if the file at `file_path` does not exist.
         TypeError
             Raised if `file_path` is not of type str.
         """
-        if not isinstance(file_path, str):
-            raise TypeError(f'"{file_path}" is not of type str')
-        file_path = expanduser(file_path)
-        if not isfile(file_path):
-            raise FileNotFoundError(f'"{file_path}" does not exist')
-        self._global_tags_file = file_path
+        self._global_tags_file = checking_file_path(file_path)
 
-    def track_tags(self, *track_ids, exclusive=False):
+    def track_tags(self, *track_ids: int | list | tuple, exclusive: bool | None = False) -> None:
         """Include or exclude tags from specific tracks.
 
         Parameters
         ----------
         *track_ids : int, list, tuple
             Track ids to have tags included or excluded from.
         exclusive : bool, optional
@@ -908,45 +949,48 @@
         TypeError
             Raised if an ids from `*track_ids` are not of type int.
         ValueError
             Raised if `*track_ids` are improperly formatted.
         """
         ids_flat = MKVFile.flatten(track_ids)
         if not track_ids:
-            raise ValueError(f'"{track_ids}" are not properly formatted track ids')
+            msg = f'"{track_ids}" are not properly formatted track ids'
+            raise ValueError(msg)
         for tid in ids_flat:
             if not isinstance(tid, int):
-                raise TypeError(f'track id "{tid}" not an int')
+                msg = f'track id "{tid}" not an int'
+                raise TypeError(msg)
             if tid < 0 or tid >= len(self.tracks):
-                raise IndexError('track id out of range')
+                msg = "track id out of range"
+                raise IndexError(msg)
         for tid in ids_flat if exclusive else list(set(range(len(self.tracks))) - set(ids_flat)):
             self.tracks[tid].no_track_tags = True
 
-    def no_chapters(self):
+    def no_chapters(self) -> None:
         """Ignore the existing chapters of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_chapters = True
 
-    def no_global_tags(self):
+    def no_global_tags(self) -> None:
         """Ignore the existing global tags of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_global_tags = True
 
-    def no_track_tags(self):
+    def no_track_tags(self) -> None:
         """Ignore the existing track tags of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_track_tags = True
 
-    def no_attachments(self):
+    def no_attachments(self) -> None:
         """Ignore the existing attachments of the :class:`~pymkv.MKVFile` object."""
         for track in self.tracks:
             track.no_attachments = True
 
     @staticmethod
-    def flatten(item):
+    def flatten(item: list | tuple) -> list:
         """Flatten a list or a tuple.
 
         Takes a list or a tuple that contains other lists or tuples and flattens into a non-nested list.
 
         Examples
         --------
         >>> tup = ((1, 2), (3, (4, 5)))
@@ -962,19 +1006,19 @@
         -------
         list
             A flattened version of `item`.
         """
         if not isinstance(item, (list, tuple)):
             return [item]
         flat_list = []
-        for item in item:
+        for item in item:  # noqa: B020
             flat_list.extend(MKVFile.flatten(item))
         return flat_list
 
-    def order_tracks_by_file_id(self):
+    def order_tracks_by_file_id(self) -> None:
         """
         Orders tracks based on their file ID. Tracks from the same file will have the same file ID.
 
         This method first generates a list of unique file paths from the existing tracks.
         Then, it assigns each track a file ID, which is the index of its file path in the unique list.
         As a result, tracks from the same file will have the same file ID.
         """
```

### Comparing `pymkv2-2.0.2/pymkv/MKVTrack.py` & `pymkv2-2.0.3/pymkv/MKVTrack.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,34 +31,34 @@
 >>> file = MKVFile()
 >>> file.add_track(track1)
 >>> file.add_track(track2)
 >>> file.add_track(track3)
 >>> file.mux('path/to/output.mkv')
 """
 
+from __future__ import annotations
+
 import json
-import os.path
-from os import devnull
-from os.path import expanduser, isfile
+import os
 import subprocess as sp
+from os import devnull
 from pathlib import Path
 
+from pymkv.BCP47 import is_bcp47
+from pymkv.ISO639_2 import is_iso639_2
 from pymkv.TypeTrack import get_track_extension
+from pymkv.utils import prepare_mkvtoolnix_path
 from pymkv.Verifications import verify_supported
-from pymkv.ISO639_2 import is_iso639_2
-from pymkv.BCP47 import is_bcp47
 
 
 class MKVTrack:
     """A class that represents a track for an :class:`~pymkv.MKVFile` object.
-
     :class:`~pymkv.MKVTrack` objects are video, audio, or subtitles. Tracks can be standalone files or a single track
     within an MKV file, both can be handled by pymkv. An :class:`~pymkv.MKVTrack` object can be added to an
     :class:`~pymkv.MKVFile` and will be included when the MKV is muxed.
-
     Parameters
     ----------
     file_path : str
         Path to the track file. This can also be an MKV where the `track_id` is the track represented in the MKV.
     track_id : int, optional
         The id of the track to be used from the file. `track_id` only needs to be set when importing a track from
         an MKV. In this case, you can specify `track_id` to indicate which track from the MKV should be used. If not
@@ -70,23 +70,28 @@
         The language of the track. It must be an ISO639-2 language code.
     language_ietf : str, optional
         The language of the track. It must be a BCP47 language code. Has priority over 'language'.
     default_track : bool, optional
         Determines if the track should be the default track of its type when muxed into an MKV file.
     forced_track : bool, optional
         Determines if the track should be a forced track when muxed into an MKV file.
-    mkvmerge_path : str, optional
+    mkvmerge_path : str, list, os.PathLike, optional
         The path where pymkv looks for the mkvmerge executable. pymkv relies on the mkvmerge executable to parse
         files. By default, it is assumed mkvmerge is in your shell's $PATH variable. If it is not, you need to set
         *mkvmerge_path* to the executable location.
-
+    mkvextract_path : str, list, os.PathLike, optional
+        The path where pymkv looks for the mkvextract executable. pymkv relies on the mkvextract executable to extract
+        files. By default, it is assumed mkvextract is in your shell's $PATH variable. If it is not, you need to set
+        *mkvextract_path* to the executable location.
     Attributes
     ----------
-    mkvmerge_path : str
+    mkvmerge_path : list
         The path of the mkvmerge executable.
+    mkvextract_path : list
+        The path of the mkvextract executable.
     track_name : str
         The name that will be given to the track when muxed into a file.
     default_track : bool
         Determines if the track should be the default track of its type when muxed into an MKV file.
     forced_track : bool
         Determines if the track should be a forced track when muxed into an MKV file.
     no_chapters : bool
@@ -103,23 +108,37 @@
         effect on standalone track files, only tracks that are already part of an MKV file.
     no_attachments : bool
         If attachments exist in the track file, don't include them when this :class:`~pymkv.MKVTrack` object is a track
         in an :class:`~pymkv.MKVFile` mux operation. This option has no effect on standalone track files, only tracks
         that are already part of an MKV file.
     """
 
-    def __init__(self, file_path, track_id=0, track_name=None, language=None, language_ietf=None, default_track=False,
-                 forced_track=False, flag_commentary=False, flag_hearing_impaired=False, flag_visual_impaired=False,
-                 flag_original=False, mkvmerge_path='mkvmerge', mkvextract_path='mkvextract', sync=None):
+    def __init__(  # noqa: PLR0913
+        self,
+        file_path: str,
+        track_id: int | None = 0,
+        track_name: str | None = None,
+        language: str | None = None,
+        language_ietf: str | None = None,
+        default_track: bool | None = False,
+        forced_track: bool | None = False,
+        flag_commentary: bool | None = False,
+        flag_hearing_impaired: bool | None = False,
+        flag_visual_impaired: bool | None = False,
+        flag_original: bool | None = False,
+        mkvmerge_path: str | list | os.PathLike | None = "mkvmerge",
+        mkvextract_path: str | list | os.PathLike | None = "mkvextract",
+        sync: int | None = None,
+    ) -> None:
         # track info
         self._track_codec = None
         self._track_type = None
 
         # base
-        self.mkvmerge_path = mkvmerge_path
+        self.mkvmerge_path = prepare_mkvtoolnix_path(mkvmerge_path)
         self._file_path = None
         self.file_path = file_path
         self._track_id = None
         self.track_id = track_id
         self._file_id = 0
         self._pts = 0
 
@@ -142,235 +161,247 @@
         # exclusions
         self.no_chapters = False
         self.no_global_tags = False
         self.no_track_tags = False
         self.no_attachments = False
 
         # mkvextract
-        self.mkvextract_path = mkvextract_path
+        self.mkvextract_path = prepare_mkvtoolnix_path(mkvextract_path)
         self.extension = get_track_extension(self)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return repr(self.__dict__)
 
     @property
-    def file_path(self):
+    def file_path(self) -> str:
         """str: The path to the track or MKV file containing the desired track.
 
         Setting this property will verify the passed in file is supported by mkvmerge and set the track_id to 0. It
         is recommended to recreate MKVTracks instead of setting their file path after instantiation.
 
         Raises
         ------
         ValueError
             Raised if `file_path` is not a supported file type.
         """
         return self._file_path
 
     @file_path.setter
-    def file_path(self, file_path):
-        file_path = expanduser(file_path)
+    def file_path(self, file_path: str) -> None:
+        file_path = str(Path(file_path).expanduser())
         if not verify_supported(file_path, mkvmerge_path=self.mkvmerge_path):
-            raise ValueError('"{}" is not a supported file')
+            msg = '"{}" is not a supported file'
+            raise ValueError(msg)
         self._file_path = file_path
         self.track_id = 0
 
     @property
-    def file_id(self):
+    def file_id(self) -> int:
         """int: The ID of the file the track belongs to.
 
         The file ID represents which file the current track is associated with. This is particularly useful
         when handling multiple files.
 
         Raises
         ------
         IndexError
             Raised if the passed in index is out of range of the file's tracks.
         """
         return self._file_id
 
     @file_id.setter
-    def file_id(self, file_id: int):
+    def file_id(self, file_id: int) -> None:
         if isinstance(file_id, int):
             self._file_id = file_id
         else:
-            raise ValueError('file_id must be an integer')
+            msg = "file_id must be an integer"
+            raise ValueError(msg)  # noqa: TRY004
 
     @property
-    def track_id(self):
+    def track_id(self) -> int:
         """int: The ID of the track within the file.
 
         Setting *track_id* will check that the ID passed in exists in the file. It will then look at the new track
         and set the codec and track type. Should be left at 0 unless extracting a specific track from an MKV.
 
         Raises
         ------
         IndexError
             Raised if the passed in index is out of range of the file's tracks.
         """
         return self._track_id
 
     @track_id.setter
-    def track_id(self, track_id):
-        info_json = json.loads(sp.check_output([self.mkvmerge_path, '-J', self.file_path]).decode())
-        if not 0 <= track_id < len(info_json['tracks']):
-            raise IndexError('track index out of range')
+    def track_id(self, track_id: int) -> None:
+        info_json = json.loads(sp.check_output([*self.mkvmerge_path, "-J", self.file_path]).decode())  # noqa: S603
+        if not 0 <= track_id < len(info_json["tracks"]):
+            msg = "track index out of range"
+            raise IndexError(msg)
         self._track_id = track_id
         try:
-            self._pts = info_json['tracks'][track_id]["start_pts"]
+            self._pts = info_json["tracks"][track_id]["start_pts"]
         except KeyError:
             self._pts = 0
-        self._track_codec = info_json['tracks'][track_id]['codec']
-        self._track_type = info_json['tracks'][track_id]['type']
+        self._track_codec = info_json["tracks"][track_id]["codec"]
+        self._track_type = info_json["tracks"][track_id]["type"]
 
     @property
-    def language(self):
+    def language(self) -> str:
         """str: The language of the track.
 
         Setting this property will verify that the passed in language is an ISO-639 language code and use it as the
         language for the track.
 
         Raises
         ------
         ValueError
             Raised if the passed in language is not an ISO 639-2 language code.
         """
         return self._language
 
     @language.setter
-    def language(self, language):
+    def language(self, language: str) -> None:
         """Sets the language of the MKVTrack.
 
         Args:
             language: The language to be set for the MKVTrack.
 
         Returns:
             None
 
         Raises:
             ValueError: If the provided language is not a valid ISO639-2 language code.
         """
         if language is None or is_iso639_2(language):
             self._language = language
         else:
-            raise ValueError('not an ISO639-2 language code')
+            msg = "not an ISO639-2 language code"
+            raise ValueError(msg)
 
     @property
-    def pts(self):
+    def pts(self) -> int:
         """Returns the value of the `pts` property.
         The Presentation Timestamp (PTS) in multimedia files indicates the exact time when a frame or audio sample
         should be presented to the user, ensuring accurate synchronization between audio and video streams.
 
         Args:
             self: The instance of the class.
 
         Returns:
             The value of the `pts` property.
         """
         return self._pts
 
     @property
-    def sync(self):
+    def sync(self) -> int:
         """int: track delay.
 
         Setting this property allows you to wiggle the track negatively/positively.
         """
         return self._sync
 
     @sync.setter
-    def sync(self, sync):
+    def sync(self, sync: int) -> None:
         """Sets the value of the `sync` property.
 
         Args:
             sync: The value to be set for the `sync` property.
 
         Returns:
             None
 
         Raises:
             None
         """
         self._sync = sync
 
     @property
-    def language_ietf(self):
+    def language_ietf(self) -> str:
         """str: The language of the track with BCP47 format.
         Setting this property will verify that the passed in language is a BCP47 language code and use it as the
         language for the track.
         Raises
         ------
         ValueError
             Raised if the passed in language is not a BCP47 language code.
         """
         return self._language_ietf
 
     @language_ietf.setter
-    def language_ietf(self, language_ietf):
+    def language_ietf(self, language_ietf: str) -> None:
         if language_ietf is None or is_bcp47(language_ietf):
             self._language_ietf = language_ietf
         else:
-            raise ValueError('not a BCP47 language code')
+            msg = "not a BCP47 language code"
+            raise ValueError(msg)
 
     @property
-    def tags(self):
+    def tags(self) -> str:
         """str: The tags file to include with the track.
 
         Setting this property will check that the file path passed in exists and set it as the tags file.
 
         Raises
         ------
         FileNotFoundError
             Raised if the passed in file does not exist or is not a file.
         TypeError
             Raises if the passed in file is not of type str.
         """
         return self._tags
 
     @tags.setter
-    def tags(self, file_path):
+    def tags(self, file_path: str) -> None:
         if not isinstance(file_path, str):
-            raise TypeError(f'"{file_path}" is not of type str')
-        file_path = expanduser(file_path)
-        if not isfile(file_path):
-            raise FileNotFoundError(f'"{file_path}" does not exist')
-        self._tags = file_path
+            msg = f'"{file_path}" is not of type str'
+            raise TypeError(msg)
+        file_path = Path(file_path).expanduser()
+        if not file_path.is_file():
+            msg = f'"{file_path}" does not exist'
+            raise FileNotFoundError(msg)
+        self._tags = str(file_path)
 
     @property
-    def track_codec(self):
+    def track_codec(self) -> str:
         """str: The codec of the track such as h264 or AAC."""
         return self._track_codec
 
     @property
-    def track_type(self):
+    def track_type(self) -> str:
         """str: The type of track such as video or audio."""
         return self._track_type
 
-    def extract(self, output_path: str = None, silent: bool = False) -> str:
-        """Extract the track as a file.
+    def extract(self, output_path: str | os.PathLike | None = None, silent: bool | None = False) -> str:
+        """
+        Extract the track as a file.
 
         Parameters
         ----------
-        output_path : str
+        output_path : str, os.PathLike, optional
             The path to be used as the output file in the mkvextract command.
         silent : bool, optional
             By default the mkvmerge output will be shown unless silent is True.
+
+        Returns
+        -------
+        str
+            The path of the extracted file.
         """
         extract_info_file = f"_[{self.track_id}]"
         if self.language:
             extract_info_file += f"_{self.language}"
         if self.extension:
             extract_info_file += f".{self.extension}"
         if (not self.language and not self.expansion) and self.track_name:
             extract_info_file += f"_{self.track_name}"
         if output_path is None:
             output_path = f"{self.file_path}{extract_info_file}"
         else:
             file = Path(self.file_path)
-            output_path = os.path.join(output_path, f"{file.name}{extract_info_file}")
-        output_path = expanduser(output_path)
-        command = [self.mkvextract_path, 'tracks', f"{self.file_path}", f"{self.track_id}:{output_path}"]
+            output_path = Path(output_path, f"{file.name}{extract_info_file}")
+        output_path = str(Path(output_path).expanduser())
+        command = [*self.mkvextract_path, "tracks", f"{self.file_path}", f"{self.track_id}:{output_path}"]
         if silent:
-            sp.run(command, stdout=open(devnull, 'wb'), check=True)
+            sp.run(command, stdout=open(devnull, "wb"), check=True)  # noqa: S603, PTH123, SIM115
         else:
-            print('Running with command:\n"' + " ".join(command) + '"')
-            sp.run(command, check=True, capture_output=True)
+            sp.run(command, check=True, capture_output=True)  # noqa: S603
         return output_path
```

### Comparing `pymkv2-2.0.2/pymkv/Timestamp.py` & `pymkv2-2.0.3/pymkv/Timestamp.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-# sheldon woodward
-# 3/16/18
-
-"""Timestamp Class"""
+from __future__ import annotations
 
 from re import match
 
 
 class Timestamp:
-    def __init__(self, timestamp=None, hh=None, mm=None, ss=None, nn=None, form='MM:SS'):
+    def __init__(  # noqa: PLR0913
+        self,
+        timestamp: str | int | Timestamp = None,
+        hh: int | None = None,
+        mm: int | None = None,
+        ss: int | None = None,
+        nn: int | None = None,
+        form: str | None = "MM:SS",
+    ) -> None:
         """A class that represents a timestamp used in MKVFiles.
 
         The Timestamp class represents a timestamp used in mkvmerge. These are commonly used for splitting MKVFiles.
         Specific time values can overridden in the timestamp using 'hh', 'mm', 'ss', and 'nn'. Any override value
         that is greater than its maximum (ex. 61 minutes) will be set to 0.
 
         timestamp (str, int, Timestamp):
@@ -21,15 +26,15 @@
             Hours in the timestamp. This will override the hours in the given timestamp.
         mm (int):
             Minutes in the timestamp. This will override the minutes in the given timestamp.
         ss (int):
             Seconds in the timestamp. This will override the seconds in the given timestamp.
         nn (int):
             Nanoseconds in the timestamp. This will override the nanoseconds in the given timestamp.
-        form (int):
+        form (str):
             A str for the form of the returned timestamp. 'MM' and 'SS' must be included where 'HH' and 'NN' are
             optional but will be included if 'hh' and 'nn' are not zero.
         """
         self._hh = hh
         self._mm = mm
         self._ss = ss
         self._nn = nn
@@ -43,207 +48,268 @@
             self.extract(timestamp)
         else:
             self._hh = 0 if self._hh is None else self._hh
             self._mm = 0 if self._mm is None else self._mm
             self._ss = 0 if self._ss is None else self._ss
             self._nn = 0 if self._nn is None else self._nn
 
-    def __eq__(self, other):
+    def __eq__(self, other: Timestamp) -> bool:
+        """
+        Compares the Timestamp object with another Timestamp object for equality.
+
+        Args:
+            other: The Timestamp object to compare with.
+
+        Returns:
+            bool: True if the Timestamp objects are equal, False otherwise.
+        """
         return self.hh == other.hh and self.mm == other.mm and self.ss == other.ss and self.nn == other.nn
 
-    def __ne__(self, other):
+    def __ne__(self, other: Timestamp) -> bool:
+        """
+        Compares the Timestamp object with another Timestamp object for inequality.
+
+        Args:
+            other: The Timestamp object to compare with.
+
+        Returns:
+            bool: True if the Timestamp objects are not equal, False otherwise.
+        """
         return self.hh != other.hh or self.mm != other.mm or self.ss != other.ss or self.nn != other.nn
 
-    def __lt__(self, other):
+    def __lt__(self, other: Timestamp) -> bool:
+        """
+        Compares the Timestamp object with another Timestamp object to determine if it is less than.
+
+        Args:
+            other: The Timestamp object to compare with.
+
+        Returns:
+            bool: True if the Timestamp object is less than the other Timestamp object, False otherwise.
+        """
         if self.hh != other.hh:
             return self.hh < other.hh
-        elif self.mm != other.mm:
+        elif self.mm != other.mm:  # noqa: RET505
             return self.mm < other.mm
         elif self.ss != other.ss:
             return self.ss < other.ss
         elif self.nn != other.nn:
             return self.nn < other.nn
         return False
 
-    def __le__(self, other):
+    def __le__(self, other: Timestamp) -> bool:
+        """
+        Compares the Timestamp object with another Timestamp object to determine if it is less than or equal to.
+
+        Args:
+            other: The Timestamp object to compare with.
+
+        Returns:
+            bool: True if the Timestamp object is less than or equal to the other Timestamp object, False otherwise.
+        """
         if self.hh != other.hh:
             return self.hh <= other.hh
-        elif self.mm != other.mm:
+        elif self.mm != other.mm:  # noqa: RET505
             return self.mm <= other.mm
         elif self.ss != other.ss:
             return self.ss <= other.ss
         elif self.nn != other.nn:
             return self.nn <= other.nn
         return True
 
-    def __gt__(self, other):
+    def __gt__(self, other: Timestamp) -> bool:
+        """
+        Compares the Timestamp object with another Timestamp object to determine if it is greater than.
+
+        Args:
+            other: The Timestamp object to compare with.
+
+        Returns:
+            bool: True if the Timestamp object is greater than the other Timestamp object, False otherwise.
+        """
         if self.hh != other.hh:
             return self.hh > other.hh
-        elif self.mm != other.mm:
+        elif self.mm != other.mm:  # noqa: RET505
             return self.mm > other.mm
         elif self.ss != other.ss:
             return self.ss > other.ss
         elif self.nn != other.nn:
             return self.nn > other.nn
         return False
 
-    def __ge__(self, other):
+    def __ge__(self, other: Timestamp) -> bool:
+        """
+        Compares the Timestamp object with another Timestamp object to determine if it is greater than or equal to.
+
+        Args:
+            other: The Timestamp object to compare with.
+
+        Returns:
+            bool: True if the Timestamp object is greater than or equal to the other Timestamp object, False otherwise.
+        """
         if self.hh != other.hh:
             return self.hh >= other.hh
-        elif self.mm != other.mm:
+        elif self.mm != other.mm:  # noqa: RET505
             return self.mm >= other.mm
         elif self.ss != other.ss:
             return self.ss >= other.ss
         elif self.nn != other.nn:
             return self.nn >= other.nn
         return True
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.ts
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> int:
+        """
+        Retrieves the element at the specified index from the Timestamp object.
+
+        Args:
+            index: The index of the element to retrieve.
+
+        Returns:
+            int: The element at the specified index.
+        """
         return (self.hh, self.mm, self.ss, self.ss)[index]
 
     @property
-    def ts(self):
+    def ts(self) -> str:
         """Generates the timestamp specified in the object."""
         # parse timestamp format
-        format_groups = match('^(([Hh]{1,2}):)?([Mm]{1,2}):([Ss]{1,2})(\.([Nn]{1,9}))?$', self.form).groups()
+        format_groups = match(r"^(([Hh]{1,2}):)?([Mm]{1,2}):([Ss]{1,2})(\.([Nn]{1,9}))?$", self.form).groups()
         timestamp_format = [format_groups[i] is not None for i in (1, 2, 3, 5)]
 
         # create timestamp string
-        timestamp_string = ''
+        timestamp_string = ""
         if timestamp_format[0] or self._hh:
-            timestamp_string += '{0:0=2d}:'.format(self.hh)
+            timestamp_string += f"{self.hh:0=2d}:"
         if timestamp_format[1] or self._mm:
-            timestamp_string += '{0:0=2d}:'.format(self.mm)
+            timestamp_string += f"{self.mm:0=2d}:"
         if timestamp_format[2] or self._ss:
-            timestamp_string += '{0:0=2d}'.format(self.ss)
+            timestamp_string += f"{self.ss:0=2d}"
         if timestamp_format[3] or self._nn:
-            timestamp_string += '{:.9f}'.format(self.nn / 1000000000).rstrip('0')[1:] if self.nn else '.0'
+            timestamp_string += f"{self.nn / 1000000000:.9f}".rstrip("0")[1:] if self.nn else ".0"
         return timestamp_string
 
     @ts.setter
-    def ts(self, timestamp):
+    def ts(self, timestamp: Timestamp) -> None:
         """Set a new timestamp.
 
         timestamp (str, int):
             A str of a timestamp acceptable to mkvmerge or an int representing seconds. This value will be
             the basis of the timestamp.
         """
         if not isinstance(timestamp, (int, str)):
-            raise TypeError(f'"{type(timestamp)}" is not str or int type')
+            msg = f'"{type(timestamp)}" is not str or int type'
+            raise TypeError(msg)
         self._hh = None
         self._mm = None
         self._ss = None
         self._nn = None
         self.extract(timestamp)
 
     @property
-    def hh(self):
+    def hh(self) -> int:
         return self._hh
 
     @hh.setter
-    def hh(self, value):
+    def hh(self, value: int) -> None:
         self._hh = value
 
     @property
-    def mm(self):
+    def mm(self) -> int:
         return self._mm
 
     @mm.setter
-    def mm(self, value):
-        self._mm = value if value < 60 else 0
+    def mm(self, value: int) -> None:
+        self._mm = value if value < 60 else 0  # noqa: PLR2004
 
     @property
-    def ss(self):
+    def ss(self) -> int:
         return self._ss
 
     @ss.setter
-    def ss(self, value):
-        self._ss = value if value < 60 else 0
+    def ss(self, value: int) -> None:
+        self._ss = value if value < 60 else 0  # noqa: PLR2004
 
     @property
-    def nn(self):
+    def nn(self) -> int:
         return self._nn
 
     @nn.setter
-    def nn(self, value):
-        self._nn = value if value < 1000000000 else 0
+    def nn(self, value: int) -> None:
+        self._nn = value if value < 1000000000 else 0  # noqa: PLR2004
 
     @property
-    def form(self):
+    def form(self) -> str:
         return self._form
 
     @form.setter
-    def form(self, form):
+    def form(self, form: str) -> None:
         self._form = form
 
     @staticmethod
-    def verify(timestamp):
+    def verify(timestamp: str | int) -> bool:
         """Verify a timestamp has the proper form to be used in mkvmerge.
 
         timestamp (str, int):
             The timestamp to be verified.
         """
         if not isinstance(timestamp, str):
-            raise TypeError(f'"{type(timestamp)}" is not str type')
-        elif match('^[0-9]{1,2}(:[0-9]{1,2}){1,2}(\.[0-9]{1,9})?$', timestamp):
+            msg = f'"{type(timestamp)}" is not str type'
+            raise TypeError(msg)
+        elif match(r"^[0-9]{1,2}(:[0-9]{1,2}){1,2}(\.[0-9]{1,9})?$", timestamp):  # noqa: RET506
             return True
         return False
 
-    def extract(self, timestamp):
+    def extract(self, timestamp: str | int) -> None:
         """Extracts time info from a timestamp.
 
         timestamp (str, int):
             A str of a timestamp acceptable to mkvmerge or an int representing seconds. The timing info will be
             extracted from this parameter.
         """
         if not isinstance(timestamp, (str, int)):
-            raise TypeError(f'"{type(timestamp)}" is not str or int type')
-        elif isinstance(timestamp, str) and not Timestamp.verify(timestamp):
-            raise ValueError(f'"{timestamp}" is not a valid timestamp')
+            msg = f'"{type(timestamp)}" is not str or int type'
+            raise TypeError(msg)
+        elif isinstance(timestamp, str) and not Timestamp.verify(timestamp):  # noqa: RET506
+            msg = f'"{timestamp}" is not a valid timestamp'
+            raise ValueError(msg)
         elif isinstance(timestamp, str):
             self.splitting_timestamp(timestamp)
         elif isinstance(timestamp, int):
             self._hh = int(timestamp / 3600)
             self._mm = int(timestamp % 3600 / 60)
             self._ss = int(timestamp % 3600 % 60)
             self._nn = 0
 
-    def splitting_timestamp(self, timestamp):
-        """
-        The `splitting_timestamp` function splits a timestamp into its individual components and assigns them to instance variables.
-
-        Args:
-        self: The instance of the class.
-
-        Returns:
-        None
+    def splitting_timestamp(self, timestamp: str) -> None:
+        """This method splits the given timestamp string into hours, minutes, seconds, and nanoseconds. The timestamp
+        string should be in the format "HH:MM:SS.NNNNNNNNN", where HH represents hours,
+        MM represents minutes, SS represents seconds, and NNNNNNNNN represents nanoseconds.
+
+        Parameters
+        ----------
+        timestamp : str
+            The timestamp string to be split.
 
-        Raises:
+        Returns
+        -------
         None
 
-        Examples:
-        ```
-        timestamp = "12:34:56.789"
-        splitting_timestamp(self, timestamp)
-        print(self.hh)  # Output: 12
-        print(self.mm)  # Output: 34
-        print(self.ss)  # Output: 56
-        print(self.nn)  # Output: 789000000
-            Parameters
-            ----------
-            timestamp
-
-            Returns
-            -------
-        '''
+        Example
+        -------
+        >>> obj.splitting_timestamp("12:34:56.789012345")
+        # Assuming self._hh, self._mm, self._ss, and self._nn are all None initially
+        The hours (self.hh) will be set to 12.
+        The minutes (self.mm) will be set to 34.
+        The seconds (self.ss) will be set to 56.
+        The nanoseconds (self.nn) will be set to 789012345.
         """
-        timestamp_groups = match('^(([0-9]{1,2}):)?([0-9]{1,2}):([0-9]{1,2})(\.([0-9]{1,9}))?$', timestamp).groups()
+        timestamp_groups = match(r"^(([0-9]{1,2}):)?([0-9]{1,2}):([0-9]{1,2})(\.([0-9]{1,9}))?$", timestamp).groups()
 
         timestamp = [timestamp_groups[i] for i in (1, 2, 3, 4)]
         timestamp_clean = []
         for ts in timestamp:
             if ts is None:
                 timestamp_clean.append(0)
             else:
```

### Comparing `pymkv2-2.0.2/pymkv/TypeTrack.py` & `pymkv2-2.0.3/pymkv/TypeTrack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from typing import Optional
+from __future__ import annotations
 
-from pymkv import MKVTrack
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from pymkv import MKVTrack
 
 type_files = {
     "video": {
         "V_MPEG1": "mpg",
         "V_MPEG2": "mpg",
         "V_MPEG4/ISO/AVC": "264",
         "MPEG-4p10": "h264",
         "HEVC": "h265",
         "V_MS/VFW/FOURCC": "avi",
         "V_REAL": "rm",
         "V_THEORA": "ogg",
         "V_VP8": "ivf",
         "V_VP9": "ivf",
+        "AVC/H.264/MPEG-4p10": "mp4",
     },
     "audio": {
         "AAC": "aac",
         "AC3": "ac3",
         "AC-3": "ac3",
         "ALAC": "caf",
         "DTS": "dts",
@@ -30,14 +34,15 @@
         "TRUEHD": "thd",
         "MLP": "mlp",
         "TTA1": "tta",
         "VORBIS": "ogg",
         "WAVPACK4": "wv",
         "V_MS/VFW/FOURCC, WVC1": "wvc",
         "VC-1": "wvc",
+        "Vorbis": "ogg",
     },
     "subtitles": {
         "PGS": "sup",
         "ASS": "ass",
         "SSA": "ssa",
         "UTF8": "srt",
         "SubRip/SRT": "srt",
@@ -45,15 +50,15 @@
         "VOBSUB": "sub",
         "USF": "usf",
         "WEBVTT": "vtt",
     },
 }
 
 
-def get_track_extension(track: MKVTrack) -> Optional[str]:
+def get_track_extension(track: MKVTrack) -> str | None:
     """str: Extension of a track.
 
     Parameters
     ----------
     track : :class:`~pymkv.MKVTrack`
         The :class:`~pymkv.MKVTrack` from which the file extension by track type will be obtained.
 
@@ -62,7 +67,8 @@
     str
         Return the extension of a track. If the track is a video, audio or subtitle track, an extension is returned.
     """
     track_type = track.track_type
     track_codec = track.track_codec
     if track_type in type_files and track_codec in type_files[track_type]:
         return type_files[track_type][track_codec]
+    return None
```

### Comparing `pymkv2-2.0.2/pyproject.toml` & `pymkv2-2.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "pymkv2"
-version = "2.0.2"
+version = "2.0.3"
 description = "A Python wrapper for mkvmerge. It provides support for muxing, splitting, linking, chapters, tags, and attachments through the use of mkvmerge."
 authors = [
     "Sheldon Woodward <me@sheldonw.com>",
-    "GitBib"
+    "GitBib <job@bnff.website>"
 ]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pymkv" }
 ]
 classifiers = [
@@ -27,18 +27,20 @@
 ]
 keywords = ["wrapper"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 bitmath = "1.3.3.1"
 iso-639 = "0.4.5"
-bcp47 = "0.0.6"
+bcp47 = "0.1.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^7.3.7"
+pytest = "^8.2.1"
+pytest-cov = "^5.0.0"
 sphinx-material = {git = "https://github.com/bashtage/sphinx-material.git"}
 
 [tool.poetry.urls]
 homepage = "https://github.com/GitBib/pymkv2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools", "wheel"]
@@ -121,14 +123,15 @@
   "PL",
   "TRY",
   "FLY",
   "PERF",
   "RUF"
 ]
 ignore = [
+  "N999",
   "FBT002",
   "FBT001",
   "ANN101",
   "S101", # Use of assert detected https://docs.astral.sh/ruff/rules/assert/
   "RUF012", # Mutable class attributes should be annotated with `typing.ClassVar`
   "SIM102", # sometimes it's better to nest
   "UP038" # Checks for uses of isinstance/issubclass that take a tuple
```

### Comparing `pymkv2-2.0.2/PKG-INFO` & `pymkv2-2.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymkv2
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Python wrapper for mkvmerge. It provides support for muxing, splitting, linking, chapters, tags, and attachments through the use of mkvmerge.
 License: MIT
 Keywords: wrapper
 Author: Sheldon Woodward
 Author-email: me@sheldonw.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Utilities
-Requires-Dist: bcp47 (==0.0.6)
+Requires-Dist: bcp47 (==0.1.0)
 Requires-Dist: bitmath (==1.3.3.1)
 Requires-Dist: iso-639 (==0.4.5)
 Project-URL: homepage, https://github.com/GitBib/pymkv2
 Description-Content-Type: text/markdown
 
 # pymkv2
 [![PyPI Version](https://img.shields.io/pypi/v/pymkv2.svg)](https://pypi.python.org/pypi/pymkv2)
@@ -39,25 +39,27 @@
 scriptable and easier to use. Please open new issues for any bugs you find, support is greatly appreciated!
 
 ## Installation
 mkvmerge must be installed on your computer, it is needed to process files when creating MKV objects. It is also
 recommended to add it to your $PATH variable but a different path can be manually specified. mkvmerge can be found
 and downloaded from [here](https://mkvtoolnix.download/downloads.html) or from most package managers.
 
+To install pymkv from PyPI, use the following command:
+
+    $ pip install pymkv2
+
 You can also clone the repo and run the following command in the project root to install the source code as editable:
 
     $ pip install -e .
 
 ## Documentation
 The documentation for pymkv can be found [here](https://gitbib.github.io/pymkv2/) or in the project's docstrings.
 
 ### Tests
-~~After completing documentation for the existing features, unit tests need to be written to "lock in" the existing
-functionality. Generating mkvmerge commands can be complex and it is easy to subtly modify an existing feature when
-adding a new one. Unit tests will ensure that features remain the same and help prevent bugs in the future.~~
+Added the first tests for the project. Still a lot to do, but it’s a start. Currently, 49% is covered by tests.
 
 ### Cleanup
 ~~The existing code base could use some tidying, better commenting, debugging, and a general styling overhaul. Setting up
 [pre-commit](https://pre-commit.com/) and the [Black code formatter](https://github.com/psf/black) will help keep the
 code base more readable and maintainable.~~
 
 ### Features
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

