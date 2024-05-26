# Comparing `tmp/mihomo-2.2.0.tar.gz` & `tmp/mihomo-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mihomo-2.2.0.tar", max compression
+gzip compressed data, was "mihomo-2.3.0.tar", max compression
```

## Comparing `mihomo-2.2.0.tar` & `mihomo-2.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-2.2.0/LICENSE
--rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-2.2.0/mihomo/__init__.py
--rw-r--r--   0        0        0    11229 2024-05-23 12:35:29.351454 mihomo-2.2.0/mihomo/api.py
--rw-r--r--   0        0        0     2722 2024-05-23 12:35:33.779456 mihomo-2.2.0/mihomo/model.py
--rw-r--r--   0        0        0      479 2024-05-23 12:41:33.511016 mihomo-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      366 2024-02-06 13:37:45.700640 mihomo-2.2.0/README.md
--rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 mihomo-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-01 05:14:24.496130 mihomo-2.3.0/LICENSE
+-rw-r--r--   0        0        0       90 2023-06-07 08:41:32.652372 mihomo-2.3.0/mihomo/__init__.py
+-rw-r--r--   0        0        0    11395 2024-05-26 10:07:40.419468 mihomo-2.3.0/mihomo/api.py
+-rw-r--r--   0        0        0     2799 2024-05-26 10:06:49.546106 mihomo-2.3.0/mihomo/model.py
+-rw-r--r--   0        0        0      479 2024-05-26 10:17:11.566883 mihomo-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      366 2024-02-06 13:37:45.700640 mihomo-2.3.0/README.md
+-rw-r--r--   0        0        0     1166 1970-01-01 00:00:00.000000 mihomo-2.3.0/PKG-INFO
```

### Comparing `mihomo-2.2.0/LICENSE` & `mihomo-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mihomo-2.2.0/mihomo/api.py` & `mihomo-2.3.0/mihomo/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,17 +260,20 @@
                         chaos_star_count=space_info.challengeInfo.abyssStarCount,
                     )
                 else:
                     memory_info = None
                 player_info.space_info = SpaceInfo(
                     memory_data=memory_info,
                     universe_level=space_info.maxRogueChallengeScore,
-                    light_cone_count=space_info.equipmentCount,
                     avatar_count=space_info.avatarCount,
+                    light_cone_count=space_info.equipmentCount,
+                    relic_count=space_info.relicCount,
                     achievement_count=space_info.achievementCount,
+                    book_count=space_info.bookCount,
+                    music_count=space_info.musicCount,
                 )
         pos_dict: Dict[str, List[int]] = {}
         characters: List[CharacterInfo] = []
         if api_data.detailInfo.assistAvatarList:
             for character in api_data.detailInfo.assistAvatarList:
                 pos_dict[str(character.avatarId)] = [character.pos]
                 character_info = self.character_parse(character, language)
```

### Comparing `mihomo-2.2.0/mihomo/model.py` & `mihomo-2.3.0/mihomo/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,20 @@
     chaos_level: Optional[int] = None
     chaos_star_count: Optional[int] = None
 
 
 class SpaceInfo(Struct):
     memory_data: Optional[MemoryInfo] = None
     universe_level: int = 0
-    light_cone_count: int = 0
     avatar_count: int = 0
+    light_cone_count: int = 0
+    relic_count: int = 0
     achievement_count: int = 0
+    book_count: int = 0
+    music_count: int = 0
 
 
 class PlayerInfo(Struct):
     uid: str
     nickname: str
     level: int = 0
     world_level: int = 0
```

### Comparing `mihomo-2.2.0/PKG-INFO` & `mihomo-2.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mihomo
-Version: 2.2.0
+Version: 2.3.0
 Summary: Library for API wrapper data from mihomo
 Home-page: https://github.com/Mar-7th/mihomo.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
-Requires-Dist: starrailres (>=2.0.0,<3.0.0)
+Requires-Dist: starrailres (>=2.1.0,<3.0.0)
 Project-URL: Repository, https://github.com/Mar-7th/mihomo.py
 Description-Content-Type: text/markdown
 
 # mihomo.py
 
 ## Introduction
```

