# Comparing `tmp/xssbase-2.0.3.tar.gz` & `tmp/xssbase-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xssbase-2.0.3.tar", last modified: Sun May 26 09:55:06 2024, max compression
+gzip compressed data, was "xssbase-2.0.4.tar", last modified: Sun May 26 10:03:31 2024, max compression
```

## Comparing `xssbase-2.0.3.tar` & `xssbase-2.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 09:55:06.645058 xssbase-2.0.3/
--rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.3/LICENSE
--rw-rw-rw-   0        0        0      774 2024-05-26 09:55:06.645058 xssbase-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-26 09:55:06.645058 xssbase-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-26 09:54:54.000000 xssbase-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:55:06.613816 xssbase-2.0.3/xssbase/
--rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.3/xssbase/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-05-26 09:45:39.000000 xssbase-2.0.3/xssbase/cli.py
--rw-rw-rw-   0        0        0     2428 2024-05-26 09:54:48.000000 xssbase-2.0.3/xssbase/main.py
--rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.3/xssbase/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-26 09:55:06.645058 xssbase-2.0.3/xssbase.egg-info/
--rw-rw-rw-   0        0        0      774 2024-05-26 09:55:06.000000 xssbase-2.0.3/xssbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-26 09:55:06.000000 xssbase-2.0.3/xssbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 09:55:06.000000 xssbase-2.0.3/xssbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-26 09:55:06.000000 xssbase-2.0.3/xssbase.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-26 09:55:06.000000 xssbase-2.0.3/xssbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-26 09:55:06.000000 xssbase-2.0.3/xssbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 10:03:31.760531 xssbase-2.0.4/
+-rw-rw-rw-   0        0        0     1065 2024-05-21 19:45:33.000000 xssbase-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0      774 2024-05-26 10:03:31.760531 xssbase-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2024-05-21 19:45:33.000000 xssbase-2.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 10:03:31.760531 xssbase-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1056 2024-05-26 10:03:14.000000 xssbase-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:03:31.738371 xssbase-2.0.4/xssbase/
+-rw-rw-rw-   0        0        0       20 2024-05-26 06:44:34.000000 xssbase-2.0.4/xssbase/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-05-26 10:03:05.000000 xssbase-2.0.4/xssbase/cli.py
+-rw-rw-rw-   0        0        0     2411 2024-05-26 10:02:40.000000 xssbase-2.0.4/xssbase/main.py
+-rw-rw-rw-   0        0        0      739 2024-05-26 09:18:29.000000 xssbase-2.0.4/xssbase/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-26 10:03:31.760531 xssbase-2.0.4/xssbase.egg-info/
+-rw-rw-rw-   0        0        0      774 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-26 10:03:31.000000 xssbase-2.0.4/xssbase.egg-info/top_level.txt
```

### Comparing `xssbase-2.0.3/LICENSE` & `xssbase-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.3/PKG-INFO` & `xssbase-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.3
+Version: 2.0.4
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xssbase-2.0.3/setup.py` & `xssbase-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xssbase',
-    version='2.0.3',
+    version='2.0.4',
     description='A professional tool for scanning XSS vulnerabilities.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://mrfidal.in/cyber-security/xssbase',
     author='Fidal',
     author_email='mrfidal@proton.me',
     license='MIT',
```

### Comparing `xssbase-2.0.3/xssbase/cli.py` & `xssbase-2.0.4/xssbase/cli.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.3/xssbase/main.py` & `xssbase-2.0.4/xssbase/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,148 +5,147 @@
 00000040: 6976 6572 2e63 6f6d 6d6f 6e2e 6b65 7973  iver.common.keys
 00000050: 2069 6d70 6f72 7420 4b65 7973 0d0a 696d   import Keys..im
 00000060: 706f 7274 2074 696d 650d 0a66 726f 6d20  port time..from 
 00000070: 7365 6c65 6e69 756d 2e63 6f6d 6d6f 6e2e  selenium.common.
 00000080: 6578 6365 7074 696f 6e73 2069 6d70 6f72  exceptions impor
 00000090: 7420 5374 616c 6545 6c65 6d65 6e74 5265  t StaleElementRe
 000000a0: 6665 7265 6e63 6545 7863 6570 7469 6f6e  ferenceException
-000000b0: 0d0a 0d0a 2320 4465 6669 6e65 2058 5353  ....# Define XSS
-000000c0: 2070 6179 6c6f 6164 7320 746f 2074 6573   payloads to tes
-000000d0: 740d 0a78 7373 5f70 6179 6c6f 6164 7320  t..xss_payloads 
-000000e0: 3d20 5b0d 0a20 2020 2022 3c73 6372 6970  = [..    "<scrip
-000000f0: 743e 616c 6572 7428 2758 5353 2729 3c2f  t>alert('XSS')</
-00000100: 7363 7269 7074 3e22 2c0d 0a20 2020 2022  script>",..    "
-00000110: 3c69 6d67 2073 7263 3d5c 226a 6176 6173  <img src=\"javas
-00000120: 6372 6970 743a 616c 6572 7428 2758 5353  cript:alert('XSS
-00000130: 2729 3b5c 223e 222c 0d0a 2020 2020 223c  ');\">",..    "<
-00000140: 7376 672f 6f6e 6c6f 6164 3d61 6c65 7274  svg/onload=alert
-00000150: 2827 5853 5327 293e 220d 0a20 2020 2023  ('XSS')>"..    #
-00000160: 2041 6464 206d 6f72 6520 7061 796c 6f61   Add more payloa
-00000170: 6473 2068 6572 650d 0a5d 0d0a 0d0a 6465  ds here..]....de
-00000180: 6620 6669 6e64 5f61 6e64 5f66 696c 6c5f  f find_and_fill_
-00000190: 696e 7075 7473 2864 7269 7665 722c 2070  inputs(driver, p
-000001a0: 6179 6c6f 6164 293a 0d0a 2020 2020 2320  ayload):..    # 
-000001b0: 4675 6e63 7469 6f6e 2074 6f20 6669 6e64  Function to find
-000001c0: 2061 6e64 2066 696c 6c20 696e 7075 7420   and fill input 
-000001d0: 656c 656d 656e 7473 2077 6974 6820 6120  elements with a 
-000001e0: 7061 796c 6f61 640d 0a20 2020 2064 6566  payload..    def
-000001f0: 2066 696c 6c5f 696e 7075 7473 2829 3a0d   fill_inputs():.
-00000200: 0a20 2020 2020 2020 2069 6e70 7574 5f65  .        input_e
-00000210: 6c65 6d65 6e74 7320 3d20 6472 6976 6572  lements = driver
-00000220: 2e66 696e 645f 656c 656d 656e 7473 2842  .find_elements(B
-00000230: 792e 5441 475f 4e41 4d45 2c20 2269 6e70  y.TAG_NAME, "inp
-00000240: 7574 2229 0d0a 2020 2020 2020 2020 666f  ut")..        fo
-00000250: 7220 696e 7075 745f 656c 656d 656e 7420  r input_element 
-00000260: 696e 2069 6e70 7574 5f65 6c65 6d65 6e74  in input_element
-00000270: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00000280: 696e 7075 745f 7479 7065 203d 2069 6e70  input_type = inp
-00000290: 7574 5f65 6c65 6d65 6e74 2e67 6574 5f61  ut_element.get_a
-000002a0: 7474 7269 6275 7465 2822 7479 7065 2229  ttribute("type")
-000002b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000002c0: 2069 6e70 7574 5f74 7970 6520 696e 205b   input_type in [
-000002d0: 226e 756d 6265 7222 2c20 2265 6d61 696c  "number", "email
-000002e0: 222c 2022 6461 7465 225d 3a0d 0a20 2020  ", "date"]:..   
-000002f0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00000300: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
-00000310: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00000320: 2020 2020 2020 2020 2069 6e70 7574 5f65           input_e
-00000330: 6c65 6d65 6e74 2e63 6c65 6172 2829 0d0a  lement.clear()..
-00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000350: 696e 7075 745f 656c 656d 656e 742e 7365  input_element.se
-00000360: 6e64 5f6b 6579 7328 7061 796c 6f61 6429  nd_keys(payload)
-00000370: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000380: 2020 696e 7075 745f 656c 656d 656e 742e    input_element.
-00000390: 7365 6e64 5f6b 6579 7328 4b65 7973 2e45  send_keys(Keys.E
-000003a0: 4e54 4552 290d 0a20 2020 2020 2020 2020  NTER)..         
-000003b0: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-000003c0: 7028 3129 2020 2320 416c 6c6f 7720 7469  p(1)  # Allow ti
-000003d0: 6d65 2066 6f72 2070 6f74 656e 7469 616c  me for potential
-000003e0: 2061 6c65 7274 2062 6f78 6573 2074 6f20   alert boxes to 
-000003f0: 6170 7065 6172 0d0a 2020 2020 2020 2020  appear..        
-00000400: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00000410: 7469 6f6e 2061 7320 653a 0d0a 2020 2020  tion as e:..    
-00000420: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00000430: 7428 6622 436f 756c 6420 6e6f 7420 6669  t(f"Could not fi
-00000440: 6c6c 2069 6e70 7574 2062 6f78 3a20 7b65  ll input box: {e
-00000450: 7d22 290d 0a0d 0a20 2020 2023 2052 6574  }")....    # Ret
-00000460: 7279 206d 6563 6861 6e69 736d 2066 6f72  ry mechanism for
-00000470: 2068 616e 646c 696e 6720 7374 616c 6520   handling stale 
-00000480: 656c 656d 656e 7420 7265 6665 7265 6e63  element referenc
-00000490: 650d 0a20 2020 2061 7474 656d 7074 7320  e..    attempts 
-000004a0: 3d20 330d 0a20 2020 2066 6f72 2061 7474  = 3..    for att
-000004b0: 656d 7074 2069 6e20 7261 6e67 6528 6174  empt in range(at
-000004c0: 7465 6d70 7473 293a 0d0a 2020 2020 2020  tempts):..      
-000004d0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000004e0: 2020 2020 6669 6c6c 5f69 6e70 7574 7328      fill_inputs(
-000004f0: 290d 0a20 2020 2020 2020 2020 2020 2062  )..            b
-00000500: 7265 616b 0d0a 2020 2020 2020 2020 6578  reak..        ex
-00000510: 6365 7074 2053 7461 6c65 456c 656d 656e  cept StaleElemen
-00000520: 7452 6566 6572 656e 6365 4578 6365 7074  tReferenceExcept
-00000530: 696f 6e3a 0d0a 2020 2020 2020 2020 2020  ion:..          
-00000540: 2020 6966 2061 7474 656d 7074 203c 2061    if attempt < a
-00000550: 7474 656d 7074 7320 2d20 313a 0d0a 2020  ttempts - 1:..  
-00000560: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00000570: 696e 7428 2253 7461 6c65 2065 6c65 6d65  int("Stale eleme
-00000580: 6e74 2072 6566 6572 656e 6365 2c20 7265  nt reference, re
-00000590: 7472 7969 6e67 2e2e 2e22 290d 0a20 2020  trying...")..   
-000005a0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-000005b0: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
-000005c0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000005e0: 7269 6e74 2822 4661 696c 6564 2061 6674  rint("Failed aft
-000005f0: 6572 2073 6576 6572 616c 2061 7474 656d  er several attem
-00000600: 7074 7320 6475 6520 746f 2073 7461 6c65  pts due to stale
-00000610: 2065 6c65 6d65 6e74 2072 6566 6572 656e   element referen
-00000620: 6365 2e22 290d 0a0d 0a64 6566 2074 6573  ce.")....def tes
-00000630: 745f 7873 735f 7061 796c 6f61 6473 2864  t_xss_payloads(d
-00000640: 7269 7665 722c 2075 726c 293a 0d0a 2020  river, url):..  
-00000650: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-00000660: 6472 6976 6572 2e67 6574 2875 726c 290d  driver.get(url).
-00000670: 0a20 2020 2020 2020 206f 7269 6769 6e61  .        origina
-00000680: 6c5f 7572 6c20 3d20 6472 6976 6572 2e63  l_url = driver.c
-00000690: 7572 7265 6e74 5f75 726c 0d0a 2020 2020  urrent_url..    
-000006a0: 2020 2020 7873 735f 666f 756e 6420 3d20      xss_found = 
-000006b0: 4661 6c73 6520 2023 2046 6c61 6720 746f  False  # Flag to
-000006c0: 2074 7261 636b 2069 6620 5853 5320 7675   track if XSS vu
-000006d0: 6c6e 6572 6162 696c 6974 7920 6973 2066  lnerability is f
-000006e0: 6f75 6e64 0d0a 0d0a 2020 2020 2020 2020  ound....        
-000006f0: 666f 7220 7061 796c 6f61 6420 696e 2078  for payload in x
-00000700: 7373 5f70 6179 6c6f 6164 733a 0d0a 2020  ss_payloads:..  
-00000710: 2020 2020 2020 2020 2020 6669 6e64 5f61            find_a
-00000720: 6e64 5f66 696c 6c5f 696e 7075 7473 2864  nd_fill_inputs(d
-00000730: 7269 7665 722c 2070 6179 6c6f 6164 290d  river, payload).
-00000740: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00000750: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
-00000760: 636b 2069 6620 5552 4c20 6368 616e 6765  ck if URL change
-00000770: 7320 6475 6520 746f 2070 6179 6c6f 6164  s due to payload
-00000780: 2069 6e6a 6563 7469 6f6e 0d0a 2020 2020   injection..    
-00000790: 2020 2020 2020 2020 6375 7272 656e 745f          current_
-000007a0: 7572 6c20 3d20 6472 6976 6572 2e63 7572  url = driver.cur
-000007b0: 7265 6e74 5f75 726c 0d0a 2020 2020 2020  rent_url..      
-000007c0: 2020 2020 2020 6966 2063 7572 7265 6e74        if current
-000007d0: 5f75 726c 2021 3d20 6f72 6967 696e 616c  _url != original
-000007e0: 5f75 726c 3a0d 0a20 2020 2020 2020 2020  _url:..         
-000007f0: 2020 2020 2020 2070 7269 6e74 2822 506f         print("Po
-00000800: 7465 6e74 6961 6c20 5853 5320 7675 6c6e  tential XSS vuln
-00000810: 6572 6162 696c 6974 7920 6465 7465 6374  erability detect
-00000820: 6564 2122 290d 0a20 2020 2020 2020 2020  ed!")..         
-00000830: 2020 2020 2020 2070 7269 6e74 2822 4f72         print("Or
-00000840: 6967 696e 616c 2055 524c 3a22 2c20 6f72  iginal URL:", or
-00000850: 6967 696e 616c 5f75 726c 290d 0a20 2020  iginal_url)..   
-00000860: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00000870: 6e74 2822 4375 7272 656e 7420 5552 4c3a  nt("Current URL:
-00000880: 222c 2063 7572 7265 6e74 5f75 726c 290d  ", current_url).
-00000890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000008a0: 2078 7373 5f66 6f75 6e64 203d 2054 7275   xss_found = Tru
-000008b0: 650d 0a0d 0a20 2020 2020 2020 2069 6620  e....        if 
-000008c0: 6e6f 7420 7873 735f 666f 756e 643a 0d0a  not xss_found:..
-000008d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-000008e0: 7428 224e 6f20 5853 5320 7675 6c6e 6572  t("No XSS vulner
-000008f0: 6162 696c 6974 7920 666f 756e 642e 2054  ability found. T
-00000900: 6865 2073 6974 6520 6d61 7920 6265 2069  he site may be i
-00000910: 6e20 676f 6f64 2068 6561 6c74 682e 2054  n good health. T
-00000920: 7279 2061 6e6f 7468 6572 2073 6974 652e  ry another site.
-00000930: 2229 0d0a 0d0a 2020 2020 6578 6365 7074  ")....    except
-00000940: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00000950: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00000960: 2245 7272 6f72 206f 6363 7572 7265 643a  "Error occurred:
-00000970: 222c 2073 7472 2865 2929 0d0a            ", str(e))..
+000000b0: 0d0a 0d0a 6465 6620 6669 6e64 5f61 6e64  ....def find_and
+000000c0: 5f66 696c 6c5f 696e 7075 7473 2864 7269  _fill_inputs(dri
+000000d0: 7665 722c 2070 6179 6c6f 6164 293a 0d0a  ver, payload):..
+000000e0: 2020 2020 2320 4675 6e63 7469 6f6e 2074      # Function t
+000000f0: 6f20 6669 6e64 2061 6e64 2066 696c 6c20  o find and fill 
+00000100: 696e 7075 7420 656c 656d 656e 7473 2077  input elements w
+00000110: 6974 6820 6120 7061 796c 6f61 640d 0a20  ith a payload.. 
+00000120: 2020 2064 6566 2066 696c 6c5f 696e 7075     def fill_inpu
+00000130: 7473 2829 3a0d 0a20 2020 2020 2020 2069  ts():..        i
+00000140: 6e70 7574 5f65 6c65 6d65 6e74 7320 3d20  nput_elements = 
+00000150: 6472 6976 6572 2e66 696e 645f 656c 656d  driver.find_elem
+00000160: 656e 7473 2842 792e 5441 475f 4e41 4d45  ents(By.TAG_NAME
+00000170: 2c20 2269 6e70 7574 2229 0d0a 2020 2020  , "input")..    
+00000180: 2020 2020 666f 7220 696e 7075 745f 656c      for input_el
+00000190: 656d 656e 7420 696e 2069 6e70 7574 5f65  ement in input_e
+000001a0: 6c65 6d65 6e74 733a 0d0a 2020 2020 2020  lements:..      
+000001b0: 2020 2020 2020 696e 7075 745f 7479 7065        input_type
+000001c0: 203d 2069 6e70 7574 5f65 6c65 6d65 6e74   = input_element
+000001d0: 2e67 6574 5f61 7474 7269 6275 7465 2822  .get_attribute("
+000001e0: 7479 7065 2229 0d0a 2020 2020 2020 2020  type")..        
+000001f0: 2020 2020 6966 2069 6e70 7574 5f74 7970      if input_typ
+00000200: 6520 696e 205b 226e 756d 6265 7222 2c20  e in ["number", 
+00000210: 2265 6d61 696c 222c 2022 6461 7465 225d  "email", "date"]
+00000220: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00000230: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
+00000240: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00000250: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00000260: 6e70 7574 5f65 6c65 6d65 6e74 2e63 6c65  nput_element.cle
+00000270: 6172 2829 0d0a 2020 2020 2020 2020 2020  ar()..          
+00000280: 2020 2020 2020 696e 7075 745f 656c 656d        input_elem
+00000290: 656e 742e 7365 6e64 5f6b 6579 7328 7061  ent.send_keys(pa
+000002a0: 796c 6f61 6429 0d0a 2020 2020 2020 2020  yload)..        
+000002b0: 2020 2020 2020 2020 696e 7075 745f 656c          input_el
+000002c0: 656d 656e 742e 7365 6e64 5f6b 6579 7328  ement.send_keys(
+000002d0: 4b65 7973 2e45 4e54 4552 290d 0a20 2020  Keys.ENTER)..   
+000002e0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+000002f0: 652e 736c 6565 7028 3129 2020 2320 416c  e.sleep(1)  # Al
+00000300: 6c6f 7720 7469 6d65 2066 6f72 2070 6f74  low time for pot
+00000310: 656e 7469 616c 2061 6c65 7274 2062 6f78  ential alert box
+00000320: 6573 2074 6f20 6170 7065 6172 0d0a 2020  es to appear..  
+00000330: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00000340: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00000350: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000360: 2020 7072 696e 7428 6622 436f 756c 6420    print(f"Could 
+00000370: 6e6f 7420 6669 6c6c 2069 6e70 7574 2062  not fill input b
+00000380: 6f78 3a20 7b65 7d22 290d 0a0d 0a20 2020  ox: {e}")....   
+00000390: 2023 2052 6574 7279 206d 6563 6861 6e69   # Retry mechani
+000003a0: 736d 2066 6f72 2068 616e 646c 696e 6720  sm for handling 
+000003b0: 7374 616c 6520 656c 656d 656e 7420 7265  stale element re
+000003c0: 6665 7265 6e63 650d 0a20 2020 2061 7474  ference..    att
+000003d0: 656d 7074 7320 3d20 330d 0a20 2020 2066  empts = 3..    f
+000003e0: 6f72 2061 7474 656d 7074 2069 6e20 7261  or attempt in ra
+000003f0: 6e67 6528 6174 7465 6d70 7473 293a 0d0a  nge(attempts):..
+00000400: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00000410: 2020 2020 2020 2020 2020 6669 6c6c 5f69            fill_i
+00000420: 6e70 7574 7328 290d 0a20 2020 2020 2020  nputs()..       
+00000430: 2020 2020 2062 7265 616b 0d0a 2020 2020       break..    
+00000440: 2020 2020 6578 6365 7074 2053 7461 6c65      except Stale
+00000450: 456c 656d 656e 7452 6566 6572 656e 6365  ElementReference
+00000460: 4578 6365 7074 696f 6e3a 0d0a 2020 2020  Exception:..    
+00000470: 2020 2020 2020 2020 6966 2061 7474 656d          if attem
+00000480: 7074 203c 2061 7474 656d 7074 7320 2d20  pt < attempts - 
+00000490: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+000004a0: 2020 2020 7072 696e 7428 2253 7461 6c65      print("Stale
+000004b0: 2065 6c65 6d65 6e74 2072 6566 6572 656e   element referen
+000004c0: 6365 2c20 7265 7472 7969 6e67 2e2e 2e22  ce, retrying..."
+000004d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000004e0: 2020 2074 696d 652e 736c 6565 7028 3129     time.sleep(1)
+000004f0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+00000500: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00000510: 2020 2020 2070 7269 6e74 2822 4661 696c       print("Fail
+00000520: 6564 2061 6674 6572 2073 6576 6572 616c  ed after several
+00000530: 2061 7474 656d 7074 7320 6475 6520 746f   attempts due to
+00000540: 2073 7461 6c65 2065 6c65 6d65 6e74 2072   stale element r
+00000550: 6566 6572 656e 6365 2e22 290d 0a0d 0a64  eference.")....d
+00000560: 6566 2074 6573 745f 7873 735f 7061 796c  ef test_xss_payl
+00000570: 6f61 6473 2864 7269 7665 722c 2075 726c  oads(driver, url
+00000580: 293a 0d0a 2020 2020 7472 793a 0d0a 2020  ):..    try:..  
+00000590: 2020 2020 2020 6472 6976 6572 2e67 6574        driver.get
+000005a0: 2875 726c 290d 0a20 2020 2020 2020 206f  (url)..        o
+000005b0: 7269 6769 6e61 6c5f 7572 6c20 3d20 6472  riginal_url = dr
+000005c0: 6976 6572 2e63 7572 7265 6e74 5f75 726c  iver.current_url
+000005d0: 0d0a 2020 2020 2020 2020 7873 735f 666f  ..        xss_fo
+000005e0: 756e 6420 3d20 4661 6c73 6520 2023 2046  und = False  # F
+000005f0: 6c61 6720 746f 2074 7261 636b 2069 6620  lag to track if 
+00000600: 5853 5320 7675 6c6e 6572 6162 696c 6974  XSS vulnerabilit
+00000610: 7920 6973 2066 6f75 6e64 0d0a 0d0a 2020  y is found....  
+00000620: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00000630: 2270 6179 6c6f 6164 732e 7478 7422 2920  "payloads.txt") 
+00000640: 6173 2066 3a0d 0a20 2020 2020 2020 2020  as f:..         
+00000650: 2020 2070 6179 6c6f 6164 7320 3d20 662e     payloads = f.
+00000660: 7265 6164 2829 2e73 706c 6974 6c69 6e65  read().splitline
+00000670: 7328 290d 0a0d 0a20 2020 2020 2020 2066  s()....        f
+00000680: 6f72 2070 6179 6c6f 6164 2069 6e20 7061  or payload in pa
+00000690: 796c 6f61 6473 3a0d 0a20 2020 2020 2020  yloads:..       
+000006a0: 2020 2020 2066 696e 645f 616e 645f 6669       find_and_fi
+000006b0: 6c6c 5f69 6e70 7574 7328 6472 6976 6572  ll_inputs(driver
+000006c0: 2c20 7061 796c 6f61 6429 0d0a 2020 2020  , payload)..    
+000006d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000006e0: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
+000006f0: 2055 524c 2063 6861 6e67 6573 2064 7565   URL changes due
+00000700: 2074 6f20 7061 796c 6f61 6420 696e 6a65   to payload inje
+00000710: 6374 696f 6e0d 0a20 2020 2020 2020 2020  ction..         
+00000720: 2020 2063 7572 7265 6e74 5f75 726c 203d     current_url =
+00000730: 2064 7269 7665 722e 6375 7272 656e 745f   driver.current_
+00000740: 7572 6c0d 0a20 2020 2020 2020 2020 2020  url..           
+00000750: 2069 6620 6375 7272 656e 745f 7572 6c20   if current_url 
+00000760: 213d 206f 7269 6769 6e61 6c5f 7572 6c3a  != original_url:
+00000770: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000780: 2020 7072 696e 7428 2250 6f74 656e 7469    print("Potenti
+00000790: 616c 2058 5353 2076 756c 6e65 7261 6269  al XSS vulnerabi
+000007a0: 6c69 7479 2064 6574 6563 7465 6421 2229  lity detected!")
+000007b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000007c0: 2020 7072 696e 7428 224f 7269 6769 6e61    print("Origina
+000007d0: 6c20 5552 4c3a 222c 206f 7269 6769 6e61  l URL:", origina
+000007e0: 6c5f 7572 6c29 0d0a 2020 2020 2020 2020  l_url)..        
+000007f0: 2020 2020 2020 2020 7072 696e 7428 2243          print("C
+00000800: 7572 7265 6e74 2055 524c 3a22 2c20 6375  urrent URL:", cu
+00000810: 7272 656e 745f 7572 6c29 0d0a 2020 2020  rrent_url)..    
+00000820: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000830: 7428 290d 0a0d 0a20 2020 2020 2020 2020  t()....         
+00000840: 2020 2020 2020 2078 7373 5f66 6f75 6e64         xss_found
+00000850: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+00000860: 2020 2020 2020 2020 2062 7265 616b 2020           break  
+00000870: 2320 4164 6420 6272 6561 6b20 6865 7265  # Add break here
+00000880: 2074 6f20 7374 6f70 2061 6674 6572 2066   to stop after f
+00000890: 696e 6469 6e67 2066 6972 7374 2058 5353  inding first XSS
+000008a0: 0d0a 0d0a 2020 2020 2020 2020 6966 206e  ....        if n
+000008b0: 6f74 2078 7373 5f66 6f75 6e64 3a0d 0a20  ot xss_found:.. 
+000008c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000008d0: 2822 4e6f 2058 5353 2076 756c 6e65 7261  ("No XSS vulnera
+000008e0: 6269 6c69 7479 2066 6f75 6e64 2e20 5468  bility found. Th
+000008f0: 6520 7369 7465 206d 6179 2062 6520 696e  e site may be in
+00000900: 2067 6f6f 6420 6865 616c 7468 2e20 5472   good health. Tr
+00000910: 7920 616e 6f74 6865 7220 7369 7465 2e22  y another site."
+00000920: 290d 0a0d 0a20 2020 2065 7863 6570 7420  )....    except 
+00000930: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
+00000940: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00000950: 4572 726f 7220 6f63 6375 7272 6564 3a22  Error occurred:"
+00000960: 2c20 7374 7228 6529 290d 0a              , str(e))..
```

### Comparing `xssbase-2.0.3/xssbase/utils.py` & `xssbase-2.0.4/xssbase/utils.py`

 * *Files identical despite different names*

### Comparing `xssbase-2.0.3/xssbase.egg-info/PKG-INFO` & `xssbase-2.0.4/xssbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xssbase
-Version: 2.0.3
+Version: 2.0.4
 Summary: A professional tool for scanning XSS vulnerabilities.
 Home-page: https://mrfidal.in/cyber-security/xssbase
 Author: Fidal
 Author-email: mrfidal@proton.me
 License: MIT
 Keywords: xssbase,xss,vulnerability,scanning,mrfidal
 Classifier: Development Status :: 5 - Production/Stable
```

