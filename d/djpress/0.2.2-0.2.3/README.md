# Comparing `tmp/djpress-0.2.2.tar.gz` & `tmp/djpress-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpress-0.2.2.tar", last modified: Sat May 25 12:52:48 2024, max compression
+gzip compressed data, was "djpress-0.2.3.tar", last modified: Sat May 25 13:10:01 2024, max compression
```

## Comparing `djpress-0.2.2.tar` & `djpress-0.2.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.535237 djpress-0.2.2/
--rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.2.2/LICENSE
--rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.2.2/MANIFEST.in
--rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 12:52:48.535008 djpress-0.2.2/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)      504 2024-05-25 05:32:01.000000 djpress-0.2.2/README.md
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.529016 djpress-0.2.2/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.2.2/djpress/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/admin.py
--rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.2.2/djpress/app_settings.py
--rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.2.2/djpress/apps.py
--rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.2.2/djpress/conf.py
--rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/feeds.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.530216 djpress-0.2.2/djpress/migrations/
--rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/migrations/0001_initial.py
--rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/migrations/0002_rename_content_type_post_post_type.py
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/migrations/__init__.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.530619 djpress-0.2.2/djpress/models/
--rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/models/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.2.2/djpress/models/category.py
--rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.2.2/djpress/models/post.py
--rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/signals.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.525234 djpress-0.2.2/djpress/static/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.525288 djpress-0.2.2/djpress/static/djpress/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.531379 djpress-0.2.2/djpress/static/djpress/css/
--rw-r--r--   0 stuart     (501) staff       (20)     3388 2024-05-25 12:51:02.000000 djpress-0.2.2/djpress/static/djpress/css/style.css
--rw-r--r--   0 stuart     (501) staff       (20)     1104 2024-05-25 10:57:09.000000 djpress-0.2.2/djpress/static/djpress/css/style.min.css
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.525407 djpress-0.2.2/djpress/templates/
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.531651 djpress-0.2.2/djpress/templates/djpress/
--rw-r--r--   0 stuart     (501) staff       (20)     2195 2024-05-25 12:48:26.000000 djpress-0.2.2/djpress/templates/djpress/index.html
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.531935 djpress-0.2.2/djpress/templatetags/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/templatetags/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     8838 2024-05-25 10:41:54.000000 djpress-0.2.2/djpress/templatetags/djpress_tags.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.534102 djpress-0.2.2/djpress/tests/
--rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/__init__.py
--rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/test_category_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.2.2/djpress/tests/test_djpress_tags.py
--rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.2.2/djpress/tests/test_feeds.py
--rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.2.2/djpress/tests/test_models.py
--rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/test_post_authors.py
--rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.2.2/djpress/tests/test_published_posts_cache.py
--rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.2.2/djpress/tests/test_views.py
--rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.2.2/djpress/urls.py
--rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.2.2/djpress/utils.py
--rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.2.2/djpress/views.py
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.534763 djpress-0.2.2/djpress.egg-info/
--rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/PKG-INFO
--rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/SOURCES.txt
--rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/dependency_links.txt
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/requires.txt
--rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 12:52:48.000000 djpress-0.2.2/djpress.egg-info/top_level.txt
-drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 12:52:48.534447 djpress-0.2.2/docs/
--rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.2.2/docs/index.md
--rw-r--r--   0 stuart     (501) staff       (20)     1256 2024-05-25 12:52:31.000000 djpress-0.2.2/pyproject.toml
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 12:52:48.535283 djpress-0.2.2/setup.cfg
--rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.2.2/setup.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.314502 djpress-0.2.3/
+-rw-r--r--   0 stuart     (501) staff       (20)     1071 2024-05-25 02:51:53.000000 djpress-0.2.3/LICENSE
+-rw-r--r--   0 stuart     (501) staff       (20)      132 2024-05-25 03:38:25.000000 djpress-0.2.3/MANIFEST.in
+-rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 13:10:01.314268 djpress-0.2.3/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)      504 2024-05-25 05:32:01.000000 djpress-0.2.3/README.md
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.308096 djpress-0.2.3/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)       22 2024-04-24 12:01:53.000000 djpress-0.2.3/djpress/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)      197 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/admin.py
+-rw-r--r--   0 stuart     (501) staff       (20)      733 2024-05-25 04:49:43.000000 djpress-0.2.3/djpress/app_settings.py
+-rw-r--r--   0 stuart     (501) staff       (20)      362 2024-05-25 03:38:21.000000 djpress-0.2.3/djpress/apps.py
+-rw-r--r--   0 stuart     (501) staff       (20)      907 2024-05-25 05:08:15.000000 djpress-0.2.3/djpress/conf.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1254 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/feeds.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.309565 djpress-0.2.3/djpress/migrations/
+-rw-r--r--   0 stuart     (501) staff       (20)     2077 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/migrations/0001_initial.py
+-rw-r--r--   0 stuart     (501) staff       (20)      359 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/migrations/0002_rename_content_type_post_post_type.py
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/migrations/__init__.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.310390 djpress-0.2.3/djpress/models/
+-rw-r--r--   0 stuart     (501) staff       (20)      149 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/models/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3137 2024-05-25 05:11:16.000000 djpress-0.2.3/djpress/models/category.py
+-rw-r--r--   0 stuart     (501) staff       (20)     9716 2024-05-25 05:11:32.000000 djpress-0.2.3/djpress/models/post.py
+-rw-r--r--   0 stuart     (501) staff       (20)      798 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/signals.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.304182 djpress-0.2.3/djpress/static/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.304243 djpress-0.2.3/djpress/static/djpress/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.310938 djpress-0.2.3/djpress/static/djpress/css/
+-rw-r--r--   0 stuart     (501) staff       (20)     3388 2024-05-25 12:51:02.000000 djpress-0.2.3/djpress/static/djpress/css/style.css
+-rw-r--r--   0 stuart     (501) staff       (20)     1104 2024-05-25 10:57:09.000000 djpress-0.2.3/djpress/static/djpress/css/style.min.css
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.304371 djpress-0.2.3/djpress/templates/
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.311191 djpress-0.2.3/djpress/templates/djpress/
+-rw-r--r--   0 stuart     (501) staff       (20)     2139 2024-05-25 13:03:48.000000 djpress-0.2.3/djpress/templates/djpress/index.html
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.311507 djpress-0.2.3/djpress/templatetags/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/templatetags/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     9760 2024-05-25 13:06:13.000000 djpress-0.2.3/djpress/templatetags/djpress_tags.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.313455 djpress-0.2.3/djpress/tests/
+-rw-r--r--   0 stuart     (501) staff       (20)       33 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/tests/__init__.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2804 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/tests/test_category_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14780 2024-05-25 05:11:45.000000 djpress-0.2.3/djpress/tests/test_djpress_tags.py
+-rw-r--r--   0 stuart     (501) staff       (20)     2279 2024-05-25 05:11:50.000000 djpress-0.2.3/djpress/tests/test_feeds.py
+-rw-r--r--   0 stuart     (501) staff       (20)    14353 2024-05-25 05:12:00.000000 djpress-0.2.3/djpress/tests/test_models.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1083 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/tests/test_post_authors.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3903 2024-05-11 07:24:31.000000 djpress-0.2.3/djpress/tests/test_published_posts_cache.py
+-rw-r--r--   0 stuart     (501) staff       (20)     4665 2024-05-25 05:11:55.000000 djpress-0.2.3/djpress/tests/test_views.py
+-rw-r--r--   0 stuart     (501) staff       (20)     1558 2024-05-25 05:10:42.000000 djpress-0.2.3/djpress/urls.py
+-rw-r--r--   0 stuart     (501) staff       (20)      869 2024-05-25 05:10:58.000000 djpress-0.2.3/djpress/utils.py
+-rw-r--r--   0 stuart     (501) staff       (20)     3845 2024-05-22 08:34:14.000000 djpress-0.2.3/djpress/views.py
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.314026 djpress-0.2.3/djpress.egg-info/
+-rw-r--r--   0 stuart     (501) staff       (20)     3006 2024-05-25 13:10:01.000000 djpress-0.2.3/djpress.egg-info/PKG-INFO
+-rw-r--r--   0 stuart     (501) staff       (20)     1052 2024-05-25 13:10:01.000000 djpress-0.2.3/djpress.egg-info/SOURCES.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        1 2024-05-25 13:10:01.000000 djpress-0.2.3/djpress.egg-info/dependency_links.txt
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 13:10:01.000000 djpress-0.2.3/djpress.egg-info/requires.txt
+-rw-r--r--   0 stuart     (501) staff       (20)        8 2024-05-25 13:10:01.000000 djpress-0.2.3/djpress.egg-info/top_level.txt
+drwxr-xr-x   0 stuart     (501) staff       (20)        0 2024-05-25 13:10:01.313726 djpress-0.2.3/docs/
+-rw-r--r--   0 stuart     (501) staff       (20)       16 2024-05-25 03:04:28.000000 djpress-0.2.3/docs/index.md
+-rw-r--r--   0 stuart     (501) staff       (20)     1256 2024-05-25 13:09:32.000000 djpress-0.2.3/pyproject.toml
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 13:10:01.314551 djpress-0.2.3/setup.cfg
+-rw-r--r--   0 stuart     (501) staff       (20)       38 2024-05-25 03:38:24.000000 djpress-0.2.3/setup.py
```

### Comparing `djpress-0.2.2/LICENSE` & `djpress-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/PKG-INFO` & `djpress-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.2.2
+Version: 0.2.3
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `djpress-0.2.2/djpress/app_settings.py` & `djpress-0.2.3/djpress/app_settings.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/conf.py` & `djpress-0.2.3/djpress/conf.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/feeds.py` & `djpress-0.2.3/djpress/feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/migrations/0001_initial.py` & `djpress-0.2.3/djpress/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/models/category.py` & `djpress-0.2.3/djpress/models/category.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/models/post.py` & `djpress-0.2.3/djpress/models/post.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/signals.py` & `djpress-0.2.3/djpress/signals.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/static/djpress/css/style.css` & `djpress-0.2.3/djpress/static/djpress/css/style.css`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/static/djpress/css/style.min.css` & `djpress-0.2.3/djpress/static/djpress/css/style.min.css`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/templates/djpress/index.html` & `djpress-0.2.3/djpress/templates/djpress/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         {% endif %}
 
         {% for post in posts %}
 
           <article>
             <header>
-              <h1><a href="{% url 'djpress:post_detail' post.permalink %}">{% post_title %}</a></h1>
+              <h1>{% post_title_link %}</h1>
               <p>By {% post_author %}. {% post_date %}</p>
             </header>
             <section>
               {{ post.truncated_content_markdown|safe }}
 
               {% if post.is_truncated %}
                 <p><a href="{% url 'djpress:post_detail' post.permalink %}">Read more</a></p>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 {% post_content %}
 Categories: {% post_categories "span" "badge" %}
 {% comment %}If we get multiple posts, then show the truncated content.{%
 endcomment %} {% elif posts %} {% comment %}If we get posts for a category,
 then we can show the category header.{% endcomment %} {% if category %}
 ************ {{%% ccaatteeggoorryy__nnaammee %%}} ************
 {% endif %} {% for post in posts %}
-************ _{{_%%_ _pp_oo_ss_tt____tt_ii_tt_ll_ee_ _%%_}} ************
+************ {{%% ppoosstt__ttiittllee__lliinnkk %%}} ************
 By {% post_author %}. {% post_date %}
 {{ post.truncated_content_markdown|safe }} {% if post.is_truncated %}
 _R_e_a_d_ _m_o_r_e
 {% endif %}
 Categories: {% post_categories "span" "badge" %}
 {% endfor %} {% else %}
 No posts available.
```

### Comparing `djpress-0.2.2/djpress/templatetags/djpress_tags.py` & `djpress-0.2.3/djpress/templatetags/djpress_tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,24 @@
         f'{settings.BLOG_TITLE}</a>'
     )
 
     return mark_safe(ouptut)
 
 
 @register.simple_tag
+def get_categories() -> models.QuerySet[Category] | None:
+    """Return all categories as a queryset.
+
+    Returns:
+        models.QuerySet[Category]: All categories.
+    """
+    return Category.objects.get_categories()
+
+
+@register.simple_tag
 def blog_categories(outer: str = "ul", link_class: str = "") -> str:
     """Return the categories of the blog.
 
     Args:
         outer: The outer HTML tag for the categories.
         link_class: The CSS class(es) for the link.
 
@@ -113,14 +123,41 @@
     if not post:
         return ""
 
     return post.title
 
 
 @register.simple_tag(takes_context=True)
+def post_title_link(context: Context, link_class: str = "") -> str:
+    """Return the title link for a post.
+
+    Args:
+        context: The context.
+        link_class: The CSS class(es) for the link.
+
+    Returns:
+        str: The title link for the post.
+    """
+    post: Post | None = context.get("post")
+    if not post:
+        return ""
+
+    post_url = reverse("djpress:post_detail", args=[post.permalink])
+
+    link_class_html = f' class="{link_class}"' if link_class else ""
+
+    output = (
+        f'<a href="{post_url}" title="{post.title}"{link_class_html}>'
+        f"{post.title}</a>"
+    )
+
+    return mark_safe(output)
+
+
+@register.simple_tag(takes_context=True)
 def post_author(context: Context) -> str:
     """Return the author display name.
 
     Tries to display the first name and last name if available, otherwise falls back to
     the username.
 
     Args:
```

### Comparing `djpress-0.2.2/djpress/tests/test_category_cache.py` & `djpress-0.2.3/djpress/tests/test_category_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/tests/test_djpress_tags.py` & `djpress-0.2.3/djpress/tests/test_djpress_tags.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/tests/test_feeds.py` & `djpress-0.2.3/djpress/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/tests/test_models.py` & `djpress-0.2.3/djpress/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/tests/test_post_authors.py` & `djpress-0.2.3/djpress/tests/test_post_authors.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/tests/test_published_posts_cache.py` & `djpress-0.2.3/djpress/tests/test_published_posts_cache.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/tests/test_views.py` & `djpress-0.2.3/djpress/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/urls.py` & `djpress-0.2.3/djpress/urls.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/utils.py` & `djpress-0.2.3/djpress/utils.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress/views.py` & `djpress-0.2.3/djpress/views.py`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/djpress.egg-info/PKG-INFO` & `djpress-0.2.3/djpress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpress
-Version: 0.2.2
+Version: 0.2.3
 Summary: A blog application for Django sites, inspired by classic WordPress.
 Author-email: Stuart Maxwell <stuart@amanzi.nz>
 License: MIT License
         
         Copyright (c) 2024 Stuart Maxwell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `djpress-0.2.2/djpress.egg-info/SOURCES.txt` & `djpress-0.2.3/djpress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djpress-0.2.2/pyproject.toml` & `djpress-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "djpress"
-version = "0.2.2"
+version = "0.2.3"
 authors = [{ name = "Stuart Maxwell", email = "stuart@amanzi.nz" }]
 description = "A blog application for Django sites, inspired by classic WordPress."
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = ["django", "markdown"]
 license = { file = "LICENSE" }
 classifiers = [
```

