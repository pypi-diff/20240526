# Comparing `tmp/jellyash-0.5.3.tar.gz` & `tmp/jellyash-0.6.0.tar.gz`

## Comparing `jellyash-0.5.3.tar` & `jellyash-0.6.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jellyash-0.5.3/tox.ini
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 jellyash-0.5.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/bundle.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/cli.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/client.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/duration.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/nextup.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/search.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/token.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jellyash-0.5.3/jellyash/unwatched.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/conftest.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_bundle.py
--rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_client.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_duration.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_nextup.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_search.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_token.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/test_unwatched.py
--rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.client.yaml
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
--rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.client.yaml
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.client.yaml
--rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_single_term.yaml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_special_season.yaml
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.5.3/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.5.3/LICENSE
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 jellyash-0.5.3/README.md
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 jellyash-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 jellyash-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jellyash-0.6.0/tox.ini
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 jellyash-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/bundle.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/cli.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/client.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/duration.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/nextup.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/search.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/token.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jellyash-0.6.0/jellyash/unwatched.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_bundle.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_client.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_duration.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_nextup.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_search.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_token.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/test_unwatched.py
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_bundle/TestApiResponse.client.yaml
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_client/TestAuthedClient.client.yaml
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_duration/TestDuration.client.yaml
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_single_term.yaml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_special_season.yaml
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 jellyash-0.6.0/README.md
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 jellyash-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 jellyash-0.6.0/PKG-INFO
```

### Comparing `jellyash-0.5.3/.github/workflows/ci.yml` & `jellyash-0.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/jellyash/bundle.py` & `jellyash-0.6.0/jellyash/bundle.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/jellyash/client.py` & `jellyash-0.6.0/jellyash/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-import inspect
 import json
 import pathlib
 import platform
 import sys
 from json.decoder import JSONDecodeError
-from typing import Optional
 from uuid import uuid4
 
 from jellyfin_apiclient_python.client import JellyfinClient
 from jellyfin_apiclient_python.connection_manager import CONNECTION_STATE
 
 from . import __version__
 from .bundle import WrappedAPI
 
 CREDENTIALS_FILE = pathlib.Path.home() / ".jellyfin_creds"
 
 
-def create_client(app_name: Optional[str] = None):
+def create_client():
     client = JellyfinClient()
-    if not app_name:
-        app_name = determine_app_name()
-    client.config.app(app_name, __version__, platform.node(), str(uuid4()))
+    client.config.app("jellyash", __version__, platform.node(), str(uuid4()))
     client.config.data["auth.ssl"] = True
     client.jellyfin = WrappedAPI(client.http)
     return client
 
 
 def auth_with_password(client, address: str, user: str, password: str):
     client.auth.connect_to_address(address)
@@ -38,22 +34,17 @@
         credentials = json.load(f)
     state = client.authenticate({"Servers": [credentials]}, discover=False)
     if state["State"] != CONNECTION_STATE["SignedIn"]:
         raise ConnectionError("Failed to establish connection")
 
 
 def authed_client():
-    client = create_client(None)
+    client = create_client()
     try:
         auth_with_token(client)
     except (
         PermissionError, ValueError, JSONDecodeError, ConnectionError
         ) as e:
         print(f"{sys.argv[0]}: {e}")
         sys.exit(1)
     return client
 
-
-def determine_app_name() -> str:
-    frame = inspect.stack()[-2]
-    return f"jellyfin_{inspect.getmodulename(frame.filename)}"
-
```

### Comparing `jellyash-0.5.3/jellyash/duration.py` & `jellyash-0.6.0/jellyash/duration.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/jellyash/nextup.py` & `jellyash-0.6.0/jellyash/nextup.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/jellyash/search.py` & `jellyash-0.6.0/jellyash/search.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/jellyash/token.py` & `jellyash-0.6.0/jellyash/token.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     parser = argparse_parser()
     parser.add_argument("-u", "--user", dest="user", default=getuser())
     parser.add_argument(
         "server", nargs="?", default="https://jellyfin.wedontsleep.org/"
     )
     args = parser.parse_args()
     password = getpassword()
-    client = create_client("create_jellyfin_token")
+    client = create_client()
     result = auth_with_password(client, args.server, args.user, password)
     if "AccessToken" in result:
         credentials = client.auth.credentials.get_credentials()
         server = credentials["Servers"][0]
         server["username"] = args.user
         with open(CREDENTIALS_FILE, "w") as f:
             json.dump(server, f)
```

### Comparing `jellyash-0.5.3/jellyash/unwatched.py` & `jellyash-0.6.0/jellyash/unwatched.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/conftest.py` & `jellyash-0.6.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     dir_name = klass.__module__.split(".")[1]
     cassette_filename = f"{klass.__name__}.client.yaml"
     cassette = Path(f"tests/cassettes/{dir_name}/{cassette_filename}")
     if klass.is_recording:
         # vcrpy will not overwrite an existing cassette, remove it.
         cassette.unlink(missing_ok=True)
     with vcr.use_cassette(cassette, record_mode="once"):
-        client = create_client(f"jellyash_test_{klass.__name__.lower()}")
+        client = create_client()
         server_url = "https://demo.jellyfin.org/stable"
         auth_result = auth_with_password(client, server_url, "demo", "")
         assert "AccessToken" in auth_result
         return client
 
 
 @pytest.fixture(scope="class")
```

### Comparing `jellyash-0.5.3/tests/test_bundle.py` & `jellyash-0.6.0/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/test_client.py` & `jellyash-0.6.0/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 
 from jellyash import __version__
 from jellyash.client import (
     auth_with_password,
     auth_with_token,
     authed_client,
     create_client,
-    determine_app_name,
 )
 
 from .conftest import ClientTest
 
 
 class TestClient(unittest.TestCase):
     def setUp(self):
-        self.client = create_client("test")
+        self.client = create_client()
 
-    def test_create_client_with_app_name(self):
+    def test_create_client(self):
         data = self.client.config.data
-        self.assertEqual(data['app.name'], "test")
+        self.assertEqual(data['app.name'], "jellyash")
         self.assertEqual(data['app.device_name'], platform.node())
         self.assertEqual(data['app.version'], __version__)
         self.assertTrue(data['auth.ssl'])
 
     @pytest.mark.vcr
     def test_auth_with_password(self):
         server_url = "https://demo.jellyfin.org/stable"
@@ -119,12 +118,7 @@
         self.assertEqual(captured.err, "")
 
     def test_authed_client_non_existant_file(self):
         non_exist = pathlib.Path("/does/not/exist")
         with patch("jellyash.client.CREDENTIALS_FILE", non_exist):
             with self.assertRaises(SystemExit):
                 authed_client()
-
-
-class TestDetermineAppName(unittest.TestCase):
-    def test_determine_app_name(self):
-        self.assertEqual(determine_app_name(), "jellyfin___init__")
```

### Comparing `jellyash-0.5.3/tests/test_duration.py` & `jellyash-0.6.0/tests/test_duration.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/test_nextup.py` & `jellyash-0.6.0/tests/test_nextup.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/test_search.py` & `jellyash-0.6.0/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/test_token.py` & `jellyash-0.6.0/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/test_unwatched.py` & `jellyash-0.6.0/tests/test_unwatched.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.client.yaml` & `jellyash-0.6.0/tests/cassettes/test_bundle/TestApiResponse.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml` & `jellyash-0.6.0/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml` & `jellyash-0.6.0/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml` & `jellyash-0.6.0/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_bool_response.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml` & `jellyash-0.6.0/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_dict_response.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.client.yaml` & `jellyash-0.6.0/tests/cassettes/test_client/TestAuthedClient.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml` & `jellyash-0.6.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml` & `jellyash-0.6.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml` & `jellyash-0.6.0/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.client.yaml` & `jellyash-0.6.0/tests/cassettes/test_duration/TestDuration.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml` & `jellyash-0.6.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml` & `jellyash-0.6.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml` & `jellyash-0.6.0/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml` & `jellyash-0.6.0/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml` & `jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml` & `jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact_with_space.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml` & `jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_search/TestSearch.test_single_term.yaml` & `jellyash-0.6.0/tests/cassettes/test_search/TestSearch.test_single_term.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml` & `jellyash-0.6.0/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.client.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_season.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_special_season.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_unknown_special_season.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml` & `jellyash-0.6.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_with_season.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/LICENSE` & `jellyash-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/README.md` & `jellyash-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Jelly **A**eroplane **S**hark **H**elper
 
 Wrapper around jellyfin-apiclient-python to provide convenience functions:
 
 Create an unauthenticated client:
 
 ```
-create_client(app_name)
+create_client()
 ```
 
 Authenticate with username and password:
 
 ```
 auth_with_password(client, address, user, password)
 ```
```

### Comparing `jellyash-0.5.3/pyproject.toml` & `jellyash-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jellyash-0.5.3/PKG-INFO` & `jellyash-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jellyash
-Version: 0.5.3
+Version: 0.6.0
 Project-URL: Source, https://github.com/s-t-e-v-e-n-k/jellyash
 License: Copyright 2023 Steve Kowalik <steven@wedontsleep.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -24,15 +24,15 @@
 Jelly **A**eroplane **S**hark **H**elper
 
 Wrapper around jellyfin-apiclient-python to provide convenience functions:
 
 Create an unauthenticated client:
 
 ```
-create_client(app_name)
+create_client()
 ```
 
 Authenticate with username and password:
 
 ```
 auth_with_password(client, address, user, password)
 ```
```

