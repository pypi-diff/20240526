# Comparing `tmp/bvhio-1.3.9.tar.gz` & `tmp/bvhio-1.4.0.tar.gz`

## Comparing `bvhio-1.3.9.tar` & `bvhio-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.3.9/.flake8
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.3.9/CITATION.cff
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.3.9/changelog.txt
--rw-r--r--   0        0        0    17292 2020-02-02 00:00:00.000000 bvhio-1.3.9/test.ipynb
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.3.9/.github/workflows/build_main.yml
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.3.9/.github/workflows/build_preview.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/__init__.py
--rw-r--r--   0        0        0    13640 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/lib/Parser.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/lib/bvh/BvhContainer.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/lib/bvh/BvhJoint.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/lib/bvh/__init__.py
--rw-r--r--   0        0        0    17687 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/lib/hierarchy/Joint.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/lib/hierarchy/__init__.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/tests/example.bvh
--rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/tests/test_bvh.py
--rw-r--r--   0        0        0    22186 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/tests/test_hierarchy.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/tests/test_io.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.3.9/bvhio/tests/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bvhio-1.3.9/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.3.9/LICENSE
--rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 bvhio-1.3.9/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.3.9/pyproject.toml
--rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bvhio-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 bvhio-1.4.0/.flake8
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 bvhio-1.4.0/CITATION.cff
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bvhio-1.4.0/changelog.txt
+-rw-r--r--   0        0        0    22903 2020-02-02 00:00:00.000000 bvhio-1.4.0/test.ipynb
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 bvhio-1.4.0/.github/workflows/build_main.yml
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 bvhio-1.4.0/.github/workflows/build_preview.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/__init__.py
+-rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/Parser.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/bvh/BvhContainer.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/bvh/BvhJoint.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/bvh/__init__.py
+-rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/hierarchy/Joint.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/lib/hierarchy/__init__.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/test_bvh.py
+-rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/test_hierarchy.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/test_io.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 bvhio-1.4.0/bvhio/tests/utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bvhio-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 bvhio-1.4.0/LICENSE
+-rw-r--r--   0        0        0    19372 2020-02-02 00:00:00.000000 bvhio-1.4.0/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bvhio-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    20005 2020-02-02 00:00:00.000000 bvhio-1.4.0/PKG-INFO
```

### Comparing `bvhio-1.3.9/test.ipynb` & `bvhio-1.4.0/test.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'cells'": "{insert: [(11, OrderedDict([('cell_type', 'code'), ('execution_count', 1), "*

 * *            "('metadata', OrderedDict()), ('outputs', [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['Loading test2.bvh\\n', '| Set T-pose\\n', '| "*

 * *            "Correct bone roll\\n', '| Correct scale\\n', '| Write file\\n', 'Done.\\n'])])]), "*

 * *            "('source', ['import sys\\n', 'import os\\n', 'import glm\\n', 'import bvhio\\n', "*

 * *            "'from pathlib import Path\\n […]*

```diff
@@ -387,14 +387,130 @@
                 "    joint.Keyframes.extend(data2[index][0].Keyframes)\n",
                 "\n",
                 "# update framecount to write all animation\n",
                 "file1.FrameCount += file2.FrameCount\n",
                 "\n",
                 "bvhio.writeBvh('test.bvh', file1, 4)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Loading test2.bvh\n",
+                        "| Set T-pose\n",
+                        "| Correct bone roll\n",
+                        "| Correct scale\n",
+                        "| Write file\n",
+                        "Done.\n"
+                    ]
+                }
+            ],
+            "source": [
+                "import sys\n",
+                "import os\n",
+                "import glm\n",
+                "import bvhio\n",
+                "from pathlib import Path\n",
+                "\n",
+                "# requires two packages:\n",
+                "# pip install PyGLM\n",
+                "# pip install bvhio\n",
+                "# pip install spatial-transform\n",
+                "\n",
+                "# usage\n",
+                "# - destination and source directiory has to exist\n",
+                "# - does not parese directories recusivley\n",
+                "# - VERY slow, because the libary is written purely in pythn and recursivly\n",
+                "# - example for cmd: python .\\converter.py .\\sourceDir\\ .\\destinationDir\n",
+                "\n",
+                "\n",
+                "# this script will correct the rest pose of the .bvh files from the bandai namco set\n",
+                "# https://github.com/BandaiNamcoResearchInc/Bandai-Namco-Research-Motiondataset\n",
+                "def modifyFile(source: str, destination: str):\n",
+                "    print(f'Loading {os.path.basename(source)}')\n",
+                "    root = bvhio.readAsHierarchy(source)\n",
+                "    layout = root.layout()\n",
+                "\n",
+                "    # set up T-pose\n",
+                "    print('| Set T-pose')\n",
+                "    root.loadRestPose()\n",
+                "    layout[ 0][0].setEuler((   0,   0,   0))                # joint_Root\n",
+                "    layout[ 1][0].setEuler((   0,   0,   0))                # Hips\n",
+                "    layout[ 1][0].Position = (0, 94, 0)                     # Hips\n",
+                "    layout[ 2][0].setEuler((   0,   0,   0))                # Spine\n",
+                "    layout[ 3][0].setEuler((   0, +90,   0)).roll(-90)      # Chest\n",
+                "    layout[ 4][0].setEuler((   0,   0,   0))                # Neck\n",
+                "    layout[ 5][0].setEuler((   0,   0,   0))                # Head\n",
+                "\n",
+                "    layout[ 6][0].setEuler((   0,   0, -90))                # Shoulder_L\n",
+                "    layout[ 7][0].setEuler((   0,   0,   0))                # UpperArm_L\n",
+                "    layout[ 8][0].setEuler((   0,   0,   0))                # LowerArm_L\n",
+                "    layout[ 9][0].setEuler((   0,   0,   0))                # Hand_L\n",
+                "\n",
+                "    layout[10][0].setEuler((   0,   0, +90))                # Shoulder_R\n",
+                "    layout[11][0].setEuler((   0,   0,   0))                # UpperArm_R\n",
+                "    layout[12][0].setEuler((   0,   0,   0))                # LowerArm_R\n",
+                "    layout[13][0].setEuler((   0,   0,   0))                # Hand_R\n",
+                "\n",
+                "    layout[14][0].setEuler((   0,   0, 180))                # UpperLeg_L\n",
+                "    layout[15][0].setEuler((   0,   0,   0))                # LowerLeg_L\n",
+                "    layout[16][0].setEuler((   0,   0,   0))                # Foot_L\n",
+                "    layout[17][0].setEuler((   0,   0,   0))                # Toes_L\n",
+                "\n",
+                "    layout[18][0].setEuler((   0,   0, 180))                # UpperLeg_R\n",
+                "    layout[19][0].setEuler((   0,   0,   0))                # LowerLeg_R\n",
+                "    layout[20][0].setEuler((   0,   0,   0))                # Foot_R\n",
+                "    layout[21][0].setEuler((   0,   0,   0))                # Toes_R\n",
+                "    root.writeRestPose(recursive=True, keep=['position', 'rotation', 'scale'])\n",
+                "\n",
+                "    # key frame corrections, turns joints so than Z- axis always points forward\n",
+                "    # DELETE THIS LOOP IF THE BONE ROLL DOES NOT MATTER TO YOU.\n",
+                "    print('| Correct bone roll')\n",
+                "    for frame in range(*root.getKeyframeRange()):\n",
+                "        root.loadPose(frame, recursive=True)\n",
+                "        layout[ 2][0].roll(-90)                                   # Spine\n",
+                "        layout[ 3][0].roll(-90)                                   # Chest\n",
+                "        layout[ 4][0].roll(-90)                                   # Neck\n",
+                "        layout[ 5][0].roll(-90)                                   # Head\n",
+                "        layout[10][0].roll(180, recursive=True)                   # Shoulder_R\n",
+                "        layout[18][0].roll(180, recursive=True)                   # UpperLeg_R\n",
+                "\n",
+                "        layout[ 5][0].Rotation *= glm.angleAxis(glm.radians(-90), (1, 0, 0))  # Head\n",
+                "        layout[ 9][0].Rotation *= glm.angleAxis(glm.radians(-90), (0, 0, 1))  # Hand_L\n",
+                "        layout[13][0].Rotation *= glm.angleAxis(glm.radians(-90), (0, 0, 1))  # Hand_R\n",
+                "        layout[17][0].Rotation *= glm.angleAxis(glm.radians(-90), (0, 0, 1))  # Toes_L\n",
+                "        layout[21][0].Rotation *= glm.angleAxis(glm.radians(-90), (0, 0, 1))  # Toes_R\n",
+                "        root.writePose(frame, recursive=True)\n",
+                "\n",
+                "    # scale to meters\n",
+                "    print('| Correct scale')\n",
+                "    root.RestPose.Scale = 0.012\n",
+                "    root.applyRestposeScale(recursive=True, bake=False, bakeKeyframes=True)\n",
+                "\n",
+                "    # remove the root joint\n",
+                "    root = root.Children[0].clearParent()\n",
+                "\n",
+                "    print('| Write file')\n",
+                "    bvhio.writeHierarchy(path=destination, root=root, frameTime=1/30)\n",
+                "\n",
+                "modifyFile('test2.bvh', 'out.bvh')\n",
+                "print('Done.')\n",
+                "\n",
+                "bvh = bvhio.readAsBvh('out.bvh')\n",
+                "for joint, index, depth in bvh.Root.layout():\n",
+                "    joint.Channels = ['Xposition', 'Yposition', 'Zposition'] if joint.Name == \"Hips\" else []\n",
+                "    joint.Channels.extend(['Zrotation', 'Yrotation', 'Xrotation'])\n",
+                "bvhio.writeBvh('final.bvh', bvh, percision=6)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `bvhio-1.3.9/.github/workflows/build_main.yml` & `bvhio-1.4.0/.github/workflows/build_main.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/.github/workflows/build_preview.yml` & `bvhio-1.4.0/.github/workflows/build_preview.yml`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/bvhio/lib/Parser.py` & `bvhio-1.4.0/bvhio/lib/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         return bvh
 
 
 def convertBvhToHierarchy(bvh: BvhJoint) -> Joint:
     """Converts a deserialized bvh structure into a joint hierarchy."""
     # copy data into a joint
-    restPose = Transform(name='RestPose', position=bvh.Offset, rotation=bvh.getRotation())
+    restPose = Transform(name=f'RestPose.{bvh.Name}', position=bvh.Offset, rotation=bvh.getRotation())
     joint = Joint(bvh.Name, restPose=restPose)
     for frame, key in enumerate(bvh.Keyframes):
         joint.setKeyframe(frame, Transform.fromPose(key), keep=None)
 
     # correct bvh keyframe data
     for frame, key in joint.Keyframes:
         # project offset into rest pose because it is given as overwrite and does not include the rest pose rotation.
```

### Comparing `bvhio-1.3.9/bvhio/lib/bvh/BvhContainer.py` & `bvhio-1.4.0/bvhio/lib/bvh/BvhContainer.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/bvhio/lib/bvh/BvhJoint.py` & `bvhio-1.4.0/bvhio/lib/bvh/BvhJoint.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/bvhio/lib/hierarchy/Joint.py` & `bvhio-1.4.0/bvhio/lib/hierarchy/Joint.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def __findFrameIndex(self, frame: int):
         if not self.Keyframes:
             return 0
 
         if frame > self.Keyframes[-1][0]:
             return len(self.Keyframes)
-               
+
         return bisect.bisect_left([key[0] for key in self.Keyframes], frame)
 
     def __insertKeyframe(self, frame: int, key: Transform) -> None:
         bisect.insort(self.Keyframes, (frame, key))
         self._KeyframeMap[frame] = key
 
     def getKeyframe(self, frame: int) -> Transform:
@@ -92,15 +92,15 @@
 
         if frame < 0: frame = max(0, self.getKeyframeRange(includeChildren=False)[1] + 1 - frame)
 
         existingFrame = self._KeyframeMap.get(frame)
 
         if existingFrame:
             return existingFrame
-        
+
         # pose definition
         index = self.__findFrameIndex(frame)
         if index == len(self.Keyframes):
             # index is bigger than last frame, take last key
             return self.Keyframes[-1][1]
         elif self.Keyframes[index][0] == frame:
             # index matches a keyframe
@@ -298,24 +298,56 @@
             child.Rotation = changeInverse * child.Rotation
 
             if recursive:
                 child.roll(degrees, recursive=True)
 
         return self
 
-    def attach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale']) -> "Joint":
-        return super().attach(*nodes, keep=keep)
+    def attach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
+        super().attach(*nodes, keep=keep)
+
+        if keep is not None and 'anim' in keep:
+            root = self
+            while root.Parent is not None:
+                root = self.Parent
+
+            for frame in range(*root.getKeyframeRange()):
+                root.loadPose(frame, recursive=True)
+                for node in nodes:
+                    node.loadPose(frame, recursive=True)
+                    node.Position = self.SpaceWorldInverse * node.Position
+                    node.Rotation = self.RotationWorldInverse * node.Rotation
+                    node.Scale = self.ScaleWorldInverse * node.Scale
+                    node.writePose(frame, recursive=False)
+
+        return self
+
+    def detach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
+        super().detach(*nodes, keep=keep)
 
-    def detach(self, *nodes: "Joint", keep: list[str] = ['position', 'rotation', 'scale']) -> "Joint":
-        return super().detach(*nodes, keep=keep)
+        if keep is not None and 'anim' in keep:
+            root = self
+            while root.Parent is not None:
+                root = self.Parent
+
+            for frame in range(*root.getKeyframeRange()):
+                root.loadPose(frame, recursive=True)
+                for node in nodes:
+                    node.loadPose(frame, recursive=True)
+                    node.Position = self.SpaceWorld * node.Position
+                    node.Rotation = self.RotationWorld * node.Rotation
+                    node.Scale = self.ScaleWorld * node.Scale
+                    node.writePose(frame, recursive=False)
+
+        return self
 
-    def clearParent(self, keep: list[str] = ['position', 'rotation', 'scale']) -> "Joint":
+    def clearParent(self, keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
         return super().clearParent(keep=keep)
 
-    def clearChildren(self, keep: list[str] = ['position', 'rotation', 'scale']) -> "Joint":
+    def clearChildren(self, keep: list[str] = ['position', 'rotation', 'scale', 'anim']) -> "Joint":
         return super().clearChildren(keep=keep)
 
     def applyPosition(self, position: glm.vec3 = None, recursive: bool = False) -> "Joint":
         return super().applyPosition(position, recursive)
 
     def applyRestposePosition(self, position: glm.vec3 = None, recursive: bool = False) -> "Joint":
         """"Resets the position of the Restpose to (0,0,0) or adds the given position.
```

### Comparing `bvhio-1.3.9/bvhio/tests/test_bvh.py` & `bvhio-1.4.0/bvhio/tests/test_bvh.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/bvhio/tests/test_hierarchy.py` & `bvhio-1.4.0/bvhio/tests/test_hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,168 +1,169 @@
 import unittest
 import bvhio
 import glm
 from utils import *
 
+Joints = [ # for j, i, d in root.layout(): print(f"( {d}, {len(j.Children)}, {len(j.Keyframes)}, {j.KeyframeRange}, '{j.Name}', ),")
+    ( 0, 3, 2, (0, 1), 'Hips', ),
+    ( 1, 3, 2, (0, 1), 'Chest', ),
+    ( 2, 1, 2, (0, 1), 'Neck', ),
+    ( 3, 0, 2, (0, 1), 'Head', ),
+    ( 2, 1, 2, (0, 1), 'LeftCollar', ),
+    ( 3, 1, 2, (0, 1), 'LeftUpArm', ),
+    ( 4, 1, 2, (0, 1), 'LeftLowArm', ),
+    ( 5, 0, 2, (0, 1), 'LeftHand', ),
+    ( 2, 1, 2, (0, 1), 'RightCollar', ),
+    ( 3, 1, 2, (0, 1), 'RightUpArm', ),
+    ( 4, 1, 2, (0, 1), 'RightLowArm', ),
+    ( 5, 0, 2, (0, 1), 'RightHand', ),
+    ( 1, 1, 2, (0, 1), 'LeftUpLeg', ),
+    ( 2, 1, 2, (0, 1), 'LeftLowLeg', ),
+    ( 3, 0, 2, (0, 1), 'LeftFoot', ),
+    ( 1, 1, 2, (0, 1), 'RightUpLeg', ),
+    ( 2, 1, 2, (0, 1), 'RightLowLeg', ),
+    ( 3, 0, 2, (0, 1), 'RightFoot', ),
+]
+RestPoseLocal = [ # for j, i, d in root.layout(): print(f"( glm.{j.Position}, glm.{j.Rotation}, glm.{j.Scale}, ),")
+    ( glm.vec3(            0,            0,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         5.21,            0 ), glm.quat(     0.999333,    0.0365139,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,      18.6003,     -1.36106 ), glm.quat(     0.999333,   -0.0365139,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         5.45,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         1.12,      16.3232,     0.680562 ), glm.quat(     0.706635,   -0.0258192,   -0.0258192,    -0.706635 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3( -4.76837e-07,         5.54,            0 ), glm.quat(    -0.707107,            0,            0,     0.707107 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        11.96,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         9.93,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -1.12,      16.3232,     0.680562 ), glm.quat(     0.706635,   -0.0258192,    0.0258192,     0.706635 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(  9.53674e-07,         6.07,            0 ), glm.quat(     0.707107,            0,            0,     0.707107 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        11.82,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        10.65,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        18.34,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        17.37,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        17.63,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        17.14,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+]
+RestPoseWorld = [ # for j, i, d in root.layout(): print(f"( glm.{j.PositionWorld}, glm.{j.RotationWorld}, glm.{j.ScaleWorld}, ),")
+    ( glm.vec3(            0,            0,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         5.21,            0 ), glm.quat(     0.999333,    0.0365139,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        23.86,  1.19209e-07 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        29.31,  1.19209e-07 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         1.12,        21.44,         1.87 ), glm.quat(     0.707107,            0,            0,    -0.707107 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         6.66,        21.44,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         6.66,         9.48,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         6.66,    -0.450002,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -1.12,        21.44,         1.87 ), glm.quat(     0.707107,            0,            0,     0.707107 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -7.19,        21.44,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -7.19,         9.62,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -7.19,        -1.03,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         3.91,       -18.34,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         3.91,       -35.71,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -3.91,       -17.63,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -3.91,       -34.77,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
+]
+Pose0Local = [
+    ( glm.vec3(         8.03,        35.01,        88.36 ), glm.quat(     0.131166,   -0.0117277,    -0.982546,    -0.131386 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         5.21,            0 ), glm.quat(     0.905976,     0.390515,    -0.159062,    0.0374775 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,      18.6003,     -1.36106 ), glm.quat(     0.938613,     0.338059,    0.0279395,     0.062775 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         5.45,            0 ), glm.quat(     0.933054,    -0.351756,    0.0585907,   -0.0473785 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         1.12,      16.3232,     0.680562 ), glm.quat(     0.760453,   -0.0960347,    0.0337522,    -0.641365 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3( -4.76837e-07,         5.54,            0 ), glm.quat(    -0.976203,    -0.202105,   -0.0323696,   -0.0716515 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        11.96,            0 ), glm.quat(     0.694325,     0.714836,    0.0378194,   -0.0741041 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,         9.93,            0 ), glm.quat(     0.999982, -0.000261795, -1.57639e-06,   0.00602135 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -1.12,      16.3232,     0.680562 ), glm.quat(     0.781762,    -0.100736,   -0.0338954,     0.614452 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(  9.53674e-07,         6.07,            0 ), glm.quat(     0.614408,    0.0440009,     0.778943,     0.117536 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        11.82,            0 ), glm.quat(     0.762976,     0.606189,    -0.177084,     0.138002 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        10.65,            0 ), glm.quat(     0.999888,  -0.00602318, -9.20184e-05,   -0.0136991 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(         3.91,            0,            0 ), glm.quat(    -0.117674,    -0.024446,    -0.202143,     0.971953 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        18.34,            0 ), glm.quat(     0.894013,    -0.411485,    -0.106536,     0.141674 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        17.37,            0 ), glm.quat(     0.999951,   0.00994821,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(        -3.91,            0,            0 ), glm.quat(     0.141065,   -0.0135394,    0.0944943,     0.985387 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        17.63,            0 ), glm.quat(     0.883393,      -0.4543,     0.109673,    0.0346498 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(            0,        17.14,            0 ), glm.quat(     0.978238,     0.207485,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
+]
+Pose0World = [
+    ( glm.vec3(         8.03,        35.01,        88.36 ), glm.quat(     0.131166,   -0.0117277,    -0.982546,    -0.131386 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      8.32964,      40.0387,      89.6891 ), glm.quat(    -0.027949,   -0.0171246,    -0.961895,     0.271448 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      9.16411,       56.599,      81.1521 ), glm.quat(   -0.0106095,   -0.0934888,    -0.810788,     0.577729 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      10.0571,      58.3157,      76.0571 ), glm.quat(    0.0320922,   -0.0789339,    -0.964779,     0.248878 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      8.02774,      53.6106,      80.5308 ), glm.quat(     0.183665,     0.597426,    -0.769471,     0.131396 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      2.66686,      55.0047,      80.6263 ), glm.quat(   -0.0740443,    -0.560941,     0.761465,    -0.316281 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(     -8.11043,      57.0454,       75.859 ), glm.quat(     0.297335,    -0.486871,     0.258247,    -0.779652 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(     -6.00359,      50.1956,      68.9853 ), glm.quat(     0.301897,    -0.485386,     0.261377,    -0.777779 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      10.2629,      53.5708,      80.6721 ), glm.quat(     -0.22297,     -0.59241,    -0.767848,     0.098717 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      16.0524,       55.262,      81.3554 ), glm.quat(     0.475579,    -0.540937,     -0.57148,    -0.393222 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      27.7812,      56.5094,      80.5862 ), glm.quat(     0.643831,     -0.27293,    -0.683958,     0.207828 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      28.9073,      64.6527,      73.8156 ), glm.quat(     0.644899,    -0.267389,    -0.688931,      0.19489 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      4.25561,      34.9653,      89.3799 ), glm.quat(   -0.0866354,    -0.983374,     0.103717,     0.121299 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(     0.900007,      17.2952,      92.9663 ), glm.quat(    -0.488232,    -0.815883,      0.19136,     0.243612 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(    -0.391913,      9.47834,      108.424 ), glm.quat(    -0.480091,    -0.820699,     0.193774,     0.241696 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      11.8044,      35.0547,      87.3401 ), glm.quat(     0.240655,    -0.959203,    -0.112873,    0.0963038 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      14.8047,       19.916,      78.8176 ), glm.quat(    -0.214131,    -0.971155,   -0.0838329,   -0.0630639 ), glm.vec3(            1,            1,            1 ), ),
+    ( glm.vec3(      17.1327,      4.58869,      86.1275 ), glm.quat(  -0.00797081,     -0.99445,   -0.0950934,   -0.0442974 ), glm.vec3(            1,            1,            1 ), ),
+]
+
 class Reading(unittest.TestCase):
     def setUp(self):
         self.instance = bvhio.readAsHierarchy('bvhio/tests/example.bvh')
-        self.joints = [ # for j, i, d in root.layout(): print(f"( {d}, {len(j.Children)}, {len(j.Keyframes)}, {j.KeyframeRange}, '{j.Name}', ),")
-            ( 0, 3, 2, (0, 1), 'Hips', ),
-            ( 1, 3, 2, (0, 1), 'Chest', ),
-            ( 2, 1, 2, (0, 1), 'Neck', ),
-            ( 3, 0, 2, (0, 1), 'Head', ),
-            ( 2, 1, 2, (0, 1), 'LeftCollar', ),
-            ( 3, 1, 2, (0, 1), 'LeftUpArm', ),
-            ( 4, 1, 2, (0, 1), 'LeftLowArm', ),
-            ( 5, 0, 2, (0, 1), 'LeftHand', ),
-            ( 2, 1, 2, (0, 1), 'RightCollar', ),
-            ( 3, 1, 2, (0, 1), 'RightUpArm', ),
-            ( 4, 1, 2, (0, 1), 'RightLowArm', ),
-            ( 5, 0, 2, (0, 1), 'RightHand', ),
-            ( 1, 1, 2, (0, 1), 'LeftUpLeg', ),
-            ( 2, 1, 2, (0, 1), 'LeftLowLeg', ),
-            ( 3, 0, 2, (0, 1), 'LeftFoot', ),
-            ( 1, 1, 2, (0, 1), 'RightUpLeg', ),
-            ( 2, 1, 2, (0, 1), 'RightLowLeg', ),
-            ( 3, 0, 2, (0, 1), 'RightFoot', ),
-        ]
-        self.restPoseLocal = [ # for j, i, d in root.layout(): print(f"( glm.{j.Position}, glm.{j.Rotation}, glm.{j.Scale}, ),")
-            ( glm.vec3(            0,            0,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         5.21,            0 ), glm.quat(     0.999333,    0.0365139,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,      18.6003,     -1.36106 ), glm.quat(     0.999333,   -0.0365139,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         5.45,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         1.12,      16.3232,     0.680562 ), glm.quat(     0.706635,   -0.0258192,   -0.0258192,    -0.706635 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3( -4.76837e-07,         5.54,            0 ), glm.quat(    -0.707107,            0,            0,     0.707107 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        11.96,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         9.93,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -1.12,      16.3232,     0.680562 ), glm.quat(     0.706635,   -0.0258192,    0.0258192,     0.706635 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(  9.53674e-07,         6.07,            0 ), glm.quat(     0.707107,            0,            0,     0.707107 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        11.82,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        10.65,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        18.34,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        17.37,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        17.63,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        17.14,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-        ]
-        self.restPoseWorld = [ # for j, i, d in root.layout(): print(f"( glm.{j.PositionWorld}, glm.{j.RotationWorld}, glm.{j.ScaleWorld}, ),")
-            ( glm.vec3(            0,            0,            0 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         5.21,            0 ), glm.quat(     0.999333,    0.0365139,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        23.86,  1.19209e-07 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        29.31,  1.19209e-07 ), glm.quat(            1,            0,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         1.12,        21.44,         1.87 ), glm.quat(     0.707107,            0,            0,    -0.707107 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         6.66,        21.44,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         6.66,         9.48,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         6.66,    -0.450002,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -1.12,        21.44,         1.87 ), glm.quat(     0.707107,            0,            0,     0.707107 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -7.19,        21.44,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -7.19,         9.62,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -7.19,        -1.03,         1.87 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         3.91,       -18.34,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         3.91,       -35.71,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -3.91,            0,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -3.91,       -17.63,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -3.91,       -34.77,            0 ), glm.quat(            0,            0,            0,            1 ), glm.vec3(            1,            1,            1 ), ),
-        ]
-        self.pose0Local = [
-            ( glm.vec3(         8.03,        35.01,        88.36 ), glm.quat(     0.131166,   -0.0117277,    -0.982546,    -0.131386 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         5.21,            0 ), glm.quat(     0.905976,     0.390515,    -0.159062,    0.0374775 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,      18.6003,     -1.36106 ), glm.quat(     0.938613,     0.338059,    0.0279395,     0.062775 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         5.45,            0 ), glm.quat(     0.933054,    -0.351756,    0.0585907,   -0.0473785 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         1.12,      16.3232,     0.680562 ), glm.quat(     0.760453,   -0.0960347,    0.0337522,    -0.641365 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3( -4.76837e-07,         5.54,            0 ), glm.quat(    -0.976203,    -0.202105,   -0.0323696,   -0.0716515 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        11.96,            0 ), glm.quat(     0.694325,     0.714836,    0.0378194,   -0.0741041 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,         9.93,            0 ), glm.quat(     0.999982, -0.000261795, -1.57639e-06,   0.00602135 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -1.12,      16.3232,     0.680562 ), glm.quat(     0.781762,    -0.100736,   -0.0338954,     0.614452 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(  9.53674e-07,         6.07,            0 ), glm.quat(     0.614408,    0.0440009,     0.778943,     0.117536 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        11.82,            0 ), glm.quat(     0.762976,     0.606189,    -0.177084,     0.138002 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        10.65,            0 ), glm.quat(     0.999888,  -0.00602318, -9.20184e-05,   -0.0136991 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(         3.91,            0,            0 ), glm.quat(    -0.117674,    -0.024446,    -0.202143,     0.971953 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        18.34,            0 ), glm.quat(     0.894013,    -0.411485,    -0.106536,     0.141674 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        17.37,            0 ), glm.quat(     0.999951,   0.00994821,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(        -3.91,            0,            0 ), glm.quat(     0.141065,   -0.0135394,    0.0944943,     0.985387 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        17.63,            0 ), glm.quat(     0.883393,      -0.4543,     0.109673,    0.0346498 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(            0,        17.14,            0 ), glm.quat(     0.978238,     0.207485,            0,            0 ), glm.vec3(            1,            1,            1 ), ),
-        ]
-        self.pose0World = [
-            ( glm.vec3(         8.03,        35.01,        88.36 ), glm.quat(     0.131166,   -0.0117277,    -0.982546,    -0.131386 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      8.32964,      40.0387,      89.6891 ), glm.quat(    -0.027949,   -0.0171246,    -0.961895,     0.271448 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      9.16411,       56.599,      81.1521 ), glm.quat(   -0.0106095,   -0.0934888,    -0.810788,     0.577729 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      10.0571,      58.3157,      76.0571 ), glm.quat(    0.0320922,   -0.0789339,    -0.964779,     0.248878 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      8.02774,      53.6106,      80.5308 ), glm.quat(     0.183665,     0.597426,    -0.769471,     0.131396 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      2.66686,      55.0047,      80.6263 ), glm.quat(   -0.0740443,    -0.560941,     0.761465,    -0.316281 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(     -8.11043,      57.0454,       75.859 ), glm.quat(     0.297335,    -0.486871,     0.258247,    -0.779652 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(     -6.00359,      50.1956,      68.9853 ), glm.quat(     0.301897,    -0.485386,     0.261377,    -0.777779 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      10.2629,      53.5708,      80.6721 ), glm.quat(     -0.22297,     -0.59241,    -0.767848,     0.098717 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      16.0524,       55.262,      81.3554 ), glm.quat(     0.475579,    -0.540937,     -0.57148,    -0.393222 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      27.7812,      56.5094,      80.5862 ), glm.quat(     0.643831,     -0.27293,    -0.683958,     0.207828 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      28.9073,      64.6527,      73.8156 ), glm.quat(     0.644899,    -0.267389,    -0.688931,      0.19489 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      4.25561,      34.9653,      89.3799 ), glm.quat(   -0.0866354,    -0.983374,     0.103717,     0.121299 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(     0.900007,      17.2952,      92.9663 ), glm.quat(    -0.488232,    -0.815883,      0.19136,     0.243612 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(    -0.391913,      9.47834,      108.424 ), glm.quat(    -0.480091,    -0.820699,     0.193774,     0.241696 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      11.8044,      35.0547,      87.3401 ), glm.quat(     0.240655,    -0.959203,    -0.112873,    0.0963038 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      14.8047,       19.916,      78.8176 ), glm.quat(    -0.214131,    -0.971155,   -0.0838329,   -0.0630639 ), glm.vec3(            1,            1,            1 ), ),
-            ( glm.vec3(      17.1327,      4.58869,      86.1275 ), glm.quat(  -0.00797081,     -0.99445,   -0.0950934,   -0.0442974 ), glm.vec3(            1,            1,            1 ), ),
-        ]
 
     def test_JointCount(self):
-        self.assertEqual(len(self.joints), len(self.instance.layout()))
+        self.assertEqual(len(Joints), len(self.instance.layout()))
 
     def test_Name(self):
         for j, i, d in self.instance.layout():
-            self.assertEqual(j.Name, self.joints[i][-1])
+            self.assertEqual(j.Name, Joints[i][-1])
 
     def test_Depth(self):
         for j, i, d in self.instance.layout():
-            self.assertEqual(d, self.joints[i][0])
+            self.assertEqual(d, Joints[i][0])
 
     def test_Children(self):
         for j, i, d in self.instance.layout():
-            self.assertEqual(len(j.Children), self.joints[i][1])
+            self.assertEqual(len(j.Children), Joints[i][1])
 
     def test_Keyframes(self):
         for j, i, d in self.instance.layout():
-            self.assertEqual(2, self.joints[i][2])
+            self.assertEqual(2, Joints[i][2])
 
     def test_KeyframeRange(self):
         for j, i, d in self.instance.layout():
-            self.assertEqual(j.getKeyframeRange(includeChildren=True), self.joints[i][3])
+            self.assertEqual(j.getKeyframeRange(includeChildren=True), Joints[i][3])
 
     def test_PositionsRestPose(self):
         for j, i, d in self.instance.loadRestPose(recursive=True).layout():
-            self.assertGreater(1e-04, deviationPosition(j.Position, self.restPoseLocal[i][0]))
-            self.assertGreater(1e-04, deviationPosition(j.PositionWorld, self.restPoseWorld[i][0]))
+            self.assertGreater(1e-04, deviationPosition(j.Position, RestPoseLocal[i][0]))
+            self.assertGreater(1e-04, deviationPosition(j.PositionWorld, RestPoseWorld[i][0]))
 
     def test_RotationsRestPose(self):
         for j, i, d in self.instance.loadRestPose(recursive=True).layout():
-            self.assertGreater(1e-06, deviationQuaternion(j.Rotation, self.restPoseLocal[i][1]))
-            self.assertGreater(1e-06, deviationQuaternion(j.RotationWorld, self.restPoseWorld[i][1]))
+            self.assertGreater(1e-06, deviationQuaternion(j.Rotation, RestPoseLocal[i][1]))
+            self.assertGreater(1e-06, deviationQuaternion(j.RotationWorld, RestPoseWorld[i][1]))
 
     def test_ScalesRestPose(self):
         for j, i, d in self.instance.loadRestPose(recursive=True).layout():
-            self.assertGreater(1e-06,  glm.length(j.Scale - self.restPoseLocal[i][2]))
-            self.assertGreater(1e-06,  glm.length(j.ScaleWorld - self.restPoseWorld[i][2]))
+            self.assertGreater(1e-06,  glm.length(j.Scale - RestPoseLocal[i][2]))
+            self.assertGreater(1e-06,  glm.length(j.ScaleWorld - RestPoseWorld[i][2]))
 
     def test_PositionsPose0(self):
         for j, i, d in self.instance.loadPose(0, recursive=True).layout():
-            self.assertGreater(1e-04, deviationPosition(j.Position, self.pose0Local[i][0]))
-            self.assertGreater(1e-03, deviationPosition(j.PositionWorld, self.pose0World[i][0]))
+            self.assertGreater(1e-04, deviationPosition(j.Position, Pose0Local[i][0]))
+            self.assertGreater(1e-03, deviationPosition(j.PositionWorld, Pose0World[i][0]))
 
     def test_RotationsPose0(self):
         for j, i, d in self.instance.loadPose(0, recursive=True).layout():
-            self.assertGreater(1e-05, deviationQuaternion(j.Rotation, self.pose0Local[i][1]))
-            self.assertGreater(1e-05, deviationQuaternion(j.RotationWorld, self.pose0World[i][1]))
+            self.assertGreater(1e-05, deviationQuaternion(j.Rotation, Pose0Local[i][1]))
+            self.assertGreater(1e-05, deviationQuaternion(j.RotationWorld, Pose0World[i][1]))
 
     def test_ScalesPose0(self):
         for j, i, d in self.instance.loadPose(0, recursive=True).layout():
-            self.assertGreater(1e-06,  glm.length(j.Scale - self.pose0Local[i][2]))
-            self.assertGreater(1e-06,  glm.length(j.ScaleWorld - self.pose0World[i][2]))
+            self.assertGreater(1e-06,  glm.length(j.Scale - Pose0Local[i][2]))
+            self.assertGreater(1e-06,  glm.length(j.ScaleWorld - Pose0World[i][2]))
 
 class Methods(unittest.TestCase):
     def test_write_read_RestPose(self):
         instance = bvhio.readAsHierarchy('bvhio/tests/example.bvh')
         instance.loadRestPose(recursive=True)
         restPose = [(joint.PositionWorld, joint.RotationWorld, joint.ScaleWorld) for joint, _ , _ in instance.layout()]
         instance.loadPose(0, recursive=True)
@@ -224,7 +225,20 @@
             instance.roll(step*5, recursive=False)
             for i, child in enumerate(instance.Children):
                 self.assertGreater(1e-04, deviationPosition(childPose[i][0], child.PositionWorld))
                 self.assertGreater(1e-04, deviationQuaternion(childPose[i][1], child.RotationWorld))
                 self.assertGreater(1e-04, deviationScale(childPose[i][2], child.ScaleWorld))
 
         self.assertTrue(True)
+
+    def test_detach(self):
+        instance = bvhio.readAsHierarchy('bvhio/tests/example.bvh')
+        leftCollar = instance.filter('LeftCollar')[0]
+        leftCollar.clearParent(keep=['position', 'rotation', 'scale', 'anim'])
+        leftCollar.loadPose(0, recursive=True)
+        instance.loadPose(0, recursive=True)
+
+        for j, i, d in leftCollar.layout():
+            i += 4
+            self.assertGreater(1e-03, deviationPosition(j.PositionWorld, Pose0World[i][0]))
+            self.assertGreater(1e-05, deviationQuaternion(j.RotationWorld, Pose0World[i][1]))
+            self.assertGreater(1e-06,  glm.length(j.ScaleWorld - Pose0World[i][2]))
```

### Comparing `bvhio-1.3.9/bvhio/tests/test_io.py` & `bvhio-1.4.0/bvhio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/bvhio/tests/utils.py` & `bvhio-1.4.0/bvhio/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/LICENSE` & `bvhio-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/README.md` & `bvhio-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bvhio-1.3.9/pyproject.toml` & `bvhio-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bvhio"
-version = "1.3.9"
+version = "1.4.0"
 authors = [ { name="Wasserwecken", email="author@example.com" }, ]
 description = "Read, write, edit and create .bvh files with hierarchical 3D transforms."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bvhio-1.3.9/PKG-INFO` & `bvhio-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bvhio
-Version: 1.3.9
+Version: 1.4.0
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
-Metadata-Version: 2.3 Name: bvhio Version: 1.3.9 Summary: Read, write, edit and
+Metadata-Version: 2.3 Name: bvhio Version: 1.4.0 Summary: Read, write, edit and
 create .bvh files with hierarchical 3D transforms. Project-URL: Homepage,
 https://github.com/Wasserwecken/bvhio Project-URL: Bug Tracker, https://
 github.com/Wasserwecken/bvhio/issues Author-email: Wasserwecken
 example.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Requires-Dist: numpy Requires-
 Dist: pyglm==2.7.1 Requires-Dist: spatial-transform==1.2.13 Description-
```

