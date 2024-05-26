# Comparing `tmp/node-ec2-instance-0.0.3.tar.gz` & `tmp/node-ec2-instance-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "node-ec2-instance-0.0.3.tar", last modified: Sat May 25 12:34:49 2024, max compression
+gzip compressed data, was "node-ec2-instance-0.0.4.tar", last modified: Sat May 25 12:55:36 2024, max compression
```

## Comparing `node-ec2-instance-0.0.3.tar` & `node-ec2-instance-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.817197 node-ec2-instance-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/src/node_ec2_instance/
--rw-r--r--   0 runner    (1001) docker     (127)    49104 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/src/node_ec2_instance/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23433 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:34:39.000000 node-ec2-instance-0.0.3/src/node_ec2_instance/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:34:49.821197 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 12:34:49.000000 node-ec2-instance-0.0.3/src/node_ec2_instance.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/src/node_ec2_instance/
+-rw-r--r--   0 runner    (1001) docker     (127)    50392 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/src/node_ec2_instance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/src/node_ec2_instance/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/src/node_ec2_instance/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24395 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/src/node_ec2_instance/_jsii/cdk-node-ec2-instance@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:55:26.000000 node-ec2-instance-0.0.4/src/node_ec2_instance/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:55:36.210555 node-ec2-instance-0.0.4/src/node_ec2_instance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-25 12:55:36.000000 node-ec2-instance-0.0.4/src/node_ec2_instance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 12:55:36.000000 node-ec2-instance-0.0.4/src/node_ec2_instance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:55:36.000000 node-ec2-instance-0.0.4/src/node_ec2_instance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 12:55:36.000000 node-ec2-instance-0.0.4/src/node_ec2_instance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 12:55:36.000000 node-ec2-instance-0.0.4/src/node_ec2_instance.egg-info/top_level.txt
```

### Comparing `node-ec2-instance-0.0.3/LICENSE` & `node-ec2-instance-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `node-ec2-instance-0.0.3/setup.py` & `node-ec2-instance-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "node-ec2-instance",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "CDK construct library for creating an EC2 instance with Node.js installed",
     "license": "Apache-2.0",
     "url": "https://github.com/badmintoncryer/cdk-node-ec2-instance.git",
     "long_description_content_type": "text/markdown",
     "author": "Kazuho CryerShinozuka<malaysia.cryer@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "node_ec2_instance",
         "node_ec2_instance._jsii"
     ],
     "package_data": {
         "node_ec2_instance._jsii": [
-            "cdk-node-ec2-instance@0.0.3.jsii.tgz"
+            "cdk-node-ec2-instance@0.0.4.jsii.tgz"
         ],
         "node_ec2_instance": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `node-ec2-instance-0.0.3/src/node_ec2_instance/__init__.py` & `node-ec2-instance-0.0.4/src/node_ec2_instance/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,48 @@
 After the stack is deployed, you can SSH into the EC2 instance and use Node.js:
 
 ```bash
 $ ssh ec2-user@<public-ip>
 $ node --version
 v20.13.1
 ```
+
+## user data
+
+Installation of Node.js is done by user data script. You can see the script in the `src/index.ts` file.
+
+```python
+nodejsUserData.addCommands(
+  'touch ~/.bashrc',
+  'curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash',
+  'source ~/.bashrc',
+  'export NVM_DIR="$HOME/.nvm"',
+  '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"',
+  `nvm install ${props.nodeJsVersion ?? '--lts'}`,
+  // Note that the above will install nvm, node and npm for the root user.
+  // It will not add the correct ENV VAR in ec2-user's environment.
+  `cat <<EOF >> /home/ec2-user/.bashrc
+export NVM_DIR="/.nvm"
+[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
+EOF`);
+```
+
+Ofcourse, you can customize the additional user data script by calling `instance.userData.addCommands()` method.
+
+```python
+declare const instance: NodeEc2Instance;
+
+// install VScode for linux
+instance.userData.addCommands(
+  'sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc',
+  'echo -e "[code]\nname=Visual Studio Code\nbaseurl=https://packages.microsoft.com/yumrepos/vscode\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/vscode.repo > /dev/null',
+  'sudo dnf check-update',
+  'sudo dnf install -y code',
+);
+```
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
 
 import abc
 import builtins
 import datetime
```

