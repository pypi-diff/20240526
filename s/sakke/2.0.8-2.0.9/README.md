# Comparing `tmp/sakke-2.0.8-py3-none-any.whl.zip` & `tmp/sakke-2.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 21401 bytes, number of entries: 10
--rw-r--r--  2.0 unx       44 b- defN 22-Dec-26 09:40 sakke/__init__.py
--rw-r--r--  2.0 unx    18887 b- defN 22-Dec-26 09:37 sakke/sakke.py
+-rw-r--r--  2.0 unx       44 b- defN 22-Dec-26 17:44 sakke/__init__.py
+-rw-r--r--  2.0 unx    18891 b- defN 22-Dec-26 17:42 sakke/sakke.py
 -rw-r--r--  2.0 unx     2357 b- defN 22-Dec-26 08:28 sakke/templates/stats.html.j2
 -rw-r--r--  2.0 unx     1199 b- defN 22-Dec-26 08:28 sakke/templates/stats.tex.j2
--rw-r--r--  2.0 unx    35141 b- defN 22-Dec-26 09:40 sakke-2.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      445 b- defN 22-Dec-26 09:40 sakke-2.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-26 09:40 sakke-2.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 22-Dec-26 09:40 sakke-2.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 22-Dec-26 09:40 sakke-2.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      783 b- defN 22-Dec-26 09:40 sakke-2.0.8.dist-info/RECORD
-10 files, 58997 bytes uncompressed, 20069 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx    35141 b- defN 22-Dec-26 17:44 sakke-2.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      445 b- defN 22-Dec-26 17:44 sakke-2.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Dec-26 17:44 sakke-2.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 22-Dec-26 17:44 sakke-2.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 22-Dec-26 17:44 sakke-2.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      783 b- defN 22-Dec-26 17:44 sakke-2.0.9.dist-info/RECORD
+10 files, 59001 bytes uncompressed, 20069 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sakke/templates/stats.html.j2
 Comment: 
 
 Filename: sakke/templates/stats.tex.j2
 Comment: 
 
-Filename: sakke-2.0.8.dist-info/LICENSE
+Filename: sakke-2.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: sakke-2.0.8.dist-info/METADATA
+Filename: sakke-2.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sakke-2.0.8.dist-info/WHEEL
+Filename: sakke-2.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sakke-2.0.8.dist-info/entry_points.txt
+Filename: sakke-2.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: sakke-2.0.8.dist-info/top_level.txt
+Filename: sakke-2.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sakke-2.0.8.dist-info/RECORD
+Filename: sakke-2.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sakke/__init__.py

```diff
@@ -1,2 +1,2 @@
 # -*- coding: utf-8 -
-__version__ = "2.0.8"
+__version__ = "2.0.9"
```

## sakke/sakke.py

```diff
@@ -358,15 +358,15 @@
 
     entete_par_eleve = {}
     for student in students:
         entete_par_eleve[student] = dict(
             nom_devoir=f"{metadata['nom_devoir']}",
             nom=f"{' '.join(student)}",
             rang=f"rang: {devoir_par_eleve.loc[student][LABEL_RANG]:.0f}",
-            note=f"note: {devoir_par_eleve.loc[student][LABEL_TRANSFORM]:.2f}",
+            note=f"note: {devoir_par_eleve.loc[student][LABEL_NORMALISATION]:.2f}",
             moyenne=f"moyenne: {metadata['moyenne']:.2f}",
             ecart_type=f"écart-type: {metadata['ecart_type']:.2f}",
         )
 
     # on créé le répertoire de sortie
     output_dir = Path(outdir)
     output_dir.mkdir(parents=True, exist_ok=True)
```

## Comparing `sakke-2.0.8.dist-info/LICENSE` & `sakke-2.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sakke-2.0.8.dist-info/RECORD` & `sakke-2.0.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-sakke/__init__.py,sha256=xgcnktQo9UxSproQDQq9Bj7mu213qGh_IHELTKAxRE8,44
-sakke/sakke.py,sha256=IzANkdyrSZfFm7j2ryhShLmva0oV_7NeHfsayxkOwcw,18887
+sakke/__init__.py,sha256=utJJU0vmAnvcppVIoW4HdV-c9aIWKemqz5B7t3X-WqI,44
+sakke/sakke.py,sha256=qFIVQgjwHE41UxrhFPAbHDogy4FZlYg01KsyQPhP9X0,18891
 sakke/templates/stats.html.j2,sha256=DEN_WjMSlEmSHFI5ooT8bBPgIsGdHq0kZzVM6q99V8U,2357
 sakke/templates/stats.tex.j2,sha256=v6AlH49M894RtfsYtGxgF3C7_BaJ4Fa9dNQVjDIp8CE,1199
-sakke-2.0.8.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
-sakke-2.0.8.dist-info/METADATA,sha256=Mr_Li_HVovV8_rd9uunQkLUsCYb2n4sm6oKo5NmYygk,445
-sakke-2.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-sakke-2.0.8.dist-info/entry_points.txt,sha256=Q6v7SD34dKiDS-Wf99Zsmot1gPvF8wVA7sBOzRM9c-Y,43
-sakke-2.0.8.dist-info/top_level.txt,sha256=vJj98_iGXRfcL6ZQJ34f_fxoahqUzdT3dP9u2BhJj9Q,6
-sakke-2.0.8.dist-info/RECORD,,
+sakke-2.0.9.dist-info/LICENSE,sha256=WJ7YI-moTFb-uVrFjnzzhGJrnL9P2iqQe8NuED3hutI,35141
+sakke-2.0.9.dist-info/METADATA,sha256=LDGBi8MpdS0RmJfj_d-_z_7M9vkWvewy78JvjSz68Ks,445
+sakke-2.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+sakke-2.0.9.dist-info/entry_points.txt,sha256=Q6v7SD34dKiDS-Wf99Zsmot1gPvF8wVA7sBOzRM9c-Y,43
+sakke-2.0.9.dist-info/top_level.txt,sha256=vJj98_iGXRfcL6ZQJ34f_fxoahqUzdT3dP9u2BhJj9Q,6
+sakke-2.0.9.dist-info/RECORD,,
```

