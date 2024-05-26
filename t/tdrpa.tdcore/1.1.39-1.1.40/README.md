# Comparing `tmp/tdrpa.tdcore-1.1.39-py39-none-win_amd64.whl.zip` & `tmp/tdrpa.tdcore-1.1.40-py39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 509266 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat   642560 b- defN 24-May-22 14:07 tdrpa/bot.exe
--rw-rw-rw-  2.0 fat   615936 b- defN 24-May-22 14:08 tdrpa/tdcore.cp39-win_amd64.pyd
+Zip file size: 509587 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat   642560 b- defN 24-May-26 01:51 tdrpa/bot.exe
+-rw-rw-rw-  2.0 fat   616960 b- defN 24-May-26 01:51 tdrpa/tdcore.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat      353 b- defN 24-May-22 13:57 tdrpa/tdcore/__init__.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-19 00:55 tdrpa/tdcore/locator/__init__.pyi
 -rw-rw-rw-  2.0 fat      265 b- defN 24-May-19 00:59 tdrpa/tdcore/locator/locatorWindows.pyi
 -rw-rw-rw-  2.0 fat      264 b- defN 24-May-19 00:59 tdrpa/tdcore/locator/tdObject.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-19 00:55 tdrpa/tdcore/log/__init__.pyi
 -rw-rw-rw-  2.0 fat      130 b- defN 24-May-19 00:55 tdrpa/tdcore/log/log.pyi
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-19 00:55 tdrpa/tdcore/util/__init__.pyi
@@ -12,12 +12,12 @@
 -rw-rw-rw-  2.0 fat    11357 b- defN 23-Jan-16 01:15 tdrpa/tdcore-license/LICENSE
 -rw-rw-rw-  2.0 fat     1473 b- defN 23-Sep-05 03:08 tdrpa/tdcore-license/infi.systray/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1548 b- defN 23-Sep-05 03:10 tdrpa/tdcore-license/psutil/LICENSE.txt
 -rw-rw-rw-  2.0 fat     7656 b- defN 24-May-18 00:04 tdrpa/tdcore-license/pynput/COPYING.LGPL
 -rw-rw-rw-  2.0 fat    10142 b- defN 23-Sep-05 03:11 tdrpa/tdcore-license/requests/LICENSE.txt
 -rw-rw-rw-  2.0 fat     1060 b- defN 23-Sep-05 03:12 tdrpa/tdcore-license/tzlocal/LICENSE.txt
 -rw-rw-rw-  2.0 fat    11336 b- defN 23-Sep-05 03:13 tdrpa/tdcore-license/uiautomation/LICENSE.txt
--rw-rw-rw-  2.0 fat      612 b- defN 24-May-22 14:08 tdrpa.tdcore-1.1.39.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 14:08 tdrpa.tdcore-1.1.39.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-22 14:08 tdrpa.tdcore-1.1.39.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1844 b- defN 24-May-22 14:08 tdrpa.tdcore-1.1.39.dist-info/RECORD
-21 files, 1306698 bytes uncompressed, 506218 bytes compressed:  61.3%
+-rw-rw-rw-  2.0 fat      612 b- defN 24-May-26 01:51 tdrpa.tdcore-1.1.40.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 01:51 tdrpa.tdcore-1.1.40.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-26 01:51 tdrpa.tdcore-1.1.40.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1844 b- defN 24-May-26 01:51 tdrpa.tdcore-1.1.40.dist-info/RECORD
+21 files, 1307722 bytes uncompressed, 506539 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: tdrpa/tdcore-license/tzlocal/LICENSE.txt
 Comment: 
 
 Filename: tdrpa/tdcore-license/uiautomation/LICENSE.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.39.dist-info/METADATA
+Filename: tdrpa.tdcore-1.1.40.dist-info/METADATA
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.39.dist-info/WHEEL
+Filename: tdrpa.tdcore-1.1.40.dist-info/WHEEL
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.39.dist-info/top_level.txt
+Filename: tdrpa.tdcore-1.1.40.dist-info/top_level.txt
 Comment: 
 
-Filename: tdrpa.tdcore-1.1.39.dist-info/RECORD
+Filename: tdrpa.tdcore-1.1.40.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdrpa/bot.exe

### objdump

```diff
@@ -6,15 +6,15 @@
 Characteristics 0x22e
 	executable
 	line numbers stripped
 	symbols stripped
 	large address aware
 	debugging information removed
 
-Time/Date		Wed May 22 14:07:39 2024
+Time/Date		Sun May 26 01:51:22 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	41
 SizeOfCode		0000000000079600
 SizeOfInitializedData	000000000009ca00
 SizeOfUninitializedData	0000000000003400
 AddressOfEntryPoint	00000000000010f6
@@ -27,15 +27,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		000a8000
 SizeOfHeaders		00000400
-CheckSum		00097d21
+CheckSum		00091695
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000968000
 SizeOfStackCommit	0000000000001000
@@ -184563,19 +184563,19 @@
    1400a65e6:	rex.WRXB add %r8b,(%r8)
    1400a65e9:	add    %al,(%rax)
    1400a65eb:	add    %bh,0xfeef04(%rbp)
    1400a65f1:	add    %al,(%rax)
    1400a65f3:	add    %al,(%rcx)
    1400a65f5:	add    %al,(%rcx)
    1400a65f7:	add    %al,(%rax)
-   1400a65f9:	add    %ah,(%rdi)
+   1400a65f9:	add    %ch,(%rax)
    1400a65fb:	add    %al,(%rcx)
    1400a65fd:	add    %al,(%rcx)
    1400a65ff:	add    %al,(%rax)
-   1400a6601:	add    %ah,(%rdi)
+   1400a6601:	add    %ch,(%rax)
    1400a6603:	add    %bh,(%rdi)
    1400a6605:	add    %al,(%rax)
    1400a6607:	add    %al,(%rax)
    1400a6609:	add    %al,(%rax)
    1400a660b:	add    %al,(%rax,%rax,1)
    1400a660e:	add    %al,(%rax)
    1400a6610:	add    %eax,(%rax)
@@ -184656,18 +184656,17 @@
    1400a66cc:	jb     0x1400a66ce
    1400a66ce:	jae    0x1400a66d0
    1400a66d0:	imul   $0x6e006f,(%rax),%eax
    1400a66d6:	add    %al,(%rax)
    1400a66d8:	xor    %eax,(%rax)
    1400a66da:	cs add %dh,(%rcx)
    1400a66dd:	add    %ch,(%rsi)
-   1400a66df:	add    %dh,(%rbx)
-   1400a66e1:	add    %bh,(%rcx)
-   1400a66e3:	add    %ch,(%rsi)
-   1400a66e5:	add    %dh,(%rax)
+   1400a66df:	add    %dh,(%rax,%rax,1)
+   1400a66e2:	xor    %al,(%rax)
+   1400a66e4:	cs add %dh,(%rax)
    1400a66e7:	add    %al,(%rax)
    1400a66e9:	add    %al,(%rax)
    1400a66eb:	add    %dh,(%rdx)
    1400a66ed:	add    %dl,(%rdx)
    1400a66ef:	add    %al,(%rcx)
    1400a66f1:	add    %al,0x0(%rsi)
    1400a66f4:	imul   $0x65006c,(%rax),%eax
@@ -184677,18 +184676,17 @@
    1400a6700:	jae    0x1400a6702
    1400a6702:	imul   $0x6e006f,(%rax),%eax
    1400a6708:	add    %al,(%rax)
    1400a670a:	add    %al,(%rax)
    1400a670c:	xor    %eax,(%rax)
    1400a670e:	cs add %dh,(%rcx)
    1400a6711:	add    %ch,(%rsi)
-   1400a6713:	add    %dh,(%rbx)
-   1400a6715:	add    %bh,(%rcx)
-   1400a6717:	add    %ch,(%rsi)
-   1400a6719:	add    %dh,(%rax)
+   1400a6713:	add    %dh,(%rax,%rax,1)
+   1400a6716:	xor    %al,(%rax)
+   1400a6718:	cs add %dh,(%rax)
    1400a671b:	add    %al,(%rax)
    1400a671d:	add    %al,(%rax)
    1400a671f:	add    %bh,(%rax)
    1400a6721:	add    %dl,(%rax)
    1400a6723:	add    %al,(%rcx)
    1400a6725:	add    %cl,0x0(%rdi)
    1400a6728:	jb     0x1400a672a
```

## Comparing `tdrpa.tdcore-1.1.39.dist-info/METADATA` & `tdrpa.tdcore-1.1.40.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdrpa.tdcore
-Version: 1.1.39
+Version: 1.1.40
 Summary: RPA SDK for software developers. Supports Python3.7+, Windows x64
 Home-page: https://tdrpa.thingswell.cn
 Author: tdrpa
 Author-email: armstrong.wang@gmail.com
 License: Apache 2.0
 Keywords: RPA,tdRPA,uiautomation,uia
 Platform: Windows Only
```

## Comparing `tdrpa.tdcore-1.1.39.dist-info/RECORD` & `tdrpa.tdcore-1.1.40.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tdrpa/bot.exe,sha256=B8_eblvHdWYVbL-H6BAT2r6u4rK53VV6ULsAB6K7dvc,642560
-tdrpa/tdcore.cp39-win_amd64.pyd,sha256=AiNteZeX-p4qc0fzX3cHb6H81ZeTAJihIPv_9b_B7qs,615936
+tdrpa/bot.exe,sha256=29mczjb3kJOguevu4-3OwAxztrPhulRiaqvbQoq1iE4,642560
+tdrpa/tdcore.cp39-win_amd64.pyd,sha256=4_QjccQ-35x1KTp0P8XusBtfXdgrPiVeQDwvx7P2puc,616960
 tdrpa/tdcore/__init__.pyi,sha256=Ocw8nZCCyCW315mR-pjAv0Eh-7zfwtEkwyBKlehJKTw,353
 tdrpa/tdcore/locator/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore/locator/locatorWindows.pyi,sha256=4doiswkToDtOV5MKbkuX8gC-H6jOtLeUnraQLCaaBrA,265
 tdrpa/tdcore/locator/tdObject.pyi,sha256=bL4-DFpaE17uuCuN9ksd02DzNykVceBJsPSyw3wtSpI,264
 tdrpa/tdcore/log/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tdrpa/tdcore/log/log.pyi,sha256=0Ykq8rzUvpHtC9Hx9_BLZy_bARD9weAH_bbXacEEknQ,130
 tdrpa/tdcore/util/__init__.pyi,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -11,11 +11,11 @@
 tdrpa/tdcore-license/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 tdrpa/tdcore-license/infi.systray/LICENSE.txt,sha256=-9Uy-R2R7bZjSp8m31SUjOX8_6Og1laqYUB8npdzUHI,1473
 tdrpa/tdcore-license/psutil/LICENSE.txt,sha256=uJwGOzeG4o4MCjjxkx22H-015p3SopZvvs_-4PRsjRA,1548
 tdrpa/tdcore-license/pynput/COPYING.LGPL,sha256=eInlwsfJhthC1m5_bBVCQ1Mmf5nTUtL8MpjKfZxi0LU,7656
 tdrpa/tdcore-license/requests/LICENSE.txt,sha256=CeipvOyAZxBGUsFoaFqwkx54aPnIKEtm9a5u2uXxEws,10142
 tdrpa/tdcore-license/tzlocal/LICENSE.txt,sha256=2ZqyCa6xaq0sJckP_YPBqYHikP__dqQgoqsD4D8EG4w,1060
 tdrpa/tdcore-license/uiautomation/LICENSE.txt,sha256=dbcOQowi1H0PtxOlQxoO0HxUwqrfphk-OGwrkfn_Sys,11336
-tdrpa.tdcore-1.1.39.dist-info/METADATA,sha256=Q6bOcpV7Eoln63-v8J3bsRqD-1-nAoMMerlYFtdAYxs,612
-tdrpa.tdcore-1.1.39.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-tdrpa.tdcore-1.1.39.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
-tdrpa.tdcore-1.1.39.dist-info/RECORD,,
+tdrpa.tdcore-1.1.40.dist-info/METADATA,sha256=UanYp7SjtPQDQbB_PFrQ23E7Nb_qxxynie0bjN5FDNk,612
+tdrpa.tdcore-1.1.40.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tdrpa.tdcore-1.1.40.dist-info/top_level.txt,sha256=S9UoqmC_cyGqKbGsBkLQPEeQLbDrWD0SRwbxPpQpyyU,6
+tdrpa.tdcore-1.1.40.dist-info/RECORD,,
```

