# Comparing `tmp/yet-another-io-channels-library-0.2.2.tar.gz` & `tmp/yet_another_io_channels_library-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yet-another-io-channels-library-0.2.2.tar", last modified: Mon Nov  5 16:34:14 2018, max compression
+gzip compressed data, was "yet_another_io_channels_library-0.2.3.tar", max compression
```

## Comparing `yet-another-io-channels-library-0.2.2.tar` & `yet_another_io_channels_library-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,8 @@
-drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)       38 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/setup.cfg
-drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/channels/
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)      432 2018-10-25 19:46:44.000000 yet-another-io-channels-library-0.2.2/channels/testing.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)       82 2018-10-25 07:44:24.000000 yet-another-io-channels-library-0.2.2/channels/__init__.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3766 2018-10-25 20:16:38.000000 yet-another-io-channels-library-0.2.2/channels/channel.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     2793 2018-11-05 16:28:42.000000 yet-another-io-channels-library-0.2.2/channels/poller.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)      876 2018-11-05 16:31:51.000000 yet-another-io-channels-library-0.2.2/setup.py
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     5272 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/PKG-INFO
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     3769 2018-11-05 16:30:22.000000 yet-another-io-channels-library-0.2.2/README.md
-drwxr-xr-x   0 aragaer   (1000) aragaer   (1000)        0 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/yet_another_io_channels_library.egg-info/
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)        9 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/yet_another_io_channels_library.egg-info/top_level.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)        1 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/yet_another_io_channels_library.egg-info/dependency_links.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)      318 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/yet_another_io_channels_library.egg-info/SOURCES.txt
--rw-r--r--   0 aragaer   (1000) aragaer   (1000)     5272 2018-11-05 16:34:14.000000 yet-another-io-channels-library-0.2.2/yet_another_io_channels_library.egg-info/PKG-INFO
+-rw-r--r--   0        0        0     1071 2018-10-14 15:23:38.622748 yet_another_io_channels_library-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3769 2018-11-05 16:30:22.038313 yet_another_io_channels_library-0.2.3/README.md
+-rw-r--r--   0        0        0       82 2018-10-25 07:44:24.040450 yet_another_io_channels_library-0.2.3/channels/__init__.py
+-rw-r--r--   0        0        0     3766 2024-05-26 21:18:36.103891 yet_another_io_channels_library-0.2.3/channels/channel.py
+-rw-r--r--   0        0        0     2781 2024-05-26 21:18:37.494891 yet_another_io_channels_library-0.2.3/channels/poller.py
+-rw-r--r--   0        0        0      432 2024-05-26 20:52:25.346757 yet_another_io_channels_library-0.2.3/channels/testing.py
+-rw-r--r--   0        0        0      434 2024-05-26 21:22:24.778910 yet_another_io_channels_library-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 yet_another_io_channels_library-0.2.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yet-another-io-channels-library-0.2.2/channels/channel.py` & `yet_another_io_channels_library-0.2.3/channels/channel.py`

 * *Files identical despite different names*

### Comparing `yet-another-io-channels-library-0.2.2/channels/poller.py` & `yet_another_io_channels_library-0.2.3/channels/poller.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         result = []
         for fd, event in self._poll.poll(timeout):
             _LOGGER.debug("Got event %s on fd %d", _event_to_str(event), fd)
             if fd in self._channels:
                 channel = self._channels[fd]
                 try:
                     if channel.buffering == 'line':
-                        result.extend([(data, channel)
-                                       for data in self._readlines(channel)])
+                        for data in self._readlines(channel):
+                            result.append((data, channel))
                     else:
                         result.append((channel.read(), channel))
                 except EndpointClosedException:
                     result.append((b'', channel))
                     self._unregister(channel, fd)
             elif event & select.POLLIN:
                 server = self._servers[fd]
```

### Comparing `yet-another-io-channels-library-0.2.2/README.md` & `yet_another_io_channels_library-0.2.3/README.md`

 * *Files identical despite different names*

