# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.26a1716673050.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.26a1716684593.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.26a1716673050.tar", last modified: Sat May 25 21:39:54 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.26a1716684593.tar", last modified: Sun May 26 00:52:52 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050.tar` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.886719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4977 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.890719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      864 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    39619 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9584 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     5740 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     4399 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)     4531 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     3065 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     2560 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)     2860 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8791 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4826 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)     5799 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23901 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12558 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    56778 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.898719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1159 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1767 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    26794 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    14674 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_service.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)    13465 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    25513 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5199 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
--rw-------   0 runner    (1001) docker     (127)     5115 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     5187 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
--rw-------   0 runner    (1001) docker     (127)     5157 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
--rw-------   0 runner    (1001) docker     (127)    43829 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/worker_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.898719 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      570 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     2920 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    61362 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    52391 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 21:39:54.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-25 21:39:45.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:39:54.902720 pulumi_kubernetes_the_hard_way-0.0.26a1716673050/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.171073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 00:52:52.171073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.159073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4977 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.163073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      864 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    39619 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9584 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5740 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4399 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4531 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     3065 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2560 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2860 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8791 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4826 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5799 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23901 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12558 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    56778 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.167073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1159 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1767 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    26794 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14674 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/containerd_service.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)    13465 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    25513 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5199 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
+-rw-------   0 runner    (1001) docker     (127)     5115 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     5187 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
+-rw-------   0 runner    (1001) docker     (127)     5157 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+-rw-------   0 runner    (1001) docker     (127)    43829 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/worker_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.167073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.171073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      570 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     2920 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    61362 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    52391 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:52:52.171073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-26 00:52:52.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-05-26 00:52:52.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:52:52.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-26 00:52:52.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-26 00:52:52.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-26 00:52:40.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:52:52.171073 pulumi_kubernetes_the_hard_way-0.0.26a1716684593/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.26a1716673050
+Version: 0.0.26a1716684593
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/README.md` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/containerd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/containerd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_containerd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_containerd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/remote/worker_node.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/remote/worker_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.26a1716673050
+Version: 0.0.26a1716684593
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716673050/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.26a1716684593/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.12.0,<5.0.0", "pulumi-random>=4.16.2,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.26a1716673050"
+  version = "0.0.26a1716684593"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

