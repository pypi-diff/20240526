# Comparing `tmp/jpterm-0.2.11.tar.gz` & `tmp/jpterm-0.2.12.tar.gz`

## Comparing `jpterm-0.2.11.tar` & `jpterm-0.2.12.tar`

### file list

```diff
@@ -1,154 +1,153 @@
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jpterm-0.2.11/.gitattributes
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 jpterm-0.2.11/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15529 2020-02-02 00:00:00.000000 jpterm-0.2.11/CHANGELOG.md
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 jpterm-0.2.11/config.yaml
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 jpterm-0.2.11/mkdocs.yml
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jpterm-0.2.11/.github/workflows/test.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/index.md
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/install.md
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/assets/logo.png
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/plugins/console.md
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/plugins/notebook_editor.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/usage/CLI.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jpterm-0.2.11/docs/usage/key_bindings.md
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/button.ipynb
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/demo.md
--rw-r--r--   0        0        0    37737 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/jupyter.png
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/plotext.ipynb
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/plotext2.ipynb
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/switch.ipynb
--rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 jpterm-0.2.11/examples/widget.ipynb
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/jpterm/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 jpterm-0.2.11/jpterm/cli.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/cell/LICENSE.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/cell/README.md
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/cell/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/cell/txl_cell/__init__.py
--rw-r--r--   0        0        0    12472 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/cell/txl_cell/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/console/LICENSE.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/console/README.md
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/console/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/console/txl_console/__init__.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/console/txl_console/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/editors/LICENSE.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/editors/README.md
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/editors/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/editors/txl_editors/__init__.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/editors/txl_editors/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/file_browser/LICENSE.txt
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/file_browser/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/file_browser/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/file_browser/txl_file_browser/__init__.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/file_browser/txl_file_browser/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/image_viewer/LICENSE.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/image_viewer/README.md
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/image_viewer/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/image_viewer/txl_image_viewer/__init__.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/image_viewer/txl_image_viewer/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/LICENSE.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/README.md
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/txl_jpterm/__init__.py
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/txl_jpterm/components.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/txl_jpterm/footer.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/txl_jpterm/header.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/txl_jpterm/jpterm.css
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/jpterm/txl_jpterm/main_area.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/kernel/LICENSE.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/kernel/README.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/kernel/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/kernel/txl_kernel/__init__.py
--rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/kernel/txl_kernel/driver.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/kernel/txl_kernel/message.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/launcher/LICENSE.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/launcher/README.md
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/launcher/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/launcher/txl_launcher/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/launcher/txl_launcher/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_contents/LICENSE.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_contents/README.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_contents/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_contents/txl_local_contents/__init__.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_contents/txl_local_contents/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/LICENSE.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/README.md
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/components.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/connect.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/kernelspec.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/paths.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/LICENSE.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/components.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/terminal.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/win_terminal.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/markdown_viewer/LICENSE.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/markdown_viewer/README.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/markdown_viewer/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/markdown_viewer/txl_markdown_viewer/__init__.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/markdown_viewer/txl_markdown_viewer/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_editor/LICENSE.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_editor/README.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_editor/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_editor/txl_notebook_editor/__init__.py
--rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_editor/txl_notebook_editor/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_viewer/LICENSE.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_viewer/README.md
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_viewer/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_viewer/txl_notebook_viewer/__init__.py
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/notebook_viewer/txl_notebook_viewer/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_contents/LICENSE.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_contents/README.md
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_contents/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_contents/txl_remote_contents/__init__.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_contents/txl_remote_contents/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/LICENSE.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/README.md
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/components.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/driver.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/message.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_terminals/LICENSE.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_terminals/README.md
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_terminals/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_terminals/txl_remote_terminals/__init__.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/remote_terminals/txl_remote_terminals/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/terminal/LICENSE.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/terminal/README.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/terminal/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/terminal/txl_terminal/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/terminal/txl_terminal/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_editor/LICENSE.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_editor/README.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_editor/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_editor/txl_text_editor/__init__.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_editor/txl_text_editor/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_viewer/LICENSE.txt
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_viewer/README.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_viewer/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_viewer/txl_text_viewer/__init__.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/text_viewer/txl_text_viewer/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/widgets/LICENSE.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/widgets/README.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/widgets/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/widgets/txl_widgets/__init__.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jpterm-0.2.11/plugins/widgets/txl_widgets/components.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/LICENSE.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/pyproject.toml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/txl/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/txl/app.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/txl/base.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/txl/cli.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 jpterm-0.2.11/txl/txl/text_input.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 jpterm-0.2.11/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jpterm-0.2.11/LICENSE
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 jpterm-0.2.11/README.md
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 jpterm-0.2.11/pyproject.toml
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jpterm-0.2.11/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 jpterm-0.2.12/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15529 2020-02-02 00:00:00.000000 jpterm-0.2.12/CHANGELOG.md
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 jpterm-0.2.12/config.yaml
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 jpterm-0.2.12/mkdocs.yml
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 jpterm-0.2.12/.github/workflows/test.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/index.md
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/install.md
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/assets/logo.png
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/plugins/console.md
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/plugins/notebook_editor.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/usage/CLI.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 jpterm-0.2.12/docs/usage/key_bindings.md
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/button.ipynb
+-rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/demo.md
+-rw-r--r--   0        0        0    37737 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/jupyter.png
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/plotext.ipynb
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/plotext2.ipynb
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/switch.ipynb
+-rw-r--r--   0        0        0     9256 2020-02-02 00:00:00.000000 jpterm-0.2.12/examples/widget.ipynb
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/jpterm/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 jpterm-0.2.12/jpterm/cli.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/cell/LICENSE.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/cell/README.md
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/cell/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/cell/txl_cell/__init__.py
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/cell/txl_cell/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/console/LICENSE.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/console/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/console/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/console/txl_console/__init__.py
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/console/txl_console/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/editors/LICENSE.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/editors/README.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/editors/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/editors/txl_editors/__init__.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/editors/txl_editors/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/file_browser/LICENSE.txt
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/file_browser/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/file_browser/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/file_browser/txl_file_browser/__init__.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/file_browser/txl_file_browser/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/image_viewer/LICENSE.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/image_viewer/README.md
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/image_viewer/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/image_viewer/txl_image_viewer/__init__.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/image_viewer/txl_image_viewer/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/LICENSE.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/README.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/txl_jpterm/__init__.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/txl_jpterm/components.py
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/txl_jpterm/footer.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/txl_jpterm/header.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/txl_jpterm/jpterm.css
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/jpterm/txl_jpterm/main_area.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/kernel/LICENSE.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/kernel/README.md
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/kernel/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/kernel/txl_kernel/__init__.py
+-rw-r--r--   0        0        0     8216 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/kernel/txl_kernel/driver.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/kernel/txl_kernel/message.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/launcher/LICENSE.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/launcher/README.md
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/launcher/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/launcher/txl_launcher/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/launcher/txl_launcher/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_contents/LICENSE.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_contents/README.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_contents/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_contents/txl_local_contents/__init__.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_contents/txl_local_contents/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/LICENSE.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/README.md
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/components.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/connect.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/kernelspec.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/paths.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/LICENSE.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/components.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/terminal.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/win_terminal.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/markdown_viewer/LICENSE.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/markdown_viewer/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/markdown_viewer/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/markdown_viewer/txl_markdown_viewer/__init__.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/markdown_viewer/txl_markdown_viewer/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_editor/LICENSE.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_editor/README.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_editor/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_editor/txl_notebook_editor/__init__.py
+-rw-r--r--   0        0        0    16203 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_editor/txl_notebook_editor/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_viewer/LICENSE.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_viewer/README.md
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_viewer/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_viewer/txl_notebook_viewer/__init__.py
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/notebook_viewer/txl_notebook_viewer/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_contents/LICENSE.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_contents/README.md
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_contents/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_contents/txl_remote_contents/__init__.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_contents/txl_remote_contents/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/LICENSE.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/README.md
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/components.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/driver.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/message.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_terminals/LICENSE.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_terminals/README.md
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_terminals/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_terminals/txl_remote_terminals/__init__.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/remote_terminals/txl_remote_terminals/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/terminal/LICENSE.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/terminal/README.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/terminal/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/terminal/txl_terminal/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/terminal/txl_terminal/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_editor/LICENSE.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_editor/README.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_editor/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_editor/txl_text_editor/__init__.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_editor/txl_text_editor/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_viewer/LICENSE.txt
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_viewer/README.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_viewer/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_viewer/txl_text_viewer/__init__.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/text_viewer/txl_text_viewer/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/widgets/LICENSE.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/widgets/README.md
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/widgets/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/widgets/txl_widgets/__init__.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jpterm-0.2.12/plugins/widgets/txl_widgets/components.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/LICENSE.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/README.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/pyproject.toml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/txl/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/txl/app.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/txl/base.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/txl/cli.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 jpterm-0.2.12/txl/txl/text_input.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 jpterm-0.2.12/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 jpterm-0.2.12/LICENSE
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 jpterm-0.2.12/README.md
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 jpterm-0.2.12/pyproject.toml
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 jpterm-0.2.12/PKG-INFO
```

### Comparing `jpterm-0.2.11/CHANGELOG.md` & `jpterm-0.2.12/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/mkdocs.yml` & `jpterm-0.2.12/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/.github/workflows/test.yml` & `jpterm-0.2.12/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/docs/assets/logo.png` & `jpterm-0.2.12/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/docs/plugins/notebook_editor.md` & `jpterm-0.2.12/docs/plugins/notebook_editor.md`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/docs/usage/CLI.md` & `jpterm-0.2.12/docs/usage/CLI.md`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/button.ipynb` & `jpterm-0.2.12/examples/button.ipynb`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/demo.md` & `jpterm-0.2.12/examples/demo.md`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/jupyter.png` & `jpterm-0.2.12/examples/jupyter.png`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/plotext.ipynb` & `jpterm-0.2.12/examples/plotext.ipynb`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/plotext2.ipynb` & `jpterm-0.2.12/examples/plotext2.ipynb`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/switch.ipynb` & `jpterm-0.2.12/examples/switch.ipynb`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/examples/widget.ipynb` & `jpterm-0.2.12/examples/widget.ipynb`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/jpterm/cli.py` & `jpterm-0.2.12/jpterm/cli.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/cell/LICENSE.txt` & `jpterm-0.2.12/plugins/cell/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/cell/pyproject.toml` & `jpterm-0.2.12/plugins/cell/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/cell/txl_cell/components.py` & `jpterm-0.2.12/plugins/cell/txl_cell/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 from functools import partial
 from importlib.metadata import entry_points
 
 from asphalt.core import Component, Context
 from pycrdt import Doc, Map, MapEvent, Text
 from rich.text import Text as RichText
+from textual.app import ComposeResult
 from textual.containers import Container
 from textual.widgets import Static
 
 from txl.base import Cell, CellFactory, Contents, Kernel, Widgets
 from txl.text_input import TextInput
 
 YDOCS = {ep.name: ep.load() for ep in entry_points(group="ypywidgets")}
@@ -64,15 +65,15 @@
         self._language = language
         self.kernel = kernel
         self.contents = contents
         self.widgets = widgets
         self.show_execution_count = show_execution_count
         self.show_border = show_border
         self.outputs = []
-        self.update()
+        self.update(mount=False)
         self.ycell.observe_deep(self.on_change)
         self.styles.height = "auto"
         self.cell_change_events = asyncio.Queue()
         self.widget_change_events = asyncio.Queue()
         self.tasks = [
             asyncio.create_task(self.observe_cell_changes()),
             asyncio.create_task(self.observe_widget_changes()),
@@ -170,46 +171,56 @@
                                         self.mount(output_widget)
                                         self.outputs.append(output_widget)
 
     def get_execution_count(self, value):
         execution_count = " " if value is None else str(value).removesuffix(".0")
         return f"[green]In [[#66ff00]{execution_count}[/#66ff00]]:[/green]"
 
-    def update(self):
+    def compose(self) -> ComposeResult:
+        if self.show_execution_count:
+            yield self.execution_count
+        yield self.source
+        for output in self.outputs:
+            yield output
+
+    def update(self, mount: bool = True):
         cell = json.loads(str(self.ycell))
         if self.show_execution_count:
             execution_state = self.ycell.get("execution_state")
             if execution_state != "busy":
                 execution_count = (
                     self.get_execution_count(self.ycell.get("execution_count", ""))
                 )
             else:
                 execution_count = (
                     self.get_execution_count("*")
                 )
             self.execution_count = Static(execution_count)
-            self.mount(self.execution_count)
+            if mount:
+                self.mount(self.execution_count)
         cell_type = cell["cell_type"]
         if cell_type == "markdown":
             language = "markdown"
         elif cell_type == "code":
             language = self.language
         else:
             language = None
         self.source = Source(
             ycell=self.ycell,
             language=language,
             show_border=self.show_border,
         )
-        self.mount(self.source)
+        if mount:
+            self.mount(self.source)
 
         for output in cell.get("outputs", []):
             output_widget = self.get_output_widget(output)
             if output_widget is not None:
-                self.mount(output_widget)
+                if mount:
+                    self.mount(output_widget)
                 self.outputs.append(output_widget)
 
     def get_output_widget(self, output):
         if "guid" in output:
             guid = output["guid"]
             ywidget_doc = Doc()
             room_id = f"ywidget:{guid}"
```

### Comparing `jpterm-0.2.11/plugins/console/LICENSE.txt` & `jpterm-0.2.12/plugins/console/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/console/pyproject.toml` & `jpterm-0.2.12/plugins/console/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/console/txl_console/components.py` & `jpterm-0.2.12/plugins/console/txl_console/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/editors/LICENSE.txt` & `jpterm-0.2.12/plugins/editors/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/editors/pyproject.toml` & `jpterm-0.2.12/plugins/editors/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/editors/txl_editors/components.py` & `jpterm-0.2.12/plugins/editors/txl_editors/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/file_browser/LICENSE.txt` & `jpterm-0.2.12/plugins/file_browser/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/file_browser/pyproject.toml` & `jpterm-0.2.12/plugins/file_browser/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/file_browser/txl_file_browser/components.py` & `jpterm-0.2.12/plugins/file_browser/txl_file_browser/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/image_viewer/LICENSE.txt` & `jpterm-0.2.12/plugins/image_viewer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/image_viewer/pyproject.toml` & `jpterm-0.2.12/plugins/image_viewer/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/image_viewer/txl_image_viewer/components.py` & `jpterm-0.2.12/plugins/image_viewer/txl_image_viewer/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/jpterm/LICENSE.txt` & `jpterm-0.2.12/plugins/jpterm/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/jpterm/pyproject.toml` & `jpterm-0.2.12/plugins/jpterm/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/jpterm/txl_jpterm/components.py` & `jpterm-0.2.12/plugins/jpterm/txl_jpterm/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     def __init__(self, header, footer, main_area, file_browser, editors, launcher, *args, **kwargs):
         self.header = header
         self.footer = footer
         self.main_area = main_area
         self.file_browser = file_browser
         self.editors = editors
         self.launcher = launcher
+        self.main_area.show(self.launcher, "Launcher", mount=False)
         super().__init__(*args, **kwargs)
 
     def watch_show_browser(self, show_browser: bool) -> None:
         self.set_class(show_browser, "-show-browser")
 
     def compose(self) -> ComposeResult:
         yield self.header
-        self.main_area.show(self.launcher, "Launcher")
         yield Container(
             self.file_browser,
             self.main_area,
         )
         yield self.footer
 
     def action_toggle_files(self) -> None:
```

### Comparing `jpterm-0.2.11/plugins/jpterm/txl_jpterm/footer.py` & `jpterm-0.2.12/plugins/jpterm/txl_jpterm/footer.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
             end="",
         )
         highlight_style = self.get_component_rich_style("footer--highlight")
         highlight_key_style = self.get_component_rich_style("footer--highlight-key")
         key_style = self.get_component_rich_style("footer--key")
 
         bindings = [
-            binding
-            for (_namespace, binding) in self.app.namespace_bindings.values()
-            if binding.show
+            active_binding.binding
+            for active_binding in self.app.active_bindings.values()
+            if active_binding.binding.show
         ]
 
         action_to_bindings = defaultdict(list)
         for binding in bindings:
             action_to_bindings[binding.action].append(binding)
 
         for action, bindings in action_to_bindings.items():
```

### Comparing `jpterm-0.2.11/plugins/jpterm/txl_jpterm/main_area.py` & `jpterm-0.2.12/plugins/jpterm/txl_jpterm/main_area.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 
+from textual.app import ComposeResult
 from textual.widget import Widget
 from textual.widgets import Tab, Tabs
 
 from txl.base import MainArea as AbstractMainArea
 
 
 class MainAreaMeta(type(Widget), type(AbstractMainArea)):
@@ -15,33 +16,38 @@
         super().__init__(id="main-view")
         self.mounted = []
         self.shown = None
         self.tabs = None
         self.widget_to_tab = {}
         self.title = 0
 
-    def show(self, widget: Widget, title: Optional[str] = None):
+    def show(self, widget: Widget, title: Optional[str] = None, mount: bool = True):
         if widget not in self.mounted:
             if title is None:
                 title = self.title
                 self.title += 1
             tab = Tab(str(title))
             if self.tabs is None:
                 self.tabs = Tabs(tab)
-                self.mount(self.tabs)
             else:
                 self.tabs.add_tab(tab)
                 self.tabs.active = tab.id
             self.widget_to_tab[widget] = (tab, False)
             self.mounted.append(widget)
-            self.mount(widget)
+            if mount:
+                self.mount(widget)
         else:
             tab, dirty = self.widget_to_tab[widget]
             self.tabs.active = tab.id
 
+    def compose(self) -> ComposeResult:
+        yield self.tabs
+        for widget in self.mounted:
+            yield widget
+
     def get_label(self) -> str:
         tab = self.tabs.active_tab
         return tab.label_text
 
     def set_label(self, title: str) -> None:
         tab = self.tabs.active_tab
         tab.label = title
```

### Comparing `jpterm-0.2.11/plugins/kernel/LICENSE.txt` & `jpterm-0.2.12/plugins/kernel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/kernel/pyproject.toml` & `jpterm-0.2.12/plugins/kernel/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/kernel/txl_kernel/driver.py` & `jpterm-0.2.12/plugins/kernel/txl_kernel/driver.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/kernel/txl_kernel/message.py` & `jpterm-0.2.12/plugins/kernel/txl_kernel/message.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/launcher/LICENSE.txt` & `jpterm-0.2.12/plugins/launcher/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/launcher/pyproject.toml` & `jpterm-0.2.12/plugins/launcher/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/launcher/txl_launcher/components.py` & `jpterm-0.2.12/plugins/launcher/txl_launcher/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_contents/LICENSE.txt` & `jpterm-0.2.12/plugins/local_contents/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_contents/pyproject.toml` & `jpterm-0.2.12/plugins/local_contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_contents/txl_local_contents/components.py` & `jpterm-0.2.12/plugins/local_contents/txl_local_contents/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/LICENSE.txt` & `jpterm-0.2.12/plugins/local_kernels/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/pyproject.toml` & `jpterm-0.2.12/plugins/local_kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/components.py` & `jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/connect.py` & `jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/connect.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/driver.py` & `jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/driver.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/kernelspec.py` & `jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/message.py` & `jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/message.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_kernels/txl_local_kernels/paths.py` & `jpterm-0.2.12/plugins/local_kernels/txl_local_kernels/paths.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_terminals/LICENSE.txt` & `jpterm-0.2.12/plugins/local_terminals/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_terminals/pyproject.toml` & `jpterm-0.2.12/plugins/local_terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/components.py` & `jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/terminal.py` & `jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/terminal.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/local_terminals/txl_local_terminals/win_terminal.py` & `jpterm-0.2.12/plugins/local_terminals/txl_local_terminals/win_terminal.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/markdown_viewer/LICENSE.txt` & `jpterm-0.2.12/plugins/markdown_viewer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/markdown_viewer/pyproject.toml` & `jpterm-0.2.12/plugins/markdown_viewer/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/markdown_viewer/txl_markdown_viewer/components.py` & `jpterm-0.2.12/plugins/markdown_viewer/txl_markdown_viewer/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/notebook_editor/LICENSE.txt` & `jpterm-0.2.12/plugins/notebook_editor/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/notebook_editor/pyproject.toml` & `jpterm-0.2.12/plugins/notebook_editor/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/notebook_editor/txl_notebook_editor/components.py` & `jpterm-0.2.12/plugins/notebook_editor/txl_notebook_editor/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import partial
 from importlib.metadata import entry_points
 from typing import Any
 
 import anyio
 from asphalt.core import Component, Context
 from httpx import AsyncClient
-from textual.app import RenderResult
+from textual.app import ComposeResult, RenderResult
 from textual.containers import VerticalScroll
 from textual.events import Event
 from textual.keys import Keys
 from textual.reactive import Reactive
 from textual.widget import Widget
 from textual.widgets import Select
 
@@ -82,15 +82,17 @@
         self.cells = []
         self.cell_i = 0
         self.cell_copy = None
         self.edit_mode = False
         self.nb_change_target = asyncio.Queue()
         self.nb_change_events = asyncio.Queue()
         self.top_bar = TopBar()
-        self.mount(self.top_bar)
+
+    def compose(self) -> ComposeResult:
+        yield self.top_bar
 
     async def watch_busy(self, event):
         self.top_bar.busy = event.busy
 
     async def on_open(self, event: FileOpenEvent) -> None:
         await self.open(event.path)
```

### Comparing `jpterm-0.2.11/plugins/notebook_viewer/LICENSE.txt` & `jpterm-0.2.12/plugins/notebook_viewer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/notebook_viewer/pyproject.toml` & `jpterm-0.2.12/plugins/notebook_viewer/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/notebook_viewer/txl_notebook_viewer/components.py` & `jpterm-0.2.12/plugins/notebook_viewer/txl_notebook_viewer/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_contents/LICENSE.txt` & `jpterm-0.2.12/plugins/remote_contents/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_contents/pyproject.toml` & `jpterm-0.2.12/plugins/remote_contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_contents/txl_remote_contents/components.py` & `jpterm-0.2.12/plugins/remote_contents/txl_remote_contents/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_kernels/LICENSE.txt` & `jpterm-0.2.12/plugins/remote_kernels/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_kernels/pyproject.toml` & `jpterm-0.2.12/plugins/remote_kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/components.py` & `jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/driver.py` & `jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/driver.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_kernels/txl_remote_kernels/message.py` & `jpterm-0.2.12/plugins/remote_kernels/txl_remote_kernels/message.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_terminals/LICENSE.txt` & `jpterm-0.2.12/plugins/remote_terminals/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_terminals/pyproject.toml` & `jpterm-0.2.12/plugins/remote_terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/remote_terminals/txl_remote_terminals/components.py` & `jpterm-0.2.12/plugins/remote_terminals/txl_remote_terminals/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/terminal/LICENSE.txt` & `jpterm-0.2.12/plugins/terminal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/terminal/pyproject.toml` & `jpterm-0.2.12/plugins/terminal/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/terminal/txl_terminal/components.py` & `jpterm-0.2.12/plugins/terminal/txl_terminal/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/text_editor/LICENSE.txt` & `jpterm-0.2.12/plugins/text_editor/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/text_editor/pyproject.toml` & `jpterm-0.2.12/plugins/text_editor/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/text_editor/txl_text_editor/components.py` & `jpterm-0.2.12/plugins/text_editor/txl_text_editor/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/text_viewer/LICENSE.txt` & `jpterm-0.2.12/plugins/text_viewer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/text_viewer/pyproject.toml` & `jpterm-0.2.12/plugins/text_viewer/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/text_viewer/txl_text_viewer/components.py` & `jpterm-0.2.12/plugins/text_viewer/txl_text_viewer/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/widgets/LICENSE.txt` & `jpterm-0.2.12/plugins/widgets/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/widgets/pyproject.toml` & `jpterm-0.2.12/plugins/widgets/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/plugins/widgets/txl_widgets/components.py` & `jpterm-0.2.12/plugins/widgets/txl_widgets/components.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/txl/LICENSE.txt` & `jpterm-0.2.12/txl/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/txl/pyproject.toml` & `jpterm-0.2.12/txl/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "asphalt >=4.12.0,<5",
-  "textual[syntax] >=0.53.1,<0.54.0",
+  "textual[syntax] >=0.63.4,<0.64.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/davidbrochart/jpterm/txl"
 
 [tool.hatch.version]
```

### Comparing `jpterm-0.2.11/txl/txl/app.py` & `jpterm-0.2.12/txl/txl/app.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/txl/txl/base.py` & `jpterm-0.2.12/txl/txl/base.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/txl/txl/cli.py` & `jpterm-0.2.12/txl/txl/cli.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/txl/txl/text_input.py` & `jpterm-0.2.12/txl/txl/text_input.py`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/LICENSE` & `jpterm-0.2.12/LICENSE`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/README.md` & `jpterm-0.2.12/README.md`

 * *Files identical despite different names*

### Comparing `jpterm-0.2.11/pyproject.toml` & `jpterm-0.2.12/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 ]
 keywords = [
     "jupyter",
     "textual",
 ]
 dependencies = [
     "rich-click >=1.6.0",
-    "txl ==0.2.11",
-    "txl_cell ==0.2.11",
-    "txl_console ==0.2.11",
-    "txl_editors ==0.2.11",
-    "txl_file_browser ==0.2.11",
-    "txl_image_viewer ==0.2.11",
-    "txl_jpterm ==0.2.11",
-    "txl_kernel ==0.2.11",
-    "txl_local_contents ==0.2.11",
-    "txl_local_terminals ==0.2.11",
-    "txl_local_kernels ==0.2.11",
-    "txl_notebook_editor ==0.2.11",
-    "txl_remote_contents ==0.2.11",
-    "txl_remote_terminals ==0.2.11",
-    "txl_remote_kernels ==0.2.11",
-    "txl_text_editor ==0.2.11",
-    "txl_markdown_viewer ==0.2.11",
-    "txl_terminal ==0.2.11",
-    "txl_launcher ==0.2.11",
-    "txl_widgets ==0.2.11",
+    "txl ==0.2.12",
+    "txl_cell ==0.2.12",
+    "txl_console ==0.2.12",
+    "txl_editors ==0.2.12",
+    "txl_file_browser ==0.2.12",
+    "txl_image_viewer ==0.2.12",
+    "txl_jpterm ==0.2.12",
+    "txl_kernel ==0.2.12",
+    "txl_local_contents ==0.2.12",
+    "txl_local_terminals ==0.2.12",
+    "txl_local_kernels ==0.2.12",
+    "txl_notebook_editor ==0.2.12",
+    "txl_remote_contents ==0.2.12",
+    "txl_remote_terminals ==0.2.12",
+    "txl_remote_kernels ==0.2.12",
+    "txl_text_editor ==0.2.12",
+    "txl_markdown_viewer ==0.2.12",
+    "txl_terminal ==0.2.12",
+    "txl_launcher ==0.2.12",
+    "txl_widgets ==0.2.12",
 ]
 
 [project.optional-dependencies]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings-python",
```

### Comparing `jpterm-0.2.11/PKG-INFO` & `jpterm-0.2.12/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jpterm
-Version: 0.2.11
+Version: 0.2.12
 Summary: Jupyter in the terminal
 Project-URL: Homepage, https://github.com/davidbrochart/jpterm
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: jupyter,textual
 Classifier: Development Status :: 4 - Beta
@@ -12,34 +12,34 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: rich-click>=1.6.0
-Requires-Dist: txl-cell==0.2.11
-Requires-Dist: txl-console==0.2.11
-Requires-Dist: txl-editors==0.2.11
-Requires-Dist: txl-file-browser==0.2.11
-Requires-Dist: txl-image-viewer==0.2.11
-Requires-Dist: txl-jpterm==0.2.11
-Requires-Dist: txl-kernel==0.2.11
-Requires-Dist: txl-launcher==0.2.11
-Requires-Dist: txl-local-contents==0.2.11
-Requires-Dist: txl-local-kernels==0.2.11
-Requires-Dist: txl-local-terminals==0.2.11
-Requires-Dist: txl-markdown-viewer==0.2.11
-Requires-Dist: txl-notebook-editor==0.2.11
-Requires-Dist: txl-remote-contents==0.2.11
-Requires-Dist: txl-remote-kernels==0.2.11
-Requires-Dist: txl-remote-terminals==0.2.11
-Requires-Dist: txl-terminal==0.2.11
-Requires-Dist: txl-text-editor==0.2.11
-Requires-Dist: txl-widgets==0.2.11
-Requires-Dist: txl==0.2.11
+Requires-Dist: txl-cell==0.2.12
+Requires-Dist: txl-console==0.2.12
+Requires-Dist: txl-editors==0.2.12
+Requires-Dist: txl-file-browser==0.2.12
+Requires-Dist: txl-image-viewer==0.2.12
+Requires-Dist: txl-jpterm==0.2.12
+Requires-Dist: txl-kernel==0.2.12
+Requires-Dist: txl-launcher==0.2.12
+Requires-Dist: txl-local-contents==0.2.12
+Requires-Dist: txl-local-kernels==0.2.12
+Requires-Dist: txl-local-terminals==0.2.12
+Requires-Dist: txl-markdown-viewer==0.2.12
+Requires-Dist: txl-notebook-editor==0.2.12
+Requires-Dist: txl-remote-contents==0.2.12
+Requires-Dist: txl-remote-kernels==0.2.12
+Requires-Dist: txl-remote-terminals==0.2.12
+Requires-Dist: txl-terminal==0.2.12
+Requires-Dist: txl-text-editor==0.2.12
+Requires-Dist: txl-widgets==0.2.12
+Requires-Dist: txl==0.2.12
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/davidbrochart/jpterm/workflows/CI/badge.svg)](https://github.com/davidbrochart/jpterm/actions)
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.3 Name: jpterm Version: 0.2.11 Summary: Jupyter in the
+Metadata-Version: 2.3 Name: jpterm Version: 0.2.12 Summary: Jupyter in the
 terminal Project-URL: Homepage, https://github.com/davidbrochart/jpterm Author-
 email: David Brochart
 gmail.com> License: MIT License-File: LICENSE Keywords: jupyter,textual
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10 Requires-Dist: rich-click>=1.6.0 Requires-Dist: txl-
-cell==0.2.11 Requires-Dist: txl-console==0.2.11 Requires-Dist: txl-
-editors==0.2.11 Requires-Dist: txl-file-browser==0.2.11 Requires-Dist: txl-
-image-viewer==0.2.11 Requires-Dist: txl-jpterm==0.2.11 Requires-Dist: txl-
-kernel==0.2.11 Requires-Dist: txl-launcher==0.2.11 Requires-Dist: txl-local-
-contents==0.2.11 Requires-Dist: txl-local-kernels==0.2.11 Requires-Dist: txl-
-local-terminals==0.2.11 Requires-Dist: txl-markdown-viewer==0.2.11 Requires-
-Dist: txl-notebook-editor==0.2.11 Requires-Dist: txl-remote-contents==0.2.11
-Requires-Dist: txl-remote-kernels==0.2.11 Requires-Dist: txl-remote-
-terminals==0.2.11 Requires-Dist: txl-terminal==0.2.11 Requires-Dist: txl-text-
-editor==0.2.11 Requires-Dist: txl-widgets==0.2.11 Requires-Dist: txl==0.2.11
+cell==0.2.12 Requires-Dist: txl-console==0.2.12 Requires-Dist: txl-
+editors==0.2.12 Requires-Dist: txl-file-browser==0.2.12 Requires-Dist: txl-
+image-viewer==0.2.12 Requires-Dist: txl-jpterm==0.2.12 Requires-Dist: txl-
+kernel==0.2.12 Requires-Dist: txl-launcher==0.2.12 Requires-Dist: txl-local-
+contents==0.2.12 Requires-Dist: txl-local-kernels==0.2.12 Requires-Dist: txl-
+local-terminals==0.2.12 Requires-Dist: txl-markdown-viewer==0.2.12 Requires-
+Dist: txl-notebook-editor==0.2.12 Requires-Dist: txl-remote-contents==0.2.12
+Requires-Dist: txl-remote-kernels==0.2.12 Requires-Dist: txl-remote-
+terminals==0.2.12 Requires-Dist: txl-terminal==0.2.12 Requires-Dist: txl-text-
+editor==0.2.12 Requires-Dist: txl-widgets==0.2.12 Requires-Dist: txl==0.2.12
 Provides-Extra: docs Requires-Dist: mkdocs; extra == 'docs' Requires-Dist:
 mkdocs-material; extra == 'docs' Requires-Dist: mkdocstrings-python; extra ==
 'docs' Description-Content-Type: text/markdown [![Build Status](https://
 github.com/davidbrochart/jpterm/workflows/CI/badge.svg)](https://github.com/
 davidbrochart/jpterm/actions) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Hatch
 project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://
```

