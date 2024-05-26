# Comparing `tmp/jaeger-1.7.2.tar.gz` & `tmp/jaeger-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.7.2.tar", max compression
+gzip compressed data, was "jaeger-1.7.3.tar", max compression
```

## Comparing `jaeger-1.7.2.tar` & `jaeger-1.7.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1504 2024-05-24 18:30:47.797006 jaeger-1.7.2/LICENSE.md
--rw-r--r--   0        0        0     2393 2024-05-24 18:30:47.797006 jaeger-1.7.2/README.md
--rw-r--r--   0        0        0     3613 2024-05-24 18:30:47.801006 jaeger-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1764 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/__init__.py
--rw-r--r--   0        0        0    20331 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5033 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    35429 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      722 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2690 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    15129 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11373 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5314 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16070 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9994 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1397 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14035 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/alerts.py
--rw-r--r--   0        0        0    21709 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/can.py
--rw-r--r--   0        0        0     5257 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/chiller.py
--rw-r--r--   0        0        0     4054 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22135 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/base.py
--rw-r--r--   0        0        0     9010 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12181 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10788 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6013 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/status.py
--rw-r--r--   0        0        0    26797 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2024-05-24 18:30:47.801006 jaeger-1.7.2/src/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3597 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3347 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8711 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3545 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/exceptions.py
--rw-r--r--   0        0        0    52574 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/fps.py
--rw-r--r--   0        0        0    42576 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/fvc.py
--rw-r--r--   0        0        0     4518 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6759 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12892 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1874 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1199 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    20177 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/maskbits.py
--rw-r--r--   0        0        0     7797 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/plotting.py
--rw-r--r--   0        0        0    18121 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1851 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/scripts/generate_chiller_yaml.py
--rw-r--r--   0        0        0      346 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/__init__.py
--rw-r--r--   0        0        0    19651 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/assignment.py
--rw-r--r--   0        0        0    41675 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/configuration.py
--rw-r--r--   0        0        0    19864 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/coordinates.py
--rw-r--r--   0        0        0    12248 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/design.py
--rw-r--r--   0        0        0     6580 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/schemas.py
--rw-r--r--   0        0        0    11232 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/too.py
--rw-r--r--   0        0        0    16554 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/target/tools.py
--rw-r--r--   0        0        0    15709 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/testing.py
--rw-r--r--   0        0        0       60 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9610 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/database.py
--rw-r--r--   0        0        0    14611 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9164 2024-05-24 18:30:47.805006 jaeger-1.7.2/src/jaeger/utils/utils.py
--rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 jaeger-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-26 18:08:20.314605 jaeger-1.7.3/LICENSE.md
+-rw-r--r--   0        0        0     2393 2024-05-26 18:08:20.314605 jaeger-1.7.3/README.md
+-rw-r--r--   0        0        0     3613 2024-05-26 18:08:20.318605 jaeger-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1764 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    35429 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      722 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    15129 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11373 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1397 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14035 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/can.py
+-rw-r--r--   0        0        0     5257 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/chiller.py
+-rw-r--r--   0        0        0     4054 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26797 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3597 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3347 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/exceptions.py
+-rw-r--r--   0        0        0    52574 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/fps.py
+-rw-r--r--   0        0        0    42576 2024-05-26 18:08:20.318605 jaeger-1.7.3/src/jaeger/fvc.py
+-rw-r--r--   0        0        0     4518 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    20177 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7797 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/scripts/generate_chiller_yaml.py
+-rw-r--r--   0        0        0      346 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    19651 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/assignment.py
+-rw-r--r--   0        0        0    41675 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/configuration.py
+-rw-r--r--   0        0        0    19864 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/coordinates.py
+-rw-r--r--   0        0        0    12248 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/design.py
+-rw-r--r--   0        0        0     6580 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/schemas.py
+-rw-r--r--   0        0        0    11232 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/too.py
+-rw-r--r--   0        0        0    16549 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/target/tools.py
+-rw-r--r--   0        0        0    15709 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9610 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14611 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9164 2024-05-26 18:08:20.322605 jaeger-1.7.3/src/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     4060 1970-01-01 00:00:00.000000 jaeger-1.7.3/PKG-INFO
```

### Comparing `jaeger-1.7.2/LICENSE.md` & `jaeger-1.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/README.md` & `jaeger-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/pyproject.toml` & `jaeger-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.7.2"
+version = "1.7.3"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
```

### Comparing `jaeger-1.7.2/src/jaeger/__init__.py` & `jaeger-1.7.3/src/jaeger/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/__main__.py` & `jaeger-1.7.3/src/jaeger/__main__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/actor.py` & `jaeger-1.7.3/src/jaeger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/__init__.py` & `jaeger-1.7.3/src/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/alerts.py` & `jaeger-1.7.3/src/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/can.py` & `jaeger-1.7.3/src/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/chiller.py` & `jaeger-1.7.3/src/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/configuration.py` & `jaeger-1.7.3/src/jaeger/actor/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/debug.py` & `jaeger-1.7.3/src/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/disable.py` & `jaeger-1.7.3/src/jaeger/actor/commands/disable.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/fvc.py` & `jaeger-1.7.3/src/jaeger/actor/commands/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/home.py` & `jaeger-1.7.3/src/jaeger/actor/commands/home.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/ieb.py` & `jaeger-1.7.3/src/jaeger/actor/commands/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/pollers.py` & `jaeger-1.7.3/src/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/positioner.py` & `jaeger-1.7.3/src/jaeger/actor/commands/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/power.py` & `jaeger-1.7.3/src/jaeger/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/snapshot.py` & `jaeger-1.7.3/src/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/talk.py` & `jaeger-1.7.3/src/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/testing.py` & `jaeger-1.7.3/src/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/unwind.py` & `jaeger-1.7.3/src/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/actor/commands/version.py` & `jaeger-1.7.3/src/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/alerts.py` & `jaeger-1.7.3/src/jaeger/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/can.py` & `jaeger-1.7.3/src/jaeger/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/chiller.py` & `jaeger-1.7.3/src/jaeger/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/__init__.py` & `jaeger-1.7.3/src/jaeger/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/base.py` & `jaeger-1.7.3/src/jaeger/commands/base.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/bootloader.py` & `jaeger-1.7.3/src/jaeger/commands/bootloader.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/calibration.py` & `jaeger-1.7.3/src/jaeger/commands/calibration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/goto.py` & `jaeger-1.7.3/src/jaeger/commands/goto.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/status.py` & `jaeger-1.7.3/src/jaeger/commands/status.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/commands/trajectory.py` & `jaeger-1.7.3/src/jaeger/commands/trajectory.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/chiller_APO.yaml` & `jaeger-1.7.3/src/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.7.3/src/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/fvc.yaml` & `jaeger-1.7.3/src/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/ieb_APO.yaml` & `jaeger-1.7.3/src/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.7.3/src/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/jaeger_APO.yml` & `jaeger-1.7.3/src/jaeger/etc/jaeger_APO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.7.3/src/jaeger/etc/jaeger_LCO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/schema.json` & `jaeger-1.7.3/src/jaeger/etc/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.7.3/src/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/sextants/osu.yaml` & `jaeger-1.7.3/src/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/sextants/schema.json` & `jaeger-1.7.3/src/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/etc/sextants/uw.yaml` & `jaeger-1.7.3/src/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/exceptions.py` & `jaeger-1.7.3/src/jaeger/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/fps.py` & `jaeger-1.7.3/src/jaeger/fps.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/fvc.py` & `jaeger-1.7.3/src/jaeger/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/ieb.py` & `jaeger-1.7.3/src/jaeger/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/interfaces/bus.py` & `jaeger-1.7.3/src/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/interfaces/cannet.py` & `jaeger-1.7.3/src/jaeger/interfaces/cannet.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/interfaces/message.py` & `jaeger-1.7.3/src/jaeger/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/interfaces/notifier.py` & `jaeger-1.7.3/src/jaeger/interfaces/notifier.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/interfaces/virtual.py` & `jaeger-1.7.3/src/jaeger/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/kaiju.py` & `jaeger-1.7.3/src/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/maskbits.py` & `jaeger-1.7.3/src/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/plotting.py` & `jaeger-1.7.3/src/jaeger/plotting.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/positioner.py` & `jaeger-1.7.3/src/jaeger/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.7.3/src/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/assignment.py` & `jaeger-1.7.3/src/jaeger/target/assignment.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/configuration.py` & `jaeger-1.7.3/src/jaeger/target/configuration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/coordinates.py` & `jaeger-1.7.3/src/jaeger/target/coordinates.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/design.py` & `jaeger-1.7.3/src/jaeger/target/design.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/schemas.py` & `jaeger-1.7.3/src/jaeger/target/schemas.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/too.py` & `jaeger-1.7.3/src/jaeger/target/too.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/target/tools.py` & `jaeger-1.7.3/src/jaeger/target/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # @Author: José Sánchez-Gallego (gallegoj@uw.edu)
 # @Date: 2021-11-10
 # @Filename: tools.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
+import os
 import pathlib
 import re
 from functools import cache
 
 from typing import TYPE_CHECKING, Any, Mapping
 
 import numpy
@@ -34,16 +35,14 @@
     get_path_pair_in_executor,
     get_robot_grid,
 )
 from jaeger.target.schemas import CONFIGURATION_SCHEMA, CONFSUMMARY_FIBER_MAP_SCHEMA
 
 
 if TYPE_CHECKING:
-    import os
-
     from jaeger import FPS
     from jaeger.target.configuration import BaseConfiguration
 
 
 __all__ = [
     "get_wok_data",
     "copy_summary_file",
```

### Comparing `jaeger-1.7.2/src/jaeger/testing.py` & `jaeger-1.7.3/src/jaeger/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/utils/database.py` & `jaeger-1.7.3/src/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/utils/helpers.py` & `jaeger-1.7.3/src/jaeger/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/src/jaeger/utils/utils.py` & `jaeger-1.7.3/src/jaeger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.7.2/PKG-INFO` & `jaeger-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.7.2
+Version: 1.7.3
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
```

