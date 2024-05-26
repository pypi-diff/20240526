# Comparing `tmp/rimc_engine-0.5.1.tar.gz` & `tmp/rimc_engine-0.5.2.tar.gz`

## Comparing `rimc_engine-0.5.1.tar` & `rimc_engine-0.5.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     8149 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/README.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/requirements.txt
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/setup.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   112378 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsCLSC.JPG
--rw-r--r--   0        0        0   166243 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsGOLD.JPG
--rw-r--r--   0        0        0   138558 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsPOL6.JPG
--rw-r--r--   0        0        0   149411 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsPORT.JPG
--rw-r--r--   0        0        0   186508 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsSUPR.JPG
--rw-r--r--   0        0        0   141906 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsbwRE.JPG
--rw-r--r--   0        0        0   157429 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowsbwSV.JPG
--rw-r--r--   0        0        0   150602 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/cows/cowscrop.JPG
--rw-r--r--   0        0        0   118082 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillCLSC.JPG
--rw-r--r--   0        0        0   157277 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillGOLD.JPG
--rw-r--r--   0        0        0   137862 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillPOL6.JPG
--rw-r--r--   0        0        0   133546 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillPORT.JPG
--rw-r--r--   0        0        0   192364 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillSUPR.JPG
--rw-r--r--   0        0        0   125091 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillbwRE.JPG
--rw-r--r--   0        0        0   153867 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillbwSV.JPG
--rw-r--r--   0        0        0   118066 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/crosshill/crosshillcrop.JPG
--rw-r--r--   0        0        0   142734 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/oliveCLSC.JPG
--rw-r--r--   0        0        0   157708 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/oliveGOLD.JPG
--rw-r--r--   0        0        0   153395 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/olivePOL6.JPG
--rw-r--r--   0        0        0   135590 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/olivePORT.JPG
--rw-r--r--   0        0        0   188908 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/oliveSUPR.JPG
--rw-r--r--   0        0        0   128770 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/olivebwRE.JPG
--rw-r--r--   0        0        0   144246 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/olivebwSV.JPG
--rw-r--r--   0        0        0   127781 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/gallery/olive/olivecrop.JPG
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/__init__.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/convert.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/convert_temp.py
--rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/effects.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/recipes.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/test_allrec.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/test_allrecipes_plot.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/test_effects.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/src/rimc_engine/tools.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/tests/main.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/LICENSE
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/readmepypl.md
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 rimc_engine-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/README.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/requirements.txt
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/setup.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   112378 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsCLSC.JPG
+-rw-r--r--   0        0        0   166243 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsGOLD.JPG
+-rw-r--r--   0        0        0   138558 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsPOL6.JPG
+-rw-r--r--   0        0        0   149411 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsPORT.JPG
+-rw-r--r--   0        0        0   186508 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsSUPR.JPG
+-rw-r--r--   0        0        0   141906 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsbwRE.JPG
+-rw-r--r--   0        0        0   157429 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowsbwSV.JPG
+-rw-r--r--   0        0        0   150602 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/cows/cowscrop.JPG
+-rw-r--r--   0        0        0   118082 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillCLSC.JPG
+-rw-r--r--   0        0        0   157277 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillGOLD.JPG
+-rw-r--r--   0        0        0   137862 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillPOL6.JPG
+-rw-r--r--   0        0        0   133546 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillPORT.JPG
+-rw-r--r--   0        0        0   192364 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillSUPR.JPG
+-rw-r--r--   0        0        0   125091 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillbwRE.JPG
+-rw-r--r--   0        0        0   153867 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillbwSV.JPG
+-rw-r--r--   0        0        0   118066 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/crosshill/crosshillcrop.JPG
+-rw-r--r--   0        0        0   142734 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/oliveCLSC.JPG
+-rw-r--r--   0        0        0   157708 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/oliveGOLD.JPG
+-rw-r--r--   0        0        0   153395 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/olivePOL6.JPG
+-rw-r--r--   0        0        0   135590 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/olivePORT.JPG
+-rw-r--r--   0        0        0   188908 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/oliveSUPR.JPG
+-rw-r--r--   0        0        0   128770 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/olivebwRE.JPG
+-rw-r--r--   0        0        0   144246 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/olivebwSV.JPG
+-rw-r--r--   0        0        0   127781 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/gallery/olive/olivecrop.JPG
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/__init__.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/convert.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/convert_temp.py
+-rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/effects.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/recipes.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/test_allrec.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/test_allrecipes_plot.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/test_effects.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/src/rimc_engine/tools.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/tests/example.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/tests/test_origsize.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/LICENSE
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/readmepypl.md
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 rimc_engine-0.5.2/PKG-INFO
```

### Comparing `rimc_engine-0.5.1/README.md` & `rimc_engine-0.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,10 +178,11 @@
 - "portra":(3, 1, -5),
 - "gold":(4, 0, -5),
 - "superia":(4, 0.1, -3),
 - "silvertone":(-1, -0.5, 1),
 - "retro":(6, 3, -4),
 - "polaroid600":(4, 0, 6)
 
-
+# changelog
+ 26/05/24 - add keep_original_size to convert.py
```

#### html2text {}

```diff
@@ -95,8 +95,9 @@
 small shadow, which slightly reduces brightness - ["rect_strong"] :
 recognizable aged-look shadowing Type 2 - round, classic vignette -
 ["round_xlight"] : almost not recognizable - ["round_light"] : reduces
 brightness, but it's shape is still not really noticable - ["round"] :
 recognizable shape with almost no decrease in brightness #### Tints -
 "neutral":(0, 0, 0), - "brown":(8, 0, -8), - "red":(8, -4, -8), - "blue":(-8, -
 4, 4), - "portra":(3, 1, -5), - "gold":(4, 0, -5), - "superia":(4, 0.1, -3), -
-"silvertone":(-1, -0.5, 1), - "retro":(6, 3, -4), - "polaroid600":(4, 0, 6)
+"silvertone":(-1, -0.5, 1), - "retro":(6, 3, -4), - "polaroid600":(4, 0, 6) #
+changelog 26/05/24 - add keep_original_size to convert.py
```

### Comparing `rimc_engine-0.5.1/.github/workflows/python-publish.yml` & `rimc_engine-0.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsCLSC.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsCLSC.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsGOLD.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsGOLD.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsPOL6.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsPOL6.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsPORT.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsPORT.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsSUPR.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsSUPR.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsbwRE.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsbwRE.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowsbwSV.JPG` & `rimc_engine-0.5.2/gallery/cows/cowsbwSV.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/cows/cowscrop.JPG` & `rimc_engine-0.5.2/gallery/cows/cowscrop.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillCLSC.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillCLSC.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillGOLD.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillGOLD.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillPOL6.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillPOL6.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillPORT.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillPORT.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillSUPR.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillSUPR.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillbwRE.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillbwRE.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillbwSV.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillbwSV.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/crosshill/crosshillcrop.JPG` & `rimc_engine-0.5.2/gallery/crosshill/crosshillcrop.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/oliveCLSC.JPG` & `rimc_engine-0.5.2/gallery/olive/oliveCLSC.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/oliveGOLD.JPG` & `rimc_engine-0.5.2/gallery/olive/oliveGOLD.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/olivePOL6.JPG` & `rimc_engine-0.5.2/gallery/olive/olivePOL6.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/olivePORT.JPG` & `rimc_engine-0.5.2/gallery/olive/olivePORT.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/oliveSUPR.JPG` & `rimc_engine-0.5.2/gallery/olive/oliveSUPR.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/olivebwRE.JPG` & `rimc_engine-0.5.2/gallery/olive/olivebwRE.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/olivebwSV.JPG` & `rimc_engine-0.5.2/gallery/olive/olivebwSV.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/gallery/olive/olivecrop.JPG` & `rimc_engine-0.5.2/gallery/olive/olivecrop.JPG`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/src/rimc_engine/convert.py` & `rimc_engine-0.5.2/src/rimc_engine/convert_temp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from PIL import Image, ImageOps, ImageFilter, ImageEnhance
 
-from .effects import *
-from .tools import *
-from .recipes import Recipe, recipes_collection
+from effects import *
+from tools import *
+from recipes import Recipe, recipes_collection
 
 def apply(img: Image, size = (1080, 1080), 
           recipe: Recipe = recipes_collection['CLSC']) -> Image:
     """Applies effect by given recipe
     """
     img = ImageOps.exif_transpose(img)
     # Crop
```

### Comparing `rimc_engine-0.5.1/src/rimc_engine/convert_temp.py` & `rimc_engine-0.5.2/src/rimc_engine/convert.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from PIL import Image, ImageOps, ImageFilter, ImageEnhance
 
-from effects import *
-from tools import *
-from recipes import Recipe, recipes_collection
+from .effects import *
+from .tools import *
+from .recipes import Recipe, recipes_collection
 
-def apply(img: Image, size = (1080, 1080), 
+def apply(img: Image, size = (1080, 1080), keep_original_size = False,
           recipe: Recipe = recipes_collection['CLSC']) -> Image:
     """Applies effect by given recipe
     """
     img = ImageOps.exif_transpose(img)
     # Crop
-    img_contain = ImageOps.fit(img, size, centering=(0.55, 0.7))    
+    if (not keep_original_size):
+        img_contain = ImageOps.fit(img, size, centering=(0.55, 0.7))    
+    else: 
+        img_contain = img
 
     # Color
     enhancer = ImageEnhance.Color(img_contain)
     img_contain = enhancer.enhance(1 + recipe.color)
 
     # Brightness
     br = ImageEnhance.Brightness(img_contain)
@@ -50,28 +53,28 @@
     # post color
     enhancer = ImageEnhance.Color(img_contain)
     img_contain = enhancer.enhance(0.8)
         
     return img_contain
 
 def open_apply_save(name, orig_path = "orig/", out_path = "out/", 
-                    suffix="_edit", size = (1080, 1080), 
+                    suffix="_edit", size = (1080, 1080), keep_original_size = False,
                     recipe: Recipe = recipes_collection['CLSC']) -> None:
     """Opens file, applies filter, saves the file
     name:
         filename to open
     orig_path:
         where to open
     out_path:
         where to save
     suffix:
         mark outputed filename
     """      
     orig = Image.open(orig_path+name)
-    out = apply(orig, size=size, recipe=recipe)
+    out = apply(orig, size=size, recipe=recipe, keep_original_size=keep_original_size)
 
     # save        
     o = out_path+suffixname(name, suffix)
     print("Saving: ", o)
     out.save(o)
```

### Comparing `rimc_engine-0.5.1/src/rimc_engine/effects.py` & `rimc_engine-0.5.2/src/rimc_engine/effects.py`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/src/rimc_engine/recipes.py` & `rimc_engine-0.5.2/src/rimc_engine/recipes.py`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/src/rimc_engine/test_allrec.py` & `rimc_engine-0.5.2/src/rimc_engine/test_allrec.py`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/src/rimc_engine/test_allrecipes_plot.py` & `rimc_engine-0.5.2/src/rimc_engine/test_allrecipes_plot.py`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/src/rimc_engine/test_effects.py` & `rimc_engine-0.5.2/src/rimc_engine/test_effects.py`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/src/rimc_engine/tools.py` & `rimc_engine-0.5.2/src/rimc_engine/tools.py`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/tests/main.py` & `rimc_engine-0.5.2/tests/example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from rimc_engine import open_apply_save, Recipe
+from rimc_engine import open_apply_save, Recipe, recipes_collection
 import os
 from datetime import datetime
 
 
 def main():
     path = "orig/"    
     
     print(os.listdir(path))
     for f in os.listdir(path):
         if os.path.isfile(os.path.join(path, f)):
             # Get the current timestamp
             current_timestamp = round(datetime.timestamp(datetime.now())/10)
             print(current_timestamp)
-            open_apply_save(f, suffix=str(current_timestamp))
+            print(recipes_collection)
+            open_apply_save(f, suffix=str(current_timestamp), recipe=recipes_collection["GOLD"])
+            open_apply_save(f, suffix=str(current_timestamp)+"S", recipe=recipes_collection["SUPR"])
 
         
 
 if __name__ == "__main__":
     main()
```

### Comparing `rimc_engine-0.5.1/LICENSE` & `rimc_engine-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/pyproject.toml` & `rimc_engine-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rimc_engine"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Bogdan Pokrepin", email="pokrepin@gmail.com" },
 ]
 description = "Film simulation / photo processor python module."
 readme = "readmepypl.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rimc_engine-0.5.1/readmepypl.md` & `rimc_engine-0.5.2/readmepypl.md`

 * *Files identical despite different names*

### Comparing `rimc_engine-0.5.1/PKG-INFO` & `rimc_engine-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: rimc_engine
-Version: 0.5.1
+Version: 0.5.2
 Summary: Film simulation / photo processor python module.
 Project-URL: Homepage, https://github.com/bogpok/rimc_engine
 Project-URL: Bug Tracker, https://github.com/bogpok/rimc_engine/issues
 Author-email: Bogdan Pokrepin <pokrepin@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

