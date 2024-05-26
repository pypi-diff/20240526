# Comparing `tmp/ragdaemon-0.6.2.tar.gz` & `tmp/ragdaemon-0.7.0.tar.gz`

## Comparing `ragdaemon-0.6.2.tar` & `ragdaemon-0.7.0.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/app.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/context.py
--rw-r--r--   0        0        0     8180 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0    10267 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/database/pg_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/README.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 ragdaemon-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/app.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/context.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/utils.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_astroid.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_line.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_llm.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/utils.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/pg_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/chunk_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_sample.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/PKG-INFO
```

### Comparing `ragdaemon-0.6.2/scratch.ipynb` & `ragdaemon-0.7.0/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tutorial.ipynb` & `ragdaemon-0.7.0/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/.github/workflows/run-tests.yml` & `ragdaemon-0.7.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/app.py` & `ragdaemon-0.7.0/ragdaemon/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 args = parser.parse_args()
 refresh = args.refresh
 verbose = 2  # Always verbose in server mode
 code_extensions = None if args.code_extensions is None else set(args.code_extensions)
 diff = args.diff
 annotators = {
     "hierarchy": {},
-    "chunker_llm": {"chunk_extensions": code_extensions},
+    "chunker": {"use_llm": True},
     # "summarizer": {},
     # "clusterer_binary": {},
     # "call_graph": {"call_extensions": code_extensions},
     "diff": {"diff": diff},
     "layout_hierarchy": {},
 }
 logging_dir = mentat_dir_path / "ragdaemon" / "spice_logs"
```

### Comparing `ragdaemon-0.6.2/ragdaemon/context.py` & `ragdaemon-0.7.0/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/daemon.py` & `ragdaemon-0.7.0/ragdaemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ragdaemon.locate import locate
 from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, match_refresh, mentat_dir_path
 
 
 def default_annotators():
     return {
         "hierarchy": {},
-        "chunker_line": {"lines_per_chunk": 30},
+        "chunker": {"use_llm": False},
         "diff": {},
     }
 
 
 class Daemon:
     """Build and maintain a searchable knowledge graph of codebase."""
 
@@ -105,15 +105,15 @@
             print(f"Saved updated graph to {self.graph_path}")
 
     async def update(self, refresh: str | bool = False):
         """Iteratively build the knowledge graph
 
         Refresh can be
         - boolean to refresh all annotators/nodes
-        - string matching annotator names / node ids, e.g. ("chunker_llm")
+        - string matching annotator names / node ids, e.g. ("chunker")
         - string with wildcard operators to fuzzy-match annotators/nodes, e.g. ("*diff*")
         """
         _graph = self.graph.copy()
         for name, annotator in self.pipeline.items():
             _refresh = (
                 match_refresh(refresh, name)
                 if isinstance(refresh, str) and refresh in self.pipeline
```

### Comparing `ragdaemon-0.6.2/ragdaemon/get_paths.py` & `ragdaemon-0.7.0/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/graph.py` & `ragdaemon-0.7.0/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/locate.py` & `ragdaemon-0.7.0/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/utils.py` & `ragdaemon-0.7.0/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/__init__.py` & `ragdaemon-0.7.0/ragdaemon/annotators/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from ragdaemon.annotators.base_annotator import Annotator  # noqa: F401
 from ragdaemon.annotators.call_graph import CallGraph  # noqa: F401
 from ragdaemon.annotators.chunker import Chunker
-from ragdaemon.annotators.chunker_line import ChunkerLine
-from ragdaemon.annotators.chunker_llm import ChunkerLLM
 from ragdaemon.annotators.diff import Diff
 from ragdaemon.annotators.hierarchy import Hierarchy
 from ragdaemon.annotators.layout_hierarchy import LayoutHierarchy
 from ragdaemon.annotators.summarizer import Summarizer
 
 annotators_map = {
     "call_graph": CallGraph,
     "chunker": Chunker,
-    "chunker_line": ChunkerLine,
-    "chunker_llm": ChunkerLLM,
     "diff": Diff,
     "hierarchy": Hierarchy,
     "layout_hierarchy": LayoutHierarchy,
     "summarizer": Summarizer,
 }
```

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.7.0/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.7.0/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/chunker.py` & `ragdaemon-0.7.0/ragdaemon/annotators/chunker/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,108 +1,99 @@
-"""
-Chunk data a list of objects following [
-    {id: path/to/file:class.method, start_line: int, end_line: int}
-]
-
-It's stored on the file node as data['chunks'] and json.dumped into the database.
-
-A chunker annotator:
-1. Is complete when all files (with matching extensions) have a 'chunks' field
-2. Generates chunks using a subclass method (llm, ctags..)
-3. Adds that data to each file's graph node and database record
-4. Add graph nodes (and db records) for each of those chunks
-5. Add hierarchy edges connecting everything back to cwd
-
-The Chunker base class below handles everything except step 2.
-"""
-
 import asyncio
 import json
 from copy import deepcopy
+from functools import partial
 from pathlib import Path
-from typing import Any, Optional
 
+from astroid.exceptions import AstroidSyntaxError
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import (
     Database,
     remove_add_to_db_duplicates,
     remove_update_db_duplicates,
 )
+from ragdaemon.annotators.chunker.utils import resolve_chunk_parent
+from ragdaemon.annotators.chunker.chunk_astroid import chunk_document as chunk_astroid
+from ragdaemon.annotators.chunker.chunk_llm import chunk_document as chunk_llm
+from ragdaemon.annotators.chunker.chunk_line import chunk_document as chunk_line
+
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import (
     DEFAULT_CODE_EXTENSIONS,
     get_document,
     hash_str,
     match_refresh,
     truncate,
 )
 
 
-def resolve_chunk_parent(id: str, nodes: set[str]) -> str | None:
-    file, chunk_str = id.split(":")
-    if chunk_str == "BASE":
-        return file
-    elif "." not in chunk_str:
-        return f"{file}:BASE"
-    else:
-        parts = chunk_str.split(".")
-        while True:
-            parent = f"{file}:{'.'.join(parts[:-1])}"
-            if parent in nodes:
-                return parent
-            parent_str = parent.split(":")[1]
-            if "." not in parent_str:
-                return None
-            # If intermediate parents are missing, skip them
-            parts = parent_str.split(".")
-
-
 class Chunker(Annotator):
     name = "chunker"
     chunk_field_id = "chunks"
 
-    def __init__(self, *args, chunk_extensions: Optional[list[str]] = None, **kwargs):
+    def __init__(self, *args, use_llm: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
-        if chunk_extensions is None:
-            chunk_extensions = DEFAULT_CODE_EXTENSIONS
-        self.chunk_extensions = chunk_extensions
+
+        # By default, use either the LLM chunker or a basic line chunker.
+        if use_llm and self.spice_client is not None:
+            default_chunk_fn = partial(
+                chunk_llm, spice_client=self.spice_client, verbose=self.verbose
+            )
+        else:
+            default_chunk_fn = chunk_line
+
+        # For python files, try to use astroid. If that fails, fall back to the default chunker.
+        async def python_chunk_fn(document: str):
+            try:
+                return await chunk_astroid(document)
+            except AstroidSyntaxError:
+                if self.verbose > 0:
+                    file = document.split("\n")[0]
+                    print(
+                        f"Error chunking {file} with astroid; falling back to default chunker."
+                    )
+                return await default_chunk_fn(document)
+
+        self.chunk_extensions_map = {}
+        for extension in DEFAULT_CODE_EXTENSIONS:
+            if extension == ".py":
+                self.chunk_extensions_map[extension] = python_chunk_fn
+            else:
+                self.chunk_extensions_map[extension] = default_chunk_fn
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         for node, data in graph.nodes(data=True):
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") != "file":
                 continue
             chunks = data.get(self.chunk_field_id, None)
             if chunks is None:
-                if self.chunk_extensions is None:
+                if self.chunk_extensions_map is None:
                     return False
                 extension = Path(data["ref"]).suffix
-                if extension in self.chunk_extensions:
+                if extension in self.chunk_extensions_map:
                     return False
             else:
                 if not isinstance(chunks, list):
                     chunks = json.loads(chunks)
                 for chunk in chunks:
                     if chunk["id"] not in graph:
                         return False
         return True
 
-    async def chunk_document(self, document: str) -> list[dict[str, Any]]:
-        """Return a list of {id, ref} chunks for the given document."""
-        raise NotImplementedError()
-
     async def get_file_chunk_data(self, node, data):
         """Generate and save chunk data for a file node to graph and db"""
         document = data["document"]
+        extension = Path(data["ref"]).suffix
         try:
-            chunks = await self.chunk_document(document)
+            chunks = await self.chunk_extensions_map[extension](document)
         except RagdaemonError:
             if self.verbose > 0:
                 print(f"Error chunking {node}; skipping.")
             chunks = []
         chunks = sorted(chunks, key=lambda x: len(x["id"]))
         data[self.chunk_field_id] = chunks
 
@@ -114,19 +105,19 @@
         all_nodes = list(graph.nodes(data=True))
         for node, data in all_nodes:
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") == "chunk":
                 graph.remove_node(node)
             elif data.get("type") == "file":
-                if self.chunk_extensions is None:
+                if self.chunk_extensions_map is None:
                     files_with_chunks.append((node, data))
                 else:
                     extension = Path(data["ref"]).suffix
-                    if extension in self.chunk_extensions:
+                    if extension in self.chunk_extensions_map:
                         files_with_chunks.append((node, data))
 
         # Generate/add chunk data for nodes that don't have it
         tasks = []
         files_just_chunked = set()
         for node, data in files_with_chunks:
             if (
```

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_llm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import json
 from collections import Counter, defaultdict
 from functools import partial
 from json.decoder import JSONDecodeError
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
-from spice import SpiceMessages
-from spice.models import TextModel
+from spice import Spice, SpiceMessages
+from spice.models import GPT_4o
 
-from ragdaemon.annotators.chunker import Chunker, resolve_chunk_parent
+from ragdaemon.annotators.chunker.utils import (
+    Chunk,
+    RawChunk,
+    resolve_chunk_parent,
+    resolve_raw_chunks,
+)
 from ragdaemon.errors import RagdaemonError
-from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, lines_set_to_ref, semaphore
+from ragdaemon.utils import semaphore
 
 
 class ChunkErrorInPreviousBatch(RagdaemonError):
     pass
 
 
 def validate(
     response: str,
     file: str,
     max_line: int,
     file_chunks: Optional[set[str]],
-    last_chunk: Optional[dict[str, Any]],
+    last_chunk: Optional[RawChunk],
 ):
     try:
         chunks = json.loads(response).get("chunks")
     except JSONDecodeError:
         return False
     if not isinstance(chunks, list):
         return False
@@ -95,170 +100,115 @@
             if count > 1:
                 raise ChunkErrorInPreviousBatch(parent)  # Case B)
             return False  # Case A)
 
     return True
 
 
-class ChunkerLLM(Chunker):
-    name = "chunker_llm"
-    chunk_field_id = "chunks_llm"
-
-    def __init__(
-        self,
-        *args,
-        batch_size: int = 800,
-        model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        self.batch_size = batch_size
-        self.model = model
-
-    async def get_llm_response(
-        self,
-        file: str,
-        file_lines: list[str],
-        file_chunks: Optional[set[str]] = None,
-        last_chunk: Optional[dict[str, Any]] = None,
-    ) -> List[Dict[str, Any]]:
-        """Get one chunking response from the LLM model."""
-        if self.spice_client is None:
-            raise RagdaemonError("Spice client is not initialized.")
-
-        messages = SpiceMessages(self.spice_client)
-        messages.add_system_prompt(name="chunker_llm.base")
-        if last_chunk is not None:
-            messages.add_system_prompt(
-                "chunker_llm.continuation", last_chunk=last_chunk
-            )
-        messages.add_user_prompt(
-            "chunker_llm.user", path=file, code="\n".join(file_lines)
-        )
+async def get_llm_response(
+    spice_client: Spice,
+    file: str,
+    file_lines: list[str],
+    file_chunks: Optional[set[str]] = None,
+    last_chunk: Optional[RawChunk] = None,
+    verbose: int = 0,
+) -> List[RawChunk]:
+    """Get one chunking response from the LLM model."""
+    messages = SpiceMessages(spice_client)
+    messages.add_system_prompt(name="chunk_llm.base")
+    if last_chunk is not None:
+        messages.add_system_prompt("chunk_llm.continuation", last_chunk=last_chunk)
+    messages.add_user_prompt("chunk_llm.user", path=file, code="\n".join(file_lines))
 
-        max_line = int(file_lines[-1].split(":")[0])  # Extract line number
+    max_line = int(file_lines[-1].split(":")[0])  # Extract line number
+    validator = partial(
+        validate,
+        file=file,
+        max_line=max_line,
+        file_chunks=file_chunks,
+        last_chunk=last_chunk,
+    )
+    async with semaphore:
+        try:
+            response = await spice_client.get_response(
+                messages=messages,
+                model=GPT_4o,
+                response_format={"type": "json_object"},
+                validator=validator,
+                retries=2,
+            )
+            return json.loads(response.text).get("chunks")
+        except ValueError:
+            pass
         validator = partial(
             validate,
             file=file,
             max_line=max_line,
-            file_chunks=file_chunks,
+            file_chunks=None,  # Skip parent chunk validation
             last_chunk=last_chunk,
         )
-        async with semaphore:
-            try:
-                response = await self.spice_client.get_response(
-                    messages=messages,
-                    model=self.model,
-                    response_format={"type": "json_object"},
-                    validator=validator,
-                    retries=2,
-                )
-                return json.loads(response.text).get("chunks")
-            except ValueError:
-                pass
-            validator = partial(
-                validate,
-                file=file,
-                max_line=max_line,
-                file_chunks=None,  # Skip parent chunk validation
-                last_chunk=last_chunk,
+        try:
+            response = await spice_client.get_response(
+                messages=messages,
+                model=GPT_4o,
+                response_format={"type": "json_object"},
+                validator=validator,
+                retries=1,
             )
-            try:
-                response = await self.spice_client.get_response(
-                    messages=messages,
-                    model=self.model,
-                    response_format={"type": "json_object"},
-                    validator=validator,
-                    retries=1,
+            return json.loads(response.text).get("chunks")
+        except ValueError:
+            if verbose > 0:
+                print(
+                    f"Failed to get chunks for {file} batch ending at line {max_line}."
                 )
-                return json.loads(response.text).get("chunks")
-            except ValueError:
-                if self.verbose > 0:
-                    print(
-                        f"Failed to get chunks for {file} batch ending at line {max_line}."
-                    )
-                return []
-
-    async def chunk_document(self, document: str, retries=1) -> list[dict[str, Any]]:
-        """Parse file_lines into a list of {id, ref} chunks."""
-        lines = document.split("\n")
-        file = lines[0]
-        file_lines = lines[1:]
-        if not file_lines or not any(line for line in file_lines):
             return []
-        file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
 
-        # Get raw llm output: {id, start_line, end_line}
-        chunks = list[dict[str, Any]]()
-        n_batches = (len(file_lines) + self.batch_size - 1) // self.batch_size
-        retries_by_batch = {i: retries for i in range(n_batches)}
-        chunk_index_by_batch = defaultdict(int)
-        i = 0
-        while i < n_batches:
-            while retries_by_batch[i] >= 0:
-                batch_lines = file_lines[
-                    i * self.batch_size : (i + 1) * self.batch_size
-                ]
-                chunk_index_by_batch[i] = len(chunks)
-                last_chunk = chunks.pop() if chunks else None
-                if retries_by_batch[i] > 0:
-                    file_chunks = {c["id"] for c in chunks}
-                else:
-                    file_chunks = None  # Skip parent chunk validation
-                try:
-                    _chunks = await self.get_llm_response(
-                        file, batch_lines, file_chunks, last_chunk
-                    )
-                    chunks.extend(_chunks)
-                    i += 1
-                    break
-                except ChunkErrorInPreviousBatch as e:
-                    if self.verbose > 1:
-                        print(f"Chunker missed parent {e} in file {file}, retrying.")
-                    retries_by_batch[i] -= 1
-                    chunks = chunks[: chunk_index_by_batch[i]]
-                    i = max(0, i - 1)
-
-        # Convert to {id: set(lines)} for easier manipulation
-        chunks = {
-            c["id"]: set(range(c["start_line"], c["end_line"] + 1)) for c in chunks
-        }
-
-        def update_parent_nodes(id: str, _chunks: dict[str, set[int]]):
-            parent_lines = _chunks[id]
-            child_chunks = {k: v for k, v in _chunks.items() if k.startswith(id + ".")}
-            if child_chunks:
-                # Make sure end_line of each 'parent' chunk covers all children
-                start_line = min(parent_lines)
-                end_line = start_line
-                for child_lines in child_chunks.values():
-                    if not child_lines:
-                        continue
-                    end_line = max(end_line, max(child_lines))
-                parent_lines = set(range(start_line, end_line + 1))
-                # Remove child lines from parent lines
-                for child_lines in child_chunks.values():
-                    parent_lines -= child_lines
-                _chunks[id] = parent_lines
-            return _chunks
-
-        ids_longest_first = sorted(chunks, key=lambda x: len(x), reverse=True)
-        for id in ids_longest_first:
-            chunks = update_parent_nodes(id, chunks)
-
-        output = []
-        if chunks:
-            # Generate a 'BASE chunk' with all lines not already part of a chunk
-            base_chunk_lines = set(range(1, len(file_lines) + 1))
-            for lines in chunks.values():
-                base_chunk_lines -= lines
-            lines_ref = lines_set_to_ref(base_chunk_lines)
-            ref = f"{file}:{lines_ref}" if lines_ref else file
-            base_chunk = {"id": f"{file}:BASE", "ref": ref}
-            output.append(base_chunk)
-
-        # Convert to refs and return
-        for id, lines in chunks.items():
-            lines_ref = lines_set_to_ref(lines)
-            ref = f"{file}:{lines_ref}" if lines_ref else file
-            output.append({"id": id, "ref": ref})
-        return output
+
+async def chunk_document(
+    document: str,
+    spice_client: Spice,
+    retries=1,
+    batch_size: int = 800,
+    verbose: int = 0,
+) -> list[Chunk]:
+    """Parse file_lines into a list of {id, ref} chunks."""
+    lines = document.split("\n")
+    file = lines[0]
+    file_lines = lines[1:]
+    if not file_lines or not any(line for line in file_lines):
+        return []
+    file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
+
+    # Get raw llm output: {id, start_line, end_line}
+    chunks = list[RawChunk]()
+    n_batches = (len(file_lines) + batch_size - 1) // batch_size
+    retries_by_batch = {i: retries for i in range(n_batches)}
+    chunk_index_by_batch = defaultdict(int)
+    i = 0
+    while i < n_batches:
+        while retries_by_batch[i] >= 0:
+            batch_lines = file_lines[i * batch_size : (i + 1) * batch_size]
+            chunk_index_by_batch[i] = len(chunks)
+            last_chunk = chunks.pop() if chunks else None
+            if retries_by_batch[i] > 0:
+                file_chunks = {c["id"] for c in chunks}
+            else:
+                file_chunks = None  # Skip parent chunk validation
+            try:
+                _chunks = await get_llm_response(
+                    spice_client,
+                    file,
+                    batch_lines,
+                    file_chunks,
+                    last_chunk,
+                )
+                chunks.extend(_chunks)
+                i += 1
+                break
+            except ChunkErrorInPreviousBatch as e:
+                if verbose > 1:
+                    print(f"Chunker missed parent {e} in file {file}, retrying.")
+                retries_by_batch[i] -= 1
+                chunks = chunks[: chunk_index_by_batch[i]]
+                i = max(0, i - 1)
+
+    return resolve_raw_chunks(document, chunks)
```

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/diff.py` & `ragdaemon-0.7.0/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.7.0/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.7.0/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.7.0/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/database/__init__.py` & `ragdaemon-0.7.0/ragdaemon/database/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-import os
+import os  # noqa: F401
 from pathlib import Path
 from typing import Optional
 
 from spice import Spice
 
 from ragdaemon.database.chroma_database import (
     # ChromaDB,
     remove_add_to_db_duplicates,  # noqa: F401
     remove_update_db_duplicates,  # noqa: F401
 )
 from ragdaemon.database.database import Database
+
+# from ragdaemon.database.chroma_database import ChromaDB
 from ragdaemon.database.lite_database import LiteDB
-from ragdaemon.database.pg_database import PGDB
+
+# from ragdaemon.database.pg_database import PGDB
 from ragdaemon.utils import mentat_dir_path
 
 DEFAULT_EMBEDDING_MODEL = "text-embedding-3-large"
 
 
 def get_db(
     cwd: Path,
     spice_client: Spice,
     embedding_model: str | None = None,
     embedding_provider: Optional[str] = None,
     verbose: int = 0,
 ) -> Database:
     db_path = mentat_dir_path / "chroma"
     db_path.mkdir(parents=True, exist_ok=True)
-    if embedding_model is not None and "PYTEST_CURRENT_TEST" not in os.environ:
-        try:
-            # db = ChromaDB(
-            #     cwd=cwd,
-            #     db_path=db_path,
-            #     spice_client=spice_client,
-            #     embedding_model=embedding_model,
-            #     embedding_provider=embedding_provider,
-            #     verbose=verbose,
-            # )
-            # # In case the api key is wrong, try to embed something to trigger an error.
-            # _ = db.add(ids="test", documents="test doc")
-            # db.delete(ids="test")
-            db = PGDB(cwd=cwd, db_path=db_path, verbose=verbose)
-            return db
-        except Exception as e:
-            if verbose > 1:
-                print(
-                    f"Failed to initialize Postgres Database: {e}. Falling back to LiteDB."
-                )
-            pass
+    # if embedding_model is not None and "PYTEST_CURRENT_TEST" not in os.environ:
+    #     try:
+    #         # db = ChromaDB(
+    #         #     cwd=cwd,
+    #         #     db_path=db_path,
+    #         #     spice_client=spice_client,
+    #         #     embedding_model=embedding_model,
+    #         #     embedding_provider=embedding_provider,
+    #         #     verbose=verbose,
+    #         # )
+    #         # # In case the api key is wrong, try to embed something to trigger an error.
+    #         # _ = db.add(ids="test", documents="test doc")
+    #         # db.delete(ids="test")
+    #         db = PGDB(cwd=cwd, db_path=db_path, verbose=verbose)
+    #         return db
+    #     except Exception as e:
+    #         if verbose > 1:
+    #             print(
+    #                 f"Failed to initialize Postgres Database: {e}. Falling back to LiteDB."
+    #             )
+    #         pass
     return LiteDB(cwd=cwd, db_path=db_path, verbose=verbose)
```

### Comparing `ragdaemon-0.6.2/ragdaemon/database/chroma_database.py` & `ragdaemon-0.7.0/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/database/database.py` & `ragdaemon-0.7.0/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/database/lite_database.py` & `ragdaemon-0.7.0/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/database/pg_database.py` & `ragdaemon-0.7.0/ragdaemon/database/pg_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 
 
 class DocumentMetadata(Base):
     __tablename__ = "document_metadata"
 
     id: Mapped[str] = mapped_column(primary_key=True)
     # We serialize whatever we get, which can be 'null', so we need Optional
-    chunks_llm: Mapped[Optional[str]]
+    chunks: Mapped[Optional[str]]
 
 
-def retry_on_exception(retries: int=3, exceptions={OperationalError}):
+def retry_on_exception(retries: int = 3, exceptions={OperationalError}):
     def decorator(func):
         def wrapper(*args, **kwargs):
             for i in range(retries):
                 try:
                     return func(*args, **kwargs)
                 except exceptions as e:
                     print(f"Caught exception: {e}")
                     if i == retries - 1:
                         raise e
+
         return wrapper
+
     return decorator
 
 
 class Engine:
     def __init__(self, verbose: int = 0):
         database = "ragdaemon"
         host = os.environ.get("RAGDAEMON_DB_ENDPOINT", None)
@@ -128,15 +130,15 @@
         super().__init__(*args, **kwargs)
         self._collection = PGCollection(self.verbose)
 
 
 class PGCollection(LiteCollection):
     """Wraps a LiteDB and adds/gets targeted fields from a remote Postgres Database."""
 
-    def __init__(self, *args, fields: list[str] = ["chunks_llm"], **kwargs):
+    def __init__(self, *args, fields: list[str] = ["chunks"], **kwargs):
         super().__init__(*args, **kwargs)
         self.engine = Engine(self.verbose)
         self.fields = fields
 
     @override
     def update(self, ids: list[str] | str, metadatas: list[dict] | dict):
         remote_records = defaultdict(dict)
@@ -165,27 +167,20 @@
     @override
     def get(
         self,
         ids: list[str] | str,
         include: list[str] | None = None,
     ):
         response = super().get(ids, include)
-        if include is not None and "metadatas" in include:
-            if not isinstance(ids, list):
-                ids = [ids]
-            remote_metadatas = self.engine.get_document_metadata(ids)
-            seen = set()
+        response_ids = response.get("ids", [])
+        if response_ids and include is not None and "metadatas" in include:
+            remote_metadatas = self.engine.get_document_metadata(response_ids)
             for id, metadata in zip(
                 response.get("ids", []), response.get("metadatas", [])
             ):
                 if id in remote_metadatas:
                     metadata.update(remote_metadatas[id])
-                    seen.add(id)
-            for k, v in remote_metadatas.items():
-                if k not in seen:
-                    response["ids"].append(k)
-                    response["metadatas"].append(v)
         return response
 
 
 if __name__ == "__main__":
     Engine().migrate()
```

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.7.0/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.7.0/ragdaemon/prompts/chunk_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/locate.toml` & `ragdaemon-0.7.0/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/static/favicon.ico` & `ragdaemon-0.7.0/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.7.0/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/static/js/main.js` & `ragdaemon-0.7.0/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.7.0/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/static/js/three/node.js` & `ragdaemon-0.7.0/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.7.0/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/ragdaemon/templates/index.html` & `ragdaemon-0.7.0/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/conftest.py` & `ragdaemon-0.7.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/test_comments.py` & `ragdaemon-0.7.0/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/test_context.py` & `ragdaemon-0.7.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/test_daemon.py` & `ragdaemon-0.7.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/test_get_paths.py` & `ragdaemon-0.7.0/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/test_sample.py` & `ragdaemon-0.7.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/annotators/test_diff.py` & `ragdaemon-0.7.0/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/annotators/test_hierarchy.py` & `ragdaemon-0.7.0/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.7.0/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/annotators/test_summarizer.py` & `ragdaemon-0.7.0/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/chunker_graph.json` & `ragdaemon-0.7.0/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/context_message.txt` & `ragdaemon-0.7.0/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/diff_graph.json` & `ragdaemon-0.7.0/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/hard_to_chunk.txt` & `ragdaemon-0.7.0/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/hierarchy_graph.json` & `ragdaemon-0.7.0/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.7.0/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/tests/data/summarizer_graph.json` & `ragdaemon-0.7.0/tests/data/summarizer_graph.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957894736842106%*

 * *Differences: {"'nodes'": "{0: {'chunks': [OrderedDict([('id', 'src/interface.py:BASE'), ('ref', "*

 * *            "'src/interface.py:1-4,15-16,19')]), OrderedDict([('id', "*

 * *            "'src/interface.py:parse_arguments'), ('ref', 'src/interface.py:5-14')]), "*

 * *            "OrderedDict([('id', 'src/interface.py:render_response'), ('ref', "*

 * *            "'src/interface.py:17-18')])], delete: ['chunks_llm']}, 2: {'chunks': [], delete: "*

 * *            "['chunks_llm']}, 4: {'chunks': [OrderedDict([('id', 'src/operations.py:BASE'),  […]*

```diff
@@ -151,15 +151,15 @@
         }
     ],
     "multigraph": true,
     "nodes": [
         {
             "calls": "{}",
             "checksum": "0d78297d1a17a762d876be21cc8692cb",
-            "chunks_llm": [
+            "chunks": [
                 {
                     "id": "src/interface.py:BASE",
                     "ref": "src/interface.py:1-4,15-16,19"
                 },
                 {
                     "id": "src/interface.py:parse_arguments",
                     "ref": "src/interface.py:5-14"
@@ -184,15 +184,15 @@
             "summary": "Describe the application's experimental purpose in testing the limits of the treesitter parser.",
             "summary_checksum": "f512afb951427a1494eecd927607aa42",
             "type": "file"
         },
         {
             "calls": "{}",
             "checksum": "b9ba74388a4d956f0aff968bfc165db3",
-            "chunks_llm": [],
+            "chunks": [],
             "document": "src/__init__.py\n",
             "id": "src/__init__.py",
             "ref": "src/__init__.py",
             "summary": "Establish the 'src' as a Python package to organize related modules concerning command-line based arithmetic operations, without adding any explicit functionality.",
             "summary_checksum": "207e3de4ed658542202ca6ccc3376a96",
             "type": "file"
         },
@@ -204,15 +204,15 @@
             "summary": "Manage exclusions for version control by specifying files and directories that Git should ignore, while ensuring the .gitignore file itself remains tracked.",
             "summary_checksum": "5f3c1aebfa8418a5845a2c5ddc2b33cf",
             "type": "file"
         },
         {
             "calls": "{}",
             "checksum": "cfe1b2f9cda812d0e1f68eac86539e94",
-            "chunks_llm": [
+            "chunks": [
                 {
                     "id": "src/operations.py:BASE",
                     "ref": "src/operations.py:1-3,6-7,10-11,14-15,18-19,22"
                 },
                 {
                     "id": "src/operations.py:add",
                     "ref": "src/operations.py:4-5"
@@ -240,15 +240,15 @@
             "summary": "Define basic arithmetic operations including addition, subtraction, multiplication, division, and square root calculation utilizing Python's math library.",
             "summary_checksum": "f32593b8091a214cc0042312abb4626c",
             "type": "file"
         },
         {
             "calls": "{\"src/interface.py:parse_arguments\": [6], \"src/interface.py:render_response\": [19], \"src/operations.py:add\": [9], \"src/operations.py:subtract\": [11], \"src/operations.py:multiply\": [13], \"src/operations.py:divide\": [15]}",
             "checksum": "30a15283b0f5d5ac17a2d890a00675d9",
-            "chunks_llm": [
+            "chunks": [
                 {
                     "id": "main.py:BASE",
                     "ref": "main.py:1-4,20-24"
                 },
                 {
                     "id": "main.py:main",
                     "ref": "main.py:5-19"
```

### Comparing `ragdaemon-0.6.2/tests/sample/src/interface.py` & `ragdaemon-0.7.0/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/LICENSE` & `ragdaemon-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/README.md` & `ragdaemon-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.6.2/pyproject.toml` & `ragdaemon-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.6.2"
+version = "0.7.0"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
+    "astroid==3.2.2",
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
     "psycopg2-binary==2.9.9",
     "rank_bm25==0.2.2",
```

### Comparing `ragdaemon-0.6.2/PKG-INFO` & `ragdaemon-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.6.2
+Version: 0.7.0
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: astroid==3.2.2
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: dict2xml==1.7.5
 Requires-Dist: fastapi==0.109.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: networkx==3.2.1
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: rank-bm25==0.2.2
```

