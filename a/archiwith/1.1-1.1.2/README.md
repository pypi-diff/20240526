# Comparing `tmp/archiwith-1.1.tar.gz` & `tmp/archiwith-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archiwith-1.1.tar", last modified: Tue May 21 06:23:28 2024, max compression
+gzip compressed data, was "archiwith-1.1.2.tar", last modified: Sun May 26 07:23:03 2024, max compression
```

## Comparing `archiwith-1.1.tar` & `archiwith-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:23:28.705295 archiwith-1.1/
--rw-r--r--   0 nicospok   (501) staff       (20)     8196 2024-05-21 06:19:40.000000 archiwith-1.1/.DS_Store
--rw-r--r--   0 nicospok   (501) staff       (20)       44 2024-05-15 05:39:58.000000 archiwith-1.1/.gitignore
--rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:58.000000 archiwith-1.1/LICENSE
--rw-r--r--   0 nicospok   (501) staff       (20)     2212 2024-05-21 06:23:28.704588 archiwith-1.1/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)     1753 2024-05-15 05:39:58.000000 archiwith-1.1/README.md
-drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-21 06:23:28.703786 archiwith-1.1/archiwith.egg-info/
--rw-r--r--   0 nicospok   (501) staff       (20)     2212 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/PKG-INFO
--rw-r--r--   0 nicospok   (501) staff       (20)      179 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/SOURCES.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/dependency_links.txt
--rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-21 06:23:28.000000 archiwith-1.1/archiwith.egg-info/top_level.txt
--rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-21 06:23:28.705511 archiwith-1.1/setup.cfg
--rw-r--r--   0 nicospok   (501) staff       (20)      648 2024-05-21 06:20:33.000000 archiwith-1.1/setup.py
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-26 07:23:03.368749 archiwith-1.1.2/
+-rw-r--r--   0 nicospok   (501) staff       (20)     8196 2024-05-26 07:19:32.000000 archiwith-1.1.2/.DS_Store
+-rw-r--r--   0 nicospok   (501) staff       (20)       44 2024-05-15 05:39:58.000000 archiwith-1.1.2/.gitignore
+-rw-r--r--   0 nicospok   (501) staff       (20)     1066 2024-05-15 05:39:58.000000 archiwith-1.1.2/LICENSE
+-rw-r--r--   0 nicospok   (501) staff       (20)     2214 2024-05-26 07:23:03.367398 archiwith-1.1.2/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)     1753 2024-05-15 05:39:58.000000 archiwith-1.1.2/README.md
+drwxr-xr-x   0 nicospok   (501) staff       (20)        0 2024-05-26 07:23:03.365904 archiwith-1.1.2/archiwith.egg-info/
+-rw-r--r--   0 nicospok   (501) staff       (20)     2214 2024-05-26 07:23:02.000000 archiwith-1.1.2/archiwith.egg-info/PKG-INFO
+-rw-r--r--   0 nicospok   (501) staff       (20)      179 2024-05-26 07:23:03.000000 archiwith-1.1.2/archiwith.egg-info/SOURCES.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-26 07:23:02.000000 archiwith-1.1.2/archiwith.egg-info/dependency_links.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)        1 2024-05-26 07:23:02.000000 archiwith-1.1.2/archiwith.egg-info/top_level.txt
+-rw-r--r--   0 nicospok   (501) staff       (20)       38 2024-05-26 07:23:03.369070 archiwith-1.1.2/setup.cfg
+-rw-r--r--   0 nicospok   (501) staff       (20)      650 2024-05-26 07:21:32.000000 archiwith-1.1.2/setup.py
```

### Comparing `archiwith-1.1/.DS_Store` & `archiwith-1.1.2/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -263,79 +263,79 @@
 00001060: 9cf3 372e 53f8 c541 0000 0004 002e 0067  ..7.S..A.......g
 00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
 00001080: 0002 6000 0000 0009 0061 0072 0063 0068  ..`......a.r.c.h
 00001090: 0069 0077 0069 0074 0068 496c 6f63 626c  .i.w.i.t.hIlocbl
 000010a0: 6f62 0000 0010 0000 011d 0000 002e ffff  ob..............
 000010b0: ffff ffff 0000 0000 0009 0061 0072 0063  ...........a.r.c
 000010c0: 0068 0069 0077 0069 0074 0068 6277 7370  .h.i.w.i.t.hbwsp
-000010d0: 626c 6f62 0000 00b6 6270 6c69 7374 3030  blob....bplist00
+000010d0: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
 000010e0: d601 0203 0405 0607 0709 070b 075d 5368  .............]Sh
 000010f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001100: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001110: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00001120: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00001130: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001140: 6261 7209 0908 095f 1016 7b7b 3634 2c20  bar...._..{{64, 
-00001150: 3538 7d2c 207b 3931 302c 2037 3033 7d7d  58}, {910, 703}}
-00001160: 0908 1523 2f3b 525f 6b6c 6d6e 6f88 0000  ...#/;R_klmno...
-00001170: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-00001180: 0000 0000 0000 0000 0000 0000 0089 0000  ................
-00001190: 0009 0061 0072 0063 0068 0069 0077 0069  ...a.r.c.h.i.w.i
-000011a0: 0074 0068 7653 726e 6c6f 6e67 0000 0001  .t.hvSrnlong....
-000011b0: 0000 0012 0061 0072 0063 0068 0069 0077  .....a.r.c.h.i.w
-000011c0: 0069 0074 0068 002e 0065 0067 0067 002d  .i.t.h...e.g.g.-
-000011d0: 0069 006e 0066 006f 496c 6f63 626c 6f62  .i.n.f.oIlocblob
-000011e0: 0000 0010 0000 018b 0000 002e ffff ffff  ................
-000011f0: ffff 0000 0000 0012 0061 0072 0063 0068  .........a.r.c.h
-00001200: 0069 0077 0069 0074 0068 002e 0065 0067  .i.w.i.t.h...e.g
-00001210: 0067 002d 0069 006e 0066 006f 6277 7370  .g.-.i.n.f.obwsp
-00001220: 626c 6f62 0000 00b6 6270 6c69 7374 3030  blob....bplist00
-00001230: d601 0203 0405 0607 0709 070b 075d 5368  .............]Sh
-00001240: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00001250: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00001260: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00001270: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00001280: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001290: 6261 7209 0908 095f 1016 7b7b 332c 2031  bar...._..{{3, 1
-000012a0: 3037 7d2c 207b 3931 302c 2037 3033 7d7d  07}, {910, 703}}
-000012b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f88 0000  ...#/;R_klmno...
-000012c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-000012d0: 0000 0000 0000 0000 0000 0000 0089 0000  ................
-000012e0: 0012 0061 0072 0063 0068 0069 0077 0069  ...a.r.c.h.i.w.i
-000012f0: 0074 0068 002e 0065 0067 0067 002d 0069  .t.h...e.g.g.-.i
-00001300: 006e 0066 006f 7653 726e 6c6f 6e67 0000  .n.f.ovSrnlong..
-00001310: 0001 0000 0005 0062 0075 0069 006c 0064  .......b.u.i.l.d
-00001320: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
-00001330: 0000 002e ffff ffff ffff 0000 0000 0005  ................
-00001340: 0062 0075 0069 006c 0064 6277 7370 626c  .b.u.i.l.dbwspbl
-00001350: 6f62 0000 00b6 6270 6c69 7374 3030 d601  ob....bplist00..
-00001360: 0203 0405 0607 0709 070b 075d 5368 6f77  ...........]Show
-00001370: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-00001380: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001390: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-000013a0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-000013b0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-000013c0: 7209 0908 095f 1016 7b7b 332c 2031 3037  r...._..{{3, 107
-000013d0: 7d2c 207b 3931 302c 2037 3033 7d7d 0908  }, {910, 703}}..
-000013e0: 1523 2f3b 525f 6b6c 6d6e 6f88 0000 0000  .#/;R_klmno.....
-000013f0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00001400: 0000 0000 0000 0000 0000 0089 0000 0005  ................
-00001410: 0062 0075 0069 006c 0064 7653 726e 6c6f  .b.u.i.l.dvSrnlo
-00001420: 6e67 0000 0001 0000 0004 0064 0069 0073  ng.........d.i.s
-00001430: 0074 496c 6f63 626c 6f62 0000 0010 0000  .tIlocblob......
-00001440: 0267 0000 002e ffff ffff ffff 0000 0000  .g..............
-00001450: 0007 004c 0049 0043 0045 004e 0053 0045  ...L.I.C.E.N.S.E
-00001460: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
-00001470: 0000 002e ffff ffff ffff 0000 0000 0009  ................
-00001480: 0052 0045 0041 0044 004d 0045 002e 006d  .R.E.A.D.M.E...m
-00001490: 0064 496c 6f63 626c 6f62 0000 0010 0000  .dIlocblob......
-000014a0: 00af 0000 002e ffff ffff ffff 0000 0000  ................
-000014b0: 0008 0073 0065 0074 0075 0070 002e 0070  ...s.e.t.u.p...p
-000014c0: 0079 496c 6f63 626c 6f62 0000 0010 0000  .yIlocblob......
-000014d0: 0041 0000 009e ffff ffff ffff 0000 0000  .A..............
+00001140: 6261 7209 0908 095f 1019 7b7b 3338 352c  bar...._..{{385,
+00001150: 2031 3333 7d2c 207b 3130 3530 2c20 3730   133}, {1050, 70
+00001160: 387d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  8}}...#/;R_klmno
+00001170: 8b00 0000 0000 0001 0100 0000 0000 0000  ................
+00001180: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+00001190: 8c00 0000 0900 6100 7200 6300 6800 6900  ......a.r.c.h.i.
+000011a0: 7700 6900 7400 6876 5372 6e6c 6f6e 6700  w.i.t.hvSrnlong.
+000011b0: 0000 0100 0000 1200 6100 7200 6300 6800  ........a.r.c.h.
+000011c0: 6900 7700 6900 7400 6800 2e00 6500 6700  i.w.i.t.h...e.g.
+000011d0: 6700 2d00 6900 6e00 6600 6f49 6c6f 6362  g.-.i.n.f.oIlocb
+000011e0: 6c6f 6200 0000 1000 0001 8b00 0000 2eff  lob.............
+000011f0: ffff ffff ff00 0000 0000 1200 6100 7200  ............a.r.
+00001200: 6300 6800 6900 7700 6900 7400 6800 2e00  c.h.i.w.i.t.h...
+00001210: 6500 6700 6700 2d00 6900 6e00 6600 6f62  e.g.g.-.i.n.f.ob
+00001220: 7773 7062 6c6f 6200 0000 b662 706c 6973  wspblob....bplis
+00001230: 7430 30d6 0102 0304 0506 0707 0907 0b07  t00.............
+00001240: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00001250: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00001260: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00001270: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00001280: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+00001290: 6964 6562 6172 0909 0809 5f10 167b 7b33  idebar...._..{{3
+000012a0: 2c20 3130 377d 2c20 7b39 3130 2c20 3730  , 107}, {910, 70
+000012b0: 337d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  3}}...#/;R_klmno
+000012c0: 8800 0000 0000 0001 0100 0000 0000 0000  ................
+000012d0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+000012e0: 8900 0000 1200 6100 7200 6300 6800 6900  ......a.r.c.h.i.
+000012f0: 7700 6900 7400 6800 2e00 6500 6700 6700  w.i.t.h...e.g.g.
+00001300: 2d00 6900 6e00 6600 6f76 5372 6e6c 6f6e  -.i.n.f.ovSrnlon
+00001310: 6700 0000 0100 0000 0500 6200 7500 6900  g.........b.u.i.
+00001320: 6c00 6449 6c6f 6362 6c6f 6200 0000 1000  l.dIlocblob.....
+00001330: 0001 f900 0000 2eff ffff ffff ff00 0000  ................
+00001340: 0000 0500 6200 7500 6900 6c00 6462 7773  ....b.u.i.l.dbws
+00001350: 7062 6c6f 6200 0000 b662 706c 6973 7430  pblob....bplist0
+00001360: 30d6 0102 0304 0506 0707 0907 0b07 5d53  0.............]S
+00001370: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+00001380: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00001390: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+000013a0: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+000013b0: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+000013c0: 6562 6172 0909 0809 5f10 167b 7b33 2c20  ebar...._..{{3, 
+000013d0: 3130 377d 2c20 7b39 3130 2c20 3730 337d  107}, {910, 703}
+000013e0: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8800  }...#/;R_klmno..
+000013f0: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+00001400: 0000 0000 0000 0000 0000 0000 0000 8900  ................
+00001410: 0000 0500 6200 7500 6900 6c00 6476 5372  ....b.u.i.l.dvSr
+00001420: 6e6c 6f6e 6700 0000 0100 0000 0400 6400  nlong.........d.
+00001430: 6900 7300 7449 6c6f 6362 6c6f 6200 0000  i.s.tIlocblob...
+00001440: 1000 0002 6700 0000 2eff ffff ffff ff00  ....g...........
+00001450: 0000 0000 0700 4c00 4900 4300 4500 4e00  ......L.I.C.E.N.
+00001460: 5300 4549 6c6f 6362 6c6f 6200 0000 1000  S.EIlocblob.....
+00001470: 0000 4100 0000 2eff ffff ffff ff00 0000  ..A.............
+00001480: 0000 0900 5200 4500 4100 4400 4d00 4500  ....R.E.A.D.M.E.
+00001490: 2e00 6d00 6449 6c6f 6362 6c6f 6200 0000  ..m.dIlocblob...
+000014a0: 1000 0000 af00 0000 2eff ffff ffff ff00  ................
+000014b0: 0000 0000 0800 7300 6500 7400 7500 7000  ......s.e.t.u.p.
+000014c0: 2e00 7000 7949 6c6f 6362 6c6f 6200 0000  ..p.yIlocblob...
+000014d0: 1000 0000 4100 0000 9eff ffff ffff ff00  ....A...........
 000014e0: 0000 0001 2000 0000 0000 0001 4000 0000  .... .......@...
 000014f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `archiwith-1.1/LICENSE` & `archiwith-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `archiwith-1.1/PKG-INFO` & `archiwith-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archiwith
-Version: 1.1
+Version: 1.1.2
 Summary: File opener and closener when managed via `with`.
 Home-page: https://github.com/niCodeLine/archiwith
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `archiwith-1.1/README.md` & `archiwith-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `archiwith-1.1/archiwith.egg-info/PKG-INFO` & `archiwith-1.1.2/archiwith.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archiwith
-Version: 1.1
+Version: 1.1.2
 Summary: File opener and closener when managed via `with`.
 Home-page: https://github.com/niCodeLine/archiwith
 Author: Nico Spok
 Author-email: nicospok@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `archiwith-1.1/setup.py` & `archiwith-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='archiwith',
-    version='1.1',
+    version='1.1.2',
     packages=find_packages(),
     description='File opener and closener when managed via `with`.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/niCodeLine/archiwith',
     author='Nico Spok',
     author_email='nicospok@hotmail.com',
```

