# Comparing `tmp/ppynet-0.0.2.tar.gz` & `tmp/ppynet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppynet-0.0.2.tar", last modified: Sun Apr  7 21:25:42 2024, max compression
+gzip compressed data, was "ppynet-0.0.3.tar", last modified: Wed May 22 21:19:54 2024, max compression
```

## Comparing `ppynet-0.0.2.tar` & `ppynet-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:25:42.175691 ppynet-0.0.2/
--rw-rw-rw-   0        0        0      555 2024-04-07 21:25:42.175691 ppynet-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 21:25:42.157773 ppynet-0.0.2/PPyNet/
--rw-rw-rw-   0        0        0       34 2024-04-06 17:21:19.000000 ppynet-0.0.2/PPyNet/__init__.py
--rw-rw-rw-   0        0        0     4844 2024-04-07 21:23:27.000000 ppynet-0.0.2/PPyNet/connection.py
--rw-rw-rw-   0        0        0       56 2024-03-27 22:48:22.000000 ppynet-0.0.2/PPyNet/db.py
--rw-rw-rw-   0        0        0     2666 2024-04-07 21:19:15.000000 ppynet-0.0.2/PPyNet/rawws.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:25:42.173691 ppynet-0.0.2/ppynet.egg-info/
--rw-rw-rw-   0        0        0      555 2024-04-07 21:25:42.000000 ppynet-0.0.2/ppynet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-04-07 21:25:42.000000 ppynet-0.0.2/ppynet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:25:42.000000 ppynet-0.0.2/ppynet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-07 21:25:42.000000 ppynet-0.0.2/ppynet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-07 21:25:42.000000 ppynet-0.0.2/ppynet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 21:25:42.176691 ppynet-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-07 21:23:55.000000 ppynet-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:19:54.634364 ppynet-0.0.3/
+-rw-rw-rw-   0        0        0      555 2024-05-22 21:19:54.634364 ppynet-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 21:19:54.618373 ppynet-0.0.3/PPyNet/
+-rw-rw-rw-   0        0        0       76 2024-05-22 16:25:58.000000 ppynet-0.0.3/PPyNet/__init__.py
+-rw-rw-rw-   0        0        0     3459 2024-05-15 05:02:42.000000 ppynet-0.0.3/PPyNet/rawws.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:19:54.632363 ppynet-0.0.3/ppynet.egg-info/
+-rw-rw-rw-   0        0        0      555 2024-05-22 21:19:54.000000 ppynet-0.0.3/ppynet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-05-22 21:19:54.000000 ppynet-0.0.3/ppynet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 21:19:54.000000 ppynet-0.0.3/ppynet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 21:19:54.000000 ppynet-0.0.3/ppynet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 21:19:54.000000 ppynet-0.0.3/ppynet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 21:19:54.634364 ppynet-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-05-22 21:19:43.000000 ppynet-0.0.3/setup.py
```

### Comparing `ppynet-0.0.2/PKG-INFO` & `ppynet-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppynet
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy to use low level websocket based utility package.
 Home-page: UNKNOWN
 Author: Darkodaaa
 Author-email: 
 License: UNKNOWN
 Keywords: python,sockets,connection,utility
 Platform: UNKNOWN
```

### Comparing `ppynet-0.0.2/PPyNet/rawws.py` & `ppynet-0.0.3/PPyNet/rawws.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         """
 
         self.__uri = "wss://ppynet.darkodaaa.one"
         self.__protocol = protocol
         try:
             self.__ws = create_connection(self.__uri)
         except:
-            ConnectionError("Couldn't create to server. Is the server down?")
+            raise ConnectionError("Couldn't create to server. Is the server down?")
 
     def reConnect(self) -> None:
         """
             Reconnect the websocket mostly when it times out.
             Creates a new connection to the server.
 
             Raises:
@@ -58,21 +58,39 @@
         data["protocol"] = self.__protocol
         data["subProtocol"] = protocol
         try:
             return self.__ws.send(json.dumps(data))
         except:
             raise ConnectionError("Sending failed. Is the server down?")
         
-    def receive(self):
+    def receive(self) -> dict:
         """
-            Receive a raw json message from the server and converts it into a dictionary.
+            Receives a raw json message from the server and converts it into a dictionary.
 
             Raises:
                 ConnectionError: When the connection to the server is closed.
 
             Returns: Dict the dictionary containing the data sent by the server.
         """
 
         try:
             return json.loads(self.__ws.recv())
         except:
-            raise ConnectionError("Receive failed, is the server down?")
+            raise ConnectionError("Receive failed. Is the server down?")
+        
+    def request(self, protocol: str, data: dict) -> dict:
+        """
+            Sends a request to the server in a form of send with a protocol and payload.
+            It returns the data recieved right after sending the payload.
+
+            Params:
+                protocol: String the subprotocol to use for the server to handle.
+                data: Dict a dictionary containing all data that is needed for the server to process the given protocol and subprotocol.
+            
+            Raises:
+                ConnectionError: When the connection to the server is closed.
+
+            Returns: Dict the dictionary containing the data sent by the server.
+        """
+        
+        self.send(protocol, data)
+        return self.receive()
```

### Comparing `ppynet-0.0.2/ppynet.egg-info/PKG-INFO` & `ppynet-0.0.3/ppynet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppynet
-Version: 0.0.2
+Version: 0.0.3
 Summary: An easy to use low level websocket based utility package.
 Home-page: UNKNOWN
 Author: Darkodaaa
 Author-email: 
 License: UNKNOWN
 Keywords: python,sockets,connection,utility
 Platform: UNKNOWN
```

### Comparing `ppynet-0.0.2/setup.py` & `ppynet-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'An easy to use low level websocket based utility package.'
 
 # Setting up
 setup(
     name="ppynet",
     version=VERSION,
     author="Darkodaaa",
```

