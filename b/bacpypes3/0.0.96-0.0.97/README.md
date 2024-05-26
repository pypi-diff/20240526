# Comparing `tmp/bacpypes3-0.0.96.tar.gz` & `tmp/bacpypes3-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacpypes3-0.0.96.tar", last modified: Fri May 24 03:43:00 2024, max compression
+gzip compressed data, was "bacpypes3-0.0.97.tar", last modified: Sun May 26 03:43:05 2024, max compression
```

## Comparing `bacpypes3-0.0.96.tar` & `bacpypes3-0.0.97.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.122239 bacpypes3-0.0.96/
--rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-05-24 03:43:00.122239 bacpypes3-0.0.96/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.96/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.106239 bacpypes3-0.0.96/bacpypes3/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1391 2024-05-24 03:42:08.000000 bacpypes3-0.0.96/bacpypes3/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    25537 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/bacpypes3/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    56670 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/bacpypes3/apdu.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    34748 2024-03-21 12:00:37.000000 bacpypes3-0.0.96/bacpypes3/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    65965 2023-10-31 15:46:12.000000 bacpypes3-0.0.96/bacpypes3/appservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    21688 2024-03-31 21:04:35.000000 bacpypes3-0.0.96/bacpypes3/argparse.py
--rw-rw-r--   0 joel      (1000) joel      (1000)   106036 2024-05-24 03:42:08.000000 bacpypes3-0.0.96/bacpypes3/basetypes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16296 2023-10-14 01:56:06.000000 bacpypes3-0.0.96/bacpypes3/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.96/bacpypes3/comm.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.96/bacpypes3/console.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64628 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/bacpypes3/constructeddata.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.96/bacpypes3/debugging.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.96/bacpypes3/errors.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.110239 bacpypes3-0.0.96/bacpypes3/ipv4/
--rw-rw-r--   0 joel      (1000) joel      (1000)     9911 2024-01-20 06:39:19.000000 bacpypes3-0.0.96/bacpypes3/ipv4/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.96/bacpypes3/ipv4/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.96/bacpypes3/ipv4/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.96/bacpypes3/ipv4/link.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.96/bacpypes3/ipv4/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.110239 bacpypes3-0.0.96/bacpypes3/ipv6/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6919 2024-01-20 06:39:19.000000 bacpypes3-0.0.96/bacpypes3/ipv6/__init__.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.96/bacpypes3/ipv6/bvll.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.96/bacpypes3/ipv6/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.110239 bacpypes3-0.0.96/bacpypes3/json/
--rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.96/bacpypes3/json/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.96/bacpypes3/json/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/bacpypes3/json/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.110239 bacpypes3-0.0.96/bacpypes3/lib/
--rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.96/bacpypes3/lib/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    15883 2023-11-13 00:20:14.000000 bacpypes3-0.0.96/bacpypes3/lib/batchread.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.110239 bacpypes3-0.0.96/bacpypes3/local/
--rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/bacpypes3/local/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5836 2024-03-21 05:28:34.000000 bacpypes3-0.0.96/bacpypes3/local/analog.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4696 2024-03-21 05:28:34.000000 bacpypes3-0.0.96/bacpypes3/local/binary.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.96/bacpypes3/local/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.96/bacpypes3/local/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.96/bacpypes3/local/device.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    89092 2024-03-31 21:04:35.000000 bacpypes3-0.0.96/bacpypes3/local/event.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.96/bacpypes3/local/fault.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1998 2024-03-21 05:28:34.000000 bacpypes3-0.0.96/bacpypes3/local/multistate.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.96/bacpypes3/local/networkport.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.96/bacpypes3/local/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.96/bacpypes3/local/oos.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    24849 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/bacpypes3/local/schedule.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    82059 2024-03-31 21:04:35.000000 bacpypes3-0.0.96/bacpypes3/netservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.96/bacpypes3/npdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    91150 2024-05-24 03:42:08.000000 bacpypes3-0.0.96/bacpypes3/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    66217 2024-03-31 21:04:35.000000 bacpypes3-0.0.96/bacpypes3/pdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    95071 2024-04-22 04:44:28.000000 bacpypes3-0.0.96/bacpypes3/primitivedata.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.114239 bacpypes3-0.0.96/bacpypes3/rdf/
--rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.96/bacpypes3/rdf/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.96/bacpypes3/rdf/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10764 2024-04-02 15:17:43.000000 bacpypes3-0.0.96/bacpypes3/rdf/core.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    19657 2024-04-22 04:44:28.000000 bacpypes3-0.0.96/bacpypes3/rdf/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.114239 bacpypes3-0.0.96/bacpypes3/sc/
--rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/bacpypes3/sc/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/bacpypes3/sc/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.96/bacpypes3/sc/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.114239 bacpypes3-0.0.96/bacpypes3/service/
--rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.96/bacpypes3/service/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22864 2023-10-31 15:28:33.000000 bacpypes3-0.0.96/bacpypes3/service/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23249 2023-09-15 04:35:23.000000 bacpypes3-0.0.96/bacpypes3/service/device.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    40398 2024-03-21 12:00:37.000000 bacpypes3-0.0.96/bacpypes3/service/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.96/bacpypes3/settings.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3854 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/bacpypes3/vendor.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.114239 bacpypes3-0.0.96/bacpypes3/vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.96/bacpypes3/vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.96/bacpypes3/vlan/link.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.122239 bacpypes3-0.0.96/bacpypes3.egg-info/
--rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-05-24 03:43:00.000000 bacpypes3-0.0.96/bacpypes3.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     3099 2024-05-24 03:43:00.000000 bacpypes3-0.0.96/bacpypes3.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2024-05-24 03:43:00.000000 bacpypes3-0.0.96/bacpypes3.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.96/bacpypes3.egg-info/not-zip-safe
--rw-rw-r--   0 joel      (1000) joel      (1000)       16 2024-05-24 03:43:00.000000 bacpypes3-0.0.96/bacpypes3.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      101 2023-10-23 02:32:34.000000 bacpypes3-0.0.96/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-05-24 03:43:00.122239 bacpypes3-0.0.96/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.96/setup.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.114239 bacpypes3-0.0.96/tests/
--rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/clocked_test.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/conftest.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/state_machine.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_1.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test__template.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.118239 bacpypes3-0.0.96/tests/test_constructed_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_any.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_array.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_choice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_list.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_read_property_multiple.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_sequence.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_constructed_data/test_sequence_of.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.118239 bacpypes3-0.0.96/tests/test_pdu/
--rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_pdu/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16956 2024-03-31 21:04:35.000000 bacpypes3-0.0.96/tests/test_pdu/test_address.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_pdu/test_pci.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_pdu/test_pdu.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.118239 bacpypes3-0.0.96/tests/test_primitive_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_bit_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_boolean.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_character_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4503 2024-04-22 04:44:28.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_date.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_double.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_enumerated.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_integer.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_null.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_object_identifier.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_octet_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_real.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_tag.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3648 2024-04-22 04:44:28.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_time.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.96/tests/test_primitive_data/test_unsigned.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.118239 bacpypes3-0.0.96/tests/test_utilities/
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_utilities/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_utilities/test_state_machine.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-24 03:43:00.118239 bacpypes3-0.0.96/tests/test_vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_vlan/test_ipv4_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_vlan/test_ipv4_router.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/test_vlan/test_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/trapped_classes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.96/tests/utilities.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.181564 bacpypes3-0.0.97/
+-rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-05-26 03:43:05.181564 bacpypes3-0.0.97/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.97/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.165564 bacpypes3-0.0.97/bacpypes3/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1391 2024-05-26 03:42:27.000000 bacpypes3-0.0.97/bacpypes3/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    25537 2023-10-23 02:32:34.000000 bacpypes3-0.0.97/bacpypes3/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    56670 2023-10-23 02:32:34.000000 bacpypes3-0.0.97/bacpypes3/apdu.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    34748 2024-03-21 12:00:37.000000 bacpypes3-0.0.97/bacpypes3/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    65965 2023-10-31 15:46:12.000000 bacpypes3-0.0.97/bacpypes3/appservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    21688 2024-03-31 21:04:35.000000 bacpypes3-0.0.97/bacpypes3/argparse.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)   106036 2024-05-24 03:42:08.000000 bacpypes3-0.0.97/bacpypes3/basetypes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16296 2023-10-14 01:56:06.000000 bacpypes3-0.0.97/bacpypes3/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.97/bacpypes3/comm.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.97/bacpypes3/console.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64650 2024-05-26 03:42:27.000000 bacpypes3-0.0.97/bacpypes3/constructeddata.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10659 2023-06-29 13:02:40.000000 bacpypes3-0.0.97/bacpypes3/debugging.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.97/bacpypes3/errors.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.169564 bacpypes3-0.0.97/bacpypes3/ipv4/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9911 2024-01-20 06:39:19.000000 bacpypes3-0.0.97/bacpypes3/ipv4/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.97/bacpypes3/ipv4/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.97/bacpypes3/ipv4/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.97/bacpypes3/ipv4/link.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.97/bacpypes3/ipv4/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.169564 bacpypes3-0.0.97/bacpypes3/ipv6/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6919 2024-01-20 06:39:19.000000 bacpypes3-0.0.97/bacpypes3/ipv6/__init__.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.97/bacpypes3/ipv6/bvll.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.97/bacpypes3/ipv6/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.169564 bacpypes3-0.0.97/bacpypes3/json/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.97/bacpypes3/json/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.97/bacpypes3/json/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/bacpypes3/json/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.169564 bacpypes3-0.0.97/bacpypes3/lib/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.97/bacpypes3/lib/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    15883 2023-11-13 00:20:14.000000 bacpypes3-0.0.97/bacpypes3/lib/batchread.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.173564 bacpypes3-0.0.97/bacpypes3/local/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      463 2023-10-23 02:32:34.000000 bacpypes3-0.0.97/bacpypes3/local/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5836 2024-03-21 05:28:34.000000 bacpypes3-0.0.97/bacpypes3/local/analog.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4696 2024-03-21 05:28:34.000000 bacpypes3-0.0.97/bacpypes3/local/binary.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6059 2023-06-20 12:14:17.000000 bacpypes3-0.0.97/bacpypes3/local/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18826 2023-06-20 12:14:17.000000 bacpypes3-0.0.97/bacpypes3/local/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.97/bacpypes3/local/device.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    89092 2024-03-31 21:04:35.000000 bacpypes3-0.0.97/bacpypes3/local/event.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    14523 2023-06-21 18:50:45.000000 bacpypes3-0.0.97/bacpypes3/local/fault.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1998 2024-03-21 05:28:34.000000 bacpypes3-0.0.97/bacpypes3/local/multistate.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5022 2023-07-01 17:57:36.000000 bacpypes3-0.0.97/bacpypes3/local/networkport.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23309 2023-06-21 18:50:45.000000 bacpypes3-0.0.97/bacpypes3/local/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.97/bacpypes3/local/oos.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    24849 2023-10-23 02:32:34.000000 bacpypes3-0.0.97/bacpypes3/local/schedule.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    82059 2024-03-31 21:04:35.000000 bacpypes3-0.0.97/bacpypes3/netservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.97/bacpypes3/npdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    91149 2024-05-26 03:42:27.000000 bacpypes3-0.0.97/bacpypes3/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    66217 2024-03-31 21:04:35.000000 bacpypes3-0.0.97/bacpypes3/pdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    95071 2024-04-22 04:44:28.000000 bacpypes3-0.0.97/bacpypes3/primitivedata.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.173564 bacpypes3-0.0.97/bacpypes3/rdf/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.97/bacpypes3/rdf/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.97/bacpypes3/rdf/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10764 2024-04-02 15:17:43.000000 bacpypes3-0.0.97/bacpypes3/rdf/core.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    19657 2024-04-22 04:44:28.000000 bacpypes3-0.0.97/bacpypes3/rdf/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.173564 bacpypes3-0.0.97/bacpypes3/sc/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/bacpypes3/sc/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/bacpypes3/sc/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.97/bacpypes3/sc/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.173564 bacpypes3-0.0.97/bacpypes3/service/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.97/bacpypes3/service/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22864 2023-10-31 15:28:33.000000 bacpypes3-0.0.97/bacpypes3/service/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23249 2023-09-15 04:35:23.000000 bacpypes3-0.0.97/bacpypes3/service/device.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    40398 2024-03-21 12:00:37.000000 bacpypes3-0.0.97/bacpypes3/service/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3869 2023-05-31 11:51:39.000000 bacpypes3-0.0.97/bacpypes3/settings.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3854 2023-10-23 02:32:34.000000 bacpypes3-0.0.97/bacpypes3/vendor.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.173564 bacpypes3-0.0.97/bacpypes3/vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)    11838 2023-07-01 17:57:36.000000 bacpypes3-0.0.97/bacpypes3/vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1692 2023-07-01 17:57:36.000000 bacpypes3-0.0.97/bacpypes3/vlan/link.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.181564 bacpypes3-0.0.97/bacpypes3.egg-info/
+-rw-r--r--   0 joel      (1000) joel      (1000)      666 2024-05-26 03:43:05.000000 bacpypes3-0.0.97/bacpypes3.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3099 2024-05-26 03:43:05.000000 bacpypes3-0.0.97/bacpypes3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2024-05-26 03:43:05.000000 bacpypes3-0.0.97/bacpypes3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.97/bacpypes3.egg-info/not-zip-safe
+-rw-rw-r--   0 joel      (1000) joel      (1000)       16 2024-05-26 03:43:05.000000 bacpypes3-0.0.97/bacpypes3.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      101 2023-10-23 02:32:34.000000 bacpypes3-0.0.97/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2024-05-26 03:43:05.181564 bacpypes3-0.0.97/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.97/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.177564 bacpypes3-0.0.97/tests/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/clocked_test.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/conftest.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/state_machine.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_1.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test__template.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.177564 bacpypes3-0.0.97/tests/test_constructed_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_any.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_array.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_choice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_list.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_read_property_multiple.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_sequence.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_constructed_data/test_sequence_of.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.177564 bacpypes3-0.0.97/tests/test_pdu/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_pdu/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16956 2024-03-31 21:04:35.000000 bacpypes3-0.0.97/tests/test_pdu/test_address.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_pdu/test_pci.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_pdu/test_pdu.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.177564 bacpypes3-0.0.97/tests/test_primitive_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_bit_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_boolean.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_character_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4503 2024-04-22 04:44:28.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_date.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_double.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_enumerated.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_integer.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_null.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_object_identifier.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_octet_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_real.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_tag.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3648 2024-04-22 04:44:28.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_time.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.97/tests/test_primitive_data/test_unsigned.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.181564 bacpypes3-0.0.97/tests/test_utilities/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_utilities/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_utilities/test_state_machine.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2024-05-26 03:43:05.181564 bacpypes3-0.0.97/tests/test_vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_vlan/test_ipv4_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_vlan/test_ipv4_router.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/test_vlan/test_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/trapped_classes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.97/tests/utilities.py
```

### Comparing `bacpypes3-0.0.96/PKG-INFO` & `bacpypes3-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.96
+Version: 0.0.97
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.96/bacpypes3/__init__.py` & `bacpypes3-0.0.97/bacpypes3/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.96"
+__version__ = "0.0.97"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

### Comparing `bacpypes3-0.0.96/bacpypes3/__main__.py` & `bacpypes3-0.0.97/bacpypes3/__main__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/apdu.py` & `bacpypes3-0.0.97/bacpypes3/apdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/app.py` & `bacpypes3-0.0.97/bacpypes3/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/appservice.py` & `bacpypes3-0.0.97/bacpypes3/appservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/argparse.py` & `bacpypes3-0.0.97/bacpypes3/argparse.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/basetypes.py` & `bacpypes3-0.0.97/bacpypes3/basetypes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/cmd.py` & `bacpypes3-0.0.97/bacpypes3/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/comm.py` & `bacpypes3-0.0.97/bacpypes3/comm.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/console.py` & `bacpypes3-0.0.97/bacpypes3/console.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/constructeddata.py` & `bacpypes3-0.0.97/bacpypes3/constructeddata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1392,15 +1392,15 @@
             Array._debug("    - value: %r", value)
         if inspect.isawaitable(value):
             if _debug:
                 Array._debug("    - awaitable")
             value = await value
 
         # check the index
-        if index is not None:
+        if index is not None and value is not None:
             if (index < 0) or (index > len(value)):
                 raise PropertyError("invalidArrayIndex")
             if index == 0:
                 value = Unsigned(len(value))
             else:
                 value = value[index - 1]
```

### Comparing `bacpypes3-0.0.96/bacpypes3/debugging.py` & `bacpypes3-0.0.97/bacpypes3/debugging.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/errors.py` & `bacpypes3-0.0.97/bacpypes3/errors.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv4/__init__.py` & `bacpypes3-0.0.97/bacpypes3/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv4/app.py` & `bacpypes3-0.0.97/bacpypes3/ipv4/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv4/bvll.py` & `bacpypes3-0.0.97/bacpypes3/ipv4/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv4/link.py` & `bacpypes3-0.0.97/bacpypes3/ipv4/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv4/service.py` & `bacpypes3-0.0.97/bacpypes3/ipv4/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv6/__init__.py` & `bacpypes3-0.0.97/bacpypes3/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv6/bvll.py` & `bacpypes3-0.0.97/bacpypes3/ipv6/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/ipv6/service.py` & `bacpypes3-0.0.97/bacpypes3/ipv6/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/json/util.py` & `bacpypes3-0.0.97/bacpypes3/json/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/lib/batchread.py` & `bacpypes3-0.0.97/bacpypes3/lib/batchread.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/analog.py` & `bacpypes3-0.0.97/bacpypes3/local/analog.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/binary.py` & `bacpypes3-0.0.97/bacpypes3/local/binary.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/cmd.py` & `bacpypes3-0.0.97/bacpypes3/local/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/cov.py` & `bacpypes3-0.0.97/bacpypes3/local/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/device.py` & `bacpypes3-0.0.97/bacpypes3/local/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/event.py` & `bacpypes3-0.0.97/bacpypes3/local/event.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/fault.py` & `bacpypes3-0.0.97/bacpypes3/local/fault.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/multistate.py` & `bacpypes3-0.0.97/bacpypes3/local/multistate.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/networkport.py` & `bacpypes3-0.0.97/bacpypes3/local/networkport.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/object.py` & `bacpypes3-0.0.97/bacpypes3/local/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/oos.py` & `bacpypes3-0.0.97/bacpypes3/local/oos.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/local/schedule.py` & `bacpypes3-0.0.97/bacpypes3/local/schedule.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/netservice.py` & `bacpypes3-0.0.97/bacpypes3/netservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/npdu.py` & `bacpypes3-0.0.97/bacpypes3/npdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/object.py` & `bacpypes3-0.0.97/bacpypes3/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1824,15 +1824,15 @@
     presentValue: Double
     statusFlags: StatusFlags
     eventState: EventState
     reliability: Reliability
     outOfService: Boolean
     units: EngineeringUnits
     priorityArray: ArrayOf(PriorityValue, _length=16)
-    relinquishDefault: Integer
+    relinquishDefault: Double
     covIncrement: Double
     timeDelay: Unsigned
     notificationClass: Unsigned
     highLimit: Double
     lowLimit: Double
     deadband: Double
     limitEnable: LimitEnable
```

### Comparing `bacpypes3-0.0.96/bacpypes3/pdu.py` & `bacpypes3-0.0.97/bacpypes3/pdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/primitivedata.py` & `bacpypes3-0.0.97/bacpypes3/primitivedata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/rdf/core.py` & `bacpypes3-0.0.97/bacpypes3/rdf/core.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/rdf/util.py` & `bacpypes3-0.0.97/bacpypes3/rdf/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/sc/bvll.py` & `bacpypes3-0.0.97/bacpypes3/sc/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/sc/service.py` & `bacpypes3-0.0.97/bacpypes3/sc/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/service/cov.py` & `bacpypes3-0.0.97/bacpypes3/service/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/service/device.py` & `bacpypes3-0.0.97/bacpypes3/service/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/service/object.py` & `bacpypes3-0.0.97/bacpypes3/service/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/settings.py` & `bacpypes3-0.0.97/bacpypes3/settings.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/vendor.py` & `bacpypes3-0.0.97/bacpypes3/vendor.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/vlan/__init__.py` & `bacpypes3-0.0.97/bacpypes3/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3/vlan/link.py` & `bacpypes3-0.0.97/bacpypes3/vlan/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/bacpypes3.egg-info/PKG-INFO` & `bacpypes3-0.0.97/bacpypes3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.96
+Version: 0.0.97
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.96/bacpypes3.egg-info/SOURCES.txt` & `bacpypes3-0.0.97/bacpypes3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/setup.py` & `bacpypes3-0.0.97/setup.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/clocked_test.py` & `bacpypes3-0.0.97/tests/clocked_test.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/state_machine.py` & `bacpypes3-0.0.97/tests/state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_1.py` & `bacpypes3-0.0.97/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test__template.py` & `bacpypes3-0.0.97/tests/test__template.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_any.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_any.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_array.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_array.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_choice.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_choice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_list.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_list.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_read_property_multiple.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_read_property_multiple.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_sequence.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_constructed_data/test_sequence_of.py` & `bacpypes3-0.0.97/tests/test_constructed_data/test_sequence_of.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_pdu/test_address.py` & `bacpypes3-0.0.97/tests/test_pdu/test_address.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_bit_string.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_bit_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_boolean.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_boolean.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_character_string.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_character_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_date.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_date.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_double.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_double.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_enumerated.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_enumerated.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_integer.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_integer.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_null.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_null.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_object_identifier.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_object_identifier.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_octet_string.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_octet_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_real.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_real.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_tag.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_tag.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_time.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_time.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_primitive_data/test_unsigned.py` & `bacpypes3-0.0.97/tests/test_primitive_data/test_unsigned.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_utilities/test_state_machine.py` & `bacpypes3-0.0.97/tests/test_utilities/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_vlan/test_ipv4_network.py` & `bacpypes3-0.0.97/tests/test_vlan/test_ipv4_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_vlan/test_ipv4_router.py` & `bacpypes3-0.0.97/tests/test_vlan/test_ipv4_router.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/test_vlan/test_network.py` & `bacpypes3-0.0.97/tests/test_vlan/test_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/trapped_classes.py` & `bacpypes3-0.0.97/tests/trapped_classes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.96/tests/utilities.py` & `bacpypes3-0.0.97/tests/utilities.py`

 * *Files identical despite different names*

