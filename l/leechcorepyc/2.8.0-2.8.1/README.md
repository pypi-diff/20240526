# Comparing `tmp/leechcorepyc-2.8.0.tar.gz` & `tmp/leechcorepyc-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/leechcorepyc-2.8.0.tar", last modified: Sat Sep 25 19:45:35 2021, max compression
+gzip compressed data, was "dist/leechcorepyc-2.8.1.tar", last modified: Sat Sep 25 21:26:26 2021, max compression
```

## Comparing `leechcorepyc-2.8.0.tar` & `leechcorepyc-2.8.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:35.008127 leechcorepyc-2.8.0/
--rwxrwxrwx   0 user      (1001) user      (1001)      236 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/MANIFEST.in
--rwxrwxrwx   0 user      (1001) user      (1001)      493 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)      566 2021-09-25 19:45:35.007125 leechcorepyc-2.8.0/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)      136 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/README
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.762846 leechcorepyc-2.8.0/files/
--rwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/files/dummy
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.772846 leechcorepyc-2.8.0/includes/
--rwxrwxrwx   0 user      (1001) user      (1001)    21903 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/includes/leechcore.h
--rwxrwxrwx   0 user      (1001) user      (1001)     6565 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/includes/leechcore_device.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.898175 leechcorepyc-2.8.0/leechcore/
--rwxrwxrwx   0 user      (1001) user      (1001)      869 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)    29242 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/device_file.c
--rwxrwxrwx   0 user      (1001) user      (1001)   104804 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/device_fpga.c
--rwxrwxrwx   0 user      (1001) user      (1001)    13959 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/device_pmem.c
--rwxrwxrwx   0 user      (1001) user      (1001)    11845 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/device_tmd.c
--rwxrwxrwx   0 user      (1001) user      (1001)    15956 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/device_usb3380.c
--rwxrwxrwx   0 user      (1001) user      (1001)     8937 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/device_vmware.c
--rwxrwxrwx   0 user      (1001) user      (1001)    42579 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechcore.c
--rwxrwxrwx   0 user      (1001) user      (1001)    21903 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechcore.h
--rwxrwxrwx   0 user      (1001) user      (1001)     2928 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechcore.rc
--rwxrwxrwx   0 user      (1001) user      (1001)     6565 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechcore_device.h
--rwxrwxrwx   0 user      (1001) user      (1001)     1648 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechcore_internal.h
--rwxrwxrwx   0 user      (1001) user      (1001)     6146 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechrpc.h
--rwxrwxrwx   0 user      (1001) user      (1001)      418 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechrpc.idl
--rwxrwxrwx   0 user      (1001) user      (1001)    18362 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechrpc_c.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1794 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechrpc_h.h
--rwxrwxrwx   0 user      (1001) user      (1001)    28593 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechrpcclient.c
--rwxrwxrwx   0 user      (1001) user      (1001)     5673 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/leechrpcshared.c
--rwxrwxrwx   0 user      (1001) user      (1001)     7309 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/memmap.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10039 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)    10231 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/oscompatibility.h
--rwxrwxrwx   0 user      (1001) user      (1001)     6075 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/util.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3142 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/util.h
--rwxrwxrwx   0 user      (1001) user      (1001)     1085 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore/version.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.928397 leechcorepyc-2.8.0/leechcore_device_rawtcp/
--rwxrwxrwx   0 user      (1001) user      (1001)      399 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)     8220 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/leechcore_device_rawtcp.c
--rwxrwxrwx   0 user      (1001) user      (1001)      437 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1471 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/oscompatibility.h
--rwxrwxrwx   0 user      (1001) user      (1001)     2928 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/plugin.rc
--rwxrwxrwx   0 user      (1001) user      (1001)      383 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/resource.h
--rwxrwxrwx   0 user      (1001) user      (1001)     1115 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_rawtcp/version.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.972952 leechcorepyc-2.8.0/leechcore_device_sp605tcp/
--rwxrwxrwx   0 user      (1001) user      (1001)      411 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)    19245 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/leechcore_device_sp605tcp.c
--rwxrwxrwx   0 user      (1001) user      (1001)      602 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)     1904 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/oscompatibility.h
--rwxrwxrwx   0 user      (1001) user      (1001)     2928 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/plugin.rc
--rwxrwxrwx   0 user      (1001) user      (1001)      383 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/resource.h
--rwxrwxrwx   0 user      (1001) user      (1001)    10443 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/tlp.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3832 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/tlp.h
--rwxrwxrwx   0 user      (1001) user      (1001)     1119 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_device_sp605tcp/version.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.987127 leechcorepyc-2.8.0/leechcore_ft601_driver_linux/
--rwxrwxrwx   0 user      (1001) user      (1001)      471 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_ft601_driver_linux/Makefile
--rwxrwxrwx   0 user      (1001) user      (1001)     8968 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_ft601_driver_linux/fpga_libusb.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3897 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_ft601_driver_linux/fpga_libusb.h
--rwxrwxrwx   0 user      (1001) user      (1001)     5352 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.c
--rwxrwxrwx   0 user      (1001) user      (1001)     3375 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.h
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:34.990122 leechcorepyc-2.8.0/leechcorepyc/
--rwxrwxrwx   0 user      (1001) user      (1001)     7226 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcorepyc/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)    30358 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/leechcorepyc.c
-drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 19:45:35.004122 leechcorepyc-2.8.0/leechcorepyc.egg-info/
--rwxrwxrwx   0 user      (1001) user      (1001)      566 2021-09-25 19:45:33.000000 leechcorepyc-2.8.0/leechcorepyc.egg-info/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     1748 2021-09-25 19:45:33.000000 leechcorepyc-2.8.0/leechcorepyc.egg-info/SOURCES.txt
--rwxrwxrwx   0 user      (1001) user      (1001)        1 2021-09-25 19:45:33.000000 leechcorepyc-2.8.0/leechcorepyc.egg-info/dependency_links.txt
--rwxrwxrwx   0 user      (1001) user      (1001)       13 2021-09-25 19:45:33.000000 leechcorepyc-2.8.0/leechcorepyc.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     8441 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/oscompatibility.c
--rwxrwxrwx   0 user      (1001) user      (1001)     9591 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/oscompatibility.h
--rwxrwxrwx   0 user      (1001) user      (1001)       38 2021-09-25 19:45:35.008127 leechcorepyc-2.8.0/setup.cfg
--rwxrwxrwx   0 user      (1001) user      (1001)     1467 2021-09-25 19:45:26.000000 leechcorepyc-2.8.0/setup.py
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.382387 leechcorepyc-2.8.1/
+-rwxrwxrwx   0 user      (1001) user      (1001)      236 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/MANIFEST.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      493 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)      566 2021-09-25 21:26:26.366765 leechcorepyc-2.8.1/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)      136 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/README
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.163647 leechcorepyc-2.8.1/files/
+-rwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/files/dummy
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.179271 leechcorepyc-2.8.1/includes/
+-rwxrwxrwx   0 user      (1001) user      (1001)    21903 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/includes/leechcore.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     6565 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/includes/leechcore_device.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.288623 leechcorepyc-2.8.1/leechcore/
+-rwxrwxrwx   0 user      (1001) user      (1001)      869 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)    29242 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/device_file.c
+-rwxrwxrwx   0 user      (1001) user      (1001)   104804 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/device_fpga.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    13959 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/device_pmem.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    11845 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/device_tmd.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    15956 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/device_usb3380.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     8937 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/device_vmware.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    42579 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechcore.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    21903 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechcore.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     2928 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechcore.rc
+-rwxrwxrwx   0 user      (1001) user      (1001)     6565 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechcore_device.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     1648 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechcore_internal.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     6146 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechrpc.h
+-rwxrwxrwx   0 user      (1001) user      (1001)      418 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechrpc.idl
+-rwxrwxrwx   0 user      (1001) user      (1001)    18362 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechrpc_c.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1794 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechrpc_h.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    28593 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechrpcclient.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     5673 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/leechrpcshared.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     7309 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/memmap.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10039 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)    10231 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/oscompatibility.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     6075 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/util.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3142 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/util.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     1085 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore/version.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.304262 leechcorepyc-2.8.1/leechcore_device_rawtcp/
+-rwxrwxrwx   0 user      (1001) user      (1001)      399 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)     8220 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/leechcore_device_rawtcp.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      437 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1471 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/oscompatibility.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     2928 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/plugin.rc
+-rwxrwxrwx   0 user      (1001) user      (1001)      383 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/resource.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     1115 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_rawtcp/version.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.335515 leechcorepyc-2.8.1/leechcore_device_sp605tcp/
+-rwxrwxrwx   0 user      (1001) user      (1001)      411 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)    19245 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/leechcore_device_sp605tcp.c
+-rwxrwxrwx   0 user      (1001) user      (1001)      602 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     1904 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/oscompatibility.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     2928 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/plugin.rc
+-rwxrwxrwx   0 user      (1001) user      (1001)      383 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/resource.h
+-rwxrwxrwx   0 user      (1001) user      (1001)    10443 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/tlp.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3832 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/tlp.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     1119 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_device_sp605tcp/version.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.366765 leechcorepyc-2.8.1/leechcore_ft601_driver_linux/
+-rwxrwxrwx   0 user      (1001) user      (1001)      471 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_ft601_driver_linux/Makefile
+-rwxrwxrwx   0 user      (1001) user      (1001)     8968 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_ft601_driver_linux/fpga_libusb.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3897 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_ft601_driver_linux/fpga_libusb.h
+-rwxrwxrwx   0 user      (1001) user      (1001)     5352 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     3375 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.h
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.366765 leechcorepyc-2.8.1/leechcorepyc/
+-rwxrwxrwx   0 user      (1001) user      (1001)     7226 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcorepyc/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)    30358 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/leechcorepyc.c
+drwxrwxrwx   0 user      (1001) user      (1001)        0 2021-09-25 21:26:26.366765 leechcorepyc-2.8.1/leechcorepyc.egg-info/
+-rwxrwxrwx   0 user      (1001) user      (1001)      566 2021-09-25 21:26:25.000000 leechcorepyc-2.8.1/leechcorepyc.egg-info/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     1748 2021-09-25 21:26:26.000000 leechcorepyc-2.8.1/leechcorepyc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)        1 2021-09-25 21:26:25.000000 leechcorepyc-2.8.1/leechcorepyc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)       13 2021-09-25 21:26:25.000000 leechcorepyc-2.8.1/leechcorepyc.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     8441 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/oscompatibility.c
+-rwxrwxrwx   0 user      (1001) user      (1001)     9591 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/oscompatibility.h
+-rwxrwxrwx   0 user      (1001) user      (1001)       38 2021-09-25 21:26:26.382387 leechcorepyc-2.8.1/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1467 2021-09-25 21:26:20.000000 leechcorepyc-2.8.1/setup.py
```

### Comparing `leechcorepyc-2.8.0/PKG-INFO` & `leechcorepyc-2.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: leechcorepyc
-Version: 2.8.0
+Version: 2.8.1
 Summary: LeechCore for Python
 Home-page: https://github.com/ufrisk/LeechCore
 Author: Ulf Frisk
 Author-email: pcileech@frizk.net
 License: GNU General Public License v3.0
 Description: LeechCore for Python : native extension for physical memory access
 Platform: manylinux1_x86_64
```

### Comparing `leechcorepyc-2.8.0/includes/leechcore.h` & `leechcorepyc-2.8.1/includes/leechcore.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/includes/leechcore_device.h` & `leechcorepyc-2.8.1/includes/leechcore_device.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/Makefile` & `leechcorepyc-2.8.1/leechcore/Makefile`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/device_file.c` & `leechcorepyc-2.8.1/leechcore/device_file.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/device_fpga.c` & `leechcorepyc-2.8.1/leechcore/device_fpga.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/device_pmem.c` & `leechcorepyc-2.8.1/leechcore/device_pmem.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/device_tmd.c` & `leechcorepyc-2.8.1/leechcore/device_tmd.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/device_usb3380.c` & `leechcorepyc-2.8.1/leechcore/device_usb3380.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/device_vmware.c` & `leechcorepyc-2.8.1/leechcore/device_vmware.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechcore.c` & `leechcorepyc-2.8.1/leechcore/leechcore.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechcore.h` & `leechcorepyc-2.8.1/leechcore/leechcore.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechcore.rc` & `leechcorepyc-2.8.1/leechcore/leechcore.rc`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechcore_device.h` & `leechcorepyc-2.8.1/leechcore/leechcore_device.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechcore_internal.h` & `leechcorepyc-2.8.1/leechcore/leechcore_internal.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechrpc.h` & `leechcorepyc-2.8.1/leechcore/leechrpc.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechrpc_c.c` & `leechcorepyc-2.8.1/leechcore/leechrpc_c.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechrpc_h.h` & `leechcorepyc-2.8.1/leechcore/leechrpc_h.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechrpcclient.c` & `leechcorepyc-2.8.1/leechcore/leechrpcclient.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/leechrpcshared.c` & `leechcorepyc-2.8.1/leechcore/leechrpcshared.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/memmap.c` & `leechcorepyc-2.8.1/leechcore/memmap.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/oscompatibility.c` & `leechcorepyc-2.8.1/leechcore/oscompatibility.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/oscompatibility.h` & `leechcorepyc-2.8.1/leechcore/oscompatibility.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/util.c` & `leechcorepyc-2.8.1/leechcore/util.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/util.h` & `leechcorepyc-2.8.1/leechcore/util.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore/version.h` & `leechcorepyc-2.8.1/leechcore/version.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #define STRINGIZE2(s) #s
 #define STRINGIZE(s) STRINGIZE2(s)
 
 #define VERSION_MAJOR               2
 #define VERSION_MINOR               8
-#define VERSION_REVISION            0
-#define VERSION_BUILD               34
+#define VERSION_REVISION            1
+#define VERSION_BUILD               35
 
 #define VER_FILE_DESCRIPTION_STR    "LeechCore Memory Acquisition Library"
 #define VER_FILE_VERSION            VERSION_MAJOR, VERSION_MINOR, VERSION_REVISION, VERSION_BUILD
 #define VER_FILE_VERSION_STR        STRINGIZE(VERSION_MAJOR)        \
                                     "." STRINGIZE(VERSION_MINOR)    \
                                     "." STRINGIZE(VERSION_REVISION) \
                                     "." STRINGIZE(VERSION_BUILD)    \
```

### Comparing `leechcorepyc-2.8.0/leechcore_device_rawtcp/leechcore_device_rawtcp.c` & `leechcorepyc-2.8.1/leechcore_device_rawtcp/leechcore_device_rawtcp.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_rawtcp/oscompatibility.h` & `leechcorepyc-2.8.1/leechcore_device_rawtcp/oscompatibility.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_rawtcp/plugin.rc` & `leechcorepyc-2.8.1/leechcore_device_rawtcp/plugin.rc`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_rawtcp/version.h` & `leechcorepyc-2.8.1/leechcore_device_rawtcp/version.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/leechcore_device_sp605tcp.c` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/leechcore_device_sp605tcp.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/oscompatibility.c` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/oscompatibility.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/oscompatibility.h` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/oscompatibility.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/plugin.rc` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/plugin.rc`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/tlp.c` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/tlp.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/tlp.h` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/tlp.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_device_sp605tcp/version.h` & `leechcorepyc-2.8.1/leechcore_device_sp605tcp/version.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_ft601_driver_linux/fpga_libusb.c` & `leechcorepyc-2.8.1/leechcore_ft601_driver_linux/fpga_libusb.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_ft601_driver_linux/fpga_libusb.h` & `leechcorepyc-2.8.1/leechcore_ft601_driver_linux/fpga_libusb.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.c` & `leechcorepyc-2.8.1/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.h` & `leechcorepyc-2.8.1/leechcore_ft601_driver_linux/leechcore_ft601_driver_linux.h`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcorepyc/__init__.py` & `leechcorepyc-2.8.1/leechcorepyc/__init__.py`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcorepyc.c` & `leechcorepyc-2.8.1/leechcorepyc.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/leechcorepyc.egg-info/PKG-INFO` & `leechcorepyc-2.8.1/leechcorepyc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: leechcorepyc
-Version: 2.8.0
+Version: 2.8.1
 Summary: LeechCore for Python
 Home-page: https://github.com/ufrisk/LeechCore
 Author: Ulf Frisk
 Author-email: pcileech@frizk.net
 License: GNU General Public License v3.0
 Description: LeechCore for Python : native extension for physical memory access
 Platform: manylinux1_x86_64
```

### Comparing `leechcorepyc-2.8.0/leechcorepyc.egg-info/SOURCES.txt` & `leechcorepyc-2.8.1/leechcorepyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/oscompatibility.c` & `leechcorepyc-2.8.1/oscompatibility.c`

 * *Files identical despite different names*

### Comparing `leechcorepyc-2.8.0/oscompatibility.h` & `leechcorepyc-2.8.1/oscompatibility.h`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 typedef uint8_t                             UCHAR, *PUCHAR;
 typedef char                                CHAR, *PCHAR, *PSTR, *LPSTR;
 typedef uint16_t                            WORD, *PWORD, USHORT, *PUSHORT;
 typedef uint16_t                            WCHAR, *PWCHAR, *LPWSTR, *LPCWSTR;
 typedef uint32_t                            DWORD, *PDWORD, ULONG, *PULONG;
 typedef long long unsigned int              QWORD, *PQWORD, ULONG64, *PULONG64;
 typedef uint64_t                            LARGE_INTEGER, *PLARGE_INTEGER, FILETIME;
-typedef uint64_t                            SIZE_T, *PSIZE_T;
+typedef size_t                              SIZE_T, *PSIZE_T;
 typedef void                                *OVERLAPPED, *LPOVERLAPPED;
 typedef struct tdEXCEPTION_RECORD32         { CHAR sz[80]; } EXCEPTION_RECORD32;
 typedef struct tdEXCEPTION_RECORD64         { CHAR sz[152]; } EXCEPTION_RECORD64;
 #define TRUE                                1
 #define FALSE                               0
 #define MAX_PATH                            260
 #define LMEM_ZEROINIT                       0x0040
```

### Comparing `leechcorepyc-2.8.0/setup.py` & `leechcorepyc-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     extra_compile_args=["-I.", "-L.", "-l:leechcore.so", "-shared", "-fPIC", "-fvisibility=hidden"],
     extra_link_args=["-Wl,-rpath,$ORIGIN", "-g", "-ldl", "-shared"],
     py_limited_api=True
     )
 
 setup(
     name='leechcorepyc',
-    version='2.8.0', # VERSION_END
+    version='2.8.1', # VERSION_END
     description='LeechCore for Python',
     long_description='LeechCore for Python : native extension for physical memory access',
     url='https://github.com/ufrisk/LeechCore',
     author='Ulf Frisk',
     author_email='pcileech@frizk.net',
     license='GNU General Public License v3.0',
     platforms='manylinux1_x86_64',
```

