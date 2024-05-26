# Comparing `tmp/lenlp-1.0.1.tar.gz` & `tmp/lenlp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenlp-1.0.1.tar", last modified: Sun May 26 01:37:25 2024, max compression
+gzip compressed data, was "lenlp-1.0.2.tar", last modified: Sun May 26 01:44:15 2024, max compression
```

## Comparing `lenlp-1.0.1.tar` & `lenlp-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.709364 lenlp-1.0.1/
--rw-r--r--   0 runner     (501) staff       (20)      479 2024-05-26 01:35:47.000000 lenlp-1.0.1/Cargo.toml
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-26 01:35:47.000000 lenlp-1.0.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      447 2024-05-26 01:37:25.709189 lenlp-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.705540 lenlp-1.0.1/lenlp/
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/__version__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.706565 lenlp-1.0.1/lenlp/analyzer/
--rw-r--r--   0 runner     (501) staff       (20)       59 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/analyzer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1921 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/analyzer/analyze.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.707027 lenlp-1.0.1/lenlp/counter/
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/counter/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3909 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/counter/count.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.707454 lenlp-1.0.1/lenlp/flash/
--rw-r--r--   0 runner     (501) staff       (20)       59 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/flash/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1414 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/flash/flash_text.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.707992 lenlp-1.0.1/lenlp/normalizer/
--rw-r--r--   0 runner     (501) staff       (20)       58 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/normalizer/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      493 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/normalizer/normalize.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.708897 lenlp-1.0.1/lenlp/sparse/
--rw-r--r--   0 runner     (501) staff       (20)      204 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3749 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/bm25_vectorizer.py
--rw-r--r--   0 runner     (501) staff       (20)     3649 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/count_vectorizer.py
--rw-r--r--   0 runner     (501) staff       (20)     3864 2024-05-26 01:35:47.000000 lenlp-1.0.1/lenlp/sparse/tfidf_vectorizer.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-26 01:37:25.706189 lenlp-1.0.1/lenlp.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      447 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      548 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      135 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-26 01:37:25.000000 lenlp-1.0.1/lenlp.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-26 01:37:25.709437 lenlp-1.0.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1027 2024-05-26 01:35:47.000000 lenlp-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.113121 lenlp-1.0.2/
+-rw-rw-rw-   0        0        0      504 2024-05-26 01:43:32.000000 lenlp-1.0.2/Cargo.toml
+-rw-rw-rw-   0        0        0       47 2024-05-26 01:43:32.000000 lenlp-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      460 2024-05-26 01:44:15.113121 lenlp-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.102611 lenlp-1.0.2/lenlp/
+-rw-rw-rw-   0        0        0       97 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.106047 lenlp-1.0.2/lenlp/analyzer/
+-rw-rw-rw-   0        0        0       64 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     1973 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/analyzer/analyze.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.107206 lenlp-1.0.2/lenlp/counter/
+-rw-rw-rw-   0        0        0       49 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/counter/__init__.py
+-rw-rw-rw-   0        0        0     3999 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/counter/count.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.108367 lenlp-1.0.2/lenlp/flash/
+-rw-rw-rw-   0        0        0       62 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/flash/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/flash/flash_text.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.109521 lenlp-1.0.2/lenlp/normalizer/
+-rw-rw-rw-   0        0        0       61 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/normalizer/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/normalizer/normalize.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.112601 lenlp-1.0.2/lenlp/sparse/
+-rw-rw-rw-   0        0        0      209 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/sparse/__init__.py
+-rw-rw-rw-   0        0        0     3866 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/sparse/bm25_vectorizer.py
+-rw-rw-rw-   0        0        0     3763 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/sparse/count_vectorizer.py
+-rw-rw-rw-   0        0        0     3988 2024-05-26 01:43:32.000000 lenlp-1.0.2/lenlp/sparse/tfidf_vectorizer.py
+drwxrwxrwx   0        0        0        0 2024-05-26 01:44:15.104844 lenlp-1.0.2/lenlp.egg-info/
+-rw-rw-rw-   0        0        0      460 2024-05-26 01:44:15.000000 lenlp-1.0.2/lenlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2024-05-26 01:44:15.000000 lenlp-1.0.2/lenlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 01:44:15.000000 lenlp-1.0.2/lenlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-05-26 01:44:15.000000 lenlp-1.0.2/lenlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-26 01:44:15.000000 lenlp-1.0.2/lenlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 01:44:15.113121 lenlp-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2024-05-26 01:43:32.000000 lenlp-1.0.2/setup.py
```

### Comparing `lenlp-1.0.1/lenlp/analyzer/analyze.py` & `lenlp-1.0.2/lenlp/analyzer/analyze.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from rslenlp import rschar_ngrams_many, rschar_wb_ngrams_many, rssplit_words_many
-
-__all__ = ["analyze"]
-
-
-def analyze(
-    x: str | list[str],
-    analyzer: str = "word",
-    ngram_range: tuple[int, int] = (1, 1),
-) -> str | list[str]:
-    """Split text or list of texts into words or characters.
-
-    Parameters
-    ----------
-    x
-        str or list of str.
-    analyzer
-        {word, char, char_wb}, default=word.
-        Whether the feature should be made of word n-gram or character n-grams. Option
-        char_wb creates character n-grams only from text inside word boundaries;
-        n-grams at the edges of words are padded with space.
-    ngram_range
-        tuple (min_n, max_n), default=(1).
-        The lower and upper boundary of the range of n-values for different n-grams to
-        be extracted. All values of n such that min_n <= n <= max_n will be used.
-    Examples
-    --------
-    >>> from lenlp import analyzer
-
-    >>> analyzer.analyze("Hello, world!", analyzer="word")
-    ['Hello,', 'world!']
-
-    >>> analyzer.analyze("Hello, world!", analyzer="char_wb", ngram_range=(3, 3))
-    ['Hel', 'ell', 'llo', 'lo,', 'o, ', ', w', ' wo', 'wor', 'orl', 'rld', 'ld!']
-
-    >>> analyzer.analyze(["hello, world", "good"], analyzer="char", ngram_range=(2, 3))
-    [['he', 'el', 'll', 'lo', 'o,', ', ', ' w', 'wo', 'or', 'rl', 'ld', 'hel', 'ell', 'llo', 'lo,', 'o, ', ', w', ' wo', 'wor', 'orl', 'rld'], ['go', 'oo', 'od', 'goo', 'ood']]
-
-    """
-    return_string = True if isinstance(x, str) else False
-    x = [x] if isinstance(x, str) else x
-    n_sizes = list(range(ngram_range[0], ngram_range[1] + 1))
-
-    match analyzer:
-        case "word":
-            y = rssplit_words_many(x, n_sizes=n_sizes)
-        case "char":
-            y = rschar_ngrams_many(x, n_sizes=n_sizes)
-        case "char_wb":
-            y = rschar_wb_ngrams_many(x, n_sizes=n_sizes)
-
-    return y[0] if return_string else y
+from rslenlp import rschar_ngrams_many, rschar_wb_ngrams_many, rssplit_words_many
+
+__all__ = ["analyze"]
+
+
+def analyze(
+    x: str | list[str],
+    analyzer: str = "word",
+    ngram_range: tuple[int, int] = (1, 1),
+) -> str | list[str]:
+    """Split text or list of texts into words or characters.
+
+    Parameters
+    ----------
+    x
+        str or list of str.
+    analyzer
+        {word, char, char_wb}, default=word.
+        Whether the feature should be made of word n-gram or character n-grams. Option
+        char_wb creates character n-grams only from text inside word boundaries;
+        n-grams at the edges of words are padded with space.
+    ngram_range
+        tuple (min_n, max_n), default=(1).
+        The lower and upper boundary of the range of n-values for different n-grams to
+        be extracted. All values of n such that min_n <= n <= max_n will be used.
+    Examples
+    --------
+    >>> from lenlp import analyzer
+
+    >>> analyzer.analyze("Hello, world!", analyzer="word")
+    ['Hello,', 'world!']
+
+    >>> analyzer.analyze("Hello, world!", analyzer="char_wb", ngram_range=(3, 3))
+    ['Hel', 'ell', 'llo', 'lo,', 'o, ', ', w', ' wo', 'wor', 'orl', 'rld', 'ld!']
+
+    >>> analyzer.analyze(["hello, world", "good"], analyzer="char", ngram_range=(2, 3))
+    [['he', 'el', 'll', 'lo', 'o,', ', ', ' w', 'wo', 'or', 'rl', 'ld', 'hel', 'ell', 'llo', 'lo,', 'o, ', ', w', ' wo', 'wor', 'orl', 'rld'], ['go', 'oo', 'od', 'goo', 'ood']]
+
+    """
+    return_string = True if isinstance(x, str) else False
+    x = [x] if isinstance(x, str) else x
+    n_sizes = list(range(ngram_range[0], ngram_range[1] + 1))
+
+    match analyzer:
+        case "word":
+            y = rssplit_words_many(x, n_sizes=n_sizes)
+        case "char":
+            y = rschar_ngrams_many(x, n_sizes=n_sizes)
+        case "char_wb":
+            y = rschar_wb_ngrams_many(x, n_sizes=n_sizes)
+
+    return y[0] if return_string else y
```

### Comparing `lenlp-1.0.1/lenlp/counter/count.py` & `lenlp-1.0.2/lenlp/counter/count.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from rslenlp import (
-    rsvectorize_char_ngrams_many,
-    rsvectorize_char_wb_ngrams_many,
-    rsvectorize_split_words_many,
-)
-
-__all__ = ["count"]
-
-
-def count(
-    x: str | list[str],
-    analyzer: str = "word",
-    ngram_range: tuple[int, int] = (1, 1),
-    normalize: bool = True,
-    stop_words: list[str] = None,
-    sort: bool = False,
-) -> dict[str, int]:
-    """Count the frequency of words in a text or in a list of texts. Tokens are unordered within
-    the same text.
-
-    Parameters
-    ----------
-    x
-        str or list of str.
-    analyzer
-        {word, char, char_wb}, default=word.
-        Whether the feature should be made of word n-gram or character n-grams. Option
-        char_wb creates character n-grams only from text inside word boundaries;
-        n-grams at the edges of words are padded with space.
-    ngram_range
-        tuple (min_n, max_n), default=1.
-        The lower and upper boundary of the range of n-values for different n-grams to
-        be extracted. All values of n such that min_n <= n <= max_n will be used.
-    normalize
-        bool, default=True.
-        Whether to normalize the text before counting. It will lowercase the text and remove
-        punctuation.
-    stop_words
-        list of str, default=None.
-        A list of stop words that will be removed from the text.
-
-    Examples
-    --------
-    >>> from lenlp import counter
-
-    >>> counter.count("Hello, world!", sort=True)
-    {'hello': 1, 'world': 1}
-
-    >>> counter.count("Hello, world!", ngram_range=[2, 2], sort=True, normalize=False)
-    {'Hello, world!': 1}
-
-    >>> counter.count(["Hello, world!", "How are you?"], stop_words=["are", "you"], sort=True)
-    [{'hello': 1, 'world': 1}, {'how': 1}]
-
-    >>> counter.count(["Hello, world!", "hello"], analyzer="char_wb", ngram_range=(3, 7), stop_words=["hello"], sort=True)
-    [{'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}, {}]
-
-    >>> counter.count("Hello, world!", analyzer="char_wb", ngram_range=(3, 7), sort=True)
-    {' wo': 1, ' wor': 1, ' worl': 1, ' world': 1, 'ell': 1, 'ello': 1, 'ello ': 1, 'ello w': 1, 'ello wo': 1, 'hel': 1, 'hell': 1, 'hello': 1, 'hello ': 1, 'hello w': 1, 'llo': 1, 'llo ': 1, 'llo w': 1, 'llo wo': 1, 'llo wor': 1, 'lo ': 1, 'lo w': 1, 'lo wo': 1, 'lo wor': 1, 'lo worl': 1, 'o w': 1, 'o wo': 1, 'o wor': 1, 'o worl': 1, 'o world': 1, 'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}
-
-    >>> counter.count("Hello, world!", analyzer="char", ngram_range=(3, 7), sort=True)
-    {' wo': 1, ' wor': 1, ' worl': 1, ' world': 1, 'ell': 1, 'ello': 1, 'ello ': 1, 'ello w': 1, 'ello wo': 1, 'hel': 1, 'hell': 1, 'hello': 1, 'hello ': 1, 'hello w': 1, 'llo': 1, 'llo ': 1, 'llo w': 1, 'llo wo': 1, 'llo wor': 1, 'lo ': 1, 'lo w': 1, 'lo wo': 1, 'lo wor': 1, 'lo worl': 1, 'o w': 1, 'o wo': 1, 'o wor': 1, 'o worl': 1, 'o world': 1, 'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}
-
-    >>> counter.count(["Hello, world!", "hello"], analyzer="char", ngram_range=(3, 7), stop_words=["hello"], sort=True)
-    [{'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}, {}]
-
-    """
-    return_string = True if isinstance(x, str) else False
-    x = [x] if isinstance(x, str) else x
-    n_sizes = list(range(ngram_range[0], ngram_range[1] + 1))
-
-    match analyzer:
-        case "word":
-            y = rsvectorize_split_words_many(
-                x, n_sizes=n_sizes, stop_words=stop_words, normalize=normalize
-            )
-        case "char":
-            y = rsvectorize_char_ngrams_many(
-                x, n_sizes=n_sizes, stop_words=stop_words, normalize=normalize
-            )
-
-        case "char_wb":
-            y = rsvectorize_char_wb_ngrams_many(
-                x, n_sizes=n_sizes, stop_words=stop_words, normalize=normalize
-            )
-
-    if sort:
-        y = [dict(sorted(d.items())) for d in y]
-
-    return y[0] if return_string else y
+from rslenlp import (
+    rsvectorize_char_ngrams_many,
+    rsvectorize_char_wb_ngrams_many,
+    rsvectorize_split_words_many,
+)
+
+__all__ = ["count"]
+
+
+def count(
+    x: str | list[str],
+    analyzer: str = "word",
+    ngram_range: tuple[int, int] = (1, 1),
+    normalize: bool = True,
+    stop_words: list[str] = None,
+    sort: bool = False,
+) -> dict[str, int]:
+    """Count the frequency of words in a text or in a list of texts. Tokens are unordered within
+    the same text.
+
+    Parameters
+    ----------
+    x
+        str or list of str.
+    analyzer
+        {word, char, char_wb}, default=word.
+        Whether the feature should be made of word n-gram or character n-grams. Option
+        char_wb creates character n-grams only from text inside word boundaries;
+        n-grams at the edges of words are padded with space.
+    ngram_range
+        tuple (min_n, max_n), default=1.
+        The lower and upper boundary of the range of n-values for different n-grams to
+        be extracted. All values of n such that min_n <= n <= max_n will be used.
+    normalize
+        bool, default=True.
+        Whether to normalize the text before counting. It will lowercase the text and remove
+        punctuation.
+    stop_words
+        list of str, default=None.
+        A list of stop words that will be removed from the text.
+
+    Examples
+    --------
+    >>> from lenlp import counter
+
+    >>> counter.count("Hello, world!", sort=True)
+    {'hello': 1, 'world': 1}
+
+    >>> counter.count("Hello, world!", ngram_range=[2, 2], sort=True, normalize=False)
+    {'Hello, world!': 1}
+
+    >>> counter.count(["Hello, world!", "How are you?"], stop_words=["are", "you"], sort=True)
+    [{'hello': 1, 'world': 1}, {'how': 1}]
+
+    >>> counter.count(["Hello, world!", "hello"], analyzer="char_wb", ngram_range=(3, 7), stop_words=["hello"], sort=True)
+    [{'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}, {}]
+
+    >>> counter.count("Hello, world!", analyzer="char_wb", ngram_range=(3, 7), sort=True)
+    {' wo': 1, ' wor': 1, ' worl': 1, ' world': 1, 'ell': 1, 'ello': 1, 'ello ': 1, 'ello w': 1, 'ello wo': 1, 'hel': 1, 'hell': 1, 'hello': 1, 'hello ': 1, 'hello w': 1, 'llo': 1, 'llo ': 1, 'llo w': 1, 'llo wo': 1, 'llo wor': 1, 'lo ': 1, 'lo w': 1, 'lo wo': 1, 'lo wor': 1, 'lo worl': 1, 'o w': 1, 'o wo': 1, 'o wor': 1, 'o worl': 1, 'o world': 1, 'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}
+
+    >>> counter.count("Hello, world!", analyzer="char", ngram_range=(3, 7), sort=True)
+    {' wo': 1, ' wor': 1, ' worl': 1, ' world': 1, 'ell': 1, 'ello': 1, 'ello ': 1, 'ello w': 1, 'ello wo': 1, 'hel': 1, 'hell': 1, 'hello': 1, 'hello ': 1, 'hello w': 1, 'llo': 1, 'llo ': 1, 'llo w': 1, 'llo wo': 1, 'llo wor': 1, 'lo ': 1, 'lo w': 1, 'lo wo': 1, 'lo wor': 1, 'lo worl': 1, 'o w': 1, 'o wo': 1, 'o wor': 1, 'o worl': 1, 'o world': 1, 'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}
+
+    >>> counter.count(["Hello, world!", "hello"], analyzer="char", ngram_range=(3, 7), stop_words=["hello"], sort=True)
+    [{'orl': 1, 'orld': 1, 'rld': 1, 'wor': 1, 'worl': 1, 'world': 1}, {}]
+
+    """
+    return_string = True if isinstance(x, str) else False
+    x = [x] if isinstance(x, str) else x
+    n_sizes = list(range(ngram_range[0], ngram_range[1] + 1))
+
+    match analyzer:
+        case "word":
+            y = rsvectorize_split_words_many(
+                x, n_sizes=n_sizes, stop_words=stop_words, normalize=normalize
+            )
+        case "char":
+            y = rsvectorize_char_ngrams_many(
+                x, n_sizes=n_sizes, stop_words=stop_words, normalize=normalize
+            )
+
+        case "char_wb":
+            y = rsvectorize_char_wb_ngrams_many(
+                x, n_sizes=n_sizes, stop_words=stop_words, normalize=normalize
+            )
+
+    if sort:
+        y = [dict(sorted(d.items())) for d in y]
+
+    return y[0] if return_string else y
```

### Comparing `lenlp-1.0.1/lenlp/flash/flash_text.py` & `lenlp-1.0.2/lenlp/flash/flash_text.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from rslenlp import RSKeywordProcessor
-
-__all__ = ["FlashText"]
-
-
-class FlashText:
-    """FlashText retrieve keywords from text.
-
-    Parameters
-    ----------
-    lowercase
-        bool, default=True.
-        Whether to lowercase the text before extracting keywords.
-    normalize
-        bool, default=True.
-        Whether to normalize the text before extracting keywords. It will lowercase the text
-        and remove punctuation.
-
-    Examples
-    --------
-    >>> from lenlp import flash
-
-    >>> flash_text = flash.FlashText(normalize=True)
-    >>> flash_text = flash_text.add(["hello", "world"])
-
-    >>> flash_text.extract(["Hello, world!", "world", "hello"], span_info=True)
-    [['hello:0:5'], [], []]
-
-    """
-
-    def __init__(self, lowercase: bool = True, normalize: bool = True) -> None:
-        self.flash = RSKeywordProcessor(lowercase=lowercase, normalize=normalize)
-
-    def add(self, x: str | list[str]) -> None:
-        """Add a keyword to the FlashText object."""
-        x = [x] if isinstance(x, str) else x
-        self.flash.add_keywords_many(x)
-        return self
-
-    def extract(self, x: str | list[str], span_info: bool = False) -> list[str]:
-        """Extract keywords from a sentence."""
-        is_string = isinstance(x, str)
-        x = [x] if isinstance(x, str) else x
-        y = self.flash.extract_keywords_many(x, span_info=span_info)
-        return y[0] if is_string else y
+from rslenlp import RSKeywordProcessor
+
+__all__ = ["FlashText"]
+
+
+class FlashText:
+    """FlashText retrieve keywords from text.
+
+    Parameters
+    ----------
+    lowercase
+        bool, default=True.
+        Whether to lowercase the text before extracting keywords.
+    normalize
+        bool, default=True.
+        Whether to normalize the text before extracting keywords. It will lowercase the text
+        and remove punctuation.
+
+    Examples
+    --------
+    >>> from lenlp import flash
+
+    >>> flash_text = flash.FlashText(normalize=True)
+    >>> flash_text = flash_text.add(["hello", "world"])
+
+    >>> flash_text.extract(["Hello, world!", "world", "hello"], span_info=True)
+    [['hello:0:5'], [], []]
+
+    """
+
+    def __init__(self, lowercase: bool = True, normalize: bool = True) -> None:
+        self.flash = RSKeywordProcessor(lowercase=lowercase, normalize=normalize)
+
+    def add(self, x: str | list[str]) -> None:
+        """Add a keyword to the FlashText object."""
+        x = [x] if isinstance(x, str) else x
+        self.flash.add_keywords_many(x)
+        return self
+
+    def extract(self, x: str | list[str], span_info: bool = False) -> list[str]:
+        """Extract keywords from a sentence."""
+        is_string = isinstance(x, str)
+        x = [x] if isinstance(x, str) else x
+        y = self.flash.extract_keywords_many(x, span_info=span_info)
+        return y[0] if is_string else y
```

### Comparing `lenlp-1.0.1/lenlp/sparse/bm25_vectorizer.py` & `lenlp-1.0.2/lenlp/sparse/bm25_vectorizer.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import numpy as np
-from scipy.sparse import csr_matrix
-from sklearn.utils.sparsefuncs_fast import inplace_csr_row_normalize_l2
-
-from .tfidf_vectorizer import TfIdfVectorizer
-
-
-class BM25Vectorizer(TfIdfVectorizer):
-    """BM25Vectorizer is a class that converts a collection of text documents to a sparse
-    bm25 matrix.
-
-    Parameters
-    ----------
-    analyzer
-        {word, char, char_wb}, default=word.
-        Whether the feature should be made of word n-gram or character n-grams. Option
-        char_wb creates character n-grams only from text inside word boundaries;
-        n-grams at the edges of words are padded with space.
-    ngram_range
-        tuple (min_n, max_n), default=(1, 1).
-        The lower and upper boundary of the range of n-values for different n-grams to
-        be extracted. All values of n such that min_n <= n <= max_n will be used.
-    normalize
-        bool, default=True.
-        Whether to normalize the text before counting. It will lowercase the text and remove
-        punctuation.
-    stop_words
-        list of str, default=None.
-        A list of stop words that will be removed from the text.
-    b
-        The impact of document length normalization.  Default is `0.75`, Higher will
-        penalize longer documents more.
-    k1
-        How quickly the impact of term frequency saturates.  Default is `1.5`, Higher
-        will make term frequency more influential.
-    epsilon
-        Smoothing term. Default is `0`.
-
-    Examples
-    --------
-    >>> from lenlp import sparse
-
-    >>> bm25_vectorizer = sparse.BM25Vectorizer(
-    ...     analyzer="word",
-    ...     normalize=True,
-    ...     stop_words=None,
-    ... )
-
-    >>> x = ["Hello, world!", "How are you?"]
-
-    >>> bm25_vectorizer = bm25_vectorizer.fit(x)
-    >>> matrix = bm25_vectorizer.transform(x)
-    >>> matrix.shape
-    (2, 5)
-
-    >>> len(bm25_vectorizer.vocabulary)
-    5
-
-    >>> matrix = bm25_vectorizer.fit_transform(x)
-    >>> matrix.shape
-    (2, 5)
-
-    """
-
-    def __init__(
-        self,
-        analyzer: str = "word",
-        ngram_range: tuple[int, int] = (1, 1),
-        normalize: bool = True,
-        stop_words: list[str] = None,
-        k1: float = 1.5,
-        b: float = 0.75,
-        epsilon: float = 0,
-    ) -> None:
-        super().__init__(
-            analyzer=analyzer,
-            ngram_range=ngram_range,
-            normalize=normalize,
-            stop_words=stop_words,
-        )
-
-        self.k1 = k1
-        self.b = b
-        self.epsilon = epsilon
-        self.average_len = None
-
-    def update(self, matrix: csr_matrix) -> csr_matrix:
-        """Update the idf values."""
-        self.tf = (matrix > 0).sum(axis=0)
-        len_documents = (matrix).sum(axis=1)
-        self.average_len = len_documents.mean()
-        self.count = matrix.shape[0]
-
-        self.idf = np.squeeze(
-            a=np.asarray(a=np.log((self.count - self.tf + 0.5) / (self.tf + 0.5) + 1))
-        )
-
-    def _transform(self, matrix: csr_matrix) -> csr_matrix:
-        """Transform a count matrix to a bm25 matrix."""
-        len_documents = (matrix).sum(axis=1)
-        regularization = np.squeeze(
-            a=np.asarray(
-                a=(
-                    self.k1 * (1 - self.b + self.b * (len_documents / self.average_len))
-                ).flatten()
-            )
-        )
-
-        numerator = matrix.copy()
-        denominator = matrix.copy().tocsc()
-        numerator.data = numerator.data * (self.k1 + 1)
-        denominator.data += np.take(a=regularization, indices=denominator.indices)
-        matrix.data = (numerator.data / denominator.tocsr().data) + self.epsilon
-
-        matrix = matrix.multiply(other=self.idf).tocsr()
-        inplace_csr_row_normalize_l2(X=matrix)
-        return matrix
+import numpy as np
+from scipy.sparse import csr_matrix
+from sklearn.utils.sparsefuncs_fast import inplace_csr_row_normalize_l2
+
+from .tfidf_vectorizer import TfIdfVectorizer
+
+
+class BM25Vectorizer(TfIdfVectorizer):
+    """BM25Vectorizer is a class that converts a collection of text documents to a sparse
+    bm25 matrix.
+
+    Parameters
+    ----------
+    analyzer
+        {word, char, char_wb}, default=word.
+        Whether the feature should be made of word n-gram or character n-grams. Option
+        char_wb creates character n-grams only from text inside word boundaries;
+        n-grams at the edges of words are padded with space.
+    ngram_range
+        tuple (min_n, max_n), default=(1, 1).
+        The lower and upper boundary of the range of n-values for different n-grams to
+        be extracted. All values of n such that min_n <= n <= max_n will be used.
+    normalize
+        bool, default=True.
+        Whether to normalize the text before counting. It will lowercase the text and remove
+        punctuation.
+    stop_words
+        list of str, default=None.
+        A list of stop words that will be removed from the text.
+    b
+        The impact of document length normalization.  Default is `0.75`, Higher will
+        penalize longer documents more.
+    k1
+        How quickly the impact of term frequency saturates.  Default is `1.5`, Higher
+        will make term frequency more influential.
+    epsilon
+        Smoothing term. Default is `0`.
+
+    Examples
+    --------
+    >>> from lenlp import sparse
+
+    >>> bm25_vectorizer = sparse.BM25Vectorizer(
+    ...     analyzer="word",
+    ...     normalize=True,
+    ...     stop_words=None,
+    ... )
+
+    >>> x = ["Hello, world!", "How are you?"]
+
+    >>> bm25_vectorizer = bm25_vectorizer.fit(x)
+    >>> matrix = bm25_vectorizer.transform(x)
+    >>> matrix.shape
+    (2, 5)
+
+    >>> len(bm25_vectorizer.vocabulary)
+    5
+
+    >>> matrix = bm25_vectorizer.fit_transform(x)
+    >>> matrix.shape
+    (2, 5)
+
+    """
+
+    def __init__(
+        self,
+        analyzer: str = "word",
+        ngram_range: tuple[int, int] = (1, 1),
+        normalize: bool = True,
+        stop_words: list[str] = None,
+        k1: float = 1.5,
+        b: float = 0.75,
+        epsilon: float = 0,
+    ) -> None:
+        super().__init__(
+            analyzer=analyzer,
+            ngram_range=ngram_range,
+            normalize=normalize,
+            stop_words=stop_words,
+        )
+
+        self.k1 = k1
+        self.b = b
+        self.epsilon = epsilon
+        self.average_len = None
+
+    def update(self, matrix: csr_matrix) -> csr_matrix:
+        """Update the idf values."""
+        self.tf = (matrix > 0).sum(axis=0)
+        len_documents = (matrix).sum(axis=1)
+        self.average_len = len_documents.mean()
+        self.count = matrix.shape[0]
+
+        self.idf = np.squeeze(
+            a=np.asarray(a=np.log((self.count - self.tf + 0.5) / (self.tf + 0.5) + 1))
+        )
+
+    def _transform(self, matrix: csr_matrix) -> csr_matrix:
+        """Transform a count matrix to a bm25 matrix."""
+        len_documents = (matrix).sum(axis=1)
+        regularization = np.squeeze(
+            a=np.asarray(
+                a=(
+                    self.k1 * (1 - self.b + self.b * (len_documents / self.average_len))
+                ).flatten()
+            )
+        )
+
+        numerator = matrix.copy()
+        denominator = matrix.copy().tocsc()
+        numerator.data = numerator.data * (self.k1 + 1)
+        denominator.data += np.take(a=regularization, indices=denominator.indices)
+        matrix.data = (numerator.data / denominator.tocsr().data) + self.epsilon
+
+        matrix = matrix.multiply(other=self.idf).tocsr()
+        inplace_csr_row_normalize_l2(X=matrix)
+        return matrix
```

### Comparing `lenlp-1.0.1/lenlp/sparse/count_vectorizer.py` & `lenlp-1.0.2/lenlp/sparse/count_vectorizer.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-import numpy as np
-from rslenlp import SparseMatrixBuilder
-from scipy.sparse import csr_matrix
-
-__all__ = ["CountVectorizer"]
-
-
-class CountVectorizer:
-    """CountVectorizer is a class that converts a collection of text documents to a sparse
-    matrix.
-
-    Parameters
-    ----------
-    analyzer
-        {word, char, char_wb}, default=word.
-        Whether the feature should be made of word n-gram or character n-grams. Option
-        char_wb creates character n-grams only from text inside word boundaries;
-        n-grams at the edges of words are padded with space.
-    ngram_range
-        tuple (min_n, max_n), default=(1, 1).
-        The lower and upper boundary of the range of n-values for different n-grams to
-        be extracted. All values of n such that min_n <= n <= max_n will be used.
-    normalize
-        bool, default=True.
-        Whether to normalize the text before counting. It will lowercase the text and remove
-        punctuation.
-    stop_words
-        list of str, default=None.
-        A list of stop words that will be removed from the text.
-
-    Examples
-    --------
-    >>> from lenlp import sparse
-
-    >>> count_vectorizer = sparse.CountVectorizer(
-    ...     analyzer="word",
-    ...     normalize=True,
-    ...     stop_words=None,
-    ... )
-
-    >>> x = ["Hello, world!", "How are you?"]
-
-    >>> count_vectorizer = count_vectorizer.fit(x)
-
-    >>> matrix = count_vectorizer.transform(x)
-    >>> matrix.shape
-    (2, 5)
-
-    >>> matrix.toarray()
-    array([[1, 1, 0, 0, 0],
-           [0, 0, 1, 1, 1]], dtype=int16)
-
-    >>> len(count_vectorizer.vocabulary)
-    5
-
-    >>> matrix = count_vectorizer.fit_transform(x)
-    >>> matrix.shape
-    (2, 5)
-
-    """
-
-    def __init__(
-        self,
-        analyzer: str = "word",
-        ngram_range: tuple[int, int] = (1, 1),
-        normalize: bool = True,
-        stop_words: list[str] = None,
-    ) -> None:
-        assert analyzer in ("word", "char", "char_wb")
-
-        self.sparse_matrix = SparseMatrixBuilder(
-            analyzer=analyzer,
-            n_sizes=list(range(ngram_range[0], ngram_range[1] + 1)),
-            normalize=normalize,
-            stop_words=stop_words,
-        )
-
-        self.fitted = False
-
-    @property
-    def vocabulary(self) -> dict[str, int]:
-        """Get the vocabulary of the CountVectorizer object."""
-        return self.sparse_matrix.get_vocab()
-
-    def fit(self, raw_documents: list[str]) -> None:
-        """Learn the vocabulary dictionary and return the CountVectorizer object."""
-        self.fitted = True
-        self.sparse_matrix.fit(raw_documents)
-        return self
-
-    def transform(self, raw_documents: list[str]) -> csr_matrix:
-        """Transform documents to document-term matrix."""
-        if not self.fitted:
-            raise ValueError("Call fit method before calling transform method.")
-        values, row_indices, column_indices = self.sparse_matrix.transform(
-            raw_documents
-        )
-        return csr_matrix(
-            arg1=(values, (row_indices, column_indices)),
-            shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
-            dtype=np.int16,
-        )
-
-    def fit_transform(self, raw_documents: list[str]) -> csr_matrix:
-        """Learn the vocabulary dictionary and return the CountVectorizer object."""
-        self.fitted = True
-        values, row_indices, column_indices = self.sparse_matrix.fit_transform(
-            raw_documents
-        )
-        return csr_matrix(
-            arg1=(values, (row_indices, column_indices)),
-            shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
-            dtype=np.int16,
-        )
+import numpy as np
+from rslenlp import SparseMatrixBuilder
+from scipy.sparse import csr_matrix
+
+__all__ = ["CountVectorizer"]
+
+
+class CountVectorizer:
+    """CountVectorizer is a class that converts a collection of text documents to a sparse
+    matrix.
+
+    Parameters
+    ----------
+    analyzer
+        {word, char, char_wb}, default=word.
+        Whether the feature should be made of word n-gram or character n-grams. Option
+        char_wb creates character n-grams only from text inside word boundaries;
+        n-grams at the edges of words are padded with space.
+    ngram_range
+        tuple (min_n, max_n), default=(1, 1).
+        The lower and upper boundary of the range of n-values for different n-grams to
+        be extracted. All values of n such that min_n <= n <= max_n will be used.
+    normalize
+        bool, default=True.
+        Whether to normalize the text before counting. It will lowercase the text and remove
+        punctuation.
+    stop_words
+        list of str, default=None.
+        A list of stop words that will be removed from the text.
+
+    Examples
+    --------
+    >>> from lenlp import sparse
+
+    >>> count_vectorizer = sparse.CountVectorizer(
+    ...     analyzer="word",
+    ...     normalize=True,
+    ...     stop_words=None,
+    ... )
+
+    >>> x = ["Hello, world!", "How are you?"]
+
+    >>> count_vectorizer = count_vectorizer.fit(x)
+
+    >>> matrix = count_vectorizer.transform(x)
+    >>> matrix.shape
+    (2, 5)
+
+    >>> matrix.toarray()
+    array([[1, 1, 0, 0, 0],
+           [0, 0, 1, 1, 1]], dtype=int16)
+
+    >>> len(count_vectorizer.vocabulary)
+    5
+
+    >>> matrix = count_vectorizer.fit_transform(x)
+    >>> matrix.shape
+    (2, 5)
+
+    """
+
+    def __init__(
+        self,
+        analyzer: str = "word",
+        ngram_range: tuple[int, int] = (1, 1),
+        normalize: bool = True,
+        stop_words: list[str] = None,
+    ) -> None:
+        assert analyzer in ("word", "char", "char_wb")
+
+        self.sparse_matrix = SparseMatrixBuilder(
+            analyzer=analyzer,
+            n_sizes=list(range(ngram_range[0], ngram_range[1] + 1)),
+            normalize=normalize,
+            stop_words=stop_words,
+        )
+
+        self.fitted = False
+
+    @property
+    def vocabulary(self) -> dict[str, int]:
+        """Get the vocabulary of the CountVectorizer object."""
+        return self.sparse_matrix.get_vocab()
+
+    def fit(self, raw_documents: list[str]) -> None:
+        """Learn the vocabulary dictionary and return the CountVectorizer object."""
+        self.fitted = True
+        self.sparse_matrix.fit(raw_documents)
+        return self
+
+    def transform(self, raw_documents: list[str]) -> csr_matrix:
+        """Transform documents to document-term matrix."""
+        if not self.fitted:
+            raise ValueError("Call fit method before calling transform method.")
+        values, row_indices, column_indices = self.sparse_matrix.transform(
+            raw_documents
+        )
+        return csr_matrix(
+            arg1=(values, (row_indices, column_indices)),
+            shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
+            dtype=np.int16,
+        )
+
+    def fit_transform(self, raw_documents: list[str]) -> csr_matrix:
+        """Learn the vocabulary dictionary and return the CountVectorizer object."""
+        self.fitted = True
+        values, row_indices, column_indices = self.sparse_matrix.fit_transform(
+            raw_documents
+        )
+        return csr_matrix(
+            arg1=(values, (row_indices, column_indices)),
+            shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
+            dtype=np.int16,
+        )
```

### Comparing `lenlp-1.0.1/lenlp/sparse/tfidf_vectorizer.py` & `lenlp-1.0.2/lenlp/sparse/tfidf_vectorizer.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import numpy as np
-from scipy.sparse import csr_matrix
-from sklearn.utils.sparsefuncs_fast import inplace_csr_row_normalize_l2
-
-from .count_vectorizer import CountVectorizer
-
-
-class TfIdfVectorizer(CountVectorizer):
-    """TfIdfVectorizer is a class that converts a collection of text documents to a sparse
-    tfidf matrix.
-
-    Parameters
-    ----------
-    analyzer
-        {word, char, char_wb}, default=word.
-        Whether the feature should be made of word n-gram or character n-grams. Option
-        char_wb creates character n-grams only from text inside word boundaries;
-        n-grams at the edges of words are padded with space.
-    ngram_range
-        tuple (min_n, max_n), default=(1, 1).
-        The lower and upper boundary of the range of n-values for different n-grams to
-        be extracted. All values of n such that min_n <= n <= max_n will be used.
-    normalize
-        bool, default=True.
-        Whether to normalize the text before counting. It will lowercase the text and remove
-        punctuation.
-    stop_words
-        list of str, default=None.
-        A list of stop words that will be removed from the text.
-
-    Examples
-    --------
-    >>> from lenlp import sparse
-
-    >>> tfidf_vectorizer = sparse.TfIdfVectorizer(
-    ...     analyzer="word",
-    ...     normalize=True,
-    ...     stop_words=None,
-    ... )
-
-    >>> x = ["Hello, world!", "How are you?"]
-
-    >>> tfidf_vectorizer = tfidf_vectorizer.fit(x)
-    >>> matrix = tfidf_vectorizer.transform(x)
-    >>> matrix.shape
-    (2, 5)
-
-    >>> len(tfidf_vectorizer.vocabulary)
-    5
-
-    >>> matrix = tfidf_vectorizer.fit_transform(x)
-    >>> matrix.shape
-    (2, 5)
-
-    """
-
-    def __init__(
-        self,
-        analyzer: str = "word",
-        ngram_range: tuple[int, int] = (1, 1),
-        normalize: bool = True,
-        stop_words: list[str] = None,
-    ) -> None:
-        super().__init__(
-            analyzer=analyzer,
-            ngram_range=ngram_range,
-            normalize=normalize,
-            stop_words=stop_words,
-        )
-
-        self.idf = None
-
-    def fit(self, raw_documents: list[str]) -> None:
-        matrix = super().fit_transform(raw_documents=raw_documents)
-        self.update(matrix=matrix)
-        return self
-
-    def update(self, matrix: csr_matrix) -> csr_matrix:
-        """Update the idf values."""
-        tf = (matrix > 0).sum(axis=0)
-        self.idf = (
-            np.squeeze(a=np.asarray(a=np.log((matrix.shape[0] + 1.0) / (tf + 1.0)))) + 1
-        )
-
-    def _transform(self, matrix: csr_matrix) -> csr_matrix:
-        """Transform a count matrix to a bm25 matrix."""
-        matrix.data *= np.take(
-            a=self.idf,
-            indices=matrix.indices,
-        )
-
-        inplace_csr_row_normalize_l2(X=matrix)
-        return matrix
-
-    def transform(self, raw_documents: list[str]) -> csr_matrix:
-        """Transform documents to document-term matrix."""
-        values, row_indices, column_indices = self.sparse_matrix.transform(
-            raw_documents
-        )
-        return self._transform(
-            matrix=csr_matrix(
-                arg1=(values, (row_indices, column_indices)),
-                shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
-                dtype=np.float64,
-            )
-        )
-
-    def fit_transform(self, raw_documents: list[str]) -> csr_matrix:
-        """Learn the vocabulary dictionary and return the CountVectorizer object."""
-        values, row_indices, column_indices = self.sparse_matrix.fit_transform(
-            raw_documents
-        )
-
-        matrix = csr_matrix(
-            arg1=(values, (row_indices, column_indices)),
-            shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
-            dtype=np.float64,
-        )
-
-        self.update(matrix=matrix)
-
-        return self._transform(
-            matrix=matrix,
-        )
+import numpy as np
+from scipy.sparse import csr_matrix
+from sklearn.utils.sparsefuncs_fast import inplace_csr_row_normalize_l2
+
+from .count_vectorizer import CountVectorizer
+
+
+class TfIdfVectorizer(CountVectorizer):
+    """TfIdfVectorizer is a class that converts a collection of text documents to a sparse
+    tfidf matrix.
+
+    Parameters
+    ----------
+    analyzer
+        {word, char, char_wb}, default=word.
+        Whether the feature should be made of word n-gram or character n-grams. Option
+        char_wb creates character n-grams only from text inside word boundaries;
+        n-grams at the edges of words are padded with space.
+    ngram_range
+        tuple (min_n, max_n), default=(1, 1).
+        The lower and upper boundary of the range of n-values for different n-grams to
+        be extracted. All values of n such that min_n <= n <= max_n will be used.
+    normalize
+        bool, default=True.
+        Whether to normalize the text before counting. It will lowercase the text and remove
+        punctuation.
+    stop_words
+        list of str, default=None.
+        A list of stop words that will be removed from the text.
+
+    Examples
+    --------
+    >>> from lenlp import sparse
+
+    >>> tfidf_vectorizer = sparse.TfIdfVectorizer(
+    ...     analyzer="word",
+    ...     normalize=True,
+    ...     stop_words=None,
+    ... )
+
+    >>> x = ["Hello, world!", "How are you?"]
+
+    >>> tfidf_vectorizer = tfidf_vectorizer.fit(x)
+    >>> matrix = tfidf_vectorizer.transform(x)
+    >>> matrix.shape
+    (2, 5)
+
+    >>> len(tfidf_vectorizer.vocabulary)
+    5
+
+    >>> matrix = tfidf_vectorizer.fit_transform(x)
+    >>> matrix.shape
+    (2, 5)
+
+    """
+
+    def __init__(
+        self,
+        analyzer: str = "word",
+        ngram_range: tuple[int, int] = (1, 1),
+        normalize: bool = True,
+        stop_words: list[str] = None,
+    ) -> None:
+        super().__init__(
+            analyzer=analyzer,
+            ngram_range=ngram_range,
+            normalize=normalize,
+            stop_words=stop_words,
+        )
+
+        self.idf = None
+
+    def fit(self, raw_documents: list[str]) -> None:
+        matrix = super().fit_transform(raw_documents=raw_documents)
+        self.update(matrix=matrix)
+        return self
+
+    def update(self, matrix: csr_matrix) -> csr_matrix:
+        """Update the idf values."""
+        tf = (matrix > 0).sum(axis=0)
+        self.idf = (
+            np.squeeze(a=np.asarray(a=np.log((matrix.shape[0] + 1.0) / (tf + 1.0)))) + 1
+        )
+
+    def _transform(self, matrix: csr_matrix) -> csr_matrix:
+        """Transform a count matrix to a bm25 matrix."""
+        matrix.data *= np.take(
+            a=self.idf,
+            indices=matrix.indices,
+        )
+
+        inplace_csr_row_normalize_l2(X=matrix)
+        return matrix
+
+    def transform(self, raw_documents: list[str]) -> csr_matrix:
+        """Transform documents to document-term matrix."""
+        values, row_indices, column_indices = self.sparse_matrix.transform(
+            raw_documents
+        )
+        return self._transform(
+            matrix=csr_matrix(
+                arg1=(values, (row_indices, column_indices)),
+                shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
+                dtype=np.float64,
+            )
+        )
+
+    def fit_transform(self, raw_documents: list[str]) -> csr_matrix:
+        """Learn the vocabulary dictionary and return the CountVectorizer object."""
+        values, row_indices, column_indices = self.sparse_matrix.fit_transform(
+            raw_documents
+        )
+
+        matrix = csr_matrix(
+            arg1=(values, (row_indices, column_indices)),
+            shape=(len(raw_documents), self.sparse_matrix.get_num_cols()),
+            dtype=np.float64,
+        )
+
+        self.update(matrix=matrix)
+
+        return self._transform(
+            matrix=matrix,
+        )
```

### Comparing `lenlp-1.0.1/lenlp.egg-info/SOURCES.txt` & `lenlp-1.0.2/lenlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.1/setup.py` & `lenlp-1.0.2/setup.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import setuptools
-from setuptools_rust import Binding, RustExtension
-
-from lenlp.__version__ import __version__
-
-base_packages = ["scikit-learn  >= 1.5.0", "scipy >= 1.13.1"]
-dev = ["maturin >= 1.5.1", "pytest-cov >= 5.0.0", "pytest >= 7.4.4", "ruff >= 0.1.15"]
-
-
-setuptools.setup(
-    name="lenlp",
-    version=f"{__version__}",
-    author="Raphael Sourty",
-    author_email="raphael.sourty@gmail.com",
-    long_description_content_type="text/markdown",
-    url="https://github.com/raphaelsty/lenlp",
-    download_url="https://github.com/raphaelsty/lenlp/archive/v_01.tar.gz",
-    keywords=[],
-    packages=setuptools.find_packages(),
-    install_requires=base_packages,
-    extras_require={"dev": base_packages + dev},
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Rust",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.8",
-    rust_extensions=[RustExtension("rslenlp", binding=Binding.PyO3)],
-    setup_requires=["setuptools-rust>=1.9.0"],
-)
+import setuptools
+from setuptools_rust import Binding, RustExtension
+
+from lenlp.__version__ import __version__
+
+base_packages = ["scikit-learn  >= 1.5.0", "scipy >= 1.13.1"]
+dev = ["maturin >= 1.5.1", "pytest-cov >= 5.0.0", "pytest >= 7.4.4", "ruff >= 0.1.15"]
+
+
+setuptools.setup(
+    name="lenlp",
+    version=f"{__version__}",
+    author="Raphael Sourty",
+    author_email="raphael.sourty@gmail.com",
+    long_description_content_type="text/markdown",
+    url="https://github.com/raphaelsty/lenlp",
+    download_url="https://github.com/raphaelsty/lenlp/archive/v_01.tar.gz",
+    keywords=[],
+    packages=setuptools.find_packages(),
+    install_requires=base_packages,
+    extras_require={"dev": base_packages + dev},
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Rust",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.8",
+    rust_extensions=[RustExtension("rslenlp", binding=Binding.PyO3)],
+    setup_requires=["setuptools-rust>=1.9.0"],
+)
```

