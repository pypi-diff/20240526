# Comparing `tmp/hangman_solver_rs-0.2.1.tar.gz` & `tmp/hangman_solver_rs-0.3.0.tar.gz`

## Comparing `hangman_solver_rs-0.2.1.tar` & `hangman_solver_rs-0.3.0.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 hangman_solver_rs-0.2.1/Cargo.toml
--rw-r--r--   0     1000      985    11970 2023-12-31 15:22:31.000000 hangman_solver_rs-0.2.1/Cargo.lock
--rw-r--r--   0     1000      985    13827 2023-04-08 17:46:37.000000 hangman_solver_rs-0.2.1/LICENSE
--rw-r--r--   0     1000      985     6937 2023-12-31 14:36:02.000000 hangman_solver_rs-0.2.1/build.rs
--rw-r--r--   0     1000      985     2435 2023-12-31 15:08:54.000000 hangman_solver_rs-0.2.1/src/language/mod.rs
--rw-r--r--   0     1000      985     2331 2023-12-31 15:16:22.000000 hangman_solver_rs-0.2.1/src/lib.rs
--rw-r--r--   0     1000      985     2599 2023-12-31 15:08:08.000000 hangman_solver_rs-0.2.1/src/main.rs
--rw-r--r--   0     1000      985     9852 2023-12-31 16:16:42.000000 hangman_solver_rs-0.2.1/src/solver/mod.rs
--rw-r--r--   0     1000      985     1504 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
--rw-r--r--   0     1000      985      989 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE
--rw-r--r--   0     1000      985     1294 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1070 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0     1000      985      197 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/cryptography-41.0.5.dist-info/LICENSE
--rw-r--r--   0     1000      985    11358 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1081 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1078 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     2338 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0     1000      985     1053 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1536 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE
--rw-r--r--   0     1000      985     1331 2023-11-25 20:15:43.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
--rw-r--r--   0     1000      985     9694 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE
--rw-r--r--   0     1000      985    10142 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0     1000      985      596 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
--rw-r--r--   0     1000      985      564 2023-11-25 20:15:43.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1056 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1050 2023-11-25 20:15:29.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     9695 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE
--rw-r--r--   0     1000      985     1023 2023-11-25 20:15:43.000000 hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1504 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
--rw-r--r--   0     1000      985      989 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE
--rw-r--r--   0     1000      985     1294 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1070 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
--rw-r--r--   0     1000      985      197 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/cryptography-41.0.5.dist-info/LICENSE
--rw-r--r--   0     1000      985    11358 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1081 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1078 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     2338 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
--rw-r--r--   0     1000      985     1053 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1536 2023-11-25 20:15:44.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE
--rw-r--r--   0     1000      985     1331 2023-11-25 20:15:43.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
--rw-r--r--   0     1000      985     9694 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE
--rw-r--r--   0     1000      985    10142 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE
--rw-r--r--   0     1000      985      596 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
--rw-r--r--   0     1000      985      564 2023-11-25 20:15:43.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1056 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     1050 2023-11-25 20:15:29.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0     1000      985     9695 2023-11-25 20:15:45.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE
--rw-r--r--   0     1000      985     1023 2023-11-25 20:15:43.000000 hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE
--rw-r--r--   0     1000      985       54 2023-11-24 17:37:50.000000 hangman_solver_rs-0.2.1/words/LICENSE
--rw-r--r--   0     1000      985 44698353 2023-06-29 15:37:23.000000 hangman_solver_rs-0.2.1/words/de.txt
--rw-r--r--   0     1000      985  1437112 2023-11-25 19:56:51.000000 hangman_solver_rs-0.2.1/words/de_basic.txt
--rw-r--r--   0     1000      985   868719 2023-11-24 18:17:18.000000 hangman_solver_rs-0.2.1/words/en.txt
--rw-r--r--   0     1000      985      857 2023-11-24 23:38:15.000000 hangman_solver_rs-0.2.1/pyproject.toml
--rw-r--r--   0     1000      985      290 2023-11-24 23:37:09.000000 hangman_solver_rs-0.2.1/python/hangman_solver/__init__.py
--rw-r--r--   0     1000      985        0 2023-11-24 23:23:08.000000 hangman_solver_rs-0.2.1/python/hangman_solver/py.typed
--rw-r--r--   0     1000      985     1461 2023-11-28 20:39:50.000000 hangman_solver_rs-0.2.1/python/hangman_solver/__init__.pyi
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 hangman_solver_rs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 hangman_solver_rs-0.3.0/Cargo.toml
+-rw-r--r--   0     1000      985    16203 2024-05-26 21:04:59.000000 hangman_solver_rs-0.3.0/Cargo.lock
+-rw-r--r--   0     1000      985    13827 2023-04-08 17:46:37.000000 hangman_solver_rs-0.3.0/LICENSE
+-rw-r--r--   0     1000      985     7845 2024-05-26 18:31:40.000000 hangman_solver_rs-0.3.0/build.rs
+-rw-r--r--   0     1000      985    13827 2024-01-05 19:30:24.000000 hangman_solver_rs-0.3.0/pkg/LICENSE
+-rw-r--r--   0     1000      985     2593 2024-05-26 20:44:25.000000 hangman_solver_rs-0.3.0/src/language/mod.rs
+-rw-r--r--   0     1000      985     3007 2024-05-26 20:55:12.000000 hangman_solver_rs-0.3.0/src/lib.rs
+-rw-r--r--   0     1000      985     4633 2024-05-26 20:52:43.000000 hangman_solver_rs-0.3.0/src/main.rs
+-rw-r--r--   0     1000      985     1500 2024-05-26 19:27:11.000000 hangman_solver_rs-0.3.0/src/solver/char_collection.rs
+-rw-r--r--   0     1000      985    12673 2024-05-26 20:43:07.000000 hangman_solver_rs-0.3.0/src/solver/mod.rs
+-rw-r--r--   0     1000      985     1504 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
+-rw-r--r--   0     1000      985      989 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1294 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1070 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0     1000      985      197 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/cryptography-41.0.5.dist-info/LICENSE
+-rw-r--r--   0     1000      985    11358 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1081 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1078 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     2338 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1053 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1536 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1331 2023-11-25 20:15:43.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
+-rw-r--r--   0     1000      985     9694 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985    10142 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985      596 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985      564 2023-11-25 20:15:43.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1056 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1050 2023-11-25 20:15:29.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     9695 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1023 2023-11-25 20:15:43.000000 hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1504 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
+-rw-r--r--   0     1000      985      989 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1294 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1070 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE
+-rw-r--r--   0     1000      985      197 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/cryptography-41.0.5.dist-info/LICENSE
+-rw-r--r--   0     1000      985    11358 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1081 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1023 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1078 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     2338 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1053 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1536 2023-11-25 20:15:44.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1331 2023-11-25 20:15:43.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE
+-rw-r--r--   0     1000      985     9694 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985    10142 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985      596 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985      564 2023-11-25 20:15:43.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1056 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1050 2023-11-25 20:15:29.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985     9695 2023-11-25 20:15:45.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE
+-rw-r--r--   0     1000      985     1023 2023-11-25 20:15:43.000000 hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE
+-rw-r--r--   0     1000      985       54 2023-11-24 17:37:50.000000 hangman_solver_rs-0.3.0/words/LICENSE
+-rw-r--r--   0     1000      985 44698353 2023-06-29 15:37:23.000000 hangman_solver_rs-0.3.0/words/de.txt
+-rw-r--r--   0     1000      985  1437112 2023-11-25 19:56:51.000000 hangman_solver_rs-0.3.0/words/de_basic.txt
+-rw-r--r--   0     1000      985   868719 2023-11-24 18:17:18.000000 hangman_solver_rs-0.3.0/words/en.txt
+-rw-r--r--   0     1000      985      857 2024-05-26 21:05:51.000000 hangman_solver_rs-0.3.0/pyproject.toml
+-rw-r--r--   0     1000      985      290 2023-11-24 23:37:09.000000 hangman_solver_rs-0.3.0/python/hangman_solver/__init__.py
+-rw-r--r--   0     1000      985        0 2023-11-24 23:23:08.000000 hangman_solver_rs-0.3.0/python/hangman_solver/py.typed
+-rw-r--r--   0     1000      985     1499 2024-05-26 18:11:36.000000 hangman_solver_rs-0.3.0/python/hangman_solver/__init__.pyi
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 hangman_solver_rs-0.3.0/PKG-INFO
```

### Comparing `hangman_solver_rs-0.2.1/Cargo.toml` & `hangman_solver_rs-0.3.0/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "hangman_solver"
-version = "0.2.1"
+version = "0.3.0"
 edition = "2021"
 repository = "https://github.com/asozialesnetzwerk/hangman_solver"
 description = "Solves hangman puzzles"
 license-file = "LICENSE"
 include = [
     "build.rs",
     "src/*",
@@ -13,20 +13,22 @@
     "Cargo.lock",
     "LICENSE",
 ]
 build = "build.rs"
 
 [features]
 default = ["terminal_size"]
+wasm-bindgen = ["dep:wasm-bindgen", "dep:js-sys"]
 
 [profile.release]
 codegen-units = 1
 panic = "abort"
 strip = true
 lto = true
+opt-level = "z"
 
 [profile.profile]
 inherits = "release"
 strip = false
 lto = false
 debug = 1
 
@@ -36,14 +38,18 @@
 [lib]
 name = "hangman_solver_lib"
 crate-type = ["cdylib"]
 
 [dependencies]
 cfg-if = { version = "1.0.0", features = [] }
 counter = "0.5.7"
-itertools = { version = "0.12.0", features = [] }
-pyo3 = { version = "0.20.0", features = ["extension-module", "abi3", "abi3-py310"], optional = true }
+itertools = { version = "0.13.0", features = [] }
+pyo3 = { version = "0.21.2", features = ["extension-module", "abi3", "abi3-py312"], optional = true }
 terminal_size = { version = "0.3.0", optional = true }
+wasm-bindgen = { version = "0.2.92", optional = true }
+js-sys = { version = "0.3.69", optional = true }
+
 
 [build-dependencies]
-itertools = { version = "0.12.0", features = [] }
+itertools = { version = "0.13.0", features = [] }
 Inflector = "0.11.4"
+unicode-segmentation = "1.10.1"
```

### Comparing `hangman_solver_rs-0.2.1/Cargo.lock` & `hangman_solver_rs-0.3.0/Cargo.lock`

 * *Files 19% similar despite different names*

```diff
@@ -10,44 +10,38 @@
 dependencies = [
  "lazy_static",
  "regex",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
-name = "bitflags"
-version = "2.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
-
-[[package]]
-name = "cc"
-version = "1.0.79"
+name = "bumpalo"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -58,392 +52,540 @@
 checksum = "2d458e66999348f56fd3ffcfbb7f7951542075ca8359687c703de6500c1ddccd"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.1"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "errno"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys",
-]
-
-[[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
- "cc",
  "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "hangman_solver"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "Inflector",
  "cfg-if",
  "counter",
  "itertools",
+ "js-sys",
  "pyo3",
  "terminal_size",
+ "unicode-segmentation",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25db6b064527c5d482d0423354fcd07a89a2dfe07b67892e62411946db7f07b0"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "js-sys"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.11"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "969488b55f8ac402214f3f5fd243ebb7206cf82de60d3172994707a4bcc2b829"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
+
+[[package]]
 name = "memchr"
-version = "2.6.4"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.69"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dac53072f717aa1bfa4db832b39de8c875b7c7af4f4a6fe93cdbf9264cf8383b"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7774b5a8282bd4f25f803b1f0d945120be959a36c72e08e7cd031c792fdfd424"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rustix"
-version = "0.38.25"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc99bc2d4f1fed22595588a013687477aedf3cdcfb26558c559edb67b4d9b22e"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.39"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23e78b90f2fcf45d3e842032ce32e3f2d1545ba6636271dcbf24fa306d87be7a"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "terminal_size"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21bebf2b7c9e0a515f6e0f8c51dc0f8e4696391e6f1ff30379559f8365fb0df7"
 dependencies = [
  "rustix",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
+name = "unicode-segmentation"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
+
+[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
+
+[[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.0"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+
+[[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+
+[[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+
+[[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+
+[[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+
+[[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.0"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+
+[[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.0"
+version = "0.48.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `hangman_solver_rs-0.2.1/LICENSE` & `hangman_solver_rs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/build.rs` & `hangman_solver_rs-0.3.0/build.rs`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 use std::io;
 use std::io::BufRead;
 use std::io::BufReader;
 use std::path::{Path, PathBuf};
 
 use inflector::Inflector;
 use itertools::Itertools;
+use unicode_segmentation::UnicodeSegmentation;
 
 type StrConv = fn(String) -> String;
 
 fn read_lines_of_file(
     path: &Path,
 ) -> Result<impl Iterator<Item = String>, io::Error> {
     let file = File::open(path)?;
@@ -77,14 +78,22 @@
     let out_dir: &String = &env::var("OUT_DIR").unwrap();
     Path::new(out_dir).join(path)
 }
 
 fn write_words_data(words_data: &WordsData) {
     let mut words: Vec<String> = words_data.read_lines();
 
+    for word in &words {
+        assert_eq!(
+            UnicodeSegmentation::graphemes(word.as_str(), true).count(),
+            word.chars().count(),
+            "{word} is",
+        );
+    }
+
     words.sort_unstable();
     words.sort_by_key(|word: &String| word.chars().count());
 
     let words: Vec<(usize, Vec<String>)> = words
         .into_iter()
         .unique()
         .into_group_map_by(|word: &String| word.chars().count())
@@ -95,15 +104,15 @@
     let mut output = String::new();
     output += "match length {";
     for (length, words_group) in words {
         let max_real_str_length: usize = words_group
             .iter()
             .map(|word| word.as_str().len())
             .max()
-            .unwrap();
+            .expect("word group needs to have max length");
 
         output += &*format!("{length} => ({max_real_str_length}, \"");
 
         let string_content: String = if max_real_str_length == length {
             words_group.iter().join("").replace('"', "\\\"")
         } else {
             println!("{} {length} {max_real_str_length}", words_data.lang);
@@ -167,26 +176,28 @@
         }
         words_vec.push(data);
     }
 
     let words_vec: Vec<WordsData> = words_vec
         .iter()
         .sorted_by_key(|data| data.lang.as_str())
-        .map(std::clone::Clone::clone)
+        .cloned()
         .collect();
 
     for word_data in &words_vec {
         write_words_data(word_data);
     }
 
+    let language_count = words_vec.len();
+
     fs::write(
         get_out_dir_joined(String::from("language.rs")),
         format!(
             r###"#[cfg_attr(feature = "pyo3", pyclass)]
-#[derive(Copy, Clone, Eq, PartialEq)]
+#[derive(Copy, Clone, Eq, PartialEq, Debug)]
 pub enum Language {{
     {}
 }}
 
 impl Language {{
     #[must_use]
     pub const fn read_words(self, length: usize) -> StringChunkIter {{
@@ -194,15 +205,15 @@
             {}
         }};
         StringChunkIter::new(length, words, padded_length)
     }}
 
     #[inline]
     #[must_use]
-    pub const fn all() -> [Self; {}] {{
+    pub const fn all() -> [Self; {language_count}] {{
         [
             {}
         ]
     }}
 
     #[inline]
     #[must_use]
@@ -219,25 +230,49 @@
     #[inline]
     pub const fn name(&self) -> &'static str {{
         match self {{
             {}
         }}
     }}
 }}
+
+#[cfg(feature = "pyo3")]
+#[pymethods]
+impl Language {{
+    #[staticmethod]
+    #[must_use]
+    const fn values() -> [Self; {language_count}] {{
+        Self::all()
+    }}
+
+    #[allow(clippy::trivially_copy_pass_by_ref)]
+    #[getter]
+    #[must_use]
+    const fn value(&self) -> &'static str {{
+        self.name()
+    }}
+
+    #[staticmethod]
+    #[pyo3(signature = (name, default = None))]
+    pub fn parse_string(name: &str, default: Option<Self>) -> PyResult<Self> {{
+        Self::from_string(name)
+            .or(default)
+            .ok_or_else(|| UnknownLanguageError::new_err(name.to_owned()))
+    }}
+}}
 "###,
             words_vec.iter().map(WordsData::enum_name).join(",\n"),
             words_vec
                 .iter()
                 .map(|data| format!(
                     "Self::{} => include!(concat!(env!(\"OUT_DIR\"), \"/{}\"))",
                     data.enum_name(),
                     data.out_file_name()
                 ))
                 .join("\n,"),
-            words_vec.len(),
             words_vec
                 .iter()
                 .map(|data| format!("Self::{}", data.enum_name()))
                 .join(", "),
             words_vec
                 .iter()
                 .map(|data| format!(
```

### Comparing `hangman_solver_rs-0.2.1/src/language/mod.rs` & `hangman_solver_rs-0.3.0/src/language/mod.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 // SPDX-License-Identifier: EUPL-1.2
+use std::num::NonZeroUsize;
+
+#[cfg(feature = "pyo3")]
+use std::ops::Div;
 
 #[cfg(feature = "pyo3")]
 use pyo3::create_exception;
 #[cfg(feature = "pyo3")]
 use pyo3::exceptions::PyValueError;
 #[cfg(feature = "pyo3")]
 use pyo3::prelude::*;
 
+use crate::solver::char_collection::CharCollection;
+
 #[cfg_attr(feature = "pyo3", pyclass)]
 pub struct StringChunkIter {
-    word_length: usize,
-    padded_word_byte_count: usize,
+    pub word_length: usize,
+    padded_word_byte_count: NonZeroUsize,
+    is_ascii: bool,
     index: usize,
     string: &'static str,
 }
 
 impl StringChunkIter {
     #[must_use]
     pub const fn new(
         word_length: usize,
         string: &'static str,
         padded_word_byte_count: usize,
     ) -> Self {
         Self {
             word_length,
-            index: 0,
+            padded_word_byte_count: if let Some(non_zero) =
+                NonZeroUsize::new(padded_word_byte_count)
+            {
+                non_zero
+            } else {
+                NonZeroUsize::MIN
+            },
+            index: if string.is_empty() { usize::MAX } else { 0 },
+            is_ascii: word_length == padded_word_byte_count,
             string,
-            padded_word_byte_count,
         }
     }
 }
 
 impl Iterator for StringChunkIter {
     type Item = &'static str;
 
     #[must_use]
+    #[inline]
     fn next(&mut self) -> Option<Self::Item> {
-        let index = self.index;
-        if index >= self.string.len() {
-            return None;
-        }
-        self.index += self.padded_word_byte_count;
-
-        let result = &self.string.get(index..self.index)?;
-        if result.len() == self.word_length {
-            debug_assert!(!result.starts_with('\0'));
-            return Some(result);
-        }
-        let result = result.trim_start_matches('\0');
-        debug_assert!(result.len() >= self.word_length);
+        let end_index =
+            self.index.checked_add(self.padded_word_byte_count.get())?;
+        debug_assert_ne!(self.index, end_index);
+
+        let result = self.string.get(self.index..end_index)?;
+
+        let result = if self.is_ascii {
+            result
+        } else {
+            result.trim_start_matches('\0')
+        };
+
+        debug_assert!(end_index <= self.string.len());
+        self.index = end_index;
+        debug_assert!(!result.contains('\0'));
+        debug_assert_eq!(result.char_count(), self.word_length);
         Some(result)
     }
 }
 
 #[cfg(feature = "pyo3")]
 #[pymethods]
 impl StringChunkIter {
@@ -63,41 +81,24 @@
 
     #[must_use]
     fn __next__(&mut self) -> Option<&'static str> {
         self.next()
     }
 
     #[must_use]
-    const fn __len__(&self) -> usize {
-        self.string.len() / self.padded_word_byte_count
+    pub fn __len__(&self) -> usize {
+        self.string.len().div(self.padded_word_byte_count)
+    }
+
+    #[must_use]
+    pub fn __length_hint__(&self) -> usize {
+        self.string
+            .len()
+            .checked_sub(self.index)
+            .map_or(0, |rest| rest.div(self.padded_word_byte_count))
     }
 }
 
 include!(concat!(env!("OUT_DIR"), "/language.rs"));
 
 #[cfg(feature = "pyo3")]
 create_exception!(hangman_solver, UnknownLanguageError, PyValueError);
-
-#[cfg(feature = "pyo3")]
-#[pymethods]
-impl Language {
-    #[allow(clippy::trivially_copy_pass_by_ref)]
-    #[getter]
-    #[must_use]
-    const fn value(&self) -> &'static str {
-        self.name()
-    }
-
-    #[staticmethod]
-    #[must_use]
-    const fn values() -> [Self; 5] {
-        Self::all()
-    }
-
-    #[staticmethod]
-    #[pyo3(signature = (name, default = None))]
-    pub fn parse_string(name: &str, default: Option<Self>) -> PyResult<Self> {
-        Self::from_string(name)
-            .or(default)
-            .ok_or_else(|| UnknownLanguageError::new_err(name.to_owned()))
-    }
-}
```

### Comparing `hangman_solver_rs-0.2.1/src/lib.rs` & `hangman_solver_rs-0.3.0/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 #![deny(clippy::indexing_slicing, clippy::panic, clippy::unwrap_used)]
 #![allow(clippy::missing_errors_doc)]
 mod language;
 mod solver;
 
 pub use crate::language::{Language, StringChunkIter};
 
-pub use crate::solver::{solve_hangman_puzzle, HangmanResult, Pattern};
+pub use crate::solver::{HangmanResult, Pattern};
+
+#[cfg(feature = "wasm-bindgen")]
+pub use crate::solver::WasmHangmanResult;
+#[cfg(feature = "wasm-bindgen")]
+use js_sys::JsString;
+#[cfg(feature = "wasm-bindgen")]
+use wasm_bindgen::prelude::*;
 
 #[cfg(feature = "pyo3")]
 pub use crate::language::UnknownLanguageError;
 #[cfg(feature = "pyo3")]
 use pyo3::prelude::*;
 
 #[cfg(feature = "pyo3")]
@@ -27,37 +34,29 @@
 pub fn solve(
     pattern_string: String,
     invalid_letters: Vec<char>,
     language: Language,
     max_words_to_collect: usize,
 ) -> PyResult<HangmanResult> {
     let pattern = Pattern::new(&pattern_string, &invalid_letters, true);
-    Ok(solve_hangman_puzzle(
-        &pattern,
-        language,
-        Some(max_words_to_collect),
-    ))
+    Ok(pattern.solve(language, Some(max_words_to_collect)))
 }
 
 #[cfg(feature = "pyo3")]
 #[pyfunction]
 #[pyo3(signature = (pattern_string, invalid_letters, language, max_words_to_collect))]
 #[allow(clippy::needless_pass_by_value)]
 pub fn solve_crossword(
     pattern_string: String,
     invalid_letters: Vec<char>,
     language: Language,
     max_words_to_collect: usize,
 ) -> PyResult<HangmanResult> {
     let pattern = Pattern::new(&pattern_string, &invalid_letters, false);
-    Ok(solve_hangman_puzzle(
-        &pattern,
-        language,
-        Some(max_words_to_collect),
-    ))
+    Ok(pattern.solve(language, Some(max_words_to_collect)))
 }
 
 #[cfg(feature = "pyo3")]
 #[pyfunction]
 #[pyo3(signature = (language, word_length))]
 pub const fn read_words_with_length(
     language: Language,
@@ -65,19 +64,39 @@
 ) -> PyResult<StringChunkIter> {
     Ok(language.read_words(word_length))
 }
 
 #[cfg(feature = "pyo3")]
 #[pymodule]
 #[pyo3(name = "_solver")]
-pub fn hangman_solver(py: Python<'_>, m: &PyModule) -> PyResult<()> {
+pub fn hangman_solver(py: Python<'_>, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(solve, m)?)?;
     m.add_function(wrap_pyfunction!(solve_crossword, m)?)?;
     m.add_function(wrap_pyfunction!(read_words_with_length, m)?)?;
     m.add(
         "UnknownLanguageError",
-        py.get_type::<UnknownLanguageError>(),
+        py.get_type_bound::<UnknownLanguageError>(),
     )?;
     m.add_class::<HangmanResult>()?;
     m.add_class::<Language>()?;
     Ok(())
 }
+
+#[cfg(feature = "wasm-bindgen")]
+#[wasm_bindgen]
+#[allow(clippy::needless_pass_by_value)]
+pub fn solve_hangman(
+    all_words: Vec<JsString>,
+    pattern_string: JsString,
+    invalid_letters: JsString,
+    max_words_to_collect: usize,
+    crossword_mode: bool,
+) -> Result<WasmHangmanResult, JsValue> {
+    let pattern =
+        Pattern::new(&pattern_string, &invalid_letters, !crossword_mode);
+
+    let mut all_words_iter = all_words.iter();
+
+    let result: WasmHangmanResult = pattern
+        .solve_with_words(&mut all_words_iter, Some(max_words_to_collect));
+    Ok(result)
+}
```

### Comparing `hangman_solver_rs-0.2.1/src/solver/mod.rs` & `hangman_solver_rs-0.3.0/src/solver/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,27 @@
 // SPDX-License-Identifier: EUPL-1.2
+pub mod char_collection;
+
 use cfg_if::cfg_if;
 use std::char;
 use std::iter::zip;
 
-use crate::language::{Language, StringChunkIter};
+use crate::language::Language;
+use crate::solver::char_collection::CharCollection;
 
 use counter::Counter;
 use itertools::Itertools;
 
 #[cfg(feature = "pyo3")]
 use pyo3::prelude::*;
 
 const WILDCARD_CHAR: char = '_';
-const WILDCARD_CHAR_AS_STR: &str = "_";
 const WILDCARD_ALIASES: [char; 2] = ['#', '?'];
 const RESERVED_CHARS: [char; 5] = ['#', '?', '_', '\0', '\n'];
 
-trait CharCount {
-    fn char_count(&self) -> usize;
-}
-
-impl CharCount for String {
-    #[inline]
-    fn char_count(&self) -> usize {
-        self.chars().count()
-    }
-}
-
-impl CharCount for str {
-    #[inline]
-    fn char_count(&self) -> usize {
-        self.chars().count()
-    }
-}
-
 #[inline]
 fn join_with_max_length<T: ExactSizeIterator<Item = String>>(
     strings: T,
     sep: &str,
     max_len: usize,
 ) -> String {
     let last_index = strings.len() - 1;
@@ -126,48 +110,74 @@
                 )
             )?;
         };
         Ok(())
     }
 }
 
+#[cfg(feature = "wasm-bindgen")]
+use js_sys::JsString;
+#[cfg(feature = "wasm-bindgen")]
+use wasm_bindgen::prelude::*;
+
+#[cfg(feature = "wasm-bindgen")]
+#[wasm_bindgen(getter_with_clone)]
+pub struct WasmHangmanResult {
+    #[wasm_bindgen(readonly)]
+    pub input: JsString,
+    #[wasm_bindgen(readonly)]
+    pub invalid: JsString,
+    #[wasm_bindgen(readonly)]
+    pub matching_words_count: u32,
+    #[wasm_bindgen(readonly)]
+    pub possible_words: Vec<JsString>,
+    #[wasm_bindgen(readonly)]
+    pub letter_frequency: JsString,
+}
+
 #[allow(clippy::struct_field_names)]
 pub struct Pattern {
     pub invalid_letters: Vec<char>,
     pub pattern: Vec<char>,
     pub first_letter: char,
     /// true for normal hangman mode
     letters_in_pattern_have_no_other_occurrences: bool,
 }
 
 impl Pattern {
     #[must_use]
-    pub fn new(
-        pattern: &str,
-        invalid_letters: &[char],
+    #[inline]
+    pub fn new<T: CharCollection, V: CharCollection>(
+        pattern: &T,
+        invalid_letters: &V,
         letters_in_pattern_have_no_other_occurrences: bool,
     ) -> Self {
         let pattern_as_chars: Vec<char> = pattern
-            .to_lowercase()
-            .replace(WILDCARD_ALIASES, WILDCARD_CHAR_AS_STR)
-            .chars()
+            .iter_chars()
+            .flat_map(char::to_lowercase)
             .filter(|ch| !ch.is_whitespace())
+            .map(|ch| {
+                if WILDCARD_ALIASES.contains(&ch) {
+                    WILDCARD_CHAR
+                } else {
+                    ch
+                }
+            })
             .collect();
 
         let additional_invalid: Vec<char> =
             if letters_in_pattern_have_no_other_occurrences {
                 pattern_as_chars.clone()
             } else {
                 vec![]
             };
 
         let invalid_letters_vec: Vec<char> = additional_invalid
-            .iter()
-            .chain(invalid_letters)
-            .copied()
+            .into_iter()
+            .chain(invalid_letters.iter_chars())
             .filter(|ch| *ch != WILDCARD_CHAR && !ch.is_whitespace())
             .unique()
             .collect();
 
         let first_letter = *pattern_as_chars.first().unwrap_or(&WILDCARD_CHAR);
 
         Self {
@@ -181,35 +191,39 @@
     #[inline]
     #[must_use]
     const fn first_letter_is_wildcard(&self) -> bool {
         self.first_letter == WILDCARD_CHAR
     }
 
     #[must_use]
-    fn first_letter_matches(&self, word: &str) -> bool {
+    #[inline]
+    fn first_letter_matches<CC: CharCollection + ?Sized>(
+        &self,
+        word: &&CC,
+    ) -> bool {
         // This only makes sense if first_letter_is_wildcard is false
         debug_assert!(!self.first_letter_is_wildcard());
-        word.chars()
-            .next()
+        word.first_char()
             .map_or(false, |char| self.first_letter == char)
     }
 
     #[must_use]
-    fn matches(&self, word: &str) -> bool {
+    #[inline]
+    fn matches<CC: CharCollection + ?Sized>(&self, word: &&CC) -> bool {
         // This only makes sense if word has the same length as the pattern
         debug_assert_eq!(word.char_count(), self.pattern.len());
         // none of the reserved chars shall be in the word
         debug_assert_eq!(
             RESERVED_CHARS
                 .iter()
-                .filter(|ch| word.chars().contains(ch))
+                .filter(|ch| word.iter_chars().contains(ch))
                 .count(),
             0
         );
-        for (p, w) in zip(self.pattern.iter(), word.chars()) {
+        for (p, w) in zip(self.pattern.iter(), word.iter_chars()) {
             if *p == WILDCARD_CHAR {
                 if self.invalid_letters.contains(&w) {
                     return false;
                 }
             } else if *p != w {
                 return false;
             }
@@ -223,34 +237,38 @@
         self.pattern
             .iter()
             .filter(|ch| **ch != WILDCARD_CHAR)
             .count()
     }
 
     #[must_use]
-    fn collect_count_and_create_letter_frequency<
-        T: Iterator<Item = &'static str>,
+    #[inline]
+    fn _collect_count_and_create_letter_frequency<
+        'a,
+        'b,
+        CC: CharCollection + ?Sized + 'a,
+        T: Iterator<Item = &'a CC>,
     >(
         &self,
-        words: T,
+        words: &'b mut T,
         max_words_to_collect: Option<usize>,
-    ) -> (u32, Counter<char, u32>, Vec<&'static str>) {
+    ) -> (u32, Counter<char, u32>, Vec<&'a CC>) {
         let mut letter_counter: Counter<char, u32> = Counter::new();
 
-        let update_counter: fn(&mut Counter<char, u32>, &str) =
+        let update_counter: fn(&mut Counter<char, u32>, &CC) =
             if self.letters_in_pattern_have_no_other_occurrences {
-                |counter, word| counter.update(word.chars().unique())
+                |counter, word| counter.update(word.iter_chars().unique())
             } else {
-                |counter, word| counter.update(word.chars())
+                |counter, word| counter.update(word.iter_chars())
             };
 
-        let mut words = words
-            .inspect(|word: &&str| update_counter(&mut letter_counter, word));
+        let mut words =
+            words.inspect(|word| update_counter(&mut letter_counter, word));
 
-        let (words_vec, additional_count): (Vec<&'static str>, usize) =
+        let (words_vec, additional_count): (Vec<&'a CC>, usize) =
             if let Some(n) = max_words_to_collect {
                 (words.by_ref().take(n).collect(), words.count())
             } else {
                 (words.collect(), 0)
             };
 
         let words_count = u32::try_from(additional_count + words_vec.len())
@@ -274,59 +292,120 @@
                     letter_counter.remove(letter);
                 }
             }
         }
 
         (words_count, letter_counter, words_vec)
     }
-}
 
-#[must_use]
-pub fn solve_hangman_puzzle(
-    pattern: &Pattern,
-    language: Language,
-    max_words_to_collect: Option<usize>,
-) -> HangmanResult {
-    let all_words: StringChunkIter = language.read_words(pattern.pattern.len());
-
-    let (word_count, letter_frequency, words) = if pattern.known_letters_count()
-        == 0
-        && pattern.invalid_letters.is_empty()
-    {
-        pattern.collect_count_and_create_letter_frequency(
-            all_words,
-            max_words_to_collect,
-        )
-    } else if pattern.first_letter_is_wildcard() {
-        pattern.collect_count_and_create_letter_frequency(
-            all_words.filter(|word| pattern.matches(word)),
-            max_words_to_collect,
-        )
-    } else {
-        pattern.collect_count_and_create_letter_frequency(
-            all_words
-                .skip_while(|word| !pattern.first_letter_matches(word))
-                .take_while(|word| pattern.first_letter_matches(word))
-                .filter(|word| pattern.matches(word)),
-            max_words_to_collect,
-        )
-    };
-
-    let input_string: String = pattern.pattern.iter().collect();
-
-    let mut invalid_in_result: Vec<char> = pattern
-        .invalid_letters
-        .iter()
-        .filter(|ch| !pattern.pattern.contains(*ch))
-        .copied()
-        .collect();
-
-    invalid_in_result.sort_unstable();
-    HangmanResult {
-        input: input_string,
-        invalid: invalid_in_result,
-        possible_words: words,
-        language,
-        letter_frequency: letter_frequency.most_common_ordered(),
-        matching_words_count: word_count,
+    #[must_use]
+    #[inline]
+    pub fn solve(
+        &self,
+        language: Language,
+        max_words_to_collect: Option<usize>,
+    ) -> HangmanResult {
+        let mut all_words = language.read_words(self.pattern.len());
+        let (possible_words, letter_frequency, matching_words_count) =
+            self._solve_internal(&mut all_words, max_words_to_collect);
+
+        let mut invalid: Vec<char> = self
+            .invalid_letters
+            .iter()
+            .filter(|ch| !self.pattern.contains(*ch))
+            .copied()
+            .collect();
+
+        invalid.sort_unstable();
+        HangmanResult {
+            input: self.pattern.iter().collect(),
+            invalid,
+            possible_words,
+            language,
+            letter_frequency,
+            matching_words_count,
+        }
+    }
+
+    #[cfg(feature = "wasm-bindgen")]
+    #[must_use]
+    #[allow(dead_code)]
+    pub fn solve_with_words<'a, 'b, T: Iterator<Item = &'a JsString>>(
+        &self,
+        all_words: &'b mut T,
+        max_words_to_collect: Option<usize>,
+    ) -> WasmHangmanResult {
+        let (possible_words, letter_frequency, matching_words_count) =
+            self._solve_internal(all_words, max_words_to_collect);
+
+        let mut invalid: Vec<char> = self
+            .invalid_letters
+            .iter()
+            .filter(|ch| !self.pattern.contains(*ch))
+            .copied()
+            .collect();
+
+        let mut letter_frequency_string: String = String::new();
+
+        for (char, count) in letter_frequency {
+            if !letter_frequency_string.is_empty() {
+                letter_frequency_string.push_str(", ");
+            }
+            letter_frequency_string.push(char);
+            letter_frequency_string.push_str(": ");
+            letter_frequency_string.push_str(&count.to_string());
+        }
+
+        invalid.sort_unstable();
+        WasmHangmanResult {
+            input: JsString::from(self.pattern.iter().collect::<String>()),
+            invalid: JsString::from(invalid.iter().collect::<String>()),
+            possible_words: possible_words
+                .into_iter()
+                .map(JsString::to_string)
+                .collect(),
+            letter_frequency: JsString::from(letter_frequency_string),
+            matching_words_count,
+        }
+    }
+
+    #[must_use]
+    #[inline]
+    fn _solve_internal<
+        'a,
+        'b,
+        CC: CharCollection + ?Sized + 'a,
+        T: Iterator<Item = &'a CC>,
+    >(
+        &self,
+        all_words: &'b mut T,
+        max_words_to_collect: Option<usize>,
+    ) -> (Vec<&'a CC>, Vec<(char, u32)>, u32) {
+        let (word_count, letter_frequency, words) =
+            if self.known_letters_count() == 0
+                && self.invalid_letters.is_empty()
+            {
+                self._collect_count_and_create_letter_frequency(
+                    all_words,
+                    max_words_to_collect,
+                )
+            } else if self.first_letter_is_wildcard() {
+                let mut filtered_words =
+                    all_words.filter(|word| self.matches(word));
+                self._collect_count_and_create_letter_frequency(
+                    &mut filtered_words,
+                    max_words_to_collect,
+                )
+            } else {
+                let mut filtered_words = all_words
+                    .skip_while(|word| !self.first_letter_matches(word))
+                    .take_while(|word| self.first_letter_matches(word))
+                    .filter(|word| self.matches(word));
+                self._collect_count_and_create_letter_frequency(
+                    &mut filtered_words,
+                    max_words_to_collect,
+                )
+            };
+
+        (words, letter_frequency.most_common_ordered(), word_count)
     }
 }
```

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/SecretStorage-3.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/certifi-2023.11.17.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/cffi-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/charset_normalizer-3.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/importlib_metadata-6.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/jaraco.classes-3.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/jeepney-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/keyring-24.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/mdurl-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/more_itertools-10.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/pycparser-2.21.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/pygments-2.17.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/readme_renderer-42.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/requests-2.31.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/rfc3986-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/rich-13.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/setuptools-65.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/twine-4.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/venv/lib64/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE` & `hangman_solver_rs-0.3.0/venv/lib64/python3.11/site-packages/zipp-3.17.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/words/de.txt` & `hangman_solver_rs-0.3.0/words/de.txt`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/words/de_basic.txt` & `hangman_solver_rs-0.3.0/words/de_basic.txt`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/words/en.txt` & `hangman_solver_rs-0.3.0/words/en.txt`

 * *Files identical despite different names*

### Comparing `hangman_solver_rs-0.2.1/pyproject.toml` & `hangman_solver_rs-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hangman-solver-rs"
-requires-python = ">=3.10"
+requires-python = ">=3.12"
 license = {file = "LICENSE"}
 keywords = ["hangman", "solver", "rust"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
     "Operating System :: OS Independent",
```

### Comparing `hangman_solver_rs-0.2.1/python/hangman_solver/__init__.pyi` & `hangman_solver_rs-0.3.0/python/hangman_solver/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     matching_words_count: int
     invalid: list[str]
     language: Language
     words: list[str]
     letter_frequency: list[tuple[str, int]]
 
 class Language:
+    __init__ = None
+    __new__ = None
 
     @staticmethod
     def parse_string(name: str, default: Language = None) -> Language:
         pass
 
     @staticmethod
     def values() -> list[Language]:
@@ -57,15 +59,14 @@
         pass
 
     def __repr__(self) -> str:
         pass
 
     value: str
 
-
     De: ClassVar[Language]
     DeBasic: ClassVar[Language]
     DeBasicUmlauts: ClassVar[Language]
     DeUmlauts: ClassVar[Language]
     En: ClassVar[Language]
```

### Comparing `hangman_solver_rs-0.2.1/PKG-INFO` & `hangman_solver_rs-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hangman-solver-rs
-Version: 0.2.1
+Version: 0.3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 License-File: LICENSE
 License-File: LICENSE
 Summary: Solves hangman puzzles
 Keywords: hangman,solver,rust
-Requires-Python: >=3.10
+Requires-Python: >=3.12
 Project-URL: Source Code, https://github.com/asozialesnetzwerk/hangman_solver
```

