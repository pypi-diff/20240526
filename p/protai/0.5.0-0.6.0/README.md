# Comparing `tmp/protai-0.5.0.tar.gz` & `tmp/protai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.5.0.tar", last modified: Thu May 23 23:59:50 2024, max compression
+gzip compressed data, was "protai-0.6.0.tar", last modified: Sat May 25 22:44:57 2024, max compression
```

## Comparing `protai-0.5.0.tar` & `protai-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 23:59:50.645553 protai-0.5.0/
--rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.5.0/LICENSE
--rw-rw-rw-   0        0        0     3293 2024-05-23 23:59:50.645553 protai-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2619 2024-05-23 23:24:58.000000 protai-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 23:59:50.634027 protai-0.5.0/protai/
--rw-rw-rw-   0        0        0        5 2024-05-23 23:58:45.000000 protai-0.5.0/protai/VERSION
--rw-rw-rw-   0        0        0       69 2024-05-23 18:18:24.000000 protai-0.5.0/protai/__init__.py
--rw-rw-rw-   0        0        0     4608 2024-05-23 18:18:24.000000 protai-0.5.0/protai/auth.py
--rw-rw-rw-   0        0        0     2417 2024-05-23 18:18:24.000000 protai-0.5.0/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-23 23:59:50.643551 protai-0.5.0/protai.egg-info/
--rw-rw-rw-   0        0        0     3293 2024-05-23 23:59:50.000000 protai-0.5.0/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-23 23:59:50.000000 protai-0.5.0/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 23:59:50.000000 protai-0.5.0/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-23 23:59:50.000000 protai-0.5.0/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-23 23:59:50.000000 protai-0.5.0/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 23:59:50.000000 protai-0.5.0/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 23:59:50.646554 protai-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     4178 2024-05-23 18:18:24.000000 protai-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:44:57.083592 protai-0.6.0/
+-rw-rw-rw-   0        0        0     1107 2024-05-23 18:18:24.000000 protai-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3293 2024-05-25 22:44:57.082593 protai-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2619 2024-05-23 23:24:58.000000 protai-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 22:44:57.060663 protai-0.6.0/protai/
+-rw-rw-rw-   0        0        0        5 2024-05-25 22:42:27.000000 protai-0.6.0/protai/VERSION
+-rw-rw-rw-   0        0        0       69 2024-05-23 18:18:24.000000 protai-0.6.0/protai/__init__.py
+-rw-rw-rw-   0        0        0     4919 2024-05-25 22:43:02.000000 protai-0.6.0/protai/auth.py
+-rw-rw-rw-   0        0        0     3253 2024-05-25 22:42:56.000000 protai-0.6.0/protai/protai.py
+drwxrwxrwx   0        0        0        0 2024-05-25 22:44:57.080450 protai-0.6.0/protai.egg-info/
+-rw-rw-rw-   0        0        0     3293 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-25 22:44:57.000000 protai-0.6.0/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 22:44:57.083592 protai-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     4178 2024-05-23 18:18:24.000000 protai-0.6.0/setup.py
```

### Comparing `protai-0.5.0/LICENSE` & `protai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `protai-0.5.0/PKG-INFO` & `protai-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.5.0
+Version: 0.6.0
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.5.0/README.md` & `protai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `protai-0.5.0/protai/auth.py` & `protai-0.6.0/protai/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,157 @@
-#!/usr/bin/env python
-"""
-This function handles authentication with the GROQ API
-
-Author: Protik Banerji <protik09@users.noreply.github.com>
-
-"""
-
-import os
-import keyring
-import re
-import keyring.errors
-from prompt_toolkit import prompt
-
-KEYRING_SYSTEM: str = "groq"
-KEYRING_USER: str = "api-key"
-KEYRING_FLAG: bool = False
-
-
-def _checkKeyringExists() -> bool:
-    """Check if keyring exists"""
-    keyring_exists: bool = False
-    try:
-        keyring.get_keyring()  # Check if keyring is available
-        keyring_exists = True
-    except keyring.errors.NoKeyringError:  # If keyring is not available
-        print("[KeyringError]: Keyring is not available. You're probably running in WSL. ProtAI is not aupported in WSL")
-        exit(1)
-    except keyring.errors.InitError:  # If keyring is not available
-        print("[KeyringError]: Keyring initialization failed.")
-    except keyring.errors.KeyringLocked:
-        print("[KeyringError]: Keyring is locked.")
-    return keyring_exists
-
-
-def _getApiKeyFromKeyring() -> str:
-    """Get password from keyring"""
-    password: str = None
-    if _checkKeyringExists():  # If keyring is available
-        try:
-            password: str = keyring.get_password(KEYRING_SYSTEM, KEYRING_USER)
-        except keyring.errors.KeyringError as e:  # If keyring is not available
-            print(f"[KeyringError]: {e}")
-    return password
-
-
-def _getApiKeyUser() -> str:
-    """Get API key from user"""
-    try:
-        api_key = prompt("Enter GROQ API Key: ", is_password=True)
-    except KeyboardInterrupt:
-        print("KeyboardInterrupt: Exiting...")
-        exit(1)
-    return api_key
-
-
-def _validateApiKey(api_key: str) -> bool:
-    """Validate API key"""
-    pattern = re.compile(r"^gsk_[a-zA-Z0-9]{30,1024}$")
-    return bool(pattern.match(api_key))
-
-
-def _deleteApiKey() -> None:
-    """Delete API key from keyring and environment variable"""
-    if _checkKeyringExists():  # If keyring is available
-        try:
-            keyring.delete_password(KEYRING_SYSTEM, KEYRING_USER)
-            del os.environ["GROQ_API_KEY"]
-        except (
-            KeyError,
-            keyring.errors.PasswordDeleteError,
-        ):
-            print(
-                "[KeyringError]: Failed to delete password in keyring or os.environ. \
-                    It's ok though you can still overwrite it."
-            )
-    else:  # If keyring is not available
-        print("[OsEnvError]: GROQ_API_KEY is not available.")
-
-
-def changeApiKey() -> int:
-    """Change API key"""
-    error_code = 0
-    # Delete key from keyring
-    _deleteApiKey()
-    # Ask user for password
-    api_key = _getApiKeyUser()
-
-    if _validateApiKey(api_key):  # Validate API key
-        keyring.set_password(
-            KEYRING_SYSTEM, KEYRING_USER, api_key
-        )  # Store password in keyring
-    else:
-        error_code = 1  # Invalid API key
-
-    return error_code
-
-
-def authGroq() -> str:
-    """Get API key either from Environment Variable or Keyring"""
-    api_key = None
-
-    # GET API KEY
-    # Check if GROQ API Key exists as an environment variable
-    if "GROQ_API_KEY" in os.environ:
-        api_key = os.environ["GROQ_API_KEY"]
-        print("[DEBUG]: GROQ_API_KEY is set as an environment variable")
-        if api_key == "":
-            print("GROQ_API_KEY is empty")
-            del os.environ["GROQ_API_KEY"]  # Delete key from environment
-            api_key = None
-    elif _getApiKeyFromKeyring() is None:  # If password is not stored in keyring
-        # Get password from user
-        api_key = _getApiKeyUser()
-        # print(f"[DEBUG]: Entered API key length: {len(api_key)}")  # Debugging info
-        try:
-            # Store password in keyring
-            keyring.set_password(KEYRING_SYSTEM, KEYRING_USER, api_key)
-        except keyring.errors.PasswordSetError:
-            print("[KeyringError]: Failed to set password in keyring")
-    else:  # If password is stored in keyring
-        api_key = _getApiKeyFromKeyring()  # Get password from keyring
-
-    # Validate API key
-    if not _validateApiKey(api_key):
-        print("[KeyError]: Invalid API key. Please check your API key.")
-        _deleteApiKey()  # Delete API key from keyring and environment variable
-        api_key = None
-    else:  # It is a valid API Key
-        pass
-    return api_key
-
-
-if __name__ == "__main__":
-    api_key = authGroq()
-    if api_key:
-        print("Authentication successful")
-    else:
-        print("Authentication failed")
+#!/usr/bin/env python
+"""
+This function handles authentication with the GROQ API
+
+Author: Protik Banerji <protik09@users.noreply.github.com>
+
+"""
+
+import os
+import re
+import keyring
+import keyring.errors
+
+# This dependancy exists solely so I can give user feedback when typing in a masked password
+from prompt_toolkit import prompt
+
+KEYRING_SYSTEM: str = "groq"
+KEYRING_USER: str = "api-key"
+API_KEY_MIN_SIZE: int = 30
+API_KEY_MAX_SIZE: int = 1024
+
+
+def _checkKeyringExists() -> bool:
+    """Check if keyring exists"""
+    keyring_exists: bool = False
+    try:
+        keyring.get_keyring()  # Check if keyring is available
+        keyring_exists = True
+    except keyring.errors.NoKeyringError:  # If keyring is not available
+        print(
+            "[KeyringError]: Keyring is not available. You're probably running in WSL. \
+ProtAI is not aupported in WSL"
+        )
+        exit(1)
+    except keyring.errors.InitError:  # If keyring is not available
+        print("[KeyringError]: Keyring initialization failed.")
+        exit(1)
+    except keyring.errors.KeyringLocked:
+        print("[KeyringError]: Keyring is locked.")
+        exit(1)
+    return keyring_exists
+
+
+def _getApiKeyFromKeyring() -> str:
+    """Get password from keyring"""
+    password: str = None
+    if _checkKeyringExists():  # If keyring is available
+        try:
+            password: str = keyring.get_password(KEYRING_SYSTEM, KEYRING_USER)
+        except keyring.errors.KeyringError as e:  # If keyring is not available
+            print(f"[KeyringError]: {e}")
+            exit(1)
+    return password
+
+
+def _getApiKeyUser() -> str:
+    """Get API key from user"""
+    try:
+        api_key = prompt("Enter GROQ API Key: ", is_password=True)
+    except KeyboardInterrupt:
+        print("KeyboardInterrupt: Exiting...")
+        exit(1)
+    return api_key
+
+
+def _validateApiKey(api_key: str) -> bool:
+    """Validate API key"""
+    pattern = re.compile(
+        r"^gsk_[a-zA-Z0-9]{"
+        + str(API_KEY_MIN_SIZE)
+        + r","
+        + str(API_KEY_MAX_SIZE)
+        + r"}$"  # ^gsk_[a-zA-Z0-9]{30,1024}$
+    )
+    return bool(pattern.match(api_key))
+
+
+def _deleteApiKey() -> None:
+    """Delete API key from keyring and environment variable"""
+    if _checkKeyringExists():  # If keyring is available
+        try:
+            keyring.delete_password(KEYRING_SYSTEM, KEYRING_USER)
+        except keyring.errors.PasswordDeleteError:
+            print("[KeyringError]: Failed to delete password in keyring.")
+
+        try:
+            del os.environ["GROQ_API_KEY"]
+        except KeyError:
+            #             print(
+            #                 "[KeyringError]: Failed to delete password in os.environ. \
+            # It's ok though you can still overwrite it."
+            #             )
+            pass
+    else:  # If keyring is not available
+        print("[OsEnvError]: GROQ_API_KEY is not available.")
+    exit(0)
+
+
+def changeApiKey() -> int:
+    """Change API key"""
+    error_code = 0
+    # Delete key from keyring
+    _deleteApiKey()
+    # Ask user for password
+    api_key = _getApiKeyUser()
+
+    if _validateApiKey(api_key):  # Validate API key
+        keyring.set_password(
+            KEYRING_SYSTEM, KEYRING_USER, api_key
+        )  # Store password in keyring
+    else:
+        error_code = 1  # Invalid API key
+
+    return error_code
+
+
+def authGroq() -> str:
+    """Get API key either from Environment Variable or Keyring"""
+    api_key = None
+
+    # GET API KEY
+    # Check if GROQ API Key exists as an environment variable
+    if "GROQ_API_KEY" in os.environ:
+        api_key = os.environ["GROQ_API_KEY"]
+        print("[DEBUG]: GROQ_API_KEY is set as an environment variable")
+        if api_key == "":
+            print("GROQ_API_KEY is empty")
+            del os.environ["GROQ_API_KEY"]  # Delete key from environment
+            api_key = None
+    elif _getApiKeyFromKeyring() is None:  # If password is not stored in keyring
+        # Get password from user
+        api_key = _getApiKeyUser()
+        # print(f"[DEBUG]: Entered API key length: {len(api_key)}")  # Debugging info
+        try:
+            # Store password in keyring
+            keyring.set_password(KEYRING_SYSTEM, KEYRING_USER, api_key)
+        except keyring.errors.PasswordSetError:
+            print("[KeyringError]: Failed to set password in keyring")
+    else:  # If password is stored in keyring
+        api_key = _getApiKeyFromKeyring()  # Get password from keyring
+
+    # Validate API key
+    if not _validateApiKey(api_key):
+        print("[KeyError]: Invalid API key. Please check your API key.")
+        _deleteApiKey()  # Delete API key from keyring and environment variable
+        api_key = None
+    else:  # It is a valid API Key
+        pass
+    return api_key
+
+
+if __name__ == "__main__":
+    api_key = authGroq()
+    if api_key:
+        print("Authentication successful")
+    else:
+        print("Authentication failed")
```

### Comparing `protai-0.5.0/protai/protai.py` & `protai-0.6.0/protai/protai.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,89 @@
-#!/usr/bin/env python
-import sys
-import os
-from rich import print
-from rich.markdown import Markdown
-from groq import Groq
-from auth import authGroq, changeApiKey
-
-
-# Set your GROQ API endpoint URL
-GROQ_API_URL = "https://api.groq.io/v1/query"
-# Get the absolute path of the current directory
-current_directory = os.path.abspath(os.path.dirname(__file__))
-# Construct the absolute path for the VERSION file
-version_file_path = os.path.join(current_directory, "VERSION")
-with open(version_file_path, "r") as f:
-    try:
-        ProtAI_VERSION = f.read().strip()
-        # print(ProtAI_VERSION)
-    except ValueError:
-        ProtAI_VERSION = "Invalid version number"
-
-
-def exitHandler(exit_code: int) -> None:
-    sys.exit(exit_code)
-
-
-def main():
-    if len(sys.argv) < 2:
-        print("Usage: protai <user input>")
-        exitHandler(1)
-
-    # user_input = urllib.parse.quote(sys.argv[1])  # Sanitize the user input
-    user_input = ""
-    for args in sys.argv:
-        if args == sys.argv[0]:
-            continue
-        if args == "-h" or args == "--help":
-            print("Usage: protai <user input>")
-            exitHandler(0)
-        if args == "-v" or args == "--version":
-            print(f"{ProtAI_VERSION}")
-            exitHandler(0)
-        if args == "-c" or args == "--change":
-            print("Change the API key for the GROQ API")
-            exitHandler(changeApiKey())
-        user_input += str(args) + " "
-    # print(f"[DEBUG] User input is: {user_input}")
-
-    # Set the query parameters
-    client = Groq(api_key=authGroq())
-    system_prompt = "You are an AI agent called ProtAI. You will reply succinctly to any input you receive. \
-        Your replies will be in the Github Markdown format. ALWAYS start your replies with '[ProtAI]: ' \
-        If providing code snippets, always ensure code highlighting for the appropriate programming language \
-        is applied."
-
-    # Send the request to the GROQ API
-    chat_completion = client.chat.completions.create(
-        messages=[
-            {"role": "system", "content": system_prompt},
-            {"role": "user", "content": user_input},
-        ],
-        model="llama3-8b-8192",
-    )
-    reply = chat_completion.choices[0].message.content
-
-    # Print the reply in Markdown using Glow
-    print(Markdown(reply))
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+import sys
+import os
+from rich import print
+from rich.markdown import Markdown
+from groq import Groq, GroqError
+from auth import authGroq, changeApiKey
+from yaspin import yaspin
+
+
+# Set your GROQ API endpoint URL
+GROQ_API_URL = "https://api.groq.io/v1/query"
+
+
+def versionHandler() -> None:
+    """Print the version number of ProtAI."""
+    # Get the absolute path of the current directory
+    current_directory = os.path.abspath(os.path.dirname(__file__))
+    # Construct the absolute path for the VERSION file
+    version_file_path = os.path.join(current_directory, "VERSION")
+    with open(version_file_path, "r") as f:
+        try:
+            ProtAI_VERSION = f.read().strip()
+            # print(ProtAI_VERSION)
+        except ValueError:
+            ProtAI_VERSION = "Invalid version number"
+    print(f"{ProtAI_VERSION}")
+    exitHandler(0)
+
+
+def exitHandler(exit_code: int) -> None:
+    """TODO: Write more comprehensive exit handler when inspiration strikes."""
+    sys.exit(exit_code)
+
+
+def main():
+    if len(sys.argv) < 2:
+        print("Usage: protai <user input>")
+        exitHandler(1)
+
+    # user_input = urllib.parse.quote(sys.argv[1])  # Sanitize the user input
+    user_input = ""
+    for args in sys.argv:
+        if args == sys.argv[0]:
+            continue
+        if args == "-h" or args == "--help":
+            print("Usage: protai <user input>")
+            exitHandler(0)
+        if args == "-v" or args == "--version":
+            versionHandler()
+        if args == "-c" or args == "--change":
+            print("Change the API key for the GROQ API")
+            exitHandler(changeApiKey())
+        user_input += str(args) + " "
+    # print(f"[DEBUG] User input is: {user_input}")
+
+    # Set the query parameters
+    try:
+        client = Groq(api_key=authGroq())
+    except GroqError:  # Catch any errors from the Groq class
+        print("An error occurred when authenticating with the GROQ API.")
+
+    system_prompt = "You are an AI agent called ProtAI. You will reply succinctly to any input you receive. \
+        Your replies will be in the Standard Markdown format. ALWAYS start your replies with '[ProtAI]: ' \
+        If providing code snippets, always ensure code highlighting for the appropriate programming language \
+        is applied. Always ensure, if sending markdown, that the markdown is sytactically correct."
+
+    with yaspin(text="Processing...", color="green") as spinner:
+        try:
+            # Send the request to the GROQ API
+            chat_completion = client.chat.completions.create(
+                messages=[
+                    {"role": "system", "content": system_prompt},
+                    {"role": "user", "content": user_input},
+                ],
+                model="llama3-8b-8192",
+            )
+            reply = chat_completion.choices[0].message.content
+            spinner.ok("[✔ ]")  # mark spinner as finished successfully
+            # Print the reply in Markdown
+            print(Markdown(str("\033[F" + reply)))
+        except Exception as e:
+            spinner.fail("[✖ ] Processing Failed...")  # mark spinner as failed
+            print(f"An error occurred: {e}")
+            exitHandler(1)
+
+
+if __name__ == "__main__":
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `protai-0.5.0/protai.egg-info/PKG-INFO` & `protai-0.6.0/protai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.5.0
+Version: 0.6.0
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.5.0/setup.py` & `protai-0.6.0/setup.py`

 * *Files identical despite different names*

