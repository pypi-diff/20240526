# Comparing `tmp/arraylake-0.9.7.tar.gz` & `tmp/arraylake-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraylake-0.9.7.tar", max compression
+gzip compressed data, was "arraylake-0.9.8.tar", max compression
```

## Comparing `arraylake-0.9.7.tar` & `arraylake-0.9.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      653 2024-05-01 17:25:24.438752 arraylake-0.9.7/README.md
--rw-r--r--   0        0        0      416 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/__init__.py
--rw-r--r--   0        0        0       63 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/__main__.py
--rw-r--r--   0        0        0    22304 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/api_utils.py
--rw-r--r--   0        0        0     9770 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/asyn.py
--rw-r--r--   0        0        0     4001 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/__init__.py
--rw-r--r--   0        0        0     4056 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/abc.py
--rw-r--r--   0        0        0     9973 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/base_chunkstore.py
--rw-r--r--   0        0        0     6664 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/fsspec_chunkstore.py
--rw-r--r--   0        0        0     1862 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/fsspec_compat.py
--rw-r--r--   0        0        0    10893 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/chunkstore/s3chunkstore.py
--rw-r--r--   0        0        0        0 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/__init__.py
--rw-r--r--   0        0        0     4915 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/auth.py
--rw-r--r--   0        0        0     4741 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/config.py
--rw-r--r--   0        0        0     1615 2024-05-01 17:25:24.438752 arraylake-0.9.7/arraylake/cli/main.py
--rw-r--r--   0        0        0     5653 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/cli/repo.py
--rw-r--r--   0        0        0     4860 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/cli/utils.py
--rw-r--r--   0        0        0    21140 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/client.py
--rw-r--r--   0        0        0     8181 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/commits.py
--rw-r--r--   0        0        0     2976 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/config.py
--rw-r--r--   0        0        0      176 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/config.yaml
--rw-r--r--   0        0        0     5221 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/diagnostics.py
--rw-r--r--   0        0        0      345 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/exceptions.py
--rw-r--r--   0        0        0      194 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/experimental.py
--rw-r--r--   0        0        0     1082 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/log_util.py
--rw-r--r--   0        0        0      261 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/metastore/__init__.py
--rw-r--r--   0        0        0    15638 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/metastore/abc.py
--rw-r--r--   0        0        0    23366 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/metastore/http_metastore.py
--rw-r--r--   0        0        0        0 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/py.typed
--rw-r--r--   0        0        0    92130 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/repo.py
--rw-r--r--   0        0        0     7180 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/retrier.py
--rw-r--r--   0        0        0     1526 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/strategies.py
--rw-r--r--   0        0        0     4776 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/token.py
--rw-r--r--   0        0        0    28691 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/types.py
--rw-r--r--   0        0        0    17216 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/virtual.py
--rw-r--r--   0        0        0      851 2024-05-01 17:25:24.442752 arraylake-0.9.7/arraylake/zarr_util.py
--rw-r--r--   0        0        0     5405 2024-05-01 17:25:42.270750 arraylake-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 arraylake-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0      653 2024-05-26 19:47:13.845913 arraylake-0.9.8/README.md
+-rw-r--r--   0        0        0      416 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/__main__.py
+-rw-r--r--   0        0        0    22304 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/api_utils.py
+-rw-r--r--   0        0        0     9770 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/asyn.py
+-rw-r--r--   0        0        0     4001 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/chunkstore/__init__.py
+-rw-r--r--   0        0        0     4056 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/chunkstore/abc.py
+-rw-r--r--   0        0        0     9973 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/chunkstore/base_chunkstore.py
+-rw-r--r--   0        0        0     6664 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/chunkstore/fsspec_chunkstore.py
+-rw-r--r--   0        0        0     1862 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/chunkstore/fsspec_compat.py
+-rw-r--r--   0        0        0    10893 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/chunkstore/s3chunkstore.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/cli/__init__.py
+-rw-r--r--   0        0        0     4915 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/cli/auth.py
+-rw-r--r--   0        0        0     4741 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/cli/config.py
+-rw-r--r--   0        0        0     1615 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/cli/main.py
+-rw-r--r--   0        0        0     5653 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/cli/repo.py
+-rw-r--r--   0        0        0     4860 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/cli/utils.py
+-rw-r--r--   0        0        0    21140 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/client.py
+-rw-r--r--   0        0        0     8187 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/commits.py
+-rw-r--r--   0        0        0     2976 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/config.py
+-rw-r--r--   0        0        0      176 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/config.yaml
+-rw-r--r--   0        0        0     5221 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/diagnostics.py
+-rw-r--r--   0        0        0      345 2024-05-26 19:47:13.845913 arraylake-0.9.8/arraylake/exceptions.py
+-rw-r--r--   0        0        0      194 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/experimental.py
+-rw-r--r--   0        0        0     1082 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/log_util.py
+-rw-r--r--   0        0        0      261 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/metastore/__init__.py
+-rw-r--r--   0        0        0    15638 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/metastore/abc.py
+-rw-r--r--   0        0        0    23366 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/metastore/http_metastore.py
+-rw-r--r--   0        0        0        0 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/py.typed
+-rw-r--r--   0        0        0    94024 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/repo.py
+-rw-r--r--   0        0        0     7180 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/retrier.py
+-rw-r--r--   0        0        0     1526 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/strategies.py
+-rw-r--r--   0        0        0     4776 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/token.py
+-rw-r--r--   0        0        0    28691 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/types.py
+-rw-r--r--   0        0        0    17216 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/virtual.py
+-rw-r--r--   0        0        0      851 2024-05-26 19:47:13.849913 arraylake-0.9.8/arraylake/zarr_util.py
+-rw-r--r--   0        0        0     5405 2024-05-26 19:47:31.897712 arraylake-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     2515 1970-01-01 00:00:00.000000 arraylake-0.9.8/PKG-INFO
```

### Comparing `arraylake-0.9.7/README.md` & `arraylake-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/api_utils.py` & `arraylake-0.9.8/arraylake/api_utils.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/asyn.py` & `arraylake-0.9.8/arraylake/asyn.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/chunkstore/__init__.py` & `arraylake-0.9.8/arraylake/chunkstore/__init__.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/chunkstore/abc.py` & `arraylake-0.9.8/arraylake/chunkstore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/chunkstore/base_chunkstore.py` & `arraylake-0.9.8/arraylake/chunkstore/base_chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/chunkstore/fsspec_chunkstore.py` & `arraylake-0.9.8/arraylake/chunkstore/fsspec_chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/chunkstore/fsspec_compat.py` & `arraylake-0.9.8/arraylake/chunkstore/fsspec_compat.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/chunkstore/s3chunkstore.py` & `arraylake-0.9.8/arraylake/chunkstore/s3chunkstore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/cli/auth.py` & `arraylake-0.9.8/arraylake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/cli/config.py` & `arraylake-0.9.8/arraylake/cli/config.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/cli/main.py` & `arraylake-0.9.8/arraylake/cli/main.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/cli/repo.py` & `arraylake-0.9.8/arraylake/cli/repo.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/cli/utils.py` & `arraylake-0.9.8/arraylake/cli/utils.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/client.py` & `arraylake-0.9.8/arraylake/client.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/commits.py` & `arraylake-0.9.8/arraylake/commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,26 +211,26 @@
             console.print(f"Date:   {commit.commit_time}")
             console.print(Padding(commit.message, (1, 4)))
 
     def _repr_html_(self):
         html = """<ul style="list-style-type: none; margin: 0; padding: 0;">\n"""
 
         def row(col1: str, col2: str) -> str:
-            return f"   <tr><td style='text-align:right'>{col1}</td><td style='text-align:left'>{col2}</td></tr>"
+            return f"""   <tr><td style="text-align:right">{col1}</td><td style="text-align:left">{col2}</td></tr>"""
 
         commit_tags = invert_mapping(self.commit_data.tags)
         for commit in self:
             html += """ <li>\n  <table style="border: 1px dashed grey">\n"""
             html += row("Commit ID", "<b>" + escape(str(commit.id)) + "</b>")
             html += row("Author", escape(commit.author_entry()))
             html += row("Date", escape(commit.commit_time.isoformat()))
 
             tags = commit_tags[commit.id]
             if tags:
                 html += row("Tags", ", ".join(tags))
-            html += "  </table>\n"
+            html += "\n  </table>\n"
             message = escape(commit.message).replace("\n", "<br />")
             html += f"""  <p style="padding: 1em 2em;">{message}</p>\n"""
             html += " </li>\n"
         html += "</ul>\n"
 
         return html
```

### Comparing `arraylake-0.9.7/arraylake/config.py` & `arraylake-0.9.8/arraylake/config.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/diagnostics.py` & `arraylake-0.9.8/arraylake/diagnostics.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/log_util.py` & `arraylake-0.9.8/arraylake/log_util.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/metastore/abc.py` & `arraylake-0.9.8/arraylake/metastore/abc.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/metastore/http_metastore.py` & `arraylake-0.9.8/arraylake/metastore/http_metastore.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/repo.py` & `arraylake-0.9.8/arraylake/repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1450,15 +1450,15 @@
             )
             for path, loc in locations.items()
         }
 
     def _validate_fs_config_for_uri(self, uri: str) -> FSConfig:
         fs_config = self.chunkstore._get_fs_config()
         if not uri.startswith(fs_config.protocol + "://"):
-            raise ValueError(f"Unsupported URI for {fs_config.protocol}-chunkstore: {uri}")
+            raise ValueError(f"Expected uri to start with: '{fs_config.protocol}://', received: {uri!r}")
         return fs_config
 
     @_write_op
     async def add_virtual_grib(self, grib_uri: str, path: Path, **kwargs) -> None:
         """Add a virtual GRIB2 dataset to the repo.
 
         If the GRIB file contains multiple messages, this method will attempt to
@@ -1479,14 +1479,46 @@
         kerchunk_refs = scan_grib2(fs_config, grib_uri, **kwargs)
         meta_docs, chunk_locations, inlined_refs = reformat_kerchunk_refs(kerchunk_refs, path)
         await async_gather(
             self._set_docs(meta_docs), self._set_chunks(inlined_refs), self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations))
         )
 
     @_write_op
+    async def add_kerchunk_references(self, refs: dict[str, Any] | str, path: Path, **kwargs) -> None:
+        """Add a kerchunk references to the repo.
+
+        Args:
+            refs: A dictionary of kerchunk references or a path to a JSON file.
+            path: The path within the repo where the virtual dataset should be created.
+            kwargs: Additional arguments to pass to `fsspec.open` (only used when `refs` is a path to a JSON file).
+
+        Note: Kerchunk version 1 is supported unless the `templates` or `gen` keys are present.
+        """
+        if isinstance(refs, str):
+            import fsspec
+
+            with fsspec.open(refs, "rb", **kwargs) as f:
+                refs = json.load(f)
+
+        assert isinstance(refs, dict)
+        if refs.get("templates", {}):
+            raise NotImplementedError("Kerchunk templates key not yet supported")
+        if refs.get("gen", {}):
+            raise NotImplementedError("Kerchunk gen key not yet supported")
+
+        if "refs" in refs:
+            refs = refs["refs"]
+
+        assert isinstance(refs, dict)
+        meta_docs, chunk_locations, inlined_refs = reformat_kerchunk_refs(refs, path)
+        await async_gather(
+            self._set_docs(meta_docs), self._set_chunks(inlined_refs), self._set_chunk_refs(self._chunk_locations_to_refs(chunk_locations))
+        )
+
+    @_write_op
     async def add_virtual_netcdf(self, netcdf_uri: str, path: Path, **kwargs) -> None:
         """Add a virtual Netcdf dataset to the repo.
 
         Args:
             netcdf_uri: The path to the netCDF file. Only `s3://` and `gs://` URIs are supported.
               Both netCDF4 and netCDF3 files are supported.
             path: The path within the repo where the virtual dataset should be created.
@@ -1853,14 +1885,24 @@
         return self._synchronize(self._arepo.tags)
 
     @property
     def branches(self):
         """Returns a list of branch names."""
         return self._synchronize(self._arepo.branches)
 
+    def add_kerchunk_references(self, refs: dict[str, Any] | str, path: Path, **kwargs) -> None:
+        """Add a kerchunk references to the repo.
+
+        Args:
+            refs: A dictionary of kerchunk references.
+            path: The path within the repo where the virtual dataset should be created.
+            kwargs: Additional arguments to pass to `fsspec.open` (only used when `refs` is a path to a JSON file).
+        """
+        self._synchronize(self._arepo.add_kerchunk_references, refs, path, **kwargs)
+
     def add_virtual_grib(self, grib_uri: str, path: Path) -> None:
         """Add a virtual GRIB2 dataset to the repo.
 
         Args:
             path: The path within the repo where the virtual dataset should be created.
             grib_uri: The path to the GRIB2 file. Only `s3://` or `gs://` URIs are supported at the moment.
         """
```

### Comparing `arraylake-0.9.7/arraylake/retrier.py` & `arraylake-0.9.8/arraylake/retrier.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/strategies.py` & `arraylake-0.9.8/arraylake/strategies.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/token.py` & `arraylake-0.9.8/arraylake/token.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/types.py` & `arraylake-0.9.8/arraylake/types.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/virtual.py` & `arraylake-0.9.8/arraylake/virtual.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/arraylake/zarr_util.py` & `arraylake-0.9.8/arraylake/zarr_util.py`

 * *Files identical despite different names*

### Comparing `arraylake-0.9.7/pyproject.toml` & `arraylake-0.9.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "arraylake"
-version = "0.9.7"  # placeholder
+version = "0.9.8"  # placeholder
 description = "Python client for ArrayLake"
 authors = ["Joe Hamman <joe@earthmover.io>"]
 readme = "README.md"
 packages = [{include = "arraylake"}]
 
 [[tool.poetry.source]]
 name = "pytorch-cpu-src"
```

### Comparing `arraylake-0.9.7/PKG-INFO` & `arraylake-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraylake
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python client for ArrayLake
 Author: Joe Hamman
 Author-email: joe@earthmover.io
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arraylake Version: 0.9.7 Summary: Python client for
+Metadata-Version: 2.1 Name: arraylake Version: 0.9.8 Summary: Python client for
 ArrayLake Author: Joe Hamman Author-email: joe@earthmover.io Requires-Python:
 >=3.10,<3.13 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Provides-
 Extra: grib Provides-Extra: virtual Provides-Extra: widgets Provides-Extra:
 xarray Requires-Dist: aiobotocore[boto3] (>=2.4.0,<3.0.0) Requires-Dist:
 aioitertools (>=0.11.0,<0.12.0) Requires-Dist: boto3 (>=1.24,<2.0) Requires-
```

