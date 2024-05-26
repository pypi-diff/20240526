# Comparing `tmp/starrailres-2.0.0.tar.gz` & `tmp/starrailres-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailres-2.0.0.tar", max compression
+gzip compressed data, was "starrailres-2.1.0.tar", max compression
```

## Comparing `starrailres-2.0.0.tar` & `starrailres-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-2.0.0/LICENSE
--rw-r--r--   0        0        0      498 2024-02-07 11:33:43.159016 starrailres-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      924 2023-05-31 11:58:49.998393 starrailres-2.0.0/README.md
--rw-r--r--   0        0        0       22 2023-06-11 09:13:33.282915 starrailres-2.0.0/starrailres/__init__.py
--rw-r--r--   0        0        0    32577 2023-09-24 11:00:45.066862 starrailres-2.0.0/starrailres/index.py
--rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-2.0.0/starrailres/models/avatars.py
--rw-r--r--   0        0        0     1695 2023-10-04 11:13:38.989084 starrailres-2.0.0/starrailres/models/characters.py
--rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-2.0.0/starrailres/models/common.py
--rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-2.0.0/starrailres/models/descriptions.py
--rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-2.0.0/starrailres/models/elements.py
--rw-r--r--   0        0        0     3071 2024-02-07 11:21:28.748135 starrailres-2.0.0/starrailres/models/info.py
--rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-2.0.0/starrailres/models/items.py
--rw-r--r--   0        0        0      739 2023-10-04 11:18:14.298635 starrailres-2.0.0/starrailres/models/light_cones.py
--rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-2.0.0/starrailres/models/paths.py
--rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-2.0.0/starrailres/models/properties.py
--rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-2.0.0/starrailres/models/relics.py
--rw-r--r--   0        0        0      323 2023-06-11 09:13:35.175657 starrailres-2.0.0/starrailres/utils.py
--rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 starrailres-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-23 12:01:47.249793 starrailres-2.1.0/LICENSE
+-rw-r--r--   0        0        0      494 2024-05-26 09:51:46.303802 starrailres-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      924 2024-05-26 10:01:45.602970 starrailres-2.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-11 09:13:33.282915 starrailres-2.1.0/starrailres/__init__.py
+-rw-r--r--   0        0        0    32953 2024-05-26 10:00:30.588733 starrailres-2.1.0/starrailres/index.py
+-rw-r--r--   0        0        0      216 2023-05-31 13:14:58.577684 starrailres-2.1.0/starrailres/models/avatars.py
+-rw-r--r--   0        0        0     1695 2023-10-04 11:13:38.989084 starrailres-2.1.0/starrailres/models/characters.py
+-rw-r--r--   0        0        0      210 2023-05-26 14:44:56.999166 starrailres-2.1.0/starrailres/models/common.py
+-rw-r--r--   0        0        0      245 2023-05-25 07:04:39.480460 starrailres-2.1.0/starrailres/models/descriptions.py
+-rw-r--r--   0        0        0      295 2023-05-23 14:27:36.388191 starrailres-2.1.0/starrailres/models/elements.py
+-rw-r--r--   0        0        0     3086 2024-05-26 09:55:41.643026 starrailres-2.1.0/starrailres/models/info.py
+-rw-r--r--   0        0        0      352 2023-05-25 07:16:41.407713 starrailres-2.1.0/starrailres/models/items.py
+-rw-r--r--   0        0        0      739 2023-10-04 11:18:14.298635 starrailres-2.1.0/starrailres/models/light_cones.py
+-rw-r--r--   0        0        0      269 2023-05-23 14:27:09.523569 starrailres-2.1.0/starrailres/models/paths.py
+-rw-r--r--   0        0        0      429 2023-05-29 14:28:24.391190 starrailres-2.1.0/starrailres/models/properties.py
+-rw-r--r--   0        0        0      993 2023-05-30 04:32:44.019242 starrailres-2.1.0/starrailres/models/relics.py
+-rw-r--r--   0        0        0      323 2023-06-11 09:13:35.175657 starrailres-2.1.0/starrailres/utils.py
+-rw-r--r--   0        0        0     1615 1970-01-01 00:00:00.000000 starrailres-2.1.0/PKG-INFO
```

### Comparing `starrailres-2.0.0/LICENSE` & `starrailres-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailres-2.0.0/README.md` & `starrailres-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `starrailres-2.0.0/starrailres/index.py` & `starrailres-2.1.0/starrailres/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,24 @@
     RelicMainAffixIndex,
     RelicSetIndex,
     RelicSubAffixIndex,
 )
 from .utils import decode_json
 
 
+relic_type_map: Dict[str, int] = {
+    "HEAD": 1,
+    "HAND": 2,
+    "BODY": 3,
+    "FOOT": 4,
+    "NECK": 5,
+    "OBJECT": 6,
+}
+
+
 class Index:
     characters: CharacterIndex
     character_ranks: CharacterRankIndex
     character_skills: CharacterSkillIndex
     character_skill_trees: CharacterSkillTreeIndex
     character_promotions: CharacterPromotionIndex
     light_cones: LightConeIndex
@@ -264,14 +274,15 @@
 
     def get_relic_info(self, basic: RelicBasicInfo) -> Optional[RelicInfo]:
         if basic.id not in self.relics:
             return None
         info = RelicInfo(
             id=basic.id,
             name=self.relics[basic.id].name,
+            type=relic_type_map.get(self.relics[basic.id].type, 0),
             set_id=self.relics[basic.id].set_id,
             set_name=self.relic_sets[self.relics[basic.id].set_id].name,
             rarity=self.relics[basic.id].rarity,
             level=basic.level,
             icon=self.relics[basic.id].icon,
             main_affix=self.get_relic_main_affix(
                 basic.id, basic.level, basic.main_affix_id
@@ -317,17 +328,19 @@
             if v >= 4:
                 relic_sets.append(
                     RelicSetInfo(
                         id=k,
                         name=self.relic_sets[k].name,
                         icon=self.relic_sets[k].icon,
                         num=4,
-                        desc=self.relic_sets[k].desc[1]
-                        if len(self.relic_sets[k].desc) > 1
-                        else "",
+                        desc=(
+                            self.relic_sets[k].desc[1]
+                            if len(self.relic_sets[k].desc) > 1
+                            else ""
+                        ),
                         properties=[
                             PropertyInfo(
                                 type=i.type,
                                 field=self.properties[i.type].field,
                                 name=self.properties[i.type].name,
                                 icon=self.properties[i.type].icon,
                                 value=i.value,
@@ -416,23 +429,27 @@
             skill_tree_dict[skill_tree.id] = skill_tree.level
         skill_tree_info_list = []
         for skill_tree_id in self.characters[id].skill_trees:
             if skill_tree_id not in self.character_skill_trees:
                 return []
             parsed_info = SkillTreeInfo(
                 id=skill_tree_id,
-                level=skill_tree_dict[skill_tree_id]
-                if skill_tree_id in skill_tree_dict
-                else 0,
+                level=(
+                    skill_tree_dict[skill_tree_id]
+                    if skill_tree_id in skill_tree_dict
+                    else 0
+                ),
                 max_level=self.character_skill_trees[skill_tree_id].max_level,
                 anchor=self.character_skill_trees[skill_tree_id].anchor,
                 icon=self.character_skill_trees[skill_tree_id].icon,
-                parent=self.character_skill_trees[skill_tree_id].pre_points[0]
-                if self.character_skill_trees[skill_tree_id].pre_points
-                else None,
+                parent=(
+                    self.character_skill_trees[skill_tree_id].pre_points[0]
+                    if self.character_skill_trees[skill_tree_id].pre_points
+                    else None
+                ),
             )
             skill_tree_info_list.append(parsed_info)
         return skill_tree_info_list
 
     def get_character_attribute_from_promotion(
         self, id: str, promotion: int, level: int
     ) -> List[AttributeInfo]:
```

### Comparing `starrailres-2.0.0/starrailres/models/characters.py` & `starrailres-2.1.0/starrailres/models/characters.py`

 * *Files identical despite different names*

### Comparing `starrailres-2.0.0/starrailres/models/info.py` & `starrailres-2.1.0/starrailres/models/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     light_cone: Optional[LightConeBasicInfo] = None
     relics: Optional[List[RelicBasicInfo]] = None
 
 
 class RelicInfo(Struct):
     id: str
     name: str
+    type: int
     set_id: str
     set_name: str
     rarity: int
     level: int
     icon: str
     main_affix: Optional[PropertyInfo] = None
     sub_affix: List[SubAffixInfo] = []
```

### Comparing `starrailres-2.0.0/starrailres/models/light_cones.py` & `starrailres-2.1.0/starrailres/models/light_cones.py`

 * *Files identical despite different names*

### Comparing `starrailres-2.0.0/starrailres/models/relics.py` & `starrailres-2.1.0/starrailres/models/relics.py`

 * *Files identical despite different names*

### Comparing `starrailres-2.0.0/PKG-INFO` & `starrailres-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: starrailres
-Version: 2.0.0
+Version: 2.1.0
 Summary: StarRailRes parse package
-Home-page: https://github.com/Mar-7th/StarRailRes-Python
+Home-page: https://github.com/Mar-7th/starrailres.py
 License: MIT
 Author: mobyw
 Author-email: mobyw66@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: msgspec (>=0.15.1,<0.16.0)
-Project-URL: Repository, https://github.com/Mar-7th/StarRailRes-Python
+Project-URL: Repository, https://github.com/Mar-7th/starrailres.py
 Description-Content-Type: text/markdown
 
 # StarRailRes-Python
 
 A python library for StarRailRes.
 
 ## Installation
```

