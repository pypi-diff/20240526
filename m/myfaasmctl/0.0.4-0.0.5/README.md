# Comparing `tmp/myfaasmctl-0.0.4.tar.gz` & `tmp/myfaasmctl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfaasmctl-0.0.4.tar", last modified: Tue May 21 14:32:09 2024, max compression
+gzip compressed data, was "myfaasmctl-0.0.5.tar", last modified: Sun May 26 12:15:33 2024, max compression
```

## Comparing `myfaasmctl-0.0.4.tar` & `myfaasmctl-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/
--rw-r--r--   0 root         (0) root         (0)    11343 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1341 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.014449 myfaasmctl-0.0.4/faasmctl/
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.014449 myfaasmctl-0.0.4/faasmctl/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3438 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/bin/gen_proto_files.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.018449 myfaasmctl-0.0.4/faasmctl/tasks/
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/cli.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/delete.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/deploy.py
--rw-r--r--   0 root         (0) root         (0)      656 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/flush.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/generate.py
--rw-r--r--   0 root         (0) root         (0)     3454 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/invoke.py
--rw-r--r--   0 root         (0) root         (0)     2192 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/logs.py
--rw-r--r--   0 root         (0) root         (0)    10483 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/monitor.py
--rw-r--r--   0 root         (0) root         (0)     1373 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/restart.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/scale.py
--rw-r--r--   0 root         (0) root         (0)      808 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/status.py
--rw-r--r--   0 root         (0) root         (0)     1346 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/tasks/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.018449 myfaasmctl-0.0.4/faasmctl/util/
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/backend.py
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/batch.py
--rw-r--r--   0 root         (0) root         (0)    14750 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/compose.py
--rw-r--r--   0 root         (0) root         (0)     2464 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/config.py
--rw-r--r--   0 root         (0) root         (0)     5829 2024-05-21 14:28:54.000000 myfaasmctl-0.0.4/faasmctl/util/deploy.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/docker.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/env.py
--rw-r--r--   0 root         (0) root         (0)      670 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/faasm.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/flush.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.018449 myfaasmctl-0.0.4/faasmctl/util/gen_proto/
--rw-r--r--   0 root         (0) root         (0)     8690 2024-05-10 02:54:00.000000 myfaasmctl-0.0.4/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5799 2024-05-10 02:54:00.000000 myfaasmctl-0.0.4/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5795 2024-05-10 02:57:43.000000 myfaasmctl-0.0.4/faasmctl/util/invoke.py
--rw-r--r--   0 root         (0) root         (0)    11303 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/k8s.py
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/message.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/network.py
--rw-r--r--   0 root         (0) root         (0)     6569 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/planner.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/random.py
--rw-r--r--   0 root         (0) root         (0)      688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/restart.py
--rw-r--r--   0 root         (0) root         (0)     1371 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/results.py
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/time.py
--rw-r--r--   0 root         (0) root         (0)     2017 2024-05-10 02:02:06.000000 myfaasmctl-0.0.4/faasmctl/util/upload.py
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-10 02:58:15.000000 myfaasmctl-0.0.4/faasmctl/util/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/myfaasmctl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1341 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 14:32:09.000000 myfaasmctl-0.0.4/myfaasmctl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      692 2024-05-21 14:31:40.000000 myfaasmctl-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-21 14:32:09.022449 myfaasmctl-0.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.401131 myfaasmctl-0.0.5/faasmctl/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.401131 myfaasmctl-0.0.5/faasmctl/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     4533 2024-05-26 09:08:38.000000 myfaasmctl-0.0.5/faasmctl/bin/gen_proto_files.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.405130 myfaasmctl-0.0.5/faasmctl/tasks/
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/cli.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/delete.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      656 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/flush.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/generate.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/logs.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2024-05-26 09:36:56.000000 myfaasmctl-0.0.5/faasmctl/tasks/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/restart.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/scale.py
+-rw-r--r--   0 root         (0) root         (0)      808 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/status.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/tasks/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/faasmctl/util/
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/backend.py
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/batch.py
+-rw-r--r--   0 root         (0) root         (0)    14750 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/compose.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     5829 2024-05-21 14:28:54.000000 myfaasmctl-0.0.5/faasmctl/util/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/docker.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/env.py
+-rw-r--r--   0 root         (0) root         (0)      670 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/faasm.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/flush.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/faasmctl/util/gen_proto/
+-rw-r--r--   0 root         (0) root         (0)    12287 2024-05-26 09:01:33.000000 myfaasmctl-0.0.5/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2024-05-26 09:01:33.000000 myfaasmctl-0.0.5/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5795 2024-05-10 02:57:43.000000 myfaasmctl-0.0.5/faasmctl/util/invoke.py
+-rw-r--r--   0 root         (0) root         (0)    11303 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/k8s.py
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/message.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/network.py
+-rw-r--r--   0 root         (0) root         (0)     7290 2024-05-26 10:29:44.000000 myfaasmctl-0.0.5/faasmctl/util/planner.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/random.py
+-rw-r--r--   0 root         (0) root         (0)      688 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/restart.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/results.py
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/time.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2024-05-10 02:02:06.000000 myfaasmctl-0.0.5/faasmctl/util/upload.py
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-26 12:14:43.000000 myfaasmctl-0.0.5/faasmctl/util/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/myfaasmctl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1341 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-26 12:15:33.000000 myfaasmctl-0.0.5/myfaasmctl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      692 2024-05-26 12:14:33.000000 myfaasmctl-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-26 12:15:33.409130 myfaasmctl-0.0.5/setup.cfg
```

### Comparing `myfaasmctl-0.0.4/LICENSE.md` & `myfaasmctl-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/PKG-INFO` & `myfaasmctl-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfaasmctl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `myfaasmctl-0.0.4/README.md` & `myfaasmctl-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/bin/gen_proto_files.py` & `myfaasmctl-0.0.5/faasmctl/bin/gen_proto_files.py`

 * *Files 27% similar despite different names*

```diff
@@ -80,15 +80,23 @@
         p_bin,
         "--proto_path={}".format(code_dir),
         "--python_out={}".format(code_dir),
         "{}/src/planner/planner.proto".format(code_dir),
         "{}/src/proto/faabric.proto".format(code_dir),
     ]
     protoc_cmd = " ".join(protoc_cmd)
+    """
+    protoc_cmd Command locally
+    /root/.conan/data/protobuf/3.20.0/_/_/build/5d8030e3dac4d78aba1403fc0ec4c411cab803ee/build_subfolder/bin/protoc --proto_path=/usr/local/code/faasm/faabric --python_out=/usr/local/code/faasm/faabric /usr/local/code/faasm/faabric/src/planner/planner.proto /usr/local/code/faasm/faabric/src/proto/faabric.proto
+    """
     docker_cmd = "{} bash -c '{}'".format(docker_exec_prefix, protoc_cmd)
+    """
+    docker_cmd Command locally
+    docker exec faasm-154600-faasm-cli-1 bash -c "/root/.conan/data/protobuf/3.20.0/_/_/build/5d8030e3dac4d78aba1403fc0ec4c411cab803ee/build_subfolder/bin/protoc --proto_path=/usr/local/code/faasm/faabric --python_out=/usr/local/code/faasm/faabric /usr/local/code/faasm/faabric/src/planner/planner.proto /usr/local/code/faasm/faabric/src/proto/faabric.proto"
+    """
     run(docker_cmd, shell=True, check=True)
 
     # Finally, copy the generated protobuf files to the desired location
     for proto_file in PROTO_FILES:
         if "planner" in proto_file:
             proto_ctr_path = join(code_dir, "src", "planner", proto_file)
         else:
@@ -96,14 +104,18 @@
         proto_faasmctl_path = join(GEN_PROTO_DIR, proto_file)
 
         docker_cp_cmd = "docker cp {}:{} {}".format(
             tmp_ctr_name, proto_ctr_path, proto_faasmctl_path
         )
         run(docker_cp_cmd, shell=True, check=True)
 
+    """
+    docker cp faasm-154600-faasm-cli-1:/usr/local/code/faasm/faabric/src/planner/planner_pb2.py /pvol/runtime/faasmctl/faasmctl/util/gen_proto/planner_pb2.py
+    docker cp faasm-154600-faasm-cli-1:/usr/local/code/faasm/faabric/src/proto/faabric_pb2.py /pvol/runtime/faasmctl/faasmctl/util/gen_proto/faabric_pb2.py
+    """
     # Delete container
     run("docker rm -f {}".format(tmp_ctr_name), shell=True, check=True)
     print("Done generating protobuf files!")
 
 
 if __name__ == "__main__":
     clean = len(argv) == 2 and argv[1] == "--clean"
```

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/cli.py` & `myfaasmctl-0.0.5/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/delete.py` & `myfaasmctl-0.0.5/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/deploy.py` & `myfaasmctl-0.0.5/faasmctl/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/flush.py` & `myfaasmctl-0.0.5/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/invoke.py` & `myfaasmctl-0.0.5/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/logs.py` & `myfaasmctl-0.0.5/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/monitor.py` & `myfaasmctl-0.0.5/faasmctl/tasks/monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from faasmctl.util.config import (
     get_faasm_ini_file,
     get_faasm_ini_value,
     get_faasm_planner_host_port,
 )
 from faasmctl.util.faasm import FAASM_CLI_IMAGE
-from faasmctl.util.planner import get_available_hosts, get_in_fligh_apps
+from faasmctl.util.planner import get_available_hosts, get_in_fligh_apps, get_function_metrics
+from faasmctl.util.gen_proto.planner_pb2 import (
+    FunctionMetricResponse,
+)
 from invoke import task
 from signal import SIGINT, signal
 from subprocess import run
 from sys import exit as sys_exit
 from time import sleep
 
 CTR_NAME_BASE = "faasm-is-migratable-workon"
@@ -311,7 +314,39 @@
     """
     Monitor the in-flight apps and host occupation in the planner
     """
     signal(SIGINT, signal_handler)
     while True:
         print_planner_resources(policy)
         sleep(poll_period_sec)
+
+# Function to print the metrics
+def print_metrics(metric_response: FunctionMetricResponse):
+    # Print ChainedFunctionsMetricsRes
+    print("Chained Functions Metrics:")
+    for chained_metric in metric_response.chainedMetrics:
+        print(f"Name: {chained_metric.name}")
+        print(f"Throughput: {chained_metric.throughput}")
+        print(f"Process Latency: {chained_metric.processLatency}")
+        print("-" * 20)
+    
+    # Print FunctionMetricsRes
+    print("Function Metrics:")
+    for function_metric in metric_response.functionMetrics:
+        print(f"Name: {function_metric.name}")
+        print(f"Throughput: {function_metric.throughput}")
+        print(f"Process Latency: {function_metric.processLatency}")
+        print(f"Average Waiting Time: {function_metric.averageWaitingTime}")
+        print(f"Host IP: {function_metric.hostIp}")
+        print(f"Lock Congestion Time: {function_metric.lockCongestionTime}")
+        print(f"Lock Hold Time: {function_metric.lockHoldTime}")
+        print("-" * 20)
+
+@task
+def metrics(ctx):
+    """
+    Retrive the function state distribution and function metrics 
+    """
+    host, port = get_faasm_planner_host_port(get_faasm_ini_file())
+    metric = get_function_metrics()
+
+    print_metrics(metric)
```

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/restart.py` & `myfaasmctl-0.0.5/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/scale.py` & `myfaasmctl-0.0.5/faasmctl/tasks/scale.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/status.py` & `myfaasmctl-0.0.5/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/tasks/upload.py` & `myfaasmctl-0.0.5/faasmctl/tasks/upload.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/compose.py` & `myfaasmctl-0.0.5/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/config.py` & `myfaasmctl-0.0.5/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/deploy.py` & `myfaasmctl-0.0.5/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/docker.py` & `myfaasmctl-0.0.5/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/faasm.py` & `myfaasmctl-0.0.5/faasmctl/util/faasm.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/flush.py` & `myfaasmctl-0.0.5/faasmctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/gen_proto/faabric_pb2.py` & `myfaasmctl-0.0.5/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17src/proto/faabric.proto\x12\x07\x66\x61\x61\x62ric\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\xeb\x02\n\x13\x42\x61tchExecuteRequest\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x10\n\x08\x66unction\x18\x04 \x01(\t\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.faabric.BatchExecuteRequest.BatchExecuteType\x12\x13\n\x0bsnapshotKey\x18\x06 \x01(\t\x12\"\n\x08messages\x18\x07 \x03(\x0b\x32\x10.faabric.Message\x12\x0f\n\x07subType\x18\x08 \x01(\x05\x12\x13\n\x0b\x63ontextData\x18\t \x01(\x0c\x12\x12\n\nsingleHost\x18\n \x01(\x08\x12\x16\n\x0esingleHostHint\x18\x0b \x01(\x08\"L\n\x10\x42\x61tchExecuteType\x12\r\n\tFUNCTIONS\x10\x00\x12\x0b\n\x07THREADS\x10\x01\x12\r\n\tPROCESSES\x10\x02\x12\r\n\tMIGRATION\x10\x03\"\x83\x01\n\x19\x42\x61tchExecuteRequestStatus\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x10\n\x08\x66inished\x18\x02 \x01(\x08\x12(\n\x0emessageResults\x18\x03 \x03(\x0b\x32\x10.faabric.Message\x12\x1b\n\x13\x65xpectedNumMessages\x18\x04 \x01(\x05\"1\n\rHostResources\x12\r\n\x05slots\x18\x01 \x01(\x05\x12\x11\n\tusedSlots\x18\x02 \x01(\x05\"}\n\x16\x46unctionStatusResponse\x12>\n\x06status\x18\x01 \x01(\x0e\x32..faabric.FunctionStatusResponse.FunctionStatus\"#\n\x0e\x46unctionStatus\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\xb6\x08\n\x07Message\x12\n\n\x02id\x18\x01 \x01(\x05\x12\r\n\x05\x61ppId\x18\x02 \x01(\x05\x12\x0e\n\x06\x61ppIdx\x18\x03 \x01(\x05\x12\x10\n\x08mainHost\x18\x04 \x01(\t\x12*\n\x04type\x18\x05 \x01(\x0e\x32\x1c.faabric.Message.MessageType\x12\x0c\n\x04user\x18\x06 \x01(\t\x12\x10\n\x08\x66unction\x18\x07 \x01(\t\x12\x1d\n\tinputData\x18\x08 \x01(\x0cR\ninput_data\x12\x1f\n\noutputData\x18\t \x01(\tR\x0boutput_data\x12\x0f\n\x07\x66uncPtr\x18\n \x01(\x05\x12\x13\n\x0breturnValue\x18\x0b \x01(\x05\x12\x13\n\x0bsnapshotKey\x18\x0c \x01(\t\x12 \n\x0estartTimestamp\x18\x0e \x01(\x03R\x08start_ts\x12\x11\n\tresultKey\x18\x0f \x01(\t\x12\x17\n\x0f\x65xecutesLocally\x18\x10 \x01(\x08\x12\x11\n\tstatusKey\x18\x11 \x01(\t\x12\x14\n\x0c\x65xecutedHost\x18\x12 \x01(\t\x12\"\n\x0f\x66inishTimestamp\x18\x13 \x01(\x03R\tfinish_ts\x12\x18\n\x08isPython\x18\x15 \x01(\x08R\x06python\x12\x1b\n\npythonUser\x18\x18 \x01(\tR\x07py_user\x12\x1f\n\x0epythonFunction\x18\x19 \x01(\tR\x07py_func\x12\x13\n\x0bpythonEntry\x18\x1a \x01(\t\x12\x0f\n\x07groupId\x18\x1b \x01(\x05\x12\x10\n\x08groupIdx\x18\x1c \x01(\x05\x12\x11\n\tgroupSize\x18\x1d \x01(\x05\x12\x12\n\x05isMpi\x18\x1e \x01(\x08R\x03mpi\x12\x12\n\nmpiWorldId\x18\x1f \x01(\x05\x12\x0f\n\x07mpiRank\x18  \x01(\x05\x12$\n\x0cmpiWorldSize\x18! \x01(\x05R\x0empi_world_size\x12\x0f\n\x07\x63mdline\x18\" \x01(\t\x12*\n\x0frecordExecGraph\x18# \x01(\x08R\x11record_exec_graph\x12\x15\n\rchainedMsgIds\x18$ \x03(\x05\x12\x46\n\x13intExecGraphDetails\x18% \x03(\x0b\x32).faabric.Message.IntExecGraphDetailsEntry\x12@\n\x10\x65xecGraphDetails\x18& \x03(\x0b\x32&.faabric.Message.ExecGraphDetailsEntry\x1a:\n\x18IntExecGraphDetailsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x37\n\x15\x45xecGraphDetailsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"7\n\x0bMessageType\x12\x08\n\x04\x43\x41LL\x10\x00\x12\x08\n\x04KILL\x10\x01\x12\t\n\x05\x45MPTY\x10\x02\x12\t\n\x05\x46LUSH\x10\x03\"7\n\x0cStateRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"Q\n\x11StateChunkRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x04\x12\x11\n\tchunkSize\x18\x04 \x01(\x04\"8\n\rStateResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"D\n\tStatePart\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"A\n\x11StateSizeResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x11\n\tstateSize\x18\x03 \x01(\x04\"B\n\x14StateAppendedRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0f\n\x07nValues\x18\x03 \x01(\r\"\x8f\x01\n\x15StateAppendedResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12<\n\x06values\x18\x03 \x03(\x0b\x32,.faabric.StateAppendedResponse.AppendedValue\x1a\x1d\n\rAppendedValue\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"e\n\x13PointToPointMessage\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x0f\n\x07sendIdx\x18\x03 \x01(\x05\x12\x0f\n\x07recvIdx\x18\x04 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\xe6\x01\n\x14PointToPointMappings\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x43\n\x08mappings\x18\x03 \x03(\x0b\x32\x31.faabric.PointToPointMappings.PointToPointMapping\x1ai\n\x13PointToPointMapping\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x11\n\tmessageId\x18\x02 \x01(\x05\x12\x0e\n\x06\x61ppIdx\x18\x03 \x01(\x05\x12\x10\n\x08groupIdx\x18\x04 \x01(\x05\x12\x0f\n\x07mpiPort\x18\x05 \x01(\x05\"f\n\x10PendingMigration\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x10\n\x08groupIdx\x18\x03 \x01(\x05\x12\x0f\n\x07srcHost\x18\x04 \x01(\t\x12\x0f\n\x07\x64stHost\x18\x05 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17src/proto/faabric.proto\x12\x07\x66\x61\x61\x62ric\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\xeb\x02\n\x13\x42\x61tchExecuteRequest\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x10\n\x08\x66unction\x18\x04 \x01(\t\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.faabric.BatchExecuteRequest.BatchExecuteType\x12\x13\n\x0bsnapshotKey\x18\x06 \x01(\t\x12\"\n\x08messages\x18\x07 \x03(\x0b\x32\x10.faabric.Message\x12\x0f\n\x07subType\x18\x08 \x01(\x05\x12\x13\n\x0b\x63ontextData\x18\t \x01(\x0c\x12\x12\n\nsingleHost\x18\n \x01(\x08\x12\x16\n\x0esingleHostHint\x18\x0b \x01(\x08\"L\n\x10\x42\x61tchExecuteType\x12\r\n\tFUNCTIONS\x10\x00\x12\x0b\n\x07THREADS\x10\x01\x12\r\n\tPROCESSES\x10\x02\x12\r\n\tMIGRATION\x10\x03\"\x83\x01\n\x19\x42\x61tchExecuteRequestStatus\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x10\n\x08\x66inished\x18\x02 \x01(\x08\x12(\n\x0emessageResults\x18\x03 \x03(\x0b\x32\x10.faabric.Message\x12\x1b\n\x13\x65xpectedNumMessages\x18\x04 \x01(\x05\"1\n\rHostResources\x12\r\n\x05slots\x18\x01 \x01(\x05\x12\x11\n\tusedSlots\x18\x02 \x01(\x05\"}\n\x16\x46unctionStatusResponse\x12>\n\x06status\x18\x01 \x01(\x0e\x32..faabric.FunctionStatusResponse.FunctionStatus\"#\n\x0e\x46unctionStatus\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x8e\t\n\x07Message\x12\n\n\x02id\x18\x01 \x01(\x05\x12\r\n\x05\x61ppId\x18\x02 \x01(\x05\x12\x0e\n\x06\x61ppIdx\x18\x03 \x01(\x05\x12\x10\n\x08mainHost\x18\x04 \x01(\t\x12*\n\x04type\x18\x05 \x01(\x0e\x32\x1c.faabric.Message.MessageType\x12\x0c\n\x04user\x18\x06 \x01(\t\x12\x10\n\x08\x66unction\x18\x07 \x01(\t\x12\x1d\n\tinputData\x18\x08 \x01(\x0cR\ninput_data\x12\x1f\n\noutputData\x18\t \x01(\tR\x0boutput_data\x12\x0f\n\x07\x66uncPtr\x18\n \x01(\x05\x12\x13\n\x0breturnValue\x18\x0b \x01(\x05\x12\x13\n\x0bsnapshotKey\x18\x0c \x01(\t\x12 \n\x0estartTimestamp\x18\x0e \x01(\x03R\x08start_ts\x12\x11\n\tresultKey\x18\x0f \x01(\t\x12\x17\n\x0f\x65xecutesLocally\x18\x10 \x01(\x08\x12\x11\n\tstatusKey\x18\x11 \x01(\t\x12\x14\n\x0c\x65xecutedHost\x18\x12 \x01(\t\x12\"\n\x0f\x66inishTimestamp\x18\x13 \x01(\x03R\tfinish_ts\x12\x18\n\x08isPython\x18\x15 \x01(\x08R\x06python\x12\x1b\n\npythonUser\x18\x18 \x01(\tR\x07py_user\x12\x1f\n\x0epythonFunction\x18\x19 \x01(\tR\x07py_func\x12\x13\n\x0bpythonEntry\x18\x1a \x01(\t\x12\x0f\n\x07groupId\x18\x1b \x01(\x05\x12\x10\n\x08groupIdx\x18\x1c \x01(\x05\x12\x11\n\tgroupSize\x18\x1d \x01(\x05\x12\x12\n\x05isMpi\x18\x1e \x01(\x08R\x03mpi\x12\x12\n\nmpiWorldId\x18\x1f \x01(\x05\x12\x0f\n\x07mpiRank\x18  \x01(\x05\x12$\n\x0cmpiWorldSize\x18! \x01(\x05R\x0empi_world_size\x12\x0f\n\x07\x63mdline\x18\" \x01(\t\x12*\n\x0frecordExecGraph\x18# \x01(\x08R\x11record_exec_graph\x12\x15\n\rchainedMsgIds\x18$ \x03(\x05\x12\x46\n\x13intExecGraphDetails\x18% \x03(\x0b\x32).faabric.Message.IntExecGraphDetailsEntry\x12@\n\x10\x65xecGraphDetails\x18& \x03(\x0b\x32&.faabric.Message.ExecGraphDetailsEntry\x12\x16\n\x0equeueStartTime\x18` \x01(\x03\x12\x14\n\x0cqueueEndTime\x18\x61 \x01(\x03\x12\x11\n\tchainedId\x18\x62 \x01(\x05\x12\x15\n\rparallelismId\x18\x63 \x01(\x05\x1a:\n\x18IntExecGraphDetailsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\x1a\x37\n\x15\x45xecGraphDetailsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"7\n\x0bMessageType\x12\x08\n\x04\x43\x41LL\x10\x00\x12\x08\n\x04KILL\x10\x01\x12\t\n\x05\x45MPTY\x10\x02\x12\t\n\x05\x46LUSH\x10\x03\"7\n\x0cStateRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"Q\n\x11StateChunkRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x04\x12\x11\n\tchunkSize\x18\x04 \x01(\x04\"8\n\rStateResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\"D\n\tStatePart\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\"A\n\x11StateSizeResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x11\n\tstateSize\x18\x03 \x01(\x04\"B\n\x14StateAppendedRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0f\n\x07nValues\x18\x03 \x01(\r\"\x8f\x01\n\x15StateAppendedResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12<\n\x06values\x18\x03 \x03(\x0b\x32,.faabric.StateAppendedResponse.AppendedValue\x1a\x1d\n\rAppendedValue\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"e\n\x13PointToPointMessage\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x0f\n\x07sendIdx\x18\x03 \x01(\x05\x12\x0f\n\x07recvIdx\x18\x04 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\xd5\x01\n\x14PointToPointMappings\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x43\n\x08mappings\x18\x03 \x03(\x0b\x32\x31.faabric.PointToPointMappings.PointToPointMapping\x1aX\n\x13PointToPointMapping\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x11\n\tmessageId\x18\x02 \x01(\x05\x12\x0e\n\x06\x61ppIdx\x18\x03 \x01(\x05\x12\x10\n\x08groupIdx\x18\x04 \x01(\x05\"f\n\x10PendingMigration\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07groupId\x18\x02 \x01(\x05\x12\x10\n\x08groupIdx\x18\x03 \x01(\x05\x12\x0f\n\x07srcHost\x18\x04 \x01(\t\x12\x0f\n\x07\x64stHost\x18\x05 \x01(\t\"e\n\x14\x46unctionStateRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x0c\n\x04lock\x18\x05 \x01(\x08\"z\n\x19\x46unctionStateSizeResponse\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x11\n\tstateSize\x18\x04 \x01(\x04\x12\x17\n\x0flockWaitingTime\x18\x05 \x01(\x04\"q\n\x19\x46unctionStateChunkRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x0e\n\x06offset\x18\x04 \x01(\x04\x12\x11\n\tchunkSize\x18\x05 \x01(\x04\"\x9a\x01\n\x11\x46unctionStatePart\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x0e\n\x06offset\x18\x04 \x01(\x04\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\x12\x11\n\tstateSize\x18\x06 \x01(\r\x12\x0e\n\x06unlock\x18\x07 \x01(\x08\x12\x11\n\tpStateKey\x18\x08 \x01(\t\"{\n\x15\x46unctionStateRegister\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x0c\n\x04host\x18\x03 \x01(\t\x12\x12\n\nisParition\x18\x04 \x01(\x08\x12\x11\n\tpInputKey\x18\x05 \x01(\t\x12\x11\n\tpStateKey\x18\x06 \x01(\t\"e\n\x18\x46unctionStateRepartition\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x16\n\x0enewParitionMap\x18\x04 \x01(\t\"f\n\x10\x46unctionStateAdd\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x11\n\tpStateKey\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\"\x99\x01\n\x1c\x46unctionStateTransferRequest\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x0c\n\x04\x66unc\x18\x02 \x01(\t\x12\x15\n\rparallelismId\x18\x03 \x01(\r\x12\x0c\n\x04host\x18\x04 \x01(\t\x12\x12\n\nisParition\x18\x05 \x01(\x08\x12\x11\n\tpInputKey\x18\x06 \x01(\t\x12\x11\n\tpStateKey\x18\x07 \x01(\t\"\x83\x02\n\x1b\x46unctionStateMetricResponse\x12\x0c\n\x04host\x18\x01 \x01(\t\x12I\n\x07metrics\x18\x02 \x03(\x0b\x32\x38.faabric.FunctionStateMetricResponse.FunctionStateMetric\x1a\x8a\x01\n\x13\x46unctionStateMetric\x12\x13\n\x0buserFuncPar\x18\x01 \x01(\t\x12\x0c\n\x04user\x18\x02 \x01(\t\x12\x0c\n\x04\x66unc\x18\x03 \x01(\t\x12\x15\n\rparallelismId\x18\x04 \x01(\r\x12\x15\n\rlockBlockTime\x18\x05 \x01(\r\x12\x14\n\x0clockHoldTime\x18\x06 \x01(\rb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.proto.faabric_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _MESSAGE_INTEXECGRAPHDETAILSENTRY._options = None
@@ -37,39 +37,59 @@
   _HOSTRESOURCES._serialized_start=599
   _HOSTRESOURCES._serialized_end=648
   _FUNCTIONSTATUSRESPONSE._serialized_start=650
   _FUNCTIONSTATUSRESPONSE._serialized_end=775
   _FUNCTIONSTATUSRESPONSE_FUNCTIONSTATUS._serialized_start=740
   _FUNCTIONSTATUSRESPONSE_FUNCTIONSTATUS._serialized_end=775
   _MESSAGE._serialized_start=778
-  _MESSAGE._serialized_end=1856
-  _MESSAGE_INTEXECGRAPHDETAILSENTRY._serialized_start=1684
-  _MESSAGE_INTEXECGRAPHDETAILSENTRY._serialized_end=1742
-  _MESSAGE_EXECGRAPHDETAILSENTRY._serialized_start=1744
-  _MESSAGE_EXECGRAPHDETAILSENTRY._serialized_end=1799
-  _MESSAGE_MESSAGETYPE._serialized_start=1801
-  _MESSAGE_MESSAGETYPE._serialized_end=1856
-  _STATEREQUEST._serialized_start=1858
-  _STATEREQUEST._serialized_end=1913
-  _STATECHUNKREQUEST._serialized_start=1915
-  _STATECHUNKREQUEST._serialized_end=1996
-  _STATERESPONSE._serialized_start=1998
-  _STATERESPONSE._serialized_end=2054
-  _STATEPART._serialized_start=2056
-  _STATEPART._serialized_end=2124
-  _STATESIZERESPONSE._serialized_start=2126
-  _STATESIZERESPONSE._serialized_end=2191
-  _STATEAPPENDEDREQUEST._serialized_start=2193
-  _STATEAPPENDEDREQUEST._serialized_end=2259
-  _STATEAPPENDEDRESPONSE._serialized_start=2262
-  _STATEAPPENDEDRESPONSE._serialized_end=2405
-  _STATEAPPENDEDRESPONSE_APPENDEDVALUE._serialized_start=2376
-  _STATEAPPENDEDRESPONSE_APPENDEDVALUE._serialized_end=2405
-  _POINTTOPOINTMESSAGE._serialized_start=2407
-  _POINTTOPOINTMESSAGE._serialized_end=2508
-  _POINTTOPOINTMAPPINGS._serialized_start=2511
-  _POINTTOPOINTMAPPINGS._serialized_end=2741
-  _POINTTOPOINTMAPPINGS_POINTTOPOINTMAPPING._serialized_start=2636
-  _POINTTOPOINTMAPPINGS_POINTTOPOINTMAPPING._serialized_end=2741
-  _PENDINGMIGRATION._serialized_start=2743
-  _PENDINGMIGRATION._serialized_end=2845
+  _MESSAGE._serialized_end=1944
+  _MESSAGE_INTEXECGRAPHDETAILSENTRY._serialized_start=1772
+  _MESSAGE_INTEXECGRAPHDETAILSENTRY._serialized_end=1830
+  _MESSAGE_EXECGRAPHDETAILSENTRY._serialized_start=1832
+  _MESSAGE_EXECGRAPHDETAILSENTRY._serialized_end=1887
+  _MESSAGE_MESSAGETYPE._serialized_start=1889
+  _MESSAGE_MESSAGETYPE._serialized_end=1944
+  _STATEREQUEST._serialized_start=1946
+  _STATEREQUEST._serialized_end=2001
+  _STATECHUNKREQUEST._serialized_start=2003
+  _STATECHUNKREQUEST._serialized_end=2084
+  _STATERESPONSE._serialized_start=2086
+  _STATERESPONSE._serialized_end=2142
+  _STATEPART._serialized_start=2144
+  _STATEPART._serialized_end=2212
+  _STATESIZERESPONSE._serialized_start=2214
+  _STATESIZERESPONSE._serialized_end=2279
+  _STATEAPPENDEDREQUEST._serialized_start=2281
+  _STATEAPPENDEDREQUEST._serialized_end=2347
+  _STATEAPPENDEDRESPONSE._serialized_start=2350
+  _STATEAPPENDEDRESPONSE._serialized_end=2493
+  _STATEAPPENDEDRESPONSE_APPENDEDVALUE._serialized_start=2464
+  _STATEAPPENDEDRESPONSE_APPENDEDVALUE._serialized_end=2493
+  _POINTTOPOINTMESSAGE._serialized_start=2495
+  _POINTTOPOINTMESSAGE._serialized_end=2596
+  _POINTTOPOINTMAPPINGS._serialized_start=2599
+  _POINTTOPOINTMAPPINGS._serialized_end=2812
+  _POINTTOPOINTMAPPINGS_POINTTOPOINTMAPPING._serialized_start=2724
+  _POINTTOPOINTMAPPINGS_POINTTOPOINTMAPPING._serialized_end=2812
+  _PENDINGMIGRATION._serialized_start=2814
+  _PENDINGMIGRATION._serialized_end=2916
+  _FUNCTIONSTATEREQUEST._serialized_start=2918
+  _FUNCTIONSTATEREQUEST._serialized_end=3019
+  _FUNCTIONSTATESIZERESPONSE._serialized_start=3021
+  _FUNCTIONSTATESIZERESPONSE._serialized_end=3143
+  _FUNCTIONSTATECHUNKREQUEST._serialized_start=3145
+  _FUNCTIONSTATECHUNKREQUEST._serialized_end=3258
+  _FUNCTIONSTATEPART._serialized_start=3261
+  _FUNCTIONSTATEPART._serialized_end=3415
+  _FUNCTIONSTATEREGISTER._serialized_start=3417
+  _FUNCTIONSTATEREGISTER._serialized_end=3540
+  _FUNCTIONSTATEREPARTITION._serialized_start=3542
+  _FUNCTIONSTATEREPARTITION._serialized_end=3643
+  _FUNCTIONSTATEADD._serialized_start=3645
+  _FUNCTIONSTATEADD._serialized_end=3747
+  _FUNCTIONSTATETRANSFERREQUEST._serialized_start=3750
+  _FUNCTIONSTATETRANSFERREQUEST._serialized_end=3903
+  _FUNCTIONSTATEMETRICRESPONSE._serialized_start=3906
+  _FUNCTIONSTATEMETRICRESPONSE._serialized_end=4165
+  _FUNCTIONSTATEMETRICRESPONSE_FUNCTIONSTATEMETRIC._serialized_start=4027
+  _FUNCTIONSTATEMETRICRESPONSE_FUNCTIONSTATEMETRIC._serialized_end=4165
 # @@protoc_insertion_point(module_scope)
```

### Comparing `myfaasmctl-0.0.4/faasmctl/util/gen_proto/planner_pb2.py` & `myfaasmctl-0.0.5/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19src/planner/planner.proto\x12\x0f\x66\x61\x61\x62ric.planner\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"e\n\x0eResponseStatus\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.faabric.planner.ResponseStatus.Status\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07\x65pochMs\x18\x01 \x01(\x03\"\xb0\x03\n\x0bHttpMessage\x12:\n\x04type\x18\x01 \x01(\x0e\x32!.faabric.planner.HttpMessage.TypeR\thttp_type\x12\x1c\n\x0bpayloadJson\x18\x02 \x01(\tR\x07payload\"\xc6\x02\n\x04Type\x12\x0b\n\x07NO_TYPE\x10\x00\x12\t\n\x05RESET\x10\x01\x12\x19\n\x15\x46LUSH_AVAILABLE_HOSTS\x10\x02\x12\x13\n\x0f\x46LUSH_EXECUTORS\x10\x03\x12\x1a\n\x16\x46LUSH_SCHEDULING_STATE\x10\x04\x12\x17\n\x13GET_AVAILABLE_HOSTS\x10\x05\x12\x0e\n\nGET_CONFIG\x10\x06\x12\x12\n\x0eGET_EXEC_GRAPH\x10\x07\x12\x16\n\x12GET_IN_FLIGHT_APPS\x10\x08\x12\x11\n\rEXECUTE_BATCH\x10\n\x12\x18\n\x14\x45XECUTE_BATCH_STATUS\x10\x0b\x12\x1f\n\x1bPRELOAD_SCHEDULING_DECISION\x10\x0c\x12\x0e\n\nSET_POLICY\x10\r\x12\x0e\n\nGET_POLICY\x10\x0e\x12\x17\n\x13SET_NEXT_EVICTED_VM\x10\x0f\"\xdf\x02\n\x17GetInFlightAppsResponse\x12\x42\n\x04\x61pps\x18\x01 \x03(\x0b\x32\x34.faabric.planner.GetInFlightAppsResponse.InFlightApp\x12\x15\n\rnumMigrations\x18\x02 \x01(\x05\x12\x18\n\x10nextEvictedVmIps\x18\x03 \x03(\t\x12\x46\n\nfrozenApps\x18\x04 \x03(\x0b\x32\x32.faabric.planner.GetInFlightAppsResponse.FrozenApp\x1aL\n\x0bInFlightApp\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07subType\x18\x02 \x01(\x05\x12\x0c\n\x04size\x18\x03 \x01(\x05\x12\x0f\n\x07hostIps\x18\x04 \x03(\t\x1a\x39\n\tFrozenApp\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07subType\x18\x02 \x01(\x05\x12\x0c\n\x04size\x18\x03 \x01(\x05\".\n\x15NumMigrationsResponse\x12\x15\n\rnumMigrations\x18\x01 \x01(\x05\"N\n\rPlannerConfig\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x13\n\x0bhostTimeout\x18\x02 \x01(\x05\x12\x1c\n\x14numThreadsHttpServer\x18\x03 \x01(\x05\"\xbc\x01\n\x04Host\x12\n\n\x02ip\x18\x01 \x01(\t\x12\r\n\x05slots\x18\x02 \x01(\x05\x12\x11\n\tusedSlots\x18\x03 \x01(\x05\x12.\n\nregisterTs\x18\x04 \x01(\x0b\x32\x1a.faabric.planner.Timestamp\x12/\n\x08mpiPorts\x18\x05 \x03(\x0b\x32\x1d.faabric.planner.Host.MpiPort\x1a%\n\x07MpiPort\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x0c\n\x04used\x18\x02 \x01(\x08\">\n\x0cPingResponse\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\"M\n\x13RegisterHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\x12\x11\n\toverwrite\x18\x02 \x01(\x08\"\x87\x01\n\x14RegisterHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\x12.\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\x12\x0e\n\x06hostId\x18\x03 \x01(\x05\"8\n\x11RemoveHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\"E\n\x12RemoveHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\">\n\x16\x41vailableHostsResponse\x12$\n\x05hosts\x18\x01 \x03(\x0b\x32\x15.faabric.planner.Host\"\'\n\x16SetEvictedVmIpsRequest\x12\r\n\x05vmIps\x18\x01 \x03(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19src/planner/planner.proto\x12\x0f\x66\x61\x61\x62ric.planner\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"e\n\x0eResponseStatus\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.faabric.planner.ResponseStatus.Status\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07\x65pochMs\x18\x01 \x01(\x03\"\x91\x03\n\x0bHttpMessage\x12:\n\x04type\x18\x01 \x01(\x0e\x32!.faabric.planner.HttpMessage.TypeR\thttp_type\x12\x1c\n\x0bpayloadJson\x18\x02 \x01(\tR\x07payload\"\xa7\x02\n\x04Type\x12\x0b\n\x07NO_TYPE\x10\x00\x12\t\n\x05RESET\x10\x01\x12\x19\n\x15\x46LUSH_AVAILABLE_HOSTS\x10\x02\x12\x13\n\x0f\x46LUSH_EXECUTORS\x10\x03\x12\x1a\n\x16\x46LUSH_SCHEDULING_STATE\x10\x04\x12\x17\n\x13GET_AVAILABLE_HOSTS\x10\x05\x12\x0e\n\nGET_CONFIG\x10\x06\x12\x12\n\x0eGET_EXEC_GRAPH\x10\x07\x12\x16\n\x12GET_IN_FLIGHT_APPS\x10\x08\x12\x11\n\rEXECUTE_BATCH\x10\n\x12\x18\n\x14\x45XECUTE_BATCH_STATUS\x10\x0b\x12\x1f\n\x1bPRELOAD_SCHEDULING_DECISION\x10\x0c\x12\x18\n\x14GET_FUNCTION_METRICS\x10\r\"\xa3\x01\n\x17GetInFlightAppsResponse\x12\x42\n\x04\x61pps\x18\x01 \x03(\x0b\x32\x34.faabric.planner.GetInFlightAppsResponse.InFlightApp\x12\x15\n\rnumMigrations\x18\x02 \x01(\x05\x1a-\n\x0bInFlightApp\x12\r\n\x05\x61ppId\x18\x01 \x01(\x05\x12\x0f\n\x07hostIps\x18\x02 \x03(\t\".\n\x15NumMigrationsResponse\x12\x15\n\rnumMigrations\x18\x01 \x01(\x05\"N\n\rPlannerConfig\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x13\n\x0bhostTimeout\x18\x02 \x01(\x05\x12\x1c\n\x14numThreadsHttpServer\x18\x03 \x01(\x05\"d\n\x04Host\x12\n\n\x02ip\x18\x01 \x01(\t\x12\r\n\x05slots\x18\x02 \x01(\x05\x12\x11\n\tusedSlots\x18\x03 \x01(\x05\x12.\n\nregisterTs\x18\x04 \x01(\x0b\x32\x1a.faabric.planner.Timestamp\">\n\x0cPingResponse\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\"M\n\x13RegisterHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\x12\x11\n\toverwrite\x18\x02 \x01(\x08\"\x87\x01\n\x14RegisterHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\x12.\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\x12\x0e\n\x06hostId\x18\x03 \x01(\x05\"8\n\x11RemoveHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\"E\n\x12RemoveHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\">\n\x16\x41vailableHostsResponse\x12$\n\x05hosts\x18\x01 \x03(\x0b\x32\x15.faabric.planner.Host\"V\n\x1a\x43hainedFunctionsMetricsRes\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nthroughput\x18\x02 \x01(\x05\x12\x16\n\x0eprocessLatency\x18\x03 \x01(\x05\"\xac\x01\n\x12\x46unctionMetricsRes\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nthroughput\x18\x02 \x01(\x05\x12\x16\n\x0eprocessLatency\x18\x03 \x01(\x05\x12\x1a\n\x12\x61verageWaitingTime\x18\x04 \x01(\x05\x12\x0e\n\x06hostIp\x18\x05 \x01(\t\x12\x1a\n\x12lockCongestionTime\x18\x06 \x01(\x05\x12\x14\n\x0clockHoldTime\x18\x07 \x01(\x05\"\x9b\x01\n\x16\x46unctionMetricResponse\x12\x43\n\x0e\x63hainedMetrics\x18\x01 \x03(\x0b\x32+.faabric.planner.ChainedFunctionsMetricsRes\x12<\n\x0f\x66unctionMetrics\x18\x02 \x03(\x0b\x32#.faabric.planner.FunctionMetricsResb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.planner.planner_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EMPTYRESPONSE._serialized_start=46
@@ -27,39 +27,39 @@
   _RESPONSESTATUS._serialized_start=109
   _RESPONSESTATUS._serialized_end=210
   _RESPONSESTATUS_STATUS._serialized_start=183
   _RESPONSESTATUS_STATUS._serialized_end=210
   _TIMESTAMP._serialized_start=212
   _TIMESTAMP._serialized_end=240
   _HTTPMESSAGE._serialized_start=243
-  _HTTPMESSAGE._serialized_end=675
+  _HTTPMESSAGE._serialized_end=644
   _HTTPMESSAGE_TYPE._serialized_start=349
-  _HTTPMESSAGE_TYPE._serialized_end=675
-  _GETINFLIGHTAPPSRESPONSE._serialized_start=678
-  _GETINFLIGHTAPPSRESPONSE._serialized_end=1029
-  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_start=894
-  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_end=970
-  _GETINFLIGHTAPPSRESPONSE_FROZENAPP._serialized_start=972
-  _GETINFLIGHTAPPSRESPONSE_FROZENAPP._serialized_end=1029
-  _NUMMIGRATIONSRESPONSE._serialized_start=1031
-  _NUMMIGRATIONSRESPONSE._serialized_end=1077
-  _PLANNERCONFIG._serialized_start=1079
-  _PLANNERCONFIG._serialized_end=1157
-  _HOST._serialized_start=1160
-  _HOST._serialized_end=1348
-  _HOST_MPIPORT._serialized_start=1311
-  _HOST_MPIPORT._serialized_end=1348
-  _PINGRESPONSE._serialized_start=1350
-  _PINGRESPONSE._serialized_end=1412
-  _REGISTERHOSTREQUEST._serialized_start=1414
-  _REGISTERHOSTREQUEST._serialized_end=1491
-  _REGISTERHOSTRESPONSE._serialized_start=1494
-  _REGISTERHOSTRESPONSE._serialized_end=1629
-  _REMOVEHOSTREQUEST._serialized_start=1631
-  _REMOVEHOSTREQUEST._serialized_end=1687
-  _REMOVEHOSTRESPONSE._serialized_start=1689
-  _REMOVEHOSTRESPONSE._serialized_end=1758
-  _AVAILABLEHOSTSRESPONSE._serialized_start=1760
-  _AVAILABLEHOSTSRESPONSE._serialized_end=1822
-  _SETEVICTEDVMIPSREQUEST._serialized_start=1824
-  _SETEVICTEDVMIPSREQUEST._serialized_end=1863
+  _HTTPMESSAGE_TYPE._serialized_end=644
+  _GETINFLIGHTAPPSRESPONSE._serialized_start=647
+  _GETINFLIGHTAPPSRESPONSE._serialized_end=810
+  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_start=765
+  _GETINFLIGHTAPPSRESPONSE_INFLIGHTAPP._serialized_end=810
+  _NUMMIGRATIONSRESPONSE._serialized_start=812
+  _NUMMIGRATIONSRESPONSE._serialized_end=858
+  _PLANNERCONFIG._serialized_start=860
+  _PLANNERCONFIG._serialized_end=938
+  _HOST._serialized_start=940
+  _HOST._serialized_end=1040
+  _PINGRESPONSE._serialized_start=1042
+  _PINGRESPONSE._serialized_end=1104
+  _REGISTERHOSTREQUEST._serialized_start=1106
+  _REGISTERHOSTREQUEST._serialized_end=1183
+  _REGISTERHOSTRESPONSE._serialized_start=1186
+  _REGISTERHOSTRESPONSE._serialized_end=1321
+  _REMOVEHOSTREQUEST._serialized_start=1323
+  _REMOVEHOSTREQUEST._serialized_end=1379
+  _REMOVEHOSTRESPONSE._serialized_start=1381
+  _REMOVEHOSTRESPONSE._serialized_end=1450
+  _AVAILABLEHOSTSRESPONSE._serialized_start=1452
+  _AVAILABLEHOSTSRESPONSE._serialized_end=1514
+  _CHAINEDFUNCTIONSMETRICSRES._serialized_start=1516
+  _CHAINEDFUNCTIONSMETRICSRES._serialized_end=1602
+  _FUNCTIONMETRICSRES._serialized_start=1605
+  _FUNCTIONMETRICSRES._serialized_end=1777
+  _FUNCTIONMETRICRESPONSE._serialized_start=1780
+  _FUNCTIONMETRICRESPONSE._serialized_end=1935
 # @@protoc_insertion_point(module_scope)
```

### Comparing `myfaasmctl-0.0.4/faasmctl/util/invoke.py` & `myfaasmctl-0.0.5/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/k8s.py` & `myfaasmctl-0.0.5/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/network.py` & `myfaasmctl-0.0.5/faasmctl/util/network.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/planner.py` & `myfaasmctl-0.0.5/faasmctl/util/planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from faasmctl.util.config import get_faasm_ini_file, get_faasm_planner_host_port
 from faasmctl.util.gen_proto.planner_pb2 import (
     AvailableHostsResponse,
     GetInFlightAppsResponse,
     HttpMessage,
-    SetEvictedVmIpsRequest,
+    #SetEvictedVmIpsRequest,
+    FunctionMetricResponse,
 )
 from google.protobuf.json_format import MessageToJson, Parse
 from requests import post
 from time import sleep
 
 PLANNER_JSON_MESSAGE_FAILED = {"dead": "beef"}
 
@@ -40,14 +41,16 @@
         http_message.type = HttpMessage.Type.EXECUTE_BATCH_STATUS
     elif msg_type == "PRELOAD_SCHEDULING_DECISION":
         http_message.type = HttpMessage.Type.PRELOAD_SCHEDULING_DECISION
     elif msg_type == "SET_NEXT_EVICTED_VM":
         http_message.type = HttpMessage.Type.SET_NEXT_EVICTED_VM
     elif msg_type == "SET_POLICY":
         http_message.type = HttpMessage.Type.SET_POLICY
+    elif msg_type == "GET_FUNCTION_METRICS":
+        http_message.type = HttpMessage.Type.GET_FUNCTION_METRICS
     else:
         raise RuntimeError("Unrecognised HTTP msg type: {}".format(msg_type))
 
     if msg_body:
         http_message.payloadJson = msg_body
 
     return MessageToJson(http_message, indent=None)
@@ -195,7 +198,26 @@
     if response.status_code != 200:
         print(
             "Error setting planner policy '{}' (code: {}): {}".format(
                 policy, response.status_code, response.text
             )
         )
         raise RuntimeError("Error setting planner policy")
+
+def get_function_metrics():
+    host, port = get_faasm_planner_host_port(get_faasm_ini_file())
+    url = "http://{}:{}".format(host, port)
+    planner_msg = prepare_planner_msg("GET_FUNCTION_METRICS")
+
+    response = post(url, data=planner_msg, timeout=None)
+
+    if response.status_code != 200:
+        print(
+            "Error getting metrics (code: {}): {}".format(
+                response.status_code, response.text
+            )
+        )
+        raise RuntimeError("Error getting metrics")
+
+    metrics = Parse(response.text, FunctionMetricResponse())
+
+    return metrics
```

### Comparing `myfaasmctl-0.0.4/faasmctl/util/restart.py` & `myfaasmctl-0.0.5/faasmctl/util/restart.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/results.py` & `myfaasmctl-0.0.5/faasmctl/util/results.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/faasmctl/util/upload.py` & `myfaasmctl-0.0.5/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/myfaasmctl.egg-info/PKG-INFO` & `myfaasmctl-0.0.5/myfaasmctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfaasmctl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `myfaasmctl-0.0.4/myfaasmctl.egg-info/SOURCES.txt` & `myfaasmctl-0.0.5/myfaasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myfaasmctl-0.0.4/pyproject.toml` & `myfaasmctl-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "myfaasmctl"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

