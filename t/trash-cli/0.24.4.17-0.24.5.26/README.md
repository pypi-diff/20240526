# Comparing `tmp/trash_cli-0.24.4.17.tar.gz` & `tmp/trash_cli-0.24.5.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trash_cli-0.24.4.17.tar", last modified: Wed Apr 17 19:18:15 2024, max compression
+gzip compressed data, was "trash_cli-0.24.5.26.tar", last modified: Sun May 26 09:35:29 2024, max compression
```

## Comparing `trash_cli-0.24.4.17.tar` & `trash_cli-0.24.5.26.tar`

### file list

```diff
@@ -1,207 +1,194 @@
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.555893 trash_cli-0.24.4.17/
--rw-r--r--   0 andrea     (501) staff       (20)    17992 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/COPYING
--rw-r--r--   0 andrea     (501) staff       (20)     7916 2024-04-17 19:18:15.555816 trash_cli-0.24.4.17/PKG-INFO
--rw-r--r--   0 andrea     (501) staff       (20)     7349 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/README.rst
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.496624 trash_cli-0.24.4.17/man/
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.506238 trash_cli-0.24.4.17/man/man1/
--rw-r--r--   0 andrea     (501) staff       (20)     2765 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash-empty.1
--rw-r--r--   0 andrea     (501) staff       (20)     2386 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/man/man1/trash-list.1
--rw-r--r--   0 andrea     (501) staff       (20)     3216 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash-put.1
--rw-r--r--   0 andrea     (501) staff       (20)     2401 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash-restore.1
--rw-r--r--   0 andrea     (501) staff       (20)     1433 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/man/man1/trash-rm.1
--rw-r--r--   0 andrea     (501) staff       (20)     3216 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/man/man1/trash.1
--rw-r--r--   0 andrea     (501) staff       (20)       90 2022-10-04 20:03:09.000000 trash_cli-0.24.4.17/pyproject.toml
--rw-r--r--   0 andrea     (501) staff       (20)     1075 2024-04-17 19:18:15.556277 trash_cli-0.24.4.17/setup.cfg
--rw-r--r--   0 andrea     (501) staff       (20)       99 2023-05-04 13:06:54.000000 trash_cli-0.24.4.17/setup.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.514993 trash_cli-0.24.4.17/tests/
--rw-r--r--   0 andrea     (501) staff       (20)     1428 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_bump.py
--rw-r--r--   0 andrea     (501) staff       (20)     1779 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_candidate_shrink_user.py
--rw-r--r--   0 andrea     (501) staff       (20)     1363 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/tests/test_fake_file_system.py
--rw-r--r--   0 andrea     (501) staff       (20)      728 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_fake_fstab.py
--rw-r--r--   0 andrea     (501) staff       (20)     1255 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_fake_ismount.py
--rw-r--r--   0 andrea     (501) staff       (20)     1780 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_filesystem.py
--rw-r--r--   0 andrea     (501) staff       (20)     1126 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_generate_scripts.py
--rw-r--r--   0 andrea     (501) staff       (20)      426 2022-08-24 18:45:23.000000 trash_cli-0.24.4.17/tests/test_joining_paths.py
--rw-r--r--   0 andrea     (501) staff       (20)     1662 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_list_all_trashinfo_contents.py
--rw-r--r--   0 andrea     (501) staff       (20)     2056 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_make_script.py
--rw-r--r--   0 andrea     (501) staff       (20)      893 2022-09-22 13:29:20.000000 trash_cli-0.24.4.17/tests/test_mock_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      355 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_my_mock.py
--rw-r--r--   0 andrea     (501) staff       (20)     3760 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_parsing_trashinfo_contents.py
--rw-r--r--   0 andrea     (501) staff       (20)      958 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_partitions.py
--rw-r--r--   0 andrea     (501) staff       (20)      291 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/tests/test_tox_version_matches.py
--rw-r--r--   0 andrea     (501) staff       (20)      663 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_trash_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      856 2023-12-09 10:55:16.000000 trash_cli-0.24.4.17/tests/test_trash_put_reporter.py
--rw-r--r--   0 andrea     (501) staff       (20)      665 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/tests/test_volume_of.py
--rwxr-xr-x   0 andrea     (501) staff       (20)      132 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash
--rwxr-xr-x   0 andrea     (501) staff       (20)      134 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-empty
--rwxr-xr-x   0 andrea     (501) staff       (20)      133 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-list
--rwxr-xr-x   0 andrea     (501) staff       (20)      132 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-put
--rwxr-xr-x   0 andrea     (501) staff       (20)      136 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-restore
--rwxr-xr-x   0 andrea     (501) staff       (20)      131 2024-04-17 19:18:03.000000 trash_cli-0.24.4.17/trash-rm
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.555339 trash_cli-0.24.4.17/trash_cli.egg-info/
--rw-r--r--   0 andrea     (501) staff       (20)     7916 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrea     (501) staff       (20)     5575 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrea     (501) staff       (20)        1 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrea     (501) staff       (20)      117 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/requires.txt
--rw-r--r--   0 andrea     (501) staff       (20)        9 2024-04-17 19:18:15.000000 trash_cli-0.24.4.17/trash_cli.egg-info/top_level.txt
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.519984 trash_cli-0.24.4.17/trashcli/
--rw-r--r--   0 andrea     (501) staff       (20)       87 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      223 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/compat.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.525762 trash_cli-0.24.4.17/trashcli/empty/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2022-09-09 17:05:55.000000 trash_cli-0.24.4.17/trashcli/empty/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      642 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/clock.py
--rw-r--r--   0 andrea     (501) staff       (20)      655 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/console.py
--rw-r--r--   0 andrea     (501) staff       (20)      952 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/delete_according_date.py
--rw-r--r--   0 andrea     (501) staff       (20)      307 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/description.py
--rw-r--r--   0 andrea     (501) staff       (20)     2328 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/emptier.py
--rw-r--r--   0 andrea     (501) staff       (20)     2991 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/empty_action.py
--rw-r--r--   0 andrea     (501) staff       (20)     3298 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/empty_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)      306 2022-09-16 20:46:37.000000 trash_cli-0.24.4.17/trashcli/empty/errors.py
--rw-r--r--   0 andrea     (501) staff       (20)      143 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/existing_file_remover.py
--rw-r--r--   0 andrea     (501) staff       (20)      270 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/file_system_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)     1477 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/guard.py
--rw-r--r--   0 andrea     (501) staff       (20)       64 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/is_input_interactive.py
--rw-r--r--   0 andrea     (501) staff       (20)     1361 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/main.py
--rw-r--r--   0 andrea     (501) staff       (20)      179 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/older_than.py
--rw-r--r--   0 andrea     (501) staff       (20)       61 2022-09-06 20:19:17.000000 trash_cli-0.24.4.17/trashcli/empty/parse_reply.py
--rw-r--r--   0 andrea     (501) staff       (20)     3538 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/parser.py
--rw-r--r--   0 andrea     (501) staff       (20)      512 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/trashcli/empty/prepare_output_message.py
--rw-r--r--   0 andrea     (501) staff       (20)      618 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/print_time_action.py
--rw-r--r--   0 andrea     (501) staff       (20)      257 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/top_trash_dir_rules_file_system_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      490 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/empty/user.py
--rw-r--r--   0 andrea     (501) staff       (20)      514 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/file_system_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)     6321 2024-03-28 21:52:00.000000 trash_cli-0.24.4.17/trashcli/fs.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.526729 trash_cli-0.24.4.17/trashcli/fstab/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     1823 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/trashcli/fstab/mount_points_listing.py
--rw-r--r--   0 andrea     (501) staff       (20)     1171 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/volume_listing.py
--rw-r--r--   0 andrea     (501) staff       (20)      818 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/volume_of.py
--rw-r--r--   0 andrea     (501) staff       (20)     1920 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/fstab/volumes.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.530482 trash_cli-0.24.4.17/trashcli/lib/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      145 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/dir_checker.py
--rw-r--r--   0 andrea     (501) staff       (20)      328 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      126 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/enum_repr.py
--rw-r--r--   0 andrea     (501) staff       (20)      237 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/environ.py
--rw-r--r--   0 andrea     (501) staff       (20)      279 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/exit_codes.py
--rw-r--r--   0 andrea     (501) staff       (20)      207 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/logger.py
--rw-r--r--   0 andrea     (501) staff       (20)     1040 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/my_input.py
--rw-r--r--   0 andrea     (501) staff       (20)      227 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/my_permission_error.py
--rw-r--r--   0 andrea     (501) staff       (20)      281 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/path_of_backup_copy.py
--rw-r--r--   0 andrea     (501) staff       (20)      774 2024-03-28 21:52:13.000000 trash_cli-0.24.4.17/trashcli/lib/print_version.py
--rw-r--r--   0 andrea     (501) staff       (20)      919 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/trash_dir_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)      926 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/trash_dirs.py
--rw-r--r--   0 andrea     (501) staff       (20)      860 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/lib/user_info.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.531844 trash_cli-0.24.4.17/trashcli/list/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      691 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/extractors.py
--rw-r--r--   0 andrea     (501) staff       (20)      336 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/fs.py
--rw-r--r--   0 andrea     (501) staff       (20)     5915 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/list/list_trash_action.py
--rw-r--r--   0 andrea     (501) staff       (20)     3834 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/list/main.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.532701 trash_cli-0.24.4.17/trashcli/list/minor_actions/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      647 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/debug_volumes.py
--rw-r--r--   0 andrea     (501) staff       (20)     1344 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/list_trash_dirs.py
--rw-r--r--   0 andrea     (501) staff       (20)      482 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/list_volumes.py
--rw-r--r--   0 andrea     (501) staff       (20)      230 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/minor_actions/print_python_executable.py
--rw-r--r--   0 andrea     (501) staff       (20)     5083 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/list/parser.py
--rw-r--r--   0 andrea     (501) staff       (20)     2342 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/list/trash_dir_selector.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.534476 trash_cli-0.24.4.17/trashcli/parse_trashinfo/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      200 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/basket.py
--rw-r--r--   0 andrea     (501) staff       (20)      557 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/maybe_parse_deletion_date.py
--rw-r--r--   0 andrea     (501) staff       (20)      344 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_deletion_date.py
--rw-r--r--   0 andrea     (501) staff       (20)      239 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_original_location.py
--rw-r--r--   0 andrea     (501) staff       (20)      341 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_path.py
--rw-r--r--   0 andrea     (501) staff       (20)     1116 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_trashinfo.py
--rw-r--r--   0 andrea     (501) staff       (20)       76 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/parse_trashinfo/parser_error.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.541111 trash_cli-0.24.4.17/trashcli/put/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      324 2024-01-04 21:53:23.000000 trash_cli-0.24.4.17/trashcli/put/check_cast.py
--rw-r--r--   0 andrea     (501) staff       (20)      242 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/clock.py
--rw-r--r--   0 andrea     (501) staff       (20)      511 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/context.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.544371 trash_cli-0.24.4.17/trashcli/put/core/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     1139 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/candidate.py
--rw-r--r--   0 andrea     (501) staff       (20)      189 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/check_type.py
--rw-r--r--   0 andrea     (501) staff       (20)     1824 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/either.py
--rw-r--r--   0 andrea     (501) staff       (20)      715 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/failure_reason.py
--rw-r--r--   0 andrea     (501) staff       (20)      237 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/int_generator.py
--rw-r--r--   0 andrea     (501) staff       (20)     1434 2024-03-19 22:29:51.000000 trash_cli-0.24.4.17/trashcli/put/core/logs.py
--rw-r--r--   0 andrea     (501) staff       (20)      414 2023-12-16 16:38:07.000000 trash_cli-0.24.4.17/trashcli/put/core/mode.py
--rw-r--r--   0 andrea     (501) staff       (20)      123 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/path_maker_type.py
--rw-r--r--   0 andrea     (501) staff       (20)      217 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/trash_all_result.py
--rw-r--r--   0 andrea     (501) staff       (20)       97 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/core/trash_result.py
--rw-r--r--   0 andrea     (501) staff       (20)      267 2023-12-16 16:39:59.000000 trash_cli-0.24.4.17/trashcli/put/core/trashee.py
--rw-r--r--   0 andrea     (501) staff       (20)     1265 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/describer.py
--rw-r--r--   0 andrea     (501) staff       (20)      298 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/dir_maker.py
--rw-r--r--   0 andrea     (501) staff       (20)     3324 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/file_trasher.py
--rw-r--r--   0 andrea     (501) staff       (20)      665 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/format_trash_info.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.545410 trash_cli-0.24.4.17/trashcli/put/fs/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/fs/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     2112 2024-03-24 16:22:41.000000 trash_cli-0.24.4.17/trashcli/put/fs/fs.py
--rw-r--r--   0 andrea     (501) staff       (20)      275 2023-12-16 22:43:22.000000 trash_cli-0.24.4.17/trashcli/put/fs/parent_realpath.py
--rw-r--r--   0 andrea     (501) staff       (20)     2633 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/put/fs/real_fs.py
--rw-r--r--   0 andrea     (501) staff       (20)      675 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/fs/size_counter.py
--rw-r--r--   0 andrea     (501) staff       (20)      531 2023-12-16 22:43:22.000000 trash_cli-0.24.4.17/trashcli/put/fs/volume_of_parent.py
--rw-r--r--   0 andrea     (501) staff       (20)      197 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/gate.py
--rw-r--r--   0 andrea     (501) staff       (20)     3358 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.546785 trash_cli-0.24.4.17/trashcli/put/janitor_tools/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)     2108 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_creator.py
--rw-r--r--   0 andrea     (501) staff       (20)     2896 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_file_persister.py
--rw-r--r--   0 andrea     (501) staff       (20)     1534 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/put_trash_dir.py
--rw-r--r--   0 andrea     (501) staff       (20)     2545 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/security_check.py
--rw-r--r--   0 andrea     (501) staff       (20)     3073 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_checker.py
--rw-r--r--   0 andrea     (501) staff       (20)     1155 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_creator.py
--rw-r--r--   0 andrea     (501) staff       (20)     2137 2024-01-04 20:33:42.000000 trash_cli-0.24.4.17/trashcli/put/jobs.py
--rw-r--r--   0 andrea     (501) staff       (20)     3535 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/main.py
--rw-r--r--   0 andrea     (501) staff       (20)     1815 2023-12-09 21:05:26.000000 trash_cli-0.24.4.17/trashcli/put/my_logger.py
--rw-r--r--   0 andrea     (501) staff       (20)      282 2023-12-09 10:03:26.000000 trash_cli-0.24.4.17/trashcli/put/octal.py
--rw-r--r--   0 andrea     (501) staff       (20)     1305 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/original_location.py
--rw-r--r--   0 andrea     (501) staff       (20)     4803 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/parser.py
--rw-r--r--   0 andrea     (501) staff       (20)     6843 2024-01-04 21:54:10.000000 trash_cli-0.24.4.17/trashcli/put/reporter.py
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/same_volume_gate.py
--rw-r--r--   0 andrea     (501) staff       (20)      411 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/suffix.py
--rw-r--r--   0 andrea     (501) staff       (20)      838 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/trash_all.py
--rw-r--r--   0 andrea     (501) staff       (20)      514 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/trash_dir_volume_reader.py
--rw-r--r--   0 andrea     (501) staff       (20)     3214 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/trash_directories_finder.py
--rw-r--r--   0 andrea     (501) staff       (20)     1605 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/trash_put_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)     2325 2024-04-14 20:16:59.000000 trash_cli-0.24.4.17/trashcli/put/trasher.py
--rw-r--r--   0 andrea     (501) staff       (20)      775 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/put/user.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.552393 trash_cli-0.24.4.17/trashcli/restore/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      447 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/args.py
--rw-r--r--   0 andrea     (501) staff       (20)     2250 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/file_system.py
--rw-r--r--   0 andrea     (501) staff       (20)     2187 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/handler.py
--rw-r--r--   0 andrea     (501) staff       (20)      143 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/index.py
--rw-r--r--   0 andrea     (501) staff       (20)      970 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/info_dir_searcher.py
--rw-r--r--   0 andrea     (501) staff       (20)      688 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/info_files.py
--rw-r--r--   0 andrea     (501) staff       (20)     1377 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/main.py
--rw-r--r--   0 andrea     (501) staff       (20)      542 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/output.py
--rw-r--r--   0 andrea     (501) staff       (20)      271 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/restore/output_event.py
--rw-r--r--   0 andrea     (501) staff       (20)      847 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/output_recorder.py
--rw-r--r--   0 andrea     (501) staff       (20)      530 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/range.py
--rw-r--r--   0 andrea     (501) staff       (20)     1077 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/restore/real_output.py
--rw-r--r--   0 andrea     (501) staff       (20)     2595 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/restore_arg_parser.py
--rw-r--r--   0 andrea     (501) staff       (20)     5528 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/restore/restore_asking_the_user.py
--rw-r--r--   0 andrea     (501) staff       (20)     2385 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/restore_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)     1218 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/restorer.py
--rw-r--r--   0 andrea     (501) staff       (20)     1964 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/run_restore_action.py
--rw-r--r--   0 andrea     (501) staff       (20)      295 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/sequences.py
--rw-r--r--   0 andrea     (501) staff       (20)      102 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/single.py
--rw-r--r--   0 andrea     (501) staff       (20)     1526 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/sort_method.py
--rw-r--r--   0 andrea     (501) staff       (20)     2510 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/trash_directories.py
--rw-r--r--   0 andrea     (501) staff       (20)     1092 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/trashed_file.py
--rw-r--r--   0 andrea     (501) staff       (20)     3747 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/restore/trashed_files.py
-drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-04-17 19:18:15.555116 trash_cli-0.24.4.17/trashcli/rm/
--rw-r--r--   0 andrea     (501) staff       (20)        0 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/__init__.py
--rw-r--r--   0 andrea     (501) staff       (20)      584 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/cleanable_trashcan.py
--rw-r--r--   0 andrea     (501) staff       (20)      161 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/file_remover.py
--rw-r--r--   0 andrea     (501) staff       (20)      399 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/filter.py
--rw-r--r--   0 andrea     (501) staff       (20)     1612 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/list_trashinfo.py
--rw-r--r--   0 andrea     (501) staff       (20)      963 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/main.py
--rw-r--r--   0 andrea     (501) staff       (20)     3066 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/rm/rm_cmd.py
--rw-r--r--   0 andrea     (501) staff       (20)     1775 2024-03-28 21:52:14.000000 trash_cli-0.24.4.17/trashcli/shell_completion.py
--rw-r--r--   0 andrea     (501) staff       (20)       84 2024-04-17 18:48:54.000000 trash_cli-0.24.4.17/trashcli/trash.py
--rw-r--r--   0 andrea     (501) staff       (20)     4006 2023-12-09 09:53:40.000000 trash_cli-0.24.4.17/trashcli/trash_dirs_scanner.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.695224 trash_cli-0.24.5.26/
+-rw-r--r--   0 andrea     (501) staff       (20)    17992 2022-08-24 18:45:23.000000 trash_cli-0.24.5.26/COPYING
+-rw-r--r--   0 andrea     (501) staff       (20)     7910 2024-05-26 09:35:29.695147 trash_cli-0.24.5.26/PKG-INFO
+-rw-r--r--   0 andrea     (501) staff       (20)     7343 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/README.rst
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.639573 trash_cli-0.24.5.26/man/
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.645240 trash_cli-0.24.5.26/man/man1/
+-rw-r--r--   0 andrea     (501) staff       (20)     2765 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/man/man1/trash-empty.1
+-rw-r--r--   0 andrea     (501) staff       (20)     2386 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/man/man1/trash-list.1
+-rw-r--r--   0 andrea     (501) staff       (20)     3216 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/man/man1/trash-put.1
+-rw-r--r--   0 andrea     (501) staff       (20)     2401 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/man/man1/trash-restore.1
+-rw-r--r--   0 andrea     (501) staff       (20)     1433 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/man/man1/trash-rm.1
+-rw-r--r--   0 andrea     (501) staff       (20)     3216 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/man/man1/trash.1
+-rw-r--r--   0 andrea     (501) staff       (20)       90 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/pyproject.toml
+-rw-r--r--   0 andrea     (501) staff       (20)     1099 2024-05-26 09:35:29.695596 trash_cli-0.24.5.26/setup.cfg
+-rw-r--r--   0 andrea     (501) staff       (20)       99 2024-05-19 20:31:56.000000 trash_cli-0.24.5.26/setup.py
+-rwxr-xr-x   0 andrea     (501) staff       (20)      132 2024-05-26 09:32:09.000000 trash_cli-0.24.5.26/trash
+-rwxr-xr-x   0 andrea     (501) staff       (20)      134 2024-05-26 09:32:10.000000 trash_cli-0.24.5.26/trash-empty
+-rwxr-xr-x   0 andrea     (501) staff       (20)      133 2024-05-26 09:32:10.000000 trash_cli-0.24.5.26/trash-list
+-rwxr-xr-x   0 andrea     (501) staff       (20)      132 2024-05-26 09:32:09.000000 trash_cli-0.24.5.26/trash-put
+-rwxr-xr-x   0 andrea     (501) staff       (20)      136 2024-05-26 09:32:10.000000 trash_cli-0.24.5.26/trash-restore
+-rwxr-xr-x   0 andrea     (501) staff       (20)      131 2024-05-26 09:32:10.000000 trash_cli-0.24.5.26/trash-rm
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.694575 trash_cli-0.24.5.26/trash_cli.egg-info/
+-rw-r--r--   0 andrea     (501) staff       (20)     7910 2024-05-26 09:35:29.000000 trash_cli-0.24.5.26/trash_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrea     (501) staff       (20)     5254 2024-05-26 09:35:29.000000 trash_cli-0.24.5.26/trash_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrea     (501) staff       (20)        1 2024-05-26 09:35:29.000000 trash_cli-0.24.5.26/trash_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrea     (501) staff       (20)      117 2024-05-26 09:35:29.000000 trash_cli-0.24.5.26/trash_cli.egg-info/requires.txt
+-rw-r--r--   0 andrea     (501) staff       (20)        9 2024-05-26 09:35:29.000000 trash_cli-0.24.5.26/trash_cli.egg-info/top_level.txt
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.650018 trash_cli-0.24.5.26/trashcli/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      223 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/compat.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.659169 trash_cli-0.24.5.26/trashcli/empty/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      642 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/clock.py
+-rw-r--r--   0 andrea     (501) staff       (20)      655 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/console.py
+-rw-r--r--   0 andrea     (501) staff       (20)      952 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/delete_according_date.py
+-rw-r--r--   0 andrea     (501) staff       (20)      307 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/description.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2328 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/emptier.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2991 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/empty_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3298 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/empty_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)      306 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/errors.py
+-rw-r--r--   0 andrea     (501) staff       (20)      143 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/existing_file_remover.py
+-rw-r--r--   0 andrea     (501) staff       (20)      270 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/file_system_dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1477 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/guard.py
+-rw-r--r--   0 andrea     (501) staff       (20)       64 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/is_input_interactive.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1366 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/empty/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)      179 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/older_than.py
+-rw-r--r--   0 andrea     (501) staff       (20)       61 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/parse_reply.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3538 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)      512 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/empty/prepare_output_message.py
+-rw-r--r--   0 andrea     (501) staff       (20)      618 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/print_time_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)      257 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/top_trash_dir_rules_file_system_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      490 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/empty/user.py
+-rw-r--r--   0 andrea     (501) staff       (20)      514 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/file_system_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     6321 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/fs.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.660477 trash_cli-0.24.5.26/trashcli/fstab/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/fstab/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1823 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/fstab/mount_points_listing.py
+-rw-r--r--   0 andrea     (501) staff       (20)      360 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/fstab/real_volume_of.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1361 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/fstab/volume_listing.py
+-rw-r--r--   0 andrea     (501) staff       (20)      184 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/fstab/volume_of.py
+-rw-r--r--   0 andrea     (501) staff       (20)      431 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/fstab/volume_of_impl.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1961 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/fstab/volumes.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.664443 trash_cli-0.24.5.26/trashcli/lib/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      145 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/dir_checker.py
+-rw-r--r--   0 andrea     (501) staff       (20)      328 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      126 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/enum_repr.py
+-rw-r--r--   0 andrea     (501) staff       (20)      237 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/environ.py
+-rw-r--r--   0 andrea     (501) staff       (20)      279 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/exit_codes.py
+-rw-r--r--   0 andrea     (501) staff       (20)      207 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/logger.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1040 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/my_input.py
+-rw-r--r--   0 andrea     (501) staff       (20)      227 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/my_permission_error.py
+-rw-r--r--   0 andrea     (501) staff       (20)      281 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/path_of_backup_copy.py
+-rw-r--r--   0 andrea     (501) staff       (20)      774 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/lib/print_version.py
+-rw-r--r--   0 andrea     (501) staff       (20)      919 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/trash_dir_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)      926 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/trash_dirs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      860 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/lib/user_info.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.665721 trash_cli-0.24.5.26/trashcli/list/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      691 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/extractors.py
+-rw-r--r--   0 andrea     (501) staff       (20)      336 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/fs.py
+-rw-r--r--   0 andrea     (501) staff       (20)     5915 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/list_trash_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3839 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/list/main.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.668151 trash_cli-0.24.5.26/trashcli/list/minor_actions/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/minor_actions/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      647 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/list/minor_actions/debug_volumes.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1344 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/minor_actions/list_trash_dirs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      482 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/list/minor_actions/list_volumes.py
+-rw-r--r--   0 andrea     (501) staff       (20)      230 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/minor_actions/print_python_executable.py
+-rw-r--r--   0 andrea     (501) staff       (20)     5083 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2342 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/list/trash_dir_selector.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.669686 trash_cli-0.24.5.26/trashcli/parse_trashinfo/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      200 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/basket.py
+-rw-r--r--   0 andrea     (501) staff       (20)      557 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/maybe_parse_deletion_date.py
+-rw-r--r--   0 andrea     (501) staff       (20)      344 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/parse_deletion_date.py
+-rw-r--r--   0 andrea     (501) staff       (20)      239 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/parse_original_location.py
+-rw-r--r--   0 andrea     (501) staff       (20)      341 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/parse_path.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1116 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/parse_trashinfo.py
+-rw-r--r--   0 andrea     (501) staff       (20)       76 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/parse_trashinfo/parser_error.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.675196 trash_cli-0.24.5.26/trashcli/put/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      324 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/check_cast.py
+-rw-r--r--   0 andrea     (501) staff       (20)      242 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/clock.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1219 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/context.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.678772 trash_cli-0.24.5.26/trashcli/put/core/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1139 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/candidate.py
+-rw-r--r--   0 andrea     (501) staff       (20)      189 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/check_type.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1824 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/either.py
+-rw-r--r--   0 andrea     (501) staff       (20)      715 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/failure_reason.py
+-rw-r--r--   0 andrea     (501) staff       (20)      237 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/int_generator.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1628 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/core/logs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      414 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/core/mode.py
+-rw-r--r--   0 andrea     (501) staff       (20)      123 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/path_maker_type.py
+-rw-r--r--   0 andrea     (501) staff       (20)      217 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/trash_all_result.py
+-rw-r--r--   0 andrea     (501) staff       (20)       97 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/core/trash_result.py
+-rw-r--r--   0 andrea     (501) staff       (20)      267 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/core/trashee.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1221 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/describer.py
+-rw-r--r--   0 andrea     (501) staff       (20)      298 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/dir_maker.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3073 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/file_trasher.py
+-rw-r--r--   0 andrea     (501) staff       (20)      665 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/format_trash_info.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.679869 trash_cli-0.24.5.26/trashcli/put/fs/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/fs/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2290 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/fs/fs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      275 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/fs/parent_realpath.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2914 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/fs/real_fs.py
+-rw-r--r--   0 andrea     (501) staff       (20)      675 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/fs/size_counter.py
+-rw-r--r--   0 andrea     (501) staff       (20)      397 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/fs/volume_of_parent.py
+-rw-r--r--   0 andrea     (501) staff       (20)      197 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/gate.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3514 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/janitor.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.681090 trash_cli-0.24.5.26/trashcli/put/janitor_tools/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2058 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/info_creator.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2896 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/info_file_persister.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1534 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/put_trash_dir.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2545 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/security_check.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3039 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/trash_dir_checker.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1198 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/janitor_tools/trash_dir_creator.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2190 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/jobs.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1884 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1812 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/my_logger.py
+-rw-r--r--   0 andrea     (501) staff       (20)      282 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/octal.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1305 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/original_location.py
+-rw-r--r--   0 andrea     (501) staff       (20)     4803 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/parser.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.682958 trash_cli-0.24.5.26/trashcli/put/reporting/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/reporting/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1634 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/reporting/stats_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3742 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/reporting/trash_put_reporter.py
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/same_volume_gate.py
+-rw-r--r--   0 andrea     (501) staff       (20)      411 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/put/suffix.py
+-rw-r--r--   0 andrea     (501) staff       (20)      388 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/trash_dir_volume_reader.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3078 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/trash_directories_finder.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1676 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/trash_put_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2601 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/trasher.py
+-rw-r--r--   0 andrea     (501) staff       (20)      776 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/put/user.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.693176 trash_cli-0.24.5.26/trashcli/restore/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      447 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/args.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2250 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/file_system.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2187 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/handler.py
+-rw-r--r--   0 andrea     (501) staff       (20)      143 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/index.py
+-rw-r--r--   0 andrea     (501) staff       (20)      970 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/info_dir_searcher.py
+-rw-r--r--   0 andrea     (501) staff       (20)      688 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/info_files.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1447 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)      542 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/output.py
+-rw-r--r--   0 andrea     (501) staff       (20)      271 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/output_event.py
+-rw-r--r--   0 andrea     (501) staff       (20)      847 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/output_recorder.py
+-rw-r--r--   0 andrea     (501) staff       (20)      530 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/range.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1077 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/real_output.py
+-rw-r--r--   0 andrea     (501) staff       (20)      313 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/real_restore_logger.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2595 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/restore_arg_parser.py
+-rw-r--r--   0 andrea     (501) staff       (20)     5528 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/restore_asking_the_user.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2385 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/restore_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)      136 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/restore_logger.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1218 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/restorer.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1964 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/run_restore_action.py
+-rw-r--r--   0 andrea     (501) staff       (20)      295 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/sequences.py
+-rw-r--r--   0 andrea     (501) staff       (20)      102 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/single.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1526 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/sort_method.py
+-rw-r--r--   0 andrea     (501) staff       (20)     2510 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/trash_directories.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1092 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/restore/trashed_file.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3841 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/restore/trashed_files.py
+drwxr-xr-x   0 andrea     (501) staff       (20)        0 2024-05-26 09:35:29.694368 trash_cli-0.24.5.26/trashcli/rm/
+-rw-r--r--   0 andrea     (501) staff       (20)        0 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/__init__.py
+-rw-r--r--   0 andrea     (501) staff       (20)      584 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/cleanable_trashcan.py
+-rw-r--r--   0 andrea     (501) staff       (20)      161 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/file_remover.py
+-rw-r--r--   0 andrea     (501) staff       (20)      399 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/filter.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1612 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/list_trashinfo.py
+-rw-r--r--   0 andrea     (501) staff       (20)      963 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/main.py
+-rw-r--r--   0 andrea     (501) staff       (20)     3066 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/rm/rm_cmd.py
+-rw-r--r--   0 andrea     (501) staff       (20)     1775 2024-05-26 09:29:27.000000 trash_cli-0.24.5.26/trashcli/shell_completion.py
+-rw-r--r--   0 andrea     (501) staff       (20)       84 2024-05-26 09:29:45.000000 trash_cli-0.24.5.26/trashcli/trash.py
+-rw-r--r--   0 andrea     (501) staff       (20)     4006 2024-05-15 19:35:09.000000 trash_cli-0.24.5.26/trashcli/trash_dirs_scanner.py
```

### Comparing `trash_cli-0.24.4.17/COPYING` & `trash_cli-0.24.5.26/COPYING`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/PKG-INFO` & `trash_cli-0.24.5.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trash-cli
-Version: 0.24.4.17
+Version: 0.24.5.26
 Summary: Command line interface to FreeDesktop.org Trash.
 Home-page: https://github.com/andreafrancia/trash-cli
 Author: Andrea Francia
 Author-email: andrea@andreafrancia.it
 License: GPL v2
 Description-Content-Type: text/x-rst
 License-File: COPYING
@@ -249,15 +249,15 @@
 or::
 
     pip install 'trash-cli[completion]'
 
 Then::
 
     cmds=(trash-empty trash-list trash-restore trash-put trash)
-    for cmd in $cmds; do
+    for cmd in ${cmds[@]}; do
       $cmd --print-completion bash | sudo tee /usr/share/bash-completion/completions/$cmd
       $cmd --print-completion zsh | sudo tee /usr/share/zsh/site-functions/_$cmd
       $cmd --print-completion tcsh | sudo tee /etc/profile.d/$cmd.completion.csh
     done
 
 Bugs
 ----
@@ -272,16 +272,16 @@
 You can send me an email using andrea@andreafrancia.it.
 
 Development
 -----------
 
 Environment setup::
 
-    virtualenv env --no-site-packages
-    source env/bin/activate
+    python -m venv .venv
+    source .venv/bin/activate
     pip install -r requirements-dev.txt -r requirements.txt
 
 Running tests::
 
     pytest -m 'not slow'        # run only fast tests
     pytest -m 'slow'            # run slow tests
     pytest                      # run all tests
```

### Comparing `trash_cli-0.24.4.17/README.rst` & `trash_cli-0.24.5.26/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 or::
 
     pip install 'trash-cli[completion]'
 
 Then::
 
     cmds=(trash-empty trash-list trash-restore trash-put trash)
-    for cmd in $cmds; do
+    for cmd in ${cmds[@]}; do
       $cmd --print-completion bash | sudo tee /usr/share/bash-completion/completions/$cmd
       $cmd --print-completion zsh | sudo tee /usr/share/zsh/site-functions/_$cmd
       $cmd --print-completion tcsh | sudo tee /etc/profile.d/$cmd.completion.csh
     done
 
 Bugs
 ----
@@ -254,16 +254,16 @@
 You can send me an email using andrea@andreafrancia.it.
 
 Development
 -----------
 
 Environment setup::
 
-    virtualenv env --no-site-packages
-    source env/bin/activate
+    python -m venv .venv
+    source .venv/bin/activate
     pip install -r requirements-dev.txt -r requirements.txt
 
 Running tests::
 
     pytest -m 'not slow'        # run only fast tests
     pytest -m 'slow'            # run slow tests
     pytest                      # run all tests
```

### Comparing `trash_cli-0.24.4.17/man/man1/trash-empty.1` & `trash_cli-0.24.5.26/man/man1/trash-empty.1`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/man/man1/trash-list.1` & `trash_cli-0.24.5.26/man/man1/trash-list.1`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/man/man1/trash-put.1` & `trash_cli-0.24.5.26/man/man1/trash-put.1`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/man/man1/trash-restore.1` & `trash_cli-0.24.5.26/man/man1/trash-restore.1`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/man/man1/trash-rm.1` & `trash_cli-0.24.5.26/man/man1/trash-rm.1`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/man/man1/trash.1` & `trash_cli-0.24.5.26/man/man1/trash.1`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/setup.cfg` & `trash_cli-0.24.5.26/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 	trashcli
 	trashcli.empty
 	trashcli.lib
 	trashcli.list
 	trashcli.list.minor_actions
 	trashcli.put
 	trashcli.put.core
-	trashcli.put.janitor_tools
 	trashcli.put.fs
+	trashcli.put.janitor_tools
+	trashcli.put.reporting
 	trashcli.restore
 	trashcli.rm
 	trashcli.fstab
 	trashcli.parse_trashinfo
 scripts = 
 	trash
 	trash-put
```

### Comparing `trash_cli-0.24.4.17/trash_cli.egg-info/PKG-INFO` & `trash_cli-0.24.5.26/trash_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trash-cli
-Version: 0.24.4.17
+Version: 0.24.5.26
 Summary: Command line interface to FreeDesktop.org Trash.
 Home-page: https://github.com/andreafrancia/trash-cli
 Author: Andrea Francia
 Author-email: andrea@andreafrancia.it
 License: GPL v2
 Description-Content-Type: text/x-rst
 License-File: COPYING
@@ -249,15 +249,15 @@
 or::
 
     pip install 'trash-cli[completion]'
 
 Then::
 
     cmds=(trash-empty trash-list trash-restore trash-put trash)
-    for cmd in $cmds; do
+    for cmd in ${cmds[@]}; do
       $cmd --print-completion bash | sudo tee /usr/share/bash-completion/completions/$cmd
       $cmd --print-completion zsh | sudo tee /usr/share/zsh/site-functions/_$cmd
       $cmd --print-completion tcsh | sudo tee /etc/profile.d/$cmd.completion.csh
     done
 
 Bugs
 ----
@@ -272,16 +272,16 @@
 You can send me an email using andrea@andreafrancia.it.
 
 Development
 -----------
 
 Environment setup::
 
-    virtualenv env --no-site-packages
-    source env/bin/activate
+    python -m venv .venv
+    source .venv/bin/activate
     pip install -r requirements-dev.txt -r requirements.txt
 
 Running tests::
 
     pytest -m 'not slow'        # run only fast tests
     pytest -m 'slow'            # run slow tests
     pytest                      # run all tests
```

### Comparing `trash_cli-0.24.4.17/trashcli/empty/clock.py` & `trash_cli-0.24.5.26/trashcli/empty/clock.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/console.py` & `trash_cli-0.24.5.26/trashcli/empty/console.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/delete_according_date.py` & `trash_cli-0.24.5.26/trashcli/empty/delete_according_date.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/emptier.py` & `trash_cli-0.24.5.26/trashcli/empty/emptier.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/empty_action.py` & `trash_cli-0.24.5.26/trashcli/empty/empty_action.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/empty_cmd.py` & `trash_cli-0.24.5.26/trashcli/empty/empty_cmd.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/guard.py` & `trash_cli-0.24.5.26/trashcli/empty/guard.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/main.py` & `trash_cli-0.24.5.26/trashcli/empty/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from trashcli.empty.empty_cmd import EmptyCmd
 from trashcli.fs import RealContentsOf, ContentsOf
 from .existing_file_remover import ExistingFileRemover
 from .file_system_dir_reader import FileSystemDirReader
 from .top_trash_dir_rules_file_system_reader import \
     RealTopTrashDirRulesReader
 from ..fstab.volume_listing import RealVolumesListing
-from ..fstab.volume_of import RealVolumeOf
+from ..fstab.real_volume_of import RealVolumeOf
 
 
 class ContentReader(ContentsOf, Protocol):
     pass
 
 
 def main():
```

### Comparing `trash_cli-0.24.4.17/trashcli/empty/parser.py` & `trash_cli-0.24.5.26/trashcli/empty/parser.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/prepare_output_message.py` & `trash_cli-0.24.5.26/trashcli/empty/prepare_output_message.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/empty/print_time_action.py` & `trash_cli-0.24.5.26/trashcli/empty/print_time_action.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/file_system_reader.py` & `trash_cli-0.24.5.26/trashcli/file_system_reader.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/fs.py` & `trash_cli-0.24.5.26/trashcli/fs.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/fstab/mount_points_listing.py` & `trash_cli-0.24.5.26/trashcli/fstab/mount_points_listing.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/fstab/volume_listing.py` & `trash_cli-0.24.5.26/trashcli/fstab/volume_listing.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,30 @@
 from trashcli.fstab.mount_points_listing import MountPointsListing, \
     RealMountPointsListing
 
 
 @six.add_metaclass(ABCMeta)
 class VolumesListing:
     @abstractmethod
-    def list_volumes(self, environ): # type (dict) -> Iterable[str]
+    def list_volumes(self, environ):  # type (dict) -> Iterable[str]
         raise NotImplementedError()
 
 
+class FixedVolumesListing(VolumesListing):
+    def __init__(self, volumes):
+        self.volumes = volumes
+
+    def list_volumes(self, _environ):
+        return self.volumes
+
+
 class RealVolumesListing(VolumesListing):
     def list_volumes(self, environ):
-        return VolumesListingImpl(RealMountPointsListing()).list_volumes(environ)
+        return VolumesListingImpl(RealMountPointsListing()).list_volumes(
+            environ)
 
 
 class VolumesListingImpl:
     def __init__(self,
                  mount_points_listing,  # type: MountPointsListing
                  ):
         self.mount_points_listing = mount_points_listing
```

### Comparing `trash_cli-0.24.4.17/trashcli/fstab/volumes.py` & `trash_cli-0.24.5.26/trashcli/fstab/volumes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABCMeta
 
 import six
 import os
 from trashcli.fstab.mount_points_listing import MountPointsListing, \
     RealMountPointsListing
-from trashcli.fstab.volume_of import VolumeOf, RealVolumeOf
+from trashcli.fstab.volume_of import VolumeOf
+from trashcli.fstab.real_volume_of import RealVolumeOf
 
 
 @six.add_metaclass(ABCMeta)
 class Volumes(VolumeOf, MountPointsListing):
     pass
```

### Comparing `trash_cli-0.24.4.17/trashcli/lib/my_input.py` & `trash_cli-0.24.5.26/trashcli/lib/my_input.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/lib/print_version.py` & `trash_cli-0.24.5.26/trashcli/lib/print_version.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/lib/trash_dir_reader.py` & `trash_cli-0.24.5.26/trashcli/lib/trash_dir_reader.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/lib/trash_dirs.py` & `trash_cli-0.24.5.26/trashcli/lib/trash_dirs.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/lib/user_info.py` & `trash_cli-0.24.5.26/trashcli/lib/user_info.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/list/extractors.py` & `trash_cli-0.24.5.26/trashcli/list/extractors.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/list/list_trash_action.py` & `trash_cli-0.24.5.26/trashcli/list/list_trash_action.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/list/main.py` & `trash_cli-0.24.5.26/trashcli/list/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 import trashcli.trash
 from trashcli.empty.main import ContentReader
 from trashcli.file_system_reader import FileSystemReader
 from trashcli.fs import RealContentsOf
 from trashcli.fstab.volume_listing import RealVolumesListing
-from trashcli.fstab.volume_of import RealVolumeOf
+from trashcli.fstab.real_volume_of import RealVolumeOf
 from trashcli.fstab.volume_of import VolumeOf
 from trashcli.lib.dir_reader import DirReader, RealDirReader
 from trashcli.lib.print_version import PrintVersionArgs, \
     PrintVersionAction
 from trashcli.list.list_trash_action import ListTrashAction, ListTrashArgs
 from trashcli.list.minor_actions.debug_volumes import DebugVolumes, \
     DebugVolumesArgs
```

### Comparing `trash_cli-0.24.4.17/trashcli/list/minor_actions/debug_volumes.py` & `trash_cli-0.24.5.26/trashcli/list/minor_actions/debug_volumes.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/list/minor_actions/list_trash_dirs.py` & `trash_cli-0.24.5.26/trashcli/list/minor_actions/list_trash_dirs.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/list/parser.py` & `trash_cli-0.24.5.26/trashcli/list/parser.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/list/trash_dir_selector.py` & `trash_cli-0.24.5.26/trashcli/list/trash_dir_selector.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/parse_trashinfo/maybe_parse_deletion_date.py` & `trash_cli-0.24.5.26/trashcli/parse_trashinfo/maybe_parse_deletion_date.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/parse_trashinfo/parse_trashinfo.py` & `trash_cli-0.24.5.26/trashcli/parse_trashinfo/parse_trashinfo.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/core/candidate.py` & `trash_cli-0.24.5.26/trashcli/put/core/candidate.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/core/either.py` & `trash_cli-0.24.5.26/trashcli/put/core/either.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/core/failure_reason.py` & `trash_cli-0.24.5.26/trashcli/put/core/failure_reason.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/core/logs.py` & `trash_cli-0.24.5.26/trashcli/put/core/logs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import abstractmethod
 from enum import Enum
+from typing import List
 from typing import NamedTuple
 from trashcli.compat import Protocol
 
 
 class Level(Enum):
     INFO = "INFO"
     DEBUG = "DEBUG"
@@ -26,37 +27,44 @@
     @abstractmethod
     def resolve(self):
         raise NotImplementedError
 
 
 class LogEntry(NamedTuple('LogEntry', [
     ('level', Level),
-    ('message', Message),
-    ('tag', LogTag)
+    ('tag', LogTag),
+    ('messages', List[Message]),
 ])):
-    def resolve_message(self):
-        return self.message.resolve()
+    def resolve_messages(self):
+        for m in self.messages:
+            yield m.resolve()
 
 
 class MessageStr(NamedTuple('Message', [
     ('message', str),
 ]), Message):
     def resolve(self):
         return self.message
 
+    @staticmethod
+    def from_messages(messages  # type: List[str]
+                      ):
+        return [MessageStr(msg) for msg in messages]
+
 
 def log_str(level,  # type: Level
             tag,  # type: LogTag
-            message,  # type: str
+            messages,  # type: List[str]
             ):
-    return LogEntry(level, MessageStr(message), tag)
+    return LogEntry(level, tag, MessageStr.from_messages(messages))
+
 
 def warning_str(message):  # type: (str) -> LogEntry
-    return LogEntry(Level.WARNING, MessageStr(message), LogTag.unspecified)
+    return log_str(Level.WARNING, LogTag.unspecified, [message])
 
 
 def info_str(message):  # type: (str) -> LogEntry
-    return LogEntry(Level.INFO, MessageStr(message), LogTag.unspecified)
+    return log_str(Level.INFO, LogTag.unspecified, [message])
 
 
 def debug_str(message):  # type: (str) -> LogEntry
-    return LogEntry(Level.DEBUG, MessageStr(message), LogTag.unspecified)
+    return log_str(Level.DEBUG, LogTag.unspecified, [message])
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/describer.py` & `trash_cli-0.24.5.26/trashcli/put/describer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
 
-from trashcli.put.fs.real_fs import RealFs
-
 
 class Describer:
     def __init__(self, fs):
         self.fs = fs
 
     def describe(self, path):
         """
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/file_trasher.py` & `trash_cli-0.24.5.26/trashcli/rm/rm_cmd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-# Copyright (C) 2007-2023 Andrea Francia Trivolzio(PV) Italy
+# Copyright (C) 2011-2021 Andrea Francia Bereguardo(PV) Italy
+from trashcli.compat import Protocol
 
-from trashcli.fstab.volume_of import VolumeOf
-from trashcli.lib.environ import Environ
-from trashcli.put.context import Context
-from trashcli.put.core.trash_result import TrashResult
-from trashcli.put.core.trashee import Trashee
-from trashcli.put.fs.parent_realpath import ParentRealpathFs
-from trashcli.put.fs.volume_of_parent import VolumeOfParent
-from trashcli.put.janitor import Janitor
-from trashcli.put.my_logger import LogData
-from trashcli.put.my_logger import MyLogger
-from trashcli.put.reporter import TrashPutReporter
-from trashcli.put.trash_directories_finder import TrashDirectoriesFinder
+from trashcli.fs import ContentsOf
+from trashcli.lib.dir_checker import DirChecker
+from trashcli.lib.dir_reader import DirReader
+from trashcli.lib.user_info import SingleUserInfoProvider
+from trashcli.rm.cleanable_trashcan import CleanableTrashcan
+from trashcli.rm.file_remover import FileRemover
+from trashcli.rm.filter import Filter
+from trashcli.rm.list_trashinfo import ListTrashinfos
+from trashcli.trash_dirs_scanner import TrashDirsScanner, TopTrashDirRules, \
+    trash_dir_found
+
+
+class RmFileSystemReader(ContentsOf,
+                         DirReader,
+                         TopTrashDirRules.Reader,
+                         Protocol):
+    pass
 
 
-class FileTrasher:
-
+class RmCmd:
     def __init__(self,
-                 volumes,  # type: VolumeOf
-                 trash_directories_finder,  # type: TrashDirectoriesFinder
-                 parent_realpath_fs,  # type: ParentRealpathFs
-                 logger,  # type: MyLogger
-                 reporter,  # type: TrashPutReporter
-                 janitor,  # type: Janitor
-                 volume_of_parent,  # type: VolumeOfParent
-                 ):  # type: (...) -> None
-        self.volumes = volumes
-        self.trash_directories_finder = trash_directories_finder
-        self.parent_realpath_fs = parent_realpath_fs
-        self.logger = logger
-        self.reporter = reporter
-        self.janitor = janitor
-        self.volume_of_parent = volume_of_parent or volume_of_parent
-
-    def trash_file(self,
-                   path,  # type: str
-                   context,  # type: Context
-                   ):
-        volume = self._figure_out_volume(path, context.forced_volume)
-        trashee = Trashee(path, volume)
-        candidates = self._select_candidates(volume, context.user_trash_dir,
-                                             context.environ,
-                                             context.uid, context.home_fallback)
-        failures = []
-        for candidate in candidates:
-            self.reporter.trash_dir_with_volume(candidate, context.log_data)
-            trashing = self.janitor.trash_file_in(
-                candidate, context.log_data, context.environ, trashee)
-            if trashing.succeeded():
-                self.reporter.file_has_been_trashed_in_as(path,
-                                                          candidate,
-                                                          context.log_data,
-                                                          context.environ)
-                return TrashResult.Success
-            else:
-                failures.append((candidate, trashing.reason))
-        self.reporter.unable_to_trash_file2(trashee, context.log_data, failures,
-                                            context.environ)
-        return TrashResult.Failure
-
-    def _figure_out_volume(self, path, default_volume):
-        if default_volume:
-            return default_volume
-        else:
-            return self.volume_of_parent.volume_of_parent(path)
-
-    def _select_candidates(self, volume, user_trash_dir, environ, uid,
-                           home_fallback):
-        return self.trash_directories_finder. \
-            possible_trash_directories_for(volume,
-                                           user_trash_dir, environ, uid,
-                                           home_fallback)
+                 environ,
+                 getuid,
+                 volumes_listing,
+                 stderr,
+                 file_reader,  # type: RmFileSystemReader
+                 ):
+        self.environ = environ
+        self.getuid = getuid
+        self.volumes_listing = volumes_listing
+        self.stderr = stderr
+        self.file_reader = file_reader
+
+    def run(self, argv, uid):
+        args = argv[1:]
+        self.exit_code = 0
+
+        if not args:
+            self.print_err('Usage:\n'
+                           '    trash-rm PATTERN\n'
+                           '\n'
+                           'Please specify PATTERN.\n'
+                           'trash-rm uses fnmatch.fnmatchcase to match patterns, see https://docs.python.org/3/library/fnmatch.html for more details.')
+            self.exit_code = 8
+            return
+
+        trashcan = CleanableTrashcan(FileRemover())
+        cmd = Filter(args[0])
+
+        listing = ListTrashinfos.make(self.file_reader, self.file_reader)
+
+        user_info_provider = SingleUserInfoProvider()
+        scanner = TrashDirsScanner(user_info_provider,
+                                   self.volumes_listing,
+                                   TopTrashDirRules(self.file_reader),
+                                   DirChecker())
+
+        for event, args in scanner.scan_trash_dirs(self.environ, uid):
+            if event == trash_dir_found:
+                path, volume = args
+                for type, arg in listing.list_from_volume_trashdir(path,
+                                                                   volume):
+                    if type == 'unable_to_parse_path':
+                        self.unable_to_parse_path(arg)
+                    elif type == 'trashed_file':
+                        original_location, info_file = arg
+                        if cmd.matches(original_location):
+                            trashcan.delete_trash_info_and_backup_copy(
+                                info_file)
+
+    def unable_to_parse_path(self, trashinfo):
+        self.report_error('{}: unable to parse \'Path\''.format(trashinfo))
+
+    def report_error(self, error_msg):
+        self.print_err('trash-rm: {}'.format(error_msg))
+
+    def print_err(self, msg):
+        self.stderr.write(msg + '\n')
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/format_trash_info.py` & `trash_cli-0.24.5.26/trashcli/put/format_trash_info.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/fs/fs.py` & `trash_cli-0.24.5.26/trashcli/put/fs/fs.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,14 +57,22 @@
         raise NotImplementedError
 
     @abstractmethod
     def is_accessible(self, path):
         raise NotImplementedError
 
     @abstractmethod
+    def read(self, path):
+        raise NotImplementedError
+
+    @abstractmethod
+    def write_file(self, path, content):
+        raise NotImplementedError
+
+    @abstractmethod
     def make_file(self, path, content):
         raise NotImplementedError
 
     @abstractmethod
     def get_mod(self, path):
         raise NotImplementedError
 
@@ -80,14 +88,15 @@
         parent = os.path.dirname(path)
         return self.realpath(parent)
 
     def list_sorted(self, path):
         return sorted(self.listdir(path))
 
 
+
 def list_all(fs, path):  # type: (Fs, str) -> Iterable[str]
     result = fs.walk_no_follow(path)
     for top, dirs, non_dirs in result:
         for d in dirs:
             yield os.path.join(top, d)
         for f in non_dirs:
             yield os.path.join(top, f)
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/fs/real_fs.py` & `trash_cli-0.24.5.26/trashcli/put/fs/real_fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pwd
 import stat
 from typing import NamedTuple
 from typing import Optional
 
 from trashcli import fs
 from trashcli.fs import write_file
+from trashcli.fstab.real_volume_of import RealVolumeOf
 from trashcli.put.fs.fs import Fs
 
 
 class Names:
     def username(self, uid):  # type: (int) -> Optional[str]
         try:
             return pwd.getpwuid(uid).pw_name
@@ -28,15 +29,18 @@
     ('mode', int),
     ('uid', int),
     ('gid', int),
 ])):
     pass
 
 
-class RealFs(Fs):
+class RealFs(RealVolumeOf, Fs):
+
+    def __init__(self):
+        super(RealFs, self).__init__()
 
     def readlink(self, path):
         return os.readlink(path)
 
     def symlink(self, src, dest):  # type: (str, str) -> None
         os.symlink(src, dest)
 
@@ -108,9 +112,15 @@
 
     def get_mod(self, path):
         return stat.S_IMODE(os.lstat(path).st_mode)
 
     def listdir(self, path):
         return os.listdir(path)
 
-    def lexists(self, path):
+    def read(self, path):
+        return fs.read_file(path)
+
+    def write_file(self, path, content):
+        return fs.write_file(path, content)
+
+    def lexists(selfs, path):
         return os.path.lexists(path)
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/fs/size_counter.py` & `trash_cli-0.24.5.26/trashcli/put/fs/size_counter.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor.py` & `trash_cli-0.24.5.26/trashcli/put/janitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from typing import NamedTuple, TypeVar
 
+from trashcli.put.suffix import Suffix
+
+from trashcli.put.core.int_generator import IntGenerator
+
+from trashcli.put.my_logger import LoggerBackend
+
+from trashcli.put.clock import PutClock
+
 from trashcli.lib.environ import Environ
 from trashcli.put.core.candidate import Candidate
 from trashcli.put.core.either import Left
 from trashcli.put.core.failure_reason import FailureReason, LogContext
 from trashcli.put.core.trashee import Trashee
 from trashcli.put.fs.fs import Fs
 from trashcli.put.janitor_tools.info_creator import TrashInfoCreator
@@ -22,27 +30,26 @@
     def log_entries(self, context):  # type: (LogContext) -> str
         return ""
 
 
 class Janitor:
     def __init__(self,
                  fs,  # type: Fs
-                 trash_dir,  # type: PutTrashDir
-                 trashing_checker,  # type: TrashDirChecker
-                 info_dir,  # type: TrashInfoCreator
-                 persister,  # type: InfoFilePersister
-                 logger,  # type: MyLogger
+                 clock,  # type: PutClock
+                 backend,  # type: LoggerBackend
+                 randint,  # type: IntGenerator
                  ):
-        self.trash_dir = trash_dir
-        self.trashing_checker = trashing_checker
-        self.info_dir = info_dir
+        self.trash_dir = PutTrashDir(fs)
+        self.trashing_checker = TrashDirChecker(fs)
+        self.info_dir = TrashInfoCreator(fs, clock)
         self.security_check = SecurityCheck(fs)
-        self.persister = persister
+        self.persister = InfoFilePersister(fs, MyLogger(backend), Suffix(randint))
         self.dir_creator = TrashDirCreator(fs)
-        self.executor = JobExecutor(logger, TrashedFile)
+        self.executor = JobExecutor(MyLogger(backend), TrashedFile)
+
 
     class Result(NamedTuple('Result', [
         ('ok', bool),
         ('reason', FailureReason)
     ])):
         def succeeded(self):
             return self.ok
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_creator.py` & `trash_cli-0.24.5.26/trashcli/put/janitor_tools/info_creator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import os
+
 from typing import NamedTuple
 
 from trashcli.put.clock import PutClock
 from trashcli.put.core.candidate import Candidate
-from trashcli.put.core.either import Either, Right, Left
+from trashcli.put.core.either import Either
+from trashcli.put.core.either import Left
+from trashcli.put.core.either import Right
 from trashcli.put.core.failure_reason import FailureReason
 from trashcli.put.core.failure_reason import LogContext
 from trashcli.put.format_trash_info import format_trashinfo
-from trashcli.put.janitor_tools.info_file_persister import InfoFilePersister
+from trashcli.put.fs.fs import Fs
 from trashcli.put.janitor_tools.info_file_persister import TrashinfoData
 from trashcli.put.original_location import OriginalLocation
 
 
 class UnableToCreateTrashInfoContent(
     NamedTuple('UnableToCreateTrashInfoContent', [
         ('error', Exception),
@@ -19,19 +22,18 @@
     def log_entries(self, context):  # type: (LogContext) -> str
         return "failed to generate trashinfo content: %s" % (
             self.error)
 
 
 class TrashInfoCreator:
     def __init__(self,
-                 persister,  # type: InfoFilePersister
-                 original_location,  # type: OriginalLocation
+                 fs,   # type: Fs
                  clock,  # type: PutClock
                  ):
-        self.original_location = original_location
+        self.original_location = OriginalLocation(fs)
         self.clock = clock
 
     Result = Either[TrashinfoData, UnableToCreateTrashInfoContent]
 
     def make_trashinfo_data(self,
                             path,  # type: str
                             candidate,  # type: Candidate
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor_tools/info_file_persister.py` & `trash_cli-0.24.5.26/trashcli/put/janitor_tools/info_file_persister.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor_tools/put_trash_dir.py` & `trash_cli-0.24.5.26/trashcli/put/janitor_tools/put_trash_dir.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor_tools/security_check.py` & `trash_cli-0.24.5.26/trashcli/put/janitor_tools/security_check.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_checker.py` & `trash_cli-0.24.5.26/trashcli/put/janitor_tools/trash_dir_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import NamedTuple
 
-from trashcli.fstab.volume_of import VolumeOf
 from trashcli.lib.environ import Environ
 from trashcli.put.core.candidate import Candidate
-from trashcli.put.core.either import Either, Right, Left
-from trashcli.put.core.failure_reason import FailureReason, LogContext
+from trashcli.put.core.either import Either
+from trashcli.put.core.either import Left
+from trashcli.put.core.either import Right
+from trashcli.put.core.failure_reason import FailureReason
+from trashcli.put.core.failure_reason import LogContext
 from trashcli.put.core.trashee import Trashee
 from trashcli.put.fs.fs import Fs
 from trashcli.put.gate import Gate
 from trashcli.put.trash_dir_volume_reader import TrashDirVolumeReader
 
 
 class DifferentVolumes(NamedTuple('DifferentVolumes', [
@@ -29,27 +31,28 @@
         return isinstance(other, HomeFallBackNotEnabled)
 
 
 GateCheckResult = Either[None, FailureReason]
 
 
 class TrashDirChecker:
-    def __init__(self, fs, volumes):  # type: (Fs, VolumeOf) -> None
+    def __init__(self,
+                 fs,  # type: Fs
+                 ):  # type: (...) -> None
         self.fs = fs
-        self.volumes = volumes
 
     def file_could_be_trashed_in(self,
                                  trashee,  # type: Trashee
                                  candidate,  # type: Candidate
                                  environ,  # type: Environ
                                  ):  # type: (...) -> GateCheckResult
         if candidate.gate is Gate.HomeFallback:
             return self._can_be_trashed_in_home_trash_dir(environ)
         elif candidate.gate is Gate.SameVolume:
-            return SameVolumeGateImpl(self.volumes, self.fs).can_trash_in(
+            return SameVolumeGateImpl(self.fs).can_trash_in(
                 trashee, candidate)
         else:
             raise ValueError("Unknown gate: %s" % candidate.gate)
 
     @staticmethod
     def _can_be_trashed_in_home_trash_dir(environ,  # type: Environ
                                           ):
@@ -60,18 +63,16 @@
 
 def make_ok():
     return Right(None)
 
 
 class SameVolumeGateImpl:
     def __init__(self,
-                 volumes,  # type: VolumeOf
                  fs,  # type: Fs
                  ):
-        self.volumes = volumes
         self.fs = fs
 
     def can_trash_in(self,
                      trashee,  # type: Trashee
                      candidate,  # type: Candidate
                      ):
         trash_dir_volume = self._volume_of_trash_dir(candidate)
@@ -79,9 +80,9 @@
 
         if not same_volume:
             return Left(DifferentVolumes(trash_dir_volume, trashee.volume))
 
         return make_ok()
 
     def _volume_of_trash_dir(self, candidate):  # type: (Candidate) -> str
-        return (TrashDirVolumeReader(self.volumes, self.fs)
+        return (TrashDirVolumeReader(self.fs)
                 .volume_of_trash_dir(candidate.trash_dir_path))
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/janitor_tools/trash_dir_creator.py` & `trash_cli-0.24.5.26/trashcli/put/janitor_tools/trash_dir_creator.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 
 class TrashDirCreator:
     def __init__(self, fs):  # type: (Fs) -> None
         self.dir_maker = DirMaker(fs)
 
     def make_candidate_dirs(self,
-                            candidate):  # type: (Candidate) -> Either[None, TrashDirCannotBeCreated]
+                            candidate,  # type: Candidate
+                            ):  # type: (...) -> Either[None, TrashDirCannotBeCreated]
         try:
             self.dir_maker.mkdir_p(candidate.trash_dir_path, 0o700)
             self.dir_maker.mkdir_p(candidate.files_dir(), 0o700)
             self.dir_maker.mkdir_p(candidate.info_dir(), 0o700)
             return Right(None)
         except (IOError, OSError) as error:
             return Left(TrashDirCannotBeCreated(error))
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/jobs.py` & `trash_cli-0.24.5.26/trashcli/put/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 from trashcli.put.my_logger import MyLogger
 
 R = TypeVar('R')
 
 
 class JobStatus(Generic[R]):
     def __init__(self, message):  # type: (str) -> None
-        self.log_entries = [LogEntry(Level.DEBUG, MessageStr(message),
-                                     LogTag.unspecified)]
+        self.log_entries = [LogEntry(Level.DEBUG,
+                                     LogTag.unspecified,
+                                     MessageStr.from_messages([message]))]
 
     def has_succeeded(self):
         return isinstance(self, Succeeded)
 
     def result(self):  # type: () -> R
         raise NotImplementedError
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/my_logger.py` & `trash_cli-0.24.5.26/trashcli/put/my_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         self.stderr = stderr
 
     def write_message(self,
                       log_entry,  # type: LogEntry
                       log_data,  # type: LogData
                       ):
         if is_right_for_level(log_data.verbose, log_entry.level):
-            self.stderr.write("%s: %s\n" % (log_data.program_name,
-                                            log_entry.resolve_message()))
+            for message in log_entry.resolve_messages():
+                self.stderr.write("%s: %s\n" % (log_data.program_name, message))
 
 
 def is_right_for_level(verbose,  # type: int
                        level,  # type: Level
                        ):
     min_level = {
         Level.WARNING: 0,
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/original_location.py` & `trash_cli-0.24.5.26/trashcli/put/original_location.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/parser.py` & `trash_cli-0.24.5.26/trashcli/put/parser.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/put/trash_directories_finder.py` & `trash_cli-0.24.5.26/trashcli/put/trash_directories_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from trashcli.put.core.check_type import NoCheck, TopTrashDirCheck
 from trashcli.put.core.path_maker_type import PathMakerType
 from trashcli.put.gate import Gate
 
 
 class TrashDirectoriesFinder:
     def __init__(self,
-                 volumes,  # type: VolumeOf
+                 fs,  # type: VolumeOf
                  ):
-        self.volumes = volumes
+        self.fs = fs
 
     def possible_trash_directories_for(self,
                                        volume,  # type: str
                                        specific_trash_dir,  # type: str
                                        environ,  # type: Environ
                                        uid,  # type: int
                                        home_fallback,  # type: bool
@@ -48,27 +48,25 @@
                           volume=volume,
                           path_maker_type=PathMakerType.RelativePaths,
                           check_type=NoCheck,
                           gate=Gate.SameVolume))
 
         if specific_trash_dir:
             path = specific_trash_dir
-            volume = self.volumes.volume_of(path)
+            volume = self.fs.volume_of(path)
             trash_dirs.append(
                 Candidate(trash_dir_path=path,
                           volume=volume,
                           path_maker_type=PathMakerType.RelativePaths,
                           check_type=NoCheck,
                           gate=Gate.SameVolume))
         else:
-            for path, dir_volume in home_trash_dir(environ,
-                                                   self.volumes):
+            for path, dir_volume in home_trash_dir(environ, self.fs):
                 add_home_trash(path, dir_volume, Gate.SameVolume)
             for path, dir_volume in volume_trash_dir1(volume, uid):
                 add_top_trash_dir(path, dir_volume)
             for path, dir_volume in volume_trash_dir2(volume, uid):
                 add_alt_top_trash_dir(path, dir_volume)
             if home_fallback:
-                for path, dir_volume in home_trash_dir(environ,
-                                                       self.volumes):
+                for path, dir_volume in home_trash_dir(environ, self.fs):
                     add_home_trash(path, dir_volume, Gate.HomeFallback)
         return trash_dirs
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/trasher.py` & `trash_cli-0.24.5.26/trashcli/put/trasher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,32 @@
+from trashcli.put.my_logger import LoggerBackend
+
 from trashcli.put.context import Context
+from trashcli.put.context import SingleTrasher
 from trashcli.put.core.trash_result import TrashResult
 from trashcli.put.core.trashee import should_skipped_by_specs
 from trashcli.put.file_trasher import FileTrasher
 from trashcli.put.fs.fs import Fs
-from trashcli.put.reporter import TrashPutReporter
+from trashcli.put.my_logger import MyLogger
+from trashcli.put.reporting.trash_put_reporter import TrashPutReporter
 from trashcli.put.user import User
 from trashcli.put.user import user_replied_no
 
 
-class Trasher:
+class Trasher(SingleTrasher):
     def __init__(self,
                  file_trasher,  # type: FileTrasher
                  user,  # type: User
-                 reporter,  # type: TrashPutReporter
                  fs,  # type: Fs
+                 backend,  # type: LoggerBackend
                  ):
         self.file_trasher = file_trasher
         self.user = user
-        self.reporter = reporter
+        self.logger = MyLogger(backend)
+        self.reporter = TrashPutReporter(fs)
         self.fs = fs
 
     def trash_single(self,
                      path,  # type: str
                      context,  # type: Context
                      ):
         """
@@ -36,23 +41,26 @@
             - $volume/.Trash-$uid
 
         Firstly the software attempt to trash the file in the first directory
         then try to trash in the second trash directory.
         """
 
         if should_skipped_by_specs(path):
-            self.reporter.unable_to_trash_dot_entries(path, context.log_data)
+            self.logger.log_put(
+                self.reporter.unable_to_trash_dot_entries(path),
+                context.log_data)
             return TrashResult.Failure
 
         if not self.fs.lexists(path):
             if context.mode.can_ignore_not_existent_path():
                 return TrashResult.Success
             else:
-                self.reporter.unable_to_trash_file_non_existent(path,
-                                                                context.log_data)
+                self.logger.log_put(
+                    self.reporter.unable_to_trash_file_non_existent(path),
+                    context.log_data)
                 return TrashResult.Failure
 
         if context.mode.should_we_ask_to_the_user(self.fs.is_accessible(path)):
             reply = self.user.ask_user_about_deleting_file(context.program_name,
                                                            path)
             if reply == user_replied_no:
                 return TrashResult.Success
```

### Comparing `trash_cli-0.24.4.17/trashcli/put/user.py` & `trash_cli-0.24.5.26/trashcli/put/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     def __init__(self,
                  my_input,  # type: Input
                  describer,  # type: Describer
                  ):
         self.input = my_input
         self.describer = describer
 
+
     def ask_user_about_deleting_file(self, program_name, path):
         reply = self.input.read_input(
             "%s: trash %s '%s'? " % (program_name,
                                      self.describer.describe(path), path))
         return parse_user_reply(reply)
```

### Comparing `trash_cli-0.24.4.17/trashcli/restore/file_system.py` & `trash_cli-0.24.5.26/trashcli/restore/file_system.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/handler.py` & `trash_cli-0.24.5.26/trashcli/restore/handler.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/info_dir_searcher.py` & `trash_cli-0.24.5.26/trashcli/restore/info_dir_searcher.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/info_files.py` & `trash_cli-0.24.5.26/trashcli/restore/info_files.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/main.py` & `trash_cli-0.24.5.26/trashcli/restore/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import trashcli.trash
 from .file_system import RealRestoreReadFileSystem, \
     RealRestoreWriteFileSystem, RealReadCwd, RealFileReader, \
     RealListingFileSystem
 from .info_dir_searcher import InfoDirSearcher
 from .info_files import InfoFiles
+from .real_restore_logger import RealRestoreLogger
 from .restore_cmd import RestoreCmd
 from .trash_directories import TrashDirectoriesImpl
 from .trashed_files import TrashedFiles
 from ..fstab.volumes import RealVolumes
 from ..lib.logger import my_logger
 from ..lib.my_input import RealInput
 
@@ -19,15 +20,15 @@
 def main():
     info_files = InfoFiles(RealListingFileSystem())
     volumes = RealVolumes()
     trash_directories = TrashDirectoriesImpl(volumes,
                                              os.getuid(),
                                              os.environ)
     searcher = InfoDirSearcher(trash_directories, info_files)
-    trashed_files = TrashedFiles(my_logger,
+    trashed_files = TrashedFiles(RealRestoreLogger(my_logger),
                                  RealFileReader(),
                                  searcher)
     RestoreCmd.make(
         stdout=sys.stdout,
         stderr=sys.stderr,
         exit=sys.exit,
         input=RealInput(),
```

### Comparing `trash_cli-0.24.4.17/trashcli/restore/output.py` & `trash_cli-0.24.5.26/trashcli/restore/output.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/output_recorder.py` & `trash_cli-0.24.5.26/trashcli/restore/output_recorder.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/range.py` & `trash_cli-0.24.5.26/trashcli/restore/range.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/real_output.py` & `trash_cli-0.24.5.26/trashcli/restore/real_output.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/restore_arg_parser.py` & `trash_cli-0.24.5.26/trashcli/restore/restore_arg_parser.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/restore_asking_the_user.py` & `trash_cli-0.24.5.26/trashcli/restore/restore_asking_the_user.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/restore_cmd.py` & `trash_cli-0.24.5.26/trashcli/restore/restore_cmd.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/restorer.py` & `trash_cli-0.24.5.26/trashcli/restore/restorer.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/run_restore_action.py` & `trash_cli-0.24.5.26/trashcli/restore/run_restore_action.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/sort_method.py` & `trash_cli-0.24.5.26/trashcli/restore/sort_method.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/trash_directories.py` & `trash_cli-0.24.5.26/trashcli/restore/trash_directories.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/trashed_file.py` & `trash_cli-0.24.5.26/trashcli/restore/trashed_file.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/restore/trashed_files.py` & `trash_cli-0.24.5.26/trashcli/restore/trashed_files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-from logging import Logger
-from typing import Optional, Iterable, NamedTuple, Union
+from typing import Iterable
+from typing import NamedTuple
+from typing import Optional
+from typing import Union
 
 from trashcli.lib.path_of_backup_copy import path_of_backup_copy
 from trashcli.parse_trashinfo.parse_deletion_date import parse_deletion_date
 from trashcli.parse_trashinfo.parse_original_location import \
     parse_original_location
 from trashcli.restore.file_system import FileReader
 from trashcli.restore.info_dir_searcher import InfoDirSearcher
+from trashcli.restore.restore_logger import RestoreLogger
 from trashcli.restore.trashed_file import TrashedFile
 
 
 class TrashedFiles:
     def __init__(self,
-                 logger,  # type: Logger
+                 logger,  # type: RestoreLogger
                  file_reader,  # type: FileReader
                  searcher,  # type: InfoDirSearcher
                  ):
         self.logger = logger
         self.file_reader = file_reader
         self.searcher = searcher
 
@@ -25,15 +28,15 @@
                           ):  # type: (...) -> Iterable[TrashedFile]
         for event in self.all_trashed_files_internal(trash_dir_from_cli):
             if type(event) is NonTrashinfoFileFound:
                 self.logger.warning("Non .trashinfo file in info dir")
             elif type(event) is NonParsableTrashInfo:
                 self.logger.warning(
                     "Non parsable trashinfo file: %s, because %s" %
-                    event.path, event.reason)
+                    (event.path, event.reason))
             elif type(event) is IOErrorReadingTrashInfo:
                 self.logger.warning(str(event))
             elif type(event) is TrashedFileFound:
                 yield event.trashed_file
             else:
                 raise RuntimeError()
```

### Comparing `trash_cli-0.24.4.17/trashcli/rm/cleanable_trashcan.py` & `trash_cli-0.24.5.26/trashcli/rm/cleanable_trashcan.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/rm/list_trashinfo.py` & `trash_cli-0.24.5.26/trashcli/rm/list_trashinfo.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/rm/main.py` & `trash_cli-0.24.5.26/trashcli/rm/main.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/shell_completion.py` & `trash_cli-0.24.5.26/trashcli/shell_completion.py`

 * *Files identical despite different names*

### Comparing `trash_cli-0.24.4.17/trashcli/trash_dirs_scanner.py` & `trash_cli-0.24.5.26/trashcli/trash_dirs_scanner.py`

 * *Files identical despite different names*

