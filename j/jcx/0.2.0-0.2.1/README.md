# Comparing `tmp/jcx-0.2.0.tar.gz` & `tmp/jcx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jcx-0.2.0.tar", max compression
+gzip compressed data, was "jcx-0.2.1.tar", max compression
```

## Comparing `jcx-0.2.0.tar` & `jcx-0.2.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     1063 2023-11-16 06:13:34.448469 jcx-0.2.0/LICENSE
--rw-r--r--   0        0        0       32 2023-11-16 04:38:43.218700 jcx-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/api/__init__.py
--rw-r--r--   0        0        0     1519 2023-12-15 09:45:48.565558 jcx-0.2.0/jcx/api/command.py
--rw-r--r--   0        0        0      534 2023-12-15 09:41:49.314315 jcx-0.2.0/jcx/api/config.py
--rw-r--r--   0        0        0     2341 2023-11-30 05:07:15.062843 jcx-0.2.0/jcx/api/dao_item.py
--rw-r--r--   0        0        0     4648 2023-11-30 05:07:15.078843 jcx-0.2.0/jcx/api/dao_list.py
--rwxr-xr-x   0        0        0     1445 2023-11-15 14:04:24.216112 jcx-0.2.0/jcx/bin/cx_cp.py
--rwxr-xr-x   0        0        0     1629 2023-11-15 16:17:04.868790 jcx-0.2.0/jcx/bin/cx_cvt.py
--rwxr-xr-x   0        0        0     1687 2023-12-15 09:44:36.094773 jcx-0.2.0/jcx/bin/cx_dir_cmp.py
--rwxr-xr-x   0        0        0     1181 2023-11-15 14:04:24.216112 jcx-0.2.0/jcx/bin/cx_find.py
--rwxr-xr-x   0        0        0     1531 2023-11-15 14:04:24.216112 jcx-0.2.0/jcx/bin/cx_fst.py
--rwxr-xr-x   0        0        0     1454 2023-11-15 16:19:21.837393 jcx-0.2.0/jcx/bin/cx_hisotry_clean.py
--rwxr-xr-x   0        0        0     1242 2023-11-15 16:19:29.249425 jcx-0.2.0/jcx/bin/cx_ref_pick.py
--rwxr-xr-x   0        0        0     1137 2023-11-15 16:19:35.697454 jcx-0.2.0/jcx/bin/cx_rename.py
--rwxr-xr-x   0        0        0     1476 2023-11-15 16:19:41.085477 jcx-0.2.0/jcx/bin/cx_unpack.py
--rw-r--r--   0        0        0     1236 2023-11-15 16:19:57.729551 jcx-0.2.0/jcx/bin/mv_re.py
--rw-r--r--   0        0        0     1342 2023-11-15 16:20:05.193584 jcx-0.2.0/jcx/bin/rename_re.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/data/__init__.py
--rw-r--r--   0        0        0     1688 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/data/split.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/db/__init__.py
--rw-r--r--   0        0        0      607 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/db/counter.py
--rw-r--r--   0        0        0      621 2023-12-15 11:55:52.688121 jcx-0.2.0/jcx/db/ivariant.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/db/jdb/__init__.py
--rw-r--r--   0        0        0      253 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/db/jdb/counter.py
--rw-r--r--   0        0        0     3276 2023-11-30 07:59:17.360424 jcx-0.2.0/jcx/db/jdb/table.py
--rw-r--r--   0        0        0      877 2023-11-30 07:55:23.587267 jcx-0.2.0/jcx/db/jdb/util.py
--rw-r--r--   0        0        0     1208 2023-12-15 11:55:52.684121 jcx-0.2.0/jcx/db/jdb/variant.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/db/rdb/__init__.py
--rw-r--r--   0        0        0      582 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/db/rdb/counter.py
--rw-r--r--   0        0        0     1941 2023-12-15 13:53:46.132152 jcx-0.2.0/jcx/db/rdb/db.py
--rw-r--r--   0        0        0      610 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/db/rdb/mutithread.py
--rw-r--r--   0        0        0     1664 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/db/rdb/variant.py
--rw-r--r--   0        0        0      403 2023-11-30 06:23:40.470690 jcx-0.2.0/jcx/db/record.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/m/__init__.py
--rw-r--r--   0        0        0      683 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/m/average_meter.py
--rw-r--r--   0        0        0      430 2023-12-15 10:31:53.682016 jcx-0.2.0/jcx/m/fun.py
--rw-r--r--   0        0        0     1474 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/m/number.py
--rw-r--r--   0        0        0      368 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/m/rand.py
--rw-r--r--   0        0        0      573 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/m/sqrt.py
--rw-r--r--   0        0        0     1117 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/m/trace.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/__init__.py
--rw-r--r--   0        0        0      182 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/mqtt/README.md
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/mqtt/__init__.py
--rw-r--r--   0        0        0      164 2023-12-15 06:16:29.813390 jcx-0.2.0/jcx/net/mqtt/cfg.py
--rw-r--r--   0        0        0     1186 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/mqtt/mqtt_c.py
--rw-r--r--   0        0        0      437 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/mqtt/mqtt_s.py
--rw-r--r--   0        0        0      652 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/mqtt/publisher.py
--rw-r--r--   0        0        0     1743 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/net/mqtt/subscriber.py
--rw-r--r--   0        0        0        0 2023-11-17 03:33:51.114120 jcx-0.2.0/jcx/py.typed
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.212112 jcx-0.2.0/jcx/rs/__init__.py
--rw-r--r--   0        0        0      242 2023-11-15 14:04:24.212112 jcx-0.2.0/jcx/rs/proto.py
--rw-r--r--   0        0        0      587 2023-11-15 14:04:24.212112 jcx-0.2.0/jcx/rs/rs.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/sys/__init__.py
--rw-r--r--   0        0        0     9064 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/sys/fs.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/text/__init__.py
--rw-r--r--   0        0        0     1336 2023-11-30 05:53:03.397451 jcx-0.2.0/jcx/text/io.py
--rw-r--r--   0        0        0      391 2024-03-27 06:39:22.218548 jcx-0.2.0/jcx/text/test/txt_json_test.py
--rw-r--r--   0        0        0     1557 2023-11-30 06:01:25.713436 jcx-0.2.0/jcx/text/txt_json.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/time/__init__.py
--rw-r--r--   0        0        0     1569 2023-12-15 10:35:10.076692 jcx-0.2.0/jcx/time/calendar_type.py
--rw-r--r--   0        0        0     2042 2024-03-27 09:06:49.944599 jcx-0.2.0/jcx/time/clock_time.py
--rw-r--r--   0        0        0     1296 2023-12-15 09:44:36.098773 jcx-0.2.0/jcx/time/count_timer.py
--rw-r--r--   0        0        0     1068 2023-11-15 14:04:24.228112 jcx-0.2.0/jcx/time/dt.py
--rw-r--r--   0        0        0      158 2024-03-27 09:09:57.222022 jcx-0.2.0/jcx/time/test/clock_time_test.py
--rw-r--r--   0        0        0      709 2023-11-15 14:04:24.224112 jcx-0.2.0/jcx/time/timer.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/ui/__init__.py
--rw-r--r--   0        0        0      618 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/ui/key.py
--rw-r--r--   0        0        0      618 2023-11-15 14:04:24.232113 jcx-0.2.0/jcx/ui/progress_meter.py
--rw-r--r--   0        0        0        0 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/util/__init__.py
--rw-r--r--   0        0        0      873 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/util/algo.py
--rw-r--r--   0        0        0      291 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/util/array.py
--rw-r--r--   0        0        0     1167 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/util/err.py
--rw-r--r--   0        0        0     2189 2023-12-15 10:37:31.440752 jcx-0.2.0/jcx/util/lict.py
--rw-r--r--   0        0        0     1230 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/util/mutithread.py
--rw-r--r--   0        0        0      228 2023-12-15 09:29:14.150230 jcx-0.2.0/jcx/util/oo.py
--rw-r--r--   0        0        0      144 2023-11-15 14:04:24.220112 jcx-0.2.0/jcx/util/trace.py
--rw-r--r--   0        0        0      467 2024-03-27 09:07:08.168738 jcx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 jcx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-11-16 06:13:34.448469 jcx-0.2.1/LICENSE
+-rw-r--r--   0        0        0       32 2023-11-16 04:38:43.218700 jcx-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/api/__init__.py
+-rw-r--r--   0        0        0     1519 2023-12-15 09:45:48.565558 jcx-0.2.1/jcx/api/command.py
+-rw-r--r--   0        0        0      534 2023-12-15 09:41:49.314315 jcx-0.2.1/jcx/api/config.py
+-rw-r--r--   0        0        0     2341 2023-11-30 05:07:15.062843 jcx-0.2.1/jcx/api/dao_item.py
+-rw-r--r--   0        0        0     4648 2023-11-30 05:07:15.078843 jcx-0.2.1/jcx/api/dao_list.py
+-rwxr-xr-x   0        0        0     1445 2023-11-15 14:04:24.216112 jcx-0.2.1/jcx/bin/cx_cp.py
+-rwxr-xr-x   0        0        0     1629 2023-11-15 16:17:04.868790 jcx-0.2.1/jcx/bin/cx_cvt.py
+-rwxr-xr-x   0        0        0     1687 2023-12-15 09:44:36.094773 jcx-0.2.1/jcx/bin/cx_dir_cmp.py
+-rwxr-xr-x   0        0        0     1181 2023-11-15 14:04:24.216112 jcx-0.2.1/jcx/bin/cx_find.py
+-rwxr-xr-x   0        0        0     1531 2023-11-15 14:04:24.216112 jcx-0.2.1/jcx/bin/cx_fst.py
+-rwxr-xr-x   0        0        0     1454 2023-11-15 16:19:21.837393 jcx-0.2.1/jcx/bin/cx_hisotry_clean.py
+-rwxr-xr-x   0        0        0     1242 2023-11-15 16:19:29.249425 jcx-0.2.1/jcx/bin/cx_ref_pick.py
+-rwxr-xr-x   0        0        0     1137 2023-11-15 16:19:35.697454 jcx-0.2.1/jcx/bin/cx_rename.py
+-rwxr-xr-x   0        0        0     1476 2023-11-15 16:19:41.085477 jcx-0.2.1/jcx/bin/cx_unpack.py
+-rw-r--r--   0        0        0     1236 2023-11-15 16:19:57.729551 jcx-0.2.1/jcx/bin/mv_re.py
+-rw-r--r--   0        0        0     1342 2023-11-15 16:20:05.193584 jcx-0.2.1/jcx/bin/rename_re.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/data/__init__.py
+-rw-r--r--   0        0        0     1688 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/data/split.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/db/__init__.py
+-rw-r--r--   0        0        0      607 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/db/counter.py
+-rw-r--r--   0        0        0      621 2023-12-15 11:55:52.688121 jcx-0.2.1/jcx/db/ivariant.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/db/jdb/__init__.py
+-rw-r--r--   0        0        0      253 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/db/jdb/counter.py
+-rw-r--r--   0        0        0     3276 2023-11-30 07:59:17.360424 jcx-0.2.1/jcx/db/jdb/table.py
+-rw-r--r--   0        0        0      877 2023-11-30 07:55:23.587267 jcx-0.2.1/jcx/db/jdb/util.py
+-rw-r--r--   0        0        0     1208 2023-12-15 11:55:52.684121 jcx-0.2.1/jcx/db/jdb/variant.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/db/rdb/__init__.py
+-rw-r--r--   0        0        0      582 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/db/rdb/counter.py
+-rw-r--r--   0        0        0     1941 2023-12-15 13:53:46.132152 jcx-0.2.1/jcx/db/rdb/db.py
+-rw-r--r--   0        0        0      610 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/db/rdb/mutithread.py
+-rw-r--r--   0        0        0     1664 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/db/rdb/variant.py
+-rw-r--r--   0        0        0      403 2023-11-30 06:23:40.470690 jcx-0.2.1/jcx/db/record.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/m/__init__.py
+-rw-r--r--   0        0        0      683 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/m/average_meter.py
+-rw-r--r--   0        0        0      430 2023-12-15 10:31:53.682016 jcx-0.2.1/jcx/m/fun.py
+-rw-r--r--   0        0        0     1474 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/m/number.py
+-rw-r--r--   0        0        0      368 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/m/rand.py
+-rw-r--r--   0        0        0      573 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/m/sqrt.py
+-rw-r--r--   0        0        0     1117 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/m/trace.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/__init__.py
+-rw-r--r--   0        0        0      182 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/mqtt/README.md
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/mqtt/__init__.py
+-rw-r--r--   0        0        0      164 2023-12-15 06:16:29.813390 jcx-0.2.1/jcx/net/mqtt/cfg.py
+-rw-r--r--   0        0        0     1186 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/mqtt/mqtt_c.py
+-rw-r--r--   0        0        0      437 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/mqtt/mqtt_s.py
+-rw-r--r--   0        0        0      652 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/mqtt/publisher.py
+-rw-r--r--   0        0        0     1743 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/net/mqtt/subscriber.py
+-rw-r--r--   0        0        0        0 2023-11-17 03:33:51.114120 jcx-0.2.1/jcx/py.typed
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.212112 jcx-0.2.1/jcx/rs/__init__.py
+-rw-r--r--   0        0        0      242 2023-11-15 14:04:24.212112 jcx-0.2.1/jcx/rs/proto.py
+-rw-r--r--   0        0        0      587 2023-11-15 14:04:24.212112 jcx-0.2.1/jcx/rs/rs.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/sys/__init__.py
+-rw-r--r--   0        0        0     9064 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/sys/fs.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/text/__init__.py
+-rw-r--r--   0        0        0     1336 2023-11-30 05:53:03.397451 jcx-0.2.1/jcx/text/io.py
+-rw-r--r--   0        0        0      391 2024-03-27 06:39:22.218548 jcx-0.2.1/jcx/text/test/txt_json_test.py
+-rw-r--r--   0        0        0     1557 2023-11-30 06:01:25.713436 jcx-0.2.1/jcx/text/txt_json.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/time/__init__.py
+-rw-r--r--   0        0        0     1569 2023-12-15 10:35:10.076692 jcx-0.2.1/jcx/time/calendar_type.py
+-rw-r--r--   0        0        0     2042 2024-03-27 09:06:49.944599 jcx-0.2.1/jcx/time/clock_time.py
+-rw-r--r--   0        0        0     1296 2023-12-15 09:44:36.098773 jcx-0.2.1/jcx/time/count_timer.py
+-rw-r--r--   0        0        0     1068 2023-11-15 14:04:24.228112 jcx-0.2.1/jcx/time/dt.py
+-rw-r--r--   0        0        0      158 2024-03-27 09:09:57.222022 jcx-0.2.1/jcx/time/test/clock_time_test.py
+-rw-r--r--   0        0        0      709 2023-11-15 14:04:24.224112 jcx-0.2.1/jcx/time/timer.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/ui/__init__.py
+-rw-r--r--   0        0        0      618 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/ui/key.py
+-rw-r--r--   0        0        0      618 2023-11-15 14:04:24.232113 jcx-0.2.1/jcx/ui/progress_meter.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/util/__init__.py
+-rw-r--r--   0        0        0      873 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/util/algo.py
+-rw-r--r--   0        0        0      291 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/util/array.py
+-rw-r--r--   0        0        0     1167 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/util/err.py
+-rw-r--r--   0        0        0     2189 2023-12-15 10:37:31.440752 jcx-0.2.1/jcx/util/lict.py
+-rw-r--r--   0        0        0     1230 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/util/mutithread.py
+-rw-r--r--   0        0        0      228 2023-12-15 09:29:14.150230 jcx-0.2.1/jcx/util/oo.py
+-rw-r--r--   0        0        0      144 2023-11-15 14:04:24.220112 jcx-0.2.1/jcx/util/trace.py
+-rw-r--r--   0        0        0      467 2024-05-26 02:17:10.341821 jcx-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 jcx-0.2.1/PKG-INFO
```

### Comparing `jcx-0.2.0/LICENSE` & `jcx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/api/command.py` & `jcx-0.2.1/jcx/api/command.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/api/config.py` & `jcx-0.2.1/jcx/api/config.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/api/dao_item.py` & `jcx-0.2.1/jcx/api/dao_item.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/api/dao_list.py` & `jcx-0.2.1/jcx/api/dao_list.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_cp.py` & `jcx-0.2.1/jcx/bin/cx_cp.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_cvt.py` & `jcx-0.2.1/jcx/bin/cx_cvt.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_dir_cmp.py` & `jcx-0.2.1/jcx/bin/cx_dir_cmp.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_find.py` & `jcx-0.2.1/jcx/bin/cx_find.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_fst.py` & `jcx-0.2.1/jcx/bin/cx_fst.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_hisotry_clean.py` & `jcx-0.2.1/jcx/bin/cx_hisotry_clean.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_ref_pick.py` & `jcx-0.2.1/jcx/bin/cx_ref_pick.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_rename.py` & `jcx-0.2.1/jcx/bin/cx_rename.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/cx_unpack.py` & `jcx-0.2.1/jcx/bin/cx_unpack.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/mv_re.py` & `jcx-0.2.1/jcx/bin/mv_re.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/bin/rename_re.py` & `jcx-0.2.1/jcx/bin/rename_re.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/data/split.py` & `jcx-0.2.1/jcx/data/split.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/counter.py` & `jcx-0.2.1/jcx/db/counter.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/ivariant.py` & `jcx-0.2.1/jcx/db/ivariant.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/jdb/table.py` & `jcx-0.2.1/jcx/db/jdb/table.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/jdb/util.py` & `jcx-0.2.1/jcx/db/jdb/util.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/jdb/variant.py` & `jcx-0.2.1/jcx/db/jdb/variant.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/rdb/counter.py` & `jcx-0.2.1/jcx/db/rdb/counter.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/rdb/db.py` & `jcx-0.2.1/jcx/db/rdb/db.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/rdb/mutithread.py` & `jcx-0.2.1/jcx/db/rdb/mutithread.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/db/rdb/variant.py` & `jcx-0.2.1/jcx/db/rdb/variant.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/m/average_meter.py` & `jcx-0.2.1/jcx/m/average_meter.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/m/number.py` & `jcx-0.2.1/jcx/m/number.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/m/sqrt.py` & `jcx-0.2.1/jcx/m/sqrt.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/m/trace.py` & `jcx-0.2.1/jcx/m/trace.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/net/mqtt/mqtt_c.py` & `jcx-0.2.1/jcx/net/mqtt/mqtt_c.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/net/mqtt/publisher.py` & `jcx-0.2.1/jcx/net/mqtt/publisher.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/net/mqtt/subscriber.py` & `jcx-0.2.1/jcx/net/mqtt/subscriber.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/rs/rs.py` & `jcx-0.2.1/jcx/rs/rs.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/sys/fs.py` & `jcx-0.2.1/jcx/sys/fs.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/text/io.py` & `jcx-0.2.1/jcx/text/io.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/text/txt_json.py` & `jcx-0.2.1/jcx/text/txt_json.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/time/calendar_type.py` & `jcx-0.2.1/jcx/time/calendar_type.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/time/clock_time.py` & `jcx-0.2.1/jcx/time/clock_time.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/time/count_timer.py` & `jcx-0.2.1/jcx/time/count_timer.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/time/dt.py` & `jcx-0.2.1/jcx/time/dt.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/time/timer.py` & `jcx-0.2.1/jcx/time/timer.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/ui/key.py` & `jcx-0.2.1/jcx/ui/key.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/ui/progress_meter.py` & `jcx-0.2.1/jcx/ui/progress_meter.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/util/algo.py` & `jcx-0.2.1/jcx/util/algo.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/util/err.py` & `jcx-0.2.1/jcx/util/err.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/util/lict.py` & `jcx-0.2.1/jcx/util/lict.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/jcx/util/mutithread.py` & `jcx-0.2.1/jcx/util/mutithread.py`

 * *Files identical despite different names*

### Comparing `jcx-0.2.0/PKG-INFO` & `jcx-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jcx
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: dayn9t
 Author-email: dayn9t@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

