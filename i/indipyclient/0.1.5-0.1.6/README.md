# Comparing `tmp/indipyclient-0.1.5.tar.gz` & `tmp/indipyclient-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.5.tar` & `indipyclient-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.5/LICENSE
--rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.5/README.md
--rw-r--r--   0        0        0      416 2024-05-19 14:24:30.000000 indipyclient-0.1.5/indipyclient/__init__.py
--rw-r--r--   0        0        0     3663 2024-05-16 10:28:14.000000 indipyclient-0.1.5/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.5/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    21226 2024-05-15 17:27:54.000000 indipyclient-0.1.5/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.5/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.5/indipyclient/console/windows.py
--rw-r--r--   0        0        0    26848 2024-05-15 10:33:05.000000 indipyclient-0.1.5/indipyclient/events.py
--rw-r--r--   0        0        0    32802 2024-05-19 14:22:05.000000 indipyclient-0.1.5/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.1.5/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.5/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-19 14:24:11.000000 indipyclient-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.6/README.md
+-rw-r--r--   0        0        0      332 2024-05-26 20:50:36.000000 indipyclient-0.1.6/indipyclient/__init__.py
+-rw-r--r--   0        0        0     4801 2024-05-24 10:02:09.000000 indipyclient-0.1.6/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.6/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19750 2024-05-24 09:23:15.000000 indipyclient-0.1.6/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.6/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.6/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    27266 2024-05-22 18:24:53.000000 indipyclient-0.1.6/indipyclient/events.py
+-rw-r--r--   0        0        0    33860 2024-05-24 10:05:56.000000 indipyclient-0.1.6/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.1.6/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.6/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-26 20:51:25.000000 indipyclient-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.6/PKG-INFO
```

### Comparing `indipyclient-0.1.5/LICENSE` & `indipyclient-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.5/README.md` & `indipyclient-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.5/indipyclient/__main__.py` & `indipyclient-0.1.6/indipyclient/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,67 @@
 
 python3 -m indipyclient --help
 
 For a description of options
 """
 
 
-import sys, argparse, asyncio, pathlib
+import sys, argparse, asyncio, pathlib, logging
 
-import logging
-logger = logging.getLogger('indipyclient')
+logger = logging.getLogger()
+
+# logger is the root logger, with level and handler set here
+# by the arguments given. If no logging option is given, it
+# has a NullHandler() added
 
 from . import version
 
 from .console.consoleclient import ConsoleClient, ConsoleControl
 
 
 async def runclient(client, control):
     await asyncio.gather(client.asyncrun(), control.asyncrun())
 
 
+def setlogging(client, level, logfile):
+    """Sets the logging level and logfile, returns the level on success, None on failure.
+       level should be an integer, one of 1, 2, 3 or 4."""
+
+    # loglevel:1 Information and error messages only
+    # loglevel:2 log vector tags without members or contents
+    # loglevel:3 log vectors and members - but not BLOB contents
+    # loglevel:4 log vectors and all contents
+
+    try:
+        if not level in (1, 2, 3, 4):
+            return
+        logfile = pathlib.Path(logfile).expanduser().resolve()
+
+        if level == 4:
+            logger.setLevel(logging.DEBUG)
+            client.debug_verbosity(3)
+        elif level == 3:
+            logger.setLevel(logging.DEBUG)
+            client.debug_verbosity(2)
+        elif level == 2:
+            logger.setLevel(logging.DEBUG)
+            client.debug_verbosity(1)
+        elif level == 1:
+            logger.setLevel(logging.INFO)
+            client.debug_verbosity(0)
+            # If logging debug not enabled, reduce traceback info
+            sys.tracebacklimit = 0
+
+        fh = logging.FileHandler(logfile)
+        logger.addHandler(fh)
+    except Exception:
+        return
+    return level
+
+
 def main():
     """The commandline entry point to run the terminal client."""
 
     parser = argparse.ArgumentParser(usage="indipyclient [options]",
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description="Terminal client to communicate to an INDI service.",
                                      epilog="""The BLOB's folder can also be set from within the session.
@@ -55,46 +94,40 @@
         else:
             if not blobfolder.is_dir():
                 print("Error: If given, the BLOB's folder should be an existing directory")
                 return 1
     else:
         blobfolder = None
 
+    if args.loglevel:
+        if args.loglevel not in ("1", "2", "3", "4"):
+            print("Error: If given, the loglevel should be 1, 2, 3 or 4")
+            return 1
+
     # ConsoleClient is a subclass of IPyClient, with its rxevent(event) method created
     # to add events to a queue. First a queue is created and passed into ConsoleClient
     eventque = asyncio.Queue(maxsize=4)
 
     # On receiving an event, the client appends it into eventque
     client = ConsoleClient(indihost=args.host, indiport=args.port, eventque=eventque)
 
-    # Monitors eventque and acts on the events, creates the console screens
-    # and calls the send vector methods of client to transmit data
-    control = ConsoleControl(client, blobfolder=blobfolder)
-
-    loglevel = 0
-
     if args.loglevel and args.logfile:
-        try:
-            loglevel = int(args.loglevel)
-            if loglevel not in (1,2,3,4):
-                print("Error: If given, the loglevel should be 1, 2, 3 or 4")
-                return 1
-            level = control.setlogging(loglevel, args.logfile)
-            if level != loglevel:
-                print("Error: Failed to set logging")
-                return 1
-        except Exception:
-            print("Error: If given, the loglevel should be 1, 2, 3 or 4")
+        loglevel = int(args.loglevel)
+        level = setlogging(client, loglevel, args.logfile)
+        if level != loglevel:
+            print("Error: Failed to set logging")
             return 1
-
-    if loglevel < 2:
-        # If logging debug not enabled, reduce traceback info
-        sys.tracebacklimit = 0
+    else:
+        logger.addHandler(logging.NullHandler())
 
     try:
+        # Monitors eventque and acts on the events, creates the console screens
+        # and calls the send vector methods of client to transmit data
+        control = ConsoleControl(client, blobfolder=blobfolder)
+
         asyncio.run(runclient(client, control))
     finally:
         # clear curses setup
         control.console_reset()
 
     return 0
```

### Comparing `indipyclient-0.1.5/indipyclient/console/consoleclient.py` & `indipyclient-0.1.6/indipyclient/console/consoleclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import asyncio, sys, traceback, pathlib
 
 import curses
 
 import logging
-logger = logging.getLogger('indipyclient')
+logger = logging.getLogger(__name__)
 
 from ..ipyclient import IPyClient
 from ..events import (delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector,
                      setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector, Message, VectorTimeOut)
 
 from . import windows
 from . import widgets
@@ -88,48 +88,15 @@
         # list of known device names, this is needed to send
         # BLOB's enabled
         self.devicenames = []
 
         # BLOBfiles, is a dictionary of {(devicename,vectorname,membername):filepath}
         self.BLOBfiles = {}
 
-    def setlogging(self, level, logfile):
-        """Sets the logging level and logfile, returns the level, which will be None on failure.
-           As default, no logging is enabled. If logging is required, this can be called, level
-           should be an integer, one of 1, 2, 3 or 4.
-           Be warned, there is no logfile rotation, files can become large.
-           Note: it may be useful in another terminal to try tail -f logfile"""
-
-        # loglevel:1 Information and error messages only,  -> error
-        # loglevel:2 log vector tags without members or contents  -> warning
-        # loglevel:3 log vectors and members - but not BLOB contents  -> info
-        # loglevel:4 log vectors and all contents   -> debug
-
-        try:
-            if not level in (1, 2, 3, 4):
-                return None
-            logfile = pathlib.Path(logfile).expanduser().resolve()
-
-            if level == 4:
-                logger.setLevel(logging.DEBUG)
-                self.client.debug_verbosity(3)
-            elif level == 3:
-                logger.setLevel(logging.DEBUG)
-                self.client.debug_verbosity(2)
-            elif level == 2:
-                logger.setLevel(logging.DEBUG)
-                self.client.debug_verbosity(1)
-            elif level == 1:
-                logger.setLevel(logging.INFO)
-
-            fh = logging.FileHandler(logfile)
-            logger.addHandler(fh)
-        except Exception:
-            return
-        return level
+
 
 
     def color(self, state):
         "Returns curses.color_pair given a state"
         if not curses.has_colors():
             return curses.color_pair(0)
         state = state.lower()
```

### Comparing `indipyclient-0.1.5/indipyclient/console/widgets.py` & `indipyclient-0.1.6/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.5/indipyclient/console/windows.py` & `indipyclient-0.1.6/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.5/indipyclient/events.py` & `indipyclient-0.1.6/indipyclient/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     def __init__(self, device, vector):
         self.device = device
         self.devicename = self.device.devicename
         self.vector = vector
         self.vectorname = self.vector.name
         self.timestamp = datetime.now(tz=timezone.utc)
         self.eventtype = "TimeOut"
+        self.root = None
 
 
 class Event:
     "Parent class for events received from drivers"
     def __init__(self, root, device, client):
         self.device = device
         self._client = client
@@ -82,14 +83,25 @@
         if device is None:
             # state wide message
             client.messages.appendleft( (self.timestamp, self.message) )
         else:
             device.messages.appendleft( (self.timestamp, self.message) )
 
 
+class getProperties(Event):
+    """This may have a device and name, both may be None
+       But there may still be a devicename and vectorname for an unknown device"""
+
+    def __init__(self, root, device, client):
+        super().__init__(root, device, client)
+        self.eventtype = "getProperties"
+        self.devicename = root.get("device")
+        self.vectorname = root.get("name")
+
+
 class delProperty(Event):
     """The remote driver is instructing the client to delete either a device or a vector property.
        This contains attribute vectorname, if it is None, then the whole device is to be deleted.
        A 'message' attribute contains any message sent by the client with this instruction.
        This event will automatically set the appropriate enable flag to False in the effected
        device and vectors."""
```

### Comparing `indipyclient-0.1.5/indipyclient/ipyclient.py` & `indipyclient-0.1.6/indipyclient/ipyclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-import os, sys, collections, threading, asyncio, pathlib, time, copy
+import os, sys, collections, threading, asyncio, time, copy
 
 from time import sleep
 
 from datetime import datetime, timezone
 
 from base64 import standard_b64encode
 
@@ -26,15 +26,16 @@
         b'defLightVector',
         b'setLightVector',
         b'defTextVector',
         b'setTextVector',
         b'defNumberVector',
         b'setNumberVector',
         b'defBLOBVector',
-        b'setBLOBVector'
+        b'setBLOBVector',
+        b'getProperties'       # for snooping
        )
 
 DEFTAGS = ( 'defSwitchVector',
             'defLightVector',
             'defTextVector',
             'defNumberVector',
             'defBLOBVector'
@@ -145,39 +146,45 @@
         self._stop = False
         # this is set to True when asyncrun is finished
         self.stopped = False
 
         # Indicates how verbose the debug xml logs will be when created.
         self._verbose = 1
 
+        # Enables reports, by adding INFO logs to client messages
+        self.enable_reports = True
+
 
     def debug_verbosity(self, verbose):
         """Set how verbose the debug xml logs will be when created.
+           0 no xml logs will be generated
            1 for transmitted/received vector tags only,
            2 for transmitted/received vectors, members and contents (apart from BLOBs)
            3 for all transmitted/received data including BLOBs."""
-        if verbose not in (1,2,3):
+        if verbose not in (0,1,2,3):
             raise ValueError
         self._verbose = verbose
 
 
     def shutdown(self):
         "Shuts down the client"
         self._stop = True
 
     def report(self, message):
-        """This injects a message into the received data, which will be
-           picked up by the rxevent method. It is a way to set a message
-           on to your client display, in the same way messages come from
-           the INDI service. If logging is enabled the message will also
-           be logged at level INFO"""
+        """If logging is enabled message will be logged at level INFO.
+           If self.enable_reports is True, the message will be injected into
+           the received data, which will be picked up by the rxevent method.
+           It is a way to set a message on to your client display, in the
+           same way messages come from the INDI service."""
         try:
+            logger.info(message)
+            if not self.enable_reports:
+                return
             timestamp = datetime.now(tz=timezone.utc)
             timestamp = timestamp.replace(tzinfo=None)
-            logger.info(message)
             root = ET.fromstring(f"<message timestamp=\"{timestamp.isoformat(sep='T')}\" message=\"{message}\" />")
             # and place root into readerque
             try:
                 self.readerque.put_nowait(root)
             except asyncio.QueueFull:
                 # The queue is full, something may be wrong
                 # discard this data and continue
@@ -203,31 +210,31 @@
                 self.tx_timer = None
                 self.idle_timer = time.time()
                 t1 = None
                 t2 = None
                 t3 = None
                 try:
                     # start by openning a connection
-                    self.report("Attempting to connect")
+                    self.report(f"Attempting to connect to {self.indihost}:{self.indiport}")
                     reader, writer = await asyncio.open_connection(self.indihost, self.indiport)
                     self.connected = True
                     self.messages.clear()
                     # clear devices etc
                     self.clear()
                     self.report(f"Connected to {self.indihost}:{self.indiport}")
                     t1 = asyncio.create_task(self._run_tx(writer))
                     t2 = asyncio.create_task(self._run_rx(reader))
                     t3 = asyncio.create_task(self._check_alive(writer))
                     await asyncio.gather(t1, t2, t3)
                 except ConnectionRefusedError:
                     self.report(f"Connection refused on {self.indihost}:{self.indiport}")
                 except ConnectionError:
-                    self.report("Connection Lost")
+                    self.report(f"Connection Lost on {self.indihost}:{self.indiport}")
                 except Exception:
-                    logger.exception("Connection Error")
+                    logger.exception(f"Connection Error on {self.indihost}:{self.indiport}")
                     self.report("Connection failed")
                 self._clear_connection()
                 # connection has failed, ensure all tasks are done
                 if t1:
                     while not t1.done():
                         await asyncio.sleep(0)
                 if t2:
@@ -293,15 +300,16 @@
             raise
         finally:
             self.connected = False
 
 
     def _logtx(self, txdata):
         "log tx data with level debug, and detail depends on self._verbose"
-
+        if not self._verbose:
+            return
         startlog = "TX:: "
         if self._verbose == 3:
             binarydata = ET.tostring(txdata)
             logger.debug(startlog + binarydata.decode())
         elif self._verbose == 2:
             data = copy.deepcopy(txdata)
             tag = data.tag
@@ -357,14 +365,16 @@
             self.writerque.clear()
         except Exception:
             logger.exception("Exception report from IPyClient._run_tx method")
             raise
 
     def _logrx(self, rxdata):
         "log rx data to file"
+        if not self._verbose:
+            return
         startlog = "RX:: "
         if self._verbose == 3:
             binarydata = ET.tostring(rxdata)
             logger.debug(startlog + binarydata.decode())
         elif self._verbose == 2:
             data = copy.deepcopy(rxdata)
             tag = data.tag
@@ -524,29 +534,35 @@
                 # block any other thread from accessing data until update is done
                 try:
                     with threading.Lock():
                         if devicename is None:
                             if root.tag == "message":
                                 # create event
                                 event = events.Message(root, None, self)
+                            elif root.tag == "getProperties":
+                                # create event
+                                event = events.getProperties(root, None, self)
                             else:
-                                # if no devicename and not message, do nothing
+                                # if no devicename and not message or getProperties, do nothing
                                 continue
                         elif devicename in self:
                             # device is known about
                             device = self[devicename]
                             event = device.rxvector(root)
+                        elif root.tag == "getProperties":
+                            # device is not known about, but this is a getProperties, so raise an event
+                            event = events.getProperties(root, None, self)
                         elif root.tag in DEFTAGS:
                             # device not known, but a def is received
                             newdevice = _Device(devicename, self)
                             event = newdevice.rxvector(root)
                             # no error has occurred, so add this device to self.data
                             self.data[devicename] = newdevice
                         else:
-                            # device not known, not a def, so ignore it
+                            # device not known, not a def or getProperties, so ignore it
                             continue
                 except ParseException as pe:
                     # if a ParseException is raised, it is because received data is malformed
                     self.report(str(pe))
                     continue
                 finally:
                     self.readerque.task_done()
@@ -776,14 +792,16 @@
                 return events.defNumberVector(root, self, self._client)
             elif root.tag == "setNumberVector":
                 return events.setNumberVector(root, self, self._client)
             elif root.tag == "defBLOBVector":
                 return events.defBLOBVector(root, self, self._client)
             elif root.tag == "setBLOBVector":
                 return events.setBLOBVector(root, self, self._client)
+            elif root.tag == "getProperties":
+                return events.getProperties(root, self, self._client)
             else:
                 raise ParseException("Unrecognised tag received")
         except ParseException:
             raise
         except Exception:
             logger.exception("Exception report from IPyClient.rxvector method")
             raise ParseException("Error while attempting to parse received data")
```

### Comparing `indipyclient-0.1.5/indipyclient/propertymembers.py` & `indipyclient-0.1.6/indipyclient/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.5/indipyclient/propertyvectors.py` & `indipyclient-0.1.6/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.5/pyproject.toml` & `indipyclient-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.5"
+version = "0.1.6"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.5/PKG-INFO` & `indipyclient-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

