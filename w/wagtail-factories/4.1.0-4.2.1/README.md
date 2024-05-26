# Comparing `tmp/wagtail_factories-4.1.0.tar.gz` & `tmp/wagtail_factories-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail_factories-4.1.0.tar", last modified: Tue May 16 12:27:01 2023, max compression
+gzip compressed data, was "wagtail_factories-4.2.1.tar", last modified: Sun May 26 11:24:09 2024, max compression
```

## Comparing `wagtail_factories-4.1.0.tar` & `wagtail_factories-4.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2102 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/wagtail_factories/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/wagtail_factories.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/wagtail_factories.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:24:09.824760 wagtail_factories-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-26 11:24:09.824760 wagtail_factories-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 11:24:09.824760 wagtail_factories-4.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1976 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:24:09.820760 wagtail_factories-4.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:24:09.824760 wagtail_factories-4.2.1/src/wagtail_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/src/wagtail_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/src/wagtail_factories/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/src/wagtail_factories/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/src/wagtail_factories/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-26 11:24:07.000000 wagtail_factories-4.2.1/src/wagtail_factories/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 11:24:09.824760 wagtail_factories-4.2.1/src/wagtail_factories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-26 11:24:09.000000 wagtail_factories-4.2.1/src/wagtail_factories.egg-info/SOURCES.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wagtail_factories-4.1.0/CHANGES` & `wagtail_factories-4.2.1/CHANGES`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 Unreleased
 ==========
+- Update for Wagtail > 5.2
+- Drop support for Django < 4.2
+- Drop support for Wagtail < 5.2
+- Add support for Django 5
+- Add support for Wagtail 6
+- Add support for Python 3.12
+- Add support for StructBlocks with custom StructValue classes
 
 4.1.0
 =====
 - Add support Wagtail 5.0
 - Drop support for Wagtail < 4.1
 
 4.0.0
```

### Comparing `wagtail_factories-4.1.0/README.rst` & `wagtail_factories-4.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,190 +1,186 @@
-=================
-wagtail-factories
-=================
+# wagtail-factories
 
 Factory boy classes for Wagtail CMS
 
-.. start-no-pypi
+## Join the Community at Wagtail Space!
 
-Status
-------
+Join us at Wagtail Space US this year! The Call for Participation and Registration for both Wagtail Space 2024 events is open. We would love to have you give a talk, or just us as an attendee in June.
 
-.. image:: https://readthedocs.org/projects/wagtail-factories/badge/?version=latest
-    :target: https://readthedocs.org/projects/wagtail-factories/
+* [Wagtail Space NL](https://nl.wagtail.space/), Arnhem, The Netherlands. 2024-06-14
+* [Wagtail Space US](https://us.wagtail.space/), Philadelphia, PA. 2024-06-20 to 2024-06-22
 
-.. image:: https://github.com/wagtail/wagtail-factories/workflows/Python%20Tests/badge.svg
-    :target: https://github.com/wagtail/wagtail-factories/actions?query=workflow%3A%22Python+Tests%22
+## Status
 
-.. image:: https://img.shields.io/pypi/v/wagtail-factories.svg
-    :target: https://pypi.python.org/pypi/wagtail-factories/
+[![image](https://readthedocs.org/projects/wagtail-factories/badge/?version=latest)](https://readthedocs.org/projects/wagtail-factories/)
+[![image](https://github.com/wagtail/wagtail-factories/workflows/Python%20Tests/badge.svg)](https://github.com/wagtail/wagtail-factories/actions?query=workflow%3A%22Python+Tests%22)
+[![image](https://img.shields.io/pypi/v/wagtail-factories.svg)](https://pypi.python.org/pypi/wagtail-factories/)
 
+## Installation
 
-.. end-no-pypi
+``` shell
+pip install wagtail-factories
+```
 
+## Usage
 
+Documentation is still in progress, but see the
+[tests](https://github.com/wagtail/wagtail-factories/tree/main/tests)
+for more examples.
 
-Installation
-============
+``` python
+import wagtail_factories
+from . import models
 
-.. code-block:: shell
 
-   pip install wagtail-factories
+class MyCarouselItemFactory(wagtail_factories.StructBlockFactory):
+    label = 'my-label'
+    image = factory.SubFactory(
+        wagtail_factories.ImageChooserBlockFactory)
 
+    class Meta:
+        model = models.MyBlockItem
 
 
-Usage
-=====
+class MyCarouselFactory(wagtail_factories.StructBlockFactory):
+    title = "Carousel title"
+    items = wagtail_factories.ListBlockFactory(
+        MyCarouselItemFactory)
 
-Documentation is still in progress, but see the `tests`_ for more examples.
+    class Meta:
+        model = models.MyCarousel
 
-.. _tests: https://github.com/wagtail/wagtail-factories/tree/main/tests
 
-.. code-block:: python
+class MyNewsPageFactory(wagtail_factories.PageFactory):
+    class Meta:
+        model = models.MyNewsPage
 
-    import wagtail_factories
-    from . import models
 
+class MyNewsPageChooserBlockFactory(wagtail_factories.PageChooserBlockFactory):
+    page = factory.SubFactory(MyNewsPageFactory)
 
-    class MyCarouselItemFactory(wagtail_factories.StructBlockFactory):
-        label = 'my-label'
-        image = factory.SubFactory(
-            wagtail_factories.ImageChooserBlockFactory)
 
-        class Meta:
-            model = models.MyBlockItem
+class MyTestPageFactory(wagtail_factories.PageFactory):
+    body = wagtail_factories.StreamFieldFactory({
+        'carousel': factory.SubFactory(MyCarouselFactory),
+        'news_page': factory.SubFactory(MyNewsPageChooserBlockFactory),
+    })
 
+    class Meta:
+        model = models.MyTestPage
 
-    class MyCarouselFactory(wagtail_factories.StructBlockFactory):
-        title = "Carousel title"
-        items = wagtail_factories.ListBlockFactory(
-            MyCarouselItemFactory)
 
-        class Meta:
-            model = models.MyCarousel
-
-
-    class MyNewsPageFactory(wagtail_factories.PageFactory):
-        class Meta:
-            model = models.MyNewsPage
-
-
-    class MyNewsPageChooserBlockFactory(wagtail_factories.PageChooserBlockFactory):
-        page = factory.SubFactory(MyNewsPageFactory)
-
-
-    class MyTestPageFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory({
-            'carousel': factory.SubFactory(MyCarouselFactory),
-            'news_page': factory.SubFactory(MyNewsPageChooserBlockFactory),
-        })
-
-        class Meta:
-            model = models.MyTestPage
-
-
-    def test_my_page():
-        root_page = wagtail_factories.PageFactory(parent=None)
-        my_page = MyTestPageFactory(
-            parent=root_page,
-            body__0__carousel__items__0__label='Slide 1',
-            body__0__carousel__items__0__image__image__title='Image Slide 1',
-            body__0__carousel__items__1__label='Slide 2',
-            body__0__carousel__items__1__image__image__title='Image Slide 2',
-            body__0__carousel__items__2__label='Slide 3',
-            body__0__carousel__items__2__image__image__title='Image Slide 3',
-            body__1__news_page__page__title="News",
-        )
-
-
-Using StreamBlockFactory
-========================
-
-``StreamBlockFactory`` can be used in conjunction with the other block factory types to create complex, nested ``StreamValues``, much like how ``StreamBlock`` can be used to declare the blocks for a complex ``StreamField``.
-
-First, define your ``StreamBlockFactory`` subclass, using ``factory.SubFactory`` to wrap child block declarations. Be sure to include your ``StreamBlock`` subclass as the model attribute on the inner ``Meta`` class.
-
-.. code-block:: python
-
-    class MyStreamBlockFactory(wagtail_factories.StreamBlockFactory):
-        my_struct_block = factory.SubFactory(MyStructBlockFactory)
-
-        class Meta:
-            model = MyStreamBlock
-
-
-Then include your ``StreamBlockFactory`` subclass on a model factory as the argument to a ``StreamFieldFactory``.
-
-.. code-block:: python
-
-    class MyPageFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory(MyStreamBlockFactory)
-
-        class Meta:
-            model = MyPage
-
-
-You can then use a modified version of factory_boy's deep object declaration syntax to build up ``StreamValues`` on the fly.
-
-.. code-block:: python
-
-    MyPageFactory(
-        body__0__my_struct_block__some_field="some value",
-        body__0__my_struct_block__some_other_field="some other value",
+def test_my_page():
+    root_page = wagtail_factories.PageFactory(parent=None)
+    my_page = MyTestPageFactory(
+        parent=root_page,
+        body__0__carousel__items__0__label='Slide 1',
+        body__0__carousel__items__0__image__image__title='Image Slide 1',
+        body__0__carousel__items__1__label='Slide 2',
+        body__0__carousel__items__1__image__image__title='Image Slide 2',
+        body__0__carousel__items__2__label='Slide 3',
+        body__0__carousel__items__2__image__image__title='Image Slide 3',
+        body__1__news_page__page__title="News",
     )
+```
 
+### Using StreamBlockFactory
 
-To generate the default value for a block factory, terminate your declaration at the index and provide the block name as the value.
-
-.. code-block:: python
-
-    MyPageFactory(body__0="my_struct_block")
-
-
-Alternative StreamFieldFactory declaration syntax
-=================================================
-
-Prior to version 3.0, ``StreamFieldFactory`` could only be used by providing a dict mapping block names to block factory classes as the single argument, for example:
-
-.. code-block:: python
-
-    class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory(
-            {
-                "char_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.CharBlockFactory
-                ),
-                "int_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.IntegerBlockFactory
-                ),
-                "struct": MyBlockFactory,
-                "image": wagtail_factories.ImageChooserBlockFactory,
-            }
-        )
-    
-        class Meta:
-            model = models.MyTestPage
-    
-
-This style of declaration is still supported, with the caveat that nested stream blocks are not supported for this approach. From version 3.0, all ``BlockFactory`` values in a ``StreamFieldFactory`` definition of this style *must* be wrapped in factory_boy ``SubFactories``. For example, the above example must be updated to the following for 3.0 compatibility.
-
-.. code-block:: python
-
-    class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory(
-            {
-                "char_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.CharBlockFactory
-                ),
-                "int_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.IntegerBlockFactory
-                ),
-                "struct": factory.SubFactory(MyBlockFactory),
-                "image": factory.SubFactory(wagtail_factories.ImageChooserBlockFactory),
-            }
-        )
+`StreamBlockFactory` can be used in conjunction with the other block
+factory types to create complex, nested `StreamValues`, much like how
+`StreamBlock` can be used to declare the blocks for a complex
+`StreamField`.
+
+First, define your `StreamBlockFactory` subclass, using
+`factory.SubFactory` to wrap child block declarations. Be sure to
+include your `StreamBlock` subclass as the model attribute on the inner
+`Meta` class.
+
+``` python
+class MyStreamBlockFactory(wagtail_factories.StreamBlockFactory):
+    my_struct_block = factory.SubFactory(MyStructBlockFactory)
+
+    class Meta:
+        model = MyStreamBlock
+```
+
+Then include your `StreamBlockFactory` subclass on a model factory as
+the argument to a `StreamFieldFactory`.
+
+``` python
+class MyPageFactory(wagtail_factories.PageFactory):
+    body = wagtail_factories.StreamFieldFactory(MyStreamBlockFactory)
+
+    class Meta:
+        model = MyPage
+```
+
+You can then use a modified version of factory\_boy\'s deep object
+declaration syntax to build up `StreamValues` on the fly.
+
+``` python
+MyPageFactory(
+    body__0__my_struct_block__some_field="some value",
+    body__0__my_struct_block__some_other_field="some other value",
+)
+```
+
+To generate the default value for a block factory, terminate your
+declaration at the index and provide the block name as the value.
+
+``` python
+MyPageFactory(body__0="my_struct_block")
+```
+
+### Alternative StreamFieldFactory declaration syntax
+
+Prior to version 3.0, `StreamFieldFactory` could only be used by
+providing a dict mapping block names to block factory classes as the
+single argument, for example:
+
+``` python
+class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
+    body = wagtail_factories.StreamFieldFactory(
+        {
+            "char_array": wagtail_factories.ListBlockFactory(
+                wagtail_factories.CharBlockFactory
+            ),
+            "int_array": wagtail_factories.ListBlockFactory(
+                wagtail_factories.IntegerBlockFactory
+            ),
+            "struct": MyBlockFactory,
+            "image": wagtail_factories.ImageChooserBlockFactory,
+        }
+    )
 
-        class Meta:
-            model = models.MyTestPage
+    class Meta:
+        model = models.MyTestPage
+```
+
+This style of declaration is still supported, with the caveat that
+nested stream blocks are not supported for this approach. From version
+3.0, all `BlockFactory` values in a `StreamFieldFactory` definition of
+this style *must* be wrapped in factory\_boy `SubFactories`. For
+example, the above example must be updated to the following for 3.0
+compatibility.
+
+``` python
+class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
+    body = wagtail_factories.StreamFieldFactory(
+        {
+            "char_array": wagtail_factories.ListBlockFactory(
+                wagtail_factories.CharBlockFactory
+            ),
+            "int_array": wagtail_factories.ListBlockFactory(
+                wagtail_factories.IntegerBlockFactory
+            ),
+            "struct": factory.SubFactory(MyBlockFactory),
+            "image": factory.SubFactory(wagtail_factories.ImageChooserBlockFactory),
+        }
+    )
 
+    class Meta:
+        model = models.MyTestPage
+```
 
-This requirement does *not* apply to ``ListBlockFactory``, which is a subclass of ``SubFactory``.
+This requirement does *not* apply to `ListBlockFactory`, which is a
+subclass of `SubFactory`.
```

### Comparing `wagtail_factories-4.1.0/setup.py` & `wagtail_factories-4.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 import re
 
 from setuptools import find_packages, setup
 
 install_requires = [
     "factory-boy>=3.2",
-    "wagtail>=4.1",
+    "wagtail>=5.2",
 ]
 
 docs_require = [
-    "sphinx>=1.4.0",
+    "sphinx>=7.3.7",
 ]
 
 tests_require = [
-    "pytest==6.2.5",
-    "pytest-django==4.5.0",
-    "pytest-cov==3.0.0",
-    "pytest-pythonpath==0.7.3",
-    "psycopg2>=2.3.1",
-    "coverage==6.0",
-    "isort==5.10.0",
-    "flake8==4.0.0",
-    "flake8-blind-except==0.1.1",
-    "flake8-debugger==4.1.2",
+    "pytest==8.2.1",
+    "pytest-django==4.8.0",
+    "pytest-cov==5.0.0",
+    "coverage==7.5.1",
+    "ruff==0.4.4",
 ]
 
-with open("README.rst") as fh:
+with open("README.md") as fh:
     long_description = re.sub(
-        "^.. start-no-pypi.*^.. end-no-pypi", "", fh.read(), flags=re.M | re.S
+        r"^## Status.*\n(## Installation)", r"\1", fh.read(), flags=re.M | re.S
     )
 
 setup(
     name="wagtail_factories",
-    version="4.1.0",
+    version="4.2.1",
     description="Factory boy classes for wagtail",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     author="Michael van Tellingen",
     author_email="michaelvantellingen@gmail.com",
     url="https://github.com/wagtail/wagtail-factories/",
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={
         "docs": docs_require,
@@ -50,24 +46,23 @@
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Django",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 4",
         "Framework :: Wagtail :: 5",
+        "Framework :: Wagtail :: 6",
     ],
     zip_safe=False,
 )
```

### Comparing `wagtail_factories-4.1.0/src/wagtail_factories/blocks.py` & `wagtail_factories-4.2.1/src/wagtail_factories/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     _options_class = StreamBlockFactoryOptions
     _builder_class = StreamBlockStepBuilder
 
     @classmethod
     def _generate(cls, strategy, params):
         if cls._meta.abstract and not hasattr(cls, "__generate_abstract__"):
             raise factory.errors.FactoryError(
-                "Cannot generate instances of abstract factory %(f)s; "
-                "Ensure %(f)s.Meta.model is set and %(f)s.Meta.abstract "
-                "is either not set or False." % dict(f=cls.__name__)
+                "Cannot generate instances of abstract factory {f}; "
+                "Ensure {f}.Meta.model is set and {f}.Meta.abstract "
+                "is either not set or False.".format(**{"f": cls.__name__})
             )
         step = cls._builder_class(cls._meta, params, strategy)
         return step.build()
 
     @classmethod
     def _construct_stream(cls, block_class, *args, **kwargs):
         def get_index(key):
@@ -142,17 +142,17 @@
 
     class Meta:
         abstract = True
         model = blocks.StructBlock
 
     @classmethod
     def _construct_struct_value(cls, block_class, params):
-        return blocks.StructValue(
+        return block_class._meta_class.value_class(
             block_class(),
-            [(name, value) for name, value in params.items()],
+            list(params.items()),
         )
 
     @classmethod
     def _build(cls, block_class, *args, **kwargs):
         return cls._construct_struct_value(block_class, kwargs)
 
     @classmethod
```

### Comparing `wagtail_factories-4.1.0/src/wagtail_factories/builder.py` & `wagtail_factories-4.2.1/src/wagtail_factories/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,20 +73,20 @@
                         f"(got {v}, already have {indexed_block_names[key]})"
                     )
                 indexed_block_names[key] = v
             else:
                 try:
                     i, name, *params = k.split("__", maxsplit=2)
                     key = int(i)
-                except (ValueError, TypeError):
+                except (ValueError, TypeError) as err:
                     raise InvalidDeclaration(
                         "StreamFieldFactory declarations must be of the form "
                         "<index>=<block_name>, <index>__<block_name>=value or "
                         f"<index>__<block_name>__<param>=value, got: {k}"
-                    )
+                    ) from err
                 if key in indexed_block_names and indexed_block_names[key] != name:
                     raise DuplicateDeclaration(
                         f"Multiple declarations for index {key} at this level of nesting "
                         f"(got {name}, already have {indexed_block_names[key]})"
                     )
                 indexed_block_names[key] = name
                 transformed_key = self.reconstruct_key(i, name, params)
```

### Comparing `wagtail_factories-4.1.0/src/wagtail_factories/factories.py` & `wagtail_factories-4.2.1/src/wagtail_factories/factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "SiteFactory",
     "DocumentFactory",
 ]
 logger = logging.getLogger(__file__)
 
 
 class ParentNodeFactory(ParameteredAttribute):
-
     EXTEND_CONTAINERS = True
     FORCE_SEQUENCE = False
     UNROLL_CONTEXT_BEFORE_EVALUATION = False
 
     def generate(self, step, params):
         if not params:
             return None
@@ -38,15 +37,14 @@
             step,
         )
         force_sequence = step.sequence if self.FORCE_SEQUENCE else None
         return step.recurse(subfactory, params, force_sequence=force_sequence)
 
 
 class MP_NodeFactory(DjangoModelFactory):
-
     parent = ParentNodeFactory()
 
     @classmethod
     def _build(cls, model_class, *args, **kwargs):
         kwargs.pop("parent")
         return model_class(**kwargs)
 
@@ -54,15 +52,14 @@
     def _create(cls, model_class, *args, **kwargs):
         parent = kwargs.pop("parent")
 
         if cls._meta.django_get_or_create:
             instance = cls._get_or_create(model_class, *args, parent=parent, **kwargs)
         else:
             instance = cls._create_instance(model_class, parent, kwargs)
-            assert instance.pk
         return instance
 
     @classmethod
     def _create_instance(cls, model_class, parent, kwargs):
         instance = model_class(**kwargs)
         if parent:
             parent.add_child(instance=instance)
@@ -70,27 +67,28 @@
             model_class.add_root(instance=instance)
         return instance
 
     @classmethod
     def _get_or_create(cls, model_class, *args, **kwargs):
         """Create an instance of the model through objects.get_or_create."""
         manager = cls._get_manager(model_class)
-        assert "defaults" not in cls._meta.django_get_or_create, (
-            "'defaults' is a reserved keyword for get_or_create "
-            "(in %s._meta.django_get_or_create=%r)"
-            % (cls, cls._meta.django_get_or_create)
-        )
+        if "defaults" in cls._meta.django_get_or_create:
+            raise RuntimeError(
+                "'defaults' is a reserved keyword for get_or_create "
+                f"(in {cls}._meta.django_get_or_create={cls._meta.django_get_or_create!r})"
+            )
 
         lookup_fields = {}
         for field in cls._meta.django_get_or_create:
             if field not in kwargs:
                 raise errors.FactoryError(
                     "django_get_or_create - "
-                    "Unable to find initialization value for '%s' in factory %s"
-                    % (field, cls.__name__)
+                    "Unable to find initialization value for '{}' in factory {}".format(
+                        field, cls.__name__
+                    )
                 )
             lookup_fields[field] = kwargs[field]
 
         parent = lookup_fields.pop("parent", None)
         kwargs.pop("parent", None)
 
         if parent:
```

### Comparing `wagtail_factories-4.1.0/src/wagtail_factories/options.py` & `wagtail_factories-4.2.1/src/wagtail_factories/options.py`

 * *Files identical despite different names*

