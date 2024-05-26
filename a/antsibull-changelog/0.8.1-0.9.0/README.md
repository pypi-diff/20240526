# Comparing `tmp/antsibull-changelog-0.8.1.tar.gz` & `tmp/antsibull-changelog-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antsibull-changelog-0.8.1.tar", last modified: Thu Aug 27 20:16:49 2020, max compression
+gzip compressed data, was "antsibull-changelog-0.9.0.tar", last modified: Sat Jan 30 18:33:24 2021, max compression
```

## Comparing `antsibull-changelog-0.8.1.tar` & `antsibull-changelog-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0    35149 2020-05-29 18:47:37.201819 antsibull-changelog-0.8.1/LICENSE
--rw-r--r--   0        0        0     2087 2020-07-24 18:23:40.034261 antsibull-changelog-0.8.1/README.md
--rw-r--r--   0        0        0      120 2020-05-29 19:20:10.435755 antsibull-changelog-0.8.1/antsibull_changelog/__init__.py
--rw-r--r--   0        0        0      355 2020-06-10 21:21:51.197977 antsibull-changelog-0.8.1/antsibull_changelog/__main__.py
--rw-r--r--   0        0        0     1231 2020-05-29 19:20:10.435755 antsibull-changelog-0.8.1/antsibull_changelog/ansible.py
--rw-r--r--   0        0        0    15469 2020-07-26 12:04:59.696579 antsibull-changelog-0.8.1/antsibull_changelog/changelog_generator.py
--rw-r--r--   0        0        0    30547 2020-08-27 20:15:48.747953 antsibull-changelog-0.8.1/antsibull_changelog/changes.py
--rw-r--r--   0        0        0    21165 2020-08-27 20:15:48.747953 antsibull-changelog-0.8.1/antsibull_changelog/cli.py
--rw-r--r--   0        0        0    16103 2020-08-27 20:15:48.747953 antsibull-changelog-0.8.1/antsibull_changelog/config.py
--rw-r--r--   0        0        0      220 2020-05-29 19:20:10.439089 antsibull-changelog-0.8.1/antsibull_changelog/errors.py
--rw-r--r--   0        0        0     8072 2020-08-27 20:15:48.747953 antsibull-changelog-0.8.1/antsibull_changelog/fragment.py
--rw-r--r--   0        0        0    10876 2020-07-26 09:08:29.800739 antsibull-changelog-0.8.1/antsibull_changelog/lint.py
--rw-r--r--   0        0        0     1791 2020-05-29 19:20:10.439089 antsibull-changelog-0.8.1/antsibull_changelog/logger.py
--rw-r--r--   0        0        0    13616 2020-06-21 14:52:41.054821 antsibull-changelog-0.8.1/antsibull_changelog/plugins.py
--rw-r--r--   0        0        0     1765 2020-05-29 19:20:13.422619 antsibull-changelog-0.8.1/antsibull_changelog/rst.py
--rw-r--r--   0        0        0     6841 2020-08-27 19:59:12.149733 antsibull-changelog-0.8.1/antsibull_changelog/sanitize.py
--rw-r--r--   0        0        0     3414 2020-08-27 20:15:48.747953 antsibull-changelog-0.8.1/antsibull_changelog/utils.py
--rw-r--r--   0        0        0      982 2020-05-31 18:07:52.840945 antsibull-changelog-0.8.1/antsibull_changelog/yaml.py
--rw-r--r--   0        0        0     1270 2020-08-27 20:03:21.637274 antsibull-changelog-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      141 2020-06-01 20:40:00.717494 antsibull-changelog-0.8.1/tests/functional/bad/ansible-base-1.json
--rw-r--r--   0        0        0     3637 2020-05-29 18:47:37.235149 antsibull-changelog-0.8.1/tests/functional/bad/ansible-base-1.yaml
--rw-r--r--   0        0        0     3634 2020-08-18 18:05:05.074615 antsibull-changelog-0.8.1/tests/functional/bad/ansible-base-1.yaml-sanitized
--rw-r--r--   0        0        0      201 2020-05-29 18:47:37.238482 antsibull-changelog-0.8.1/tests/functional/bad/felixfontein.hosttech_dns-1.json
--rw-r--r--   0        0        0      691 2020-05-29 18:47:37.238482 antsibull-changelog-0.8.1/tests/functional/bad/felixfontein.hosttech_dns-1.yaml
--rw-r--r--   0        0        0      691 2020-08-18 18:05:05.074615 antsibull-changelog-0.8.1/tests/functional/bad/felixfontein.hosttech_dns-1.yaml-sanitized
--rw-r--r--   0        0        0     2563 2020-05-31 18:07:52.840945 antsibull-changelog-0.8.1/tests/functional/bad/random-1.json
--rw-r--r--   0        0        0     1080 2020-05-30 20:18:50.222084 antsibull-changelog-0.8.1/tests/functional/bad/random-1.yaml
--rw-r--r--   0        0        0      485 2020-08-18 18:05:05.074615 antsibull-changelog-0.8.1/tests/functional/bad/random-1.yaml-sanitized
--rw-r--r--   0        0        0      108 2020-05-31 18:07:52.840945 antsibull-changelog-0.8.1/tests/functional/bad/random-2.json
--rw-r--r--   0        0        0       12 2020-05-30 20:18:50.222084 antsibull-changelog-0.8.1/tests/functional/bad/random-2.yaml
--rw-r--r--   0        0        0      104 2020-05-31 18:07:52.844278 antsibull-changelog-0.8.1/tests/functional/bad/random-3.json
--rw-r--r--   0        0        0       13 2020-05-30 21:07:05.077511 antsibull-changelog-0.8.1/tests/functional/bad/random-3.yaml
--rw-r--r--   0        0        0       28 2020-08-18 18:05:05.074615 antsibull-changelog-0.8.1/tests/functional/bad/random-3.yaml-sanitized
--rw-r--r--   0        0        0      689 2020-05-30 21:07:05.077511 antsibull-changelog-0.8.1/tests/functional/bad/random-4.json
--rw-r--r--   0        0        0      193 2020-05-30 21:07:05.077511 antsibull-changelog-0.8.1/tests/functional/bad/random-4.yaml
--rw-r--r--   0        0        0       66 2020-08-18 18:05:05.074615 antsibull-changelog-0.8.1/tests/functional/bad/random-4.yaml-sanitized
--rw-r--r--   0        0        0    12984 2020-08-18 16:47:36.802877 antsibull-changelog-0.8.1/tests/functional/fixtures.py
--rw-r--r--   0        0        0     7451 2020-05-29 18:47:37.238482 antsibull-changelog-0.8.1/tests/functional/good/community.crypto-1.yaml
--rw-r--r--   0        0        0      711 2020-08-27 20:03:21.630608 antsibull-changelog-0.8.1/tests/functional/good/felixfontein.versioning_test_collection-1.yaml
--rw-r--r--   0        0        0      668 2020-05-29 18:47:37.238482 antsibull-changelog-0.8.1/tests/functional/good/felixfontein.versioning_test_collection-2.yaml
--rw-r--r--   0        0        0      882 2020-05-29 18:47:37.241815 antsibull-changelog-0.8.1/tests/functional/good/felixfontein.versioning_test_collection-3.yaml
--rw-r--r--   0        0        0     8390 2020-07-12 20:28:00.682764 antsibull-changelog-0.8.1/tests/functional/test_changelog_archive.py
--rw-r--r--   0        0        0    30555 2020-06-21 14:52:41.054821 antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_ansible.py
--rw-r--r--   0        0        0    27402 2020-07-12 13:29:46.620574 antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_ansible_classic.py
--rw-r--r--   0        0        0    37126 2020-08-27 20:03:21.630608 antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_collection.py
--rw-r--r--   0        0        0     3474 2020-08-27 20:03:21.633941 antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_lint.py
--rw-r--r--   0        0        0     1865 2020-05-31 18:07:52.844278 antsibull-changelog-0.8.1/tests/functional/test_changelog_yaml_linter.py
--rw-r--r--   0        0        0     2279 2020-08-18 18:05:05.074615 antsibull-changelog-0.8.1/tests/functional/test_changelog_yaml_sanitizer.py
--rw-r--r--   0        0        0      401 2020-05-31 15:46:52.354435 antsibull-changelog-0.8.1/tests/units/test_ansible.py
--rw-r--r--   0        0        0     5013 2020-05-31 15:46:52.354435 antsibull-changelog-0.8.1/tests/units/test_changes.py
--rw-r--r--   0        0        0     8617 2020-07-12 20:28:00.686097 antsibull-changelog-0.8.1/tests/units/test_config.py
--rw-r--r--   0        0        0     1821 2020-07-24 17:53:38.510047 antsibull-changelog-0.8.1/tests/units/test_fragment.py
--rw-r--r--   0        0        0     2256 2020-06-01 20:40:00.717494 antsibull-changelog-0.8.1/tests/units/test_utils.py
--rw-r--r--   0        0        0     3116 2020-08-27 20:16:49.389475 antsibull-changelog-0.8.1/setup.py
--rw-r--r--   0        0        0     3235 2020-08-27 20:16:49.389890 antsibull-changelog-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-05-29 18:47:37.201819 antsibull-changelog-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2642 2021-01-30 18:30:35.904176 antsibull-changelog-0.9.0/README.md
+-rw-r--r--   0        0        0      120 2020-05-29 19:20:10.435755 antsibull-changelog-0.9.0/antsibull_changelog/__init__.py
+-rw-r--r--   0        0        0      355 2020-06-10 21:21:51.197977 antsibull-changelog-0.9.0/antsibull_changelog/__main__.py
+-rw-r--r--   0        0        0     1320 2021-01-30 18:22:47.600377 antsibull-changelog-0.9.0/antsibull_changelog/ansible.py
+-rw-r--r--   0        0        0    17400 2021-01-30 18:22:47.600377 antsibull-changelog-0.9.0/antsibull_changelog/changelog_generator.py
+-rw-r--r--   0        0        0    33955 2021-01-30 18:22:47.600377 antsibull-changelog-0.9.0/antsibull_changelog/changes.py
+-rw-r--r--   0        0        0     6487 2021-01-30 18:22:47.603711 antsibull-changelog-0.9.0/antsibull_changelog/changes_resolvers.py
+-rw-r--r--   0        0        0    21484 2021-01-30 17:08:59.434055 antsibull-changelog-0.9.0/antsibull_changelog/cli.py
+-rw-r--r--   0        0        0    16633 2020-11-26 20:59:01.310473 antsibull-changelog-0.9.0/antsibull_changelog/config.py
+-rw-r--r--   0        0        0      220 2020-05-29 19:20:10.439089 antsibull-changelog-0.9.0/antsibull_changelog/errors.py
+-rw-r--r--   0        0        0    12532 2021-01-30 18:22:47.603711 antsibull-changelog-0.9.0/antsibull_changelog/fragment.py
+-rw-r--r--   0        0        0    12452 2021-01-30 18:22:47.603711 antsibull-changelog-0.9.0/antsibull_changelog/lint.py
+-rw-r--r--   0        0        0     1791 2020-05-29 19:20:10.439089 antsibull-changelog-0.9.0/antsibull_changelog/logger.py
+-rw-r--r--   0        0        0    13616 2020-06-21 14:52:41.054821 antsibull-changelog-0.9.0/antsibull_changelog/plugins.py
+-rw-r--r--   0        0        0     1765 2020-05-29 19:20:13.422619 antsibull-changelog-0.9.0/antsibull_changelog/rst.py
+-rw-r--r--   0        0        0     7575 2021-01-30 18:22:47.603711 antsibull-changelog-0.9.0/antsibull_changelog/sanitize.py
+-rw-r--r--   0        0        0     3414 2020-08-27 20:15:48.747953 antsibull-changelog-0.9.0/antsibull_changelog/utils.py
+-rw-r--r--   0        0        0      982 2020-05-31 18:07:52.840945 antsibull-changelog-0.9.0/antsibull_changelog/yaml.py
+-rw-r--r--   0        0        0     1276 2021-01-30 18:24:56.548086 antsibull-changelog-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      141 2020-06-01 20:40:00.717494 antsibull-changelog-0.9.0/tests/functional/bad/ansible-base-1.json
+-rw-r--r--   0        0        0     3637 2020-05-29 18:47:37.235149 antsibull-changelog-0.9.0/tests/functional/bad/ansible-base-1.yaml
+-rw-r--r--   0        0        0     3634 2020-08-18 18:05:05.074615 antsibull-changelog-0.9.0/tests/functional/bad/ansible-base-1.yaml-sanitized
+-rw-r--r--   0        0        0      201 2020-05-29 18:47:37.238482 antsibull-changelog-0.9.0/tests/functional/bad/felixfontein.hosttech_dns-1.json
+-rw-r--r--   0        0        0      691 2020-05-29 18:47:37.238482 antsibull-changelog-0.9.0/tests/functional/bad/felixfontein.hosttech_dns-1.yaml
+-rw-r--r--   0        0        0      691 2020-08-18 18:05:05.074615 antsibull-changelog-0.9.0/tests/functional/bad/felixfontein.hosttech_dns-1.yaml-sanitized
+-rw-r--r--   0        0        0     2563 2021-01-30 18:22:47.607044 antsibull-changelog-0.9.0/tests/functional/bad/random-1.json
+-rw-r--r--   0        0        0     1080 2020-05-30 20:18:50.222084 antsibull-changelog-0.9.0/tests/functional/bad/random-1.yaml
+-rw-r--r--   0        0        0      485 2020-08-18 18:05:05.074615 antsibull-changelog-0.9.0/tests/functional/bad/random-1.yaml-sanitized
+-rw-r--r--   0        0        0      108 2020-05-31 18:07:52.840945 antsibull-changelog-0.9.0/tests/functional/bad/random-2.json
+-rw-r--r--   0        0        0       12 2020-05-30 20:18:50.222084 antsibull-changelog-0.9.0/tests/functional/bad/random-2.yaml
+-rw-r--r--   0        0        0      104 2020-05-31 18:07:52.844278 antsibull-changelog-0.9.0/tests/functional/bad/random-3.json
+-rw-r--r--   0        0        0       13 2020-05-30 21:07:05.077511 antsibull-changelog-0.9.0/tests/functional/bad/random-3.yaml
+-rw-r--r--   0        0        0       28 2020-08-18 18:05:05.074615 antsibull-changelog-0.9.0/tests/functional/bad/random-3.yaml-sanitized
+-rw-r--r--   0        0        0      857 2021-01-30 18:22:47.607044 antsibull-changelog-0.9.0/tests/functional/bad/random-4.json
+-rw-r--r--   0        0        0      458 2021-01-30 18:22:47.607044 antsibull-changelog-0.9.0/tests/functional/bad/random-4.yaml
+-rw-r--r--   0        0        0      282 2021-01-30 18:22:47.607044 antsibull-changelog-0.9.0/tests/functional/bad/random-4.yaml-sanitized
+-rw-r--r--   0        0        0    13244 2021-01-30 18:22:47.607044 antsibull-changelog-0.9.0/tests/functional/fixtures.py
+-rw-r--r--   0        0        0     7451 2020-05-29 18:47:37.238482 antsibull-changelog-0.9.0/tests/functional/good/community.crypto-1.yaml
+-rw-r--r--   0        0        0      711 2020-08-27 20:03:21.630608 antsibull-changelog-0.9.0/tests/functional/good/felixfontein.versioning_test_collection-1.yaml
+-rw-r--r--   0        0        0      668 2020-05-29 18:47:37.238482 antsibull-changelog-0.9.0/tests/functional/good/felixfontein.versioning_test_collection-2.yaml
+-rw-r--r--   0        0        0      997 2021-01-30 18:22:47.607044 antsibull-changelog-0.9.0/tests/functional/good/felixfontein.versioning_test_collection-3.yaml
+-rw-r--r--   0        0        0    10829 2020-11-26 20:59:01.313806 antsibull-changelog-0.9.0/tests/functional/test_changelog_archive.py
+-rw-r--r--   0        0        0    30555 2020-06-21 14:52:41.054821 antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_ansible.py
+-rw-r--r--   0        0        0    27402 2020-07-12 13:29:46.620574 antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_ansible_classic.py
+-rw-r--r--   0        0        0    46327 2021-01-30 18:22:47.610378 antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_collection.py
+-rw-r--r--   0        0        0     5441 2021-01-30 18:22:47.610378 antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_lint.py
+-rw-r--r--   0        0        0     1865 2020-05-31 18:07:52.844278 antsibull-changelog-0.9.0/tests/functional/test_changelog_yaml_linter.py
+-rw-r--r--   0        0        0     2279 2020-08-18 18:05:05.074615 antsibull-changelog-0.9.0/tests/functional/test_changelog_yaml_sanitizer.py
+-rw-r--r--   0        0        0      401 2020-05-31 15:46:52.354435 antsibull-changelog-0.9.0/tests/units/test_ansible.py
+-rw-r--r--   0        0        0     5013 2020-05-31 15:46:52.354435 antsibull-changelog-0.9.0/tests/units/test_changes.py
+-rw-r--r--   0        0        0     8617 2020-07-12 20:28:00.686097 antsibull-changelog-0.9.0/tests/units/test_config.py
+-rw-r--r--   0        0        0     1821 2020-07-24 17:53:38.510047 antsibull-changelog-0.9.0/tests/units/test_fragment.py
+-rw-r--r--   0        0        0     2256 2020-06-01 20:40:00.717494 antsibull-changelog-0.9.0/tests/units/test_utils.py
+-rw-r--r--   0        0        0     3674 2021-01-30 18:33:24.859158 antsibull-changelog-0.9.0/setup.py
+-rw-r--r--   0        0        0     3840 2021-01-30 18:33:24.859542 antsibull-changelog-0.9.0/PKG-INFO
```

### Comparing `antsibull-changelog-0.8.1/LICENSE` & `antsibull-changelog-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/README.md` & `antsibull-changelog-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # antsibull-changelog -- Ansible Changelog Tool
+[![Python linting badge](https://github.com/ansible-community/antsibull-changelog/workflows/Python%20linting/badge.svg?event=push)](https://github.com/ansible-community/antsibull-changelog/actions)
+[![Python testing badge](https://github.com/ansible-community/antsibull-changelog/workflows/Python%20testing/badge.svg?event=push)](https://github.com/ansible-community/antsibull-changelog/actions)
+[![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-changelog)](https://codecov.io/gh/ansible-community/antsibull-changelog)
 
 A changelog generator used by Ansible and Ansible collections.
 
 - Using the
   [`antsibull-changelog` CLI tool](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelogs.rst).
 - Documentation on the [`changelogs/config.yaml` configuration file for `antsibull-changelog`](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelog-configuration.rst).
 - Documentation on the
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/ansible.py` & `antsibull-changelog-0.9.0/antsibull_changelog/ansible.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 try:
     from ansible import release as ansible_release
     HAS_ANSIBLE_RELEASE = True
 except ImportError:
     HAS_ANSIBLE_RELEASE = False
 
 
+OBJECT_TYPES = ('role', 'playbook')
+
+OTHER_PLUGIN_TYPES = ('module', 'test', 'filter')
+
+
 def get_documentable_plugins() -> Tuple[str, ...]:
     """
     Retrieve plugin types that can be documented. Does not include 'module'.
     """
     if HAS_ANSIBLE_CONSTANTS:
         return C.DOCUMENTABLE_PLUGINS
     return (
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/changelog_generator.py` & `antsibull-changelog-0.9.0/antsibull_changelog/changelog_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,23 @@
     Data for a changelog entry.
     """
 
     version: str
 
     modules: List[Any]
     plugins: Dict[Any, Any]
+    objects: Dict[Any, Any]
     changes: Dict[str, Union[str, List[str]]]
     preludes: List[Tuple[str, str]]
 
     def __init__(self, version: str):
         self.version = version
         self.modules = []
         self.plugins = dict()
+        self.objects = dict()
         self.changes = dict()
         self.preludes = []
 
     def has_no_changes(self, section_names: Optional[List[str]] = None) -> bool:
         """
         Determine whether there are changes.
 
@@ -52,15 +54,18 @@
         return all(not self.changes.get(section_name) for section_name in section_names)
 
     @property
     def empty(self) -> bool:
         """
         Determine whether the entry has no content at all.
         """
-        return not self.modules and not self.plugins and not self.preludes and self.has_no_changes()
+        return (
+            not self.modules and not self.plugins and not self.objects and
+            not self.preludes and self.has_no_changes()
+        )
 
     def add_section_content(self,
                             builder: RstBuilder,
                             section_name: str) -> None:
         """
         Add a section's content of fragments to the changelog.
         """
@@ -100,42 +105,50 @@
         Create a changelog generator.
         """
         self.config = config
         self.changes = changes
         self.flatmap = flatmap
 
         self.plugin_resolver = changes.get_plugin_resolver(plugins)
+        self.object_resolver = changes.get_object_resolver()
         self.fragment_resolver = changes.get_fragment_resolver(fragments)
 
     @staticmethod
     def _get_entry_config(release_entries: MutableMapping[str, ChangelogEntry],
                           entry_version: str) -> ChangelogEntry:
         """
         Create (if not existing) and return release entry for a given version.
         """
         if entry_version not in release_entries:
             release_entries[entry_version] = ChangelogEntry(entry_version)
 
         return release_entries[entry_version]
 
-    def _update_modules_plugins(self, entry_config: ChangelogEntry, release: dict) -> None:
+    def _update_modules_plugins_objects(self, entry_config: ChangelogEntry, release: dict) -> None:
         """
         Update a release entry given a release information dict.
         """
         plugins = self.plugin_resolver.resolve(release)
+        objects = self.object_resolver.resolve(release)
 
         if 'module' in plugins:
             entry_config.modules += plugins.pop('module')
 
         for plugin_type, plugin_list in plugins.items():
             if plugin_type not in entry_config.plugins:
                 entry_config.plugins[plugin_type] = []
 
             entry_config.plugins[plugin_type] += plugin_list
 
+        for object_type, object_list in objects.items():
+            if object_type not in entry_config.objects:
+                entry_config.objects[object_type] = []
+
+            entry_config.objects[object_type] += object_list
+
     def _collect_entry(self,
                        entry_config: ChangelogEntry,
                        entry_version: str,
                        versions: List[str]) -> None:
         """
         Do actual work of collecting data for a changelog entry.
         """
@@ -164,15 +177,15 @@
                     else:
                         content = dest_changes.get(section)
                         if isinstance(content, list):
                             content.extend(lines)
                         else:
                             dest_changes[section] = list(lines)
 
-            self._update_modules_plugins(entry_config, release)
+            self._update_modules_plugins_objects(entry_config, release)
 
     def collect(self,
                 squash: bool = False,
                 after_version: Optional[str] = None,
                 until_version: Optional[str] = None) -> List[ChangelogEntry]:
         """
         Collect release entries.
@@ -226,14 +239,19 @@
             start_level=start_level)
         self._add_modules(
             builder,
             changelog_entry.modules,
             flatmap=self.flatmap,
             fqcn_prefix=fqcn_prefix,
             start_level=start_level)
+        self._add_objects(
+            builder,
+            changelog_entry.objects,
+            fqcn_prefix=fqcn_prefix,
+            start_level=start_level)
 
     def generate_to(self,  # pylint: disable=too-many-arguments
                     builder: RstBuilder,
                     start_level: int = 0,
                     squash: bool = False,
                     after_version: Optional[str] = None,
                     until_version: Optional[str] = None) -> None:
@@ -390,14 +408,49 @@
                 if fqcn_prefix:
                     module_name = '%s.%s' % (fqcn_prefix, module_name)
 
                 builder.add_raw_rst('- %s - %s' % (module_name, module['description']))
 
             builder.add_raw_rst('')
 
+    @staticmethod
+    def _add_objects(builder: RstBuilder,
+                     objects_database: Dict[str, List[Dict[str, Any]]],
+                     fqcn_prefix: Optional[str],
+                     start_level: int = 0) -> None:
+        """
+        Add new objects to the changelog.
+        """
+        if not objects_database:
+            return
+
+        for object_type in sorted(objects_database):
+            objects = objects_database.get(object_type)
+            if not objects:
+                continue
+
+            builder.add_section('New ' + object_type.title() + 's', start_level + 1)
+
+            ChangelogGenerator.add_objects(builder, objects, fqcn_prefix)
+
+            builder.add_raw_rst('')
+
+    @staticmethod
+    def add_objects(builder: RstBuilder,
+                    objects: List[Dict[str, Any]],
+                    fqcn_prefix: Optional[str]) -> None:
+        """
+        Add new objects of one type to the changelog.
+        """
+        for ansible_object in sorted(objects, key=lambda ansible_object: ansible_object['name']):
+            object_name = ansible_object['name']
+            if fqcn_prefix:
+                object_name = '%s.%s' % (fqcn_prefix, object_name)
+            builder.add_raw_rst('- %s - %s' % (object_name, ansible_object['description']))
+
 
 def generate_changelog(paths: PathsConfig,  # pylint: disable=too-many-arguments
                        config: ChangelogConfig,
                        changes: ChangesBase,
                        plugins: Optional[List[PluginDescription]] = None,
                        fragments: Optional[List[ChangelogFragment]] = None,
                        flatmap: bool = True):
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/changes.py` & `antsibull-changelog-0.9.0/antsibull_changelog/changes.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,74 +12,53 @@
 import abc
 import collections
 import datetime
 import os
 
 from typing import Any, Callable, Dict, List, Optional, Set, cast
 
+from .changes_resolvers import (
+    FragmentResolver,
+    PluginResolver,
+    LegacyFragmentResolver,
+    LegacyPluginResolver,
+    LegacyObjectResolver,
+    ChangesDataFragmentResolver,
+    ChangesDataPluginResolver,
+    ChangesDataObjectResolver
+)
 from .config import ChangelogConfig
 from .fragment import ChangelogFragment, load_fragments
 from .logger import LOGGER
 from .plugins import PluginDescription, load_plugins
 from .sanitize import sanitize_changes
 from .utils import get_version_constructor, is_release_version
 from .yaml import load_yaml, store_yaml
 
 
-class FragmentResolver(metaclass=abc.ABCMeta):
-    # pylint: disable=too-few-public-methods
-    """
-    Allows to resolve a release section to a list of changelog fragments.
-    """
-
-    @abc.abstractmethod
-    def resolve(self, release: dict) -> List[ChangelogFragment]:
-        """
-        Return a list of ``ChangelogFragment`` objects from the given release object.
-
-        :arg release: A release description
-        :return: A list of changelog fragments
-        """
-
-
-class PluginResolver(metaclass=abc.ABCMeta):
-    # pylint: disable=too-few-public-methods
-    """
-    Allows to resolve a release section to a plugin description database.
-    """
-
-    @abc.abstractmethod
-    def resolve(self, release: dict) -> Dict[str, List[Dict[str, Any]]]:
-        """
-        Return a dictionary of plugin types mapping to lists of plugin descriptions
-        for the given release.
-
-        :arg release: A release description
-        :return: A map of plugin types to lists of plugin descriptions
-        """
-
-
 class ChangesBase(metaclass=abc.ABCMeta):
     """
     Read, write and manage change metadata.
     """
 
     config: ChangelogConfig
     path: str
     data: dict
     known_plugins: Set[str]
+    known_objects: Set[str]
     known_fragments: Set[str]
     ancestor: Optional[str]
 
     def __init__(self, config: ChangelogConfig, path: str):
         self.config = config
         self.path = path
         self.data = self.empty()
         self.known_fragments = set()
         self.known_plugins = set()
+        self.known_objects = set()
         self.ancestor = None
 
     def version_constructor(self, version: str) -> Any:
         """
         Create a version object.
         """
         return get_version_constructor(self.config)(version)
@@ -137,14 +116,22 @@
                        allow_removals: Optional[bool]) -> None:
         """
         Update plugin descriptions, and remove plugins which are not in the provided list
         of plugins.
         """
 
     @abc.abstractmethod
+    def update_objects(self, objects: List[PluginDescription],
+                       allow_removals: Optional[bool]) -> None:
+        """
+        Update object descriptions, and remove objects which are not in the provided list
+        of objects.
+        """
+
+    @abc.abstractmethod
     def update_fragments(self, fragments: List[ChangelogFragment],
                          load_extra_fragments: Optional[
                              Callable[[str], List[ChangelogFragment]]] = None
                          ) -> None:
         """
         Update fragment contents, and remove fragment contents which are not in the provided
         list of fragments.
@@ -160,26 +147,28 @@
         """
         Save the change metadata to disk.
         """
         self.sort()
         self.data['ancestor'] = self.ancestor
         store_yaml(self.path, self.data)
 
-    def add_release(self, version: str, codename: Optional[str], release_date: datetime.date):
+    def add_release(self, version: str, codename: Optional[str],
+                    release_date: datetime.date, update_existing=False):
         """
         Add a new releases to the changes metadata.
         """
         if version not in self.releases:
-            self.releases[version] = dict(
-                release_date=release_date.isoformat(),
-            )
-            if codename is not None:
-                self.releases[version]['codename'] = codename
-        else:
+            self.releases[version] = dict()
+        elif not update_existing:
             LOGGER.warning('release {} already exists', version)
+            return
+
+        self.releases[version]['release_date'] = release_date.isoformat()
+        if codename is not None:
+            self.releases[version]['codename'] = codename
 
     @abc.abstractmethod
     def add_fragment(self, fragment: ChangelogFragment, version: str):
         """
         Add a new changelog fragment to the change metadata for the given version.
         """
 
@@ -218,107 +207,65 @@
             if plugin.type not in plugins:
                 plugins[plugin.type] = []
 
             plugins[plugin.type].append(self._create_plugin_entry(plugin))
 
         return True
 
-    @abc.abstractmethod
-    def get_plugin_resolver(
-            self, plugins: Optional[List[PluginDescription]] = None) -> PluginResolver:
+    def add_object(self, ansible_object: PluginDescription, version: str):
         """
-        Create a plugin resolver.
+        Add a new object to the change metadata for the given version.
 
-        If the plugins are not provided and needed by this object, they might be loaded.
-        """
-
-    @abc.abstractmethod
-    def get_fragment_resolver(
-            self, fragments: Optional[List[ChangelogFragment]] = None) -> FragmentResolver:
-        """
-        Create a fragment resolver.
+        If the object happens to be already known (for another version),
+        it will not be added.
 
-        If the fragments are not provided and needed by this object, they might be loaded.
+        :return: ``True`` if the object was added for this version
         """
+        composite_name = '%s/%s' % (ansible_object.type, ansible_object.name)
 
+        if composite_name in self.known_objects:
+            return False
 
-class LegacyFragmentResolver(FragmentResolver):
-    # pylint: disable=too-few-public-methods
-    """
-    Given a list of changelog fragments, allows to resolve from a list of fragment names.
-    """
-
-    fragments: Dict[str, ChangelogFragment]
+        self.known_objects.add(composite_name)
 
-    def __init__(self, fragments: List[ChangelogFragment]):
-        """
-        Create a simple fragment resolver.
-        """
-        self.fragments = dict()
-        for fragment in fragments:
-            self.fragments[fragment.name] = fragment
+        if 'objects' not in self.releases[version]:
+            self.releases[version]['objects'] = {}
 
-    def resolve(self, release: dict) -> List[ChangelogFragment]:
-        """
-        Return a list of ``ChangelogFragment`` objects from the given release object.
+        objects = self.releases[version]['objects']
 
-        :arg release: A release description
-        :return: A list of changelog fragments
-        """
-        fragment_names: List[str] = release.get('fragments', [])
-        return [self.fragments[fragment] for fragment in fragment_names]
+        if ansible_object.type not in objects:
+            objects[ansible_object.type] = []
 
+        objects[ansible_object.type].append(self._create_plugin_entry(ansible_object))
 
-class LegacyPluginResolver(PluginResolver):
-    # pylint: disable=too-few-public-methods
-    """
-    Provides a plugin resolved based on a list of ``PluginDescription`` objects.
-    """
-
-    plugins: Dict[str, Dict[str, Dict[str, Any]]]
+        return True
 
-    @staticmethod
-    def resolve_plugin(plugin: PluginDescription) -> Dict[str, Any]:
+    @abc.abstractmethod
+    def get_plugin_resolver(
+            self, plugins: Optional[List[PluginDescription]] = None) -> PluginResolver:
         """
-        Convert a ``PluginDecscription`` object to a plugin description dictionary.
+        Create a plugin resolver.
+
+        If the plugins are not provided and needed by this object, they might be loaded.
         """
-        return dict(
-            name=plugin.name,
-            namespace=plugin.namespace,
-            description=plugin.description,
-        )
 
-    def __init__(self, plugins: List[PluginDescription]):
+    @abc.abstractmethod
+    def get_object_resolver(self) -> PluginResolver:
         """
-        Create a simple plugin resolver from a list of ``PluginDescription`` objects.
+        Create a object resolver.
         """
-        self.plugins = dict()
-        for plugin in plugins:
-            if plugin.type not in self.plugins:
-                self.plugins[plugin.type] = dict()
 
-            self.plugins[plugin.type][plugin.name] = self.resolve_plugin(plugin)
+    @abc.abstractmethod
+    def get_fragment_resolver(
+            self, fragments: Optional[List[ChangelogFragment]] = None) -> FragmentResolver:
+        """
+        Create a fragment resolver.
 
-    def resolve(self, release: dict) -> Dict[str, List[Dict[str, Any]]]:
+        If the fragments are not provided and needed by this object, they might be loaded.
         """
-        Return a dictionary of plugin types mapping to lists of plugin descriptions
-        for the given release.
-
-        :arg release: A release description
-        :return: A map of plugin types to lists of plugin descriptions
-        """
-        result = dict()
-        if 'modules' in release:
-            result['module'] = [self.plugins['module'][module_name]
-                                for module_name in release['modules']]
-        if 'plugins' in release:
-            for plugin_type, plugin_names in release['plugins'].items():
-                result[plugin_type] = [self.plugins[plugin_type][plugin_name]
-                                       for plugin_name in plugin_names]
-        return result
 
 
 class ChangesMetadata(ChangesBase):
     """
     Read, write and manage classic Ansible (2.9 and earlier) change metadata.
     """
 
@@ -380,14 +327,22 @@
                         if plugin not in valid_plugins[plugin_type])
                     config['plugins'][plugin_type] = [
                         plugin for plugin in config['plugins'][plugin_type]
                         if plugin not in invalid_plugins]
                     self.known_plugins -= set(
                         '%s/%s' % (plugin_type, plugin) for plugin in invalid_plugins)
 
+    def update_objects(self, objects: List[PluginDescription],
+                       allow_removals: Optional[bool]) -> None:
+        """
+        Update object descriptions, and remove objects which are not in the provided list
+        of objects.
+        """
+        return
+
     def update_fragments(self, fragments: List[ChangelogFragment],
                          load_extra_fragments: Optional[
                              Callable[[str], List[ChangelogFragment]]] = None
                          ) -> None:
         """
         Update fragment contents, and remove fragment contents which are not in the provided
         list of fragments.
@@ -447,67 +402,32 @@
         if plugins is None:
             plugins = load_plugins(paths=self.config.paths,
                                    collection_details=self.config.collection_details,
                                    version=self.latest_version,
                                    force_reload=False)
         return LegacyPluginResolver(plugins)
 
+    def get_object_resolver(self) -> PluginResolver:
+        """
+        Create a dummy object resolver.
+        """
+        return LegacyObjectResolver()
+
     def get_fragment_resolver(
             self, fragments: Optional[List[ChangelogFragment]] = None) -> FragmentResolver:
         """
         Create a fragment resolver.
 
         If the fragments are not provided and needed by this object, they **will** be loaded.
         """
         if fragments is None:
             fragments = load_fragments(paths=self.config.paths, config=self.config)
         return LegacyFragmentResolver(fragments)
 
 
-class ChangesDataFragmentResolver(FragmentResolver):
-    # pylint: disable=too-few-public-methods
-    """
-    A ``FragmentResolver`` class for modern ``ChangesData`` objects.
-    """
-
-    def resolve(self, release: dict) -> List[ChangelogFragment]:
-        """
-        Return a list of ``ChangelogFragment`` objects from the given release object.
-
-        :arg release: A release description
-        :return: A list of changelog fragments
-        """
-        changes = release.get('changes')
-        if changes is None:
-            return []
-        return [ChangelogFragment.from_dict(changes)]
-
-
-class ChangesDataPluginResolver(PluginResolver):
-    # pylint: disable=too-few-public-methods
-    """
-    A ``PluginResolver`` class for modern ``ChangesData`` objects.
-    """
-
-    def resolve(self, release: dict) -> Dict[str, List[Dict[str, Any]]]:
-        """
-        Return a dictionary of plugin types mapping to lists of plugin descriptions
-        for the given release.
-
-        :arg release: A release description
-        :return: A map of plugin types to lists of plugin descriptions
-        """
-        result = dict()
-        if 'modules' in release:
-            result['module'] = release['modules']
-        if 'plugins' in release:
-            result.update(release['plugins'])
-        return result
-
-
 class ChangesData(ChangesBase):
     """
     Read, write and manage modern change metadata.
 
     This is the format used for ansible-base 2.10+ and for Ansible collections.
     """
 
@@ -530,14 +450,18 @@
         super().load(data_override=data_override)
 
         for _, config in self.releases.items():
             for plugin_type, plugins in config.get('plugins', {}).items():
                 self.known_plugins |= set(
                     '%s/%s' % (plugin_type, plugin['name']) for plugin in plugins)
 
+            for object_type, objects in config.get('objects', {}).items():
+                self.known_objects |= set(
+                    '%s/%s' % (object_type, ansible_object['name']) for ansible_object in objects)
+
             modules = config.get('modules', [])
 
             self.known_plugins |= set('module/%s' % module['name'] for module in modules)
 
             self.known_fragments |= set(config.get('fragments', []))
 
     def update_plugins(self, plugins: List[PluginDescription],
@@ -586,14 +510,48 @@
                     else:
                         config['plugins'][plugin_type] = [
                             self._create_plugin_entry(valid_plugins[plugin_type][plugin['name']])
                             if plugin['name'] not in invalid_plugin_names else
                             plugin
                             for plugin in config['plugins'][plugin_type]]
 
+    def update_objects(self, objects: List[PluginDescription],
+                       allow_removals: Optional[bool]) -> None:
+        """
+        Update object descriptions, and remove objects which are not in the provided list
+        of objects.
+        """
+        valid_objects: Dict[str, Dict[str, PluginDescription]] = collections.defaultdict(dict)
+
+        for ansible_object in objects:
+            valid_objects[ansible_object.type][ansible_object.name] = ansible_object
+
+        for _, config in self.releases.items():
+            if 'objects' in config:
+                for object_type in config['objects']:
+                    invalid_object_names = set(
+                        ansible_object['name'] for ansible_object in config['objects'][object_type]
+                        if ansible_object['name'] not in valid_objects[object_type])
+                    if allow_removals:
+                        config['objects'][object_type] = [
+                            self._create_plugin_entry(
+                                valid_objects[object_type][ansible_object['name']])
+                            for ansible_object in config['objects'][object_type]
+                            if ansible_object['name'] not in invalid_object_names]
+                        self.known_objects -= set(
+                            '%s/%s' % (object_type, object_name)
+                            for object_name in invalid_object_names)
+                    else:
+                        config['objects'][object_type] = [
+                            self._create_plugin_entry(
+                                valid_objects[object_type][ansible_object['name']])
+                            if ansible_object['name'] not in invalid_object_names else
+                            ansible_object
+                            for ansible_object in config['objects'][object_type]]
+
     def update_fragments(self, fragments: List[ChangelogFragment],
                          load_extra_fragments: Optional[
                              Callable[[str], List[ChangelogFragment]]] = None
                          ) -> None:
         """
         Update fragment contents, and remove fragment contents which are not in the provided
         list of fragments.
@@ -617,15 +575,16 @@
                     if fragment not in valid_fragments)
                 config['fragments'] = [
                     fragment for fragment in config['fragments']
                     if fragment not in invalid_fragments]
                 self.known_fragments -= invalid_fragments
 
                 config['changes'] = ChangelogFragment.combine([
-                    valid_fragments[fragment] for fragment in config['fragments']])
+                    valid_fragments[fragment] for fragment in config['fragments']],
+                    ignore_obj_adds=True)
 
     def sort(self) -> None:
         """
         Sort change metadata in place.
         """
         super().sort()
 
@@ -634,52 +593,121 @@
                 config['modules'] = sorted(config['modules'], key=lambda module: module['name'])
 
             if 'plugins' in config:
                 for plugin_type in config['plugins']:
                     config['plugins'][plugin_type] = sorted(
                         config['plugins'][plugin_type], key=lambda plugin: plugin['name'])
 
+            if 'objects' in config:
+                for object_type in config['objects']:
+                    config['objects'][object_type] = sorted(
+                        config['objects'][object_type],
+                        key=lambda ansible_object: ansible_object['name'])
+
             if 'fragments' in config:
                 config['fragments'] = sorted(config['fragments'])
 
             if 'changes' in config:
                 config['changes'] = {
                     section: sorted(entries) if section != self.config.prelude_name else entries
                     for section, entries in sorted(config['changes'].items())
                 }
 
+    def _add_fragment_obj(self, obj_class, obj_type, entry, version: str):
+        """
+        Add an object or a plugin from a changelog fragment.
+        """
+        if obj_class == 'object':
+            composite_name = '%s/%s' % (obj_type, entry['name'])
+            if composite_name in self.known_objects:
+                LOGGER.warning(
+                    'Ignore adding %s object "%s" from changelog fragment' % (
+                        obj_type, entry['name']))
+                return
+            self.known_objects.add(composite_name)
+            toplevel_type = 'objects'
+            has_categories = True
+        if obj_class == 'plugin':
+            composite_name = '%s/%s' % (obj_type, entry['name'])
+            if composite_name in self.known_plugins:
+                LOGGER.warning(
+                    'Ignore adding %s plugin "%s" from changelog fragment' % (
+                        obj_type, entry['name']))
+                return
+            self.known_plugins.add(composite_name)
+            if obj_type == 'module':
+                toplevel_type = 'modules'
+                has_categories = False
+            else:
+                toplevel_type = 'plugins'
+                has_categories = True
+
+        if has_categories:
+            if toplevel_type not in self.releases[version]:
+                self.releases[version][toplevel_type] = {}
+
+            categories = self.releases[version][toplevel_type]
+
+            if obj_type not in categories:
+                categories[obj_type] = []
+
+            obj_list = categories[obj_type]
+        else:
+            if toplevel_type not in self.releases[version]:
+                self.releases[version][toplevel_type] = []
+
+            obj_list = self.releases[version][toplevel_type]
+
+        obj_list.append({
+            'name': entry['name'],
+            'description': entry['description'],
+            'namespace': entry.get('namespace'),
+        })
+
+    def _add_fragment_content(self, version: str, changes: Dict[str, Any],
+                              section: str, lines: Any):
+        """
+        Add contents of a changelog fragment. Helps implementing add_fragment().
+        """
+        if section == self.config.prelude_name:
+            if section in changes:
+                raise ValueError('Found prelude section "{0}" more than once!'.format(section))
+            changes[section] = lines
+        elif section == self.config.trivial_section_name:
+            # Ignore trivial section entries
+            return
+        elif section.startswith('add') and '.' in section:
+            obj_class, obj_type = section[4:].split('.', 1)
+            for entry in lines:
+                self._add_fragment_obj(obj_class, obj_type, entry, version)
+        elif section not in self.config.sections:
+            raise ValueError('Found unknown section "{0}"'.format(section))
+        else:
+            if section not in changes:
+                changes[section] = []
+            changes[section].extend(lines)
+
     def add_fragment(self, fragment: ChangelogFragment, version: str):
         """
         Add a changelog fragment to the change metadata.
         """
-        if fragment.name in self.known_fragments:
+        if fragment.name in self.known_fragments and self.config.prevent_known_fragments:
             return False
 
         self.known_fragments.add(fragment.name)
 
         if 'changes' not in self.releases[version]:
             self.releases[version]['changes'] = dict()
         changes = self.releases[version]['changes']
 
         if 'fragments' not in self.releases[version]:
             self.releases[version]['fragments'] = []
 
         for section, lines in fragment.content.items():
-            if section == self.config.prelude_name:
-                if section in changes:
-                    raise ValueError('Found prelude section "{0}" more than once!'.format(section))
-                changes[section] = lines
-            elif section == self.config.trivial_section_name:
-                continue
-            elif section not in self.config.sections:
-                raise ValueError('Found unknown section "{0}"'.format(section))
-            else:
-                if section not in changes:
-                    changes[section] = []
-                changes[section].extend(lines)
+            self._add_fragment_content(version, changes, section, lines)
 
         self.releases[version]['fragments'].append(fragment.name)
         return True
 
     @staticmethod
     def _create_plugin_entry(plugin: PluginDescription) -> dict:
         return LegacyPluginResolver.resolve_plugin(plugin)
@@ -689,14 +717,20 @@
         """
         Create a plugin resolver.
 
         The plugins list is not used.
         """
         return ChangesDataPluginResolver()
 
+    def get_object_resolver(self) -> PluginResolver:
+        """
+        Create a object resolver.
+        """
+        return ChangesDataObjectResolver()
+
     def get_fragment_resolver(
             self, fragments: Optional[List[ChangelogFragment]] = None) -> FragmentResolver:
         """
         Create a fragment resolver.
 
         The fragments list is not used.
         """
@@ -765,51 +799,80 @@
     """
     path = os.path.join(config.paths.changelog_dir, config.changes_file)
     if config.changes_format == 'classic':
         return ChangesMetadata(config, path)
     return ChangesData(config, path)
 
 
+def _add_plugins_filters(changes: ChangesBase,
+                         plugins: List[PluginDescription],
+                         objects: List[PluginDescription],
+                         version: str,
+                         ) -> None:
+    # filter out plugins which were not added in this release
+    plugins = list(filter(lambda p: any([
+        version.startswith('%s.' % p.version_added),
+        version.startswith('%s-' % p.version_added),  # needed for semver
+        version.startswith('%s+' % p.version_added),  # needed for semver
+        version == p.version_added
+    ]), plugins))
+
+    # filter out objects which were not added in this release
+    objects = list(filter(lambda p: any([
+        version.startswith('%s.' % p.version_added),
+        version.startswith('%s-' % p.version_added),  # needed for semver
+        version.startswith('%s+' % p.version_added),  # needed for semver
+        version == p.version_added
+    ]), objects))
+
+    for plugin in plugins:
+        changes.add_plugin(plugin, version)
+
+    for ansible_object in objects:
+        changes.add_object(ansible_object, version)
+
+
 def add_release(config: ChangelogConfig,  # pylint: disable=too-many-arguments
                 changes: ChangesBase,
                 plugins: List[PluginDescription],
                 fragments: List[ChangelogFragment],
                 version: str,
                 codename: Optional[str],
                 date: datetime.date,
-                save_changes: bool = True) -> None:
+                save_changes: bool = True,
+                update_existing: bool = False,
+                objects: Optional[List[PluginDescription]] = None,
+                ) -> None:
     """
     Add a release to the change metadata.
 
     :arg changes: Changes metadata to update
     :arg plugins: List of all plugin descriptions
+    :arg objects: List of all object descriptions
     :arg fragments: List of all changelog fragments
     :arg version: The version for the new release
     :arg codename: The codename for the new release. Optional for collections
     :arg date: The release date
+    :arg update_existing: When set to ``True``, will update an existing release
+                          instead of ignoring it
     """
+    # for backwards compatibility, objects can be None
+    if objects is None:
+        objects = []
+
     # make sure the version parses
     version_constructor = get_version_constructor(config)
     version_constructor(version)
 
     LOGGER.info('release version {} is a {} version', version,
                 'release' if is_release_version(config, version) else 'pre-release')
 
-    # filter out plugins which were not added in this release
-    plugins = list(filter(lambda p: any([
-        version.startswith('%s.' % p.version_added),
-        version.startswith('%s-' % p.version_added),  # needed for semver
-        version.startswith('%s+' % p.version_added),  # needed for semver
-        version == p.version_added
-    ]), plugins))
-
-    changes.add_release(version, codename, date)
+    changes.add_release(version, codename, date, update_existing=update_existing)
 
-    for plugin in plugins:
-        changes.add_plugin(plugin, version)
+    _add_plugins_filters(changes, plugins, objects, version)
 
     fragments_added = []
     for fragment in fragments:
         if changes.add_fragment(fragment, version):
             fragments_added.append(fragment)
 
     if save_changes:
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/cli.py` & `antsibull-changelog-0.9.0/antsibull_changelog/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,18 @@
     release_parser.add_argument('--version',
                                 help='override release version')
     release_parser.add_argument('--codename',
                                 help='override/set release codename')
     release_parser.add_argument('--date',
                                 default=str(datetime.date.today()),
                                 help='override release date')
+    release_parser.add_argument('--update-existing',
+                                action='store_true',
+                                help='if the release already exists, updates the release '
+                                     'date and (if relevant) the codename')
 
     generate_parser = subparsers.add_parser('generate',
                                             parents=[common, common_build,
                                                      is_collection, collection_details],
                                             help='generate the changelog')
     generate_parser.set_defaults(func=command_generate)
 
@@ -426,15 +430,16 @@
         args, paths, collection_details, config, changes, plugins, fragments)
     add_release(
         config, changes,
         # Need cast() here because there is currently no way to mark _do_refresh so that
         # it does not convert a non-None value to None for plugins or fragments
         cast(List[PluginDescription], plugins),
         cast(List[ChangelogFragment], fragments),
-        version, codename, date)
+        version, codename, date,
+        update_existing=args.update_existing)
     generate_changelog(paths, config, changes, plugins, fragments, flatmap=flatmap)
 
     return 0
 
 
 def command_generate(args: Any) -> int:
     """
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/config.py` & `antsibull-changelog-0.9.0/antsibull_changelog/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -250,14 +250,15 @@
     notes_dir: str
     prelude_name: str
     prelude_title: str
     new_plugins_after_name: str
     changes_file: str
     changes_format: str
     keep_fragments: bool
+    prevent_known_fragments: bool
     use_fqcn: bool
     archive_path_template: Optional[str]
     changelog_filename_template: str
     changelog_filename_version_depth: int
     mention_ancestor: bool
     trivial_section_name: str
     release_tag_re: str
@@ -282,14 +283,16 @@
         self.notes_dir = self.config.get('notesdir', 'fragments')
         self.prelude_name = self.config.get('prelude_section_name', 'release_summary')
         self.prelude_title = self.config.get('prelude_section_title', 'Release Summary')
         self.new_plugins_after_name = self.config.get('new_plugins_after_name', '')  # not used
         self.changes_file = self.config.get('changes_file', '.changes.yaml')
         self.changes_format = self.config.get('changes_format', 'classic')
         self.keep_fragments = self.config.get('keep_fragments', self.changes_format == 'classic')
+        self.prevent_known_fragments = self.config.get(
+            'prevent_known_fragments', self.keep_fragments)
         self.use_fqcn = self.config.get('use_fqcn', False)
         self.archive_path_template = self.config.get('archive_path_template')
         self.changelog_filename_template = self.config.get(
             'changelog_filename_template', 'CHANGELOG-v%s.rst')
         self.changelog_filename_version_depth = self.config.get(
             'changelog_filename_version_depth', 2)
         self.mention_ancestor = self.config.get('mention_ancestor', True)
@@ -315,14 +318,17 @@
             self.use_semantic_versioning = self.config.get('use_semantic_versioning', False)
 
         if self.changes_format not in ('classic', 'combined'):
             raise ChangelogError('changes_format must be one of "classic" and "combined"')
         if self.changes_format == 'classic' and not self.keep_fragments:
             raise ChangelogError('changes_format == "classic" cannot be '
                                  'combined with keep_fragments == False')
+        if self.changes_format == 'classic' and not self.prevent_known_fragments:
+            raise ChangelogError('changes_format == "classic" cannot be '
+                                 'combined with prevent_known_fragments == False')
 
         sections = collections.OrderedDict([(self.prelude_name, self.prelude_title)])
         for section_name, section_title in self.config.get('sections', DEFAULT_SECTIONS):
             sections[section_name] = section_title
         self.sections = sections
 
     def store(self) -> None:
@@ -354,14 +360,16 @@
                     'pre_release_tag_re': self.pre_release_tag_re,
                 })
         if self.title is not None:
             config['title'] = self.title
         should_always_refresh = (self.changes_format == 'classic')
         if self.always_refresh != ('full' if should_always_refresh else 'none'):
             config['always_refresh'] = self.always_refresh
+        if self.keep_fragments != self.prevent_known_fragments:
+            config['prevent_known_fragments'] = self.prevent_known_fragments
         if self.flatmap is not None:
             config['flatmap'] = self.flatmap
         if self.archive_path_template is not None:
             config['archive_path_template'] = self.archive_path_template
 
         sections = []
         for key, value in self.sections.items():
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/lint.py` & `antsibull-changelog-0.9.0/antsibull_changelog/lint.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import re
 
 from typing import Any, List, Optional, Tuple, Type, cast
 
 import semantic_version
 
-from .ansible import get_documentable_plugins
+from .ansible import get_documentable_plugins, OBJECT_TYPES, OTHER_PLUGIN_TYPES
 from .config import ChangelogConfig, CollectionDetails, PathsConfig
 from .fragment import ChangelogFragment, ChangelogFragmentLinter
 from .yaml import load_yaml
 
 
 ISO_DATE_REGEX = re.compile('^[0-9]{4}-(?:0[1-9]|1[0-2])-(?:0[1-9]|[12][0-9]|3[01])$')
 
@@ -30,14 +30,16 @@
 
     errors: List[Tuple[str, int, int, str]]
     path: str
 
     def __init__(self, path):
         self.errors = []
         self.path = path
+        self.valid_plugin_types = set(get_documentable_plugins())
+        self.valid_plugin_types.update(OTHER_PLUGIN_TYPES)
 
     def check_version(self, version: Any, message: str) -> Optional[semantic_version.Version]:
         """
         Check that the given version is a valid semantic version.
 
         :arg version: Version string to check
         :arg message: Message to prepend to error
@@ -127,25 +129,47 @@
         Lint a plugin dictionary.
 
         :arg version_str: To which release the plugin dictionary belongs
         :arg plugins_dict: The plugin dictionary
         """
         for plugin_type, plugins in plugins_dict.items():
             if self.verify_type(plugin_type, (str, ), ['releases', version_str, 'plugins']):
-                if plugin_type not in get_documentable_plugins() or plugin_type == 'module':
+                if plugin_type not in self.valid_plugin_types:
                     self.errors.append((
                         self.path, 0, 0,
                         'Unknown plugin type {0!r} in {1}'.format(
                             plugin_type, self._format_yaml_path(
                                 ['releases', version_str, 'plugins']))))
             if self.verify_type(plugins, (list, ),
                                 ['releases', version_str, 'plugins', plugin_type]):
                 for idx, plugin in enumerate(plugins):
                     self.verify_plugin(plugin,
-                                       ['releases', version_str, 'modules', plugin_type, idx],
+                                       ['releases', version_str, 'plugins', plugin_type, idx],
+                                       is_module=False)
+
+    def lint_objects(self, version_str: str, objects_dict: dict):
+        """
+        Lint a object dictionary.
+
+        :arg version_str: To which release the object dictionary belongs
+        :arg objects_dict: The object dictionary
+        """
+        for object_type, objects in objects_dict.items():
+            if self.verify_type(object_type, (str, ), ['releases', version_str, 'objects']):
+                if object_type not in OBJECT_TYPES:
+                    self.errors.append((
+                        self.path, 0, 0,
+                        'Unknown object type {0!r} in {1}'.format(
+                            object_type, self._format_yaml_path(
+                                ['releases', version_str, 'objects']))))
+            if self.verify_type(objects, (list, ),
+                                ['releases', version_str, 'objects', object_type]):
+                for idx, ansible_object in enumerate(objects):
+                    self.verify_plugin(ansible_object,
+                                       ['releases', version_str, 'objects', object_type, idx],
                                        is_module=False)
 
     def lint_changes(self, fragment_linter: ChangelogFragmentLinter,
                      version_str: str, changes: dict):
         """
         Lint changes for an entry of the releases list.
 
@@ -187,26 +211,33 @@
             self.lint_changes(fragment_linter, version_str, cast(dict, changes))
 
         modules = entry.get('modules')
         if self.verify_type(modules, (list, ),
                             ['releases', version_str, 'modules'],
                             allow_none=True) and modules:
             modules = cast(list, modules)
-            for idx, plugin in enumerate(modules):
-                self.verify_plugin(plugin,
+            for idx, module in enumerate(modules):
+                self.verify_plugin(module,
                                    ['releases', version_str, 'modules', idx],
                                    is_module=True)
 
         plugins = entry.get('plugins')
         if self.verify_type(plugins, (dict, ),
                             ['releases', version_str, 'plugins'],
                             allow_none=True) and plugins:
             plugins = cast(dict, plugins)
             self.lint_plugins(version_str, plugins)
 
+        objects = entry.get('objects')
+        if self.verify_type(objects, (dict, ),
+                            ['releases', version_str, 'objects'],
+                            allow_none=True) and objects:
+            objects = cast(dict, objects)
+            self.lint_objects(version_str, objects)
+
         fragments = entry.get('fragments')
         if self.verify_type(fragments, (list, ),
                             ['releases', version_str, 'fragments'],
                             allow_none=True) and fragments:
             fragments = cast(list, fragments)
             for idx, fragment in enumerate(fragments):
                 self.verify_type(fragment, (str, ),
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/logger.py` & `antsibull-changelog-0.9.0/antsibull_changelog/logger.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/plugins.py` & `antsibull-changelog-0.9.0/antsibull_changelog/plugins.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/rst.py` & `antsibull-changelog-0.9.0/antsibull_changelog/rst.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/sanitize.py` & `antsibull-changelog-0.9.0/antsibull_changelog/sanitize.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # License: GPLv3+
 # Copyright: Ansible Project, 2020
 
 """
 Sanitizing changelog.yaml files
 """
 
-import collections
+import collections.abc
 import re
 
 from typing import Any, Dict, List, Mapping, Optional, Union
 
 import packaging.version
 import semantic_version
 
-from .ansible import get_documentable_plugins
+from .ansible import get_documentable_plugins, OBJECT_TYPES, OTHER_PLUGIN_TYPES
 from .config import ChangelogConfig
 
 
 ISO_DATE_REGEX = re.compile('^[0-9]{4}-(?:0[1-9]|1[0-2])-(?:0[1-9]|[12][0-9]|3[01])$')
 
 
 class Sanitizer:  # pylint: disable=too-few-public-methods
@@ -27,15 +27,16 @@
     Implements changelog.yaml sanitizier.
     """
 
     config: ChangelogConfig
 
     def __init__(self, config: ChangelogConfig):
         self.config = config
-        self.documentable_plugins = get_documentable_plugins()
+        self.plugin_types = set(get_documentable_plugins())
+        self.plugin_types.update(OTHER_PLUGIN_TYPES)
 
     def _is_version(self, version: Any, allow_none: bool = False) -> bool:
         try:
             if version is None and allow_none:
                 return True
             if not isinstance(version, str):
                 return False
@@ -102,15 +103,25 @@
                     'namespace': namespace,
                 })
         return result
 
     def _sanitize_plugins(self, data: Mapping) -> Dict[str, List]:
         result = {}
         for key, value in data.items():
-            if key not in self.documentable_plugins or not isinstance(value, list):
+            if key not in self.plugin_types or not isinstance(value, list):
+                continue
+            sanitized_value = self._sanitize_modules(value, are_modules=False)
+            if sanitized_value:
+                result[key] = sanitized_value
+        return result
+
+    def _sanitize_objects(self, data: Mapping) -> Dict[str, List]:
+        result = {}
+        for key, value in data.items():
+            if key not in OBJECT_TYPES or not isinstance(value, list):
                 continue
             sanitized_value = self._sanitize_modules(value, are_modules=False)
             if sanitized_value:
                 result[key] = sanitized_value
         return result
 
     @staticmethod
@@ -130,14 +141,20 @@
 
         plugins = release.get('plugins')
         if isinstance(plugins, collections.abc.Mapping):
             sanitized_plugins = self._sanitize_plugins(plugins)
             if sanitized_plugins:
                 result['plugins'] = sanitized_plugins
 
+        objects = release.get('objects')
+        if isinstance(objects, collections.abc.Mapping):
+            sanitized_objects = self._sanitize_objects(objects)
+            if sanitized_objects:
+                result['objects'] = sanitized_objects
+
     def _sanitize_release(self, release: Mapping) -> Dict[str, Any]:
         result: Dict[str, Any] = {}
 
         release_date = self._sanitize_date(release.get('release_date'))
         if release_date is not None:
             result['release_date'] = release_date
```

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/utils.py` & `antsibull-changelog-0.9.0/antsibull_changelog/utils.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/antsibull_changelog/yaml.py` & `antsibull-changelog-0.9.0/antsibull_changelog/yaml.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/pyproject.toml` & `antsibull-changelog-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "antsibull-changelog"
-version = "0.8.1"
+version = "0.9.0"
 description = "Changelog tool for Ansible-base and Ansible collections"
 authors = ["Felix Fontein <felix@fontein.de>", "Toshio Kuratomi <a.badger@gmail.com>", "Matt Clay <matt@mystile.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ansible-community/antsibull-changelog"
 documentation = "https://github.com/ansible-community/antsibull-changelog/tree/main/docs/"
 packages = [
@@ -32,15 +32,15 @@
 PyYAML = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = "*"
 flake8 = "*"
 codecov = "*"
-pyre-check = "*"
+pyre-check = "^0.0.56"
 pylint = "*"
 mypy = "*"
 mock = "*"
 
 [tool.isort]
 line_length = 100
 multi_line_output = 0
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/ansible-base-1.yaml` & `antsibull-changelog-0.9.0/tests/functional/bad/ansible-base-1.yaml`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/ansible-base-1.yaml-sanitized` & `antsibull-changelog-0.9.0/tests/functional/bad/ansible-base-1.yaml-sanitized`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/felixfontein.hosttech_dns-1.yaml` & `antsibull-changelog-0.9.0/tests/functional/bad/felixfontein.hosttech_dns-1.yaml`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/felixfontein.hosttech_dns-1.yaml-sanitized` & `antsibull-changelog-0.9.0/tests/functional/bad/felixfontein.hosttech_dns-1.yaml-sanitized`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/random-1.json` & `antsibull-changelog-0.9.0/tests/functional/bad/random-1.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'errors'": '{13: {insert: [(2, "\'releases\' -> \'1.0.0\' -> \'plugins\' -> \'lookup\' -> 0 -> '*

 * *             '\'description\' is expected to be <class \'str\'>, but got 123")], delete: [2]}, 14: '*

 * *             '{insert: [(2, "\'releases\' -> \'1.0.0\' -> \'plugins\' -> \'lookup\' -> 0 -> '*

 * *             '\'namespace\' must be null")], delete: [2]}}'}*

```diff
@@ -64,20 +64,20 @@
             0,
             0,
             "'releases' -> '1.0.0' -> 'modules' -> 5 -> 'namespace' is expected to be <class 'str'>, but got None"
         ],
         [
             0,
             0,
-            "'releases' -> '1.0.0' -> 'modules' -> 'lookup' -> 0 -> 'description' is expected to be <class 'str'>, but got 123"
+            "'releases' -> '1.0.0' -> 'plugins' -> 'lookup' -> 0 -> 'description' is expected to be <class 'str'>, but got 123"
         ],
         [
             0,
             0,
-            "'releases' -> '1.0.0' -> 'modules' -> 'lookup' -> 0 -> 'namespace' must be null"
+            "'releases' -> '1.0.0' -> 'plugins' -> 'lookup' -> 0 -> 'namespace' must be null"
         ],
         [
             0,
             0,
             "Unknown plugin type 'woo' in 'releases' -> '1.0.0' -> 'plugins'"
         ],
         [
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/random-1.yaml` & `antsibull-changelog-0.9.0/tests/functional/bad/random-1.yaml`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/bad/random-4.json` & `antsibull-changelog-0.9.0/tests/functional/bad/random-4.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'errors'": '{4: {insert: [(2, "\'releases\' -> \'1.0.0\' -> \'plugins\' -> \'callback\' -> 1 -> '*

 * *             '\'name\' is expected to be <class \'str\'>, but got 123")], delete: [2]}, 5: '*

 * *             '{insert: [(2, "\'releases\' -> \'1.0.0\' -> \'plugins\' -> \'callback\' -> 1 -> '*

 * *             '\'description\' is expected to be <class \'str\'>, but got 234")], delete: [2]}, 6: '*

 * *             '{insert: [(2, "\'releases\' -> \'1.0.0\' -> \'plugins\' -> \'callback\' -> 1 -> '*

 * *             '\'namespace\' […]*

```diff
@@ -9,26 +9,36 @@
             0,
             0,
             "'releases' -> '1.0.0' -> 'plugins' is expected to be <class 'str'>, but got 23"
         ],
         [
             0,
             0,
-            "'releases' -> '1.0.0' -> 'modules' -> 'callback' -> 0 is expected to be <class 'dict'>, but got 42"
+            "Unknown plugin type 'foo' in 'releases' -> '1.0.0' -> 'plugins'"
         ],
         [
             0,
             0,
-            "'releases' -> '1.0.0' -> 'modules' -> 'callback' -> 1 -> 'name' is expected to be <class 'str'>, but got 123"
+            "'releases' -> '1.0.0' -> 'plugins' -> 'callback' -> 0 is expected to be <class 'dict'>, but got 42"
         ],
         [
             0,
             0,
-            "'releases' -> '1.0.0' -> 'modules' -> 'callback' -> 1 -> 'description' is expected to be <class 'str'>, but got 234"
+            "'releases' -> '1.0.0' -> 'plugins' -> 'callback' -> 1 -> 'name' is expected to be <class 'str'>, but got 123"
         ],
         [
             0,
             0,
-            "'releases' -> '1.0.0' -> 'modules' -> 'callback' -> 1 -> 'namespace' must be null"
+            "'releases' -> '1.0.0' -> 'plugins' -> 'callback' -> 1 -> 'description' is expected to be <class 'str'>, but got 234"
+        ],
+        [
+            0,
+            0,
+            "'releases' -> '1.0.0' -> 'plugins' -> 'callback' -> 1 -> 'namespace' must be null"
+        ],
+        [
+            0,
+            0,
+            "Unknown object type 'chair' in 'releases' -> '1.0.0' -> 'objects'"
         ]
     ]
 }
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/fixtures.py` & `antsibull-changelog-0.9.0/tests/functional/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import difflib
 import io
 import os
 import pathlib
 import textwrap
 
 from contextlib import redirect_stderr, redirect_stdout
-from typing import Any, Dict, List, Optional, Set, Tuple, Union
+from typing import Any, Dict, List, Mapping, Optional, Set, Tuple, Union
 
 import pytest
 import yaml
 
 from antsibull_changelog.cli import run as run_changelog_tool
 from antsibull_changelog.config import ChangelogConfig, CollectionDetails, PathsConfig
 
@@ -184,21 +184,25 @@
         if fragment_dir is None:
             fragment_dir = os.path.join(self.paths.changelog_dir, self.config.notes_dir)
         else:
             fragment_dir = os.path.join(self.paths.base_dir, fragment_dir)
         self.mkdir(fragment_dir)
         self._write(os.path.join(fragment_dir, fragment_name), content.encode('utf-8'))
 
-    def add_fragment_line(self, fragment_name: str, section: str, lines: Union[List[str], str],
-                          fragment_dir: Optional[str] = None):
+    def add_fragment_generic(self, fragment_name: str, sections: Mapping[str, Mapping[str, Any]],
+                             fragment_dir: Optional[str] = None):
         self.add_fragment(
             fragment_name,
-            yaml.dump({section: lines}, Dumper=yaml.SafeDumper),
+            yaml.dump(sections, Dumper=yaml.SafeDumper),
             fragment_dir=fragment_dir)
 
+    def add_fragment_line(self, fragment_name: str, section: str, lines: Union[List[str], str],
+                          fragment_dir: Optional[str] = None):
+        self.add_fragment_generic(fragment_name, {section: lines}, fragment_dir=fragment_dir)
+
     def _plugin_base(self, plugin_type):
         if plugin_type == 'module':
             return ['plugins', 'modules']
         return ['plugins', plugin_type]
 
     def add_plugin(self, plugin_type: str, name: str, content: str, subdirs: List[str] = None):
         plugin_dir = os.path.join(
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/good/community.crypto-1.yaml` & `antsibull-changelog-0.9.0/tests/functional/good/community.crypto-1.yaml`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/good/felixfontein.versioning_test_collection-1.yaml` & `antsibull-changelog-0.9.0/tests/functional/good/felixfontein.versioning_test_collection-1.yaml`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/good/felixfontein.versioning_test_collection-2.yaml` & `antsibull-changelog-0.9.0/tests/functional/good/felixfontein.versioning_test_collection-2.yaml`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/good/felixfontein.versioning_test_collection-3.yaml` & `antsibull-changelog-0.9.0/tests/functional/good/felixfontein.versioning_test_collection-3.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -29,10 +29,15 @@
         name: bob
         namespace: null
     release_date: '2020-04-30'
   2.1.0-beta-2:
     changes:
       bugfixes:
       - bob lookup - forgot to check whether ``Bob`` was already there.
+    objects:
+      playbook:
+      - description: Bob is wiping windows
+        name: wipe
+        namespace: null
     fragments:
     - bob-exists.yml
     release_date: '2020-05-01'
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/test_changelog_archive.py` & `antsibull-changelog-0.9.0/tests/functional/test_changelog_archive.py`

 * *Files 9% similar despite different names*

```diff
@@ -163,14 +163,117 @@
 - test - has a new option ``foo``.
 ''')
 
     # Refresh should be ignored
     assert collection_changelog.run_tool('generate', ['-v', '--refresh-fragments']) == 0
     assert collection_changelog.diff().unchanged
 
+    # Add fragment with same filename, but different content
+    collection_changelog.add_fragment_line(
+        'baz-new-option.yaml', 'minor_changes',
+        ['baz - do something crazy.'])
+    collection_changelog.set_plugin_cache('1.1.0', {})
+
+    # Release
+    assert collection_changelog.run_tool('release', ['-v', '--version', '1.1.0', '--date', '2020-01-02']) == 0
+
+    diff = collection_changelog.diff()
+    assert diff.added_dirs == []
+    assert diff.added_files == []
+    assert diff.removed_dirs == []
+    assert diff.removed_files == [
+        'changelogs/fragments/baz-new-option.yaml',
+    ]
+    assert diff.changed_files == ['CHANGELOG.rst', 'changelogs/changelog.yaml']
+
+    assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
+        r'''=========================
+Ansible 1.1 Release Notes
+=========================
+
+.. contents:: Topics
+
+
+v1.1.0
+======
+
+Minor Changes
+-------------
+
+- baz - do something crazy.
+
+v1.0.0
+======
+
+Release Summary
+---------------
+
+This is the first proper release.
+
+Minor Changes
+-------------
+
+- baz lookup - no longer ignores the ``bar`` option.
+- test - has a new option ``foo``.
+''')
+
+    # Set prevent_known_fragments to True
+    collection_changelog.config.prevent_known_fragments = True
+    collection_changelog.set_config(collection_changelog.config)
+
+    # Add fragment with same filename, but different content
+    collection_changelog.add_fragment_line(
+        'baz-new-option.yaml', 'minor_changes',
+        ['baz - do something even more crazy.'])
+    collection_changelog.set_plugin_cache('1.2.0', {})
+
+    # Release
+    assert collection_changelog.run_tool('release', ['-v', '--version', '1.2.0', '--date', '2020-01-02']) == 0
+
+    diff = collection_changelog.diff()
+    assert diff.added_dirs == []
+    assert diff.added_files == []
+    assert diff.removed_dirs == []
+    assert diff.removed_files == []
+    assert diff.changed_files == ['CHANGELOG.rst', 'changelogs/changelog.yaml']
+
+    assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
+        r'''=========================
+Ansible 1.2 Release Notes
+=========================
+
+.. contents:: Topics
+
+
+v1.2.0
+======
+
+v1.1.0
+======
+
+Minor Changes
+-------------
+
+- baz - do something crazy.
+
+v1.0.0
+======
+
+Release Summary
+---------------
+
+This is the first proper release.
+
+Minor Changes
+-------------
+
+- baz lookup - no longer ignores the ``bar`` option.
+- test - has a new option ``foo``.
+''')
+
 
 def test_changelog_release_archive_fragments(  # pylint: disable=redefined-outer-name
         collection_changelog):  # noqa: F811
     collection_changelog.set_galaxy({
         'version': '1.0.0',
     })
     collection_changelog.config.changelog_filename_version_depth = 2
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_ansible.py` & `antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_ansible.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_ansible_classic.py` & `antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_ansible_classic.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/test_changelog_basic_collection.py` & `antsibull-changelog-0.9.0/tests/functional/test_changelog_basic_collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     assert changelog['releases']['1.0.0']['release_date'] == '2020-01-02'
     assert changelog['releases']['1.0.0']['changes'] == {
         'release_summary': 'This is the first proper release.'
     }
     assert changelog['releases']['1.0.0']['fragments'] == ['1.0.0.yml', 'trivial.yml']
     assert 'modules' not in changelog['releases']['1.0.0']
     assert 'plugins' not in changelog['releases']['1.0.0']
+    assert 'objects' not in changelog['releases']['1.0.0']
     assert 'codename' not in changelog['releases']['1.0.0']
 
     assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
         r'''=====================
 Ansible Release Notes
 =====================
 
@@ -91,14 +92,46 @@
 
 This is the first proper release.
 ''')
 
     assert collection_changelog.run_tool('generate', ['-v', '--refresh']) == 0
     assert collection_changelog.diff().unchanged
 
+    assert collection_changelog.run_tool('release', ['-v', '--codename', 'primetime', '--date', '2020-01-03']) == 0
+    assert collection_changelog.diff().unchanged
+
+    assert collection_changelog.run_tool('release', ['-v', '--codename', 'primetime', '--date', '2020-01-03', '--update-existing']) == 0
+    diff = collection_changelog.diff()
+    assert diff.added_dirs == []
+    assert diff.added_files == []
+    assert diff.removed_dirs == []
+    assert diff.removed_files == []
+    assert diff.changed_files == ['CHANGELOG.rst', 'changelogs/changelog.yaml']
+
+    changelog = diff.parse_yaml('changelogs/changelog.yaml')
+    assert changelog['releases']['1.0.0']['release_date'] == '2020-01-03'
+    assert changelog['releases']['1.0.0']['codename'] == 'primetime'
+
+    assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
+        r'''=================================
+Ansible "primetime" Release Notes
+=================================
+
+.. contents:: Topics
+
+
+v1.0.0
+======
+
+Release Summary
+---------------
+
+This is the first proper release.
+''')
+
     # Version 1.1.0
 
     collection_changelog.set_galaxy({
         'version': '1.1.0',
     })
     collection_changelog.set_plugin_cache('1.1.0', {})
 
@@ -115,14 +148,15 @@
     assert changelog['ancestor'] is None
     assert list(changelog['releases']) == ['1.0.0', '1.1.0']
     assert changelog['releases']['1.1.0']['release_date'] == '2020-02-29'
     assert 'changes' not in changelog['releases']['1.1.0']
     assert 'fragments' not in changelog['releases']['1.1.0']
     assert 'modules' not in changelog['releases']['1.1.0']
     assert 'plugins' not in changelog['releases']['1.1.0']
+    assert 'objects' not in changelog['releases']['1.1.0']
     assert 'codename' not in changelog['releases']['1.1.0']
 
     assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
         r'''=====================
 Ansible Release Notes
 =====================
 
@@ -467,14 +501,15 @@
         {
             'name': 'test_new',
             'description': 'This is ANOTHER test module',
             'namespace': '',
         },
     ]
     assert 'plugins' not in changelog['releases']['1.1.0-beta-1']
+    assert 'objects' not in changelog['releases']['1.1.0-beta-1']
     assert 'codename' not in changelog['releases']['1.1.0-beta-1']
 
     assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
         r'''=========================
 Ansible 1.1 Release Notes
 =========================
 
@@ -580,14 +615,19 @@
     collection_changelog.add_fragment_line(
         '1.1.0.yml', 'release_summary', 'Final release of 1.1.0.')
     collection_changelog.add_fragment_line(
         'minorchange.yml', 'minor_changes', ['A minor change.'])
     collection_changelog.add_fragment_line(
         'bugfix.yml', 'bugfixes', ['A bugfix.'])
 
+    # Lint fragments
+    assert collection_changelog.run_tool('lint', [
+        '-vvv',
+    ]) == 0
+
     # Final release 1.1.0
     assert collection_changelog.run_tool('release', [
         '-vvv',
         '--date', '2020-02-29',
         '--version', '1.1.0',
     ]) == 0
 
@@ -625,14 +665,15 @@
         {
             'name': 'test_new3',
             'description': 'This is yet another test module.',
             'namespace': '',
         },
     ]
     assert 'plugins' not in changelog['releases']['1.1.0']
+    assert 'objects' not in changelog['releases']['1.1.0']
     assert 'codename' not in changelog['releases']['1.1.0']
 
     assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
         r'''=========================
 Ansible 1.1 Release Notes
 =========================
 
@@ -698,14 +739,313 @@
         '-vvv',
         '--date', '2020-03-01',
         '--version', '1.1.0',
     ]) == 0
 
     assert collection_changelog.diff().unchanged
 
+    # Update plugin descriptions for 1.2.0
+    collection_changelog.set_plugin_cache('1.2.0', {
+        'module': {
+            'test': {
+                'name': 'test',
+                'description': 'This is a TEST module',
+                'namespace': '',
+                'version_added': '1.0.0',
+            },
+            'test_new': {
+                'name': 'test_new',
+                'description': 'This is ANOTHER test module',
+                'namespace': '',
+                'version_added': '1.1.0',
+            },
+            'test_new2': {
+                'name': 'test_new2',
+                'description': 'This is ANOTHER test module!!!11',
+                'namespace': '',
+                'version_added': '1.1.0',
+            },
+            'test_new3': {
+                'name': 'test_new3',
+                'description': 'This is yet another test module.',
+                'namespace': '',
+                'version_added': '1.1.0',
+            },
+            'test_new4': {
+                'name': 'test_new4',
+                'description': 'This is yet another test module!',
+                'namespace': '',
+                'version_added': '1.2.0',
+            },
+        },
+        'lookup': {
+            'bar': {
+                'name': 'bar',
+                'description': 'A foo_bar lookup',
+                'namespace': None,
+                'version_added': '1.0.0',
+            },
+            'baz': {
+                'name': 'baz',
+                'description': 'Has already been here before',
+                'namespace': None,
+                'version_added': None,
+            },
+            'boom': {
+                'name': 'boom',
+                'description': 'Something older',
+                'namespace': None,
+                'version_added': '0.5.0',
+            },
+        },
+    })
+
+    collection_changelog.add_fragment_line(
+        '1.2.0.yml', 'release_summary', 'Release of 1.2.0.')
+    collection_changelog.add_fragment_generic(
+        'new-plugins.yml', {
+            'add plugin.filter': [
+                {
+                    'name': 'to_time_unit',
+                    'description': 'Converts a time expression to a given unit',
+                },
+                {
+                    'name': 'to_seconds',
+                    'description': 'Converts a time expression to seconds',
+                },
+            ],
+            'add object.role': [
+                {
+                    'name': 'nginx',
+                    'description': 'The most awesome nginx installation role ever',
+                },
+            ],
+            'add object.playbook': [
+                {
+                    'name': 'wipe_server',
+                    'description': 'Totally wipes a server',
+                },
+            ],
+        })
+    collection_changelog.add_fragment_generic(
+        'new-test-plugin.yml', {
+            'add plugin.test': [
+                {
+                    'name': 'similar',
+                    'description': 'Tests whether two objects are similar',
+                },
+            ],
+        })
+    collection_changelog.add_fragment_generic(
+        'new-module.yml', {
+            'add plugin.module': [
+                {
+                    'name': 'meh',
+                    'description': 'A meh module',
+                    'namespace': 'foo'
+                },
+            ],
+        })
+
+    # Release 1.2.0
+    assert collection_changelog.run_tool('release', [
+        '-vvv',
+        '--date', '2020-03-01',
+        '--version', '1.2.0',
+    ]) == 0
+
+    diff = collection_changelog.diff()
+    assert diff.added_dirs == []
+    assert diff.added_files == []
+    assert diff.removed_dirs == []
+    assert diff.removed_files == [
+        'changelogs/fragments/1.2.0.yml',
+        'changelogs/fragments/new-module.yml',
+        'changelogs/fragments/new-plugins.yml',
+        'changelogs/fragments/new-test-plugin.yml',
+    ]
+    assert diff.changed_files == ['CHANGELOG.rst', 'changelogs/changelog.yaml']
+
+    changelog = diff.parse_yaml('changelogs/changelog.yaml')
+    assert changelog['ancestor'] is None
+    assert list(changelog['releases']) == ['1.0.0', '1.1.0', '1.1.0-beta-1', '1.2.0']
+    assert changelog['releases']['1.2.0']['release_date'] == '2020-03-01'
+    assert changelog['releases']['1.2.0']['changes'] == {
+        'release_summary': 'Release of 1.2.0.',
+    }
+    assert changelog['releases']['1.2.0']['fragments'] == [
+        '1.2.0.yml',
+        'new-module.yml',
+        'new-plugins.yml',
+        'new-test-plugin.yml',
+    ]
+    assert changelog['releases']['1.2.0']['modules'] == [
+        {
+            'name': 'meh',
+            'description': 'A meh module',
+            'namespace': 'foo',
+        },
+        {
+            'name': 'test_new4',
+            'description': 'This is yet another test module!',
+            'namespace': '',
+        },
+    ]
+    assert changelog['releases']['1.2.0']['plugins'] == {
+        'filter': [
+            {
+                'name': 'to_seconds',
+                'description': 'Converts a time expression to seconds',
+                'namespace': None,
+            },
+            {
+                'name': 'to_time_unit',
+                'description': 'Converts a time expression to a given unit',
+                'namespace': None,
+            },
+        ],
+        'test': [
+            {
+                'name': 'similar',
+                'description': 'Tests whether two objects are similar',
+                'namespace': None,
+            },
+        ],
+    }
+    assert changelog['releases']['1.2.0']['objects'] == {
+        'playbook': [
+            {
+                'name': 'wipe_server',
+                'description': 'Totally wipes a server',
+                'namespace': None,
+            },
+        ],
+        'role': [
+            {
+                'name': 'nginx',
+                'description': 'The most awesome nginx installation role ever',
+                'namespace': None,
+            },
+        ],
+    }
+    assert 'codename' not in changelog['releases']['1.2.0']
+
+    assert diff.file_contents['CHANGELOG.rst'].decode('utf-8') == (
+        r'''=========================
+Ansible 1.2 Release Notes
+=========================
+
+.. contents:: Topics
+
+
+v1.2.0
+======
+
+Release Summary
+---------------
+
+Release of 1.2.0.
+
+New Plugins
+-----------
+
+Filter
+~~~~~~
+
+- acme.test.to_seconds - Converts a time expression to seconds
+- acme.test.to_time_unit - Converts a time expression to a given unit
+
+Test
+~~~~
+
+- acme.test.similar - Tests whether two objects are similar
+
+New Modules
+-----------
+
+- acme.test.test_new4 - This is yet another test module!
+
+Foo
+~~~
+
+- acme.test.foo.meh - A meh module
+
+New Playbooks
+-------------
+
+- acme.test.wipe_server - Totally wipes a server
+
+New Roles
+---------
+
+- acme.test.nginx - The most awesome nginx installation role ever
+
+v1.1.0
+======
+
+Release Summary
+---------------
+
+Final release of 1.1.0.
+
+Minor Changes
+-------------
+
+- A minor change.
+- Another new fragment.
+
+Bugfixes
+--------
+
+- A bugfix.
+
+New Modules
+-----------
+
+- acme.test.test_new - This is ANOTHER test module
+- acme.test.test_new2 - This is ANOTHER test module!!!11
+- acme.test.test_new3 - This is yet another test module.
+
+v1.0.0
+======
+
+Release Summary
+---------------
+
+This is the first proper release.
+
+Minor Changes
+-------------
+
+- baz lookup - no longer ignores the ``bar`` option.
+- test - has a new option ``foo``.
+
+New Plugins
+-----------
+
+Lookup
+~~~~~~
+
+- acme.test.bar - A foo_bar lookup
+
+New Modules
+-----------
+
+- acme.test.test - This is a TEST module
+''')
+
+    # Release 1.2.0 - should not change
+    assert collection_changelog.run_tool('release', [
+        '-vvv',
+        '--date', '2020-03-02',
+        '--version', '1.2.0',
+    ]) == 0
+
+    assert collection_changelog.diff().unchanged
+
 
 def test_changelog_release_simple_no_galaxy(  # pylint: disable=redefined-outer-name
         collection_changelog):  # noqa: F811
     collection_changelog.config.title = 'Test Collection'
     collection_changelog.config.use_fqcn = False
     collection_changelog.set_config(collection_changelog.config)
     collection_changelog.add_fragment_line(
```

### Comparing `antsibull-changelog-0.8.1/tests/functional/test_changelog_yaml_linter.py` & `antsibull-changelog-0.9.0/tests/functional/test_changelog_yaml_linter.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/functional/test_changelog_yaml_sanitizer.py` & `antsibull-changelog-0.9.0/tests/functional/test_changelog_yaml_sanitizer.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/units/test_changes.py` & `antsibull-changelog-0.9.0/tests/units/test_changes.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/units/test_config.py` & `antsibull-changelog-0.9.0/tests/units/test_config.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/units/test_fragment.py` & `antsibull-changelog-0.9.0/tests/units/test_fragment.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/tests/units/test_utils.py` & `antsibull-changelog-0.9.0/tests/units/test_utils.py`

 * *Files identical despite different names*

### Comparing `antsibull-changelog-0.8.1/setup.py` & `antsibull-changelog-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['PyYAML', 'docutils', 'packaging', 'rstcheck>=3,<4', 'semantic_version']
 
 entry_points = \
 {'console_scripts': ['antsibull-changelog = antsibull_changelog.cli:main']}
 
 setup_kwargs = {
     'name': 'antsibull-changelog',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'Changelog tool for Ansible-base and Ansible collections',
-    'long_description': "# antsibull-changelog -- Ansible Changelog Tool\n\nA changelog generator used by Ansible and Ansible collections.\n\n- Using the\n  [`antsibull-changelog` CLI tool](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelogs.rst).\n- Documentation on the [`changelogs/config.yaml` configuration file for `antsibull-changelog`](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelog-configuration.rst).\n- Documentation on the\n  [`changelog.yaml` format](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelog.yaml-format.md).\n\n## Installation\n\nIt can be installed with pip:\n\n    pip install antsibull-changelog\n\nFor more information, see the\n[documentation](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelogs.rst).\n\n## Using directly from git clone\n\nScripts are created by poetry at build time.  So if you want to run from\na checkout, you'll have to run them under poetry:\n\n    python3 -m pip install poetry\n    poetry install  # Installs dependencies into a virtualenv\n    poetry run antsibull-changelog --help\n\nIf you want to create a new release:\n\n    poetry build\n    poetry publish  # Uploads to pypi.  Be sure you really want to do this\n\nNote: When installing a package published by poetry, it is best to use pip >= 19.0.\nInstalling with pip-18.1 and below could create scripts which use pkg_resources\nwhich can slow down startup time (in some environments by quite a large amount).\n\nIf you prefer to work with `pip install -e`, you can use [dephell](https://pypi.org/project/dephell/)\nto create a `setup.py` file from `pyproject.toml`:\n\n    dephell deps convert --from-path pyproject.toml --from-format poetry --to-path setup.py --to-format setuppy\n\nThen you can install antsibull-changelog with `pip install -e .`.\n\n\n## License\n\nUnless otherwise noted in the code, it is licensed under the terms of the GNU\nGeneral Public License v3 or, at your option, later. See\n[LICENSE](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSE)\nfor a copy of the license.\n",
+    'long_description': "# antsibull-changelog -- Ansible Changelog Tool\n[![Python linting badge](https://github.com/ansible-community/antsibull-changelog/workflows/Python%20linting/badge.svg?event=push)](https://github.com/ansible-community/antsibull-changelog/actions)\n[![Python testing badge](https://github.com/ansible-community/antsibull-changelog/workflows/Python%20testing/badge.svg?event=push)](https://github.com/ansible-community/antsibull-changelog/actions)\n[![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-changelog)](https://codecov.io/gh/ansible-community/antsibull-changelog)\n\nA changelog generator used by Ansible and Ansible collections.\n\n- Using the\n  [`antsibull-changelog` CLI tool](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelogs.rst).\n- Documentation on the [`changelogs/config.yaml` configuration file for `antsibull-changelog`](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelog-configuration.rst).\n- Documentation on the\n  [`changelog.yaml` format](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelog.yaml-format.md).\n\n## Installation\n\nIt can be installed with pip:\n\n    pip install antsibull-changelog\n\nFor more information, see the\n[documentation](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelogs.rst).\n\n## Using directly from git clone\n\nScripts are created by poetry at build time.  So if you want to run from\na checkout, you'll have to run them under poetry:\n\n    python3 -m pip install poetry\n    poetry install  # Installs dependencies into a virtualenv\n    poetry run antsibull-changelog --help\n\nIf you want to create a new release:\n\n    poetry build\n    poetry publish  # Uploads to pypi.  Be sure you really want to do this\n\nNote: When installing a package published by poetry, it is best to use pip >= 19.0.\nInstalling with pip-18.1 and below could create scripts which use pkg_resources\nwhich can slow down startup time (in some environments by quite a large amount).\n\nIf you prefer to work with `pip install -e`, you can use [dephell](https://pypi.org/project/dephell/)\nto create a `setup.py` file from `pyproject.toml`:\n\n    dephell deps convert --from-path pyproject.toml --from-format poetry --to-path setup.py --to-format setuppy\n\nThen you can install antsibull-changelog with `pip install -e .`.\n\n\n## License\n\nUnless otherwise noted in the code, it is licensed under the terms of the GNU\nGeneral Public License v3 or, at your option, later. See\n[LICENSE](https://github.com/ansible-community/antsibull-changelog/tree/main/LICENSE)\nfor a copy of the license.\n",
     'author': 'Felix Fontein',
     'author_email': 'felix@fontein.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ansible-community/antsibull-changelog',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `antsibull-changelog-0.8.1/PKG-INFO` & `antsibull-changelog-0.9.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: antsibull-changelog
-Version: 0.8.1
+Version: 0.9.0
 Summary: Changelog tool for Ansible-base and Ansible collections
 Home-page: https://github.com/ansible-community/antsibull-changelog
 License: GPL-3.0-or-later
 Author: Felix Fontein
 Author-email: felix@fontein.de
 Requires-Python: >=3.6.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML
 Requires-Dist: docutils
 Requires-Dist: packaging
 Requires-Dist: rstcheck (>=3,<4)
 Requires-Dist: semantic_version
 Project-URL: Bug tracker, https://github.com/ansible-community/antsibull-changelog/issues
 Project-URL: Changelog, https://github.com/ansible-community/antsibull-changelog/tree/main/CHANGELOG.rst
 Project-URL: Documentation, https://github.com/ansible-community/antsibull-changelog/tree/main/docs/
 Project-URL: Repository, https://github.com/ansible-community/antsibull-changelog
 Description-Content-Type: text/markdown
 
 # antsibull-changelog -- Ansible Changelog Tool
+[![Python linting badge](https://github.com/ansible-community/antsibull-changelog/workflows/Python%20linting/badge.svg?event=push)](https://github.com/ansible-community/antsibull-changelog/actions)
+[![Python testing badge](https://github.com/ansible-community/antsibull-changelog/workflows/Python%20testing/badge.svg?event=push)](https://github.com/ansible-community/antsibull-changelog/actions)
+[![Codecov badge](https://img.shields.io/codecov/c/github/ansible-community/antsibull-changelog)](https://codecov.io/gh/ansible-community/antsibull-changelog)
 
 A changelog generator used by Ansible and Ansible collections.
 
 - Using the
   [`antsibull-changelog` CLI tool](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelogs.rst).
 - Documentation on the [`changelogs/config.yaml` configuration file for `antsibull-changelog`](https://github.com/ansible-community/antsibull-changelog/tree/main/docs/changelog-configuration.rst).
 - Documentation on the
```

