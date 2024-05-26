# Comparing `tmp/appmesh-1.1.5-py3-none-any.whl.zip` & `tmp/appmesh-1.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16415 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-22 00:38 appmesh/__init__.py
--rw-r--r--  2.0 unx    59705 b- defN 24-May-22 00:38 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-22 00:38 appmesh-1.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-22 00:38 appmesh-1.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-22 00:38 appmesh-1.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-22 00:38 appmesh-1.1.5.dist-info/RECORD
-6 files, 71057 bytes uncompressed, 15593 bytes compressed:  78.1%
+Zip file size: 16443 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-26 04:46 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59591 b- defN 24-May-26 04:46 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10832 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-26 04:47 appmesh-1.1.6.dist-info/RECORD
+6 files, 70989 bytes uncompressed, 15621 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.1.5.dist-info/METADATA
+Filename: appmesh-1.1.6.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.1.5.dist-info/WHEEL
+Filename: appmesh-1.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.1.5.dist-info/top_level.txt
+Filename: appmesh-1.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.1.5.dist-info/RECORD
+Filename: appmesh-1.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -342,31 +342,30 @@
             str: JWT token.
         """
         self.jwt_token = None
         resp = self._request_http(
             AppMeshClient.Method.POST,
             path="/appmesh/login",
             header={
-                "Username": base64.b64encode(user_name.encode()),
-                "Password": base64.b64encode(user_pwd.encode()),
+                "Authorization": "Basic " + base64.b64encode((user_name + ":" + user_pwd).encode()).decode(),
                 "Expire-Seconds": self._parse_duration(timeout_seconds),
             },
         )
         if resp.status_code == HTTPStatus.OK:
             if "Access-Token" in resp.json():
                 self.jwt_token = resp.json()["Access-Token"]
         elif resp.status_code == HTTPStatus.UNAUTHORIZED and "totp_challenge" in resp.json():
             challenge = resp.json()["totp_challenge"]
             resp = self._request_http(
                 AppMeshClient.Method.POST,
                 path="/appmesh/totp/validate",
                 header={
-                    "Username": base64.b64encode(user_name.encode()),
-                    "Totp-Challenge": base64.b64encode(challenge.encode()),
-                    "Totp": base64.b64encode(totp_code.encode()),
+                    "Username": base64.b64encode(user_name.encode()).decode(),
+                    "Totp-Challenge": base64.b64encode(challenge.encode()).decode(),
+                    "Totp": totp_code,
                     "Expire-Seconds": self._parse_duration(timeout_seconds),
                 },
             )
             if resp.status_code == HTTPStatus.OK:
                 if "Access-Token" in resp.json():
                     self.jwt_token = resp.json()["Access-Token"]
             else:
@@ -454,15 +453,15 @@
 
         Returns:
             bool: success or failure.
         """
         resp = self._request_http(
             method=AppMeshClient.Method.POST,
             path="/appmesh/totp/setup",
-            header={"Totp": base64.b64encode(totp_code.encode())},
+            header={"Totp": totp_code},
         )
         if resp.status_code != HTTPStatus.OK:
             raise Exception(resp.text)
         return resp.status_code == HTTPStatus.OK
 
     def totp_disable(self, user="self") -> bool:
         """Disable 2FA for current user
@@ -1300,18 +1299,18 @@
     def __connect_socket(self) -> None:
         """Establish tcp connection"""
         context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
         if hasattr(context, "minimum_version"):
             context.minimum_version = ssl.TLSVersion.TLSv1_2
         else:
             context.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1
-        context.verify_mode = ssl.CERT_NONE if self.ssl_verify is False else ssl.CERT_REQUIRED
+        if self.ssl_verify:
+            context.verify_mode = ssl.CERT_REQUIRED
         if isinstance(self.ssl_verify, str):
             # Load server-side certificate authority (CA) certificates
-            context.check_hostname = True
             context.load_verify_locations(self.ssl_verify)
         if self.ssl_client_cert is not None:
             # Load client-side certificate and private key
             context.load_cert_chain(certfile=self.ssl_client_cert[0], keyfile=self.ssl_client_cert[1])
 
         # Create a TCP socket
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
```

## Comparing `appmesh-1.1.5.dist-info/METADATA` & `appmesh-1.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.1.5
+Version: 1.1.6
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 ---|---
 Application management | 1. Manage independent applications and guard the process running, similar with systemd but more flexible (long/short running, periodic long running, cron schedule, customized day time and error handling control) and comprehensive monitoring (number of starts, return code, error message, health-check) for both native and docker application. <br> 2. Use SDK/CLI run application on a remote host with sync/async mode and fetch result to client. <br> 3. Full control of application lifecycle (cgroup for resource limitation, specific OS user for execution user). <br> 4. Interactive application start support specify input data by pipe and environment variables.<br> 5. All functionality provides by [CLI](https://app-mesh.readthedocs.io/en/latest/CLI.html), [REST](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis), [SDK](https://github.com/laoshanxi/app-mesh/tree/main/src/sdk) and [WebGUI](https://github.com/laoshanxi/app-mesh-ui) interface.<br>
 Security |  ⚡️ [JWT authentication](https://app-mesh.readthedocs.io/en/latest/JWT.html) for CLI and REST interface <br> ⚡️ [LDAP support](https://app-mesh.readthedocs.io/en/latest/LDAP.html) <br> ⚡️ [Role based permission control](https://app-mesh.readthedocs.io/en/latest/USER_ROLE.html) <br> ⚡️ [Multi-factor authentication](https://app-mesh.readthedocs.io/en/latest/MFA.html)<br> SSL support (ECDH and secure ciphers) for REST http connection  <br> Multi-tenant support
 Cloud native | Schedule cloud level applications for running on multile hosts with resource size request.<br> ⚡️ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/latest/PROMETHEUS.html) <br> ⚡️ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/latest/GrafanaDataSource.html) <br> ⚡️ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html) <br>⚡️ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
 Micro service application | ⚡️ [Consul micro-service cluster management](https://app-mesh.readthedocs.io/en/latest/CONSUL.html)
 Extra Features | Collect host/app resource usage <br> Remote run shell commands <br> Download/Upload files interface <br> Hot-update support `systemctl reload appmesh` <br> Bash completion <br> Reverse proxy <br> [Web GUI](https://github.com/laoshanxi/app-mesh-ui)
 Platform support | X86_64 <br> ARM32 <br> ARM64
-SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/appmesh_client.html) <br> [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/appmesh_client.go)
+SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/appmesh_client.html) <br> [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/appmesh_client.go) <br> Swagger `https://localhost:6060/swagger`
 
 ## Getting started
 
 The [Installation doc](https://app-mesh.readthedocs.io/en/latest/Install.html) introduces how
 to install App Mesh via docker-compose or native way and setup App Mesh cluster.
 
 ## Documentation
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.1.5 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.1.6 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
@@ -66,38 +66,39 @@
 Bash completion
 Reverse proxy
 [Web GUI](https://github.com/laoshanxi/app-mesh-ui) Platform support | X86_64
 ARM32
 ARM64 SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/
 appmesh_client.html)
 [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/
-appmesh_client.go) ## Getting started The [Installation doc](https://app-
-mesh.readthedocs.io/en/latest/Install.html) introduces how to install App Mesh
-via docker-compose or native way and setup App Mesh cluster. ## Documentation -
-[Read the Docs](https://app-mesh.readthedocs.io/) - [REST API](https://app-
-mesh.readthedocs.io/en/latest/Development.html#rest-apis) - [Command lines]
-(https://app-mesh.readthedocs.io/en/latest/CLI.html) - [Security](https://app-
-mesh.readthedocs.io/en/latest/JWT.html) ## Comparison ### Standalone mode |
-Feature | App Mesh | [Supervisor](http://supervisord.org/) | [crontab](https://
-crontab.guru/) | | ------------------------ | -------- | ----------------------
---------------- | -------------------------------- | | Accuracy | Seconds |
-Seconds | Minutes | | Language | C++11 | Python | C | | Web GUI | â | â | |
-Command lines | â | â | â | | SDK | â | | | Cron schedule expression |
-â | | â | | Manage daemon process | | | â | | Manage docker app | â | |
-| Start check (avoid leak) | â | â | | Session login | | | | Manage stdout/
-stderr | â | â | | Health check | â | | | Rich control options | â | |
-| Authentication | â | â | | Multi-tenant | â | | â | ### Cluster mode
-| Feature | App Mesh | Kubernetes | | ----------------- | -------- | ---------
-- | | Easy deploy | â | | More features | | â | | Non-container app | â |
-| Service expose | â | â | | Scheduler | â | â | | Definition file |
-JSON | YAML | | GUI | â | â | | Virtual Network | | â | | Monitor tools |
-â | â | --- ### Component diagram ![block-diagram](https://github.com/
-laoshanxi/app-mesh/raw/main/docs/source/block_diagram.png) --- ## Success -
-[Build a powerful monitor system with Grafana/Prometheus/Loki](https://app-
-mesh.readthedocs.io/en/latest/success/
+appmesh_client.go)
+Swagger `https://localhost:6060/swagger` ## Getting started The [Installation
+doc](https://app-mesh.readthedocs.io/en/latest/Install.html) introduces how to
+install App Mesh via docker-compose or native way and setup App Mesh cluster.
+## Documentation - [Read the Docs](https://app-mesh.readthedocs.io/) - [REST
+API](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis) -
+[Command lines](https://app-mesh.readthedocs.io/en/latest/CLI.html) -
+[Security](https://app-mesh.readthedocs.io/en/latest/JWT.html) ## Comparison
+### Standalone mode | Feature | App Mesh | [Supervisor](http://supervisord.org/
+) | [crontab](https://crontab.guru/) | | ------------------------ | -------- |
+------------------------------------- | -------------------------------- | |
+Accuracy | Seconds | Seconds | Minutes | | Language | C++11 | Python | C | |
+Web GUI | â | â | | Command lines | â | â | â | | SDK | â | | |
+Cron schedule expression | â | | â | | Manage daemon process | | | â | |
+Manage docker app | â | | | Start check (avoid leak) | â | â | | Session
+login | | | | Manage stdout/stderr | â | â | | Health check | â | | |
+Rich control options | â | | | Authentication | â | â | | Multi-tenant |
+â | | â | ### Cluster mode | Feature | App Mesh | Kubernetes | | ----------
+------- | -------- | ---------- | | Easy deploy | â | | More features | | â
+| | Non-container app | â | | Service expose | â | â | | Scheduler | â
+| â | | Definition file | JSON | YAML | | GUI | â | â | | Virtual Network
+| | â | | Monitor tools | â | â | --- ### Component diagram ![block-
+diagram](https://github.com/laoshanxi/app-mesh/raw/main/docs/source/
+block_diagram.png) --- ## Success - [Build a powerful monitor system with
+Grafana/Prometheus/Loki](https://app-mesh.readthedocs.io/en/latest/success/
 build_powerful_monitor_system_with_Grafana_Prometheus_Loki.html) - [Customize
 application start behavior](https://app-mesh.readthedocs.io/en/latest/success/
 customize_app_startup_behavior.html) - [Manage cluster-level microservice
 applications](https://app-mesh.readthedocs.io/en/latest/success/
 manage_cluster_level_microservice_applications.html) - [Open service broker
 support local PV for Kubernetes](https://app-mesh.readthedocs.io/en/latest/
 success/open_service_broker_support_local_pv_for_K8S.html) - [Promote native
```

