# Comparing `tmp/ragdaemon-0.7.0.tar.gz` & `tmp/ragdaemon-0.7.1.tar.gz`

## Comparing `ragdaemon-0.7.0.tar` & `ragdaemon-0.7.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/app.py
--rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/context.py
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/utils.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_astroid.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_line.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_llm.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/annotators/chunker/utils.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/database/pg_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/chunk_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/test_sample.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    63754 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/app.py
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/context.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/utils.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/__init__.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_astroid.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_line.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_llm.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/annotators/chunker/utils.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/database/pg_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/chunk_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/test_sample.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17442 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ragdaemon-0.7.1/PKG-INFO
```

### Comparing `ragdaemon-0.7.0/scratch.ipynb` & `ragdaemon-0.7.1/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tutorial.ipynb` & `ragdaemon-0.7.1/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/.github/workflows/run-tests.yml` & `ragdaemon-0.7.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/app.py` & `ragdaemon-0.7.1/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/context.py` & `ragdaemon-0.7.1/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/daemon.py` & `ragdaemon-0.7.1/ragdaemon/daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -197,28 +197,24 @@
         self,
         query: str,
         instruction: Optional[str] = None,
         revise: bool = True,
         model: Model | TextModel | str = DEFAULT_COMPLETION_MODEL,
     ) -> list[str]:
         """Use summaries to scan the codebase and return relevant nodes."""
-        if "summarizer" not in self.pipeline:
-            raise RagdaemonError("Summarizer annotator required for locate.")
         if instruction is None:
             instruction = "Return items which are relevant to fulfilling the query."
         if isinstance(model, str):
             model = get_model_from_name(model)
         if not isinstance(model, TextModel):
             raise RagdaemonError(f"Invalid model: {model}")
 
         edge_type = "hierarchy"
-        summary_field_id = "summary"
         return await locate(
             self.graph,
             edge_type,
-            summary_field_id,
             self.spice_client,
             instruction,
             query,
             model,
             revise=revise,
         )
```

### Comparing `ragdaemon-0.7.0/ragdaemon/get_paths.py` & `ragdaemon-0.7.1/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/graph.py` & `ragdaemon-0.7.1/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/locate.py` & `ragdaemon-0.7.1/ragdaemon/locate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import asyncio
 
 from spice import Spice, SpiceMessages
 from spice.models import TextModel
 
+from ragdaemon.annotators.summarizer import get_leaf_nodes
 from ragdaemon.graph import KnowledgeGraph
 
 
 async def scan(
     nodes: list[str],
     graph: KnowledgeGraph,
+    edge_type: str,
     spice_client: Spice,
-    summary_field_id: str,
     instruction: str,
     query: str,
     model: TextModel,
 ) -> list[str]:
     """Use an LLM to select relevant nodes from a list."""
-    items = "\n".join(
-        [
-            f"{i+1}: {graph.nodes[child][summary_field_id]}"
-            for i, child in enumerate(nodes)
-        ]
-    )
+    items = []
+    for i, node in enumerate(nodes):
+        children = get_leaf_nodes(graph, node, edge_type)
+        message = f"{i+1}: {node} | {len(children)} children: {', '.join(children[:10])}"
+        if len(children) > 10:
+            message += "..."
+        items.append(message)
 
     def validator(text: str) -> bool:
         if not text:
             return True
         try:
             _ = [int(i) for i in text.split(",")]
             return True
@@ -50,70 +52,65 @@
     return [nodes[int(i) - 1] for i in selected.split(",")]
 
 
 async def bfs(
     node: str,
     graph: KnowledgeGraph,
     edge_type: str,
-    summary_field_id: str,
     spice_client: Spice,
     instruction: str,
     query: str,
     model: TextModel,
 ) -> list[str]:
     """Traverse the graph breadth-first and return relevant nodes."""
     child_nodes = [
         edge[1]
         for edge in graph.out_edges(node, data=True)
         if edge[-1].get("type") == edge_type
-        and graph.nodes[edge[1]].get(summary_field_id) is not None
     ]
     if len(child_nodes) == 0:
         return [node]  # Leaf node (chunk or file)
     nodes = await scan(
-        child_nodes, graph, spice_client, summary_field_id, instruction, query, model
+        child_nodes, graph, edge_type, spice_client, instruction, query, model
     )
     if not nodes:
         return []
     tasks = [
         bfs(
             child,
             graph,
             edge_type,
-            summary_field_id,
             spice_client,
             instruction,
             query,
             model,
         )
         for child in nodes
     ]
     results = await asyncio.gather(*tasks)
     return [node for result in results for node in result]
 
 
 async def locate(
     graph: KnowledgeGraph,
     edge_type: str,
-    summary_field_id: str,
     spice_client: Spice,
     instruction: str,
     query: str,
     model: TextModel,
     revise: bool = False,
 ) -> list[str]:
     """Use summaries to scan the codebase and return relevant nodes."""
     nodes = await bfs(
         "ROOT",
         graph,
         edge_type,
-        summary_field_id,
         spice_client,
         instruction,
         query,
         model,
     )
     if revise:
         nodes = await scan(
-            nodes, graph, spice_client, summary_field_id, instruction, query, model
+            nodes, graph, edge_type, spice_client, instruction, query, model
         )
     return nodes
```

### Comparing `ragdaemon-0.7.0/ragdaemon/utils.py` & `ragdaemon-0.7.1/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/__init__.py` & `ragdaemon-0.7.1/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.7.1/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.7.1/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/diff.py` & `ragdaemon-0.7.1/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.7.1/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.7.1/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.7.1/ragdaemon/annotators/summarizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
-from typing import Optional
+from collections import deque
+from typing import List, Optional
 
 from spice import Spice, SpiceMessages
 from spice.models import TextModel
 from spice.spice import get_model_from_name
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
@@ -15,32 +16,36 @@
     DEFAULT_COMPLETION_MODEL,
     match_refresh,
     semaphore,
     truncate,
 )
 
 
-def count_leaf_nodes_any_depth(
+def get_leaf_nodes(
     graph: KnowledgeGraph,
     node: str,
     edge_type: str = "hierarchy",
     seen: Optional[set[str]] = None,
-) -> int:
-    """Return the number of leaf nodes in the hierarchy rooted at the given node."""
+) -> list[str]:
+    """Return all leaf nodes in the hierarchy rooted at the given node, breadth-first"""
     if seen is None:
         seen = set()
-    seen.add(node)
-    leaf_nodes = 0
-    for edge in graph.out_edges(node, data=True):
-        if edge[-1].get("type") == edge_type:
-            child = edge[1]
-            if child not in seen:
-                leaf_nodes += count_leaf_nodes_any_depth(graph, child, edge_type, seen)
-    if leaf_nodes == 0:
-        leaf_nodes = 1
+    queue: deque = deque([node])
+    leaf_nodes: List[str] = []
+
+    while queue:
+        current = queue.popleft()
+        if current not in seen:
+            seen.add(current)
+            children = [edge[1] for edge in graph.out_edges(current, data=True) if edge[-1].get("type") == edge_type]
+            if children:
+                queue.extend(children)
+            else:
+                leaf_nodes.append(current)
+
     return leaf_nodes
 
 
 def build_filetree(
     graph: KnowledgeGraph,
     target: str,
     current: str = "ROOT",
@@ -51,15 +56,15 @@
     filetree = list[str]()
     edges = sorted(graph.out_edges(current, data=True), key=lambda x: x[1])
     for edge in edges:
         if edge[-1].get("type") == "hierarchy":
             child = edge[1]
             line = child
             summary = graph.nodes[child].get(summary_field_id)
-            leaf_nodes = count_leaf_nodes_any_depth(graph, child)
+            leaf_nodes = len(get_leaf_nodes(graph, child))
             if leaf_nodes > 1:
                 line += f" ({leaf_nodes} items)"
             if summary:
                 line += " - " + summary
             if child == target:
                 line = f"<b>{line}</b>"
             line = prefix + line
```

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/chunker/__init__.py` & `ragdaemon-0.7.1/ragdaemon/annotators/chunker/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_astroid.py` & `ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_astroid.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_line.py` & `ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/chunker/chunk_llm.py` & `ragdaemon-0.7.1/ragdaemon/annotators/chunker/chunk_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/annotators/chunker/utils.py` & `ragdaemon-0.7.1/ragdaemon/annotators/chunker/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/database/__init__.py` & `ragdaemon-0.7.1/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/database/chroma_database.py` & `ragdaemon-0.7.1/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/database/database.py` & `ragdaemon-0.7.1/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/database/lite_database.py` & `ragdaemon-0.7.1/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/database/pg_database.py` & `ragdaemon-0.7.1/ragdaemon/database/pg_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.7.1/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/chunk_llm.toml` & `ragdaemon-0.7.1/ragdaemon/prompts/chunk_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/locate.toml` & `ragdaemon-0.7.1/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.7.1/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/static/favicon.ico` & `ragdaemon-0.7.1/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.7.1/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/static/js/main.js` & `ragdaemon-0.7.1/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.7.1/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/static/js/three/node.js` & `ragdaemon-0.7.1/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.7.1/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/ragdaemon/templates/index.html` & `ragdaemon-0.7.1/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/conftest.py` & `ragdaemon-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/test_comments.py` & `ragdaemon-0.7.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/test_context.py` & `ragdaemon-0.7.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/test_daemon.py` & `ragdaemon-0.7.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/test_get_paths.py` & `ragdaemon-0.7.1/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/test_sample.py` & `ragdaemon-0.7.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/annotators/test_chunker.py` & `ragdaemon-0.7.1/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/annotators/test_diff.py` & `ragdaemon-0.7.1/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/annotators/test_hierarchy.py` & `ragdaemon-0.7.1/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.7.1/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/annotators/test_summarizer.py` & `ragdaemon-0.7.1/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/chunker_graph.json` & `ragdaemon-0.7.1/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/context_message.txt` & `ragdaemon-0.7.1/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/diff_graph.json` & `ragdaemon-0.7.1/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/hard_to_chunk.txt` & `ragdaemon-0.7.1/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/hierarchy_graph.json` & `ragdaemon-0.7.1/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.7.1/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/data/summarizer_graph.json` & `ragdaemon-0.7.1/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/tests/sample/src/interface.py` & `ragdaemon-0.7.1/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/LICENSE` & `ragdaemon-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/README.md` & `ragdaemon-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.7.0/pyproject.toml` & `ragdaemon-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.7.0"
+version = "0.7.1"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "astroid==3.2.2",
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
```

### Comparing `ragdaemon-0.7.0/PKG-INFO` & `ragdaemon-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.7.0
+Version: 0.7.1
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

