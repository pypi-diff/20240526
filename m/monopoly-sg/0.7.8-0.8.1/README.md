# Comparing `tmp/monopoly_sg-0.7.8.tar.gz` & `tmp/monopoly_sg-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monopoly_sg-0.7.8.tar", max compression
+gzip compressed data, was "monopoly_sg-0.8.1.tar", max compression
```

## Comparing `monopoly_sg-0.7.8.tar` & `monopoly_sg-0.8.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.8/LICENSE.md
--rw-r--r--   0        0        0     2624 2024-04-21 03:16:26.522623 monopoly_sg-0.7.8/README.md
--rw-r--r--   0        0        0     2052 2024-04-21 10:15:23.763661 monopoly_sg-0.7.8/pyproject.toml
--rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.8/src/monopoly/__init__.py
--rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.8/src/monopoly/cli.py
--rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.8/src/monopoly/config.py
--rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.8/src/monopoly/constants.py
--rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.8/src/monopoly/examples/example_statement.pdf
--rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/examples/multiple_statements.py
--rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.8/src/monopoly/examples/single_statement.py
--rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.8/src/monopoly/log.py
--rw-r--r--   0        0        0     5935 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/pdf.py
--rw-r--r--   0        0        0     3808 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/processor.py
--rw-r--r--   0        0        0     3032 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/processors/__init__.py
--rw-r--r--   0        0        0     4100 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/processors/base.py
--rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/citibank/__init__.py
--rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.8/src/monopoly/processors/citibank/citibank.py
--rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/dbs/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.8/src/monopoly/processors/dbs/dbs.py
--rw-r--r--   0        0        0      964 2024-04-21 07:51:47.386734 monopoly_sg-0.7.8/src/monopoly/processors/example_bank.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/hsbc/__init__.py
--rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.8/src/monopoly/processors/hsbc/hsbc.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/ocbc/__init__.py
--rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.8/src/monopoly/processors/ocbc/ocbc.py
--rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/standard_chartered/__init__.py
--rw-r--r--   0        0        0     1007 2024-04-21 10:15:14.953665 monopoly_sg-0.7.8/src/monopoly/processors/standard_chartered/standard_chartered.py
--rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.8/src/monopoly/statements/__init__.py
--rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.8/src/monopoly/statements/base.py
--rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.8/src/monopoly/statements/credit_statement.py
--rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.8/src/monopoly/statements/debit_statement.py
--rw-r--r--   0        0        0     1465 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/write.py
--rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.8/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.8/tests/test_utils/skip.py
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 monopoly_sg-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-16 16:12:15.783983 monopoly_sg-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0     2833 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/README.md
+-rw-r--r--   0        0        0     2094 2024-05-26 08:08:41.007823 monopoly_sg-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.8.1/src/monopoly/__init__.py
+-rw-r--r--   0        0        0     2749 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/__init__.py
+-rw-r--r--   0        0        0     1713 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/base.py
+-rw-r--r--   0        0        0       55 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/citibank/__init__.py
+-rw-r--r--   0        0        0      925 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/citibank/citibank.py
+-rw-r--r--   0        0        0       40 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/dbs/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/dbs/dbs.py
+-rw-r--r--   0        0        0       43 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/hsbc/__init__.py
+-rw-r--r--   0        0        0     1064 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/hsbc/hsbc.py
+-rw-r--r--   0        0        0       43 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/ocbc/__init__.py
+-rw-r--r--   0        0        0     1261 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/ocbc/ocbc.py
+-rw-r--r--   0        0        0       83 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/standard_chartered/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/banks/standard_chartered/standard_chartered.py
+-rw-r--r--   0        0        0     9532 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/cli.py
+-rw-r--r--   0        0        0     3882 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/config.py
+-rw-r--r--   0        0        0     4005 2024-05-23 14:20:56.996834 monopoly_sg-0.8.1/src/monopoly/constants.py
+-rw-r--r--   0        0        0       83 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/examples/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-25 04:37:45.117476 monopoly_sg-0.8.1/src/monopoly/examples/example_bank.py
+-rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.8.1/src/monopoly/examples/example_statement.pdf
+-rw-r--r--   0        0        0      927 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/examples/single_statement.py
+-rw-r--r--   0        0        0     4685 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/handler.py
+-rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.8.1/src/monopoly/log.py
+-rw-r--r--   0        0        0     8785 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/pdf.py
+-rw-r--r--   0        0        0      216 2024-05-22 14:38:33.782767 monopoly_sg-0.8.1/src/monopoly/statements/__init__.py
+-rw-r--r--   0        0        0     6679 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/statements/base.py
+-rw-r--r--   0        0        0     2568 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/statements/credit_statement.py
+-rw-r--r--   0        0        0     3722 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/statements/debit_statement.py
+-rw-r--r--   0        0        0     3907 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/statements/transaction.py
+-rw-r--r--   0        0        0     1447 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/src/monopoly/write.py
+-rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.8.1/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      790 2024-05-26 02:54:58.761662 monopoly_sg-0.8.1/tests/test_utils/skip.py
+-rw-r--r--   0        0        0      622 2024-05-26 08:08:41.017823 monopoly_sg-0.8.1/tests/test_utils/transactions.py
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 monopoly_sg-0.8.1/PKG-INFO
```

### Comparing `monopoly_sg-0.7.8/README.md` & `monopoly_sg-0.8.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,178 @@
 00000000: 215b 5d28 6874 7470 733a 2f2f 7261 772e  ![](https://raw.
 00000010: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
 00000020: 742e 636f 6d2f 6265 6e6a 616d 696e 2d61  t.com/benjamin-a
 00000030: 7764 2f6d 6f6e 6f70 6f6c 792f 6d61 696e  wd/monopoly/main
 00000040: 2f64 6f63 732f 6c6f 676f 2e73 7667 290a  /docs/logo.svg).
 00000050: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
-00000060: 2d2d 0a0a 5b21 5b54 6573 7473 5d28 6874  --..[![Tests](ht
-00000070: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000080: 2f62 656e 6a61 6d69 6e2d 6177 642f 6d6f  /benjamin-awd/mo
-00000090: 6e6f 706f 6c79 2f61 6374 696f 6e73 2f77  nopoly/actions/w
-000000a0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
-000000b0: 616d 6c2f 6261 6467 652e 7376 673f 6272  aml/badge.svg?br
-000000c0: 616e 6368 3d6d 6169 6e26 6576 656e 743d  anch=main&event=
-000000d0: 7075 7368 295d 2868 7474 7073 3a2f 2f67  push)](https://g
-000000e0: 6974 6875 622e 636f 6d2f 6265 6e6a 616d  ithub.com/benjam
-000000f0: 696e 2d61 7764 2f6d 6f6e 6f70 6f6c 792f  in-awd/monopoly/
-00000100: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
-00000110: 732f 7465 7374 732e 7961 6d6c 290a 5b21  s/tests.yaml).[!
-00000120: 5b43 495d 2868 7474 7073 3a2f 2f67 6974  [CI](https://git
-00000130: 6875 622e 636f 6d2f 6265 6e6a 616d 696e  hub.com/benjamin
-00000140: 2d61 7764 2f6d 6f6e 6f70 6f6c 792f 6163  -awd/monopoly/ac
-00000150: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000160: 6369 2e79 616d 6c2f 6261 6467 652e 7376  ci.yaml/badge.sv
-00000170: 673f 6272 616e 6368 3d6d 6169 6e26 6576  g?branch=main&ev
-00000180: 656e 743d 7075 7368 295d 2868 7474 7073  ent=push)](https
-00000190: 3a2f 2f67 6974 6875 622e 636f 6d2f 6265  ://github.com/be
-000001a0: 6e6a 616d 696e 2d61 7764 2f6d 6f6e 6f70  njamin-awd/monop
-000001b0: 6f6c 792f 6163 7469 6f6e 732f 776f 726b  oly/actions/work
-000001c0: 666c 6f77 732f 6369 2e79 616d 6c29 0a5b  flows/ci.yaml).[
-000001d0: 215b 436f 6465 2073 7479 6c65 3a20 626c  ![Code style: bl
-000001e0: 6163 6b5d 2868 7474 7073 3a2f 2f69 6d67  ack](https://img
-000001f0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000200: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
-00000210: 6c61 636b 2d30 3030 3030 302e 7376 6729  lack-000000.svg)
-00000220: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000230: 2e63 6f6d 2f70 7366 2f62 6c61 636b 290a  .com/psf/black).
-00000240: 5b21 5b4c 696e 7469 6e67 3a20 7079 6c69  [![Linting: pyli
-00000250: 6e74 5d28 6874 7470 733a 2f2f 696d 672e  nt](https://img.
-00000260: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000270: 2f6c 696e 7469 6e67 2d70 796c 696e 742d  /linting-pylint-
-00000280: 6f72 616e 6765 295d 2868 7474 7073 3a2f  orange)](https:/
-00000290: 2f67 6974 6875 622e 636f 6d2f 7079 6c69  /github.com/pyli
-000002a0: 6e74 2d64 6576 2f70 796c 696e 7429 0a5b  nt-dev/pylint).[
-000002b0: 215b 4c69 6365 6e73 653a 204d 4954 5d28  ![License: MIT](
-000002c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000002d0: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
-000002e0: 656e 7365 2d4d 4954 2d79 656c 6c6f 772e  ense-MIT-yellow.
-000002f0: 7376 6729 5d28 6874 7470 733a 2f2f 6f70  svg)](https://op
-00000300: 656e 736f 7572 6365 2e6f 7267 2f6c 6963  ensource.org/lic
-00000310: 656e 7365 732f 4d49 5429 0a0a 0a4d 6f6e  enses/MIT)...Mon
-00000320: 6f70 6f6c 7920 6973 2061 2050 7974 686f  opoly is a Pytho
-00000330: 6e20 6c69 6272 6172 7920 7468 6174 2063  n library that c
-00000340: 6f6e 7665 7274 7320 5369 6e67 6170 6f72  onverts Singapor
-00000350: 6520 6261 6e6b 2073 7461 7465 6d65 6e74  e bank statement
-00000360: 2050 4446 7320 746f 2043 5356 2075 7369   PDFs to CSV usi
-00000370: 6e67 2070 6466 746f 7465 7874 0a0a 215b  ng pdftotext..![
-00000380: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
-00000390: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-000003a0: 636f 6d2f 6265 6e6a 616d 696e 2d61 7764  com/benjamin-awd
-000003b0: 2f6d 6f6e 6f70 6f6c 792f 6d61 696e 2f64  /monopoly/main/d
-000003c0: 6f63 732f 6d6f 6e6f 706f 6c79 2e67 6966  ocs/monopoly.gif
-000003d0: 290a 0a53 7570 706f 7274 6564 2062 616e  )..Supported ban
-000003e0: 6b73 3a0a 7c20 4261 6e6b 2020 2020 2020  ks:.| Bank      
-000003f0: 2020 2020 2020 2020 2020 7c20 4372 6564            | Cred
-00000400: 6974 2053 7461 7465 6d65 6e74 2020 2020  it Statement    
-00000410: 7c20 4465 6269 7420 5374 6174 656d 656e  | Debit Statemen
-00000420: 7420 2020 2020 7c0a 7c20 2d2d 2d2d 2d2d  t     |.| ------
-00000430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c20  --------------| 
-00000440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000450: 2d2d 2d2d 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  ----| ----------
-00000460: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 4369  ----------|.| Ci
-00000470: 7469 6261 6e6b 2020 2020 2020 2020 2020  tibank          
-00000480: 2020 7c20 3a77 6869 7465 5f63 6865 636b    | :white_check
-00000490: 5f6d 6172 6b3a 2020 7c20 3a78 3a20 2020  _mark:  | :x:   
-000004a0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-000004b0: 7c20 4442 5320 2020 2020 2020 2020 2020  | DBS           
-000004c0: 2020 2020 2020 7c20 3a77 6869 7465 5f63        | :white_c
-000004d0: 6865 636b 5f6d 6172 6b3a 2020 7c20 3a77  heck_mark:  | :w
-000004e0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
-000004f0: 2020 7c0a 7c20 4853 4243 2020 2020 2020    |.| HSBC      
-00000500: 2020 2020 2020 2020 2020 7c20 3a77 6869            | :whi
-00000510: 7465 5f63 6865 636b 5f6d 6172 6b3a 2020  te_check_mark:  
-00000520: 7c20 3a78 3a20 2020 2020 2020 2020 2020  | :x:           
-00000530: 2020 2020 2020 7c0a 7c20 4f43 4243 2020        |.| OCBC  
-00000540: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00000550: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
-00000560: 6b3a 2020 7c20 3a77 6869 7465 5f63 6865  k:  | :white_che
-00000570: 636b 5f6d 6172 6b3a 2020 7c0a 7c20 5374  ck_mark:  |.| St
-00000580: 616e 6461 7264 2043 6861 7274 6572 6564  andard Chartered
-00000590: 2020 7c20 3a77 6869 7465 5f63 6865 636b    | :white_check
-000005a0: 5f6d 6172 6b3a 2020 7c20 3a78 3a20 2020  _mark:  | :x:   
-000005b0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-000005c0: 0a23 2320 496e 7374 616c 6c0a 436c 6f6e  .## Install.Clon
-000005d0: 6520 7468 6520 7265 706f 0a60 6060 6261  e the repo.```ba
-000005e0: 7368 0a67 6974 2063 6c6f 6e65 2068 7474  sh.git clone htt
-000005f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000600: 6265 6e6a 616d 696e 2d61 7764 2f6d 6f6e  benjamin-awd/mon
-00000610: 6f70 6f6c 792e 6769 740a 6060 600a 0a49  opoly.git.```..I
-00000620: 6e73 7461 6c6c 2064 6570 656e 6465 6e63  nstall dependenc
-00000630: 6965 7320 7573 696e 6720 5b48 6f6d 6562  ies using [Homeb
-00000640: 7265 775d 2868 7474 7073 3a2f 2f62 7265  rew](https://bre
-00000650: 772e 7368 2f29 0a60 6060 6261 7368 0a62  w.sh/).```bash.b
-00000660: 7265 7720 696e 7374 616c 6c20 6d61 6b65  rew install make
-00000670: 0a6d 616b 6520 7365 7475 700a 6060 600a  .make setup.```.
-00000680: 0a23 2320 5573 6167 650a 4d6f 6e6f 706f  .## Usage.Monopo
-00000690: 6c79 2063 616e 2062 6520 7275 6e20 6173  ly can be run as
-000006a0: 2061 2050 7974 686f 6e20 7061 636b 6167   a Python packag
-000006b0: 652c 2061 6c6c 6f77 696e 6720 796f 7520  e, allowing you 
-000006c0: 746f 2065 7874 7261 6374 2c20 7472 616e  to extract, tran
-000006d0: 7366 6f72 6d20 616e 6420 7772 6974 6520  sform and write 
-000006e0: 6261 6e6b 2073 7461 7465 6d65 6e74 7320  bank statements 
-000006f0: 746f 2061 2043 5356 2066 696c 652e 0a0a  to a CSV file...
-00000700: 546f 2073 6565 2068 6f77 204d 6f6e 6f70  To see how Monop
-00000710: 6f6c 7920 776f 726b 732c 2079 6f75 2063  oly works, you c
-00000720: 616e 2072 756e 2074 6869 7320 6578 616d  an run this exam
-00000730: 706c 650a 6060 6062 6173 680a 7079 7468  ple.```bash.pyth
-00000740: 6f6e 3320 7372 632f 6d6f 6e6f 706f 6c79  on3 src/monopoly
-00000750: 2f65 7861 6d70 6c65 732f 7369 6e67 6c65  /examples/single
-00000760: 5f73 7461 7465 6d65 6e74 2e70 790a 6060  _statement.py.``
-00000770: 600a 0a49 6620 796f 7520 6e65 6564 2074  `..If you need t
-00000780: 6f20 7275 6e20 6d6f 6e6f 706f 6c79 206f  o run monopoly o
-00000790: 6e20 6120 7061 7373 776f 7264 2070 726f  n a password pro
-000007a0: 7465 6374 6564 2066 696c 652c 2065 6e73  tected file, ens
-000007b0: 7572 6520 7468 6174 2070 6173 7377 6f72  ure that passwor
-000007c0: 6473 2061 7265 2073 6574 2069 6e20 7468  ds are set in th
-000007d0: 6520 2e65 6e76 2066 696c 653a 0a60 6060  e .env file:.```
-000007e0: 7368 0a63 7020 2e65 6e76 2e74 656d 706c  sh.cp .env.templ
-000007f0: 6174 6520 656e 760a 6060 600a 0a49 6620  ate env.```..If 
-00000800: 796f 7520 6861 7665 206d 756c 7469 706c  you have multipl
-00000810: 6520 7374 6174 656d 656e 7473 2066 726f  e statements fro
-00000820: 6d20 7468 6520 7361 6d65 2062 616e 6b20  m the same bank 
-00000830: 7769 7468 2064 6966 6665 7265 6e74 2070  with different p
-00000840: 6173 7377 6f72 6473 2028 652e 672e 2048  asswords (e.g. H
-00000850: 5342 4320 7374 6174 656d 656e 7473 292c  SBC statements),
-00000860: 206d 616b 6520 7375 7265 2074 6f20 7365   make sure to se
-00000870: 7420 626f 7468 2070 6173 7377 6f72 6473  t both passwords
-00000880: 2069 6e20 616e 2061 7272 6179 2066 6f72   in an array for
-00000890: 6d61 7420 6c69 6b65 2073 6f3a 0a60 6060  mat like so:.```
-000008a0: 7368 0a48 5342 435f 5044 465f 5041 5353  sh.HSBC_PDF_PASS
-000008b0: 574f 5244 533d 5b22 7061 7373 776f 7264  WORDS=["password
-000008c0: 3122 2c22 7061 7373 776f 7264 3222 5d0a  1","password2"].
-000008d0: 6060 600a 0a23 2320 4665 6174 7572 6573  ```..## Features
-000008e0: 0a2d 2055 6e6c 6f63 6b73 2050 4446 7320  .- Unlocks PDFs 
-000008f0: 7573 696e 6720 7573 6572 2d70 726f 7669  using user-provi
-00000900: 6465 6420 6372 6564 656e 7469 616c 730a  ded credentials.
-00000910: 2d20 5374 6174 656d 656e 7473 2063 616e  - Statements can
-00000920: 2062 6520 7061 7273 6564 2077 6974 6820   be parsed with 
-00000930: 7468 6520 434c 492c 206f 7220 6d61 6e75  the CLI, or manu
-00000940: 616c 6c79 2077 6974 6820 7468 6520 6261  ally with the ba
-00000950: 6e6b 2070 726f 6365 7373 6f72 2063 6c61  nk processor cla
-00000960: 7373 2e0a 2d20 5375 7070 6f72 7420 666f  ss..- Support fo
-00000970: 7220 6361 7368 6261 636b 2074 7261 6e73  r cashback trans
-00000980: 6163 7469 6f6e 7320 616e 6420 7265 6675  actions and refu
-00000990: 6e64 730a 2d20 4d6f 6e6f 706f 6c79 2063  nds.- Monopoly c
-000009a0: 616e 2062 6520 7275 6e20 6f6e 2047 6f6f  an be run on Goo
-000009b0: 676c 6520 436c 6f75 6420 6173 2061 2073  gle Cloud as a s
-000009c0: 6368 6564 756c 6564 2043 6c6f 7564 2052  cheduled Cloud R
-000009d0: 756e 206a 6f62 2c20 7768 6963 6820 6f70  un job, which op
-000009e0: 656e 7320 7570 206d 6f72 6520 736f 7068  ens up more soph
-000009f0: 6973 7469 6361 7465 6420 7573 652d 6361  isticated use-ca
-00000a00: 7365 7320 6c69 6b65 2068 6973 746f 7269  ses like histori
-00000a10: 6361 6c20 616e 616c 7973 6973 2061 6e64  cal analysis and
-00000a20: 2070 6572 736f 6e61 6c20 6669 6e61 6e63   personal financ
-00000a30: 6520 7669 7375 616c 697a 6174 696f 6e0a  e visualization.
+00000060: 2d2d 0a5b 215b 5374 7265 616d 6c69 745d  --.[![Streamlit]
+00000070: 2868 7474 7073 3a2f 2f73 7461 7469 632e  (https://static.
+00000080: 7374 7265 616d 6c69 742e 696f 2f62 6164  streamlit.io/bad
+00000090: 6765 732f 7374 7265 616d 6c69 745f 6261  ges/streamlit_ba
+000000a0: 6467 655f 626c 6163 6b5f 7768 6974 652e  dge_black_white.
+000000b0: 7376 6729 5d28 6874 7470 733a 2f2f 6d6f  svg)](https://mo
+000000c0: 6e6f 706f 6c79 2e73 7472 6561 6d6c 6974  nopoly.streamlit
+000000d0: 2e61 7070 290a 5b21 5b54 6573 7473 5d28  .app).[![Tests](
+000000e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000000f0: 6f6d 2f62 656e 6a61 6d69 6e2d 6177 642f  om/benjamin-awd/
+00000100: 6d6f 6e6f 706f 6c79 2f61 6374 696f 6e73  monopoly/actions
+00000110: 2f77 6f72 6b66 6c6f 7773 2f74 6573 7473  /workflows/tests
+00000120: 2e79 616d 6c2f 6261 6467 652e 7376 673f  .yaml/badge.svg?
+00000130: 6272 616e 6368 3d6d 6169 6e26 6576 656e  branch=main&even
+00000140: 743d 7075 7368 295d 2868 7474 7073 3a2f  t=push)](https:/
+00000150: 2f67 6974 6875 622e 636f 6d2f 6265 6e6a  /github.com/benj
+00000160: 616d 696e 2d61 7764 2f6d 6f6e 6f70 6f6c  amin-awd/monopol
+00000170: 792f 6163 7469 6f6e 732f 776f 726b 666c  y/actions/workfl
+00000180: 6f77 732f 7465 7374 732e 7961 6d6c 290a  ows/tests.yaml).
+00000190: 5b21 5b43 495d 2868 7474 7073 3a2f 2f67  [![CI](https://g
+000001a0: 6974 6875 622e 636f 6d2f 6265 6e6a 616d  ithub.com/benjam
+000001b0: 696e 2d61 7764 2f6d 6f6e 6f70 6f6c 792f  in-awd/monopoly/
+000001c0: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+000001d0: 732f 6369 2e79 616d 6c2f 6261 6467 652e  s/ci.yaml/badge.
+000001e0: 7376 673f 6272 616e 6368 3d6d 6169 6e26  svg?branch=main&
+000001f0: 6576 656e 743d 7075 7368 295d 2868 7474  event=push)](htt
+00000200: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000210: 6265 6e6a 616d 696e 2d61 7764 2f6d 6f6e  benjamin-awd/mon
+00000220: 6f70 6f6c 792f 6163 7469 6f6e 732f 776f  opoly/actions/wo
+00000230: 726b 666c 6f77 732f 6369 2e79 616d 6c29  rkflows/ci.yaml)
+00000240: 0a5b 215b 4c69 6365 6e73 653a 204d 4954  .[![License: MIT
+00000250: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000260: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
+00000270: 6963 656e 7365 2d4d 4954 2d79 656c 6c6f  icense-MIT-yello
+00000280: 772e 7376 6729 5d28 6874 7470 733a 2f2f  w.svg)](https://
+00000290: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+000002a0: 6963 656e 7365 732f 4d49 5429 0a0a 4d6f  icenses/MIT)..Mo
+000002b0: 6e6f 706f 6c79 2069 7320 6120 5079 7468  nopoly is a Pyth
+000002c0: 6f6e 206c 6962 7261 7279 2026 2043 4c49  on library & CLI
+000002d0: 2074 6861 7420 636f 6e76 6572 7473 2053   that converts S
+000002e0: 696e 6761 706f 7265 2062 616e 6b20 7374  ingapore bank st
+000002f0: 6174 656d 656e 7420 5044 4673 2074 6f20  atement PDFs to 
+00000300: 4353 562e 0a0a 215b 5d28 6874 7470 733a  CSV...![](https:
+00000310: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
+00000320: 636f 6e74 656e 742e 636f 6d2f 6265 6e6a  content.com/benj
+00000330: 616d 696e 2d61 7764 2f6d 6f6e 6f70 6f6c  amin-awd/monopol
+00000340: 792f 6d61 696e 2f64 6f63 732f 6d6f 6e6f  y/main/docs/mono
+00000350: 706f 6c79 2e67 6966 290a 0a53 7570 706f  poly.gif)..Suppo
+00000360: 7274 6564 2062 616e 6b73 3a0a 7c20 4261  rted banks:.| Ba
+00000370: 6e6b 2020 2020 2020 2020 2020 2020 2020  nk              
+00000380: 2020 7c20 4372 6564 6974 2053 7461 7465    | Credit State
+00000390: 6d65 6e74 2020 2020 7c20 4465 6269 7420  ment    | Debit 
+000003a0: 5374 6174 656d 656e 7420 2020 2020 7c0a  Statement     |.
+000003b0: 7c20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  | --------------
+000003c0: 2d2d 2d2d 2d2d 7c20 2d2d 2d2d 2d2d 2d2d  ------| --------
+000003d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c20 2d2d  ------------| --
+000003e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003f0: 2d2d 7c0a 7c20 4369 7469 6261 6e6b 2020  --|.| Citibank  
+00000400: 2020 2020 2020 2020 2020 7c20 3a77 6869            | :whi
+00000410: 7465 5f63 6865 636b 5f6d 6172 6b3a 2020  te_check_mark:  
+00000420: 7c20 3a78 3a20 2020 2020 2020 2020 2020  | :x:           
+00000430: 2020 2020 2020 7c0a 7c20 4442 5320 2020        |.| DBS   
+00000440: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00000450: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+00000460: 6b3a 2020 7c20 3a77 6869 7465 5f63 6865  k:  | :white_che
+00000470: 636b 5f6d 6172 6b3a 2020 7c0a 7c20 4853  ck_mark:  |.| HS
+00000480: 4243 2020 2020 2020 2020 2020 2020 2020  BC              
+00000490: 2020 7c20 3a77 6869 7465 5f63 6865 636b    | :white_check
+000004a0: 5f6d 6172 6b3a 2020 7c20 3a78 3a20 2020  _mark:  | :x:   
+000004b0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+000004c0: 7c20 4f43 4243 2020 2020 2020 2020 2020  | OCBC          
+000004d0: 2020 2020 2020 7c20 3a77 6869 7465 5f63        | :white_c
+000004e0: 6865 636b 5f6d 6172 6b3a 2020 7c20 3a77  heck_mark:  | :w
+000004f0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
+00000500: 2020 7c0a 7c20 5374 616e 6461 7264 2043    |.| Standard C
+00000510: 6861 7274 6572 6564 2020 7c20 3a77 6869  hartered  | :whi
+00000520: 7465 5f63 6865 636b 5f6d 6172 6b3a 2020  te_check_mark:  
+00000530: 7c20 3a78 3a20 2020 2020 2020 2020 2020  | :x:           
+00000540: 2020 2020 2020 7c0a 0a3c 6833 2061 6c69        |..<h3 ali
+00000550: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000560: 20f0 9f8e 8920 4d6f 6e6f 706f 6c79 2069   .... Monopoly i
+00000570: 7320 6e6f 7720 6c69 7665 2120 f09f 8e89  s now live! ....
+00000580: 0a20 2020 203c 6272 3e3c 6272 3e0a 2020  .    <br><br>.  
+00000590: 2020 5472 7920 6974 206f 7574 3a20 3c62    Try it out: <b
+000005a0: 723e 0a20 2020 203c 6120 6872 6566 3d22  r>.    <a href="
+000005b0: 6874 7470 733a 2f2f 6d6f 6e6f 706f 6c79  https://monopoly
+000005c0: 2e73 7472 6561 6d6c 6974 6170 702e 636f  .streamlitapp.co
+000005d0: 6d2f 223e 6874 7470 733a 2f2f 6d6f 6e6f  m/">https://mono
+000005e0: 706f 6c79 2e73 7472 6561 6d6c 6974 6170  poly.streamlitap
+000005f0: 702e 636f 6d2f 3c2f 613e 0a3c 2f68 333e  p.com/</a>.</h3>
+00000600: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
+00000610: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
+00000620: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+00000630: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00000640: 2e63 6f6d 2f62 656e 6a61 6d69 6e2d 6177  .com/benjamin-aw
+00000650: 642f 6d6f 6e6f 706f 6c79 2f6d 6169 6e2f  d/monopoly/main/
+00000660: 646f 6373 2f73 7472 6561 6d6c 6974 5f64  docs/streamlit_d
+00000670: 656d 6f2e 6769 6622 2077 6964 7468 3d38  emo.gif" width=8
+00000680: 3030 3e0a 3c2f 703e 0a0a 2323 2049 6e73  00>.</p>..## Ins
+00000690: 7461 6c6c 0a43 6c6f 6e65 2074 6865 2072  tall.Clone the r
+000006a0: 6570 6f0a 6060 6062 6173 680a 6769 7420  epo.```bash.git 
+000006b0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
+000006c0: 7468 7562 2e63 6f6d 2f62 656e 6a61 6d69  thub.com/benjami
+000006d0: 6e2d 6177 642f 6d6f 6e6f 706f 6c79 2e67  n-awd/monopoly.g
+000006e0: 6974 0a60 6060 0a0a 496e 7374 616c 6c20  it.```..Install 
+000006f0: 6465 7065 6e64 656e 6369 6573 2075 7369  dependencies usi
+00000700: 6e67 205b 486f 6d65 6272 6577 5d28 6874  ng [Homebrew](ht
+00000710: 7470 733a 2f2f 6272 6577 2e73 682f 290a  tps://brew.sh/).
+00000720: 6060 6062 6173 680a 6272 6577 2069 6e73  ```bash.brew ins
+00000730: 7461 6c6c 206d 616b 650a 6d61 6b65 2073  tall make.make s
+00000740: 6574 7570 0a60 6060 0a0a 2323 2055 7361  etup.```..## Usa
+00000750: 6765 0a4d 6f6e 6f70 6f6c 7920 6361 6e20  ge.Monopoly can 
+00000760: 6265 2072 756e 2061 7320 6120 5079 7468  be run as a Pyth
+00000770: 6f6e 2070 6163 6b61 6765 2c20 616c 6c6f  on package, allo
+00000780: 7769 6e67 2079 6f75 2074 6f20 6578 7472  wing you to extr
+00000790: 6163 742c 2074 7261 6e73 666f 726d 2061  act, transform a
+000007a0: 6e64 2077 7269 7465 2062 616e 6b20 7374  nd write bank st
+000007b0: 6174 656d 656e 7473 2074 6f20 6120 4353  atements to a CS
+000007c0: 5620 6669 6c65 2e0a 0a54 6f20 7365 6520  V file...To see 
+000007d0: 686f 7720 4d6f 6e6f 706f 6c79 2077 6f72  how Monopoly wor
+000007e0: 6b73 2c20 796f 7520 6361 6e20 7275 6e20  ks, you can run 
+000007f0: 7468 6973 2065 7861 6d70 6c65 0a60 6060  this example.```
+00000800: 6261 7368 0a70 7974 686f 6e33 2073 7263  bash.python3 src
+00000810: 2f6d 6f6e 6f70 6f6c 792f 6578 616d 706c  /monopoly/exampl
+00000820: 6573 2f73 696e 676c 655f 7374 6174 656d  es/single_statem
+00000830: 656e 742e 7079 0a60 6060 0a0a 4966 2079  ent.py.```..If y
+00000840: 6f75 206e 6565 6420 746f 2072 756e 206d  ou need to run m
+00000850: 6f6e 6f70 6f6c 7920 6f6e 2061 2070 6173  onopoly on a pas
+00000860: 7377 6f72 6420 7072 6f74 6563 7465 6420  sword protected 
+00000870: 6669 6c65 2c20 656e 7375 7265 2074 6861  file, ensure tha
+00000880: 7420 7061 7373 776f 7264 7320 6172 6520  t passwords are 
+00000890: 7365 7420 696e 2074 6865 202e 656e 7620  set in the .env 
+000008a0: 6669 6c65 3a0a 6060 6073 680a 6370 202e  file:.```sh.cp .
+000008b0: 656e 762e 7465 6d70 6c61 7465 2065 6e76  env.template env
+000008c0: 0a60 6060 0a0a 4966 2079 6f75 2068 6176  .```..If you hav
+000008d0: 6520 6d75 6c74 6970 6c65 2073 7461 7465  e multiple state
+000008e0: 6d65 6e74 7320 6672 6f6d 2074 6865 2073  ments from the s
+000008f0: 616d 6520 6261 6e6b 2077 6974 6820 6469  ame bank with di
+00000900: 6666 6572 656e 7420 7061 7373 776f 7264  fferent password
+00000910: 7320 2865 2e67 2e20 4853 4243 2073 7461  s (e.g. HSBC sta
+00000920: 7465 6d65 6e74 7329 2c20 6d61 6b65 2073  tements), make s
+00000930: 7572 6520 746f 2073 6574 2062 6f74 6820  ure to set both 
+00000940: 7061 7373 776f 7264 7320 696e 2061 6e20  passwords in an 
+00000950: 6172 7261 7920 666f 726d 6174 206c 696b  array format lik
+00000960: 6520 736f 3a0a 6060 6073 680a 4853 4243  e so:.```sh.HSBC
+00000970: 5f50 4446 5f50 4153 5357 4f52 4453 3d5b  _PDF_PASSWORDS=[
+00000980: 2270 6173 7377 6f72 6431 222c 2270 6173  "password1","pas
+00000990: 7377 6f72 6432 225d 0a60 6060 0a0a 2323  sword2"].```..##
+000009a0: 2046 6561 7475 7265 730a 2d20 556e 6c6f   Features.- Unlo
+000009b0: 636b 7320 5044 4673 2075 7369 6e67 2075  cks PDFs using u
+000009c0: 7365 722d 7072 6f76 6964 6564 2063 7265  ser-provided cre
+000009d0: 6465 6e74 6961 6c73 0a2d 2053 7461 7465  dentials.- State
+000009e0: 6d65 6e74 7320 6361 6e20 6265 2070 6172  ments can be par
+000009f0: 7365 6420 7769 7468 2074 6865 2043 4c49  sed with the CLI
+00000a00: 2c20 6f72 2077 6974 6820 6120 7363 7269  , or with a scri
+00000a10: 7074 2075 7369 6e67 2074 6865 2053 7461  pt using the Sta
+00000a20: 7465 6d65 6e74 4861 6e64 6c65 7220 636c  tementHandler cl
+00000a30: 6173 732e 0a2d 2053 7570 706f 7274 2066  ass..- Support f
+00000a40: 6f72 2063 6173 6862 6163 6b20 7472 616e  or cashback tran
+00000a50: 7361 6374 696f 6e73 2061 6e64 2072 6566  sactions and ref
+00000a60: 756e 6473 0a2d 204d 6f6e 6f70 6f6c 7920  unds.- Monopoly 
+00000a70: 6361 6e20 6265 2072 756e 206f 6e20 476f  can be run on Go
+00000a80: 6f67 6c65 2043 6c6f 7564 2061 7320 6120  ogle Cloud as a 
+00000a90: 7363 6865 6475 6c65 6420 436c 6f75 6420  scheduled Cloud 
+00000aa0: 5275 6e20 6a6f 622c 2077 6869 6368 206f  Run job, which o
+00000ab0: 7065 6e73 2075 7020 6d6f 7265 2073 6f70  pens up more sop
+00000ac0: 6869 7374 6963 6174 6564 2075 7365 2d63  histicated use-c
+00000ad0: 6173 6573 206c 696b 6520 6869 7374 6f72  ases like histor
+00000ae0: 6963 616c 2061 6e61 6c79 7369 7320 616e  ical analysis an
+00000af0: 6420 7065 7273 6f6e 616c 2066 696e 616e  d personal finan
+00000b00: 6365 2076 6973 7561 6c69 7a61 7469 6f6e  ce visualization
+00000b10: 0a                                       .
```

### Comparing `monopoly_sg-0.7.8/pyproject.toml` & `monopoly_sg-0.8.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monopoly-sg"
-version = "0.7.8"
+version = "0.8.1"
 description = "PDF parsing for Singaporean banks"
 repository = "https://github.com/benjamin-awd/monopoly"
 authors = ["benjamin-awd <benjamindornel@gmail.com>"]
 packages = [
     { include = "monopoly", from = "src" },
     { include = "test_utils", from = "tests" }
 ]
@@ -13,37 +13,38 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11, <3.12"
-pandas = "^2.1.3"
 pydantic-settings = "^2.0.3"
 pymupdf = "^1.23.7"
 pdftotext = "^2.2.2"
 click = "^8.1.7"
 tqdm = "^4.66.1"
-pdf2john = "^0.2.0"
 tabulate = "^0.9.0"
 mypy = "^1.7.1"
 pydantic = "^2.5.2"
+dateparser = "^1.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7,<25.0"
 pylint = ">=2.17.5,<4.0.0"
 isort = "^5.12.0"
 taskipy = "^1.12.0"
 flake8 = ">=6.1,<8.0"
 pytest = ">=7.4.1,<9.0.0"
 pysnooper = "^1.2.0"
 pylint-pydantic = "^0.3.0"
 mypy = "^1.6.1"
 types-tqdm = "^4.66.0.5"
+types-dateparser = "^1.2.0.20240420"
+types-tabulate = "^0.9.0.20240106"
 
 
 [tool.taskipy.tasks]
 format = "isort . && black ."
 lint = "flake8 src & pylint src"
 test = "pytest ."
 mypy = "mypy src"
@@ -79,15 +80,14 @@
 ]
 
 [[tool.mypy.overrides]]
 module = [
     "fitz",
     "pdftotext",
     "pdf2john",
-    "pandas",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/cli.py` & `monopoly_sg-0.8.1/src/monopoly/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 import traceback
 from concurrent.futures import ProcessPoolExecutor
 from pathlib import Path
-from typing import Collection, Iterable, Optional
+from typing import Collection, Iterable, Optional, TypedDict
 
 import click
 from pydantic.dataclasses import dataclass
+from tabulate import tabulate
 from tqdm import tqdm
 
-from monopoly.processors import detect_processor
+
+class TqdmSettings(TypedDict):
+    """
+    Stores settings for `tqdm`
+    """
+
+    total: int
+    desc: str
+    leave: bool
+    delay: float
+    ncols: int
+    bar_format: str
 
 
 @dataclass
 class Result:
     """
     Stores information about processed bank statement
     """
@@ -91,70 +103,105 @@
             in a tabular format. No file is generated in this case.
 
     Returns:
         Optional[Result]: If print_df is False, returns a Result object containing
         information about the processed statement. If an error occurs during processing,
         returns a Result object with error information.
     """
+    from monopoly.handler import (  # pylint: disable=import-outside-toplevel
+        StatementHandler,
+    )
 
     try:
-        processor = detect_processor(file)
-        statement = processor.extract()
-        transformed_df = processor.transform(statement)
+        handler = StatementHandler(file)
+        statement = handler.extract()
+        transactions = handler.transform(
+            transactions=statement.transactions,
+            statement_date=statement.statement_date,
+            transaction_date_order=statement.config.transaction_date_order,
+        )
 
         if print_df:
-            click.echo(f"{file.name}")
-            click.echo(transformed_df.to_markdown(tablefmt="psql", numalign="right"))
-            click.echo()
+            pprint_transactions(transactions, statement, file)
+            # don't load to CSV if pprint
             return None
 
         # saves processed statements to the same directory by default
         if not output_directory:
             output_directory = file.parent
 
-        output_file = processor.load(transformed_df, statement, output_directory)
+        output_file = handler.load(transactions, statement, output_directory)
         return Result(file.name, output_file.name)
 
     except Exception as err:  # pylint: disable=broad-exception-caught
         error_info = {
             "message": f"{type(err).__name__}: {str(err)}",
             "traceback": traceback.format_exc(),
         }
         return Result(file.name, error_info=error_info)
 
 
+def pprint_transactions(transactions: list, statement, file: Path) -> None:
+    """Prints transactions in a markdown style tabular format"""
+    click.echo(f"{file.name}")
+    transactions_as_dict = [transaction.as_raw_dict() for transaction in transactions]
+    headers = {col: col for col in statement.columns}
+    click.echo(
+        tabulate(
+            transactions_as_dict,
+            headers=headers,
+            tablefmt="psql",
+            numalign="right",
+        )
+    )
+    click.echo()
+
+
 def run(
     input_files: Collection[Path],
     output_directory: Optional[Path] = None,
     print_df: bool = False,
+    single_process: bool = False,
 ):
     """
     Process a collection of input files concurrently
 
     If any statements are processed successfully or encounter errors, a Report object
     is created and its display_report() method is called to provide a summary
     of the processing outcomes.
     """
-    with ProcessPoolExecutor() as executor:
-        results = list(
-            tqdm(
-                executor.map(
-                    process_statement,
-                    input_files,
-                    [output_directory] * len(input_files),
-                    [print_df] * len(input_files),
-                ),
-                total=len(input_files),
-                desc="Processing statements",
-                leave=False,
-                delay=0.5,
-                ncols=80,
-                bar_format="{l_bar}{bar}| {n_fmt}/{total_fmt}",
+
+    tqdm_settings: TqdmSettings = {
+        "total": len(input_files),
+        "desc": "Processing statements",
+        "leave": False,
+        "delay": 0.2,
+        "ncols": 80,
+        "bar_format": "{l_bar}{bar}| {n_fmt}/{total_fmt}",
+    }
+
+    if not single_process:
+        with ProcessPoolExecutor() as executor:
+            results = list(
+                tqdm(
+                    executor.map(
+                        process_statement,
+                        input_files,
+                        [output_directory] * len(input_files),
+                        [print_df] * len(input_files),
+                    ),
+                    **tqdm_settings,
+                )
             )
-        )
+
+    else:
+        results = []
+        for file in tqdm(input_files, **tqdm_settings):
+            result = process_statement(file, output_directory, print_df)
+            results.append(result)
 
     if any(results):
         # filter out null values, for cases where print_df is True
         # and processing errors occur to avoid pydantic validation errors
         report = Report([res for res in results if res])
         report.display_report()
 
@@ -181,34 +228,49 @@
     nargs=-1,
     type=click.Path(exists=True, allow_dash=True, resolve_path=True, path_type=Path),
 )
 @click.option(
     "-o",
     "--output",
     type=click.Path(exists=True, allow_dash=True, resolve_path=True, path_type=Path),
-    help="Specify output folder",
+    help="Specify output folder.",
 )
 @click.option(
     "-p",
     "--pprint",
     is_flag=True,
-    help="Print the processed statement(s)",
+    help="Print the processed statement(s).",
+)
+@click.option(
+    "-s",
+    "--single-process",
+    is_flag=True,
+    help=(
+        "Runs `monopoly` in single-threaded mode, even when processing "
+        "multiple files. Useful for debugging."
+    ),
 )
 @click.pass_context
-def monopoly(ctx: click.Context, files: list[Path], output: Path, pprint: bool):
+def monopoly(
+    ctx: click.Context,
+    files: list[Path],
+    output: Path,
+    pprint: bool,
+    single_process: bool,
+):
     """
     Monopoly helps convert your bank statements from PDF to CSV.
 
     A file or directory can be passed in via the FILES argument
     """
     if files:
         matched_files = get_statement_paths(files)
 
         if matched_files:
-            run(matched_files, output, pprint)
+            run(matched_files, output, pprint, single_process)
             ctx.exit(0)
 
         else:
             click.echo(
                 click.style("Could not find .pdf files", fg="yellow", bold=True),
                 err=True,
             )
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/config.py` & `monopoly_sg-0.8.1/src/monopoly/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from typing import Annotated, Optional
+import re
+from typing import Any, Optional
 
-from pydantic import SecretStr, StringConstraints
+from pydantic import ConfigDict, SecretStr
 from pydantic.dataclasses import dataclass
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from monopoly.constants import BankNames
 
 
 class PdfPasswords(BaseSettings):
@@ -12,72 +13,92 @@
     citibank_pdf_passwords: list[SecretStr] = [SecretStr("")]
     standard_chartered_pdf_passwords: list[SecretStr] = [SecretStr("")]
     hsbc_pdf_passwords: list[SecretStr] = [SecretStr("")]
 
     model_config = SettingsConfigDict(env_file=".env", extra="allow")
 
 
-class Settings(BaseSettings):
+class Passwords(BaseSettings):
     """
     Pydantic model that automatically populates variables from a .env file,
     or an environment variable called `passwords`.
     e.g. export PASSWORDS='{"OCBC_PDF_PASSWORDS": ...}'
     """
 
     passwords: PdfPasswords = PdfPasswords()
 
 
+@dataclass(frozen=True)
+class DateOrder:
+    """
+    Supported `dateparser` DATE_ORDER arguments can be found here:
+    https://dateparser.readthedocs.io/en/latest/settings.html#date-order
+    """
+
+    date_order: str
+
+    @property
+    def settings(self):
+        return {"DATE_ORDER": self.date_order}
+
+
 # pylint: disable=too-many-instance-attributes
-@dataclass
+@dataclass(kw_only=True)
 class StatementConfig:
     """
     Base configuration class storing configuration values for debit and
     credit card statements
 
     - `transaction_pattern` refers to the regex pattern used to capture transactions,
     where a pattern like:
         "(?P<transaction_date>\\d+/\\d+)\\s*"
         "(?P<description>.*?)\\s*"
         "(?P<amount>[\\d.,]+)$"
     is used to capture a transaction like:
         06/07 URBAN TRANSIT CO. SINGAPORE SG  1.38
-    - `transaction_date_format` represents the datetime format that a specific bank uses
-    for transactions. For example, "%d/%m" will match 06/07
+    - `transaction_date_order` represents the datetime format that a specific bank uses
+    for transactions. For example, "DMY" will parse 01/02/2024 as 1 Feb 2024.
+    Defaults to DMY.
     - `multiline_transactions` controls whether Monopoly tries to concatenate
     transactions that are split across two lines
     - `debit_statement_identifier` is a regex pattern that is used to determine whether
     a statement from a bank is a debit or credit card statement.
     """
 
     bank_name: BankNames
     transaction_pattern: str
-    transaction_date_format: Annotated[str, StringConstraints(pattern="%")]
     statement_date_pattern: str
-    statement_date_format: Annotated[str, StringConstraints(pattern="%.+%.+%")]
+    transaction_date_order: DateOrder = DateOrder("DMY")
+    statement_date_order: DateOrder = DateOrder("DMY")
     multiline_transactions: bool = False
-    debit_statement_identifier: Optional[str] = None
 
 
-@dataclass
+@dataclass(config=ConfigDict(extra="forbid"), kw_only=True)
 class DebitStatementConfig(StatementConfig):
     """
     Dataclass storing configuration values unique to debit statements
     """
 
+    debit_statement_identifier: str
 
-@dataclass
+
+@dataclass(config=ConfigDict(extra="forbid"))
 class CreditStatementConfig(StatementConfig):
     """
     Dataclass storing configuration values unique to credit statements
 
     - `prev_balance_pattern` is a regex pattern used to match the previous balance
     line in a credit statements, which is then treated as a transaction.
     """
 
-    prev_balance_pattern: Optional[str] = None
+    prev_balance_pattern: Optional[Any | re.Pattern] = None
+
+    def __post_init__(self):
+        if self.prev_balance_pattern:
+            self.prev_balance_pattern = re.compile(self.prev_balance_pattern)
 
 
 @dataclass
 class PdfConfig:
     """Stores PDF configuration values for the `PdfParser` class
 
     - `password`: The password used to unlock the PDF (if it is locked)
@@ -85,13 +106,12 @@
     example, a range of (1, -1) will mean that the first and last pages
     are skipped.
     - `page_bbox`: A tuple representing the bounding box range for every
     page. This is used to avoid weirdness like vertical text, and other
     PDF artifacts that may affect parsing.
     """
 
-    passwords: Optional[list[SecretStr]] = None
     page_range: tuple[Optional[int], Optional[int]] = (None, None)
     page_bbox: Optional[tuple[float, float, float, float]] = None
 
 
-settings = Settings().passwords
+passwords = Passwords().passwords
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/constants.py` & `monopoly_sg-0.8.1/src/monopoly/constants.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.8/src/monopoly/examples/example_statement.pdf` & `monopoly_sg-0.8.1/src/monopoly/examples/example_statement.pdf`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.8/src/monopoly/examples/single_statement.py` & `monopoly_sg-0.8.1/src/monopoly/examples/single_statement.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-from monopoly.processors import ExampleBankProcessor
+from monopoly.handler import StatementHandler
 
 
+# pylint: disable=duplicate-code
 def example():
     """Example showing how monopoly can be used to extract data from
     a single bank statement
     """
-    processor = ExampleBankProcessor(
-        file_path="src/monopoly/examples/example_statement.pdf",
-    )
+    handler = StatementHandler(file_path="src/monopoly/examples/example_statement.pdf")
 
     # This runs pdftotext on the PDF and
     # extracts transactions as raw text
-    statement = processor.extract()
+    statement = handler.extract()
 
     # Dates are converted into an ISO 8601 date format
-    transformed_df = processor.transform(statement)
-    print(transformed_df)
+    transactions = handler.transform(
+        transactions=statement.transactions,
+        statement_date=statement.statement_date,
+        transaction_date_order=statement.config.transaction_date_order,
+    )
 
     # Parsed transactions writen to a CSV file in the "example" directory
-    processor.load(transformed_df, statement, output_directory="src/monopoly/examples")
+    handler.load(
+        transactions=transactions,
+        statement=statement,
+        output_directory="src/monopoly/examples",
+    )
 
 
 if __name__ == "__main__":
     example()
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/pdf.py` & `monopoly_sg-0.8.1/src/monopoly/pdf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,44 @@
 import logging
-from dataclasses import dataclass
-from functools import cached_property
+from dataclasses import dataclass, field
+from functools import cached_property, lru_cache
 from io import BytesIO
 from pathlib import Path
-from typing import Optional
+from typing import Any, Optional
 
 import fitz
 import pdftotext
-from pdf2john import PdfHashExtractor as EncryptionMetadataExtractor
 from pydantic import SecretStr
 
-from monopoly.config import PdfConfig
+from monopoly.banks import detect_bank
+from monopoly.constants import EncryptionIdentifier, MetadataIdentifier
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
+class EncryptDict:
+    """Stores encryption dictionary of a PDF"""
+
+    raw_encrypt_dict: dict
+    pdf_version: str
+    algorithm: int = field(init=False)
+    length: int = field(init=False)
+    permissions: int = field(init=False)
+    revision: int = field(init=False)
+
+    def __post_init__(self):
+        self.pdf_version = float(self.pdf_version[-3:])
+        self.algorithm = int(self.raw_encrypt_dict.get("V"))
+        self.length = int(self.raw_encrypt_dict.get("Length"))
+        self.permissions = int(self.raw_encrypt_dict.get("P"))
+        self.revision = int(self.raw_encrypt_dict.get("R"))
+
+
+@dataclass
 class PdfPage:
     """
     Dataclass representation of a bank statement PDF page.
     Contains the raw text of a PDF page, and allows access
     to the raw text as a list via the `lines` property
     """
 
@@ -41,33 +60,75 @@
 class BadPasswordFormatError(Exception):
     """Exception raised passwords are not provided in a proper format"""
 
 
 class PdfParser:
     def __init__(
         self,
+        passwords: Optional[list[SecretStr]] = None,
         file_path: Optional[Path] = None,
         file_bytes: Optional[bytes] = None,
-        pdf_config: Optional[PdfConfig] = None,
     ):
         """
         Class responsible for parsing PDFs and returning raw text
 
         The page_range variable determines which pages are extracted.
         All pages are extracted by default.
         """
+        self._passwords = passwords
         self.file_path = file_path
         self.file_bytes = file_bytes
 
-        if pdf_config is None:
-            pdf_config = PdfConfig()
+    @property
+    def bank(self):
+        return detect_bank(self.metadata_items)
+
+    @property
+    def passwords(self):
+        if not self._passwords:
+            return self.bank.passwords
+        return self._passwords
+
+    @property
+    def pdf_config(self):
+        return self.bank.pdf_config
+
+    @cached_property
+    def page_range(self):
+        return slice(*self.pdf_config.page_range)
+
+    @cached_property
+    def page_bbox(self):
+        return self.pdf_config.page_bbox
+
+    @property
+    def metadata_items(self) -> list[Any]:
+        """
+        Retrieves encryption and metadata identifiers from a bank statement PDF
+        """
+        identifiers = []
+        # pylint: disable=protected-access
+        if encrypt_dict := self.encrypt_dict:
+            encryption_identifier = EncryptionIdentifier(
+                float(encrypt_dict.pdf_version),
+                encrypt_dict.algorithm,
+                encrypt_dict.revision,
+                encrypt_dict.length,
+                encrypt_dict.permissions,
+            )
+            identifiers.append(encryption_identifier)
+
+        if metadata := self.document.metadata:
+            metadata_identifier = MetadataIdentifier(**metadata)
+            identifiers.append(metadata_identifier)  # type: ignore
+
+        if not identifiers:
+            raise ValueError("Could not get identifier")
 
-        self.passwords = pdf_config.passwords
-        self.page_range = slice(*pdf_config.page_range)
-        self.page_bbox = pdf_config.page_bbox
+        return identifiers
 
     def open(self):
         """
         Opens and decrypts a PDF document
         """
         document = self.document
 
@@ -90,14 +151,15 @@
             document.authenticate(password.get_secret_value())
 
             if not document.is_encrypted:
                 logger.debug("Successfully authenticated with password")
                 return document
         raise WrongPasswordError(f"Could not open document: {document.name}")
 
+    @lru_cache
     def get_pages(self) -> list[PdfPage]:
         logger.debug("Extracting text from PDF")
         document: fitz.Document = self.open()
 
         num_pages = list(range(document.page_count))
         document.select(num_pages[self.page_range])
 
@@ -125,35 +187,35 @@
         raise RuntimeError("Unable to retrieve pages")
 
     @cached_property
     def document(self) -> fitz.Document:
         """
         Returns a Python representation of a PDF document.
         """
-        if self.file_path:
-            return fitz.Document(filename=self.file_path)
+        if not self.file_path and not self.file_bytes:
+            raise RuntimeError("Either `file_path` or `file_bytes` must be passed")
 
-        if self.file_bytes:
-            return fitz.Document(stream=self.file_bytes)
+        if self.file_path and self.file_bytes:
+            raise RuntimeError(
+                "Only one of `file_path` or `file_bytes` should be defined"
+            )
 
-        raise RuntimeError("Either file path or file bytestream must be passed")
+        args = {"filename": self.file_path, "stream": self.file_bytes}
+        return fitz.Document(**args)
 
     @cached_property
-    def extractor(self) -> EncryptionMetadataExtractor:
-        """
-        Returns an instance of pdf2john, used to retrieve and return
-        the encryption metadata from a PDF's encryption dictionary
-        """
-        if self.file_path:
-            return EncryptionMetadataExtractor(file_name=self.file_path)
-
-        if self.file_bytes:
-            return EncryptionMetadataExtractor(file_bytes=self.file_bytes)
-
-        raise RuntimeError("Either file path or file bytestream must be passed")
+    def encrypt_dict(self) -> EncryptDict | None:
+        stream = self._get_doc_byte_stream()
+        pdf_version_string = stream.read(8).decode("utf-8", "backslashreplace")
+
+        if self.document.is_encrypted:
+            raw_encrypt_dict = self._get_raw_encrypt_dict(self.document)
+            encrypt_dict = EncryptDict(raw_encrypt_dict, pdf_version_string)
+            return encrypt_dict
+        return None
 
     @staticmethod
     def _remove_vertical_text(page: fitz.Page):
         """Helper function to remove vertical text, based on writing direction (wdir).
 
         This helps avoid situations where the PDF is oddly parsed, due to vertical text
         inside the PDF.
@@ -173,7 +235,30 @@
         for block in page.get_text("dict", flags=fitz.TEXTFLAGS_TEXT)["blocks"]:
             for line in block["lines"]:
                 writing_direction = line["dir"]
                 if writing_direction != (1, 0):
                     page.add_redact_annot(line["bbox"])
         page.apply_redactions(images=fitz.PDF_REDACT_IMAGE_NONE)
         return page
+
+    @staticmethod
+    def _get_raw_encrypt_dict(doc: fitz.Document) -> dict:
+        """
+        Helper function to extract the PDF encryption dictionary, since
+        `fitz` doesn't provide it
+        """
+        encrypt_metadata = {}
+        pdf_object, value = doc.xref_get_key(-1, "Encrypt")
+        if pdf_object != "xref":
+            pass  # PDF has no metadata
+        else:
+            xref = int(value.replace("0 R", ""))  # extract the metadata xref
+            for key in doc.xref_get_keys(xref):
+                encrypt_metadata[key] = doc.xref_get_key(xref, key)[1]
+        return encrypt_metadata
+
+    def _get_doc_byte_stream(self) -> BytesIO:
+        if self.file_path:
+            with open(self.file_path, "rb") as file:
+                stream = BytesIO(file.read())
+            return stream
+        raise RuntimeError("Unable to create stream since `file_path` not passed")
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processor.py` & `monopoly_sg-0.8.1/src/monopoly/handler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,110 +1,135 @@
+import csv
 import logging
 from datetime import datetime
 from pathlib import Path
 
-from pandas import DataFrame
+from dateparser import parse
 
-from monopoly.config import CreditStatementConfig, DebitStatementConfig
-from monopoly.constants import StatementFields
+from monopoly.config import DateOrder
 from monopoly.pdf import PdfParser
 from monopoly.statements import CreditStatement, DebitStatement
+from monopoly.statements.transaction import Transaction
 from monopoly.write import generate_name
 
 logger = logging.getLogger(__name__)
 
 
-class StatementProcessor:
+class StatementHandler:
     """
     Handles extract, transform and load (ETL) logic for bank statements
 
     Transactions are extracted from pages, before undergoing various
     transformations like converting various date formats into ISO 8601.
     Transformed statements are then written to a CSV file.
     """
 
-    credit_config: CreditStatementConfig
-    debit_config: DebitStatementConfig
-    statement: CreditStatement | DebitStatement
-
     def __init__(
         self,
-        file_name: str,
-        parser: PdfParser,
-        statement: CreditStatement | DebitStatement,
+        file_path: Path,
     ):
-        self.file_name = file_name
-        self.parser = parser
-        self.statement = statement
+        self.parser = PdfParser(file_path=file_path)
+        self.statement = self.get_statement(self.parser)
+        self.transactions = self.statement.transactions
+
+    @staticmethod
+    def get_statement(parser: PdfParser) -> CreditStatement | DebitStatement:
+        bank = parser.bank
+        debit_config, credit_config = bank.debit_config, bank.credit_config
+
+        if debit_config:
+            debit_statement = DebitStatement(parser, debit_config)
+            if debit_statement.debit_header:
+                return debit_statement
+
+        # if it's not a debit statement, assume that it's a credit statement
+        return CreditStatement(parser, credit_config)
 
     def extract(self) -> CreditStatement | DebitStatement:
         """Extracts transactions from the statement, and performs
         a safety check to make sure that total transactions add up"""
-        statement = self.statement
-
-        if not statement.transactions:
+        if not self.statement.transactions:
             raise ValueError("No transactions found - statement extraction failed")
 
-        if not statement.statement_date:
+        if not self.statement.statement_date:
             raise ValueError("No statement date found")
 
-        statement.perform_safety_check()
+        self.statement.perform_safety_check()
 
-        return statement
+        return self.statement
 
-    def transform(self, statement: CreditStatement | DebitStatement) -> DataFrame:
+    @staticmethod
+    def transform(
+        transactions: list[Transaction],
+        statement_date: datetime,
+        transaction_date_order: DateOrder,
+    ) -> list[Transaction]:
         logger.debug("Running transformation functions on DataFrame")
 
-        df = statement.df
-        statement_date = statement.statement_date
-        date_format = statement.statement_config.transaction_date_format
-
-        def convert_date(row, date_format):
+        def convert_date(transaction: Transaction, transaction_date_order: DateOrder):
             """
             Converts each date to a ISO 8601 (YYYY-MM-DD) format.
 
             Implements cross-year logic by attributing transactions from
             October, November, and December to the previous year if
             the statement month is January.
             e.g. if the statement month is Jan/Feb 2024, transactions from
             Oct/Nov/Dec should be attributed to the previous year.
             """
-            if "%Y" not in date_format and "%y" not in date_format:
-                date_format += " %Y"
-                row[StatementFields.TRANSACTION_DATE] += f" {statement_date.year}"
-
-            parsed_date = datetime.strptime(
-                row[StatementFields.TRANSACTION_DATE], date_format
+            transaction.transaction_date += f" {statement_date.year}"
+            parsed_date = parse(
+                transaction.transaction_date,
+                settings=transaction_date_order.settings,
             )
-            if statement_date.month in (1, 2) and parsed_date.month > 2:
-                parsed_date = parsed_date.replace(year=parsed_date.year - 1)
+            if parsed_date:
+                if statement_date.month in (1, 2) and parsed_date.month > 2:
+                    parsed_date = parsed_date.replace(year=parsed_date.year - 1)
 
-            return parsed_date.isoformat()[:10]
+                return parsed_date.isoformat()[:10]
+            raise RuntimeError("Could not convert date")
 
         logger.debug("Transforming dates to ISO 8601")
-        df[StatementFields.TRANSACTION_DATE] = df.apply(
-            convert_date, args=(date_format,), axis=1
-        )
-        return df
+
+        for transaction in transactions:
+            transaction.transaction_date = convert_date(
+                transaction, transaction_date_order
+            )
+        return transactions
 
     def load(
         self,
-        df: DataFrame,
+        transactions: list[Transaction],
         statement: CreditStatement | DebitStatement,
         output_directory: Path,
     ):
         if isinstance(output_directory, str):
             output_directory = Path(output_directory)
 
         filename = generate_name(
             document=self.parser.document,
             format_type="file",
-            statement_config=statement.statement_config,
+            statement_config=statement.config,
             statement_type=statement.statement_type,
             statement_date=statement.statement_date,
         )
 
         output_path = output_directory / filename
         logger.debug("Writing CSV to file path: %s", output_path)
-        df.to_csv(output_path, index=False)
+
+        with open(output_path, mode="w", encoding="utf8") as file:
+            writer = csv.writer(file)
+
+            # header
+            writer.writerow(statement.columns)
+
+            for transaction in transactions:
+                writer.writerow(
+                    (
+                        [
+                            transaction.transaction_date,
+                            transaction.description,
+                            transaction.amount,
+                        ]
+                    )
+                )
 
         return output_path
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processors/__init__.py` & `monopoly_sg-0.8.1/src/monopoly/banks/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,100 @@
 import logging
 from dataclasses import Field, fields
 from itertools import product
-from pathlib import Path
-from typing import Optional, Type
+from typing import Type
 
-from pydantic import SecretStr
-
-from monopoly.config import PdfConfig
 from monopoly.constants import EncryptionIdentifier, MetadataIdentifier
-from monopoly.pdf import PdfParser
 
-from .base import ProcessorBase
+from ..examples.example_bank import ExampleBankProcessor
+from .base import BankBase
 from .citibank import Citibank
 from .dbs import Dbs
-from .example_bank import ExampleBankProcessor
 from .hsbc import Hsbc
 from .ocbc import Ocbc
 from .standard_chartered import StandardChartered
 
-processors: list[Type[ProcessorBase]] = [
+banks: list[Type[BankBase]] = [
     Citibank,
     Dbs,
     ExampleBankProcessor,
     Hsbc,
     Ocbc,
     StandardChartered,
 ]
 
-
 logger = logging.getLogger(__name__)
 
 
 class UnsupportedBankError(Exception):
     """Raised when a processor cannot be found for a specific bank"""
 
 
-def detect_processor(
-    file_path: Optional[Path] = None,
-    file_bytes: Optional[bytes] = None,
-    passwords: Optional[list[SecretStr]] = None,
-) -> ProcessorBase:
+def detect_bank(
+    metadata_items: list[EncryptionIdentifier | MetadataIdentifier],
+) -> Type[BankBase]:
     """
     Reads the encryption metadata or actual metadata (if the PDF is not encrypted),
     and checks for a bank based on unique identifiers.
     """
-    parser = PdfParser(
-        file_path=file_path,
-        file_bytes=file_bytes,
-        pdf_config=PdfConfig(passwords=passwords),
-    )
-    for processor in processors:
-        metadata_items = processor.get_identifiers(parser)
-        if is_bank_identified(metadata_items, processor):
-            return processor(
-                file_path=file_path, file_bytes=file_bytes, passwords=passwords
-            )
+    for bank in banks:
+        if is_bank_identified(metadata_items, bank):
+            return bank
 
-    raise UnsupportedBankError("This bank is currently unsupported")
+    raise UnsupportedBankError("This bank is currently not supported")
 
 
 def is_bank_identified(
     metadata_items: list[EncryptionIdentifier | MetadataIdentifier],
-    processor: Type[ProcessorBase],
+    bank: Type[BankBase],
 ) -> bool:
     """
     Checks if a bank is identified based on a list of metadata items.
     """
-    for identifier, metadata in product(processor.identifiers, metadata_items):
+    for identifier, metadata in product(
+        bank.identifiers, metadata_items
+    ):  # type: ignore
         logger.debug(
             "Comparing bank %s identifier %s against PDF metadata %s",
-            processor.__name__,
+            bank.__name__,
             identifier,
             metadata,
         )
+
         if all(
             check_matching_field(field, metadata, identifier)
             for field in fields(metadata)
         ):
+            logger.debug("Match found for bank %s", bank.__name__)
             return True
+
     return False
 
 
 def check_matching_field(
     field: Field,
     metadata: EncryptionIdentifier | MetadataIdentifier,
     identifier: EncryptionIdentifier | MetadataIdentifier,
 ) -> bool:
     """
     Checks if a field in the metadata matches the corresponding identifier field.
     """
     # Only compare matching identifier types
-    if type(metadata) is type(identifier):
-        field_value = getattr(metadata, field.name)
-        identifier_value = getattr(identifier, field.name)
-
-        # allow for partial string matching
-        if isinstance(field.type(), str):
-            return identifier_value in field_value
+    if type(metadata) is not type(identifier):
+        return False
+
+    field_value = getattr(metadata, field.name)
+    identifier_value = getattr(identifier, field.name)
+
+    # allow for partial string matching
+    partial_string_match = (
+        isinstance(field.type(), str) and identifier_value in field_value
+    )
+
+    # other types should match exactly
+    full_match = identifier_value == field_value
+
+    if any([partial_string_match, full_match]):
+        logger.debug("Match: %s - %s", identifier_value, field_value)
+        return True
 
-        # otherwise check that values match exactly
-        return identifier_value == field_value
     return False
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processors/citibank/citibank.py` & `monopoly_sg-0.8.1/src/monopoly/banks/citibank/citibank.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import logging
 
-from monopoly.config import CreditStatementConfig, PdfConfig, settings
+from monopoly.config import CreditStatementConfig, PdfConfig, passwords
 from monopoly.constants import (
     BankNames,
     CreditTransactionPatterns,
     MetadataIdentifier,
     StatementBalancePatterns,
 )
 
-from ..base import ProcessorBase
+from ..base import BankBase
 
 logger = logging.getLogger(__name__)
 
 
-class Citibank(ProcessorBase):
+class Citibank(BankBase):
     credit_config = CreditStatementConfig(
         bank_name=BankNames.CITIBANK,
         statement_date_pattern=r"Statement\sDate\s+(.*)",
-        statement_date_format=r"%B %d, %Y",
         prev_balance_pattern=StatementBalancePatterns.CITIBANK,
         transaction_pattern=CreditTransactionPatterns.CITIBANK,
-        transaction_date_format="%d %b",
     )
 
     pdf_config = PdfConfig(
-        passwords=settings.citibank_pdf_passwords,
         page_bbox=(20, 0, 595, 840),
         page_range=(0, -3),
     )
 
     identifiers = [
         MetadataIdentifier(
             creator="Ricoh Americas Corporation, AFP2PDF",
             producer="Ricoh Americas Corporation, AFP2PDF",
         )
     ]
+
+    passwords = passwords.citibank_pdf_passwords
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processors/dbs/dbs.py` & `monopoly_sg-0.8.1/src/monopoly/banks/ocbc/ocbc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import logging
 
-from monopoly.config import CreditStatementConfig, DebitStatementConfig
+from monopoly.config import CreditStatementConfig, DebitStatementConfig, passwords
 from monopoly.constants import (
     BankNames,
     CreditTransactionPatterns,
     DebitTransactionPatterns,
     EncryptionIdentifier,
     MetadataIdentifier,
     StatementBalancePatterns,
 )
 
-from ..base import ProcessorBase
+from ..base import BankBase
 
 logger = logging.getLogger(__name__)
 
 
-class Dbs(ProcessorBase):
+class Ocbc(BankBase):
     credit_config = CreditStatementConfig(
-        bank_name=BankNames.DBS,
-        statement_date_pattern=r"(\d{2}\s[A-Za-z]{3}\s\d{4})",
-        statement_date_format=r"%d %b %Y",
-        transaction_date_format=r"%d %b",
-        multiline_transactions=True,
-        transaction_pattern=CreditTransactionPatterns.DBS,
-        prev_balance_pattern=StatementBalancePatterns.DBS,
+        bank_name=BankNames.OCBC,
+        statement_date_pattern=r"(\d{2}\-\d{2}\-\d{4})",
+        prev_balance_pattern=StatementBalancePatterns.OCBC,
+        transaction_pattern=CreditTransactionPatterns.OCBC,
     )
 
     debit_config = DebitStatementConfig(
-        bank_name=BankNames.DBS,
-        statement_date_pattern=r"(\d{2}\s[A-Za-z]{3}\s\d{4})",
-        statement_date_format=r"%d %b %Y",
-        transaction_date_format=r"%d %b",
+        bank_name=BankNames.OCBC,
+        statement_date_pattern=r"(\d+\s[A-Za-z]{3}\s\d{4})",
+        debit_statement_identifier=r"(Withdrawal.*Deposit.*Balance)",
+        transaction_pattern=DebitTransactionPatterns.OCBC,
         multiline_transactions=True,
-        debit_statement_identifier=r"(WITHDRAWAL.*DEPOSIT.*BALANCE)",
-        transaction_pattern=DebitTransactionPatterns.DBS,
     )
 
     identifiers = [
         EncryptionIdentifier(
-            pdf_version=1.4, algorithm=2, revision=3, length=128, permissions=-1852
+            pdf_version=1.4, algorithm=4, revision=4, length=128, permissions=-1036
+        ),
+        MetadataIdentifier(
+            creator="pdfgen", producer="Streamline PDFGen for OCBC Group"
         ),
-        MetadataIdentifier(creator="Quadient CXM AG"),
     ]
+
+    passwords = passwords.ocbc_pdf_passwords
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processors/example_bank.py` & `monopoly_sg-0.8.1/src/monopoly/examples/example_bank.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,26 @@
+from monopoly.banks.base import BankBase
 from monopoly.config import CreditStatementConfig
 from monopoly.constants import BankNames, MetadataIdentifier, SharedPatterns
-from monopoly.processors.base import ProcessorBase
 
 
-class ExampleBankProcessor(ProcessorBase):
+class ExampleBankProcessor(BankBase):
     """Dummy class to help with reading the example PDF statement"""
 
     credit_config = CreditStatementConfig(
         bank_name=BankNames.EXAMPLE,
         statement_date_pattern=r"(\d{2}\-\d{2}\-\d{4})",
-        statement_date_format=r"%d-%m-%Y",
         prev_balance_pattern=(
             r"(?P<description>LAST MONTH'S BALANCE?)\s+" + SharedPatterns.AMOUNT
         ),
         transaction_pattern=(
             r"(?P<transaction_date>\d+/\d+)\s*"
             + SharedPatterns.DESCRIPTION
             + SharedPatterns.AMOUNT_EXTENDED
         ),
-        transaction_date_format=r"%d/%m",
     )
 
     identifiers = [
         MetadataIdentifier(
             creator="Adobe Acrobat 23.3", producer="Adobe Acrobat Pro (64-bit)"
         )
     ]
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processors/hsbc/hsbc.py` & `monopoly_sg-0.8.1/src/monopoly/banks/dbs/dbs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import logging
 
-from monopoly.config import CreditStatementConfig, PdfConfig, settings
+from monopoly.config import CreditStatementConfig, DebitStatementConfig
 from monopoly.constants import (
     BankNames,
     CreditTransactionPatterns,
+    DebitTransactionPatterns,
     EncryptionIdentifier,
     MetadataIdentifier,
     StatementBalancePatterns,
 )
 
-from ..base import ProcessorBase
+from ..base import BankBase
 
 logger = logging.getLogger(__name__)
 
 
-class Hsbc(ProcessorBase):
+class Dbs(BankBase):
     credit_config = CreditStatementConfig(
-        bank_name=BankNames.HSBC,
-        statement_date_pattern=r"Statement From .* to (\d{2}\s[A-Z]{3}\s\d{4})",
-        prev_balance_pattern=StatementBalancePatterns.HSBC,
-        statement_date_format=r"%d %b %Y",
-        transaction_pattern=CreditTransactionPatterns.HSBC,
-        transaction_date_format="%d %b",
+        bank_name=BankNames.DBS,
+        statement_date_pattern=r"(\d{2}\s[A-Za-z]{3}\s\d{4})",
         multiline_transactions=True,
+        transaction_pattern=CreditTransactionPatterns.DBS,
+        prev_balance_pattern=StatementBalancePatterns.DBS,
     )
 
-    pdf_config = PdfConfig(
-        passwords=settings.hsbc_pdf_passwords,
-        page_bbox=(0, 0, 379, 842),
+    debit_config = DebitStatementConfig(
+        bank_name=BankNames.DBS,
+        statement_date_pattern=r"(\d{2}\s[A-Za-z]{3}\s\d{4})",
+        multiline_transactions=True,
+        debit_statement_identifier=r"(WITHDRAWAL.*DEPOSIT.*BALANCE)",
+        transaction_pattern=DebitTransactionPatterns.DBS,
     )
 
     identifiers = [
         EncryptionIdentifier(
-            pdf_version=1.6, algorithm=4, revision=4, length=128, permissions=-1804
-        ),
-        MetadataIdentifier(
-            title="PRJ_BEAGLE_ST_CNS_SGH_APP_Orchid",
-            creator="OpenText Exstream",
+            pdf_version=1.4, algorithm=2, revision=3, length=128, permissions=-1852
         ),
+        MetadataIdentifier(creator="Quadient CXM AG"),
     ]
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/processors/standard_chartered/standard_chartered.py` & `monopoly_sg-0.8.1/src/monopoly/banks/standard_chartered/standard_chartered.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import logging
 
-from monopoly.config import CreditStatementConfig, PdfConfig, settings
+from monopoly.config import CreditStatementConfig, PdfConfig, passwords
 from monopoly.constants import (
     BankNames,
     CreditTransactionPatterns,
     MetadataIdentifier,
     StatementBalancePatterns,
 )
 
-from ..base import ProcessorBase
+from ..base import BankBase
 
 logger = logging.getLogger(__name__)
 
 
-class StandardChartered(ProcessorBase):
+class StandardChartered(BankBase):
     credit_config = CreditStatementConfig(
         bank_name=BankNames.STANDARD_CHARTERED,
         statement_date_pattern=r"(\d{2}\s\w+\s\d{4})",
-        statement_date_format=r"%d %b %Y",
         prev_balance_pattern=StatementBalancePatterns.STANDARD_CHARTERED,
         transaction_pattern=CreditTransactionPatterns.STANDARD_CHARTERED,
-        transaction_date_format="%d %b",
     )
 
     pdf_config = PdfConfig(
-        passwords=settings.standard_chartered_pdf_passwords,
         page_range=(0, -1),
         page_bbox=(0, 0, 580, 820),
     )
 
     identifiers = [
         MetadataIdentifier(
             title="eStatement",
             producer="iText",
         )
     ]
+
+    passwords = passwords.standard_chartered_pdf_passwords
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/statements/credit_statement.py` & `monopoly_sg-0.8.1/src/monopoly/statements/credit_statement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,70 @@
 import logging
 import re
-from functools import cached_property
-from typing import Any
-
-import fitz
 
 from monopoly.config import CreditStatementConfig
-from monopoly.constants import AccountType, StatementFields
-from monopoly.pdf import PdfPage
+from monopoly.constants import AccountType
+from monopoly.statements.transaction import Transaction, TransactionGroupDict
 
-from .base import BaseStatement, SafetyCheckError, Transaction
+from .base import BaseStatement, SafetyCheckError
 
 logger = logging.getLogger(__name__)
 
 
 class CreditStatement(BaseStatement):
     """
     A dataclass representation of a credit statement
     """
 
-    def __init__(
-        self,
-        document: fitz.Document,
-        pages: list[PdfPage],
-        credit_config: CreditStatementConfig,
-    ):
-        self.config = credit_config
-        self.statement_type = AccountType.CREDIT
-        super().__init__(document, pages, credit_config)
+    statement_type = AccountType.CREDIT
+
+    def post_process_transactions(self, transactions) -> list[Transaction]:
+        previous_month_balances = self.get_prev_month_balances()
+        if previous_month_balances:
+            first_transaction_date = next(iter(transactions)).transaction_date
+            for prev_month_balance in previous_month_balances:
+                groupdict = TransactionGroupDict(**prev_month_balance.groupdict())
+                groupdict.transaction_date = first_transaction_date
+                prev_month_transaction = Transaction(**groupdict)
+                transactions.insert(0, prev_month_transaction)
+        return transactions
 
-    @cached_property
-    def prev_month_balance(self) -> list[Transaction]:
+    def get_prev_month_balances(self) -> list[re.Match]:
         """
         Returns the previous month's statement balance as a transaction,
         if it exists in the statement.
 
-        The date is later replaced with a more accurate date by the statement processor.
+        The date is later replaced with a more accurate date by the statement handler.
         """
         prev_balances = []
-        if prev_balance_pattern := self.config.prev_balance_pattern:
-            raw_text = "".join(page.raw_text for page in self.pages)
-            matches = re.finditer(prev_balance_pattern, raw_text)
-
-            for match in matches:
-                groupdict: dict[str, Any] = match.groupdict()
-                groupdict[StatementFields.TRANSACTION_DATE] = "1900-01-01"
-                prev_balances.append(Transaction(**groupdict))
-
-        return prev_balances
 
-    @cached_property
-    def account_type(self) -> str:
-        return AccountType.CREDIT
+        if isinstance(self.config, CreditStatementConfig):
+            if pattern := self.config.prev_balance_pattern:
+                raw_text = "".join(page.raw_text for page in self.pages)
+                matches = pattern.finditer(raw_text)
 
-    def _inject_prev_month_balance(self, transactions: list[Transaction]):
-        """
-        Injects the previous month's balance as a transaction, if it exists
-        """
-        if self.prev_month_balance:
-            first_transaction_date = transactions[0].transaction_date
-            for prev_month_balance in self.prev_month_balance:
-                prev_month_balance.transaction_date = first_transaction_date
-                transactions.insert(0, prev_month_balance)
-        return transactions
+                for match in matches:
+                    prev_balances.append(match)
 
-    @cached_property
-    def transactions(self) -> list[Transaction]:
-        transactions = self._inject_prev_month_balance(super().transactions)
-        return transactions
+        return prev_balances
 
     def perform_safety_check(self) -> bool:
         """Checks that the total sum of all transactions is present
         somewhere within the document
 
         Text is re-extracted from the page, as some bank-specific bounding-box
         configurations (e.g. HSBC) may preclude the total from being extracted
 
         Returns `False` if the total does not exist in the document.
         """
-        df = self.df
-        amount = StatementFields.AMOUNT
         numbers = self.get_all_numbers_from_document()
+        transactions = self.transactions
 
-        total_amount = abs(round(df[amount].sum(), 2))
+        amounts = [transaction.amount for transaction in transactions]
+        total_amount = abs(round(sum(amounts), 2))
 
         result = total_amount in numbers
         if not result:
             raise SafetyCheckError(
                 f"Total amount {total_amount} cannot be found in credit statement"
             )
```

### Comparing `monopoly_sg-0.7.8/src/monopoly/write.py` & `monopoly_sg-0.8.1/src/monopoly/write.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,26 +33,24 @@
     month will not overwrite each other.
     """
     bank_name = statement_config.bank_name
     year = statement_date.year
     month = statement_date.month
     file_uuid = generate_hash(document)
 
-    file_suffix = "csv"
+    filename = f"{bank_name}-{statement_type}-{year}-{month:02d}-{file_uuid}.csv"
 
-    filename = (
-        f"{bank_name}-{statement_type}-{year}-{month:02d}-{file_uuid}.{file_suffix}"
-    )
-
-    if format_type == "blob":
-        return (
+    formats = {
+        "blob": (
             f"bank_name={bank_name}/"
             f"account_type={statement_type}/"
             f"year={year}/"
             f"month={month}/"
             f"{filename}"
-        )
+        ),
+        "file": filename,
+    }
 
-    if format_type == "file":
-        return filename
+    if format_type in formats:
+        return formats[format_type]
 
     raise ValueError("Invalid format_type")
```

### Comparing `monopoly_sg-0.7.8/tests/test_utils/skip.py` & `monopoly_sg-0.8.1/tests/test_utils/skip.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.8/PKG-INFO` & `monopoly_sg-0.8.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6f 6e6f  : 2.1.Name: mono
 00000020: 706f 6c79 2d73 670a 5665 7273 696f 6e3a  poly-sg.Version:
-00000030: 2030 2e37 2e38 0a53 756d 6d61 7279 3a20   0.7.8.Summary: 
+00000030: 2030 2e38 2e31 0a53 756d 6d61 7279 3a20   0.8.1.Summary: 
 00000040: 5044 4620 7061 7273 696e 6720 666f 7220  PDF parsing for 
 00000050: 5369 6e67 6170 6f72 6561 6e20 6261 6e6b  Singaporean bank
 00000060: 730a 486f 6d65 2d70 6167 653a 2068 7474  s.Home-page: htt
 00000070: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000080: 6265 6e6a 616d 696e 2d61 7764 2f6d 6f6e  benjamin-awd/mon
 00000090: 6f70 6f6c 790a 4c69 6365 6e73 653a 204d  opoly.License: M
 000000a0: 4954 0a41 7574 686f 723a 2062 656e 6a61  IT.Author: benja
@@ -25,201 +25,211 @@
 00000180: 5079 7468 6f6e 203a 3a20 330a 436c 6173  Python :: 3.Clas
 00000190: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
 000001a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
 000001b0: 5079 7468 6f6e 203a 3a20 332e 3131 0a52  Python :: 3.11.R
 000001c0: 6571 7569 7265 732d 4469 7374 3a20 636c  equires-Dist: cl
 000001d0: 6963 6b20 283e 3d38 2e31 2e37 2c3c 392e  ick (>=8.1.7,<9.
 000001e0: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
-000001f0: 7374 3a20 6d79 7079 2028 3e3d 312e 372e  st: mypy (>=1.7.
-00000200: 312c 3c32 2e30 2e30 290a 5265 7175 6972  1,<2.0.0).Requir
-00000210: 6573 2d44 6973 743a 2070 616e 6461 7320  es-Dist: pandas 
-00000220: 283e 3d32 2e31 2e33 2c3c 332e 302e 3029  (>=2.1.3,<3.0.0)
-00000230: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000240: 7064 6632 6a6f 686e 2028 3e3d 302e 322e  pdf2john (>=0.2.
-00000250: 302c 3c30 2e33 2e30 290a 5265 7175 6972  0,<0.3.0).Requir
-00000260: 6573 2d44 6973 743a 2070 6466 746f 7465  es-Dist: pdftote
-00000270: 7874 2028 3e3d 322e 322e 322c 3c33 2e30  xt (>=2.2.2,<3.0
-00000280: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000290: 743a 2070 7964 616e 7469 6320 283e 3d32  t: pydantic (>=2
-000002a0: 2e35 2e32 2c3c 332e 302e 3029 0a52 6571  .5.2,<3.0.0).Req
-000002b0: 7569 7265 732d 4469 7374 3a20 7079 6461  uires-Dist: pyda
-000002c0: 6e74 6963 2d73 6574 7469 6e67 7320 283e  ntic-settings (>
-000002d0: 3d32 2e30 2e33 2c3c 332e 302e 3029 0a52  =2.0.3,<3.0.0).R
-000002e0: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-000002f0: 6d75 7064 6620 283e 3d31 2e32 332e 372c  mupdf (>=1.23.7,
-00000300: 3c32 2e30 2e30 290a 5265 7175 6972 6573  <2.0.0).Requires
-00000310: 2d44 6973 743a 2074 6162 756c 6174 6520  -Dist: tabulate 
-00000320: 283e 3d30 2e39 2e30 2c3c 302e 3130 2e30  (>=0.9.0,<0.10.0
-00000330: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000340: 2074 7164 6d20 283e 3d34 2e36 362e 312c   tqdm (>=4.66.1,
-00000350: 3c35 2e30 2e30 290a 5072 6f6a 6563 742d  <5.0.0).Project-
-00000360: 5552 4c3a 2052 6570 6f73 6974 6f72 792c  URL: Repository,
-00000370: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000380: 636f 6d2f 6265 6e6a 616d 696e 2d61 7764  com/benjamin-awd
-00000390: 2f6d 6f6e 6f70 6f6c 790a 4465 7363 7269  /monopoly.Descri
-000003a0: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-000003b0: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-000003c0: 6e0a 0a21 5b5d 2868 7474 7073 3a2f 2f72  n..![](https://r
-000003d0: 6177 2e67 6974 6875 6275 7365 7263 6f6e  aw.githubusercon
-000003e0: 7465 6e74 2e63 6f6d 2f62 656e 6a61 6d69  tent.com/benjami
-000003f0: 6e2d 6177 642f 6d6f 6e6f 706f 6c79 2f6d  n-awd/monopoly/m
-00000400: 6169 6e2f 646f 6373 2f6c 6f67 6f2e 7376  ain/docs/logo.sv
-00000410: 6729 0a0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  g)..------------
-00000420: 2d2d 2d2d 2d0a 0a5b 215b 5465 7374 735d  -----..[![Tests]
-00000430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000440: 636f 6d2f 6265 6e6a 616d 696e 2d61 7764  com/benjamin-awd
-00000450: 2f6d 6f6e 6f70 6f6c 792f 6163 7469 6f6e  /monopoly/action
-00000460: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000470: 732e 7961 6d6c 2f62 6164 6765 2e73 7667  s.yaml/badge.svg
-00000480: 3f62 7261 6e63 683d 6d61 696e 2665 7665  ?branch=main&eve
-00000490: 6e74 3d70 7573 6829 5d28 6874 7470 733a  nt=push)](https:
-000004a0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 656e  //github.com/ben
-000004b0: 6a61 6d69 6e2d 6177 642f 6d6f 6e6f 706f  jamin-awd/monopo
-000004c0: 6c79 2f61 6374 696f 6e73 2f77 6f72 6b66  ly/actions/workf
-000004d0: 6c6f 7773 2f74 6573 7473 2e79 616d 6c29  lows/tests.yaml)
-000004e0: 0a5b 215b 4349 5d28 6874 7470 733a 2f2f  .[![CI](https://
-000004f0: 6769 7468 7562 2e63 6f6d 2f62 656e 6a61  github.com/benja
-00000500: 6d69 6e2d 6177 642f 6d6f 6e6f 706f 6c79  min-awd/monopoly
-00000510: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00000520: 7773 2f63 692e 7961 6d6c 2f62 6164 6765  ws/ci.yaml/badge
-00000530: 2e73 7667 3f62 7261 6e63 683d 6d61 696e  .svg?branch=main
-00000540: 2665 7665 6e74 3d70 7573 6829 5d28 6874  &event=push)](ht
-00000550: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000560: 2f62 656e 6a61 6d69 6e2d 6177 642f 6d6f  /benjamin-awd/mo
-00000570: 6e6f 706f 6c79 2f61 6374 696f 6e73 2f77  nopoly/actions/w
-00000580: 6f72 6b66 6c6f 7773 2f63 692e 7961 6d6c  orkflows/ci.yaml
-00000590: 290a 5b21 5b43 6f64 6520 7374 796c 653a  ).[![Code style:
-000005a0: 2062 6c61 636b 5d28 6874 7470 733a 2f2f   black](https://
-000005b0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000005c0: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-000005d0: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
-000005e0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-000005f0: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
-00000600: 6b29 0a5b 215b 4c69 6e74 696e 673a 2070  k).[![Linting: p
-00000610: 796c 696e 745d 2868 7474 7073 3a2f 2f69  ylint](https://i
-00000620: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000630: 6467 652f 6c69 6e74 696e 672d 7079 6c69  dge/linting-pyli
-00000640: 6e74 2d6f 7261 6e67 6529 5d28 6874 7470  nt-orange)](http
-00000650: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000660: 796c 696e 742d 6465 762f 7079 6c69 6e74  ylint-dev/pylint
-00000670: 290a 5b21 5b4c 6963 656e 7365 3a20 4d49  ).[![License: MI
-00000680: 545d 2868 7474 7073 3a2f 2f69 6d67 2e73  T](https://img.s
-00000690: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-000006a0: 4c69 6365 6e73 652d 4d49 542d 7965 6c6c  License-MIT-yell
-000006b0: 6f77 2e73 7667 295d 2868 7474 7073 3a2f  ow.svg)](https:/
-000006c0: 2f6f 7065 6e73 6f75 7263 652e 6f72 672f  /opensource.org/
-000006d0: 6c69 6365 6e73 6573 2f4d 4954 290a 0a0a  licenses/MIT)...
-000006e0: 4d6f 6e6f 706f 6c79 2069 7320 6120 5079  Monopoly is a Py
-000006f0: 7468 6f6e 206c 6962 7261 7279 2074 6861  thon library tha
-00000700: 7420 636f 6e76 6572 7473 2053 696e 6761  t converts Singa
-00000710: 706f 7265 2062 616e 6b20 7374 6174 656d  pore bank statem
-00000720: 656e 7420 5044 4673 2074 6f20 4353 5620  ent PDFs to CSV 
-00000730: 7573 696e 6720 7064 6674 6f74 6578 740a  using pdftotext.
-00000740: 0a21 5b5d 2868 7474 7073 3a2f 2f72 6177  .![](https://raw
-00000750: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000760: 6e74 2e63 6f6d 2f62 656e 6a61 6d69 6e2d  nt.com/benjamin-
-00000770: 6177 642f 6d6f 6e6f 706f 6c79 2f6d 6169  awd/monopoly/mai
-00000780: 6e2f 646f 6373 2f6d 6f6e 6f70 6f6c 792e  n/docs/monopoly.
-00000790: 6769 6629 0a0a 5375 7070 6f72 7465 6420  gif)..Supported 
-000007a0: 6261 6e6b 733a 0a7c 2042 616e 6b20 2020  banks:.| Bank   
-000007b0: 2020 2020 2020 2020 2020 2020 207c 2043               | C
-000007c0: 7265 6469 7420 5374 6174 656d 656e 7420  redit Statement 
-000007d0: 2020 207c 2044 6562 6974 2053 7461 7465     | Debit State
-000007e0: 6d65 6e74 2020 2020 207c 0a7c 202d 2d2d  ment     |.| ---
-000007f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000800: 2d7c 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -| -------------
-00000810: 2d2d 2d2d 2d2d 2d7c 202d 2d2d 2d2d 2d2d  -------| -------
-00000820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c 0a7c  -------------|.|
-00000830: 2043 6974 6962 616e 6b20 2020 2020 2020   Citibank       
-00000840: 2020 2020 207c 203a 7768 6974 655f 6368       | :white_ch
-00000850: 6563 6b5f 6d61 726b 3a20 207c 203a 783a  eck_mark:  | :x:
-00000860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000870: 207c 0a7c 2044 4253 2020 2020 2020 2020   |.| DBS        
-00000880: 2020 2020 2020 2020 207c 203a 7768 6974           | :whit
-00000890: 655f 6368 6563 6b5f 6d61 726b 3a20 207c  e_check_mark:  |
-000008a0: 203a 7768 6974 655f 6368 6563 6b5f 6d61   :white_check_ma
-000008b0: 726b 3a20 207c 0a7c 2048 5342 4320 2020  rk:  |.| HSBC   
-000008c0: 2020 2020 2020 2020 2020 2020 207c 203a               | :
-000008d0: 7768 6974 655f 6368 6563 6b5f 6d61 726b  white_check_mark
-000008e0: 3a20 207c 203a 783a 2020 2020 2020 2020  :  | :x:        
-000008f0: 2020 2020 2020 2020 207c 0a7c 204f 4342           |.| OCB
-00000900: 4320 2020 2020 2020 2020 2020 2020 2020  C               
-00000910: 207c 203a 7768 6974 655f 6368 6563 6b5f   | :white_check_
-00000920: 6d61 726b 3a20 207c 203a 7768 6974 655f  mark:  | :white_
-00000930: 6368 6563 6b5f 6d61 726b 3a20 207c 0a7c  check_mark:  |.|
-00000940: 2053 7461 6e64 6172 6420 4368 6172 7465   Standard Charte
-00000950: 7265 6420 207c 203a 7768 6974 655f 6368  red  | :white_ch
-00000960: 6563 6b5f 6d61 726b 3a20 207c 203a 783a  eck_mark:  | :x:
-00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 207c 0a0a 2323 2049 6e73 7461 6c6c 0a43   |..## Install.C
-00000990: 6c6f 6e65 2074 6865 2072 6570 6f0a 6060  lone the repo.``
-000009a0: 6062 6173 680a 6769 7420 636c 6f6e 6520  `bash.git clone 
-000009b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000009c0: 6f6d 2f62 656e 6a61 6d69 6e2d 6177 642f  om/benjamin-awd/
-000009d0: 6d6f 6e6f 706f 6c79 2e67 6974 0a60 6060  monopoly.git.```
-000009e0: 0a0a 496e 7374 616c 6c20 6465 7065 6e64  ..Install depend
-000009f0: 656e 6369 6573 2075 7369 6e67 205b 486f  encies using [Ho
-00000a00: 6d65 6272 6577 5d28 6874 7470 733a 2f2f  mebrew](https://
-00000a10: 6272 6577 2e73 682f 290a 6060 6062 6173  brew.sh/).```bas
-00000a20: 680a 6272 6577 2069 6e73 7461 6c6c 206d  h.brew install m
-00000a30: 616b 650a 6d61 6b65 2073 6574 7570 0a60  ake.make setup.`
-00000a40: 6060 0a0a 2323 2055 7361 6765 0a4d 6f6e  ``..## Usage.Mon
-00000a50: 6f70 6f6c 7920 6361 6e20 6265 2072 756e  opoly can be run
-00000a60: 2061 7320 6120 5079 7468 6f6e 2070 6163   as a Python pac
-00000a70: 6b61 6765 2c20 616c 6c6f 7769 6e67 2079  kage, allowing y
-00000a80: 6f75 2074 6f20 6578 7472 6163 742c 2074  ou to extract, t
-00000a90: 7261 6e73 666f 726d 2061 6e64 2077 7269  ransform and wri
-00000aa0: 7465 2062 616e 6b20 7374 6174 656d 656e  te bank statemen
-00000ab0: 7473 2074 6f20 6120 4353 5620 6669 6c65  ts to a CSV file
-00000ac0: 2e0a 0a54 6f20 7365 6520 686f 7720 4d6f  ...To see how Mo
-00000ad0: 6e6f 706f 6c79 2077 6f72 6b73 2c20 796f  nopoly works, yo
-00000ae0: 7520 6361 6e20 7275 6e20 7468 6973 2065  u can run this e
-00000af0: 7861 6d70 6c65 0a60 6060 6261 7368 0a70  xample.```bash.p
-00000b00: 7974 686f 6e33 2073 7263 2f6d 6f6e 6f70  ython3 src/monop
-00000b10: 6f6c 792f 6578 616d 706c 6573 2f73 696e  oly/examples/sin
-00000b20: 676c 655f 7374 6174 656d 656e 742e 7079  gle_statement.py
-00000b30: 0a60 6060 0a0a 4966 2079 6f75 206e 6565  .```..If you nee
-00000b40: 6420 746f 2072 756e 206d 6f6e 6f70 6f6c  d to run monopol
-00000b50: 7920 6f6e 2061 2070 6173 7377 6f72 6420  y on a password 
-00000b60: 7072 6f74 6563 7465 6420 6669 6c65 2c20  protected file, 
-00000b70: 656e 7375 7265 2074 6861 7420 7061 7373  ensure that pass
-00000b80: 776f 7264 7320 6172 6520 7365 7420 696e  words are set in
-00000b90: 2074 6865 202e 656e 7620 6669 6c65 3a0a   the .env file:.
-00000ba0: 6060 6073 680a 6370 202e 656e 762e 7465  ```sh.cp .env.te
-00000bb0: 6d70 6c61 7465 2065 6e76 0a60 6060 0a0a  mplate env.```..
-00000bc0: 4966 2079 6f75 2068 6176 6520 6d75 6c74  If you have mult
-00000bd0: 6970 6c65 2073 7461 7465 6d65 6e74 7320  iple statements 
-00000be0: 6672 6f6d 2074 6865 2073 616d 6520 6261  from the same ba
-00000bf0: 6e6b 2077 6974 6820 6469 6666 6572 656e  nk with differen
-00000c00: 7420 7061 7373 776f 7264 7320 2865 2e67  t passwords (e.g
-00000c10: 2e20 4853 4243 2073 7461 7465 6d65 6e74  . HSBC statement
-00000c20: 7329 2c20 6d61 6b65 2073 7572 6520 746f  s), make sure to
-00000c30: 2073 6574 2062 6f74 6820 7061 7373 776f   set both passwo
-00000c40: 7264 7320 696e 2061 6e20 6172 7261 7920  rds in an array 
-00000c50: 666f 726d 6174 206c 696b 6520 736f 3a0a  format like so:.
-00000c60: 6060 6073 680a 4853 4243 5f50 4446 5f50  ```sh.HSBC_PDF_P
-00000c70: 4153 5357 4f52 4453 3d5b 2270 6173 7377  ASSWORDS=["passw
-00000c80: 6f72 6431 222c 2270 6173 7377 6f72 6432  ord1","password2
-00000c90: 225d 0a60 6060 0a0a 2323 2046 6561 7475  "].```..## Featu
-00000ca0: 7265 730a 2d20 556e 6c6f 636b 7320 5044  res.- Unlocks PD
-00000cb0: 4673 2075 7369 6e67 2075 7365 722d 7072  Fs using user-pr
-00000cc0: 6f76 6964 6564 2063 7265 6465 6e74 6961  ovided credentia
-00000cd0: 6c73 0a2d 2053 7461 7465 6d65 6e74 7320  ls.- Statements 
-00000ce0: 6361 6e20 6265 2070 6172 7365 6420 7769  can be parsed wi
-00000cf0: 7468 2074 6865 2043 4c49 2c20 6f72 206d  th the CLI, or m
-00000d00: 616e 7561 6c6c 7920 7769 7468 2074 6865  anually with the
-00000d10: 2062 616e 6b20 7072 6f63 6573 736f 7220   bank processor 
-00000d20: 636c 6173 732e 0a2d 2053 7570 706f 7274  class..- Support
-00000d30: 2066 6f72 2063 6173 6862 6163 6b20 7472   for cashback tr
-00000d40: 616e 7361 6374 696f 6e73 2061 6e64 2072  ansactions and r
-00000d50: 6566 756e 6473 0a2d 204d 6f6e 6f70 6f6c  efunds.- Monopol
-00000d60: 7920 6361 6e20 6265 2072 756e 206f 6e20  y can be run on 
-00000d70: 476f 6f67 6c65 2043 6c6f 7564 2061 7320  Google Cloud as 
-00000d80: 6120 7363 6865 6475 6c65 6420 436c 6f75  a scheduled Clou
-00000d90: 6420 5275 6e20 6a6f 622c 2077 6869 6368  d Run job, which
-00000da0: 206f 7065 6e73 2075 7020 6d6f 7265 2073   opens up more s
-00000db0: 6f70 6869 7374 6963 6174 6564 2075 7365  ophisticated use
-00000dc0: 2d63 6173 6573 206c 696b 6520 6869 7374  -cases like hist
-00000dd0: 6f72 6963 616c 2061 6e61 6c79 7369 7320  orical analysis 
-00000de0: 616e 6420 7065 7273 6f6e 616c 2066 696e  and personal fin
-00000df0: 616e 6365 2076 6973 7561 6c69 7a61 7469  ance visualizati
-00000e00: 6f6e 0a0a                                on..
+000001f0: 7374 3a20 6461 7465 7061 7273 6572 2028  st: dateparser (
+00000200: 3e3d 312e 322e 302c 3c32 2e30 2e30 290a  >=1.2.0,<2.0.0).
+00000210: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+00000220: 7970 7920 283e 3d31 2e37 2e31 2c3c 322e  ypy (>=1.7.1,<2.
+00000230: 302e 3029 0a52 6571 7569 7265 732d 4469  0.0).Requires-Di
+00000240: 7374 3a20 7064 6674 6f74 6578 7420 283e  st: pdftotext (>
+00000250: 3d32 2e32 2e32 2c3c 332e 302e 3029 0a52  =2.2.2,<3.0.0).R
+00000260: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
+00000270: 6461 6e74 6963 2028 3e3d 322e 352e 322c  dantic (>=2.5.2,
+00000280: 3c33 2e30 2e30 290a 5265 7175 6972 6573  <3.0.0).Requires
+00000290: 2d44 6973 743a 2070 7964 616e 7469 632d  -Dist: pydantic-
+000002a0: 7365 7474 696e 6773 2028 3e3d 322e 302e  settings (>=2.0.
+000002b0: 332c 3c33 2e30 2e30 290a 5265 7175 6972  3,<3.0.0).Requir
+000002c0: 6573 2d44 6973 743a 2070 796d 7570 6466  es-Dist: pymupdf
+000002d0: 2028 3e3d 312e 3233 2e37 2c3c 322e 302e   (>=1.23.7,<2.0.
+000002e0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000002f0: 3a20 7461 6275 6c61 7465 2028 3e3d 302e  : tabulate (>=0.
+00000300: 392e 302c 3c30 2e31 302e 3029 0a52 6571  9.0,<0.10.0).Req
+00000310: 7569 7265 732d 4469 7374 3a20 7471 646d  uires-Dist: tqdm
+00000320: 2028 3e3d 342e 3636 2e31 2c3c 352e 302e   (>=4.66.1,<5.0.
+00000330: 3029 0a50 726f 6a65 6374 2d55 524c 3a20  0).Project-URL: 
+00000340: 5265 706f 7369 746f 7279 2c20 6874 7470  Repository, http
+00000350: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+00000360: 656e 6a61 6d69 6e2d 6177 642f 6d6f 6e6f  enjamin-awd/mono
+00000370: 706f 6c79 0a44 6573 6372 6970 7469 6f6e  poly.Description
+00000380: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+00000390: 6578 742f 6d61 726b 646f 776e 0a0a 215b  ext/markdown..![
+000003a0: 5d28 6874 7470 733a 2f2f 7261 772e 6769  ](https://raw.gi
+000003b0: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+000003c0: 636f 6d2f 6265 6e6a 616d 696e 2d61 7764  com/benjamin-awd
+000003d0: 2f6d 6f6e 6f70 6f6c 792f 6d61 696e 2f64  /monopoly/main/d
+000003e0: 6f63 732f 6c6f 676f 2e73 7667 290a 0a2d  ocs/logo.svg)..-
+000003f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000400: 0a5b 215b 5374 7265 616d 6c69 745d 2868  .[![Streamlit](h
+00000410: 7474 7073 3a2f 2f73 7461 7469 632e 7374  ttps://static.st
+00000420: 7265 616d 6c69 742e 696f 2f62 6164 6765  reamlit.io/badge
+00000430: 732f 7374 7265 616d 6c69 745f 6261 6467  s/streamlit_badg
+00000440: 655f 626c 6163 6b5f 7768 6974 652e 7376  e_black_white.sv
+00000450: 6729 5d28 6874 7470 733a 2f2f 6d6f 6e6f  g)](https://mono
+00000460: 706f 6c79 2e73 7472 6561 6d6c 6974 2e61  poly.streamlit.a
+00000470: 7070 290a 5b21 5b54 6573 7473 5d28 6874  pp).[![Tests](ht
+00000480: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000490: 2f62 656e 6a61 6d69 6e2d 6177 642f 6d6f  /benjamin-awd/mo
+000004a0: 6e6f 706f 6c79 2f61 6374 696f 6e73 2f77  nopoly/actions/w
+000004b0: 6f72 6b66 6c6f 7773 2f74 6573 7473 2e79  orkflows/tests.y
+000004c0: 616d 6c2f 6261 6467 652e 7376 673f 6272  aml/badge.svg?br
+000004d0: 616e 6368 3d6d 6169 6e26 6576 656e 743d  anch=main&event=
+000004e0: 7075 7368 295d 2868 7474 7073 3a2f 2f67  push)](https://g
+000004f0: 6974 6875 622e 636f 6d2f 6265 6e6a 616d  ithub.com/benjam
+00000500: 696e 2d61 7764 2f6d 6f6e 6f70 6f6c 792f  in-awd/monopoly/
+00000510: 6163 7469 6f6e 732f 776f 726b 666c 6f77  actions/workflow
+00000520: 732f 7465 7374 732e 7961 6d6c 290a 5b21  s/tests.yaml).[!
+00000530: 5b43 495d 2868 7474 7073 3a2f 2f67 6974  [CI](https://git
+00000540: 6875 622e 636f 6d2f 6265 6e6a 616d 696e  hub.com/benjamin
+00000550: 2d61 7764 2f6d 6f6e 6f70 6f6c 792f 6163  -awd/monopoly/ac
+00000560: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000570: 6369 2e79 616d 6c2f 6261 6467 652e 7376  ci.yaml/badge.sv
+00000580: 673f 6272 616e 6368 3d6d 6169 6e26 6576  g?branch=main&ev
+00000590: 656e 743d 7075 7368 295d 2868 7474 7073  ent=push)](https
+000005a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6265  ://github.com/be
+000005b0: 6e6a 616d 696e 2d61 7764 2f6d 6f6e 6f70  njamin-awd/monop
+000005c0: 6f6c 792f 6163 7469 6f6e 732f 776f 726b  oly/actions/work
+000005d0: 666c 6f77 732f 6369 2e79 616d 6c29 0a5b  flows/ci.yaml).[
+000005e0: 215b 4c69 6365 6e73 653a 204d 4954 5d28  ![License: MIT](
+000005f0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000600: 6c64 732e 696f 2f62 6164 6765 2f4c 6963  lds.io/badge/Lic
+00000610: 656e 7365 2d4d 4954 2d79 656c 6c6f 772e  ense-MIT-yellow.
+00000620: 7376 6729 5d28 6874 7470 733a 2f2f 6f70  svg)](https://op
+00000630: 656e 736f 7572 6365 2e6f 7267 2f6c 6963  ensource.org/lic
+00000640: 656e 7365 732f 4d49 5429 0a0a 4d6f 6e6f  enses/MIT)..Mono
+00000650: 706f 6c79 2069 7320 6120 5079 7468 6f6e  poly is a Python
+00000660: 206c 6962 7261 7279 2026 2043 4c49 2074   library & CLI t
+00000670: 6861 7420 636f 6e76 6572 7473 2053 696e  hat converts Sin
+00000680: 6761 706f 7265 2062 616e 6b20 7374 6174  gapore bank stat
+00000690: 656d 656e 7420 5044 4673 2074 6f20 4353  ement PDFs to CS
+000006a0: 562e 0a0a 215b 5d28 6874 7470 733a 2f2f  V...![](https://
+000006b0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
+000006c0: 6e74 656e 742e 636f 6d2f 6265 6e6a 616d  ntent.com/benjam
+000006d0: 696e 2d61 7764 2f6d 6f6e 6f70 6f6c 792f  in-awd/monopoly/
+000006e0: 6d61 696e 2f64 6f63 732f 6d6f 6e6f 706f  main/docs/monopo
+000006f0: 6c79 2e67 6966 290a 0a53 7570 706f 7274  ly.gif)..Support
+00000700: 6564 2062 616e 6b73 3a0a 7c20 4261 6e6b  ed banks:.| Bank
+00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000720: 7c20 4372 6564 6974 2053 7461 7465 6d65  | Credit Stateme
+00000730: 6e74 2020 2020 7c20 4465 6269 7420 5374  nt    | Debit St
+00000740: 6174 656d 656e 7420 2020 2020 7c0a 7c20  atement     |.| 
+00000750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000760: 2d2d 2d2d 7c20 2d2d 2d2d 2d2d 2d2d 2d2d  ----| ----------
+00000770: 2d2d 2d2d 2d2d 2d2d 2d2d 7c20 2d2d 2d2d  ----------| ----
+00000780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000790: 7c0a 7c20 4369 7469 6261 6e6b 2020 2020  |.| Citibank    
+000007a0: 2020 2020 2020 2020 7c20 3a77 6869 7465          | :white
+000007b0: 5f63 6865 636b 5f6d 6172 6b3a 2020 7c20  _check_mark:  | 
+000007c0: 3a78 3a20 2020 2020 2020 2020 2020 2020  :x:             
+000007d0: 2020 2020 7c0a 7c20 4442 5320 2020 2020      |.| DBS     
+000007e0: 2020 2020 2020 2020 2020 2020 7c20 3a77              | :w
+000007f0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
+00000800: 2020 7c20 3a77 6869 7465 5f63 6865 636b    | :white_check
+00000810: 5f6d 6172 6b3a 2020 7c0a 7c20 4853 4243  _mark:  |.| HSBC
+00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000830: 7c20 3a77 6869 7465 5f63 6865 636b 5f6d  | :white_check_m
+00000840: 6172 6b3a 2020 7c20 3a78 3a20 2020 2020  ark:  | :x:     
+00000850: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00000860: 4f43 4243 2020 2020 2020 2020 2020 2020  OCBC            
+00000870: 2020 2020 7c20 3a77 6869 7465 5f63 6865      | :white_che
+00000880: 636b 5f6d 6172 6b3a 2020 7c20 3a77 6869  ck_mark:  | :whi
+00000890: 7465 5f63 6865 636b 5f6d 6172 6b3a 2020  te_check_mark:  
+000008a0: 7c0a 7c20 5374 616e 6461 7264 2043 6861  |.| Standard Cha
+000008b0: 7274 6572 6564 2020 7c20 3a77 6869 7465  rtered  | :white
+000008c0: 5f63 6865 636b 5f6d 6172 6b3a 2020 7c20  _check_mark:  | 
+000008d0: 3a78 3a20 2020 2020 2020 2020 2020 2020  :x:             
+000008e0: 2020 2020 7c0a 0a3c 6833 2061 6c69 676e      |..<h3 align
+000008f0: 3d22 6365 6e74 6572 223e 0a20 2020 20f0  ="center">.    .
+00000900: 9f8e 8920 4d6f 6e6f 706f 6c79 2069 7320  ... Monopoly is 
+00000910: 6e6f 7720 6c69 7665 2120 f09f 8e89 0a20  now live! ..... 
+00000920: 2020 203c 6272 3e3c 6272 3e0a 2020 2020     <br><br>.    
+00000930: 5472 7920 6974 206f 7574 3a20 3c62 723e  Try it out: <br>
+00000940: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+00000950: 7470 733a 2f2f 6d6f 6e6f 706f 6c79 2e73  tps://monopoly.s
+00000960: 7472 6561 6d6c 6974 6170 702e 636f 6d2f  treamlitapp.com/
+00000970: 223e 6874 7470 733a 2f2f 6d6f 6e6f 706f  ">https://monopo
+00000980: 6c79 2e73 7472 6561 6d6c 6974 6170 702e  ly.streamlitapp.
+00000990: 636f 6d2f 3c2f 613e 0a3c 2f68 333e 0a0a  com/</a>.</h3>..
+000009a0: 3c70 2061 6c69 676e 3d22 6365 6e74 6572  <p align="center
+000009b0: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+000009c0: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
+000009d0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+000009e0: 6f6d 2f62 656e 6a61 6d69 6e2d 6177 642f  om/benjamin-awd/
+000009f0: 6d6f 6e6f 706f 6c79 2f6d 6169 6e2f 646f  monopoly/main/do
+00000a00: 6373 2f73 7472 6561 6d6c 6974 5f64 656d  cs/streamlit_dem
+00000a10: 6f2e 6769 6622 2077 6964 7468 3d38 3030  o.gif" width=800
+00000a20: 3e0a 3c2f 703e 0a0a 2323 2049 6e73 7461  >.</p>..## Insta
+00000a30: 6c6c 0a43 6c6f 6e65 2074 6865 2072 6570  ll.Clone the rep
+00000a40: 6f0a 6060 6062 6173 680a 6769 7420 636c  o.```bash.git cl
+00000a50: 6f6e 6520 6874 7470 733a 2f2f 6769 7468  one https://gith
+00000a60: 7562 2e63 6f6d 2f62 656e 6a61 6d69 6e2d  ub.com/benjamin-
+00000a70: 6177 642f 6d6f 6e6f 706f 6c79 2e67 6974  awd/monopoly.git
+00000a80: 0a60 6060 0a0a 496e 7374 616c 6c20 6465  .```..Install de
+00000a90: 7065 6e64 656e 6369 6573 2075 7369 6e67  pendencies using
+00000aa0: 205b 486f 6d65 6272 6577 5d28 6874 7470   [Homebrew](http
+00000ab0: 733a 2f2f 6272 6577 2e73 682f 290a 6060  s://brew.sh/).``
+00000ac0: 6062 6173 680a 6272 6577 2069 6e73 7461  `bash.brew insta
+00000ad0: 6c6c 206d 616b 650a 6d61 6b65 2073 6574  ll make.make set
+00000ae0: 7570 0a60 6060 0a0a 2323 2055 7361 6765  up.```..## Usage
+00000af0: 0a4d 6f6e 6f70 6f6c 7920 6361 6e20 6265  .Monopoly can be
+00000b00: 2072 756e 2061 7320 6120 5079 7468 6f6e   run as a Python
+00000b10: 2070 6163 6b61 6765 2c20 616c 6c6f 7769   package, allowi
+00000b20: 6e67 2079 6f75 2074 6f20 6578 7472 6163  ng you to extrac
+00000b30: 742c 2074 7261 6e73 666f 726d 2061 6e64  t, transform and
+00000b40: 2077 7269 7465 2062 616e 6b20 7374 6174   write bank stat
+00000b50: 656d 656e 7473 2074 6f20 6120 4353 5620  ements to a CSV 
+00000b60: 6669 6c65 2e0a 0a54 6f20 7365 6520 686f  file...To see ho
+00000b70: 7720 4d6f 6e6f 706f 6c79 2077 6f72 6b73  w Monopoly works
+00000b80: 2c20 796f 7520 6361 6e20 7275 6e20 7468  , you can run th
+00000b90: 6973 2065 7861 6d70 6c65 0a60 6060 6261  is example.```ba
+00000ba0: 7368 0a70 7974 686f 6e33 2073 7263 2f6d  sh.python3 src/m
+00000bb0: 6f6e 6f70 6f6c 792f 6578 616d 706c 6573  onopoly/examples
+00000bc0: 2f73 696e 676c 655f 7374 6174 656d 656e  /single_statemen
+00000bd0: 742e 7079 0a60 6060 0a0a 4966 2079 6f75  t.py.```..If you
+00000be0: 206e 6565 6420 746f 2072 756e 206d 6f6e   need to run mon
+00000bf0: 6f70 6f6c 7920 6f6e 2061 2070 6173 7377  opoly on a passw
+00000c00: 6f72 6420 7072 6f74 6563 7465 6420 6669  ord protected fi
+00000c10: 6c65 2c20 656e 7375 7265 2074 6861 7420  le, ensure that 
+00000c20: 7061 7373 776f 7264 7320 6172 6520 7365  passwords are se
+00000c30: 7420 696e 2074 6865 202e 656e 7620 6669  t in the .env fi
+00000c40: 6c65 3a0a 6060 6073 680a 6370 202e 656e  le:.```sh.cp .en
+00000c50: 762e 7465 6d70 6c61 7465 2065 6e76 0a60  v.template env.`
+00000c60: 6060 0a0a 4966 2079 6f75 2068 6176 6520  ``..If you have 
+00000c70: 6d75 6c74 6970 6c65 2073 7461 7465 6d65  multiple stateme
+00000c80: 6e74 7320 6672 6f6d 2074 6865 2073 616d  nts from the sam
+00000c90: 6520 6261 6e6b 2077 6974 6820 6469 6666  e bank with diff
+00000ca0: 6572 656e 7420 7061 7373 776f 7264 7320  erent passwords 
+00000cb0: 2865 2e67 2e20 4853 4243 2073 7461 7465  (e.g. HSBC state
+00000cc0: 6d65 6e74 7329 2c20 6d61 6b65 2073 7572  ments), make sur
+00000cd0: 6520 746f 2073 6574 2062 6f74 6820 7061  e to set both pa
+00000ce0: 7373 776f 7264 7320 696e 2061 6e20 6172  sswords in an ar
+00000cf0: 7261 7920 666f 726d 6174 206c 696b 6520  ray format like 
+00000d00: 736f 3a0a 6060 6073 680a 4853 4243 5f50  so:.```sh.HSBC_P
+00000d10: 4446 5f50 4153 5357 4f52 4453 3d5b 2270  DF_PASSWORDS=["p
+00000d20: 6173 7377 6f72 6431 222c 2270 6173 7377  assword1","passw
+00000d30: 6f72 6432 225d 0a60 6060 0a0a 2323 2046  ord2"].```..## F
+00000d40: 6561 7475 7265 730a 2d20 556e 6c6f 636b  eatures.- Unlock
+00000d50: 7320 5044 4673 2075 7369 6e67 2075 7365  s PDFs using use
+00000d60: 722d 7072 6f76 6964 6564 2063 7265 6465  r-provided crede
+00000d70: 6e74 6961 6c73 0a2d 2053 7461 7465 6d65  ntials.- Stateme
+00000d80: 6e74 7320 6361 6e20 6265 2070 6172 7365  nts can be parse
+00000d90: 6420 7769 7468 2074 6865 2043 4c49 2c20  d with the CLI, 
+00000da0: 6f72 2077 6974 6820 6120 7363 7269 7074  or with a script
+00000db0: 2075 7369 6e67 2074 6865 2053 7461 7465   using the State
+00000dc0: 6d65 6e74 4861 6e64 6c65 7220 636c 6173  mentHandler clas
+00000dd0: 732e 0a2d 2053 7570 706f 7274 2066 6f72  s..- Support for
+00000de0: 2063 6173 6862 6163 6b20 7472 616e 7361   cashback transa
+00000df0: 6374 696f 6e73 2061 6e64 2072 6566 756e  ctions and refun
+00000e00: 6473 0a2d 204d 6f6e 6f70 6f6c 7920 6361  ds.- Monopoly ca
+00000e10: 6e20 6265 2072 756e 206f 6e20 476f 6f67  n be run on Goog
+00000e20: 6c65 2043 6c6f 7564 2061 7320 6120 7363  le Cloud as a sc
+00000e30: 6865 6475 6c65 6420 436c 6f75 6420 5275  heduled Cloud Ru
+00000e40: 6e20 6a6f 622c 2077 6869 6368 206f 7065  n job, which ope
+00000e50: 6e73 2075 7020 6d6f 7265 2073 6f70 6869  ns up more sophi
+00000e60: 7374 6963 6174 6564 2075 7365 2d63 6173  sticated use-cas
+00000e70: 6573 206c 696b 6520 6869 7374 6f72 6963  es like historic
+00000e80: 616c 2061 6e61 6c79 7369 7320 616e 6420  al analysis and 
+00000e90: 7065 7273 6f6e 616c 2066 696e 616e 6365  personal finance
+00000ea0: 2076 6973 7561 6c69 7a61 7469 6f6e 0a0a   visualization..
```

