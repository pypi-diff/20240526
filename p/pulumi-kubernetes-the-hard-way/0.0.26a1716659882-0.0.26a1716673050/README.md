# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.26a1716659882.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.26a1716673050.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.26a1716659882.tar", last modified: Sat May 25 18:00:54 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.26a1716673050.tar", last modified: Sat May 25 21:39:54 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882.tar` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050.tar`

### file list

```diff
@@ -1,92 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.620301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-25 18:00:54.620301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.604301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4915 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.608301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      864 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    39619 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    10400 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     6556 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     4399 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)     4880 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     3418 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     2560 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)     2860 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8791 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4826 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)     5799 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23901 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12558 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    56778 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.616301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1132 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1767 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    26794 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    14674 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/containerd_service.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)    13465 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    25513 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5199 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
--rw-------   0 runner    (1001) docker     (127)     5115 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     5187 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
--rw-------   0 runner    (1001) docker     (127)     5157 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.616301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.620301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      570 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     2920 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    61362 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    52391 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:00:54.620301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-25 18:00:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-25 18:00:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:00:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 18:00:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 18:00:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-25 18:00:48.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 18:00:54.620301 pulumi_kubernetes_the_hard_way-0.0.26a1716659882/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.886719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4977 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.890719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      864 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    39619 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9584 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5740 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4399 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4531 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     3065 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2560 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2860 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8791 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4826 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5799 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23901 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12558 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    56778 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.898719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1159 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1767 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    26794 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14674 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_service.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)    13465 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    25513 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5199 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
+-rw-------   0 runner    (1001) docker     (127)     5115 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     5187 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
+-rw-------   0 runner    (1001) docker     (127)     5157 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+-rw-------   0 runner    (1001) docker     (127)    43829 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/worker_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.898719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      570 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     2920 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    61362 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    52391 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.26a1716659882
+Version: 0.0.26a1716673050
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/README.md` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,16 @@
    "kubernetes-the-hard-way:remote:ProvisionEtcd": "ProvisionEtcd",
    "kubernetes-the-hard-way:remote:RuncInstall": "RuncInstall",
    "kubernetes-the-hard-way:remote:StartContainerd": "StartContainerd",
    "kubernetes-the-hard-way:remote:StartEtcd": "StartEtcd",
    "kubernetes-the-hard-way:remote:StartKubeProxy": "StartKubeProxy",
    "kubernetes-the-hard-way:remote:StartKubelet": "StartKubelet",
    "kubernetes-the-hard-way:remote:StaticPod": "StaticPod",
-   "kubernetes-the-hard-way:remote:SystemdService": "SystemdService"
+   "kubernetes-the-hard-way:remote:SystemdService": "SystemdService",
+   "kubernetes-the-hard-way:remote:WorkerNode": "WorkerNode"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "tls",
   "fqn": "pulumi_kubernetes_the_hard_way.tls",
   "classes": {
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,24 @@
                  subnet: pulumi.Input[str],
                  bridge: Optional[pulumi.Input[str]] = None,
                  cni_version: Optional[pulumi.Input[str]] = None,
                  ip_masq: Optional[pulumi.Input[bool]] = None,
                  ipam: Optional[pulumi.Input['CniBridgeIpamArgs']] = None,
                  is_gateway: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a CniBridgePluginConfiguration resource.
         :param pulumi.Input[str] subnet: The subnet to use.
         :param pulumi.Input[str] bridge: Bridge name.
         :param pulumi.Input[str] cni_version: CNI version.
         :param pulumi.Input[bool] ip_masq: IP masq.
         :param pulumi.Input['CniBridgeIpamArgs'] ipam: IPAM
         :param pulumi.Input[bool] is_gateway: Is gateway.
         :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
         :param pulumi.Input[str] type: CNI plugin type.
         """
         pulumi.set(__self__, "subnet", subnet)
         if bridge is not None:
             pulumi.set(__self__, "bridge", bridge)
         if cni_version is not None:
             pulumi.set(__self__, "cni_version", cni_version)
@@ -46,16 +44,14 @@
             pulumi.set(__self__, "ip_masq", ip_masq)
         if ipam is not None:
             pulumi.set(__self__, "ipam", ipam)
         if is_gateway is not None:
             pulumi.set(__self__, "is_gateway", is_gateway)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if path is not None:
-            pulumi.set(__self__, "path", path)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def subnet(self) -> pulumi.Input[str]:
         """
@@ -137,26 +133,14 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Path to put the configuration file on the remote system
-        """
-        return pulumi.get(self, "path")
-
-    @path.setter
-    def path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "path", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         CNI plugin type.
         """
         return pulumi.get(self, "type")
 
     @type.setter
@@ -171,30 +155,28 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  bridge: Optional[pulumi.Input[str]] = None,
                  cni_version: Optional[pulumi.Input[str]] = None,
                  ip_masq: Optional[pulumi.Input[bool]] = None,
                  ipam: Optional[pulumi.Input[pulumi.InputType['CniBridgeIpamArgs']]] = None,
                  is_gateway: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  subnet: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Get the `bridge` configuration.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] bridge: Bridge name.
         :param pulumi.Input[str] cni_version: CNI version.
         :param pulumi.Input[bool] ip_masq: IP masq.
         :param pulumi.Input[pulumi.InputType['CniBridgeIpamArgs']] ipam: IPAM
         :param pulumi.Input[bool] is_gateway: Is gateway.
         :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
         :param pulumi.Input[str] subnet: The subnet to use.
         :param pulumi.Input[str] type: CNI plugin type.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -220,15 +202,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  bridge: Optional[pulumi.Input[str]] = None,
                  cni_version: Optional[pulumi.Input[str]] = None,
                  ip_masq: Optional[pulumi.Input[bool]] = None,
                  ipam: Optional[pulumi.Input[pulumi.InputType['CniBridgeIpamArgs']]] = None,
                  is_gateway: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  subnet: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
@@ -240,15 +221,14 @@
 
             __props__.__dict__["bridge"] = bridge
             __props__.__dict__["cni_version"] = cni_version
             __props__.__dict__["ip_masq"] = ip_masq
             __props__.__dict__["ipam"] = ipam
             __props__.__dict__["is_gateway"] = is_gateway
             __props__.__dict__["name"] = name
-            __props__.__dict__["path"] = path
             if subnet is None and not opts.urn:
                 raise TypeError("Missing required property 'subnet'")
             __props__.__dict__["subnet"] = subnet
             __props__.__dict__["type"] = type
             __props__.__dict__["result"] = None
             __props__.__dict__["yaml"] = None
         super(CniBridgePluginConfiguration, __self__).__init__(
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,25 @@
 __all__ = ['CniLoopbackPluginConfigurationArgs', 'CniLoopbackPluginConfiguration']
 
 @pulumi.input_type
 class CniLoopbackPluginConfigurationArgs:
     def __init__(__self__, *,
                  cni_version: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a CniLoopbackPluginConfiguration resource.
         :param pulumi.Input[str] cni_version: CNI version.
         :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
         :param pulumi.Input[str] type: CNI plugin type.
         """
         if cni_version is not None:
             pulumi.set(__self__, "cni_version", cni_version)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if path is not None:
-            pulumi.set(__self__, "path", path)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="cniVersion")
     def cni_version(self) -> Optional[pulumi.Input[str]]:
         """
@@ -57,26 +53,14 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Path to put the configuration file on the remote system
-        """
-        return pulumi.get(self, "path")
-
-    @path.setter
-    def path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "path", value)
-
-    @property
-    @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
         """
         CNI plugin type.
         """
         return pulumi.get(self, "type")
 
     @type.setter
@@ -87,25 +71,23 @@
 class CniLoopbackPluginConfiguration(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cni_version: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Get the `loopback` configuration.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cni_version: CNI version.
         :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
         :param pulumi.Input[str] type: CNI plugin type.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[CniLoopbackPluginConfigurationArgs] = None,
@@ -126,30 +108,28 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cni_version: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CniLoopbackPluginConfigurationArgs.__new__(CniLoopbackPluginConfigurationArgs)
 
             __props__.__dict__["cni_version"] = cni_version
             __props__.__dict__["name"] = name
-            __props__.__dict__["path"] = path
             __props__.__dict__["type"] = type
             __props__.__dict__["result"] = None
             __props__.__dict__["yaml"] = None
         super(CniLoopbackPluginConfiguration, __self__).__init__(
             'kubernetes-the-hard-way:config:CniLoopbackPluginConfiguration',
             resource_name,
             __props__,
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,40 +45,37 @@
 
 def get_cni_bridge_plugin_configuration(bridge: Optional[str] = None,
                                         cni_version: Optional[str] = None,
                                         ip_masq: Optional[bool] = None,
                                         ipam: Optional[pulumi.InputType['CniBridgeIpam']] = None,
                                         is_gateway: Optional[bool] = None,
                                         name: Optional[str] = None,
-                                        path: Optional[str] = None,
                                         subnet: Optional[str] = None,
                                         type: Optional[str] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCniBridgePluginConfigurationResult:
     """
     Get the `bridge` configuration.
 
 
     :param str bridge: Bridge name.
     :param str cni_version: CNI version.
     :param bool ip_masq: IP masq.
     :param pulumi.InputType['CniBridgeIpam'] ipam: IPAM
     :param bool is_gateway: Is gateway.
     :param str name: CNI plugin name.
-    :param str path: Path to put the configuration file on the remote system
     :param str subnet: The subnet to use.
     :param str type: CNI plugin type.
     """
     __args__ = dict()
     __args__['bridge'] = bridge
     __args__['cniVersion'] = cni_version
     __args__['ipMasq'] = ip_masq
     __args__['ipam'] = ipam
     __args__['isGateway'] = is_gateway
     __args__['name'] = name
-    __args__['path'] = path
     __args__['subnet'] = subnet
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('kubernetes-the-hard-way:config:getCniBridgePluginConfiguration', __args__, opts=opts, typ=GetCniBridgePluginConfigurationResult).value
 
     return AwaitableGetCniBridgePluginConfigurationResult(
         result=pulumi.get(__ret__, 'result'))
@@ -87,26 +84,24 @@
 @_utilities.lift_output_func(get_cni_bridge_plugin_configuration)
 def get_cni_bridge_plugin_configuration_output(bridge: Optional[pulumi.Input[Optional[str]]] = None,
                                                cni_version: Optional[pulumi.Input[Optional[str]]] = None,
                                                ip_masq: Optional[pulumi.Input[Optional[bool]]] = None,
                                                ipam: Optional[pulumi.Input[Optional[pulumi.InputType['CniBridgeIpam']]]] = None,
                                                is_gateway: Optional[pulumi.Input[Optional[bool]]] = None,
                                                name: Optional[pulumi.Input[Optional[str]]] = None,
-                                               path: Optional[pulumi.Input[Optional[str]]] = None,
                                                subnet: Optional[pulumi.Input[str]] = None,
                                                type: Optional[pulumi.Input[Optional[str]]] = None,
                                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCniBridgePluginConfigurationResult]:
     """
     Get the `bridge` configuration.
 
 
     :param str bridge: Bridge name.
     :param str cni_version: CNI version.
     :param bool ip_masq: IP masq.
     :param pulumi.InputType['CniBridgeIpam'] ipam: IPAM
     :param bool is_gateway: Is gateway.
     :param str name: CNI plugin name.
-    :param str path: Path to put the configuration file on the remote system
     :param str subnet: The subnet to use.
     :param str type: CNI plugin type.
     """
     ...
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,47 +40,42 @@
             yield self
         return GetCniLoopbackPluginConfigurationResult(
             result=self.result)
 
 
 def get_cni_loopback_plugin_configuration(cni_version: Optional[str] = None,
                                           name: Optional[str] = None,
-                                          path: Optional[str] = None,
                                           type: Optional[str] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCniLoopbackPluginConfigurationResult:
     """
     Get the `loopback` configuration.
 
 
     :param str cni_version: CNI version.
     :param str name: CNI plugin name.
-    :param str path: Path to put the configuration file on the remote system
     :param str type: CNI plugin type.
     """
     __args__ = dict()
     __args__['cniVersion'] = cni_version
     __args__['name'] = name
-    __args__['path'] = path
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('kubernetes-the-hard-way:config:getCniLoopbackPluginConfiguration', __args__, opts=opts, typ=GetCniLoopbackPluginConfigurationResult).value
 
     return AwaitableGetCniLoopbackPluginConfigurationResult(
         result=pulumi.get(__ret__, 'result'))
 
 
 @_utilities.lift_output_func(get_cni_loopback_plugin_configuration)
 def get_cni_loopback_plugin_configuration_output(cni_version: Optional[pulumi.Input[Optional[str]]] = None,
                                                  name: Optional[pulumi.Input[Optional[str]]] = None,
-                                                 path: Optional[pulumi.Input[Optional[str]]] = None,
                                                  type: Optional[pulumi.Input[Optional[str]]] = None,
                                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCniLoopbackPluginConfigurationResult]:
     """
     Get the `loopback` configuration.
 
 
     :param str cni_version: CNI version.
     :param str name: CNI plugin name.
-    :param str path: Path to put the configuration file on the remote system
     :param str type: CNI plugin type.
     """
     ...
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,9 +28,10 @@
 from .runc_install import *
 from .start_containerd import *
 from .start_etcd import *
 from .start_kube_proxy import *
 from .start_kubelet import *
 from .static_pod import *
 from .systemd_service import *
+from .worker_node import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/containerd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_containerd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_containerd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.26a1716659882
+Version: 0.0.26a1716673050
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 pulumi_kubernetes_the_hard_way/remote/runc_install.py
 pulumi_kubernetes_the_hard_way/remote/start_containerd.py
 pulumi_kubernetes_the_hard_way/remote/start_etcd.py
 pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
 pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
 pulumi_kubernetes_the_hard_way/remote/static_pod.py
 pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+pulumi_kubernetes_the_hard_way/remote/worker_node.py
 pulumi_kubernetes_the_hard_way/tls/__init__.py
 pulumi_kubernetes_the_hard_way/tls/_enums.py
 pulumi_kubernetes_the_hard_way/tls/_inputs.py
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
 pulumi_kubernetes_the_hard_way/tls/encryption_key.py
 pulumi_kubernetes_the_hard_way/tls/outputs.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716659882/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.12.0,<5.0.0", "pulumi-random>=4.16.2,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.26a1716659882"
+  version = "0.0.26a1716673050"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

