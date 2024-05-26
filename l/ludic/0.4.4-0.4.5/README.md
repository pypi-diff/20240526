# Comparing `tmp/ludic-0.4.4.tar.gz` & `tmp/ludic-0.4.5.tar.gz`

## Comparing `ludic-0.4.4.tar` & `ludic-0.4.5.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.4/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.4/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.4/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.4/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.4/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.4/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/catalog.md
--rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/getting-started.md
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.4/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/README.md
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/bulk_update.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/click_to_edit.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/click_to_load.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/delete_row.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/edit_row.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/infinite_scroll.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.4/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/__init__.py
--rw-r--r--   0        0        0    16518 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/attrs.py
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/components.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/format.py
--rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/utils.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/forms.py
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/headers.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/items.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/layouts.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/lists.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/loaders.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/messages.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/pages.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/tables.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/typography.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/styles/collect.py
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/styles/themes.py
--rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/styles/types.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/__init__.py
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/parsers.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/responses.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.4/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/test_components.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/test_exceptions.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/test_formatting.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/test_types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/styles/__init__.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/styles/test_styles.py
--rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/styles/test_themes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.4/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.4/LICENCE
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.4/README.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ludic-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.5/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.5/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.5/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.5/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/catalog.md
+-rw-r--r--   0        0        0    11706 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/getting-started.md
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.5/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/README.md
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/click_to_load.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/infinite_scroll.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 ludic-0.4.5/examples/lazy_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/__init__.py
+-rw-r--r--   0        0        0    16518 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/attrs.py
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/components.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/format.py
+-rw-r--r--   0        0        0    12137 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     8599 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/headers.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/icons.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/items.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/messages.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/collect.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/themes.py
+-rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/types.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/__init__.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/responses.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 ludic-0.4.5/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0     6868 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_components.py
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     3715 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.5/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.5/LICENCE
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.5/README.md
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 ludic-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 ludic-0.4.5/PKG-INFO
```

### Comparing `ludic-0.4.4/.pre-commit-config.yaml` & `ludic-0.4.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/CONTRIBUTING.md` & `ludic-0.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/mkdocs.yaml` & `ludic-0.4.5/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/.github/workflows/publish.yaml` & `ludic-0.4.5/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/.github/workflows/test.yaml` & `ludic-0.4.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/catalog.md` & `ludic-0.4.5/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/components.md` & `ludic-0.4.5/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/getting-started.md` & `ludic-0.4.5/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/htmx.md` & `ludic-0.4.5/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/index.md` & `ludic-0.4.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/styles.md` & `ludic-0.4.5/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/web-framework.md` & `ludic-0.4.5/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/docs/assets/ludic.png` & `ludic-0.4.5/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/README.md` & `ludic-0.4.5/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/__init__.py` & `ludic-0.4.5/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/bulk_update.py` & `ludic-0.4.5/examples/bulk_update.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/click_to_edit.py` & `ludic-0.4.5/examples/click_to_edit.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/click_to_load.py` & `ludic-0.4.5/examples/click_to_load.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/delete_row.py` & `ludic-0.4.5/examples/delete_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/edit_row.py` & `ludic-0.4.5/examples/edit_row.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/infinite_scroll.py` & `ludic-0.4.5/examples/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/examples/lazy_loading.py` & `ludic-0.4.5/examples/lazy_loading.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/attrs.py` & `ludic-0.4.5/ludic/attrs.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/base.py` & `ludic-0.4.5/ludic/base.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/components.py` & `ludic-0.4.5/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/format.py` & `ludic-0.4.5/ludic/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,20 @@
 
     Returns:
         dict[str, Any]: The formatted attributes.
     """
     hints = get_element_attrs_annotations(attrs_type, include_extras=True)
 
     def _get_key(key: str) -> str:
-        if get_origin(hints[key]) is Annotated:
+        if key in hints and get_origin(hints[key]) is Annotated:
             args = get_args(hints[key])
             if len(args) > 1 and isinstance(args[1], str):
                 return args[1]
+        elif key.startswith("data_"):
+            return f"data-{key[5:]}"
         return key
 
     result: dict[str, str] = {}
     for key, value in attrs.items():
         if formatted_value := format_attr_value(key, value, is_html=is_html):
             alias = _get_key(key)
             if alias in result:
```

### Comparing `ludic-0.4.4/ludic/html.py` & `ludic-0.4.5/ludic/html.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/types.py` & `ludic-0.4.5/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/utils.py` & `ludic-0.4.5/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/buttons.py` & `ludic-0.4.5/ludic/catalog/buttons.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/forms.py` & `ludic-0.4.5/ludic/catalog/forms.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/headers.py` & `ludic-0.4.5/ludic/catalog/headers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/items.py` & `ludic-0.4.5/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/layouts.py` & `ludic-0.4.5/ludic/catalog/layouts.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/lists.py` & `ludic-0.4.5/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/loaders.py` & `ludic-0.4.5/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/messages.py` & `ludic-0.4.5/ludic/catalog/messages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/navigation.py` & `ludic-0.4.5/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/pages.py` & `ludic-0.4.5/ludic/catalog/pages.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/quotes.py` & `ludic-0.4.5/ludic/catalog/quotes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/tables.py` & `ludic-0.4.5/ludic/catalog/tables.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/typography.py` & `ludic-0.4.5/ludic/catalog/typography.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/catalog/utils.py` & `ludic-0.4.5/ludic/catalog/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/styles/collect.py` & `ludic-0.4.5/ludic/styles/collect.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/styles/themes.py` & `ludic-0.4.5/ludic/styles/themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/styles/types.py` & `ludic-0.4.5/ludic/styles/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/styles/utils.py` & `ludic-0.4.5/ludic/styles/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/app.py` & `ludic-0.4.5/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/datastructures.py` & `ludic-0.4.5/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/endpoints.py` & `ludic-0.4.5/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/exceptions.py` & `ludic-0.4.5/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/parsers.py` & `ludic-0.4.5/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/requests.py` & `ludic-0.4.5/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/responses.py` & `ludic-0.4.5/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/ludic/web/routing.py` & `ludic-0.4.5/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/test_components.py` & `ludic-0.4.5/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/test_elements.py` & `ludic-0.4.5/tests/test_elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,7 +158,14 @@
     assert str(dom) == (
         '<div id="test">\n'
         "  <p>1</p>\n"
         "  <p>2</p>\n"
         "  <p>3</p>\n"
         "</div>"
     )  # fmt: skip
+
+
+def test_data_attributes() -> None:
+    dom = div("content", data_foo="1", data_bar="test")
+
+    assert dom.attrs == {"data_foo": "1", "data_bar": "test"}
+    assert dom.to_html() == '<div data-foo="1" data-bar="test">content</div>'
```

### Comparing `ludic-0.4.4/tests/test_examples.py` & `ludic-0.4.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/test_exceptions.py` & `ludic-0.4.5/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/test_formatting.py` & `ludic-0.4.5/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/test_types.py` & `ludic-0.4.5/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/styles/__init__.py` & `ludic-0.4.5/tests/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/styles/test_styles.py` & `ludic-0.4.5/tests/styles/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/tests/styles/test_themes.py` & `ludic-0.4.5/tests/styles/test_themes.py`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/.gitignore` & `ludic-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/LICENCE` & `ludic-0.4.5/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/README.md` & `ludic-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/pyproject.toml` & `ludic-0.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.4.4/PKG-INFO` & `ludic-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.4.4
+Version: 0.4.5
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

