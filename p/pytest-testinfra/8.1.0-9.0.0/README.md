# Comparing `tmp/pytest-testinfra-8.1.0.tar.gz` & `tmp/pytest-testinfra-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testinfra-8.1.0.tar", last modified: Sun May 21 15:38:13 2023, max compression
+gzip compressed data, was "pytest-testinfra-9.0.0.tar", last modified: Thu Aug 24 21:57:00 2023, max compression
```

## Comparing `pytest-testinfra-8.1.0.tar` & `pytest-testinfra-9.0.0.tar`

### file list

```diff
@@ -1,108 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/_templates/piwik.html
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/invocation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.916854 pytest-testinfra-8.1.0/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/alpine/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/alpine/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/archlinux/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/archlinux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/debian_bullseye/
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/debian_bullseye/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/rockylinux8/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/rockylinux8/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/ubuntu_xenial/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/ubuntu_xenial/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.924854 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.924854 pytest-testinfra-8.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/ssh_key
--rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/test_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.924854 pytest-testinfra-8.1.0/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.928854 pytest-testinfra-8.1.0/testinfra/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/chroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/lxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/openshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/paramiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/winrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/host.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/testinfra/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/addr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/blockdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/iptables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/mountpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/puppet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/systeminfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/testinfra/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/utils/ansible_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.815958 pytest-testinfra-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (999)      273 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (999)     1696 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)      122 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (999)    11873 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      996 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (999)    10142 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)      523 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)       54 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (999)     3535 2023-08-24 21:57:00.815958 pytest-testinfra-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2283 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       83 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)       36 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.783956 pytest-testinfra-9.0.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (999)     6783 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.791957 pytest-testinfra-9.0.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.791957 pytest-testinfra-9.0.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (999)     9916 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.791957 pytest-testinfra-9.0.0/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (999)      592 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/_templates/piwik.html
+-rw-r--r--   0 runner    (1001) docker     (999)      664 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     7205 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (999)       33 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     9477 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5206 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      192 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     1859 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/invocation.rst
+-rw-r--r--   0 runner    (1001) docker     (999)     4597 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (999)      767 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/doc/source/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.775956 pytest-testinfra-9.0.0/images/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.791957 pytest-testinfra-9.0.0/images/debian_bookworm/
+-rw-r--r--   0 runner    (1001) docker     (999)     3276 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/images/debian_bookworm/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.791957 pytest-testinfra-9.0.0/images/rockylinux9/
+-rw-r--r--   0 runner    (1001) docker     (999)     1470 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/images/rockylinux9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (999)      396 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (999)      240 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.795957 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3535 2023-08-24 21:57:00.000000 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2182 2023-08-24 21:57:00.000000 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 21:57:00.000000 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       49 2023-08-24 21:57:00.000000 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      121 2023-08-24 21:57:00.000000 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       10 2023-08-24 21:57:00.000000 pytest-testinfra-9.0.0/pytest_testinfra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)     1369 2023-08-24 21:57:00.815958 pytest-testinfra-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1072 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.799957 pytest-testinfra-9.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (999)     8757 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1675 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/test/ssh_key
+-rw-r--r--   0 runner    (1001) docker     (999)    21283 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/test/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1963 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/test/test_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20248 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.799957 pytest-testinfra-9.0.0/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (999)      629 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.803957 pytest-testinfra-9.0.0/testinfra/backend/
+-rw-r--r--   0 runner    (1001) docker     (999)     4152 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3079 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9060 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1433 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1288 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/docker.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1945 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1069 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1113 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1788 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5772 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/paramiko.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1288 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/podman.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2567 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/salt.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4975 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3347 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/backend/winrm.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6279 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/host.py
+-rw-r--r--   0 runner    (1001) docker     (999)      711 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/main.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.815958 pytest-testinfra-9.0.0/testinfra/modules/
+-rw-r--r--   0 runner    (1001) docker     (999)     1797 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4739 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/addr.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4185 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1702 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4164 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/blockdevice.py
+-rw-r--r--   0 runner    (1001) docker     (999)      854 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/command.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3766 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/docker.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1019 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/environment.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13494 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/file.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1431 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/group.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5455 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/interface.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2911 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/iptables.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4404 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/mountpoint.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6017 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/package.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4829 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/pip.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2789 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/podman.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6491 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/process.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2985 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/puppet.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1707 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/salt.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8926 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/service.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12705 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/socket.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1584 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5265 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1147 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5839 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/systeminfo.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6524 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/modules/user.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6411 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 21:57:00.815958 pytest-testinfra-9.0.0/testinfra/utils/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13732 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/testinfra/utils/ansible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (999)      838 2023-08-24 21:56:44.000000 pytest-testinfra-9.0.0/tox.ini
```

### Comparing `pytest-testinfra-8.1.0/.pre-commit-config.yaml` & `pytest-testinfra-9.0.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,17 @@
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-debugger
           - flake8-logging-format
           - flake8-pep3101
           - flake8-print
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.4.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         additional_dependencies:
           - types-paramiko
           - types-setuptools
           - setuptools-scm
           - alabaster
+          - pytest
```

### Comparing `pytest-testinfra-8.1.0/CHANGELOG.rst` & `pytest-testinfra-9.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =========
 Changelog
 =========
 
+9.0.0
+=====
+
+* [BREAKING] pytest-testinfra now require python >= 3.9
+* [BREAKING] Drop deprecated module PipPackage
+* [NEW] Add support for the SSH ControlPath connection sharing option (#713)
+* [FIX] Retry SSH on ConnectionResetError (#708)
+* [FIX] List openSUSE Leap and Tumbleweed explicitly as rpm based distributions
+* [FIX] Make group name mandatory in group module
+
 8.1.0
 =====
 
 * [NEW] Add Windows support for File and Service modules
 * [NEW] Add File.is_executable property
 
 8.0.0
```

### Comparing `pytest-testinfra-8.1.0/CONTRIBUTING.rst` & `pytest-testinfra-9.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/LICENSE` & `pytest-testinfra-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/MANIFEST.in` & `pytest-testinfra-9.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/PKG-INFO` & `pytest-testinfra-9.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pytest-testinfra
-Version: 8.1.0
+Version: 9.0.0
 Summary: Test infrastructures
 Home-page: https://github.com/pytest-dev/pytest-testinfra
 Author: Philippe Pepiot
 Author-email: phil@philpep.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Systems Administration
 Classifier: Framework :: Pytest
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: ansible
 Provides-Extra: docker
 Provides-Extra: kubectl
 Provides-Extra: local
 Provides-Extra: lxc
 Provides-Extra: paramiko
```

### Comparing `pytest-testinfra-8.1.0/README.rst` & `pytest-testinfra-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/Makefile` & `pytest-testinfra-9.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/_static/logo.svg` & `pytest-testinfra-9.0.0/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/_templates/piwik.html` & `pytest-testinfra-9.0.0/doc/source/_templates/piwik.html`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/api.rst` & `pytest-testinfra-9.0.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/backends.rst` & `pytest-testinfra-9.0.0/doc/source/backends.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/conf.py` & `pytest-testinfra-9.0.0/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
 import datetime
 import os
 import subprocess
 import sys
-from typing import Dict, List
 
 import alabaster
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath("../.."))
@@ -88,15 +87,15 @@
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns: List[str] = []
+exclude_patterns: list[str] = []
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
@@ -217,15 +216,15 @@
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "testinfradoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
-latex_elements: Dict[str, tuple] = {
+latex_elements: dict[str, tuple[str, ...]] = {
     # The paper size ('letterpaper' or 'a4paper')
     # 'papersize': 'letterpaper',
     # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
     # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
 }
```

### Comparing `pytest-testinfra-8.1.0/doc/source/examples.rst` & `pytest-testinfra-9.0.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/invocation.rst` & `pytest-testinfra-9.0.0/doc/source/invocation.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/doc/source/modules.rst` & `pytest-testinfra-9.0.0/doc/source/modules.rst`

 * *Files 3% similar despite different names*

```diff
@@ -62,18 +62,14 @@
 
        :class:`testinfra.modules.package.Package` class
 
     .. attribute:: pip
 
        :class:`testinfra.modules.pip.Pip` class
 
-    .. attribute:: pip_package
-
-       :class:`testinfra.modules.pip.PipPackage` class
-
     .. attribute:: podman
 
        :class:`testinfra.modules.podman.Podman` class
 
     .. attribute:: process
 
        :class:`testinfra.modules.process.Process` class
@@ -200,20 +196,14 @@
 Pip
 ~~~~~~~~~~
 
 .. autoclass:: testinfra.modules.pip.Pip
    :members:
 
 
-PipPackage
-~~~~~~~~~~
-
-.. autoclass:: testinfra.modules.pip.PipPackage
-
-
 Podman
 ~~~~~~
 
 .. autoclass:: testinfra.modules.podman.Podman(name)
    :members:
```

### Comparing `pytest-testinfra-8.1.0/doc/source/support.rst` & `pytest-testinfra-9.0.0/doc/source/support.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/images/debian_bullseye/Dockerfile` & `pytest-testinfra-9.0.0/images/debian_bookworm/Dockerfile`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-FROM debian:bullseye
+FROM debian:bookworm
 
 ENV container docker
 
-# ntpd is linked to /bin/false, so the service is not running but is enabled
 RUN apt-get update && \
     DEBIAN_FRONTEND=noninteractive apt-get -y install --no-install-recommends \
     lsb-release \
-    python3 \
+    python3-pip \
     openssh-server \
     puppet \
-    salt-minion \
     locales \
-    ntp \
     sudo \
     supervisor \
     systemd-sysv \
     virtualenv \
     iproute2 \
     iputils-ping \
     iptables \
@@ -25,19 +22,16 @@
     (cd /lib/systemd/system/sysinit.target.wants/; for i in *; do if ! test $i = systemd-tmpfiles-setup.service; then rm -f $i; fi; done) && \
     rm -f /lib/systemd/system/multi-user.target.wants/* && \
     rm -f /etc/systemd/system/*.wants/* && \
     rm -f /lib/systemd/system/local-fs.target.wants/* && \
     rm -f /lib/systemd/system/sockets.target.wants/*udev* && \
     rm -f /lib/systemd/system/sockets.target.wants/*initctl* && \
     systemctl enable ssh.service && \
-    systemctl disable salt-minion.service && \
-    systemctl enable ntp.service && \
     systemctl enable supervisor.service && \
     systemctl enable netfilter-persistent.service && \
-    ln -fsn /bin/false /usr/sbin/ntpd && \
     echo "python3 hold" | dpkg --set-selections && \
     echo "LANG=fr_FR.ISO-8859-15" > /etc/default/locale && \
     echo "LANGUAGE=fr_FR" >> /etc/default/locale && \
     echo "fr_FR.ISO-8859-15 ISO-8859-15" >> /etc/locale.gen && \
     locale-gen && \
     update-locale && \
     useradd -m user -c "gecos.comment" && \
@@ -65,14 +59,17 @@
 
 # Expiration date for user "user"
 RUN chage -E 20000 -m 7 -M 90 user
 
 # Some python3 virtualenv
 RUN virtualenv /v
 RUN /v/bin/pip install -U pip
-RUN /v/bin/pip install 'requests>1,<2'
+RUN /v/bin/pip install 'requests==2.30.0'
+
+# install salt
+RUN python3 -m pip install --break-system-packages --no-cache salt
 
 ENV LANG fr_FR.ISO-8859-15
 ENV LANGUAGE fr_FR
 
 EXPOSE 22
 CMD ["/sbin/init"]
```

### Comparing `pytest-testinfra-8.1.0/images/rockylinux8/Dockerfile` & `pytest-testinfra-9.0.0/images/rockylinux9/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-FROM rockylinux:8
+FROM rockylinux:9
 
-RUN dnf -y install openssh-server procps python39 && dnf clean all &&\
+RUN dnf -y install openssh-server procps python311 iputils && dnf clean all &&\
     (cd /lib/systemd/system/sysinit.target.wants/; for i in *; do if ! test $i = systemd-tmpfiles-setup.service; then rm -f $i; fi; done) && \
     rm -f /lib/systemd/system/multi-user.target.wants/* && \
     rm -f /etc/systemd/system/*.wants/* && \
     rm -f /lib/systemd/system/local-fs.target.wants/* && \
     rm -f /lib/systemd/system/sockets.target.wants/*udev* && \
     rm -f /lib/systemd/system/sockets.target.wants/*initctl* && \
     rm -f /lib/systemd/system/basic.target.wants/* && \
```

### Comparing `pytest-testinfra-8.1.0/pytest_testinfra.egg-info/PKG-INFO` & `pytest-testinfra-9.0.0/pytest_testinfra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pytest-testinfra
-Version: 8.1.0
+Version: 9.0.0
 Summary: Test infrastructures
 Home-page: https://github.com/pytest-dev/pytest-testinfra
 Author: Philippe Pepiot
 Author-email: phil@philpep.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Systems Administration
 Classifier: Framework :: Pytest
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: ansible
 Provides-Extra: docker
 Provides-Extra: kubectl
 Provides-Extra: local
 Provides-Extra: lxc
 Provides-Extra: paramiko
```

### Comparing `pytest-testinfra-8.1.0/pytest_testinfra.egg-info/SOURCES.txt` & `pytest-testinfra-9.0.0/pytest_testinfra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .flake8
 .pre-commit-config.yaml
+.readthedocs.yaml
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 ansible.cfg
@@ -22,19 +23,16 @@
 doc/source/examples.rst
 doc/source/index.rst
 doc/source/invocation.rst
 doc/source/modules.rst
 doc/source/support.rst
 doc/source/_static/logo.svg
 doc/source/_templates/piwik.html
-images/alpine/Dockerfile
-images/archlinux/Dockerfile
-images/debian_bullseye/Dockerfile
-images/rockylinux8/Dockerfile
-images/ubuntu_xenial/Dockerfile
+images/debian_bookworm/Dockerfile
+images/rockylinux9/Dockerfile
 pytest_testinfra.egg-info/PKG-INFO
 pytest_testinfra.egg-info/SOURCES.txt
 pytest_testinfra.egg-info/dependency_links.txt
 pytest_testinfra.egg-info/entry_points.txt
 pytest_testinfra.egg-info/requires.txt
 pytest_testinfra.egg-info/top_level.txt
 test/conftest.py
```

### Comparing `pytest-testinfra-8.1.0/setup.cfg` & `pytest-testinfra-9.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 name = pytest-testinfra
 url = https://github.com/pytest-dev/pytest-testinfra
 description = Test infrastructures
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = Philippe Pepiot
 author_email = phil@philpep.org
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Testing
 	Topic :: System :: Systems Administration
 	Framework :: Pytest
 
 [options]
 use_scm_version = True
-python_requires = >=3.8
+python_requires = >=3.9
 packages = find:
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	pytest!=3.0.2
 extras_require =
```

### Comparing `pytest-testinfra-8.1.0/setup.py` & `pytest-testinfra-9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/test/conftest.py` & `pytest-testinfra-9.0.0/test/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,16 @@
 6436653132383662623364313438376662666135346266370a343934663431363661393363386633
 64656261336662623036373036363535313964313538366533313334366363613435303066316639
 3235393661656230350a326264356530326432393832353064363439393330616634633761393838
 3261
 """
 
 DOCKER_IMAGES = [
-    "alpine",
-    "archlinux",
-    "rockylinux8",
-    "debian_bullseye",
-    "ubuntu_xenial",
+    "rockylinux9",
+    "debian_bookworm",
 ]
 
 
 def setup_ansible_config(tmpdir, name, host, user, port, key):
     items = [
         name,
         "ansible_ssh_private_key_file={}".format(key),
@@ -183,17 +180,15 @@
                 ).format(hostname, docker_host, port, str(key))
             )
             kw["ssh_config"] = str(ssh_config)
 
         # Wait ssh to be up
         service = testinfra.get_host(docker_id, connection="docker").service
 
-        images_with_sshd = ("rockylinux8", "alpine", "archlinux")
-
-        if image in images_with_sshd:
+        if image == "rockylinux9":
             service_name = "sshd"
         else:
             service_name = "ssh"
 
         while not service(service_name).is_running:
             time.sleep(0.5)
 
@@ -216,15 +211,15 @@
     if "host" in metafunc.fixturenames:
         for marker in getattr(metafunc.function, "pytestmark", []):
             if marker.name == "testinfra_hosts":
                 hosts = marker.args
                 break
         else:
             # Default
-            hosts = ["docker://debian_bullseye"]
+            hosts = ["docker://debian_bookworm"]
         metafunc.parametrize("host", hosts, indirect=True, scope="function")
 
 
 def pytest_configure(config):
     if not has_docker():
         return
```

### Comparing `pytest-testinfra-8.1.0/test/ssh_key` & `pytest-testinfra-9.0.0/test/ssh_key`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/test/test_backends.py` & `pytest-testinfra-9.0.0/test/test_backends.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,44 +19,44 @@
 import testinfra
 import testinfra.backend
 from testinfra.backend.base import BaseBackend, HostSpec
 from testinfra.backend.winrm import _quote
 from testinfra.utils.ansible_runner import AnsibleRunner
 
 HOSTS = [
-    "ssh://debian_bullseye",
-    "safe-ssh://debian_bullseye",
-    "docker://debian_bullseye",
-    "paramiko://debian_bullseye",
-    "ansible://debian_bullseye",
-    "ansible://debian_bullseye?force_ansible=True",
+    "ssh://debian_bookworm",
+    "safe-ssh://debian_bookworm",
+    "docker://debian_bookworm",
+    "paramiko://debian_bookworm",
+    "ansible://debian_bookworm",
+    "ansible://debian_bookworm?force_ansible=True",
 ]
 USER_HOSTS = [
-    "ssh://user@debian_bullseye",
-    "safe-ssh://user@debian_bullseye",
-    "docker://user@debian_bullseye",
-    "paramiko://user@debian_bullseye",
-    "ansible://user@debian_bullseye",
-    "ansible://user@debian_bullseye?force_ansible=True",
+    "ssh://user@debian_bookworm",
+    "safe-ssh://user@debian_bookworm",
+    "docker://user@debian_bookworm",
+    "paramiko://user@debian_bookworm",
+    "ansible://user@debian_bookworm",
+    "ansible://user@debian_bookworm?force_ansible=True",
 ]
 SUDO_HOSTS = [
-    "ssh://user@debian_bullseye?sudo=True",
-    "safe-ssh://user@debian_bullseye?sudo=True",
-    "docker://user@debian_bullseye?sudo=True",
-    "paramiko://user@debian_bullseye?sudo=True",
-    "ansible://user@debian_bullseye?sudo=True",
-    "ansible://user@debian_bullseye?force_ansible=True&sudo=True",
+    "ssh://user@debian_bookworm?sudo=True",
+    "safe-ssh://user@debian_bookworm?sudo=True",
+    "docker://user@debian_bookworm?sudo=True",
+    "paramiko://user@debian_bookworm?sudo=True",
+    "ansible://user@debian_bookworm?sudo=True",
+    "ansible://user@debian_bookworm?force_ansible=True&sudo=True",
 ]
 SUDO_USER_HOSTS = [
-    "ssh://debian_bullseye?sudo=True&sudo_user=user",
-    "safe-ssh://debian_bullseye?sudo=True&sudo_user=user",
-    "docker://debian_bullseye?sudo=True&sudo_user=user",
-    "paramiko://debian_bullseye?sudo=True&sudo_user=user",
-    "ansible://debian_bullseye?sudo=True&sudo_user=user",
-    "ansible://debian_bullseye?force_ansible=True&sudo=True&sudo_user=user",
+    "ssh://debian_bookworm?sudo=True&sudo_user=user",
+    "safe-ssh://debian_bookworm?sudo=True&sudo_user=user",
+    "docker://debian_bookworm?sudo=True&sudo_user=user",
+    "paramiko://debian_bookworm?sudo=True&sudo_user=user",
+    "ansible://debian_bookworm?sudo=True&sudo_user=user",
+    "ansible://debian_bookworm?force_ansible=True&sudo=True&sudo_user=user",
 ]
 
 
 @pytest.mark.testinfra_hosts(*(HOSTS + USER_HOSTS + SUDO_HOSTS + SUDO_USER_HOSTS))
 def test_command(host):
     assert host.check_output("true") == ""
     # test that quotting is correct
@@ -71,15 +71,15 @@
         assert out.stderr_bytes == b"err\n"
     out = host.run("commandthatdoesnotexists")
     assert out.rc == 127
 
 
 @pytest.mark.testinfra_hosts(*HOSTS)
 def test_encoding(host):
-    # bullseye image is fr_FR@ISO-8859-15
+    # bookworm image is fr_FR@ISO-8859-15
     cmd = host.run("ls -l %s", "/é")
     if host.backend.get_connection_type() == "docker":
         # docker bug ?
         assert cmd.stderr_bytes == (
             b"ls: impossible d'acc\xe9der \xe0 '/\xef\xbf\xbd': "
             b"Aucun fichier ou dossier de ce type\n"
         )
@@ -95,15 +95,15 @@
             b"Aucun fichier ou dossier de ce type\n"
         )
         assert cmd.stderr == (
             "ls: impossible d'accéder à '/é': " "Aucun fichier ou dossier de ce type\n"
         )
 
 
-@pytest.mark.testinfra_hosts("ansible://debian_bullseye?force_ansible=True")
+@pytest.mark.testinfra_hosts("ansible://debian_bookworm?force_ansible=True")
 def test_ansible_any_error_fatal(host):
     os.environ["ANSIBLE_ANY_ERRORS_FATAL"] = "True"
     try:
         out = host.run("echo out && echo err >&2 && exit 42")
         assert out.rc == 42
         assert out.stdout == "out"
         assert out.stderr == "err"
@@ -481,15 +481,15 @@
     # just check that all declared backend are importable and NAME is set
     # correctly
     for connection_type in testinfra.backend.BACKENDS:
         obj = testinfra.backend.get_backend_class(connection_type)
         assert obj.get_connection_type() == connection_type
 
 
-@pytest.mark.testinfra_hosts("docker://rockylinux8", "ssh://rockylinux8")
+@pytest.mark.testinfra_hosts("docker://rockylinux9", "ssh://rockylinux9")
 def test_docker_encoding(host):
     encoding = host.check_output(
         "python3 -c 'import locale;print(locale.getpreferredencoding())'"
     )
     assert encoding == "UTF-8"
     string = "ťēꞩƫìṇḟřặ ṧꝕèȃǩ ửƫᵮ8"
     assert host.check_output("echo %s | tee /tmp/s.txt", string) == string
```

### Comparing `pytest-testinfra-8.1.0/test/test_invocation.py` & `pytest-testinfra-9.0.0/test/test_invocation.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/test/test_modules.py` & `pytest-testinfra-9.0.0/test/test_modules.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,74 +21,63 @@
 
 from testinfra.modules.socket import parse_socketspec
 
 all_images = pytest.mark.testinfra_hosts(
     *[
         "docker://{}".format(image)
         for image in (
-            "alpine",
-            "archlinux",
-            "rockylinux8",
-            "debian_bullseye",
-            "ubuntu_xenial",
+            "rockylinux9",
+            "debian_bookworm",
         )
     ]
 )
 
 
 @all_images
 def test_package(host, docker_image):
     assert not host.package("zsh").is_installed
-    if docker_image in ("alpine", "archlinux"):
-        name = "openssh"
-    else:
-        name = "openssh-server"
-
-    ssh = host.package(name)
+    ssh = host.package("openssh-server")
     version = {
-        "alpine": "8.",
-        "archlinux": "9.",
-        "rockylinux8": "8.",
-        "debian_bullseye": "1:8.4",
-        "ubuntu_xenial": "1:7.2",
+        "rockylinux9": "8.",
+        "debian_bookworm": "1:9.2",
     }[docker_image]
     assert ssh.is_installed
     assert ssh.version.startswith(version)
     release = {
-        "alpine": "r3",
-        "archlinux": None,
-        "rockylinux8": ".el8",
-        "debian_bullseye": None,
-        "ubuntu_xenial": None,
+        "rockylinux9": ".el9",
+        "debian_bookworm": None,
     }[docker_image]
     if release is None:
         with pytest.raises(NotImplementedError):
             ssh.release
     else:
         assert release in ssh.release
 
 
 def test_held_package(host):
     python = host.package("python3")
     assert python.is_installed
-    assert python.version.startswith("3.9.")
+    assert python.version.startswith("3.11.")
 
 
-@pytest.mark.testinfra_hosts("docker://rockylinux8")
+@pytest.mark.testinfra_hosts("docker://rockylinux9")
 def test_non_default_package_tool(host):
     # Make non default pkg tool binary present
     host.run("install -m a+rx /bin/true /usr/bin/dpkg-query")
     assert host.package("openssh").is_installed
 
 
 @pytest.mark.destructive
 def test_uninstalled_package_version(host):
     with pytest.raises(AssertionError) as excinfo:
         host.package("zsh").version
-    assert "Unexpected exit code 1 for CommandResult" in str(excinfo.value)
+    assert (
+        "The package zsh is not installed, dpkg-query output: unknown ok not-installed"
+        in str(excinfo.value)
+    )
     assert host.package("sudo").is_installed
     host.check_output("apt-get -y remove sudo")
     assert not host.package("sudo").is_installed
     with pytest.raises(AssertionError) as excinfo:
         host.package("sudo").version
     assert (
         "The package sudo is not installed, dpkg-query output: "
@@ -97,98 +86,63 @@
 
 
 @all_images
 def test_systeminfo(host, docker_image):
     assert host.system_info.type == "linux"
 
     release, distribution, codename, arch = {
-        "alpine": (r"^3\.14\.", "alpine", None, "x86_64"),
-        "archlinux": ("rolling", "arch", None, "x86_64"),
-        "rockylinux8": (r"^8.\d+$", "rocky", None, "x86_64"),
-        "debian_bullseye": (r"^11", "debian", "bullseye", "x86_64"),
-        "ubuntu_xenial": (r"^16\.04$", "ubuntu", "xenial", "x86_64"),
+        "rockylinux9": (r"^9.\d+$", "rocky", None, "x86_64"),
+        "debian_bookworm": (r"^12", "debian", "bookworm", "x86_64"),
     }[docker_image]
 
     assert host.system_info.distribution == distribution
     assert host.system_info.codename == codename
     assert re.match(release, host.system_info.release)
 
 
 @all_images
 def test_ssh_service(host, docker_image):
-    if docker_image in ("rockylinux8", "alpine", "archlinux"):
+    if docker_image == "rockylinux9":
         name = "sshd"
     else:
         name = "ssh"
 
     ssh = host.service(name)
-    if docker_image == "ubuntu_xenial":
-        assert not ssh.is_running
+    # wait at max 10 seconds for ssh is running
+    for _ in range(10):
+        if ssh.is_running:
+            break
+        time.sleep(1)
     else:
-        # wait at max 10 seconds for ssh is running
-        for _ in range(10):
-            if ssh.is_running:
-                break
-            time.sleep(1)
-        else:
-            if docker_image == "archlinux":
-                raise pytest.skip("FIXME: flapping test")
-            raise AssertionError("ssh is not running")
+        raise AssertionError("ssh is not running")
 
-    if docker_image == "ubuntu_xenial":
-        assert not ssh.is_enabled
-    else:
-        assert ssh.is_enabled
+    assert ssh.is_enabled
 
 
 def test_service_systemd_mask(host):
     ssh = host.service("ssh")
     assert not ssh.is_masked
     host.run("systemctl mask ssh")
     assert ssh.is_masked
     host.run("systemctl unmask ssh")
     assert not ssh.is_masked
 
 
-@pytest.mark.parametrize(
-    "name,running,enabled",
-    [
-        ("ntp", False, True),
-        ("salt-minion", False, False),
-    ],
-)
-def test_service(host, name, running, enabled):
-    service = host.service(name)
-    assert service.is_running == running
-    assert service.is_enabled == enabled
-    # check with systemd_properties
-    assert (
-        service.systemd_properties["UnitFileState"] == "enabled"
-        if enabled
-        else "disabled"
-    )
-    assert (
-        service.systemd_properties["ActiveState"] in ["active"]
-        if running
-        else ["failed", "inactive"]
-    )
-
-
 def test_salt(host):
     ssh_version = host.salt("pkg.version", "openssh-server", local=True)
-    assert ssh_version.startswith("1:8.4")
+    assert ssh_version.startswith("1:9.2")
 
 
 def test_puppet_resource(host):
     resource = host.puppet_resource("package", "openssh-server")
-    assert resource["openssh-server"]["ensure"].startswith("1:8.4")
+    assert resource["openssh-server"]["ensure"].startswith("1:9.2")
 
 
 def test_facter(host):
-    assert host.facter()["os"]["distro"]["codename"] == "bullseye"
+    assert host.facter()["os"]["distro"]["codename"] == "bookworm"
     assert host.facter("virtual") in (
         {"virtual": "docker"},
         {"virtual": "hyperv"},  # github action uses hyperv
         {"virtual": "physical"},  # I've this on my machine...
     )
 
 
@@ -238,42 +192,37 @@
             assert len(host.socket(spec).clients) >= 1
 
 
 @all_images
 def test_process(host, docker_image):
     init = host.process.get(pid=1)
     assert init.ppid == 0
-    if docker_image != "alpine":
-        # busybox ps doesn't have a euid equivalent
-        assert init.euid == 0
+    assert init.euid == 0
     assert init.user == "root"
 
     args, comm = {
-        "alpine": ("/sbin/init", "init"),
-        "archlinux": ("/usr/sbin/init", "systemd"),
-        "rockylinux8": ("/usr/sbin/init", "systemd"),
-        "debian_bullseye": ("/sbin/init", "systemd"),
-        "ubuntu_xenial": ("/sbin/init", "systemd"),
+        "rockylinux9": ("/usr/sbin/init", "systemd"),
+        "debian_bookworm": ("/sbin/init", "systemd"),
     }[docker_image]
     assert init.args == args
     assert init.comm == comm
 
 
 def test_user(host):
     user = host.user("sshd")
     assert user.exists
     assert user.name == "sshd"
-    assert user.uid == 104
+    assert user.uid == 100
     assert user.gid == 65534
     assert user.group == "nogroup"
     assert user.gids == [65534]
     assert user.groups == ["nogroup"]
     assert user.shell == "/usr/sbin/nologin"
     assert user.home == "/run/sshd"
-    assert user.password == "*"
+    assert user.password == "!"
 
 
 def test_user_password_days(host):
     assert host.user("root").password_max_days == 99999
     assert host.user("root").password_min_days == 0
     assert host.user("user").password_max_days == 90
     assert host.user("user").password_min_days == 7
@@ -374,18 +323,18 @@
         host.ansible("setup")
     assert expected in str(excinfo.value)
     with pytest.raises(RuntimeError) as excinfo:
         host.ansible.get_variables()
     assert expected in str(excinfo.value)
 
 
-@pytest.mark.testinfra_hosts("ansible://debian_bullseye")
+@pytest.mark.testinfra_hosts("ansible://debian_bookworm")
 def test_ansible_module(host):
     setup = host.ansible("setup")["ansible_facts"]
-    assert setup["ansible_lsb"]["codename"] == "bullseye"
+    assert setup["ansible_lsb"]["codename"] == "bookworm"
     passwd = host.ansible("file", "path=/etc/passwd state=file")
     assert passwd["changed"] is False
     assert passwd["gid"] == 0
     assert passwd["group"] == "root"
     assert passwd["mode"] == "0644"
     assert passwd["owner"] == "root"
     assert isinstance(passwd["size"], int)
@@ -394,38 +343,38 @@
     assert passwd["state"] in ("file", "hard")
     assert passwd["uid"] == 0
 
     variables = host.ansible.get_variables()
     assert variables["myvar"] == "foo"
     assert variables["myhostvar"] == "bar"
     assert variables["mygroupvar"] == "qux"
-    assert variables["inventory_hostname"] == "debian_bullseye"
+    assert variables["inventory_hostname"] == "debian_bookworm"
     assert variables["group_names"] == ["testgroup"]
     assert variables["groups"] == {
-        "all": ["debian_bullseye"],
-        "testgroup": ["debian_bullseye"],
+        "all": ["debian_bookworm"],
+        "testgroup": ["debian_bookworm"],
     }
 
     with pytest.raises(host.ansible.AnsibleException) as excinfo:
         host.ansible("command", "zzz")
     assert excinfo.value.result["msg"] == "Skipped. You might want to try check=False"
 
     try:
         host.ansible("command", "zzz", check=False)
     except host.ansible.AnsibleException as exc:
         assert exc.result["rc"] == 2
-        # notez que the debian bullseye container is set to LANG=fr_FR
+        # notez que the debian bookworm container is set to LANG=fr_FR
         assert exc.result["msg"] == ("[Errno 2] Aucun fichier ou dossier " "de ce type")
 
     result = host.ansible("command", "echo foo", check=False)
     assert result["stdout"] == "foo"
 
 
 @pytest.mark.testinfra_hosts(
-    "ansible://debian_bullseye", "ansible://user@debian_bullseye"
+    "ansible://debian_bookworm", "ansible://user@debian_bookworm"
 )
 def test_ansible_module_become(host):
     user_name = host.user().name
     assert host.ansible("shell", "echo $USER", check=False)["stdout"] == user_name
     assert (
         host.ansible("shell", "echo $USER", check=False, become=True)["stdout"]
         == "root"
@@ -436,15 +385,15 @@
         assert host.ansible("shell", "echo $USER", check=False)["stdout"] == user_name
         assert (
             host.ansible("shell", "echo $USER", check=False, become=True)["stdout"]
             == "root"
         )
 
 
-@pytest.mark.testinfra_hosts("ansible://debian_bullseye")
+@pytest.mark.testinfra_hosts("ansible://debian_bookworm")
 def test_ansible_module_options(host):
     assert (
         host.ansible(
             "command",
             "id --user --name",
             check=False,
             become=True,
@@ -549,15 +498,15 @@
             assert host.user().name == "unprivileged"
             host.check_output("ls /root/invalid")
     assert str(exc.value).startswith("Unexpected exit code")
     with host.sudo():
         assert host.user().name == "root"
 
 
-@pytest.mark.testinfra_hosts("docker://user@debian_bullseye")
+@pytest.mark.testinfra_hosts("docker://user@debian_bookworm")
 def test_sudo_to_root(host):
     assert host.user().name == "user"
     with host.sudo():
         assert host.user().name == "root"
         # Test nested sudo
         with host.sudo("www-data"):
             assert host.user().name == "www-data"
@@ -567,31 +516,30 @@
 def test_command_execution(host):
     assert host.run("false").failed
     assert host.run("true").succeeded
 
 
 def test_pip(host):
     # get_packages
-    assert host.pip.get_packages()["pip"]["version"] == "20.3.4"
+    assert host.pip.get_packages()["pip"]["version"].startswith("23.")
     pkg = host.pip.get_packages(pip_path="/v/bin/pip")["requests"]
-    assert pkg["version"].startswith("1.")
+    assert pkg["version"] == "2.30.0"
     # outdated
     outdated = host.pip.get_outdated_packages(pip_path="/v/bin/pip")["requests"]
     assert outdated["current"] == pkg["version"]
-    assert int(outdated["latest"].split(".")[0]) >= 1
     # check
     assert host.pip.check().succeeded
     # is_installed
     assert host.pip("pip").is_installed
     assert not host.pip("does_not_exist").is_installed
     pkg = host.pip("requests", pip_path="/v/bin/pip")
     assert pkg.is_installed
     # version
-    assert host.pip("pip").version == "20.3.4"
-    assert pkg.version.startswith("1.")
+    assert host.pip("pip").version.startswith("23.")
+    assert pkg.version == "2.30.0"
     assert host.pip("does_not_exist").version == ""
 
 
 def test_environment_home(host):
     assert host.environment().get("HOME") == "/root"
 
 
@@ -669,15 +617,15 @@
     for ip in google_addr.ipv6_addresses:
         assert isinstance(ip_address(ip), IPv6Address)
 
     for ip in google_addr.ip_addresses:
         assert isinstance(ip_address(ip), (IPv4Address, IPv6Address))
 
 
-@pytest.mark.testinfra_hosts("ansible://debian_bullseye")
+@pytest.mark.testinfra_hosts("ansible://debian_bookworm")
 def test_addr_namespace(host):
     namespace_lookup = host.addr("localhost", "ns1")
     assert not namespace_lookup.namespace_exists
 
 
 @pytest.mark.parametrize(
     "family",
```

### Comparing `pytest-testinfra-8.1.0/testinfra/__init__.py` & `pytest-testinfra-9.0.0/testinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/__init__.py` & `pytest-testinfra-9.0.0/testinfra/backend/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
 import os
 import urllib.parse
+from typing import TYPE_CHECKING, Any, Iterable
+
+if TYPE_CHECKING:
+    import testinfra.backend.base
 
 BACKENDS = {
     "local": "testinfra.backend.local.LocalBackend",
     "ssh": "testinfra.backend.ssh.SshBackend",
     "safe-ssh": "testinfra.backend.ssh.SafeSshBackend",
     "paramiko": "testinfra.backend.paramiko.ParamikoBackend",
     "salt": "testinfra.backend.salt.SaltBackend",
@@ -27,25 +31,25 @@
     "winrm": "testinfra.backend.winrm.WinRMBackend",
     "lxc": "testinfra.backend.lxc.LxcBackend",
     "openshift": "testinfra.backend.openshift.OpenShiftBackend",
     "chroot": "testinfra.backend.chroot.ChrootBackend",
 }
 
 
-def get_backend_class(connection):
+def get_backend_class(connection: str) -> type["testinfra.backend.base.BaseBackend"]:
     try:
         classpath = BACKENDS[connection]
     except KeyError:
         raise RuntimeError("Unknown connection type '{}'".format(connection))
     module, name = classpath.rsplit(".", 1)
-    return getattr(importlib.import_module(module), name)
+    return getattr(importlib.import_module(module), name)  # type: ignore[no-any-return]
 
 
-def parse_hostspec(hostspec):
-    kw = {}
+def parse_hostspec(hostspec: str) -> tuple[str, dict[str, Any]]:
+    kw: dict[str, Any] = {}
     if hostspec is not None and "://" in hostspec:
         url = urllib.parse.urlparse(hostspec)
         kw["connection"] = url.scheme
         host = url.netloc
         query = urllib.parse.parse_qs(url.query)
         for key in ("sudo", "ssl", "no_ssl", "no_verify_ssl", "force_ansible"):
             if query.get(key, ["false"])[0].lower() == "true":
@@ -71,26 +75,28 @@
             if key in query:
                 kw[key] = os.path.expanduser(query[key][0])
     else:
         host = hostspec
     return host, kw
 
 
-def get_backend(hostspec, **kwargs):
+def get_backend(hostspec: str, **kwargs: Any) -> "testinfra.backend.base.BaseBackend":
     host, kw = parse_hostspec(hostspec)
     for k, v in kwargs.items():
         kw.setdefault(k, v)
     kw.setdefault("connection", "paramiko")
     klass = get_backend_class(kw["connection"])
     if kw["connection"] == "local":
         return klass(**kw)
     return klass(host, **kw)
 
 
-def get_backends(hosts, **kwargs):
+def get_backends(
+    hosts: Iterable[str], **kwargs: Any
+) -> list["testinfra.backend.base.BaseBackend"]:
     backends = {}
     for hostspec in hosts:
         host, kw = parse_hostspec(hostspec)
         for k, v in kwargs.items():
             kw.setdefault(k, v)
         connection = kw.get("connection")
         if host is None and connection is None:
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/ansible.py` & `pytest-testinfra-9.0.0/testinfra/backend/ansible.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,47 +8,48 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import pprint
+from typing import Any, Optional
 
 from testinfra.backend import base
 from testinfra.utils.ansible_runner import AnsibleRunner
 
 logger = logging.getLogger("testinfra")
 
 
 class AnsibleBackend(base.BaseBackend):
     NAME = "ansible"
     HAS_RUN_ANSIBLE = True
 
     def __init__(
         self,
-        host,
-        ansible_inventory=None,
-        ssh_config=None,
-        ssh_identity_file=None,
-        force_ansible=False,
-        *args,
-        **kwargs,
+        host: str,
+        ansible_inventory: Optional[str] = None,
+        ssh_config: Optional[str] = None,
+        ssh_identity_file: Optional[str] = None,
+        force_ansible: bool = False,
+        *args: Any,
+        **kwargs: Any,
     ):
         self.host = host
         self.ansible_inventory = ansible_inventory
         self.ssh_config = ssh_config
         self.ssh_identity_file = ssh_identity_file
         self.force_ansible = force_ansible
         super().__init__(host, *args, **kwargs)
 
     @property
-    def ansible_runner(self):
+    def ansible_runner(self) -> AnsibleRunner:
         return AnsibleRunner.get_runner(self.ansible_inventory)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         command = self.get_command(command, *args)
         if not self.force_ansible:
             host = self.ansible_runner.get_host(
                 self.host,
                 ssh_config=self.ssh_config,
                 ssh_identity_file=self.ssh_identity_file,
             )
@@ -60,30 +61,32 @@
             command,
             stdout_bytes=None,
             stderr_bytes=None,
             stdout=out["stdout"],
             stderr=out["stderr"],
         )
 
-    def run_ansible(self, module_name, module_args=None, **kwargs):
-        def get_encoding():
+    def run_ansible(
+        self, module_name: str, module_args: Optional[str] = None, **kwargs: Any
+    ) -> Any:
+        def get_encoding() -> str:
             return self.encoding
 
         result = self.ansible_runner.run_module(
             self.host, module_name, module_args, get_encoding=get_encoding, **kwargs
         )
         logger.info(
             "RUN Ansible(%s, %s, %s): %s",
             repr(module_name),
             repr(module_args),
             repr(kwargs),
             pprint.pformat(result),
         )
         return result
 
-    def get_variables(self):
+    def get_variables(self) -> dict[str, Any]:
         return self.ansible_runner.get_variables(self.host)
 
     @classmethod
-    def get_hosts(cls, host, **kwargs):
+    def get_hosts(cls, host: str, **kwargs: Any) -> list[str]:
         inventory = kwargs.get("ansible_inventory")
         return AnsibleRunner.get_runner(inventory).get_hosts(host or "all")
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/base.py` & `pytest-testinfra-9.0.0/testinfra/backend/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,98 +7,108 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
-import collections
+import dataclasses
 import locale
 import logging
 import shlex
 import subprocess
 import urllib.parse
+from typing import TYPE_CHECKING, Any, Optional
+
+if TYPE_CHECKING:
+    import testinfra.host
 
 logger = logging.getLogger("testinfra")
 
-HostSpec = collections.namedtuple("HostSpec", ["name", "port", "user", "password"])
+
+@dataclasses.dataclass
+class HostSpec:
+    name: str
+    port: Optional[str]
+    user: Optional[str]
+    password: Optional[str]
 
 
 class CommandResult:
     def __init__(
         self,
-        backend,
-        exit_status,
-        command,
-        stdout_bytes,
-        stderr_bytes,
-        stdout=None,
-        stderr=None,
+        backend: "BaseBackend",
+        exit_status: int,
+        command: bytes,
+        stdout_bytes: bytes,
+        stderr_bytes: bytes,
+        stdout: Optional[str] = None,
+        stderr: Optional[str] = None,
     ):
         self.exit_status = exit_status
         self._stdout_bytes = stdout_bytes
         self._stderr_bytes = stderr_bytes
         self._stdout = stdout
         self._stderr = stderr
         self.command = command
         self._backend = backend
         super().__init__()
 
     @property
-    def succeeded(self):
+    def succeeded(self) -> bool:
         """Returns whether the command was successful
 
         >>> host.run("true").succeeded
         True
         """
         return self.exit_status == 0
 
     @property
-    def failed(self):
+    def failed(self) -> bool:
         """Returns whether the command failed
 
         >>> host.run("false").failed
         True
         """
         return self.exit_status != 0
 
     @property
-    def rc(self):
+    def rc(self) -> int:
         """Gets the returncode of a command
 
         >>> host.run("true").rc
         0
         """
         return self.exit_status
 
     @property
-    def stdout(self):
+    def stdout(self) -> str:
         if self._stdout is None:
             self._stdout = self._backend.decode(self._stdout_bytes)
         return self._stdout
 
     @property
-    def stderr(self):
+    def stderr(self) -> str:
         if self._stderr is None:
             self._stderr = self._backend.decode(self._stderr_bytes)
         return self._stderr
 
     @property
-    def stdout_bytes(self):
+    def stdout_bytes(self) -> bytes:
         if self._stdout_bytes is None:
             self._stdout_bytes = self._backend.encode(self._stdout)
         return self._stdout_bytes
 
     @property
-    def stderr_bytes(self):
+    def stderr_bytes(self) -> bytes:
         if self._stderr_bytes is None:
             self._stderr_bytes = self._backend.encode(self._stderr)
         return self._stderr_bytes
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             "CommandResult(command={!r}, exit_status={}, stdout={!r}, " "stderr={!r})"
         ).format(
             self.command,
             self.exit_status,
             self._stdout_bytes or self._stdout,
             self._stderr_bytes or self._stderr,
@@ -108,34 +118,41 @@
 class BaseBackend(metaclass=abc.ABCMeta):
     """Represent the connection to the remote or local system"""
 
     HAS_RUN_SALT = False
     HAS_RUN_ANSIBLE = False
     NAME: str
 
-    def __init__(self, hostname, sudo=False, sudo_user=None, *args, **kwargs):
-        self._encoding = None
-        self._host = None
+    def __init__(
+        self,
+        hostname: str,
+        sudo: bool = False,
+        sudo_user: Optional[str] = None,
+        *args: Any,
+        **kwargs: Any,
+    ):
+        self._encoding: Optional[str] = None
+        self._host: Optional["testinfra.host.Host"] = None
         self.hostname = hostname
         self.sudo = sudo
         self.sudo_user = sudo_user
         super().__init__()
 
-    def set_host(self, host):
+    def set_host(self, host: "testinfra.host.Host") -> None:
         self._host = host
 
     @classmethod
-    def get_connection_type(cls):
+    def get_connection_type(cls) -> str:
         """Return the connection backend used as string.
 
         Can be local, paramiko, ssh, docker, salt or ansible
         """
         return cls.NAME
 
-    def get_hostname(self):
+    def get_hostname(self) -> str:
         """Return the hostname (for testinfra) of the remote or local system
 
 
         Can be useful for multi-hosts tests:
 
         Example:
         ::
@@ -154,63 +171,63 @@
             $ testinfra --hosts=server1,server2 test.py
 
             test.py::test[paramiko://server1] PASSED
             test.py::test[paramiko://server2] PASSED
         """
         return self.hostname
 
-    def get_pytest_id(self):
+    def get_pytest_id(self) -> str:
         return self.get_connection_type() + "://" + self.get_hostname()
 
     @classmethod
-    def get_hosts(cls, host, **kwargs):
+    def get_hosts(cls, host: str, **kwargs: Any) -> list[str]:
         if host is None:
             raise RuntimeError(
                 "One or more hosts is required with the {} backend".format(
                     cls.get_connection_type()
                 )
             )
         return [host]
 
     @staticmethod
-    def quote(command, *args):
+    def quote(command: str, *args: str) -> str:
         if args:
             return command % tuple(shlex.quote(a) for a in args)  # noqa: S001
         return command
 
-    def get_sudo_command(self, command, sudo_user):
+    def get_sudo_command(self, command: str, sudo_user: Optional[str]) -> str:
         if sudo_user is None:
             return self.quote("sudo /bin/sh -c %s", command)
         return self.quote("sudo -u %s /bin/sh -c %s", sudo_user, command)
 
-    def get_command(self, command, *args):
+    def get_command(self, command: str, *args: str) -> str:
         command = self.quote(command, *args)
         if self.sudo:
             command = self.get_sudo_command(command, self.sudo_user)
         return command
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> CommandResult:
         raise NotImplementedError
 
-    def run_local(self, command, *args):
+    def run_local(self, command: str, *args: str) -> CommandResult:
         command = self.quote(command, *args)
-        command = self.encode(command)
+        cmd = self.encode(command)
         p = subprocess.Popen(
-            command,
+            cmd,
             shell=True,
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         stdout, stderr = p.communicate()
-        result = self.result(p.returncode, command, stdout, stderr)
+        result = self.result(p.returncode, cmd, stdout, stderr)
         return result
 
     @staticmethod
-    def parse_hostspec(hostspec):
+    def parse_hostspec(hostspec: str) -> HostSpec:
         name = hostspec
         port = None
         user = None
         password = None
         if "@" in name:
             user, name = name.split("@", 1)
             if ":" in user:
@@ -234,15 +251,15 @@
         if user is not None:
             user = urllib.parse.unquote(user)
         if password is not None:
             password = urllib.parse.unquote(password)
         return HostSpec(name, port, user, password)
 
     @staticmethod
-    def parse_containerspec(containerspec):
+    def parse_containerspec(containerspec: str) -> tuple[str, Optional[str]]:
         name = containerspec
         user = None
         if "@" in name:
             user, name = name.split("@", 1)
         return name, user
 
     def get_encoding(self) -> str:
@@ -262,28 +279,28 @@
             encoding = locale.getpreferredencoding()
         if encoding == "ANSI_X3.4-1968":
             # Workaround default encoding ascii without LANG set
             encoding = "UTF-8"
         return encoding
 
     @property
-    def encoding(self):
+    def encoding(self) -> str:
         if self._encoding is None:
             self._encoding = self.get_encoding()
         return self._encoding
 
-    def decode(self, data):
+    def decode(self, data: bytes) -> str:
         try:
             return data.decode("ascii")
         except UnicodeDecodeError:
             return data.decode(self.encoding)
 
-    def encode(self, data):
+    def encode(self, data: str) -> bytes:
         try:
             return data.encode("ascii")
         except UnicodeEncodeError:
             return data.encode(self.encoding)
 
-    def result(self, *args, **kwargs):
+    def result(self, *args: Any, **kwargs: Any) -> CommandResult:
         result = CommandResult(self, *args, **kwargs)
         logger.debug("RUN %s", result)
         return result
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/chroot.py` & `pytest-testinfra-9.0.0/testinfra/backend/lxc.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,34 +5,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import os.path
-
-from testinfra.backend import base
 
+from typing import Any
 
-class ChrootBackend(base.BaseBackend):
-    """Run commands in a chroot folder
+from testinfra.backend import base
 
-    Requires root access or sudo
-    Can be invoked by --hosts=/path/to/chroot/ --connection=chroot --sudo
-    """
 
-    NAME = "chroot"
+class LxcBackend(base.BaseBackend):
+    NAME = "lxc"
 
-    def __init__(self, name, *args, **kwargs):
+    def __init__(self, name: str, *args: Any, **kwargs: Any):
         self.name = name
         super().__init__(self.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
-        if not os.path.exists(self.name) and os.path.isdir(self.name):
-            raise RuntimeError(
-                "chroot path {} not found or not a directory".format(self.name)
-            )
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         cmd = self.get_command(command, *args)
-        out = self.run_local("chroot %s /bin/sh -c %s", self.name, cmd)
+        out = self.run_local(
+            "lxc exec %s --mode=non-interactive -- " "/bin/sh -c %s", self.name, cmd
+        )
         out.command = self.encode(cmd)
         return out
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/docker.py` & `pytest-testinfra-9.0.0/testinfra/backend/docker.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from testinfra.backend import base
 
 
 class DockerBackend(base.BaseBackend):
     NAME = "docker"
 
-    def __init__(self, name, *args, **kwargs):
+    def __init__(self, name: str, *args: Any, **kwargs: Any):
         self.name, self.user = self.parse_containerspec(name)
         super().__init__(self.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         cmd = self.get_command(command, *args)
         if self.user is not None:
             out = self.run_local(
                 "docker exec -u %s %s /bin/sh -c %s", self.user, self.name, cmd
             )
         else:
             out = self.run_local("docker exec %s /bin/sh -c %s", self.name, cmd)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/kubectl.py` & `pytest-testinfra-9.0.0/testinfra/backend/kubectl.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from testinfra.backend import base
 
 
 class KubectlBackend(base.BaseBackend):
     NAME = "kubectl"
 
-    def __init__(self, name, *args, **kwargs):
+    def __init__(self, name: str, *args: Any, **kwargs: Any):
         self.name = name
         self.container = kwargs.get("container")
         self.namespace = kwargs.get("namespace")
         self.kubeconfig = kwargs.get("kubeconfig")
         self.context = kwargs.get("context")
         super().__init__(self.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         cmd = self.get_command(command, *args)
         # `kubectl exec` does not support specifying the user to run as.
         # See https://github.com/kubernetes/kubernetes/issues/30656
         kcmd = "kubectl "
         kcmd_args = []
         if self.kubeconfig is not None:
             kcmd += '--kubeconfig="%s" '
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/local.py` & `pytest-testinfra-9.0.0/testinfra/backend/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from testinfra.backend import base
 
 
 class LocalBackend(base.BaseBackend):
     NAME = "local"
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any):
         super().__init__("local", **kwargs)
 
-    def get_pytest_id(self):
+    def get_pytest_id(self) -> str:
         return "local"
 
     @classmethod
-    def get_hosts(cls, host, **kwargs):
+    def get_hosts(cls, host: str, **kwargs: Any) -> list[str]:
         return [host]
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         return self.run_local(self.get_command(command, *args))
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/openshift.py` & `pytest-testinfra-9.0.0/testinfra/backend/openshift.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from testinfra.backend import base
 
 
 class OpenShiftBackend(base.BaseBackend):
     NAME = "openshift"
 
-    def __init__(self, name, *args, **kwargs):
+    def __init__(self, name: str, *args: Any, **kwargs: Any):
         self.name = name
         self.container = kwargs.get("container")
         self.namespace = kwargs.get("namespace")
         self.kubeconfig = kwargs.get("kubeconfig")
         super().__init__(self.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         cmd = self.get_command(command, *args)
         # `oc exec` does not support specifying the user to run as.
         # See https://github.com/kubernetes/kubernetes/issues/30656
         oscmd = "oc "
         oscmd_args = []
         if self.kubeconfig is not None:
             oscmd += '--kubeconfig="%s" '
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/paramiko.py` & `pytest-testinfra-9.0.0/testinfra/backend/paramiko.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,47 +18,58 @@
     raise RuntimeError(
         (
             "You must install paramiko package (pip install paramiko) "
             "to use the paramiko backend"
         )
     )
 
+import functools
+from typing import Any, Optional
+
+import paramiko.pkey
 import paramiko.ssh_exception
 
 from testinfra.backend import base
-from testinfra.utils import cached_property
 
 
 class IgnorePolicy(paramiko.MissingHostKeyPolicy):
     """Policy for ignoring missing host key."""
 
-    def missing_host_key(self, client, hostname, key):
+    def missing_host_key(
+        self, client: paramiko.SSHClient, hostname: str, key: paramiko.pkey.PKey
+    ) -> None:
         pass
 
 
 class ParamikoBackend(base.BaseBackend):
     NAME = "paramiko"
 
     def __init__(
         self,
-        hostspec,
-        ssh_config=None,
-        ssh_identity_file=None,
-        timeout=10,
-        *args,
-        **kwargs,
+        hostspec: str,
+        ssh_config: Optional[str] = None,
+        ssh_identity_file: Optional[str] = None,
+        timeout: int = 10,
+        *args: Any,
+        **kwargs: Any,
     ):
         self.host = self.parse_hostspec(hostspec)
         self.ssh_config = ssh_config
         self.ssh_identity_file = ssh_identity_file
         self.get_pty = False
         self.timeout = int(timeout)
         super().__init__(self.host.name, *args, **kwargs)
 
-    def _load_ssh_config(self, client, cfg, ssh_config, ssh_config_dir="~/.ssh"):
+    def _load_ssh_config(
+        self,
+        client: paramiko.SSHClient,
+        cfg: dict[str, Any],
+        ssh_config: paramiko.SSHConfig,
+        ssh_config_dir: str = "~/.ssh",
+    ) -> None:
         for key, value in ssh_config.lookup(self.host.name).items():
             if key == "hostname":
                 cfg[key] = value
             elif key == "user":
                 cfg["username"] = value
             elif key == "port":
                 cfg[key] = int(value)
@@ -79,16 +90,16 @@
                     os.path.expanduser(ssh_config_dir), value
                 )
                 with open(new_config_path) as f:
                     new_ssh_config = paramiko.SSHConfig()
                     new_ssh_config.parse(f)
                     self._load_ssh_config(client, cfg, new_ssh_config, ssh_config_dir)
 
-    @cached_property
-    def client(self):
+    @functools.cached_property
+    def client(self) -> paramiko.SSHClient:
         client = paramiko.SSHClient()
         client.set_missing_host_key_policy(paramiko.WarningPolicy())
         cfg = {
             "hostname": self.host.name,
             "port": int(self.host.port) if self.host.port else 22,
             "username": self.host.user,
             "timeout": self.timeout,
@@ -113,34 +124,38 @@
             except IOError:
                 pass
             else:
                 self._load_ssh_config(client, cfg, ssh_config, ssh_config_dir)
 
         if self.ssh_identity_file:
             cfg["key_filename"] = self.ssh_identity_file
-        client.connect(**cfg)
+        client.connect(**cfg)  # type: ignore[arg-type]
         return client
 
-    def _exec_command(self, command):
-        chan = self.client.get_transport().open_session()
+    def _exec_command(self, command: bytes) -> tuple[int, bytes, bytes]:
+        transport = self.client.get_transport()
+        assert transport is not None
+        chan = transport.open_session()
         if self.get_pty:
             chan.get_pty()
         chan.exec_command(command)
         rc = chan.recv_exit_status()
         stdout = b"".join(chan.makefile("rb"))
         stderr = b"".join(chan.makefile_stderr("rb"))
         return rc, stdout, stderr
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         command = self.get_command(command, *args)
-        command = self.encode(command)
+        cmd = self.encode(command)
         try:
-            rc, stdout, stderr = self._exec_command(command)
-        except paramiko.ssh_exception.SSHException:
-            if not self.client.get_transport().is_active():
+            rc, stdout, stderr = self._exec_command(cmd)
+        except (paramiko.ssh_exception.SSHException, ConnectionResetError):
+            transport = self.client.get_transport()
+            assert transport is not None
+            if not transport.is_active():
                 # try to reinit connection (once)
                 del self.client
-                rc, stdout, stderr = self._exec_command(command)
+                rc, stdout, stderr = self._exec_command(cmd)
             else:
                 raise
 
-        return self.result(rc, command, stdout, stderr)
+        return self.result(rc, cmd, stdout, stderr)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/podman.py` & `pytest-testinfra-9.0.0/testinfra/backend/podman.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from testinfra.backend import base
 
 
 class PodmanBackend(base.BaseBackend):
     NAME = "podman"
 
-    def __init__(self, name, *args, **kwargs):
+    def __init__(self, name: str, *args: Any, **kwargs: Any):
         self.name, self.user = self.parse_containerspec(name)
         super().__init__(self.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         cmd = self.get_command(command, *args)
         if self.user is not None:
             out = self.run_local(
                 "podman exec -u %s %s /bin/sh -c %s", self.user, self.name, cmd
             )
         else:
             out = self.run_local("podman exec %s /bin/sh -c %s", self.name, cmd)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/salt.py` & `pytest-testinfra-9.0.0/testinfra/backend/salt.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,55 +11,57 @@
 # limitations under the License.
 
 try:
     import salt.client
 except ImportError:
     raise RuntimeError("You must install salt package to use the salt backend")
 
+from typing import Any, Optional
+
 from testinfra.backend import base
 
 
 class SaltBackend(base.BaseBackend):
     HAS_RUN_SALT = True
     NAME = "salt"
 
-    def __init__(self, host, *args, **kwargs):
+    def __init__(self, host: str, *args: Any, **kwargs: Any):
         self.host = host
-        self._client = None
+        self._client: Optional[salt.client.LocalClient] = None
         super().__init__(self.host, *args, **kwargs)
 
     @property
-    def client(self):
+    def client(self) -> salt.client.LocalClient:
         if self._client is None:
             self._client = salt.client.LocalClient()
         return self._client
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         command = self.get_command(command, *args)
         out = self.run_salt("cmd.run_all", [command])
         return self.result(
             out["retcode"],
             command,
             out["stdout"].encode("utf8"),
             out["stderr"].encode("utf8"),
             stdout=out["stdout"],
             stderr=out["stderr"],
         )
 
-    def run_salt(self, func, args=None):
+    def run_salt(self, func: str, args: Any = None) -> Any:
         out = self.client.cmd(self.host, func, args or [])
         if self.host not in out:
             raise RuntimeError(
                 "Error while running {}({}): {}. "
                 "Minion not connected ?".format(func, args, out)
             )
         return out[self.host]
 
     @classmethod
-    def get_hosts(cls, host, **kwargs):
+    def get_hosts(cls, host: str, **kwargs: Any) -> list[str]:
         if host is None:
             host = "*"
         if any(c in host for c in "@*[?"):
             client = salt.client.LocalClient()
             if "@" in host:
                 hosts = client.cmd(host, "test.true", tgt_type="compound").keys()
             else:
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/ssh.py` & `pytest-testinfra-9.0.0/testinfra/backend/ssh.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,46 +7,49 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import base64
+from typing import Any, Optional
 
 from testinfra.backend import base
 
 
 class SshBackend(base.BaseBackend):
     """Run command through ssh command"""
 
     NAME = "ssh"
 
     def __init__(
         self,
-        hostspec,
-        ssh_config=None,
-        ssh_identity_file=None,
-        timeout=10,
-        controlpersist=60,
-        ssh_extra_args=None,
-        *args,
-        **kwargs,
+        hostspec: str,
+        ssh_config: Optional[str] = None,
+        ssh_identity_file: Optional[str] = None,
+        timeout: int = 10,
+        controlpath: str = "",
+        controlpersist: int = 60,
+        ssh_extra_args: Optional[str] = None,
+        *args: Any,
+        **kwargs: Any,
     ):
         self.host = self.parse_hostspec(hostspec)
         self.ssh_config = ssh_config
         self.ssh_identity_file = ssh_identity_file
         self.timeout = int(timeout)
+        self.controlpath = controlpath
         self.controlpersist = int(controlpersist)
         self.ssh_extra_args = ssh_extra_args
         super().__init__(self.host.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         return self.run_ssh(self.get_command(command, *args))
 
-    def _build_ssh_command(self, command):
+    def _build_ssh_command(self, command: str) -> tuple[list[str], list[str]]:
         if not self.host.password:
             cmd = ["ssh"]
             cmd_args = []
         else:
             cmd = ["sshpass", "-p", "%s", "ssh"]
             cmd_args = [self.host.password]
 
@@ -70,19 +73,25 @@
             "controlmaster" not in (self.ssh_extra_args or "").lower()
         ):
             cmd.append(
                 "-o ControlMaster=auto -o ControlPersist={}s".format(
                     self.controlpersist
                 )
             )
+        if (
+            "ControlMaster" in " ".join(cmd)
+            and self.controlpath
+            and ("controlpath" not in (self.ssh_extra_args or "").lower())
+        ):
+            cmd.append("-o ControlPath={}".format(self.controlpath))
         cmd.append("%s %s")
         cmd_args.extend([self.host.name, command])
         return cmd, cmd_args
 
-    def run_ssh(self, command):
+    def run_ssh(self, command: str) -> base.CommandResult:
         cmd, cmd_args = self._build_ssh_command(command)
         out = self.run_local(" ".join(cmd), *cmd_args)
         out.command = self.encode(command)
         if out.rc == 255:
             # ssh exits with the exit status of the remote command or with 255
             # if an error occurred.
             raise RuntimeError(out)
@@ -102,26 +111,28 @@
 
     where STDOUT/STDERR are base64 encoded, then we parse that magic string to
     get sanes variables
     """
 
     NAME = "safe-ssh"
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         orig_command = self.get_command(command, *args)
         orig_command = self.get_command("sh -c %s", orig_command)
 
         out = self.run_ssh(
             (
                 """of=$(mktemp)&&ef=$(mktemp)&&{} >$of 2>$ef; r=$?;"""
                 """echo "TESTINFRA_START;$r;$(base64 < $of);$(base64 < $ef);"""
                 """TESTINFRA_END";rm -f $of $ef"""
             ).format(orig_command)
         )
 
         start = out.stdout.find("TESTINFRA_START;") + len("TESTINFRA_START;")
         end = out.stdout.find("TESTINFRA_END") - 1
         rc, stdout, stderr = out.stdout[start:end].split(";")
-        rc = int(rc)
-        stdout = base64.b64decode(stdout)
-        stderr = base64.b64decode(stderr)
-        return self.result(rc, self.encode(orig_command), stdout, stderr)
+        return self.result(
+            int(rc),
+            self.encode(orig_command),
+            base64.b64decode(stdout),
+            base64.b64decode(stderr),
+        )
```

### Comparing `pytest-testinfra-8.1.0/testinfra/backend/winrm.py` & `pytest-testinfra-9.0.0/testinfra/backend/winrm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
+from typing import Any, Optional
 
 from testinfra.backend import base
 
 try:
     import winrm
 except ImportError:
     raise RuntimeError(
@@ -27,15 +28,15 @@
 import winrm.protocol
 
 _find_unsafe = re.compile(r"[^\w@%+=:,./-]", re.ASCII)
 
 
 # (gtmanfred) This is copied from pipes.quote, but changed to use double quotes
 # instead of single quotes.  This is used by the winrm backend.
-def _quote(s):
+def _quote(s: str) -> str:
     """Return a shell-escaped version of the string *s*."""
     if not s:
         return "''"
     if _find_unsafe.search(s) is None:
         return s
 
     # use single quotes, and put single quotes into double quotes
@@ -46,24 +47,24 @@
 class WinRMBackend(base.BaseBackend):
     """Run command through winrm command"""
 
     NAME = "winrm"
 
     def __init__(
         self,
-        hostspec,
-        no_ssl=False,
-        no_verify_ssl=False,
-        read_timeout_sec=None,
-        operation_timeout_sec=None,
-        *args,
-        **kwargs,
+        hostspec: str,
+        no_ssl: bool = False,
+        no_verify_ssl: bool = False,
+        read_timeout_sec: Optional[int] = None,
+        operation_timeout_sec: Optional[int] = None,
+        *args: Any,
+        **kwargs: Any,
     ):
         self.host = self.parse_hostspec(hostspec)
-        self.conn_args = {
+        self.conn_args: dict[str, Any] = {
             "endpoint": "{}://{}{}/wsman".format(
                 "http" if no_ssl else "https",
                 self.host.name,
                 ":{}".format(self.host.port) if self.host.port else "",
             ),
             "transport": "ntlm",
             "username": self.host.user,
@@ -73,24 +74,24 @@
             self.conn_args["server_cert_validation"] = "ignore"
         if read_timeout_sec is not None:
             self.conn_args["read_timeout_sec"] = read_timeout_sec
         if operation_timeout_sec is not None:
             self.conn_args["operation_timeout_sec"] = operation_timeout_sec
         super().__init__(self.host.name, *args, **kwargs)
 
-    def run(self, command, *args, **kwargs):
+    def run(self, command: str, *args: str, **kwargs: Any) -> base.CommandResult:
         return self.run_winrm(self.get_command(command, *args))
 
-    def run_winrm(self, command, *args):
+    def run_winrm(self, command: str, *args: str) -> base.CommandResult:
         p = winrm.protocol.Protocol(**self.conn_args)
         shell_id = p.open_shell()
         command_id = p.run_command(shell_id, command, *args)
         stdout, stderr, rc = p.get_command_output(shell_id, command_id)
         p.cleanup_command(shell_id, command_id)
         p.close_shell(shell_id)
         return self.result(rc, command, stdout, stderr)
 
     @staticmethod
-    def quote(command, *args):
+    def quote(command: str, *args: str) -> str:
         if args:
             return command % tuple(_quote(a) for a in args)  # noqa: S001
         return command
```

### Comparing `pytest-testinfra-8.1.0/testinfra/host.py` & `pytest-testinfra-9.0.0/testinfra/host.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,46 +6,54 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
 import os
+from collections.abc import Iterable
+from typing import Any
 
 import testinfra.backend
+import testinfra.backend.base
 import testinfra.modules
-from testinfra.utils import cached_property
+import testinfra.modules.base
 
 
 class Host:
-    _host_cache = {}  # type: ignore[var-annotated]
-    _hosts_cache = {}  # type: ignore[var-annotated]
+    _host_cache: dict[tuple[str, frozenset[tuple[str, Any]]], "Host"] = {}
+    _hosts_cache: dict[
+        tuple[frozenset[str], frozenset[tuple[str, Any]]], list["Host"]
+    ] = {}
 
-    def __init__(self, backend):
+    def __init__(self, backend: testinfra.backend.base.BaseBackend):
         self.backend = backend
         super().__init__()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<testinfra.host.Host {}>".format(self.backend.get_pytest_id())
 
-    @cached_property
-    def has_command_v(self):
+    @functools.cached_property
+    def has_command_v(self) -> bool:
         """Return True if `command -v` is available"""
         return self.run("command -v command").rc == 0
 
-    def exists(self, command):
+    def exists(self, command: str) -> bool:
         """Return True if given command exist in $PATH"""
         if self.has_command_v:
             out = self.run("command -v %s", command)
         else:
             out = self.run_expect([0, 1], "which %s", command)
         return out.rc == 0
 
-    def find_command(self, command, extrapaths=("/sbin", "/usr/sbin")):
+    def find_command(
+        self, command: str, extrapaths: Iterable[str] = ("/sbin", "/usr/sbin")
+    ) -> str:
         """Return path of given command
 
         raise ValueError if command cannot be found
         """
         if self.has_command_v:
             out = self.run("command -v %s", command)
         else:
@@ -54,15 +62,17 @@
             return out.stdout.rstrip("\r\n")
         for basedir in extrapaths:
             path = os.path.join(basedir, command)
             if self.exists(path):
                 return path
         raise ValueError('cannot find "{}" command'.format(command))
 
-    def run(self, command, *args, **kwargs):
+    def run(
+        self, command: str, *args: str, **kwargs: Any
+    ) -> testinfra.backend.base.CommandResult:
         """Run given command and return rc (exit status), stdout and stderr
 
         >>> cmd = host.run("ls -l /etc/passwd")
         >>> cmd.rc
         0
         >>> cmd.stdout
         '-rw-r--r-- 1 root root 1790 Feb 11 00:28 /etc/passwd\\n'
@@ -83,55 +93,59 @@
             rc=2, stdout='',
             stderr=(
               'ls: cannot access /;echo inject: No such file or directory\\n'),
             command="ls -l '/;echo inject'")
         """
         return self.backend.run(command, *args, **kwargs)
 
-    def run_expect(self, expected, command, *args, **kwargs):
+    def run_expect(
+        self, expected: list[int], command: str, *args: str, **kwargs: Any
+    ) -> testinfra.backend.base.CommandResult:
         """Run command and check it return an expected exit status
 
         :param expected: A list of expected exit status
         :raises: AssertionError
         """
         __tracebackhide__ = True
         out = self.run(command, *args, **kwargs)
         assert out.rc in expected, "Unexpected exit code {} for {}".format(out.rc, out)
         return out
 
-    def run_test(self, command, *args, **kwargs):
+    def run_test(
+        self, command: str, *args: str, **kwargs: Any
+    ) -> testinfra.backend.base.CommandResult:
         """Run command and check it return an exit status of 0 or 1
 
         :raises: AssertionError
         """
         return self.run_expect([0, 1], command, *args, **kwargs)
 
-    def check_output(self, command, *args, **kwargs):
+    def check_output(self, command: str, *args: str, **kwargs: Any) -> str:
         """Get stdout of a command which has run successfully
 
         :returns: stdout without trailing newline
         :raises: AssertionError
         """
         __tracebackhide__ = True
         out = self.run(command, *args, **kwargs)
         assert out.rc == 0, "Unexpected exit code {} for {}".format(out.rc, out)
         return out.stdout.rstrip("\r\n")
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> type[testinfra.modules.base.Module]:
         if name in testinfra.modules.modules:
             module_class = testinfra.modules.get_module_class(name)
             obj = module_class.get_module(self)
             setattr(self, name, obj)
             return obj
         raise AttributeError(
             "'{}' object has no attribute '{}'".format(self.__class__.__name__, name)
         )
 
     @classmethod
-    def get_host(cls, hostspec, **kwargs):
+    def get_host(cls, hostspec: str, **kwargs: Any) -> "Host":
         """Return a Host instance from `hostspec`
 
         `hostspec` should be like
         `<backend_type>://<name>?param1=value1&param2=value2`
 
         Params can also be passed in `**kwargs` (eg. get_host("local://",
         sudo=True) is equivalent to get_host("local://?sudo=true"))
@@ -147,15 +161,15 @@
         if key not in cache:
             backend = testinfra.backend.get_backend(hostspec, **kwargs)
             cache[key] = host = cls(backend)
             backend.set_host(host)
         return cache[key]
 
     @classmethod
-    def get_hosts(cls, hosts, **kwargs):
+    def get_hosts(cls, hosts: Iterable[str], **kwargs: Any) -> list["Host"]:
         key = (frozenset(hosts), frozenset(kwargs.items()))
         cache = cls._hosts_cache
         if key not in cache:
             cache[key] = []
             for backend in testinfra.backend.get_backends(hosts, **kwargs):
                 host = cls(backend)
                 backend.set_host(host)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/main.py` & `pytest-testinfra-9.0.0/testinfra/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 # limitations under the License.
 
 import warnings
 
 import pytest
 
 
-def main():
+def main() -> int:
     warnings.warn("calling testinfra is deprecated, call py.test instead", stacklevel=1)
     return pytest.main()
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/__init__.py` & `pytest-testinfra-9.0.0/testinfra/modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import importlib
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    import testinfra.modules.base
 
 modules = {
     "addr": "addr:Addr",
     "ansible": "ansible:Ansible",
     "command": "command:Command",
     "docker": "docker:Docker",
     "podman": "podman:Podman",
@@ -22,15 +26,14 @@
     "file": "file:File",
     "group": "group:Group",
     "interface": "interface:Interface",
     "iptables": "iptables:Iptables",
     "mount_point": "mountpoint:MountPoint",
     "package": "package:Package",
     "pip": "pip:Pip",
-    "pip_package": "pip:PipPackage",
     "process": "process:Process",
     "puppet_resource": "puppet:PuppetResource",
     "facter": "puppet:Facter",
     "salt": "salt:Salt",
     "service": "service:Service",
     "socket": "socket:Socket",
     "sudo": "sudo:Sudo",
@@ -38,12 +41,12 @@
     "sysctl": "sysctl:Sysctl",
     "system_info": "systeminfo:SystemInfo",
     "user": "user:User",
     "block_device": "blockdevice:BlockDevice",
 }
 
 
-def get_module_class(name):
+def get_module_class(name: str) -> type["testinfra.modules.base.Module"]:
     modname, classname = modules[name].split(":")
     modname = ".".join([__name__, modname])
     module = importlib.import_module(modname)
-    return getattr(module, classname)
+    return getattr(module, classname)  # type: ignore[no-any-return]
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/addr.py` & `pytest-testinfra-9.0.0/testinfra/modules/addr.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/ansible.py` & `pytest-testinfra-9.0.0/testinfra/modules/ansible.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/base.py` & `pytest-testinfra-9.0.0/testinfra/modules/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import typing
+from typing import TYPE_CHECKING
 
 
 class Module:
-    if typing.TYPE_CHECKING:
+    if TYPE_CHECKING:
         import testinfra.host
 
         _host: testinfra.host.Host
 
     @classmethod
-    def get_module(cls, _host):
+    def get_module(cls, _host: "testinfra.host.Host") -> type["Module"]:
         klass = cls.get_module_class(_host)
         return type(
             klass.__name__,
             (klass,),
             {"_host": _host},
         )
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/blockdevice.py` & `pytest-testinfra-9.0.0/testinfra/modules/blockdevice.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
+
 from testinfra.modules.base import Module
-from testinfra.utils import cached_property
 
 
 class BlockDevice(Module):
     """Information for block device.
 
     Should be used with sudo or under root.
 
@@ -120,15 +121,15 @@
         raise NotImplementedError
 
     def __repr__(self):
         return "<BlockDevice(path={})>".format(self.device)
 
 
 class LinuxBlockDevice(BlockDevice):
-    @cached_property
+    @functools.cached_property
     def _data(self):
         header = ["RO", "RA", "SSZ", "BSZ", "StartSec", "Size", "Device"]
         command = "blockdev  --report %s"
         blockdev = self.run(command, self.device)
         if blockdev.rc != 0 or blockdev.stderr:
             raise RuntimeError("Failed to gather data: {}".format(blockdev.stderr))
         output = blockdev.stdout.splitlines()
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/command.py` & `pytest-testinfra-9.0.0/testinfra/modules/command.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/docker.py` & `pytest-testinfra-9.0.0/testinfra/modules/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/environment.py` & `pytest-testinfra-9.0.0/testinfra/modules/environment.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/file.py` & `pytest-testinfra-9.0.0/testinfra/modules/file.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/group.py` & `pytest-testinfra-9.0.0/testinfra/modules/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 
 from testinfra.modules.base import Module
 
 
 class Group(Module):
     """Test unix group"""
 
-    def __init__(self, name=None):
+    def __init__(self, name):
         self.name = name
         super().__init__()
 
     @property
     def exists(self):
         """Test if group exists
 
         >>> host.group("wheel").exists
         True
         >>> host.group("nosuchgroup").exists
         False
-
         """
-
         return self.run_expect([0, 2], "getent group %s", self.name).rc == 0
 
     @property
     def gid(self):
         return int(self.check_output("getent group %s | cut -d':' -f3", self.name))
 
     @property
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/interface.py` & `pytest-testinfra-9.0.0/testinfra/modules/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
 import json
 import re
 
 from testinfra.modules.base import Module
-from testinfra.utils import cached_property
 
 
 class Interface(Module):
     """Test network interfaces
 
     >>> host.interface("eth0").exists
     True
@@ -103,15 +103,15 @@
         >>> host.interface.default("inet6")
         None
         """
         raise NotImplementedError
 
 
 class LinuxInterface(Interface):
-    @cached_property
+    @functools.cached_property
     def _ip(self):
         ip_cmd = self.find_command("ip")
         if self.family is not None:
             ip_cmd = f"{ip_cmd} -f {self.family}"
         return ip_cmd
 
     @property
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/iptables.py` & `pytest-testinfra-9.0.0/testinfra/modules/iptables.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/mountpoint.py` & `pytest-testinfra-9.0.0/testinfra/modules/mountpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return self._attrs["options"]
 
     @classmethod
     def get_mountpoints(cls):
         """Returns a list of MountPoint instances
 
         >>> host.mount_point.get_mountpoints()
-        [<MountPoint(path=/proc, device=proc, filesystem=proc, options=rw,nosuid,nodev,noexec,relatime)>
+        [<MountPoint(path=/proc, device=proc, filesystem=proc, options=rw,nosuid,nodev,noexec,relatime)>,
          <MountPoint(path=/, device=/dev/sda1, filesystem=ext4, options=rw,relatime,errors=remount-ro,data=ordered)>]
         """  # noqa
         mountpoints = []
         for mountpoint in cls._iter_mountpoints():
             mountpoints.append(cls(mountpoint["path"], mountpoint))
         return mountpoints
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/package.py` & `pytest-testinfra-9.0.0/testinfra/modules/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,16 @@
         if host.system_info.distribution and (
             host.system_info.distribution.lower()
             in (
                 "almalinux",
                 "centos",
                 "cloudlinux",
                 "fedora",
+                "opensuse-leap",
+                "opensuse-tumbleweed",
                 "rocky",
             )
         ):
             return RpmPackage
         if host.system_info.distribution in ("arch", "manjarolinux"):
             return ArchPackage
         if host.exists("apk"):
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/pip.py` & `pytest-testinfra-9.0.0/testinfra/modules/pip.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import re
-import warnings
 
 from testinfra.modules.base import Module
 
 
 def _re_match(line, regexp):
     match = regexp.match(line)
     if match is None:
@@ -54,15 +53,15 @@
             self.name,
         )
 
     @classmethod
     def check(cls, pip_path="pip"):
         """Verify installed packages have compatible dependencies.
 
-        >>> cmd = host.pip_package.check()
+        >>> cmd = host.pip.check()
         >>> cmd.rc
         0
         >>> cmd.stdout
         No broken requirements found.
 
         Can only be used if `pip check`_ command is available,
         for pip versions >= 9.0.0_.
@@ -72,15 +71,15 @@
         """
         return cls.run_expect([0, 1], "%s check", pip_path)
 
     @classmethod
     def get_packages(cls, pip_path="pip"):
         """Get all installed packages and versions returned by `pip list`:
 
-        >>> host.pip_package.get_packages(pip_path='~/venv/website/bin/pip')
+        >>> host.pip.get_packages(pip_path='~/venv/website/bin/pip')
         {'Django': {'version': '1.10.2'},
          'mywebsite': {'version': '1.0a3', 'path': '/srv/website'},
          'psycopg2': {'version': '2.6.2'}}
         """
         out = cls.run_expect([0, 2], "%s list --no-index --format=json", pip_path)
         pkgs = {}
         if out.rc == 0:
@@ -102,15 +101,15 @@
                     pkgs[name] = {"version": version}
         return pkgs
 
     @classmethod
     def get_outdated_packages(cls, pip_path="pip"):
         """Get all outdated packages with current and latest version
 
-        >>> host.pip_package.get_outdated_packages(
+        >>> host.pip.get_outdated_packages(
         ...     pip_path='~/venv/website/bin/pip')
         {'Django': {'current': '1.10.2', 'latest': '1.10.3'}}
         """
         out = cls.run_expect([0, 2], "%s list -o --format=json", pip_path)
         pkgs = {}
         if out.rc == 0:
             for pkg in json.loads(out.stdout):
@@ -130,38 +129,7 @@
                 if line.startswith("Warning: "):
                     # Warning: cannot find svn location for ...
                     continue
                 output_re = regexpes[1] if "Current:" in line else regexpes[0]
                 name, current, latest = _re_match(line, output_re)
                 pkgs[name] = {"current": current, "latest": latest}
         return pkgs
-
-
-class PipPackage(Pip):
-    """.. deprecated:: 6.2
-
-    Use :class:`~testinfra.modules.pip.Pip` instead.
-    """
-
-    @staticmethod
-    def _deprecated():
-        """Raise a `DeprecationWarning`"""
-        warnings.warn(
-            "Calling host.pip_package is deprecated, call host.pip instead",
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-
-    @classmethod
-    def check(cls, pip_path="pip"):
-        PipPackage._deprecated()
-        return super().check(pip_path=pip_path)
-
-    @classmethod
-    def get_packages(cls, pip_path="pip"):
-        PipPackage._deprecated()
-        return super().get_packages(pip_path=pip_path)
-
-    @classmethod
-    def get_outdated_packages(cls, pip_path="pip"):
-        PipPackage._deprecated()
-        return super().get_outdated_packages(pip_path=pip_path)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/podman.py` & `pytest-testinfra-9.0.0/testinfra/modules/podman.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/process.py` & `pytest-testinfra-9.0.0/testinfra/modules/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from testinfra.modules.base import InstanceModule
 
 
 def int_or_float(value):
     try:
         return int(value)
     except ValueError:
         try:
             return float(value)
         except ValueError:
             return value
 
 
-class _Process(dict):
+class _Process(dict[str, Any]):
     def __getattr__(self, key):
         try:
             return self.__getitem__(key)
         except KeyError:
             attrs = self["_get_process_attribute_by_pid"](self["pid"], key)
             if attrs["lstart"] != self["lstart"]:
                 raise RuntimeError(
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/puppet.py` & `pytest-testinfra-9.0.0/testinfra/modules/puppet.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/salt.py` & `pytest-testinfra-9.0.0/testinfra/modules/salt.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/service.py` & `pytest-testinfra-9.0.0/testinfra/modules/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
+
 from testinfra.modules.base import Module
-from testinfra.utils import cached_property
 
 
 class Service(Module):
     """Test services
 
     Implementations:
 
@@ -56,15 +57,15 @@
         """Test if service is masked
 
         This method is only available in the systemd implementation,
         it will raise ``NotImplementedError`` in others implementations
         """
         raise NotImplementedError
 
-    @cached_property
+    @functools.cached_property
     def systemd_properties(self):
         """Properties of the service (unit).
 
         Return service properties as a `dict`,
         empty properties are not returned.
 
         >>> ntp = host.service("ntp")
@@ -108,15 +109,15 @@
         raise NotImplementedError
 
     def __repr__(self):
         return "<service {}>".format(self.name)
 
 
 class SysvService(Service):
-    @cached_property
+    @functools.cached_property
     def _service_command(self):
         return self.find_command("service")
 
     @property
     def is_running(self):
         # based on /lib/lsb/init-functions
         # 0: program running
@@ -177,15 +178,15 @@
         return True
 
     @property
     def is_masked(self):
         cmd = self.run_test("systemctl is-enabled %s", self.name)
         return cmd.stdout.strip() == "masked"
 
-    @cached_property
+    @functools.cached_property
     def systemd_properties(self):
         out = self.check_output("systemctl show %s", self.name)
         out_d = {}
         if out:
             # maxsplit is required because values can contain `=`
             out_d = dict(
                 map(lambda pair: pair.split("=", maxsplit=1), out.splitlines())
@@ -217,15 +218,15 @@
         cmd = self.run_test("status %s", self.name)
         if cmd.rc == 0 and len(cmd.stdout.split()) > 1:
             return "running" in cmd.stdout.split()[1]
         return super().is_running
 
 
 class OpenRCService(SysvService):
-    @cached_property
+    @functools.cached_property
     def _service_command(self):
         return self.find_command("rc-service")
 
     @property
     def is_enabled(self):
         return bool(
             self.check_output(
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/socket.py` & `pytest-testinfra-9.0.0/testinfra/modules/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
 import socket
 from typing import List, Optional, Tuple
 
 from testinfra.modules.base import Module
-from testinfra.utils import cached_property
 
 
 def parse_socketspec(socketspec):
-
     protocol, address = socketspec.split("://", 1)
 
     if protocol not in ("udp", "tcp", "unix"):
         raise RuntimeError(
             "Cannot validate protocol '{}'. Should be tcp, udp or unix".format(protocol)
         )
 
@@ -310,15 +309,15 @@
                     remote_port = int(remote_port)
                     yield protocol, host, port, remote_host, remote_port
             elif protocol == "unix":
                 yield protocol, splitted[-1]
 
 
 class BSDSocket(Socket):
-    @cached_property
+    @functools.cached_property
     def _command(self):
         return self.find_command("netstat")
 
     def _iter_sockets(self, listening):
         cmd = "%s -n"
 
         if listening:
@@ -329,15 +328,14 @@
 
         for line in self.check_output(cmd, self._command).splitlines():
             line = line.replace("\t", " ")
             splitted = line.split()
             # FreeBSD: tcp4/tcp6
             # OpeNBSD/NetBSD: tcp/tcp6
             if splitted[0] in ("tcp", "udp", "udp4", "tcp4", "tcp6", "udp6"):
-
                 address = splitted[3]
                 if address == "*.*":
                     # On OpenBSD 6.3 (issue #338)
                     # udp          0      0  *.*                    *.*
                     # udp6         0      0  *.*                    *.*
                     continue
                 host, port = address.rsplit(".", 1)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/sudo.py` & `pytest-testinfra-9.0.0/testinfra/modules/sudo.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/supervisor.py` & `pytest-testinfra-9.0.0/testinfra/modules/supervisor.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/sysctl.py` & `pytest-testinfra-9.0.0/testinfra/modules/sysctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
+
 from testinfra.modules.base import InstanceModule
-from testinfra.utils import cached_property
 
 
 class Sysctl(InstanceModule):
     """Test kernel parameters
 
     >>> host.sysctl("kernel.osrelease")
     "3.16.0-4-amd64"
     >>> host.sysctl("vm.dirty_ratio")
     20
     """
 
-    @cached_property
+    @functools.cached_property
     def _sysctl_command(self):
         return self.find_command("sysctl")
 
     def __call__(self, name):
         value = self.check_output("%s -n %s", self._sysctl_command, name)
         try:
             return int(value)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/systeminfo.py` & `pytest-testinfra-9.0.0/testinfra/modules/systeminfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import functools
 import re
 
 from testinfra.modules.base import InstanceModule
-from testinfra.utils import cached_property
 
 
 class SystemInfo(InstanceModule):
     """Return system information"""
 
-    @cached_property
+    @functools.cached_property
     def sysinfo(self):
         sysinfo = {
             "type": None,
             "distribution": None,
             "codename": None,
             "release": None,
             "arch": None,
@@ -46,29 +46,14 @@
 
         sysinfo["arch"] = self.check_output("uname -m")
         return sysinfo
 
     def _get_linux_sysinfo(self):
         sysinfo = {}
 
-        # LSB
-        lsb = self.run("lsb_release -a")
-        if lsb.rc == 0:
-            for line in lsb.stdout.splitlines():
-                key, value = line.split(":", 1)
-                key = key.strip().lower()
-                value = value.strip().lower()
-                if key == "distributor id":
-                    sysinfo["distribution"] = value
-                elif key == "release":
-                    sysinfo["release"] = value
-                elif key == "codename":
-                    sysinfo["codename"] = value
-            return sysinfo
-
         # https://www.freedesktop.org/software/systemd/man/os-release.html
         os_release = self.run("cat /etc/os-release")
         if os_release.rc == 0:
             for line in os_release.stdout.splitlines():
                 for key, attname in (
                     ("ID=", "distribution"),
                     ("VERSION_ID=", "release"),
@@ -96,14 +81,29 @@
         # Alpine doesn't have /etc/os-release
         alpine_release = self.run("cat /etc/alpine-release")
         if alpine_release.rc == 0:
             sysinfo["distribution"] = "alpine"
             sysinfo["release"] = alpine_release.stdout.strip()
             return sysinfo
 
+        # LSB
+        lsb = self.run("lsb_release -a")
+        if lsb.rc == 0:
+            for line in lsb.stdout.splitlines():
+                key, value = line.split(":", 1)
+                key = key.strip().lower()
+                value = value.strip().lower()
+                if key == "distributor id":
+                    sysinfo["distribution"] = value
+                elif key == "release":
+                    sysinfo["release"] = value
+                elif key == "codename":
+                    sysinfo["codename"] = value
+            return sysinfo
+
         return sysinfo
 
     def _get_darwin_sysinfo(self):
         sysinfo = {}
 
         sw_vers = self.run("sw_vers")
         if sw_vers.rc == 0:
```

### Comparing `pytest-testinfra-8.1.0/testinfra/modules/user.py` & `pytest-testinfra-9.0.0/testinfra/modules/user.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.1.0/testinfra/plugin.py` & `pytest-testinfra-9.0.0/testinfra/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # limitations under the License.
 
 import logging
 import shutil
 import sys
 import tempfile
 import time
+from typing import AnyStr
 
 import pytest
 
 import testinfra
 import testinfra.host
 import testinfra.modules
 
@@ -169,15 +170,15 @@
             )
         )
         self.out.seek(0)
         shutil.copyfileobj(self.out, out)
         return ret
 
 
-class SpooledTemporaryFile(tempfile.SpooledTemporaryFile):
+class SpooledTemporaryFile(tempfile.SpooledTemporaryFile[AnyStr]):
     def __init__(self, *args, **kwargs):
         if "b" in kwargs.get("mode", "b"):
             self._out_encoding = kwargs.pop("encoding")
         else:
             self._out_encoding = kwargs.get("encoding")
         super().__init__(*args, **kwargs)
```

### Comparing `pytest-testinfra-8.1.0/testinfra/utils/ansible_runner.py` & `pytest-testinfra-9.0.0/testinfra/utils/ansible_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import configparser
 import fnmatch
+import functools
 import ipaddress
 import json
 import os
 import tempfile
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Iterator, Optional, Union
 
 import testinfra
-from testinfra.utils import cached_property
+import testinfra.host
 
 __all__ = ["AnsibleRunner"]
 
 local = testinfra.get_host("local://")
 
 
-def get_ansible_config():
+def get_ansible_config() -> configparser.ConfigParser:
     fname = os.environ.get("ANSIBLE_CONFIG")
     if not fname:
         for possible in (
             "ansible.cfg",
             os.path.join(os.path.expanduser("~"), ".ansible.cfg"),
             os.path.join("/", "etc", "ansible", "ansible.cfg"),
         ):
@@ -40,26 +41,37 @@
     config = configparser.ConfigParser()
     if not fname:
         return config
     config.read(fname)
     return config
 
 
-def get_ansible_inventory(config, inventory_file):
+Inventory = dict[str, Any]
+
+
+def get_ansible_inventory(
+    config: configparser.ConfigParser, inventory_file: Optional[str]
+) -> Inventory:
     # Disable ansible verbosity to avoid
     # https://github.com/ansible/ansible/issues/59973
     cmd = "ANSIBLE_VERBOSITY=0 ansible-inventory --list"
     args = []
     if inventory_file:
         cmd += " -i %s"
         args += [inventory_file]
-    return json.loads(local.check_output(cmd, *args))
+    return json.loads(local.check_output(cmd, *args))  # type: ignore[no-any-return]
 
 
-def get_ansible_host(config, inventory, host, ssh_config=None, ssh_identity_file=None):
+def get_ansible_host(
+    config: configparser.ConfigParser,
+    inventory: Inventory,
+    host: str,
+    ssh_config: Optional[str] = None,
+    ssh_identity_file: Optional[str] = None,
+) -> Optional[testinfra.host.Host]:
     if is_empty_inventory(inventory):
         if host == "localhost":
             return testinfra.get_host("local://")
         return None
     hostvars = inventory["_meta"].get("hostvars", {}).get(host, {})
     connection = hostvars.get("ansible_connection", "ssh")
     if connection not in (
@@ -77,15 +89,15 @@
     connection = {
         "community.docker.docker": "docker",
         "lxd": "lxc",
         "paramiko_ssh": "paramiko",
         "smart": "ssh",
     }.get(connection, connection)
 
-    options: Dict[str, Any] = {
+    options: dict[str, Any] = {
         "ansible_become": {
             "ini": {
                 "section": "privilege_escalation",
                 "key": "become",
             },
             "environment": "ANSIBLE_BECOME",
         },
@@ -122,15 +134,17 @@
                 "section": "defaults",
                 "key": "remote_user",
             },
             "environment": "ANSIBLE_REMOTE_USER",
         },
     }
 
-    def get_config(name, default=None):
+    def get_config(
+        name: str, default: Union[None, bool, str] = None
+    ) -> Union[None, bool, str]:
         value = default
         option = options.get(name, {})
 
         ini = option.get("ini")
         if ini:
             value = config.get(ini["section"], ini["key"], fallback=default)
 
@@ -140,19 +154,20 @@
         var = option.get("environment")
         if var and var in os.environ:
             value = os.environ[var]
 
         return value
 
     testinfra_host = get_config("ansible_host", host)
+    assert isinstance(testinfra_host, str), testinfra_host
     user = get_config("ansible_user")
     password = get_config("ansible_ssh_pass")
     port = get_config("ansible_port")
 
-    kwargs: Dict[str, Union[str, bool]] = {}
+    kwargs: dict[str, Union[None, str, bool]] = {}
     if get_config("ansible_become", False):
         kwargs["sudo"] = True
     kwargs["sudo_user"] = get_config("ansible_become_user")
     if ssh_config is not None:
         kwargs["ssh_config"] = ssh_config
     if ssh_identity_file is not None:
         kwargs["ssh_identity_file"] = ssh_identity_file
@@ -161,19 +176,29 @@
     if "ansible_ssh_private_key_file" in hostvars:
         kwargs["ssh_identity_file"] = hostvars["ansible_ssh_private_key_file"]
     elif "ansible_private_key_file" in hostvars:
         kwargs["ssh_identity_file"] = hostvars["ansible_private_key_file"]
     kwargs["ssh_extra_args"] = " ".join(
         [
             config.get("ssh_connection", "ssh_args", fallback=""),
-            get_config("ansible_ssh_common_args", ""),
-            get_config("ansible_ssh_extra_args", ""),
+            get_config("ansible_ssh_common_args", ""),  # type: ignore[list-item]
+            get_config("ansible_ssh_extra_args", ""),  # type: ignore[list-item]
         ]
     ).strip()
 
+    control_path = config.get("ssh_connection", "control_path", fallback="", raw=True)
+    if control_path:
+        directory = config.get(
+            "persistent_connection", "control_path_dir", fallback="~/.ansible/cp"
+        )
+        control_path = control_path % ({"directory": directory})  # noqa: S001
+        # restore original "%%"
+        control_path = control_path.replace("%", "%%")
+        kwargs["controlpath"] = control_path
+
     spec = "{}://".format(connection)
 
     # Fallback to user:password auth when identity file is not used
     if user and password and not kwargs.get("ssh_identity_file"):
         spec += "{}:{}@".format(user, password)
     elif user:
         spec += "{}@".format(user)
@@ -187,28 +212,28 @@
     else:
         spec += testinfra_host
     if port:
         spec += ":{}".format(port)
     return testinfra.get_host(spec, **kwargs)
 
 
-def itergroup(inventory, group):
+def itergroup(inventory: Inventory, group: str) -> Iterator[str]:
     for host in inventory.get(group, {}).get("hosts", []):
         yield host
     for g in inventory.get(group, {}).get("children", []):
         for host in itergroup(inventory, g):
             yield host
 
 
-def is_empty_inventory(inventory):
+def is_empty_inventory(inventory: Inventory) -> bool:
     return not any(True for _ in itergroup(inventory, "all"))
 
 
 class AnsibleRunner:
-    _runners: Dict[Optional[str], "AnsibleRunner"] = {}
+    _runners: dict[Optional[str], "AnsibleRunner"] = {}
     _known_options = {
         # Boolean arguments.
         "become": {
             "cli": "--become",
             "type": "boolean",
         },
         "check": {
@@ -239,20 +264,20 @@
         # Arguments serialized as JSON.
         "extra_vars": {
             "cli": "--extra-vars",
             "type": "json",
         },
     }
 
-    def __init__(self, inventory_file=None):
+    def __init__(self, inventory_file: Optional[str] = None):
         self.inventory_file = inventory_file
-        self._host_cache = {}
+        self._host_cache: dict[str, Optional[testinfra.host.Host]] = {}
         super().__init__()
 
-    def get_hosts(self, pattern="all"):
+    def get_hosts(self, pattern: str = "all") -> list[str]:
         inventory = self.inventory
         result = set()
         if is_empty_inventory(inventory):
             # empty inventory should not return any hosts except for localhost
             if pattern == "localhost":
                 result.add("localhost")
             else:
@@ -266,57 +291,57 @@
                 if groupmatch:
                     result |= set(itergroup(inventory, group))
                 for host in inventory[group].get("hosts", []):
                     if fnmatch.fnmatch(host, pattern):
                         result.add(host)
         return sorted(result)
 
-    @cached_property
-    def inventory(self):
+    @functools.cached_property
+    def inventory(self) -> Inventory:
         return get_ansible_inventory(self.ansible_config, self.inventory_file)
 
-    @cached_property
-    def ansible_config(self):
+    @functools.cached_property
+    def ansible_config(self) -> configparser.ConfigParser:
         return get_ansible_config()
 
-    def get_variables(self, host):
+    def get_variables(self, host: str) -> dict[str, Any]:
         inventory = self.inventory
         # inventory_hostname, group_names and groups are for backward
         # compatibility with testinfra 2.X
-        hostvars = inventory["_meta"].get("hostvars", {}).get(host, {})
+        hostvars: dict[str, Any] = inventory["_meta"].get("hostvars", {}).get(host, {})
         hostvars.setdefault("inventory_hostname", host)
         group_names = []
         groups = {}
         for group in sorted(inventory):
             if group == "_meta":
                 continue
             groups[group] = sorted(itergroup(inventory, group))
             if group != "all" and host in inventory[group].get("hosts", []):
                 group_names.append(group)
         hostvars.setdefault("group_names", group_names)
         hostvars.setdefault("groups", groups)
         return hostvars
 
-    def get_host(self, host, **kwargs):
+    def get_host(self, host: str, **kwargs: Any) -> Optional[testinfra.host.Host]:
         try:
             return self._host_cache[host]
         except KeyError:
             self._host_cache[host] = get_ansible_host(
                 self.ansible_config, self.inventory, host, **kwargs
             )
             return self._host_cache[host]
 
-    def options_to_cli(self, options):
+    def options_to_cli(self, options: dict[str, Any]) -> tuple[str, list[str]]:
         verbose = options.pop("verbose", 0)
 
         args = {"become": False, "check": True}
         args.update(options)
 
-        cli: List[str] = []
-        cli_args: List[str] = []
+        cli: list[str] = []
+        cli_args: list[str] = []
         if verbose:
             cli.append("-" + "v" * verbose)
         for arg_name, value in args.items():
             option = self._known_options[arg_name]
             opt_cli = option["cli"]
             opt_type = option["type"]
             if opt_type == "boolean":
@@ -330,15 +355,22 @@
                 cli.append(opt_cli + " %s")
                 value_json = json.dumps(value)
                 cli_args.append(value_json)
             else:
                 raise TypeError("Unsupported argument type '{}'.".format(opt_type))
         return " ".join(cli), cli_args
 
-    def run_module(self, host, module_name, module_args, get_encoding=None, **options):
+    def run_module(
+        self,
+        host: str,
+        module_name: str,
+        module_args: Optional[str],
+        get_encoding: Optional[Callable[[], str]] = None,
+        **options: Any,
+    ) -> Any:
         cmd, args = "ansible --tree %s", []
         if self.inventory_file:
             cmd += " -i %s"
             args += [self.inventory_file]
         cmd += " -m %s"
         args += [module_name]
         if module_args:
@@ -371,13 +403,13 @@
             except UnicodeDecodeError:
                 if get_encoding is None:
                     raise
                 with open(fpath, "r", encoding=get_encoding()) as f:
                     return json.load(f)
 
     @classmethod
-    def get_runner(cls, inventory):
+    def get_runner(cls, inventory: Optional[str]) -> "AnsibleRunner":
         try:
             return cls._runners[inventory]
         except KeyError:
             cls._runners[inventory] = cls(inventory)
             return cls._runners[inventory]
```

### Comparing `pytest-testinfra-8.1.0/tox.ini` & `pytest-testinfra-9.0.0/tox.ini`

 * *Files identical despite different names*

