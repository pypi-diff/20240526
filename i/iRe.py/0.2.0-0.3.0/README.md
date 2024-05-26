# Comparing `tmp/iRe.py-0.2.0.tar.gz` & `tmp/iRe.py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iRe.py-0.2.0.tar", last modified: Wed May 22 04:44:00 2024, max compression
+gzip compressed data, was "iRe.py-0.3.0.tar", last modified: Sun May 26 13:35:03 2024, max compression
```

## Comparing `iRe.py-0.2.0.tar` & `iRe.py-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:44:00.702634 iRe.py-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-22 04:43:45.000000 iRe.py-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      920 2024-05-22 04:44:00.701634 iRe.py-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-22 04:43:45.000000 iRe.py-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:44:00.700634 iRe.py-0.2.0/iRe.py.egg-info/
--rw-r--r--   0 root         (0) root         (0)      920 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      195 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-05-22 04:44:00.000000 iRe.py-0.2.0/iRe.py.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 04:44:00.701634 iRe.py-0.2.0/ire/
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/dvc.py
--rw-rw-rw-   0 root         (0) root         (0)     2613 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/git.py
--rw-rw-rw-   0 root         (0) root         (0)    10790 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/ire.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/md.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-22 04:43:45.000000 iRe.py-0.2.0/ire/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 04:44:00.702634 iRe.py-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-22 04:43:45.000000 iRe.py-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 13:35:03.355584 iRe.py-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-26 13:34:46.000000 iRe.py-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-26 13:35:03.354583 iRe.py-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-05-26 13:34:46.000000 iRe.py-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 13:35:03.352583 iRe.py-0.3.0/iRe.py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      920 2024-05-26 13:35:03.000000 iRe.py-0.3.0/iRe.py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-26 13:35:03.000000 iRe.py-0.3.0/iRe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-26 13:35:03.000000 iRe.py-0.3.0/iRe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2024-05-26 13:35:03.000000 iRe.py-0.3.0/iRe.py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-05-26 13:35:03.000000 iRe.py-0.3.0/iRe.py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-26 13:35:03.354583 iRe.py-0.3.0/ire/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-26 13:34:46.000000 iRe.py-0.3.0/ire/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      790 2024-05-26 13:34:46.000000 iRe.py-0.3.0/ire/dvc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-05-26 13:34:46.000000 iRe.py-0.3.0/ire/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    12107 2024-05-26 13:34:46.000000 iRe.py-0.3.0/ire/ire.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-05-26 13:34:46.000000 iRe.py-0.3.0/ire/md.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-26 13:34:46.000000 iRe.py-0.3.0/ire/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-26 13:35:03.355584 iRe.py-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-26 13:34:46.000000 iRe.py-0.3.0/setup.py
```

### Comparing `iRe.py-0.2.0/LICENSE` & `iRe.py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iRe.py-0.2.0/PKG-INFO` & `iRe.py-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRe.py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.
 Home-page: https://gitlab.com/runsascoded/ire/py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: plotly
```

### Comparing `iRe.py-0.2.0/README.md` & `iRe.py-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `iRe.py-0.2.0/iRe.py.egg-info/PKG-INFO` & `iRe.py-0.3.0/iRe.py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iRe.py
-Version: 0.2.0
+Version: 0.3.0
 Summary: Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.
 Home-page: https://gitlab.com/runsascoded/ire/py
 Author: Ryan Williams
 Author-email: ryan@runsascoded.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: plotly
```

### Comparing `iRe.py-0.2.0/ire/dvc.py` & `iRe.py-0.3.0/ire/dvc.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.2.0/ire/git.py` & `iRe.py-0.3.0/ire/git.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from ire.utils import run
 
 
 def git_has_staged_changes():
     return not check('git', 'diff', '--cached', '--quiet', 'HEAD', log=None)
 
 
+def git_staged_paths():
+    return process.lines('git', 'diff', '--cached', '--name-only', 'HEAD', log=None)
+
+
 def git_root():
     return process.line('git', 'rev-parse', '--show-toplevel', log=None)
 
 
 def current_sha():
     return process.line('git', 'rev-parse', '--short', 'HEAD', log=None)
 
@@ -27,28 +31,27 @@
 
 
 @dataclass
 class CommitConfig:
     allow_existing_staged_changes: bool = False
     verbose: bool = False
 
-    def __call__(self, path):
-        self.commit(path)
+    def __call__(self, path, staged_paths: list[str] | None = None):
+        self.commit(path, staged_paths=staged_paths)
 
-    def commit(self, path):
-        if self.allow_existing_staged_changes or not git_has_staged_changes():
+    def commit(self, path, staged_paths: list[str] | None = None):
+        if self.allow_existing_staged_changes or not (git_has_staged_changes() if staged_paths is None else bool(staged_paths)):
             run('git', 'add', '-f', path, verbose=self.verbose)
             if git_has_staged_changes():
                 run('git', 'commit', '-m', f'iRe: add {path}', verbose=self.verbose)
             else:
                 err(f"iRe: {path} appears unchanged, `git add` had no effect")
         else:
             raise RuntimeError(
-                "Refusing to Git commit given existing staged changes (passing `git=commit!` will add the new "
-                "table to staged changes, and commit)"
+                "Refusing to Git commit given existing staged changes; pass `git=commit!` to add this table to existing staged changes, and commit)"
             )
 
 
 @dataclass
 class PushConfig:
     commit: Optional[CommitConfig] = None
     remote: Optional[str] = None
@@ -62,24 +65,29 @@
 GitConfig = Union[
     Literal['add', 'commit', 'commit!', 'push'],
     CommitConfig,
     PushConfig,
 ]
 
 
-def process_git_config(git: Optional[GitConfig], path: str, verbose: bool = False):
+def process_git_config(
+        git: Optional[GitConfig],
+        path: str,
+        verbose: bool = False,
+        staged_paths: list[str] | None = None,
+):
     """Process the git config: add, commit, or push the file `path`."""
     git_configs = {
         'commit': CommitConfig(verbose=verbose),
         'commit!': CommitConfig(allow_existing_staged_changes=True, verbose=verbose),
         'push': PushConfig(commit=CommitConfig(verbose=verbose), verbose=verbose),
         'push!': PushConfig(commit=CommitConfig(allow_existing_staged_changes=True, verbose=verbose), verbose=verbose),
     }
     if isinstance(git, str) and git in git_configs:
         git = git_configs[git]
     if git == 'add':
         run('git', 'add', '-f', path, verbose=verbose)
     elif isinstance(git, CommitConfig):
-        git.commit(path)
+        git.commit(path, staged_paths=staged_paths)
     elif isinstance(git, PushConfig):
-        git.commit(path)
+        git.commit(path, staged_paths=staged_paths)
         run('git', 'push', verbose=verbose)
```

### Comparing `iRe.py-0.2.0/ire/ire.py` & `iRe.py-0.3.0/ire/ire.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,44 +7,52 @@
 from typing import Literal, Optional, Union, TypeVar, Callable, Type
 
 import pandas as pd
 from IPython.display import display, HTML, Image
 from utz import err
 
 from ire.dvc import DvcConfig, is_dvc_repo, process_dvc_config
-from ire.git import GitConfig, has_unpushed_commits, process_git_config
+from ire.git import GitConfig, has_unpushed_commits, process_git_config, git_staged_paths
 from ire.utils import md5_file, run
 
 
 DEFAULT_ARTIFACTS_DIR = ".ire"
 METADATA_KEY = 'iRe'
+IRE_NO_GIT_PUSH = 'IRE_NO_GIT_PUSH'
 
 ParquetEngine = Literal['fastparquet', 'pyarrow', 'auto'] | None
-Fmts = dict[str | Type, str]
+ColFmts = dict[str | Type, str]
+Align = Literal['left', 'center', 'right']
+ColAligns = dict[str, Align]
 ShowPlot = Union[None, 'png', 'html']
 Fmt = Union[Literal['parquet'], Literal['plotly'], Literal['png']]
+PARQUET: Literal['parquet'] = 'parquet'
+PLOTLY: Literal['plotly'] = 'plotly'
+PNG: Literal['png'] = 'png'
 
 
 @dataclass
 class Config:
     git: GitConfig
     dvc: DvcConfig
     dir: str = DEFAULT_ARTIFACTS_DIR
     relpath: str | None = None
     engine: ParquetEngine = None
+    align: Align | None = None,
     show: ShowPlot = None
 
 
 # Default config values
 config = Config(
     git='add',
     dvc='add' if is_dvc_repo() else False,
     dir=env.get('IRE_DIR', DEFAULT_ARTIFACTS_DIR),
     relpath=env.get('IRE_RELPATH'),
     engine=env.get('IRE_ENGINE'),
+    align=env.get('IRE_ALIGN'),
     show=env.get('IRE_SHOW'),
 )
 
 
 @dataclass
 class Output:
     path: str
@@ -70,38 +78,30 @@
         dir: str = DEFAULT_ARTIFACTS_DIR,
         relpath: str = None,
         extension: str = None,
         git: GitConfig | None = None,
         dvc: DvcConfig | None = None,
         id: str | None = None,
         verbose: bool = False,
-        engine: ParquetEngine = None,
-        index: bool | None = None,
-        fmts: Fmts | None = None,
+        **kwargs,
 ):
     if extension is None:
         extension = DEFAULT_EXTENSION_OVERRIDES.get(fmt, fmt)
 
     def pre_write(path: str):
         if dvc and islink(path):
             # If the file is a symlink, we need to unprotect it before writing
             run('dvc', 'unprotect', path, verbose=verbose)
 
     write_kwargs = {}
     extra_metadata = {}
     spec = getfullargspec(write)
-    if 'engine' in spec.args:
-        if engine is None:
-            engine = config.engine
-        if engine:
-            write_kwargs['engine'] = engine
-    if 'index' in spec.args:
-        write_kwargs['index'] = index
-    if 'fmts' in spec.args:
-        write_kwargs['fmts'] = fmts
+    for k, v in kwargs.items():
+        if k in spec.args and v is not None:
+            write_kwargs[k] = v
 
     if name is None:
         with TemporaryDirectory(dir=getcwd()) as tmpdir:
             basename = f"tmp.{extension}"
             tmp_path = os.path.join(tmpdir, basename)
             write_rv = write(obj, tmp_path, **write_kwargs)
             md5 = md5_file(tmp_path)
@@ -111,31 +111,35 @@
             rename(tmp_path, path)
     else:
         path = os.path.join(dir, f"{name}.{extension}")
         makedirs(dir, exist_ok=True)
         pre_write(path)
         write_rv = write(obj, path, **write_kwargs)
     err(f"Saved {fmt} to {path}")
+    staged_paths = git_staged_paths()
     path = process_dvc_config(dvc, path, verbose=verbose) or path
     md_path = join(relpath, path) if relpath else path
-    process_git_config(git, path, verbose=verbose)
+    process_git_config(git, path, verbose=verbose, staged_paths=staged_paths)
     if write_rv:
         extra_metadata.update(write_rv['metadata'])
     if id:
         extra_metadata['id'] = id
     metadata = { METADATA_KEY: { 'fmt': fmt, 'path': md_path, 'dvc': bool(dvc), **extra_metadata } }
     return metadata
 
 
 def write_parquet(
         df: pd.DataFrame,
         path: str,
         engine: ParquetEngine = None,
         index: bool | None = None,
-        fmts: Fmts | None = None,
+        fmts: ColFmts | None = None,
+        align: ColAligns | None = None,
+        per_page: int | None = None,
+        per_page_opts: list[int] | None = None,
 ):
     if engine is None:
         engine = 'auto'
     elif engine not in ('fastparquet', 'pyarrow'):
         raise ValueError(f"Unrecognized Parquet engine: {engine}")
     metadata = dict()
     index_names = list(filter(None, df.index.names))
@@ -156,14 +160,20 @@
                 raise ValueError(f"Unrecognized column type: {col}")
         fmts_obj = {}
         if cols:
             fmts_obj['cols'] = cols
         if dtypes:
             fmts_obj['dtypes'] = dtypes
         metadata['fmts'] = fmts_obj
+    if align:
+        metadata['align'] = align
+    if per_page is not None:
+        metadata['per_page'] = per_page
+    if per_page_opts is not None:
+        metadata['per_page_opts'] = per_page_opts
     df.to_parquet(path, engine=engine, index=bool(index_names) if index is None else index)
     return dict(metadata=metadata)
 
 
 def write_image(img: Union[Image, bytes], path: str):
     with open(path, 'wb') as f:
         data = img.data if isinstance(img, Image) else img
@@ -181,15 +191,15 @@
 
 
 def maybe_handle_plotly(obj, kwargs, show: ShowPlot = None):
     try:
         from plotly.graph_objs import Figure
         if isinstance(obj, Figure):
             fig = obj
-            metadata = write_obj(fig, write=write_plotly, fmt='plotly', **kwargs)
+            metadata = write_obj(fig, write=write_plotly, fmt=PLOTLY, **kwargs)
             if show == 'png':
                 img_bytes = fig.to_image(format='png')
                 display(Image(img_bytes), metadata=metadata)
             elif show == 'html':
                 html = fig.to_html()
                 display(HTML(html), metadata=metadata)
             else:
@@ -201,15 +211,15 @@
 
 
 def maybe_handle_matplotlib(obj, kwargs):
     try:
         import matplotlib.pyplot as plt
         if isinstance(obj, plt.Figure):
             fig = obj
-            metadata = write_obj(fig, write=write_matplotlib, fmt='png', **kwargs)
+            metadata = write_obj(fig, write=write_matplotlib, fmt=PNG, **kwargs)
             display(fig, metadata=metadata)
             plt.close()
             return True
     except ImportError:
         pass
     return False
 
@@ -220,17 +230,21 @@
         dir: str = None,
         relpath: str = None,
         git: GitConfig | None = None,
         dvc: DvcConfig | None = None,
         id: str | None = None,
         verbose: bool = False,
         show: ShowPlot = None,
+        # Table kwargs
         engine: ParquetEngine = None,
         index: bool | None = None,
-        fmts: Fmts | None = None,
+        fmts: ColFmts | None = None,
+        align: ColAligns | None = None,
+        per_page: int | None = None,
+        per_page_opts: list[int] | None = None,
 ):
     """Export a DataFrame, Image, or Plotly figure to disk, optionally committing to Git and/or DVC.
 
     Args:
         obj: The object to export. DataFrame ⟹ Parquet, Image ⟹ PNG, Plotly ⟹ JSON.
         name: basename of the file to write. If not provided, a name will be generated from the MD5 hash of the object.
         dir: directory in which to write the file. If not provided, the default directory will be used.
@@ -249,42 +263,64 @@
         show: Whether to display the exported object. If `'png'`, a PNG image will be displayed; if `'html'`, an HTML
             representation will be displayed. If `None`, the object will not be displayed.
         engine: The Parquet engine to use when writing a DataFrame. If `None`, the default engine will be used.
         index: Whether to include the DataFrame index when writing to Parquet. If `None`, the index will be included if
             present.
         fmts: Column formatting info to include in the output metadata; string keys are column names, `Type`s are dtypes
             (e.g. `str`, `float` to set a fallback format for all columns of that type).
+        align: Column alignment overrides: [column] -> {'left', 'center', 'right'}
+        per_page: Number of rows per page to display, in the iRe web app
+        per_page_opts: "Rows per page" dropdown options to expose in the iRe web app
     """
     if git is None:
         git = config.git
     if dvc is None:
         dvc = config.dvc
     if dir is None:
         dir = config.dir
     if relpath is None:
         relpath = config.relpath
+    if align is None:
+        align = config.align
     if show is None:
         show = config.show
     if show:
         if show not in ['html', 'png']:
             raise ValueError(f"Unrecognized `show` param: {show}")
+    if engine is None:
+        engine = config.engine
 
-    kwargs = dict(dir=dir, relpath=relpath, name=name, git=git, dvc=dvc, id=id, verbose=verbose)
+    kwargs = dict(
+        dir=dir,
+        relpath=relpath,
+        name=name,
+        git=git,
+        dvc=dvc,
+        id=id,
+        verbose=verbose,
+    )
     if isinstance(obj, pd.DataFrame):
         df = obj
-        kwargs.update(engine=engine, index=index, fmts=fmts)
-        metadata = write_obj(obj=obj, write=write_parquet, fmt='parquet', **kwargs)
+        kwargs.update(
+            engine=engine,
+            index=index,
+            fmts=fmts,
+            align=align,
+            per_page=per_page,
+            per_page_opts=per_page_opts,
+        )
+        metadata = write_obj(obj=obj, write=write_parquet, fmt=PARQUET, **kwargs)
         html = df._repr_html_()
         return display(HTML(html), metadata=metadata)
     elif isinstance(obj, Image):
-        metadata = write_obj(obj=obj, write=write_image, fmt='png', **kwargs)
+        metadata = write_obj(obj=obj, write=write_image, fmt=PNG, **kwargs)
         return display(obj, metadata=metadata)
     elif isinstance(obj, bytes):
         img = Image(obj)
-        metadata = write_obj(obj=img, write=write_image, fmt='png', **kwargs)
+        metadata = write_obj(obj=img, write=write_image, fmt=PNG, **kwargs)
         return display(img, metadata=metadata)
     elif not maybe_handle_plotly(obj, kwargs, show=show) and not maybe_handle_matplotlib(obj, kwargs):
         raise ValueError(f"Unrecognized export type: {type(obj)}")
 
 
 def _ire_df_repr_html_(df):
     return export(df)
@@ -292,15 +328,19 @@
 
 def push(
         git: bool = True,
         dvc: Optional[bool] = None,
         # Err on the side of letting the user know about Git/DVC pushes
         verbose: bool = True,
 ):
+    no_push = bool(env.get(IRE_NO_GIT_PUSH))
     if git:
         if has_unpushed_commits():
-            run('git', 'push', verbose=verbose)
+            if no_push:
+                err(f"Git appears to have unpushed commits, but skipping push due to ${IRE_NO_GIT_PUSH}")
+            else:
+                run('git', 'push', verbose=verbose)
         else:
             if verbose:
                 err("Git appears up to date, skipped push")
     if dvc or (dvc is None and config.dvc is not False):
         run('dvc', 'push', verbose=verbose)
```

### Comparing `iRe.py-0.2.0/ire/utils.py` & `iRe.py-0.3.0/ire/utils.py`

 * *Files identical despite different names*

### Comparing `iRe.py-0.2.0/setup.py` & `iRe.py-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="iRe.py",
-    version="0.2.0",
+    version="0.3.0",
     description="Export tables and plots from Jupyter notebooks, along with metadata for embedding interactive tables in downstream apps.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=open("requirements.txt", "r").read(),
     extras_require={
         "plotly": "plotly",
```

