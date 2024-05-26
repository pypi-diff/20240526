# Comparing `tmp/pih-plb_db-0.20.5.tar.gz` & `tmp/pih-plb_db-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb_db-0.20.5.tar", last modified: Sat May 25 15:28:55 2024, max compression
+gzip compressed data, was "pih-plb_db-0.21.tar", last modified: Sun May 26 11:51:27 2024, max compression
```

## Comparing `pih-plb_db-0.20.5.tar` & `pih-plb_db-0.21.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 15:28:56.094345 pih-plb_db-0.20.5/
--rw-rw-rw-   0        0        0      282 2024-05-25 15:28:56.078698 pih-plb_db-0.20.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-25 15:28:55.640160 pih-plb_db-0.20.5/PolibaseDatabaseService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/__main__.py
--rw-rw-rw-   0        0        0    11976 2024-05-25 15:24:27.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/api.py
--rw-rw-rw-   0        0        0     1081 2024-05-25 15:24:24.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/const.py
--rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.20.5/PolibaseDatabaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-25 15:28:56.031824 pih-plb_db-0.20.5/pih_plb_db.egg-info/
--rw-rw-rw-   0        0        0      282 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-25 15:28:55.000000 pih-plb_db-0.20.5/pih_plb_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 15:28:56.109948 pih-plb_db-0.20.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-26 11:51:28.048442 pih-plb_db-0.21/
+-rw-rw-rw-   0        0        0      280 2024-05-26 11:51:28.032788 pih-plb_db-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 11:51:27.672400 pih-plb_db-0.21/PolibaseDatabaseService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-plb_db-0.21/PolibaseDatabaseService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-02-15 00:09:03.000000 pih-plb_db-0.21/PolibaseDatabaseService/__main__.py
+-rw-rw-rw-   0        0        0     9490 2024-05-26 11:47:50.000000 pih-plb_db-0.21/PolibaseDatabaseService/api.py
+-rw-rw-rw-   0        0        0      982 2024-05-26 11:51:11.000000 pih-plb_db-0.21/PolibaseDatabaseService/const.py
+-rw-rw-rw-   0        0        0     1135 2024-04-22 03:09:08.000000 pih-plb_db-0.21/PolibaseDatabaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-26 11:51:27.984890 pih-plb_db-0.21/pih_plb_db.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-26 11:51:27.000000 pih-plb_db-0.21/pih_plb_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-26 11:51:27.000000 pih-plb_db-0.21/pih_plb_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 11:51:27.000000 pih-plb_db-0.21/pih_plb_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-26 11:51:27.000000 pih-plb_db-0.21/pih_plb_db.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 11:51:27.000000 pih-plb_db-0.21/pih_plb_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-26 11:51:27.000000 pih-plb_db-0.21/pih_plb_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 11:51:28.064693 pih-plb_db-0.21/setup.cfg
```

### Comparing `pih-plb_db-0.20.5/PolibaseDatabaseService/api.py` & `pih-plb_db-0.21/PolibaseDatabaseService/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ipih
 
 import os
 from pih import A
-from pih.tools import j, n, js, nn, esc
+from pih.tools import j, n, js, nn, esc, nns
 from PolibaseDatabaseService.const import *
 
 TEST: bool = False
 #
 
 
 class PolibaseDBApi:
@@ -40,79 +40,63 @@
             file_name, DATABASE_DUMP.FILE_EXTENSION
         )
         if test:
             polibase_folder_path_src: str = polibase_folder_path
             polibase_folder_path = A.PTH.for_windows(
                 A.PTH.join(polibase_folder_path, TEST_NAME)
             )
-            A.L.debug_bot(
+            os.system(
                 js(
                     (
-                        "1:",
-                        os.system(
-                            js(
-                                (
-                                    "robocopy",
-                                    A.PTH.join(
-                                        polibase_folder_path_src, STUB_DIRECTORY_NAME
-                                    ),
-                                    polibase_folder_path,
-                                    file_database_dump_name_out,
-                                )
-                            )
-                        ),
+                        "robocopy",
+                        A.PTH.join(polibase_folder_path_src, STUB_DIRECTORY_NAME),
+                        polibase_folder_path,
+                        file_database_dump_name_out,
                     )
                 )
             )
         polibase2_folder_path: str = A.PTH.for_windows(
             A.PTH.join(A.CT_H.POLIBASE2.NAME, local_polibase_database_dump_folder_name)
         )
 
         archiver_program_path: str = 'C:/"Program Files"/7-Zip/7z'
 
         file_out_name = A.PTH.add_extension(file_name, ARCHIVE_TYPE)
 
-        nas_copy_command = js(
+        nas_folder_path: str = A.PTH.for_windows(
+            A.PTH.join(A.CT_H.NAS.IP, "backups", nas_polibase_database_dump_folder_name)
+        )
+
+        nas_copy_command: str = js(
             (
                 "robocopy",
                 polibase_folder_path,
-                j(
-                    (
-                        (
-                            PRECONNECTED_MOUNT_POINT.NAS
-                            if USE_PRECONNECTED_DISKS
-                            else MOUNT_POINT.NAS
-                        ),
-                        A.CT.SPLITTER,
-                    )
+                (
+                    nas_folder_path
+                    if USE_PRECONNECTED_DISKS
+                    else j((MOUNT_POINT.NAS, A.CT.SPLITTER))
                 ),
                 file_out_name,
                 "/J",
             )
         )
-        polibase2_copy_command = js(
+        polibase2_copy_command: str = js(
             (
                 "robocopy",
                 polibase_folder_path,
-                j(
-                    (
-                        (
-                            PRECONNECTED_MOUNT_POINT.POLIBASE2
-                            if USE_PRECONNECTED_DISKS
-                            else MOUNT_POINT.POLIBASE2
-                        ),
-                        A.CT.SPLITTER,
-                    )
+                (
+                    polibase2_folder_path
+                    if USE_PRECONNECTED_DISKS
+                    else j((MOUNT_POINT.POLIBASE2, A.CT.SPLITTER))
                 ),
                 file_database_dump_name_out,
                 "/J",
             )
         )
         os.chdir(polibase_folder_path)
-        A.L.debug_bot(js(("os.curdir:", polibase_folder_path, os.curdir)))
 
         # step 1
         A.E.backup_notify_about_polibase_creation_db_dumb_start(not test)
         if not test:
             os.system(
                 j(
                     (
@@ -128,30 +112,26 @@
                 A.PTH.join(polibase_folder_path, file_database_dump_name_out)
             ),
             not test,
         )
 
         # step 2: connect net location with credentials
         if not USE_PRECONNECTED_DISKS:
-            nas_folder_path: str = A.PTH.for_windows(
-                A.PTH.join(
-                    A.CT_H.NAS.NAME, "backups", nas_polibase_database_dump_folder_name
-                )
-            )
-            nas_create_connection_command = js(
+
+            nas_create_connection_command: str = js(
                 (
                     "net",
                     "use",
                     j((MOUNT_POINT.NAS, A.CT.SPLITTER)),
                     nas_folder_path,
                     j(("/user:", A.D_V_E.value("NAS_USER_LOGIN"))),
                     A.D_V_E.value("NAS_USER_PASSWORD"),
                 )
             )
-            polibase2_create_connection_command = js(
+            polibase2_create_connection_command: str = js(
                 (
                     "net",
                     "use",
                     j((MOUNT_POINT.POLIBASE2, A.CT.SPLITTER)),
                     polibase2_folder_path,
                 )
             )
@@ -162,76 +142,71 @@
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_start()
         archive_creation_parameters: str | None = A.S.get(
             A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_CREATION_PARAMETERS
         )
         password_parameter: str = j(
             (
                 "-p",
-                "1"
-                #esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD")),
+                (
+                    "test"
+                    if test
+                    else esc(A.D_V_E.value("POLIBASE_DATABASE_ARCHIVE_PASSWORD"))
+                ),
             )
         )
         compression_level: int | None = A.S.get(
             A.CT_S.POLIBASE_DB_DUMP_ARCHIVE_COMPRESSION_LEVEL
         )
-        A.L.debug_bot(
+
+        os.system(
             js(
                 (
-                    "arch:",
-                    os.system(
-                        js(
-                            (
-                                archiver_program_path,
+                    archiver_program_path,
+                    (
+                        (
+                            js(
                                 (
+                                    j(("a -t", ARCHIVE_TYPE)),
                                     (
-                                        js(
+                                        None
+                                        if n(compression_level)
+                                        else j(
                                             (
-                                                j(("a -t", ARCHIVE_TYPE)),
-                                                (
-                                                    None
-                                                    if n(compression_level)
-                                                    else j(
-                                                        (
-                                                            "-mx",
-                                                            compression_level,
-                                                        )
-                                                    )
-                                                ),
-                                                password_parameter,
+                                                "-mx",
+                                                compression_level,
                                             )
                                         )
-                                    )
-                                    if n(archive_creation_parameters)
-                                    else js(
-                                        (
-                                            archive_creation_parameters,
-                                            password_parameter,
-                                        )
-                                    )
-                                ),
-                                file_out_name,
-                                file_database_dump_name_out,
+                                    ),
+                                    password_parameter,
+                                )
+                            )
+                        )
+                        if n(archive_creation_parameters)
+                        else js(
+                            (
+                                archive_creation_parameters,
+                                password_parameter,
                             )
                         )
                     ),
+                    file_out_name,
+                    file_database_dump_name_out,
                 )
             )
         )
 
         A.E.backup_notify_about_polibase_creation_archived_db_dumb_complete(
             os.path.getsize(A.PTH.join(polibase_folder_path, file_out_name)), not test
         )
 
         # step 4
         A.E.backup_notify_about_polibase_coping_archived_db_dumb_start(
             A.CT_H.NAS.ALIAS.upper()
         )
-        A.L.debug_bot(
-            js(("nas_copy_command:", os.system(nas_copy_command), nas_copy_command))
-        )
+        os.system(nas_copy_command)
         A.E.backup_notify_about_polibase_coping_archived_db_dumb_complete(
             A.CT_H.NAS.ALIAS.upper()
         )
 
         # step 5
         A.E.backup_notify_about_polibase_coping_db_dumb_start(
             A.CT_H.POLIBASE2.ALIAS.upper()
@@ -243,91 +218,59 @@
 
         # step 6
         polibase2_previous_file_delete_command: str = js(
             (
                 "del",
                 A.PTH.for_windows(
                     A.PTH.join(
-                        j(
-                            (
-                                (
-                                    PRECONNECTED_MOUNT_POINT.POLIBASE2
-                                    if USE_PRECONNECTED_DISKS
-                                    else MOUNT_POINT.POLIBASE2
-                                ),
-                                A.CT.SPLITTER,
-                            )
+                        (
+                            polibase2_folder_path
+                            if USE_PRECONNECTED_DISKS
+                            else j((MOUNT_POINT.POLIBASE2, A.CT.SPLITTER))
                         ),
                         os.sep,
                         dump_file_name_result,
                     )
                 ),
             )
         )
         polibase_file_rename_command: str = js(
             (
                 "ren",
                 A.PTH.for_windows(
                     A.PTH.join(
-                        j(
-                            (
-                                (
-                                    PRECONNECTED_MOUNT_POINT.POLIBASE2
-                                    if USE_PRECONNECTED_DISKS
-                                    else MOUNT_POINT.POLIBASE2
-                                ),
-                                A.CT.SPLITTER,
-                            )
+                        (
+                            polibase2_folder_path
+                            if USE_PRECONNECTED_DISKS
+                            else j((MOUNT_POINT.POLIBASE2, A.CT.SPLITTER))
                         ),
                         os.sep,
                         file_database_dump_name_out,
                     )
                 ),
                 dump_file_name_result,
             )
         )
 
         os.system(polibase2_previous_file_delete_command)
         os.system(polibase_file_rename_command)
 
         # step 7: disconnect net location with credentials
         if not USE_PRECONNECTED_DISKS:
-            os.system(
-                js(
-                    (
-                        "net use",
-                        j(
-                            (
-                                (
-                                    PRECONNECTED_MOUNT_POINT.NAS
-                                    if USE_PRECONNECTED_DISKS
-                                    else MOUNT_POINT.POLIBASE2
-                                ),
-                                A.CT.SPLITTER,
-                            )
-                        ),
-                        "/delete /y",
-                    )
-                )
-            )
-            os.system(
-                js(
-                    (
-                        "net use",
-                        j(
-                            (
+            for host in (MOUNT_POINT.NAS, MOUNT_POINT.POLIBASE2):
+                os.system(
+                    js(
+                        (
+                            "net use",
+                            j(
                                 (
-                                    PRECONNECTED_MOUNT_POINT.POLIBASE2
-                                    if USE_PRECONNECTED_DISKS
-                                    else MOUNT_POINT.POLIBASE2
-                                ),
-                                A.CT.SPLITTER,
-                            )
-                        ),
-                        "/delete /y",
+                                    host,
+                                    A.CT.SPLITTER,
+                                )
+                            ),
+                            "/delete /y",
+                        )
                     )
                 )
-            )
-
         # step 8
         os.system(js(("del", file_database_dump_name_out)))
         os.system(js(("del", file_out_name)))
```

### Comparing `pih-plb_db-0.20.5/PolibaseDatabaseService/const.py` & `pih-plb_db-0.21/PolibaseDatabaseService/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "PolibaseDatabase"
 
 HOST = A.CT_H.POLIBASE
 
-VERSION: str = "0.20.5"
+VERSION: str = "0.21"
 
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     host=HOST.NAME,
     description="Polibase database service",
     commands=("create_polibase_database_backup",),
     version=VERSION,
     use_standalone=True,
     standalone_name="plb_db",
-    host_changeable=True,
+    host_changeable=False,
     run_from_system_account=True,
     python_executable_path=CONST.UNKNOWN_VALUE,
 )
 
 TEST_NAME: str = "test"
 STUB_DIRECTORY_NAME: str = "stub"
 #
@@ -34,17 +34,11 @@
 USE_PRECONNECTED_DISKS: bool = True
 
 class MOUNT_POINT:
     POLIBASE: str = "C"
     NAS: str = "K"
     POLIBASE2: str = "L"
 
-
-class PRECONNECTED_MOUNT_POINT(MOUNT_POINT):
-    NAS: str = "N"
-    POLIBASE2: str = "T"
-
-
 class DATABASE_DUMP:
     FILE_NAME: str = "DatabaseDump"
     RESULT_FILE_NAME: str = "IN"
     FILE_EXTENSION: str = "DMP"
```

### Comparing `pih-plb_db-0.20.5/PolibaseDatabaseService/service.py` & `pih-plb_db-0.21/PolibaseDatabaseService/service.py`

 * *Files identical despite different names*

