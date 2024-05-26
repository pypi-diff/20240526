# Comparing `tmp/bvhio-1.4.0.tar.gz` & `tmp/bvhio-1.4.1.tar.gz`

## Comparing `bvhio-1.4.0.tar` & `bvhio-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.4.0/.flake8
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.4.0/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.4.0/changelog.txt
--rw-r--r--   0        0        0    22903 2020-02-02 00:00:00.000000 bvhio-1.4.0/test.ipynb
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.4.0/.github/workflows/build_main.yml
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.4.0/.github/workflows/build_preview.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/__init__.py
--rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/Parser.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/bvh/BvhContainer.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/bvh/BvhJoint.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/bvh/__init__.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/hierarchy/Joint.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/hierarchy/__init__.py
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/test_bvh.py
--rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/test_hierarchy.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/test_io.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bvhio-1.4.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.4.0/LICENSE
--rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 bvhio-1.4.0/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bvhio-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.4.1/.flake8
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.4.1/CITATION.cff
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.4.1/changelog.txt
+-rw-r--r--   0        0        0    25659 2020-02-02 00:00:00.000000 bvhio-1.4.1/test.ipynb
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.4.1/.github/workflows/build_main.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.4.1/.github/workflows/build_preview.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/__init__.py
+-rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/lib/Parser.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/lib/bvh/BvhContainer.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/lib/bvh/BvhJoint.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/lib/bvh/__init__.py
+-rw-r--r--   0        0        0    20303 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/lib/hierarchy/Joint.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/lib/hierarchy/__init__.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/tests/test_bvh.py
+-rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/tests/test_hierarchy.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/tests/test_io.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.4.1/bvhio/tests/utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bvhio-1.4.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.4.1/LICENSE
+-rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 bvhio-1.4.1/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bvhio-1.4.1/PKG-INFO
```

### Comparing `bvhio-1.4.0/test.ipynb` & `bvhio-1.4.1/test.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983760127314815%*

 * *Differences: {"'cells'": "{11: {'execution_count': 3, 'outputs': {0: {'text': {delete: [5, 4]}}, insert: [(1, "*

 * *            "OrderedDict([('ename', 'IndexError'), ('evalue', 'list index out of range'), "*

 * *            "('output_type', 'error'), ('traceback', "*

 * *            "['\\x1b[1;31m---------------------------------------------------------------------------\\x1b[0m', "*

 * *            "'\\x1b[1;31mIndexError\\x1b[0m                                Traceback (most recent "*

 * *            'call last)\', "Cell \\x1b[1;32mIn[3], l […]*

```diff
@@ -390,27 +390,37 @@
                 "file1.FrameCount += file2.FrameCount\n",
                 "\n",
                 "bvhio.writeBvh('test.bvh', file1, 4)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Loading test2.bvh\n",
                         "| Set T-pose\n",
                         "| Correct bone roll\n",
-                        "| Correct scale\n",
-                        "| Write file\n",
-                        "Done.\n"
+                        "| Correct scale\n"
+                    ]
+                },
+                {
+                    "ename": "IndexError",
+                    "evalue": "list index out of range",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[1;31mIndexError\u001b[0m                                Traceback (most recent call last)",
+                        "Cell \u001b[1;32mIn[3], line 88\u001b[0m\n\u001b[0;32m     85\u001b[0m     \u001b[38;5;28mprint\u001b[39m(\u001b[38;5;124m'\u001b[39m\u001b[38;5;124m| Write file\u001b[39m\u001b[38;5;124m'\u001b[39m)\n\u001b[0;32m     86\u001b[0m     bvhio\u001b[38;5;241m.\u001b[39mwriteHierarchy(path\u001b[38;5;241m=\u001b[39mdestination, root\u001b[38;5;241m=\u001b[39mroot, frameTime\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m1\u001b[39m\u001b[38;5;241m/\u001b[39m\u001b[38;5;241m30\u001b[39m)\n\u001b[1;32m---> 88\u001b[0m \u001b[43mmodifyFile\u001b[49m\u001b[43m(\u001b[49m\u001b[38;5;124;43m'\u001b[39;49m\u001b[38;5;124;43mtest2.bvh\u001b[39;49m\u001b[38;5;124;43m'\u001b[39;49m\u001b[43m,\u001b[49m\u001b[43m \u001b[49m\u001b[38;5;124;43m'\u001b[39;49m\u001b[38;5;124;43mout.bvh\u001b[39;49m\u001b[38;5;124;43m'\u001b[39;49m\u001b[43m)\u001b[49m\n\u001b[0;32m     89\u001b[0m \u001b[38;5;28mprint\u001b[39m(\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mDone.\u001b[39m\u001b[38;5;124m'\u001b[39m)\n\u001b[0;32m     90\u001b[0m bvh \u001b[38;5;241m=\u001b[39m bvhio\u001b[38;5;241m.\u001b[39mreadAsBvh(\u001b[38;5;124m'\u001b[39m\u001b[38;5;124mout.bvh\u001b[39m\u001b[38;5;124m'\u001b[39m)\n",
+                        "Cell \u001b[1;32mIn[3], line 83\u001b[0m, in \u001b[0;36mmodifyFile\u001b[1;34m(source, destination)\u001b[0m\n\u001b[0;32m     80\u001b[0m root\u001b[38;5;241m.\u001b[39mapplyRestposeScale(recursive\u001b[38;5;241m=\u001b[39m\u001b[38;5;28;01mTrue\u001b[39;00m, bake\u001b[38;5;241m=\u001b[39m\u001b[38;5;28;01mFalse\u001b[39;00m, bakeKeyframes\u001b[38;5;241m=\u001b[39m\u001b[38;5;28;01mTrue\u001b[39;00m)\n\u001b[0;32m     82\u001b[0m \u001b[38;5;66;03m# remove the root joint\u001b[39;00m\n\u001b[1;32m---> 83\u001b[0m root \u001b[38;5;241m=\u001b[39m \u001b[43mroot\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mChildren\u001b[49m\u001b[43m[\u001b[49m\u001b[38;5;241;43m14\u001b[39;49m\u001b[43m]\u001b[49m\u001b[38;5;241m.\u001b[39mclearParent()\n\u001b[0;32m     85\u001b[0m \u001b[38;5;28mprint\u001b[39m(\u001b[38;5;124m'\u001b[39m\u001b[38;5;124m| Write file\u001b[39m\u001b[38;5;124m'\u001b[39m)\n\u001b[0;32m     86\u001b[0m bvhio\u001b[38;5;241m.\u001b[39mwriteHierarchy(path\u001b[38;5;241m=\u001b[39mdestination, root\u001b[38;5;241m=\u001b[39mroot, frameTime\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m1\u001b[39m\u001b[38;5;241m/\u001b[39m\u001b[38;5;241m30\u001b[39m)\n",
+                        "\u001b[1;31mIndexError\u001b[0m: list index out of range"
                     ]
                 }
             ],
             "source": [
                 "import sys\n",
                 "import os\n",
                 "import glm\n",
@@ -489,22 +499,21 @@
                 "\n",
                 "    # scale to meters\n",
                 "    print('| Correct scale')\n",
                 "    root.RestPose.Scale = 0.012\n",
                 "    root.applyRestposeScale(recursive=True, bake=False, bakeKeyframes=True)\n",
                 "\n",
                 "    # remove the root joint\n",
-                "    root = root.Children[0].clearParent()\n",
+                "    root = layout[14][0].clearParent()\n",
                 "\n",
                 "    print('| Write file')\n",
                 "    bvhio.writeHierarchy(path=destination, root=root, frameTime=1/30)\n",
                 "\n",
                 "modifyFile('test2.bvh', 'out.bvh')\n",
                 "print('Done.')\n",
-                "\n",
                 "bvh = bvhio.readAsBvh('out.bvh')\n",
                 "for joint, index, depth in bvh.Root.layout():\n",
                 "    joint.Channels = ['Xposition', 'Yposition', 'Zposition'] if joint.Name == \"Hips\" else []\n",
                 "    joint.Channels.extend(['Zrotation', 'Yrotation', 'Xrotation'])\n",
                 "bvhio.writeBvh('final.bvh', bvh, percision=6)"
             ]
         }
```

### Comparing `bvhio-1.4.0/.github/workflows/build_main.yml` & `bvhio-1.4.1/.github/workflows/build_main.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/.github/workflows/build_preview.yml` & `bvhio-1.4.1/.github/workflows/build_preview.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/lib/Parser.py` & `bvhio-1.4.1/bvhio/lib/Parser.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/lib/bvh/BvhContainer.py` & `bvhio-1.4.1/bvhio/lib/bvh/BvhContainer.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/lib/bvh/BvhJoint.py` & `bvhio-1.4.1/bvhio/lib/bvh/BvhJoint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/lib/hierarchy/Joint.py` & `bvhio-1.4.1/bvhio/lib/hierarchy/Joint.py`

 * *Files 4% similar despite different names*

```diff
@@ -298,56 +298,76 @@
             child.Rotation = changeInverse * child.Rotation
 
             if recursive:
                 child.roll(degrees, recursive=True)
 
         return self
 
-    def attach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
+    def attach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale', 'rest', 'anim']) -> "Joint":
         super().attach(*nodes, keep=keep)
 
-        if keep is not None and 'anim' in keep:
+        if keep is not None and ('anim' in keep or 'rest' in keep):
             root = self
             while root.Parent is not None:
                 root = self.Parent
 
-            for frame in range(*root.getKeyframeRange()):
-                root.loadPose(frame, recursive=True)
+            if 'rest' in keep:
+                root.loadRestPose(recursive=True)
                 for node in nodes:
-                    node.loadPose(frame, recursive=True)
-                    node.Position = self.SpaceWorldInverse * node.Position
-                    node.Rotation = self.RotationWorldInverse * node.Rotation
-                    node.Scale = self.ScaleWorldInverse * node.Scale
-                    node.writePose(frame, recursive=False)
+                    node.loadRestPose(recursive=True)
+                    if 'position' in keep: node.Position = self.SpaceWorldInverse * node.Position
+                    if 'rotation' in keep: node.Rotation = self.RotationWorldInverse * node.Rotation
+                    if 'scale' in keep: node.Scale = self.ScaleWorldInverse * node.Scale
+                    node.writeRestPose(recursive=False)
+
+            if 'anim' in keep:
+                for frame in range(*root.getKeyframeRange()):
+                    root.loadPose(frame, recursive=True)
+                    for node in nodes:
+                        node.loadPose(frame, recursive=True)
+                        if 'position' in keep: node.Position = self.SpaceWorldInverse * node.Position
+                        if 'rotation' in keep: node.Rotation = self.RotationWorldInverse * node.Rotation
+                        if 'scale' in keep: node.Scale = self.ScaleWorldInverse * node.Scale
+                        node.writePose(frame, recursive=False)
 
         return self
 
-    def detach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
-        super().detach(*nodes, keep=keep)
+    def detach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale', 'rest', 'anim']) -> "Joint":
+        super().detach(*nodes)
 
-        if keep is not None and 'anim' in keep:
+        if keep is not None and ('anim' in keep or 'rest' in keep):
             root = self
             while root.Parent is not None:
                 root = self.Parent
 
-            for frame in range(*root.getKeyframeRange()):
-                root.loadPose(frame, recursive=True)
+            if 'rest' in keep:
+                root.loadRestPose(recursive=True)
                 for node in nodes:
-                    node.loadPose(frame, recursive=True)
-                    node.Position = self.SpaceWorld * node.Position
-                    node.Rotation = self.RotationWorld * node.Rotation
-                    node.Scale = self.ScaleWorld * node.Scale
-                    node.writePose(frame, recursive=False)
+                    node.loadRestPose(recursive=True)
+                    if 'position' in keep: node.Position = self.SpaceWorld * node.Position
+                    if 'rotation' in keep: node.Rotation = self.RotationWorld * node.Rotation
+                    if 'scale' in keep: node.Scale = self.ScaleWorld * node.Scale
+                    node.writeRestPose(recursive=False)
+
+            if 'anim' in keep:
+                for frame in range(*root.getKeyframeRange()):
+                    root.loadPose(frame, recursive=True)
+                    for node in nodes:
+                        node.loadPose(frame, recursive=True)
+                        if 'position' in keep: node.Position = self.SpaceWorld * node.Position
+                        if 'rotation' in keep: node.Rotation = self.RotationWorld * node.Rotation
+                        if 'scale' in keep: node.Scale = self.ScaleWorld * node.Scale
+                        node.writePose(frame, recursive=False)
 
         return self
 
-    def clearParent(self, keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
+    def clearParent(self, keep: list[str] = ['position', 'rotation', 'scale', 'rest', 'anim']) -> "Joint":
         return super().clearParent(keep=keep)
 
-    def clearChildren(self, keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
+    def clearChildren(self, keep: list[str] = ['position', 'rotation', 'scale', 'rest', 'anim']) -> "Joint":
         return super().clearChildren(keep=keep)
 
     def applyPosition(self, position: glm.vec3 = None, recursive: bool = False) -> "Joint":
         return super().applyPosition(position, recursive)
 
     def applyRestposePosition(self, position: glm.vec3 = None, recursive: bool = False) -> "Joint":
         """"Resets the position of the Restpose to (0,0,0) or adds the given position.
```

### Comparing `bvhio-1.4.0/bvhio/tests/test_bvh.py` & `bvhio-1.4.1/bvhio/tests/test_bvh.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/tests/test_hierarchy.py` & `bvhio-1.4.1/bvhio/tests/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/tests/test_io.py` & `bvhio-1.4.1/bvhio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/bvhio/tests/utils.py` & `bvhio-1.4.1/bvhio/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/LICENSE` & `bvhio-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/README.md` & `bvhio-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bvhio-1.4.0/pyproject.toml` & `bvhio-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bvhio"
-version = "1.4.0"
+version = "1.4.1"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Read, write, edit and create .bvh files with hierarchical 3D transforms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bvhio-1.4.0/PKG-INFO` & `bvhio-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bvhio
-Version: 1.4.0
+Version: 1.4.1
 Summary: Read, write, edit and create .bvh files with hierarchical 3D transforms.
 Project-URL: Homepage, https://github.com/Wasserwecken/bvhio
 Project-URL: Bug Tracker, https://github.com/Wasserwecken/bvhio/issues
 Author-email: Wasserwecken <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: bvhio Version: 1.4.0 Summary: Read, write, edit and
+Metadata-Version: 2.3 Name: bvhio Version: 1.4.1 Summary: Read, write, edit and
 create .bvh files with hierarchical 3D transforms. Project-URL: Homepage,
 https://github.com/Wasserwecken/bvhio Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/bvhio/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy Requires-
 Dist: pyglm==2.7.1 Requires-Dist: spatial-transform==1.2.13 Description-
```

