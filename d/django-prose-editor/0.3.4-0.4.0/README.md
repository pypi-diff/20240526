# Comparing `tmp/django_prose_editor-0.3.4.tar.gz` & `tmp/django_prose_editor-0.4.0.tar.gz`

## Comparing `django_prose_editor-0.3.4.tar` & `django_prose_editor-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/fields.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/sanitized.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/widgets.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/editor.css
--rw-r--r--   0        0        0   224352 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/editor.js
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/init.js
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/material-icons.css
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/material-icons.woff2
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/LICENSE
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/README.rst
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 django_prose_editor-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/fields.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/sanitized.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/widgets.py
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/editor.css
+-rw-r--r--   0        0        0   224550 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/editor.js
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/init.js
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/material-icons.css
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/material-icons.woff2
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/README.rst
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6436 2020-02-02 00:00:00.000000 django_prose_editor-0.4.0/PKG-INFO
```

### Comparing `django_prose_editor-0.3.4/django_prose_editor/fields.py` & `django_prose_editor-0.4.0/django_prose_editor/fields.py`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.4/django_prose_editor/widgets.py` & `django_prose_editor-0.4.0/django_prose_editor/widgets.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,14 @@
             "screen": [
                 "django_prose_editor/material-icons.css",
                 "django_prose_editor/editor.css",
             ]
         }
         js = [
             "django_prose_editor/editor.js",
-            "admin/js/jquery.init.js",
             "django_prose_editor/init.js",
         ]
 
     def __init__(self, *args, **kwargs):
         self.config = kwargs.pop("config", {})
         super().__init__(*args, **kwargs)
```

### Comparing `django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/editor.css` & `django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/editor.css`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-.ProseMirror{padding:1rem 1.75rem;outline:none!important;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif;margin:0!important}.ProseMirror *{color:var(--body-fg)!important}.ProseMirror p{font-size:15px!important}.ProseMirror h1{display:block!important;font-size:2em!important;margin-block-start:.67em!important;margin-block-end:.67em!important;margin-inline-start:0px!important;margin-inline-end:0px!important;font-weight:700!important}.ProseMirror h2{padding:0;display:block!important;font-size:1.5em!important;margin-block-start:.83em!important;margin-block-end:.83em!important;margin-inline-start:0px!important;margin-inline-end:0px!important;font-weight:700!important;background:#fff!important}.ProseMirror h3{display:block!important;font-size:1.17em!important;margin-block-start:1em!important;margin-block-end:1em!important;margin-inline-start:0px!important;margin-inline-end:0px!important;font-weight:700!important;padding:0!important}.ProseMirror>*+*{margin-top:.75em!important}.ProseMirror p.is-editor-empty:first-child:before{content:attr(data-placeholder);float:left;color:#a8a8a8;pointer-events:none;height:0}.ProseMirror ol{padding-left:0!important;list-style-type:decimal!important}.ProseMirror ol li::marker{font-size:16px!important}.ProseMirror ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:lower-latin!important}.ProseMirror ol>li>ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:lower-roman!important}.ProseMirror ol>li>ol>li>ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:upper-latin!important}.ProseMirror ol>li>ol>li>ol>li>ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:upper-roman!important}.ProseMirror ul{list-style-type:disc!important;margin-block-start:0!important;margin-block-end:0!important;margin-inline-start:0px!important;margin-inline-end:0px!important}.ProseMirror ul li{list-style:disc!important}.ProseMirror ul>li>ul{padding-left:10px!important;margin-left:10px!important;list-style-type:disc!important}.ProseMirror{margin:1rem 0}.ProseMirror h1,.ProseMirror h2,.ProseMirror h3,.ProseMirror h4,.ProseMirror h5,.ProseMirror h6{line-height:1.1;text-transform:none;padding:0;background:none!important;border:none!important}.ProseMirror pre{background:#0d0d0d!important;color:#fff!important;font-family:JetBrainsMono,monospace!important;padding:.75rem 1rem!important;border-radius:.5rem!important}.ProseMirror pre code{color:#fff!important;padding:0!important;background:none!important;font-size:.8rem!important}.ProseMirror img{max-width:100%;height:auto}.ProseMirror blockquote{padding-left:1rem;border-left:2px solid rgba(13,13,13,.1)}.ProseMirror hr{border:none;border-top:2px solid rgba(13,13,13,.1);margin:2rem 0!important}.ProseMirror a{text-decoration:underline}.ProseMirror table{border-collapse:collapse;table-layout:fixed;width:100%;margin:0;overflow:hidden}.ProseMirror table td,.ProseMirror table th,.ProseMirror table[show_borders=false]:hover td,.ProseMirror table[show_borders=false]:hover th{min-width:1em;border:2px solid #ced4da;padding:3px 5px;vertical-align:top;box-sizing:border-box;position:relative}.ProseMirror table[show_borders=false] td,.ProseMirror table[show_borders=false] th{border:none;box-sizing:border-box}.ProseMirror table td>*,.ProseMirror table th>*{margin-bottom:0}.ProseMirror table th{font-weight:700;text-align:left;background-color:#f1f3f5}.ProseMirror tr{background-color:#fff!important}.ProseMirror table .selectedCell:after{z-index:2;position:absolute;content:"";inset:0;background:#c8c8ff66;pointer-events:none}.ProseMirror table .column-resize-handle{position:absolute;right:-2px;top:0;bottom:-2px;width:4px;background-color:#adf;pointer-events:none}.tableWrapper{overflow-x:auto}.resize-cursor{cursor:ew-resize;cursor:col-resize}.ProseMirror{padding:0 6px;border:1px solid var(--border-color);border-radius:4px}.prose-editor *,.prose-editor *:before,.prose-editor *:after{box-sizing:inherit}.prose-editor{box-sizing:border-box;position:relative;max-width:120ch;min-width:40ch;flex-grow:1}.prose-editor+textarea{display:none}.prose-menubar{font-size:14px;background:var(--body-bg);display:inline-flex;gap:8px;flex-wrap:wrap;margin-bottom:2px}.prose-menubar__group{display:flex}.prose-menubar__button{cursor:pointer;padding:0 .25em;min-width:2em;transition:all .25s;border:1px solid var(--border-color);text-align:center;display:inline-flex;position:relative}.prose-menubar__button--heading .level{position:absolute;right:3px;bottom:2px;font-size:80%}.prose-menubar__button:first-child{border-top-left-radius:4px;border-bottom-left-radius:4px}.prose-menubar__button:last-child{border-top-right-radius:4px;border-bottom-right-radius:4px}.prose-menubar__button+.prose-menubar__button{border-left:none}.prose-menubar__button.material-icons{padding:0 .125em;min-width:auto}.prose-menubar__button:hover{filter:brightness(110%)}.prose-menubar__button.active{background-color:var(--primary)}.prose-menubar__button.disabled{background:var(--border-color);filter:brightness(100%);cursor:not-allowed;opacity:.3}.prose-editor-dialog{background:var(--body-bg);color:var(--body-fg);border:1px solid var(--border-color)}.prose-editor-dialog label{display:block}label:empty:has(+.prose-editor){display:none}.ProseMirror{position:relative}.ProseMirror{word-wrap:break-word;white-space:pre-wrap;white-space:break-spaces;font-variant-ligatures:none;font-feature-settings:"liga" 0}.ProseMirror pre{white-space:pre-wrap}.ProseMirror li{position:relative}.ProseMirror-hideselection *::selection{background:transparent}.ProseMirror-hideselection *::-moz-selection{background:transparent}.ProseMirror-hideselection{caret-color:transparent}.ProseMirror [draggable][contenteditable=false]{-webkit-user-select:text;-moz-user-select:text;user-select:text}.ProseMirror-selectednode{outline:2px solid #8cf}li.ProseMirror-selectednode{outline:none}li.ProseMirror-selectednode:after{content:"";position:absolute;inset:-2px -2px -2px -32px;border:2px solid #8cf;pointer-events:none}img.ProseMirror-separator{display:inline!important;border:none!important;margin:0!important}
+.ProseMirror{padding:1rem 1.75rem;outline:none!important;font-family:-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Open Sans,Helvetica Neue,sans-serif;margin:0!important}.ProseMirror *{color:var(--body-fg)!important}.ProseMirror p{font-size:15px!important}.ProseMirror h1{display:block!important;font-size:2em!important;margin-block-start:.67em!important;margin-block-end:.67em!important;margin-inline-start:0px!important;margin-inline-end:0px!important;font-weight:700!important}.ProseMirror h2{padding:0;display:block!important;font-size:1.5em!important;margin-block-start:.83em!important;margin-block-end:.83em!important;margin-inline-start:0px!important;margin-inline-end:0px!important;font-weight:700!important;background:#fff!important}.ProseMirror h3{display:block!important;font-size:1.17em!important;margin-block-start:1em!important;margin-block-end:1em!important;margin-inline-start:0px!important;margin-inline-end:0px!important;font-weight:700!important;padding:0!important}.ProseMirror>*+*{margin-top:.75em!important}.ProseMirror p.is-editor-empty:first-child:before{content:attr(data-placeholder);float:left;color:#a8a8a8;pointer-events:none;height:0}.ProseMirror ol{padding-left:0!important;list-style-type:decimal!important}.ProseMirror ol li::marker{font-size:16px!important}.ProseMirror ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:lower-latin!important}.ProseMirror ol>li>ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:lower-roman!important}.ProseMirror ol>li>ol>li>ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:upper-latin!important}.ProseMirror ol>li>ol>li>ol>li>ol>li>ol{padding-left:10px!important;margin-left:10px!important;list-style-type:upper-roman!important}.ProseMirror ul{list-style-type:disc!important;margin-block-start:0!important;margin-block-end:0!important;margin-inline-start:0px!important;margin-inline-end:0px!important}.ProseMirror ul li{list-style:disc!important}.ProseMirror ul>li>ul{padding-left:10px!important;margin-left:10px!important;list-style-type:disc!important}.ProseMirror{margin:1rem 0}.ProseMirror h1,.ProseMirror h2,.ProseMirror h3,.ProseMirror h4,.ProseMirror h5,.ProseMirror h6{line-height:1.1;text-transform:none;padding:0;background:none!important;border:none!important}.ProseMirror pre{background:#0d0d0d!important;color:#fff!important;font-family:JetBrainsMono,monospace!important;padding:.75rem 1rem!important;border-radius:.5rem!important}.ProseMirror pre code{color:#fff!important;padding:0!important;background:none!important;font-size:.8rem!important}.ProseMirror img{max-width:100%;height:auto}.ProseMirror blockquote{padding-left:1rem;border-left:2px solid rgba(13,13,13,.1)}.ProseMirror hr{border:none;border-top:2px solid rgba(13,13,13,.1);margin:2rem 0!important}.ProseMirror a{text-decoration:underline}.ProseMirror table{border-collapse:collapse;table-layout:fixed;width:100%;margin:0;overflow:hidden}.ProseMirror table td,.ProseMirror table th,.ProseMirror table[show_borders=false]:hover td,.ProseMirror table[show_borders=false]:hover th{min-width:1em;border:2px solid #ced4da;padding:3px 5px;vertical-align:top;box-sizing:border-box;position:relative}.ProseMirror table[show_borders=false] td,.ProseMirror table[show_borders=false] th{border:none;box-sizing:border-box}.ProseMirror table td>*,.ProseMirror table th>*{margin-bottom:0}.ProseMirror table th{font-weight:700;text-align:left;background-color:#f1f3f5}.ProseMirror tr{background-color:#fff!important}.ProseMirror table .selectedCell:after{z-index:2;position:absolute;content:"";inset:0;background:#c8c8ff66;pointer-events:none}.ProseMirror table .column-resize-handle{position:absolute;right:-2px;top:0;bottom:-2px;width:4px;background-color:#adf;pointer-events:none}.tableWrapper{overflow-x:auto}.resize-cursor{cursor:ew-resize;cursor:col-resize}.ProseMirror{padding:0 6px;border:1px solid var(--border-color);border-radius:4px}.prose-editor *,.prose-editor *:before,.prose-editor *:after{box-sizing:inherit}.prose-editor{box-sizing:border-box;position:relative;max-width:120ch;min-width:40ch;flex-grow:1}.prose-editor+textarea{display:none}.prose-menubar{font-size:14px;background:var(--body-bg);display:inline-flex;align-items:center;gap:8px;flex-wrap:wrap;margin-bottom:2px}.prose-menubar__dropdown{display:flex;>span{border-radius:4px}>div{display:none;position:absolute;background:var(--body-bg);z-index:1}&:hover>div{display:flex}}.prose-menubar__group{display:flex}.prose-menubar__button{cursor:pointer;padding:0 .25em;min-width:2em;transition:all .25s;border:1px solid var(--border-color);text-align:center;display:inline-flex;position:relative}.prose-menubar__button--heading .level{position:absolute;right:3px;bottom:2px;font-size:80%}.prose-menubar__button:first-child{border-top-left-radius:4px;border-bottom-left-radius:4px}.prose-menubar__button:last-child{border-top-right-radius:4px;border-bottom-right-radius:4px}.prose-menubar__button+.prose-menubar__button{border-left:none}.prose-menubar__button.material-icons{padding:0 .125em;min-width:auto}.prose-menubar__button:hover{filter:brightness(110%)}.prose-menubar__button.active{background-color:var(--primary)}.prose-menubar__button.disabled{background:var(--border-color);filter:brightness(100%);cursor:not-allowed;opacity:.3}.prose-editor-dialog{background:var(--body-bg);color:var(--body-fg);border:1px solid var(--border-color)}.prose-editor-dialog label{display:block}label:empty:has(+.prose-editor){display:none}.ProseMirror{position:relative}.ProseMirror{word-wrap:break-word;white-space:pre-wrap;white-space:break-spaces;font-variant-ligatures:none;font-feature-settings:"liga" 0}.ProseMirror pre{white-space:pre-wrap}.ProseMirror li{position:relative}.ProseMirror-hideselection *::selection{background:transparent}.ProseMirror-hideselection *::-moz-selection{background:transparent}.ProseMirror-hideselection{caret-color:transparent}.ProseMirror [draggable][contenteditable=false]{-webkit-user-select:text;-moz-user-select:text;user-select:text}.ProseMirror-selectednode{outline:2px solid #8cf}li.ProseMirror-selectednode{outline:none}li.ProseMirror-selectednode:after{content:"";position:absolute;inset:-2px -2px -2px -32px;border:2px solid #8cf;pointer-events:none}img.ProseMirror-separator{display:inline!important;border:none!important;margin:0!important}
```

### Comparing `django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/editor.js` & `django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/editor.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -35,86 +35,86 @@
         value: !0
     }), n);
     var jf = {};
     Js(jf, {
         createEditor: () => zs
     });
 
-    function v(n) {
+    function R(n) {
         this.content = n
     }
-    v.prototype = {
-        constructor: v,
+    R.prototype = {
+        constructor: R,
         find: function(n) {
             for (var e = 0; e < this.content.length; e += 2)
                 if (this.content[e] === n) return e;
             return -1
         },
         get: function(n) {
             var e = this.find(n);
             return e == -1 ? void 0 : this.content[e + 1]
         },
         update: function(n, e, t) {
             var r = t && t != n ? this.remove(t) : this,
                 i = r.find(n),
                 o = r.content.slice();
-            return i == -1 ? o.push(t || n, e) : (o[i + 1] = e, t && (o[i] = t)), new v(o)
+            return i == -1 ? o.push(t || n, e) : (o[i + 1] = e, t && (o[i] = t)), new R(o)
         },
         remove: function(n) {
             var e = this.find(n);
             if (e == -1) return this;
             var t = this.content.slice();
-            return t.splice(e, 2), new v(t)
+            return t.splice(e, 2), new R(t)
         },
         addToStart: function(n, e) {
-            return new v([n, e].concat(this.remove(n).content))
+            return new R([n, e].concat(this.remove(n).content))
         },
         addToEnd: function(n, e) {
             var t = this.remove(n).content.slice();
-            return t.push(n, e), new v(t)
+            return t.push(n, e), new R(t)
         },
         addBefore: function(n, e, t) {
             var r = this.remove(e),
                 i = r.content.slice(),
                 o = r.find(n);
-            return i.splice(o == -1 ? i.length : o, 0, e, t), new v(i)
+            return i.splice(o == -1 ? i.length : o, 0, e, t), new R(i)
         },
         forEach: function(n) {
             for (var e = 0; e < this.content.length; e += 2) n(this.content[e], this.content[e + 1])
         },
         prepend: function(n) {
-            return n = v.from(n), n.size ? new v(n.content.concat(this.subtract(n).content)) : this
+            return n = R.from(n), n.size ? new R(n.content.concat(this.subtract(n).content)) : this
         },
         append: function(n) {
-            return n = v.from(n), n.size ? new v(this.subtract(n).content.concat(n.content)) : this
+            return n = R.from(n), n.size ? new R(this.subtract(n).content.concat(n.content)) : this
         },
         subtract: function(n) {
             var e = this;
-            n = v.from(n);
+            n = R.from(n);
             for (var t = 0; t < n.content.length; t += 2) e = e.remove(n.content[t]);
             return e
         },
         toObject: function() {
             var n = {};
             return this.forEach(function(e, t) {
                 n[e] = t
             }), n
         },
         get size() {
             return this.content.length >> 1
         }
     };
-    v.from = function(n) {
-        if (n instanceof v) return n;
+    R.from = function(n) {
+        if (n instanceof R) return n;
         var e = [];
         if (n)
             for (var t in n) e.push(t, n[t]);
-        return new v(e)
+        return new R(e)
     };
-    var On = v;
+    var On = R;
 
     function _r(n, e, t) {
         for (let r = 0;; r++) {
             if (r == n.childCount || r == e.childCount) return n.childCount == e.childCount ? null : t;
             let i = n.child(r),
                 o = e.child(r);
             if (i == o) {
@@ -500,44 +500,44 @@
     }
 
     function En(n, e, t) {
         let r = n.node(t);
         return Qr(r, e.node(t)), r
     }
 
-    function De(n, e) {
+    function Te(n, e) {
         let t = e.length - 1;
         t >= 0 && n.isText && n.sameMarkup(e[t]) ? e[t] = n.withText(e[t].text + n.text) : e.push(n)
     }
 
     function lt(n, e, t, r) {
         let i = (e || n).node(t),
             o = 0,
             s = e ? e.index(t) : i.childCount;
-        n && (o = n.index(t), n.depth > t ? o++ : n.textOffset && (De(n.nodeAfter, r), o++));
-        for (let l = o; l < s; l++) De(i.child(l), r);
-        e && e.depth == t && e.textOffset && De(e.nodeBefore, r)
+        n && (o = n.index(t), n.depth > t ? o++ : n.textOffset && (Te(n.nodeAfter, r), o++));
+        for (let l = o; l < s; l++) Te(i.child(l), r);
+        e && e.depth == t && e.textOffset && Te(e.nodeBefore, r)
     }
 
     function Ee(n, e) {
         return n.type.checkContent(e), n.copy(e)
     }
 
     function Zr(n, e, t, r, i) {
         let o = n.depth > i && En(n, e, i + 1),
             s = r.depth > i && En(t, r, i + 1),
             l = [];
-        return lt(null, n, i, l), o && s && e.index(i) == t.index(i) ? (Qr(o, s), De(Ee(o, Zr(n, e, t, r, i + 1)), l)) : (o && De(Ee(o, Vt(n, e, i + 1)), l), lt(e, t, i, l), s && De(Ee(s, Vt(t, r, i + 1)), l)), lt(r, null, i, l), new y(l)
+        return lt(null, n, i, l), o && s && e.index(i) == t.index(i) ? (Qr(o, s), Te(Ee(o, Zr(n, e, t, r, i + 1)), l)) : (o && Te(Ee(o, Vt(n, e, i + 1)), l), lt(e, t, i, l), s && Te(Ee(s, Vt(t, r, i + 1)), l)), lt(r, null, i, l), new y(l)
     }
 
     function Vt(n, e, t) {
         let r = [];
         if (lt(null, n, t, r), n.depth > t) {
             let i = En(n, e, t + 1);
-            De(Ee(i, Vt(n, e, t + 1)), r)
+            Te(Ee(i, Vt(n, e, t + 1)), r)
         }
         return lt(e, null, t, r), new y(r)
     }
 
     function $s(n, e) {
         let t = e.depth - n.openStart,
             i = e.node(t).copy(n.content);
@@ -670,20 +670,20 @@
                 return new n(t, r, o)
             }
             static resolveCached(e, t) {
                 for (let i = 0; i < Nn.length; i++) {
                     let o = Nn[i];
                     if (o.pos == t && o.doc == e) return o
                 }
-                let r = Nn[Tn] = n.resolve(e, t);
-                return Tn = (Tn + 1) % Hs, r
+                let r = Nn[Dn] = n.resolve(e, t);
+                return Dn = (Dn + 1) % Hs, r
             }
         },
         Nn = [],
-        Tn = 0,
+        Dn = 0,
         Hs = 12,
         Ie = class {
             constructor(e, t, r) {
                 this.$from = e, this.$to = t, this.depth = r
             }
             get start() {
                 return this.$from.before(this.depth + 1)
@@ -939,15 +939,15 @@
         }
     };
 
     function ei(n, e) {
         for (let t = n.length - 1; t >= 0; t--) e = n[t].type.name + "(" + e + ")";
         return e
     }
-    var Re = class n {
+    var ve = class n {
         constructor(e) {
             this.validEnd = e, this.next = [], this.wrapCache = []
         }
         static parse(e, t) {
             let r = new In(e, t);
             if (r.next == null) return n.empty;
             let i = ti(r);
@@ -1057,15 +1057,15 @@
                 let o = i + (r.validEnd ? "*" : " ") + " ";
                 for (let s = 0; s < r.next.length; s++) o += (s ? ", " : "") + r.next[s].type.name + "->" + e.indexOf(r.next[s].next);
                 return o
             }).join(`
 `)
         }
     };
-    Re.empty = new Re(!0);
+    ve.empty = new ve(!0);
     var In = class {
         constructor(e, t) {
             this.string = e, this.nodeTypes = t, this.inline = null, this.pos = 0, this.tokens = e.split(/\s*(?=\b|\W|$)/), this.tokens[this.tokens.length - 1] == "" && this.tokens.pop(), this.tokens[0] == "" && this.tokens.shift()
         }
         get next() {
             return this.tokens[this.pos]
         }
@@ -1256,15 +1256,15 @@
                     let c;
                     for (let f = 0; f < i.length; f++) i[f][0] == l && (c = i[f][1]);
                     qr(n, a).forEach(f => {
                         c || i.push([l, c = []]), c.indexOf(f) == -1 && c.push(f)
                     })
                 })
             });
-            let o = e[r.join(",")] = new Re(r.indexOf(n.length - 1) > -1);
+            let o = e[r.join(",")] = new ve(r.indexOf(n.length - 1) > -1);
             for (let s = 0; s < i.length; s++) {
                 let l = i[s][1].sort(ni);
                 o.next.push({
                     type: i[s][0],
                     next: e[l.join(",")] || t(l)
                 })
             }
@@ -1311,29 +1311,29 @@
         }
         return t
     }
 
     function oi(n) {
         let e = Object.create(null);
         if (n)
-            for (let t in n) e[t] = new Rn(n[t]);
+            for (let t in n) e[t] = new vn(n[t]);
         return e
     }
     var Jt = class n {
             constructor(e, t, r) {
                 this.name = e, this.schema = t, this.spec = r, this.markSet = null, this.groups = r.group ? r.group.split(" ") : [], this.attrs = oi(r.attrs), this.defaultAttrs = ri(this.attrs), this.contentMatch = null, this.inlineContent = null, this.isBlock = !(r.inline || e == "text"), this.isText = e == "text"
             }
             get isInline() {
                 return !this.isBlock
             }
             get isTextblock() {
                 return this.isBlock && this.inlineContent
             }
             get isLeaf() {
-                return this.contentMatch == Re.empty
+                return this.contentMatch == ve.empty
             }
             get isAtom() {
                 return this.isLeaf || !!this.spec.atom
             }
             get whitespace() {
                 return this.spec.whitespace || (this.spec.code ? "pre" : "normal")
             }
@@ -1396,15 +1396,15 @@
                 let i = t.spec.topNode || "doc";
                 if (!r[i]) throw new RangeError("Schema is missing its top node type ('" + i + "')");
                 if (!r.text) throw new RangeError("Every schema needs a 'text' type");
                 for (let o in r.text.attrs) throw new RangeError("The text node type should not have attributes");
                 return r
             }
         },
-        Rn = class {
+        vn = class {
             constructor(e) {
                 this.hasDefault = Object.prototype.hasOwnProperty.call(e, "default"), this.default = e.default
             }
             get isRequired() {
                 return !this.hasDefault
             }
         },
@@ -1430,27 +1430,27 @@
                 for (let t = 0; t < e.length; t++)
                     if (e[t].type == this) return e[t]
             }
             excludes(e) {
                 return this.excluded.indexOf(e) > -1
             }
         },
-        ke = class {
+        xe = class {
             constructor(e) {
                 this.cached = Object.create(null);
                 let t = this.spec = {};
                 for (let i in e) t[i] = e[i];
                 t.nodes = On.from(e.nodes), t.marks = On.from(e.marks || {}), this.nodes = Jt.compile(this.spec.nodes, this), this.marks = ct.compile(this.spec.marks, this);
                 let r = Object.create(null);
                 for (let i in this.nodes) {
                     if (i in this.marks) throw new RangeError(i + " can not be both a node and a mark");
                     let o = this.nodes[i],
                         s = o.spec.content || "",
                         l = o.spec.marks;
-                    o.contentMatch = r[s] || (r[s] = Re.parse(s, this.nodes)), o.inlineContent = o.contentMatch.inlineContent, o.markSet = l == "_" ? null : l ? Kr(this, l.split(" ")) : l == "" || !o.inlineContent ? [] : null
+                    o.contentMatch = r[s] || (r[s] = ve.parse(s, this.nodes)), o.inlineContent = o.contentMatch.inlineContent, o.markSet = l == "_" ? null : l ? Kr(this, l.split(" ")) : l == "" || !o.inlineContent ? [] : null
                 }
                 for (let i in this.marks) {
                     let o = this.marks[i],
                         s = o.spec.excludes;
                     o.excluded = s == null ? [o] : s == "" ? [] : Kr(this, s.split(" "))
                 }
                 this.nodeFromJSON = this.nodeFromJSON.bind(this), this.markFromJSON = this.markFromJSON.bind(this), this.topNodeType = this.nodes[this.spec.topNode || "doc"], this.cached.wrappings = Object.create(null)
@@ -1502,15 +1502,15 @@
     function tl(n) {
         return n.tag != null
     }
 
     function nl(n) {
         return n.style != null
     }
-    var ve = class n {
+    var Re = class n {
             constructor(e, t) {
                 this.schema = e, this.rules = t, this.tags = [], this.styles = [], t.forEach(r => {
                     tl(r) ? this.tags.push(r) : nl(r) && this.styles.push(r)
                 }), this.normalizeLists = !this.tags.some(r => {
                     if (!/^(ul|ol)\b/.test(r.tag) || !r.node) return !1;
                     let i = e.nodes[r.node];
                     return i.contentMatch.matchType(i)
@@ -1958,15 +1958,15 @@
             if (n.eq(e[t])) return e[t]
     }
     var ie = class n {
         constructor(e, t) {
             this.nodes = e, this.marks = t
         }
         serializeFragment(e, t = {}, r) {
-            r || (r = Dn(t).createDocumentFragment());
+            r || (r = Tn(t).createDocumentFragment());
             let i = r,
                 o = [];
             return e.forEach(s => {
                 if (o.length || s.marks.length) {
                     let l = 0,
                         a = 0;
                     for (; l < o.length && a < s.marks.length;) {
@@ -1988,15 +1988,15 @@
                 i.appendChild(this.serializeNodeInner(s, t))
             }), r
         }
         serializeNodeInner(e, t) {
             let {
                 dom: r,
                 contentDOM: i
-            } = n.renderSpec(Dn(t), this.nodes[e.type.name](e));
+            } = n.renderSpec(Tn(t), this.nodes[e.type.name](e));
             if (i) {
                 if (e.isLeaf) throw new RangeError("Content hole not allowed in a leaf node spec");
                 this.serializeFragment(e.content, t, i)
             }
             return r
         }
         serializeNode(e, t = {}) {
@@ -2005,15 +2005,15 @@
                 let o = this.serializeMark(e.marks[i], e.isInline, t);
                 o && ((o.contentDOM || o.dom).appendChild(r), r = o.dom)
             }
             return r
         }
         serializeMark(e, t, r = {}) {
             let i = this.marks[e.type.name];
-            return i && n.renderSpec(Dn(r), i(e, t))
+            return i && n.renderSpec(Tn(r), i(e, t))
         }
         static renderSpec(e, t, r = null) {
             if (typeof t == "string") return {
                 dom: e.createTextNode(t)
             };
             if (t.nodeType != null) return {
                 dom: t
@@ -2074,15 +2074,15 @@
         for (let t in n) {
             let r = n[t].spec.toDOM;
             r && (e[t] = r)
         }
         return e
     }
 
-    function Dn(n) {
+    function Tn(n) {
         return n.document || window.document
     }
     var fi = 65535,
         hi = Math.pow(2, 16);
 
     function cl(n, e) {
         return n + e * hi
@@ -2252,31 +2252,31 @@
                         }
                     }
                     i |= l.delInfo, e = l.pos
                 }
                 return r ? e : new dt(e, i, null)
             }
         },
-        vn = Object.create(null),
-        D = class {
+        Rn = Object.create(null),
+        T = class {
             getMap() {
                 return he.empty
             }
             merge(e) {
                 return null
             }
             static fromJSON(e, t) {
                 if (!t || !t.stepType) throw new RangeError("Invalid input for Step.fromJSON");
-                let r = vn[t.stepType];
+                let r = Rn[t.stepType];
                 if (!r) throw new RangeError(`No step type ${t.stepType} defined`);
                 return r.fromJSON(e, t)
             }
             static jsonID(e, t) {
-                if (e in vn) throw new RangeError("Duplicate use of step JSON ID " + e);
-                return vn[e] = t, t.prototype.jsonID = e, t
+                if (e in Rn) throw new RangeError("Duplicate use of step JSON ID " + e);
+                return Rn[e] = t, t.prototype.jsonID = e, t
             }
         },
         A = class n {
             constructor(e, t) {
                 this.doc = e, this.failed = t
             }
             static ok(e) {
@@ -2299,15 +2299,15 @@
         let r = [];
         for (let i = 0; i < n.childCount; i++) {
             let o = n.child(i);
             o.content.size && (o = o.copy(Vn(o.content, e, o))), o.isInline && (o = e(o, t, i)), r.push(o)
         }
         return y.fromArray(r)
     }
-    var pt = class n extends D {
+    var pt = class n extends T {
         constructor(e, t, r) {
             super(), this.from = e, this.to = t, this.mark = r
         }
         apply(e) {
             let t = e.slice(this.from, this.to),
                 r = e.resolve(this.from),
                 i = r.node(r.sharedDepth(this.to)),
@@ -2334,16 +2334,16 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.from != "number" || typeof t.to != "number") throw new RangeError("Invalid input for AddMarkStep.fromJSON");
             return new n(t.from, t.to, e.markFromJSON(t.mark))
         }
     };
-    D.jsonID("addMark", pt);
-    var Pe = class n extends D {
+    T.jsonID("addMark", pt);
+    var Pe = class n extends T {
         constructor(e, t, r) {
             super(), this.from = e, this.to = t, this.mark = r
         }
         apply(e) {
             let t = e.slice(this.from, this.to),
                 r = new b(Vn(t.content, i => i.mark(this.mark.removeFromSet(i.marks)), e), t.openStart, t.openEnd);
             return A.fromReplace(e, this.from, this.to, r)
@@ -2368,16 +2368,16 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.from != "number" || typeof t.to != "number") throw new RangeError("Invalid input for RemoveMarkStep.fromJSON");
             return new n(t.from, t.to, e.markFromJSON(t.mark))
         }
     };
-    D.jsonID("removeMark", Pe);
-    var mt = class n extends D {
+    T.jsonID("removeMark", Pe);
+    var mt = class n extends T {
         constructor(e, t) {
             super(), this.pos = e, this.mark = t
         }
         apply(e) {
             let t = e.nodeAt(this.pos);
             if (!t) return A.fail("No node at mark step's position");
             let r = t.type.create(t.attrs, null, this.mark.addToSet(t.marks));
@@ -2407,16 +2407,16 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.pos != "number") throw new RangeError("Invalid input for AddNodeMarkStep.fromJSON");
             return new n(t.pos, e.markFromJSON(t.mark))
         }
     };
-    D.jsonID("addNodeMark", mt);
-    var gt = class n extends D {
+    T.jsonID("addNodeMark", mt);
+    var gt = class n extends T {
         constructor(e, t) {
             super(), this.pos = e, this.mark = t
         }
         apply(e) {
             let t = e.nodeAt(this.pos);
             if (!t) return A.fail("No node at mark step's position");
             let r = t.type.create(t.attrs, null, this.mark.removeFromSet(t.marks));
@@ -2438,16 +2438,16 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.pos != "number") throw new RangeError("Invalid input for RemoveNodeMarkStep.fromJSON");
             return new n(t.pos, e.markFromJSON(t.mark))
         }
     };
-    D.jsonID("removeNodeMark", gt);
-    var K = class n extends D {
+    T.jsonID("removeNodeMark", gt);
+    var K = class n extends T {
         constructor(e, t, r, i = !1) {
             super(), this.from = e, this.to = t, this.slice = r, this.structure = i
         }
         apply(e) {
             return this.structure && Bn(e, this.from, this.to) ? A.fail("Structure replace would overwrite content") : A.fromReplace(e, this.from, this.to, this.slice)
         }
         getMap() {
@@ -2480,16 +2480,16 @@
             return this.slice.size && (e.slice = this.slice.toJSON()), this.structure && (e.structure = !0), e
         }
         static fromJSON(e, t) {
             if (typeof t.from != "number" || typeof t.to != "number") throw new RangeError("Invalid input for ReplaceStep.fromJSON");
             return new n(t.from, t.to, b.fromJSON(e, t.slice), !!t.structure)
         }
     };
-    D.jsonID("replace", K);
-    var E = class n extends D {
+    T.jsonID("replace", K);
+    var E = class n extends T {
         constructor(e, t, r, i, o, s, l = !1) {
             super(), this.from = e, this.to = t, this.gapFrom = r, this.gapTo = i, this.slice = o, this.insert = s, this.structure = l
         }
         apply(e) {
             if (this.structure && (Bn(e, this.from, this.gapFrom) || Bn(e, this.gapTo, this.to))) return A.fail("Structure gap-replace would overwrite content");
             let t = e.slice(this.gapFrom, this.gapTo);
             if (t.openStart || t.openEnd) return A.fail("Gap is not a flat range");
@@ -2522,15 +2522,15 @@
             return this.slice.size && (e.slice = this.slice.toJSON()), this.structure && (e.structure = !0), e
         }
         static fromJSON(e, t) {
             if (typeof t.from != "number" || typeof t.to != "number" || typeof t.gapFrom != "number" || typeof t.gapTo != "number" || typeof t.insert != "number") throw new RangeError("Invalid input for ReplaceAroundStep.fromJSON");
             return new n(t.from, t.to, t.gapFrom, t.gapTo, b.fromJSON(e, t.slice), t.insert, !!t.structure)
         }
     };
-    D.jsonID("replaceAround", E);
+    T.jsonID("replaceAround", E);
 
     function Bn(n, e, t) {
         let r = n.resolve(e),
             i = t - e,
             o = r.depth;
         for (; i > 0 && o > 0 && r.indexAfter(o) == r.node(o).childCount;) o--, i--;
         if (i > 0) {
@@ -2697,29 +2697,29 @@
             r = y.from(t[s].type.create(t[s].attrs, r))
         }
         let i = e.start,
             o = e.end;
         n.step(new E(i, o, i, o, new b(r, 0, 0), t.length, !0))
     }
 
-    function kl(n, e, t, r, i) {
+    function xl(n, e, t, r, i) {
         if (!r.isTextblock) throw new RangeError("Type given to setBlockType should be a textblock");
         let o = n.steps.length;
         n.doc.nodesBetween(e, t, (s, l) => {
-            if (s.isTextblock && !s.hasMarkup(r, i) && xl(n.doc, n.mapping.slice(o).map(l), r)) {
+            if (s.isTextblock && !s.hasMarkup(r, i) && kl(n.doc, n.mapping.slice(o).map(l), r)) {
                 n.clearIncompatible(n.mapping.slice(o).map(l, 1), r);
                 let a = n.mapping.slice(o),
                     c = a.map(l, 1),
                     f = a.map(l + s.nodeSize, 1);
                 return n.step(new E(c, f, c + 1, f - 1, new b(y.from(r.create(i, null, s.marks)), 0, 0), 1, !0)), !1
             }
         })
     }
 
-    function xl(n, e, t) {
+    function kl(n, e, t) {
         let r = n.resolve(e),
             i = r.index();
         return r.parent.canReplaceWith(i, i + 1, t)
     }
 
     function Sl(n, e, t, r, i) {
         let o = n.doc.nodeAt(e);
@@ -2727,15 +2727,15 @@
         t || (t = o.type);
         let s = t.create(r, null, i || o.marks);
         if (o.isLeaf) return n.replaceWith(e, e + o.nodeSize, s);
         if (!t.validContent(o.content)) throw new RangeError("Invalid content for node type " + t.name);
         n.step(new E(e, e + o.nodeSize, e + 1, e + o.nodeSize - 1, new b(y.from(s), 0, 0), 1, !0))
     }
 
-    function xe(n, e, t = 1, r) {
+    function ke(n, e, t = 1, r) {
         let i = n.resolve(e),
             o = i.depth - t,
             s = r && r[r.length - 1] || i.parent;
         if (o < 0 || i.parent.type.spec.isolating || !i.parent.canReplace(i.index(), i.parent.childCount) || !s.type.validContent(i.parent.content.cutByIndex(i.index(), i.parent.childCount))) return !1;
         for (let c = i.depth - 1, f = t - 2; c > o; c--, f--) {
             let h = i.node(c),
                 d = i.index(c);
@@ -2943,19 +2943,19 @@
                     g = h.matchType(m.type);
                 if (!g) break;
                 c++, (c > 1 || a == 0 || m.content.size) && (h = g, f.push(gi(m.mark(d.allowedMarks(m.marks)), c == 1 ? a : 0, c == l.childCount ? p : -1)))
             }
             let u = c == l.childCount;
             u || (p = -1), this.placed = ht(this.placed, t, y.from(f)), this.frontier[t].match = h, u && p < 0 && r && r.type == this.frontier[this.depth].type && this.frontier.length > 1 && this.closeFrontierNode();
             for (let m = 0, g = l; m < p; m++) {
-                let k = g.lastChild;
+                let x = g.lastChild;
                 this.frontier.push({
-                    type: k.type,
-                    match: k.contentMatchAt(k.childCount)
-                }), g = k.content
+                    type: x.type,
+                    match: x.contentMatchAt(x.childCount)
+                }), g = x.content
             }
             this.unplaced = u ? e == 0 ? b.empty : new b(ft(s.content, e - 1, 1), e - 1, p < 0 ? s.openEnd : e - 1) : new b(ft(s.content, e, c), s.openStart, s.openEnd)
         }
         mustMoveInline() {
             if (!this.$to.parent.isTextblock) return -1;
             let e = this.frontier[this.depth],
                 t;
@@ -3042,19 +3042,19 @@
 
     function Nl(n, e, t) {
         for (let r = t; r < e.childCount; r++)
             if (!n.allowsMarks(e.child(r).marks)) return !0;
         return !1
     }
 
-    function Tl(n) {
+    function Dl(n) {
         return n.spec.defining || n.spec.definingForContent
     }
 
-    function Dl(n, e, t, r) {
+    function Tl(n, e, t, r) {
         if (!r.size) return n.deleteRange(e, t);
         let i = n.doc.resolve(e),
             o = n.doc.resolve(t);
         if (mi(i, o, r)) return n.step(new K(e, t, r));
         let s = bi(i, n.doc.resolve(t));
         s[s.length - 1] == 0 && s.pop();
         let l = -(i.depth + 1);
@@ -3070,29 +3070,29 @@
         for (let d = r.content, p = 0;; p++) {
             let u = d.firstChild;
             if (c.push(u), p == r.openStart) break;
             d = u.content
         }
         for (let d = f - 1; d >= 0; d--) {
             let p = c[d],
-                u = Tl(p.type);
+                u = Dl(p.type);
             if (u && !p.sameMarkup(i.node(Math.abs(l) - 1))) f = d;
             else if (u || !p.type.isTextblock) break
         }
         for (let d = r.openStart; d >= 0; d--) {
             let p = (d + f + 1) % (r.openStart + 1),
                 u = c[p];
             if (u)
                 for (let m = 0; m < s.length; m++) {
                     let g = s[(m + a) % s.length],
-                        k = !0;
-                    g < 0 && (k = !1, g = -g);
+                        x = !0;
+                    g < 0 && (x = !1, g = -g);
                     let N = i.node(g - 1),
                         ee = i.index(g - 1);
-                    if (N.canReplaceWith(ee, ee, u.type, u.marks)) return n.replace(i.before(g), k ? o.after(g) : t, new b(yi(r.content, 0, r.openStart, p), p, r.openEnd))
+                    if (N.canReplaceWith(ee, ee, u.type, u.marks)) return n.replace(i.before(g), x ? o.after(g) : t, new b(yi(r.content, 0, r.openStart, p), p, r.openEnd))
                 }
         }
         let h = n.steps.length;
         for (let d = s.length - 1; d >= 0 && (n.replace(e, t, r), !(n.steps.length > h)); d--) {
             let p = s[d];
             p < 0 || (e = i.before(p), t = o.after(p))
         }
@@ -3140,15 +3140,15 @@
         for (let i = r; i >= 0; i--) {
             let o = n.start(i);
             if (o < n.pos - (n.depth - i) || e.end(i) > e.pos + (e.depth - i) || n.node(i).type.spec.isolating || e.node(i).type.spec.isolating) break;
             (o == e.start(i) || i == n.depth && i == e.depth && n.parent.inlineContent && e.parent.inlineContent && i && e.start(i - 1) == o - 1) && t.push(i)
         }
         return t
     }
-    var Ht = class n extends D {
+    var Ht = class n extends T {
         constructor(e, t, r) {
             super(), this.pos = e, this.attr = t, this.value = r
         }
         apply(e) {
             let t = e.nodeAt(this.pos);
             if (!t) return A.fail("No node at attribute step's position");
             let r = Object.create(null);
@@ -3176,16 +3176,16 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.pos != "number" || typeof t.attr != "string") throw new RangeError("Invalid input for AttrStep.fromJSON");
             return new n(t.pos, t.attr, t.value)
         }
     };
-    D.jsonID("attr", Ht);
-    var jt = class n extends D {
+    T.jsonID("attr", Ht);
+    var jt = class n extends T {
         constructor(e, t) {
             super(), this.attr = e, this.value = t
         }
         apply(e) {
             let t = Object.create(null);
             for (let i in e.attrs) t[i] = e.attrs[i];
             t[this.attr] = this.value;
@@ -3209,15 +3209,15 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.attr != "string") throw new RangeError("Invalid input for DocAttrStep.fromJSON");
             return new n(t.attr, t.value)
         }
     };
-    D.jsonID("docAttr", jt);
+    T.jsonID("docAttr", jt);
     var _e = class extends Error {};
     _e = function n(e) {
         let t = Error.call(this, e);
         return t.__proto__ = n.prototype, t
     };
     _e.prototype = Object.create(Error.prototype);
     _e.prototype.constructor = _e;
@@ -3254,15 +3254,15 @@
         delete(e, t) {
             return this.replace(e, t, b.empty)
         }
         insert(e, t) {
             return this.replaceWith(e, e, t)
         }
         replaceRange(e, t, r) {
-            return Dl(this, e, t, r), this
+            return Tl(this, e, t, r), this
         }
         replaceRangeWith(e, t, r) {
             return El(this, e, t, r), this
         }
         deleteRange(e, t) {
             return Al(this, e, t), this
         }
@@ -3272,15 +3272,15 @@
         join(e, t = 1) {
             return Ol(this, e, t), this
         }
         wrap(e, t) {
             return bl(this, e, t), this
         }
         setBlockType(e, t = e, r, i = null) {
-            return kl(this, e, t, r, i), this
+            return xl(this, e, t, r, i), this
         }
         setNodeMarkup(e, t, r = null, i) {
             return Sl(this, e, t, r, i), this
         }
         setNodeAttribute(e, t, r) {
             return this.step(new Ht(e, t, r)), this
         }
@@ -3402,22 +3402,22 @@
         };
     S.prototype.visible = !0;
     var Wn = class {
             constructor(e, t) {
                 this.$from = e, this.$to = t
             }
         },
-        ki = !1;
+        xi = !1;
 
-    function xi(n) {
-        !ki && !n.parent.inlineContent && (ki = !0, console.warn("TextSelection endpoint not pointing into a node with inline content (" + n.parent.type.name + ")"))
+    function ki(n) {
+        !xi && !n.parent.inlineContent && (xi = !0, console.warn("TextSelection endpoint not pointing into a node with inline content (" + n.parent.type.name + ")"))
     }
     var w = class n extends S {
         constructor(e, t = e) {
-            xi(e), xi(t), super(e, t)
+            ki(e), ki(t), super(e, t)
         }
         get $cursor() {
             return this.$anchor.pos == this.$head.pos ? this.$head : null
         }
         map(e, t) {
             let r = e.resolve(t.map(this.head));
             if (!r.parent.inlineContent) return S.near(r);
@@ -3469,15 +3469,15 @@
             map(e) {
                 return new n(e.map(this.anchor), e.map(this.head))
             }
             resolve(e) {
                 return w.between(e.resolve(this.anchor), e.resolve(this.head))
             }
         },
-        x = class n extends S {
+        k = class n extends S {
             constructor(e) {
                 let t = e.nodeAfter,
                     r = e.node(0).resolve(e.pos + t.nodeSize);
                 super(e, r), this.node = t
             }
             map(e, t) {
                 let {
@@ -3508,31 +3508,31 @@
             static create(e, t) {
                 return new n(e.resolve(t))
             }
             static isSelectable(e) {
                 return !e.isText && e.type.spec.selectable !== !1
             }
         };
-    x.prototype.visible = !1;
-    S.jsonID("node", x);
+    k.prototype.visible = !1;
+    S.jsonID("node", k);
     var qn = class n {
             constructor(e) {
                 this.anchor = e
             }
             map(e) {
                 let {
                     deleted: t,
                     pos: r
                 } = e.mapResult(this.anchor);
                 return t ? new Qt(r, r) : new n(r)
             }
             resolve(e) {
                 let t = e.resolve(this.anchor),
                     r = t.nodeAfter;
-                return r && x.isSelectable(r) ? new x(t) : S.near(t)
+                return r && k.isSelectable(r) ? new k(t) : S.near(t)
             }
         },
         $ = class n extends S {
             constructor(e) {
                 super(e.resolve(0), e.resolve(e.content.size))
             }
             replace(e, t = b.empty) {
@@ -3571,15 +3571,15 @@
     };
 
     function Ge(n, e, t, r, i, o = !1) {
         if (e.inlineContent) return w.create(n, t);
         for (let s = r - (i > 0 ? 0 : 1); i > 0 ? s < e.childCount : s >= 0; s += i) {
             let l = e.child(s);
             if (l.isAtom) {
-                if (!o && x.isSelectable(l)) return x.create(n, t - (i < 0 ? l.nodeSize : 0))
+                if (!o && k.isSelectable(l)) return k.create(n, t - (i < 0 ? l.nodeSize : 0))
             } else {
                 let a = Ge(n, l, t + i, i < 0 ? l.childCount : 0, i, o);
                 if (a) return a
             }
             t += l.nodeSize * i
         }
         return null
@@ -3679,15 +3679,15 @@
         return !e || !n ? n : n.bind(e)
     }
     var ze = class {
             constructor(e, t, r) {
                 this.name = e, this.init = Oi(t.init, r), this.apply = Oi(t.apply, r)
             }
         },
-        Rl = [new ze("doc", {
+        vl = [new ze("doc", {
             init(n) {
                 return n.doc || n.schema.topNodeType.createAndFill()
             },
             apply(n) {
                 return n.doc
             }
         }), new ze("selection", {
@@ -3710,15 +3710,15 @@
             },
             apply(n, e) {
                 return n.scrolledIntoView ? e + 1 : e
             }
         })],
         bt = class {
             constructor(e, t) {
-                this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = Rl.slice(), t && t.forEach(r => {
+                this.schema = e, this.plugins = [], this.pluginsByKey = Object.create(null), this.fields = vl.slice(), t && t.forEach(r => {
                     if (this.pluginsByKey[r.key]) throw new RangeError("Adding different instances of a keyed plugin (" + r.key + ")");
                     this.plugins.push(r), this.pluginsByKey[r.key] = r, r.spec.state && this.fields.push(new ze(r.key, r.spec.state, r))
                 })
             }
         },
         Zt = class n {
             constructor(e) {
@@ -3865,50 +3865,50 @@
             }
         },
         Jn = Object.create(null);
 
     function Ni(n) {
         return n in Jn ? n + "$" + ++Jn[n] : (Jn[n] = 0, n + "$")
     }
-    var kt = class {
+    var xt = class {
         constructor(e = "key") {
             this.key = Ni(e)
         }
         get(e) {
             return e.config.pluginsByKey[this.key]
         }
         getState(e) {
             return e[this.key]
         }
     };
-    var Di = (n, e) => n.selection.empty ? !1 : (e && e(n.tr.deleteSelection().scrollIntoView()), !0);
+    var Ti = (n, e) => n.selection.empty ? !1 : (e && e(n.tr.deleteSelection().scrollIntoView()), !0);
 
-    function vl(n, e) {
+    function Rl(n, e) {
         let {
             $cursor: t
         } = n.selection;
         return !t || (e ? !e.endOfTextblock("backward", n) : t.parentOffset > 0) ? null : t
     }
     var Pl = (n, e, t) => {
-        let r = vl(n, t);
+        let r = Rl(n, t);
         if (!r) return !1;
         let i = Ei(r);
         if (!i) {
             let s = r.blockRange(),
                 l = s && Ue(s);
             return l == null ? !1 : (e && e(n.tr.lift(s, l).scrollIntoView()), !0)
         }
         let o = i.nodeBefore;
         if (!o.type.spec.isolating && Ii(n, i, e)) return !0;
-        if (r.parent.content.size == 0 && (Ye(o, "end") || x.isSelectable(o))) {
+        if (r.parent.content.size == 0 && (Ye(o, "end") || k.isSelectable(o))) {
             let s = Yt(n.doc, r.before(), r.after(), b.empty);
             if (s && s.slice.size < s.to - s.from) {
                 if (e) {
                     let l = n.tr.step(s);
-                    l.setSelection(Ye(o, "end") ? S.findFrom(l.doc.resolve(l.mapping.map(i.pos, -1)), -1) : x.create(l.doc, i.pos - o.nodeSize)), e(l.scrollIntoView())
+                    l.setSelection(Ye(o, "end") ? S.findFrom(l.doc.resolve(l.mapping.map(i.pos, -1)), -1) : k.create(l.doc, i.pos - o.nodeSize)), e(l.scrollIntoView())
                 }
                 return !0
             }
         }
         return o.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos - o.nodeSize, i.pos).scrollIntoView()), !0) : !1
     };
 
@@ -3926,15 +3926,15 @@
         } = n.selection, o = r;
         if (!i) return !1;
         if (r.parent.isTextblock) {
             if (t ? !t.endOfTextblock("backward", n) : r.parentOffset > 0) return !1;
             o = Ei(r)
         }
         let s = o && o.nodeBefore;
-        return !s || !x.isSelectable(s) ? !1 : (e && e(n.tr.setSelection(x.create(n.doc, o.pos - s.nodeSize)).scrollIntoView()), !0)
+        return !s || !k.isSelectable(s) ? !1 : (e && e(n.tr.setSelection(k.create(n.doc, o.pos - s.nodeSize)).scrollIntoView()), !0)
     };
 
     function Ei(n) {
         if (!n.parent.type.spec.isolating)
             for (let e = n.depth - 1; e >= 0; e--) {
                 if (n.index(e) > 0) return n.doc.resolve(n.before(e + 1));
                 if (n.node(e).type.spec.isolating) break
@@ -3951,20 +3951,20 @@
     var Fl = (n, e, t) => {
             let r = Bl(n, t);
             if (!r) return !1;
             let i = Ai(r);
             if (!i) return !1;
             let o = i.nodeAfter;
             if (Ii(n, i, e)) return !0;
-            if (r.parent.content.size == 0 && (Ye(o, "start") || x.isSelectable(o))) {
+            if (r.parent.content.size == 0 && (Ye(o, "start") || k.isSelectable(o))) {
                 let s = Yt(n.doc, r.before(), r.after(), b.empty);
                 if (s && s.slice.size < s.to - s.from) {
                     if (e) {
                         let l = n.tr.step(s);
-                        l.setSelection(Ye(o, "start") ? S.findFrom(l.doc.resolve(l.mapping.map(i.pos)), 1) : x.create(l.doc, l.mapping.map(i.pos))), e(l.scrollIntoView())
+                        l.setSelection(Ye(o, "start") ? S.findFrom(l.doc.resolve(l.mapping.map(i.pos)), 1) : k.create(l.doc, l.mapping.map(i.pos))), e(l.scrollIntoView())
                     }
                     return !0
                 }
             }
             return o.isAtom && i.depth == r.depth - 1 ? (e && e(n.tr.delete(i.pos, i.pos + o.nodeSize).scrollIntoView()), !0) : !1
         },
         Vl = (n, e, t) => {
@@ -3974,15 +3974,15 @@
             } = n.selection, o = r;
             if (!i) return !1;
             if (r.parent.isTextblock) {
                 if (t ? !t.endOfTextblock("forward", n) : r.parentOffset < r.parent.content.size) return !1;
                 o = Ai(r)
             }
             let s = o && o.nodeAfter;
-            return !s || !x.isSelectable(s) ? !1 : (e && e(n.tr.setSelection(x.create(n.doc, o.pos)).scrollIntoView()), !0)
+            return !s || !k.isSelectable(s) ? !1 : (e && e(n.tr.setSelection(k.create(n.doc, o.pos)).scrollIntoView()), !0)
         };
 
     function Ai(n) {
         if (!n.parent.type.spec.isolating)
             for (let e = n.depth - 1; e >= 0; e--) {
                 let t = n.node(e);
                 if (n.index(e) + 1 < t.childCount) return n.doc.resolve(n.after(e + 1));
@@ -4044,40 +4044,40 @@
         Wl = (n, e) => {
             let {
                 $cursor: t
             } = n.selection;
             if (!t || t.parent.content.size) return !1;
             if (t.depth > 1 && t.after() != t.end(-1)) {
                 let o = t.before();
-                if (xe(n.doc, o)) return e && e(n.tr.split(o).scrollIntoView()), !0
+                if (ke(n.doc, o)) return e && e(n.tr.split(o).scrollIntoView()), !0
             }
             let r = t.blockRange(),
                 i = r && Ue(r);
             return i == null ? !1 : (e && e(n.tr.lift(r, i).scrollIntoView()), !0)
         };
 
     function ql(n) {
         return (e, t) => {
             let {
                 $from: r,
                 $to: i
             } = e.selection;
-            if (e.selection instanceof x && e.selection.node.isBlock) return !r.parentOffset || !xe(e.doc, r.pos) ? !1 : (t && t(e.tr.split(r.pos).scrollIntoView()), !0);
+            if (e.selection instanceof k && e.selection.node.isBlock) return !r.parentOffset || !ke(e.doc, r.pos) ? !1 : (t && t(e.tr.split(r.pos).scrollIntoView()), !0);
             if (!r.parent.isBlock) return !1;
             if (t) {
                 let o = i.parentOffset == i.parent.content.size,
                     s = e.tr;
                 (e.selection instanceof w || e.selection instanceof $) && s.deleteSelection();
                 let l = r.depth == 0 ? null : Hn(r.node(-1).contentMatchAt(r.indexAfter(-1))),
                     a = n && n(i.parent, o),
                     c = a ? [a] : o && l ? [{
                         type: l
                     }] : void 0,
-                    f = xe(s.doc, s.mapping.map(r.pos), 1, c);
-                if (!c && !f && xe(s.doc, s.mapping.map(r.pos), 1, l ? [{
+                    f = ke(s.doc, s.mapping.map(r.pos), 1, c);
+                if (!c && !f && ke(s.doc, s.mapping.map(r.pos), 1, l ? [{
                         type: l
                     }] : void 0) && (l && (c = [{
                         type: l
                     }]), f = !0), f && (s.split(s.mapping.map(r.pos), 1, c), !o && !r.parentOffset && r.parent.type != l)) {
                     let h = s.mapping.map(r.before()),
                         d = s.doc.resolve(h);
                     l && r.node(-1).canReplaceWith(d.index(), d.index() + 1, l) && s.setNodeMarkup(s.mapping.map(r.before()), l)
@@ -4126,38 +4126,38 @@
             for (; d.push(h), !h.isTextblock;) h = h.lastChild;
             let p = i,
                 u = 1;
             for (; !p.isTextblock; p = p.firstChild) u++;
             if (h.canReplace(h.childCount, h.childCount, p.content)) {
                 if (t) {
                     let m = y.empty;
-                    for (let k = d.length - 1; k >= 0; k--) m = y.from(d[k].copy(m));
+                    for (let x = d.length - 1; x >= 0; x--) m = y.from(d[x].copy(m));
                     let g = n.tr.step(new E(e.pos - d.length, e.pos + i.nodeSize, e.pos + u, e.pos + i.nodeSize - u, new b(m, d.length, 0), 0, !0));
                     t(g.scrollIntoView())
                 }
                 return !0
             }
         }
         return !1
     }
 
-    function Ri(n) {
+    function vi(n) {
         return function(e, t) {
             let r = e.selection,
                 i = n < 0 ? r.$from : r.$to,
                 o = i.depth;
             for (; i.node(o).isInline;) {
                 if (!o) return !1;
                 o--
             }
             return i.node(o).isTextblock ? (t && t(e.tr.setSelection(w.create(e.doc, n < 0 ? i.start(o) : i.end(o)))), !0) : !1
         }
     }
-    var jl = Ri(-1),
-        _l = Ri(1);
+    var jl = vi(-1),
+        _l = vi(1);
 
     function en(n, e = null) {
         return function(t, r) {
             let {
                 $from: i,
                 $to: o
             } = t.selection, s = i.blockRange(o), l = s && Ut(s, n, e);
@@ -4218,15 +4218,15 @@
                     if (s) return !1;
                     s = l.inlineContent && l.type.allowsMarkType(t)
                 }), s) return !0
         }
         return !1
     }
 
-    function G(n, e = null) {
+    function X(n, e = null) {
         return function(t, r) {
             let {
                 empty: i,
                 $cursor: o,
                 ranges: s
             } = t.selection;
             if (i && !o || !Ul(t.doc, s, n)) return !1;
@@ -4250,55 +4250,55 @@
                         if (l) a.removeMark(f.pos, h.pos, n);
                         else {
                             let d = f.pos,
                                 p = h.pos,
                                 u = f.nodeAfter,
                                 m = h.nodeBefore,
                                 g = u && u.isText ? /^\s*/.exec(u.text)[0].length : 0,
-                                k = m && m.isText ? /\s*$/.exec(m.text)[0].length : 0;
-                            d + g < p && (d += g, p -= k), a.addMark(d, p, n.create(e))
+                                x = m && m.isText ? /\s*$/.exec(m.text)[0].length : 0;
+                            d + g < p && (d += g, p -= x), a.addMark(d, p, n.create(e))
                         }
                     }
                     r(a.scrollIntoView())
                 } return !0
         }
     }
 
-    function xt(...n) {
+    function kt(...n) {
         return function(e, t, r) {
             for (let i = 0; i < n.length; i++)
                 if (n[i](e, t, r)) return !0;
             return !1
         }
     }
-    var $n = xt(Di, Pl, zl),
-        Ti = xt(Di, Fl, Vl),
+    var $n = kt(Ti, Pl, zl),
+        Di = kt(Ti, Fl, Vl),
         de = {
-            Enter: xt(Ll, Jl, Wl, Kl),
+            Enter: kt(Ll, Jl, Wl, Kl),
             "Mod-Enter": jn,
             Backspace: $n,
             "Mod-Backspace": $n,
             "Shift-Backspace": $n,
-            Delete: Ti,
-            "Mod-Delete": Ti,
+            Delete: Di,
+            "Mod-Delete": Di,
             "Mod-a": $l
         },
-        vi = {
+        Ri = {
             "Ctrl-h": de.Backspace,
             "Alt-Backspace": de["Mod-Backspace"],
             "Ctrl-d": de.Delete,
             "Ctrl-Alt-Backspace": de["Mod-Delete"],
             "Alt-Delete": de["Mod-Delete"],
             "Alt-d": de["Mod-Delete"],
             "Ctrl-a": jl,
             "Ctrl-e": _l
         };
-    for (let n in de) vi[n] = de[n];
+    for (let n in de) Ri[n] = de[n];
     var Gl = typeof navigator != "undefined" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : typeof os != "undefined" && os.platform ? os.platform() == "darwin" : !1,
-        Pi = Gl ? vi : de;
+        Pi = Gl ? Ri : de;
 
     function zi(n = {}) {
         return new J({
             view(e) {
                 return new Un(e, n)
             }
         })
@@ -4477,20 +4477,20 @@
             219: "{",
             220: "|",
             221: "}",
             222: '"'
         },
         Yl = typeof navigator != "undefined" && /Mac/.test(navigator.platform),
         Xl = typeof navigator != "undefined" && /MSIE \d|Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(navigator.userAgent);
-    for (T = 0; T < 10; T++) ue[48 + T] = ue[96 + T] = String(T);
-    var T;
-    for (T = 1; T <= 24; T++) ue[T + 111] = "F" + T;
-    var T;
-    for (T = 65; T <= 90; T++) ue[T] = String.fromCharCode(T + 32), nn[T] = String.fromCharCode(T);
-    var T;
+    for (D = 0; D < 10; D++) ue[48 + D] = ue[96 + D] = String(D);
+    var D;
+    for (D = 1; D <= 24; D++) ue[D + 111] = "F" + D;
+    var D;
+    for (D = 65; D <= 90; D++) ue[D] = String.fromCharCode(D + 32), nn[D] = String.fromCharCode(D);
+    var D;
     for (tn in ue) nn.hasOwnProperty(tn) || (nn[tn] = ue[tn]);
     var tn;
 
     function Bi(n) {
         var e = Yl && n.metaKey && n.shiftKey && !n.ctrlKey && !n.altKey || Xl && n.shiftKey && n.key && n.key.length == 1 || n.key == "Unidentified",
             t = !e && n.key || (n.shiftKey ? nn : ue)[n.keyCode] || n.key || "Unidentified";
         return t == "Esc" && (t = "Escape"), t == "Del" && (t = "Delete"), t == "Left" && (t = "ArrowLeft"), t == "Up" && (t = "ArrowUp"), t == "Right" && (t = "ArrowRight"), t == "Down" && (t = "ArrowDown"), t
@@ -4573,15 +4573,15 @@
         na = /^(img|br|input|textarea|hr)$/i;
 
     function Fi(n, e, t, r, i) {
         for (;;) {
             if (n == t && e == r) return !0;
             if (e == (i < 0 ? 0 : oe(n))) {
                 let o = n.parentNode;
-                if (!o || o.nodeType != 1 || Dt(n) || na.test(n.nodeName) || n.contentEditable == "false") return !1;
+                if (!o || o.nodeType != 1 || Tt(n) || na.test(n.nodeName) || n.contentEditable == "false") return !1;
                 e = I(n) + (i < 0 ? 0 : 1), n = o
             } else if (n.nodeType == 1) {
                 if (n = n.childNodes[e + (i < 0 ? -1 : 0)], n.contentEditable == "false") return !1;
                 e = i < 0 ? oe(n) : 0
             } else return !1
         }
     }
@@ -4592,40 +4592,40 @@
 
     function ra(n, e) {
         for (;;) {
             if (n.nodeType == 3 && e) return n;
             if (n.nodeType == 1 && e > 0) {
                 if (n.contentEditable == "false") return null;
                 n = n.childNodes[e - 1], e = oe(n)
-            } else if (n.parentNode && !Dt(n)) e = I(n), n = n.parentNode;
+            } else if (n.parentNode && !Tt(n)) e = I(n), n = n.parentNode;
             else return null
         }
     }
 
     function ia(n, e) {
         for (;;) {
             if (n.nodeType == 3 && e < n.nodeValue.length) return n;
             if (n.nodeType == 1 && e < n.childNodes.length) {
                 if (n.contentEditable == "false") return null;
                 n = n.childNodes[e], e = 0
-            } else if (n.parentNode && !Dt(n)) e = I(n) + 1, n = n.parentNode;
+            } else if (n.parentNode && !Tt(n)) e = I(n) + 1, n = n.parentNode;
             else return null
         }
     }
 
     function oa(n, e, t) {
         for (let r = e == 0, i = e == oe(n); r || i;) {
             if (n == t) return !0;
             let o = I(n);
             if (n = n.parentNode, !n) return !1;
             r = r && o == 0, i = i && o == oe(n)
         }
     }
 
-    function Dt(n) {
+    function Tt(n) {
         let e;
         for (let t = n; t && !(e = t.pmViewDesc); t = t.parentNode);
         return e && e.node && e.node.isBlock && (e.dom == n || e.contentDOM == n)
     }
     var pn = function(n) {
         return n.focusNode && qe(n.focusNode, n.focusOffset, n.anchorNode, n.anchorOffset)
     };
@@ -4661,24 +4661,24 @@
         Vi = typeof document != "undefined" ? document : null,
         Ne = se && se.userAgent || "",
         rr = /Edge\/(\d+)/.exec(Ne),
         yo = /MSIE \d/.exec(Ne),
         ir = /Trident\/(?:[7-9]|\d{2,})\..*rv:(\d+)/.exec(Ne),
         W = !!(yo || ir || rr),
         Oe = yo ? document.documentMode : ir ? +ir[1] : rr ? +rr[1] : 0,
-        X = !W && /gecko\/(\d+)/i.test(Ne);
-    X && +(/Firefox\/(\d+)/.exec(Ne) || [0, 0])[1];
+        Z = !W && /gecko\/(\d+)/i.test(Ne);
+    Z && +(/Firefox\/(\d+)/.exec(Ne) || [0, 0])[1];
     var or = !W && /Chrome\/(\d+)/.exec(Ne),
         B = !!or,
         aa = or ? +or[1] : 0,
         F = !W && !!se && /Apple Computer/.test(se.vendor),
         tt = F && (/Mobile\/\w+/.test(Ne) || !!se && se.maxTouchPoints > 2),
-        j = tt || (se ? /Mac/.test(se.platform) : !1),
+        _ = tt || (se ? /Mac/.test(se.platform) : !1),
         ca = se ? /Win/.test(se.platform) : !1,
-        Y = /Android \d/.test(Ne),
+        Q = /Android \d/.test(Ne),
         Et = !!Vi && "webkitFontSmoothing" in Vi.documentElement.style,
         fa = Et ? +(/\bAppleWebKit\/(\d+)/.exec(navigator.userAgent) || [0, 0])[1] : 0;
 
     function ha(n) {
         let e = n.defaultView && n.defaultView.visualViewport;
         return e ? {
             left: 0,
@@ -4771,18 +4771,18 @@
 
     function pa({
         refDOM: n,
         refTop: e,
         stack: t
     }) {
         let r = n ? n.getBoundingClientRect().top : 0;
-        ko(t, r == 0 ? 0 : r - e)
+        xo(t, r == 0 ? 0 : r - e)
     }
 
-    function ko(n, e) {
+    function xo(n, e) {
         for (let t = 0; t < n.length; t++) {
             let {
                 dom: r,
                 top: i,
                 left: o
             } = n[t];
             r.scrollTop != i + e && (r.scrollTop = i + e), r.scrollLeft != o && (r.scrollLeft = o)
@@ -4796,18 +4796,18 @@
         let e = bo(n);
         n.focus(Xe == null ? {
             get preventScroll() {
                 return Xe = {
                     preventScroll: !0
                 }, !0
             }
-        } : void 0), Xe || (Xe = !1, ko(e, 0))
+        } : void 0), Xe || (Xe = !1, xo(e, 0))
     }
 
-    function xo(n, e) {
+    function ko(n, e) {
         let t, r = 2e8,
             i, o = 0,
             s = e.top,
             l = e.top,
             a, c;
         for (let f = n.firstChild, h = 0; f; f = f.nextSibling, h++) {
             let d;
@@ -4832,15 +4832,15 @@
                 });
                 !t && (e.left >= u.right && e.top >= u.top || e.left >= u.left && e.top >= u.bottom) && (o = h + 1)
             }
         }
         return !t && a && (t = a, i = c, r = 0), t && t.nodeType == 3 ? ga(t, i) : !t || r && t.nodeType == 1 ? {
             node: n,
             offset: o
-        } : xo(t, i)
+        } : ko(t, i)
     }
 
     function ga(n, e) {
         let t = n.nodeValue.length,
             r = document.createRange();
         for (let i = 0; i < t; i++) {
             r.setEnd(n, i + 1), r.setStart(n, i);
@@ -4865,23 +4865,23 @@
         return t && /^li$/i.test(t.nodeName) && e.left < n.getBoundingClientRect().left ? t : n
     }
 
     function ba(n, e, t) {
         let {
             node: r,
             offset: i
-        } = xo(e, t), o = -1;
+        } = ko(e, t), o = -1;
         if (r.nodeType == 1 && !r.firstChild) {
             let s = r.getBoundingClientRect();
             o = s.left != s.right && t.left > (s.left + s.right) / 2 ? 1 : -1
         }
         return n.docView.posFromDOM(r, i, o)
     }
 
-    function ka(n, e, t, r) {
+    function xa(n, e, t, r) {
         let i = -1;
         for (let o = e, s = !1; o != n.dom;) {
             let l = n.docView.nearestDesc(o, !0);
             if (!l) return null;
             if (l.dom.nodeType == 1 && (l.node.isBlock && l.parent && !s || !l.contentDOM)) {
                 let a = l.dom.getBoundingClientRect();
                 if (l.node.isBlock && l.parent && !s && (s = !0, a.left > r.left || a.top > r.top ? i = l.posBefore : (a.right < r.left || a.bottom < r.top) && (i = l.posAfter)), !l.contentDOM && i < 0 && !l.node.isText) return (l.node.isBlock ? r.top < (a.top + a.bottom) / 2 : r.left < (a.left + a.right) / 2) ? l.posBefore : l.posAfter
@@ -4904,15 +4904,15 @@
                     }
                 }
                 if ((o = (o + 1) % r) == i) break
             }
         return n
     }
 
-    function xa(n, e) {
+    function ka(n, e) {
         let t = n.dom.ownerDocument,
             r, i = 0,
             o = la(t, e.left, e.top);
         o && ({
             node: r,
             offset: i
         } = o);
@@ -4921,21 +4921,21 @@
         if (!s || !n.dom.contains(s.nodeType != 1 ? s.parentNode : s)) {
             let c = n.dom.getBoundingClientRect();
             if (!Sr(e, c) || (s = So(n.dom, e, c), !s)) return null
         }
         if (F)
             for (let c = s; r && c; c = Ot(c)) c.draggable && (r = void 0);
         if (s = ya(s, e), r) {
-            if (X && r.nodeType == 1 && (i = Math.min(i, r.childNodes.length), i < r.childNodes.length)) {
+            if (Z && r.nodeType == 1 && (i = Math.min(i, r.childNodes.length), i < r.childNodes.length)) {
                 let f = r.childNodes[i],
                     h;
                 f.nodeName == "IMG" && (h = f.getBoundingClientRect()).right <= e.left && h.bottom > e.top && i++
             }
             let c;
-            Et && i && r.nodeType == 1 && (c = r.childNodes[i - 1]).nodeType == 1 && c.contentEditable == "false" && c.getBoundingClientRect().top >= e.top && i--, r == n.dom && i == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = n.state.doc.content.size : (i == 0 || r.nodeType != 1 || r.childNodes[i - 1].nodeName != "BR") && (l = ka(n, r, i, e))
+            Et && i && r.nodeType == 1 && (c = r.childNodes[i - 1]).nodeType == 1 && c.contentEditable == "false" && c.getBoundingClientRect().top >= e.top && i--, r == n.dom && i == r.childNodes.length - 1 && r.lastChild.nodeType == 1 && e.top > r.lastChild.getBoundingClientRect().bottom ? l = n.state.doc.content.size : (i == 0 || r.nodeType != 1 || r.childNodes[i - 1].nodeName != "BR") && (l = xa(n, r, i, e))
         }
         l == null && (l = ba(n, s, e));
         let a = n.docView.nearestDesc(s, !0);
         return {
             pos: l,
             inside: a ? a.posAtStart - a.border : -1
         }
@@ -4956,19 +4956,19 @@
     var Sa = /[\u0590-\u05f4\u0600-\u06ff\u0700-\u08ac]/;
 
     function Mo(n, e, t) {
         let {
             node: r,
             offset: i,
             atom: o
-        } = n.docView.domFromPos(e, t < 0 ? -1 : 1), s = Et || X;
+        } = n.docView.domFromPos(e, t < 0 ? -1 : 1), s = Et || Z;
         if (r.nodeType == 3)
             if (s && (Sa.test(r.nodeValue) || (t < 0 ? !i : i == r.nodeValue.length))) {
                 let a = Se(me(r, i, i), t);
-                if (X && i && /\s/.test(r.nodeValue[i - 1]) && i < r.nodeValue.length) {
+                if (Z && i && /\s/.test(r.nodeValue[i - 1]) && i < r.nodeValue.length) {
                     let c = Se(me(r, i - 1, i - 1), -1);
                     if (c.top == a.top) {
                         let f = Se(me(r, i, i + 1), -1);
                         if (f.top != a.top) return St(f, f.left < c.left)
                     }
                 }
                 return a
@@ -5088,32 +5088,32 @@
                 {
                     focusNode: u,
                     focusOffset: m
                 } = n.domSelectionRange(),
                 g = u && !p.contains(u.nodeType == 1 ? u : u.parentNode) || a == u && c == m;
             try {
                 l.collapse(f, h), a && (a != f || c != h) && l.extend && l.extend(a, c)
-            } catch (k) {}
+            } catch (x) {}
             return d != null && (l.caretBidiLevel = d), g
         })
     }
     var Wi = null,
         qi = null,
         Ki = !1;
 
     function wa(n, e, t) {
         return Wi == e && qi == t ? Ki : (Wi = e, qi = t, Ki = t == "up" || t == "down" ? Ma(n, e, t) : Oa(n, e, t))
     }
-    var _ = 0,
+    var U = 0,
         $i = 1,
         Fe = 2,
         le = 3,
         Ke = class {
             constructor(e, t, r, i) {
-                this.parent = e, this.children = t, this.dom = r, this.contentDOM = i, this.dirty = _, r.pmViewDesc = this
+                this.parent = e, this.children = t, this.dom = r, this.contentDOM = i, this.dirty = U, r.pmViewDesc = this
             }
             matchesWidget(e) {
                 return !1
             }
             matchesMark(e) {
                 return !1
             }
@@ -5343,15 +5343,15 @@
                     if (o > p && s < m) return u.setSelection(e - p - u.border, t - p - u.border, r, i);
                     p = m
                 }
                 let l = this.domFromPos(e, e ? -1 : 1),
                     a = t == e ? l : this.domFromPos(t, t ? -1 : 1),
                     c = r.getSelection(),
                     f = !1;
-                if ((X || F) && e == t) {
+                if ((Z || F) && e == t) {
                     let {
                         node: d,
                         offset: p
                     } = l;
                     if (d.nodeType == 3) {
                         if (f = !!(p && d.nodeValue[p - 1] == `
 `), f && p == d.nodeValue.length)
@@ -5367,15 +5367,15 @@
                                 if (g && g.node && g.node.isBlock) break
                             }
                     } else {
                         let u = d.childNodes[p - 1];
                         f = u && (u.nodeName == "BR" || u.contentEditable == "false")
                     }
                 }
-                if (X && c.focusNode && c.focusNode != a.node && c.focusNode.nodeType == 1) {
+                if (Z && c.focusNode && c.focusNode != a.node && c.focusNode.nodeType == 1) {
                     let d = c.focusNode.childNodes[c.focusOffset];
                     d && d.contentEditable == "false" && (i = !0)
                 }
                 if (!(i || f && F) && qe(l.node, l.offset, c.anchorNode, c.anchorOffset) && qe(a.node, a.offset, c.focusNode, c.focusOffset)) return;
                 let h = !1;
                 if ((c.extend || e == t) && !f) {
                     c.collapse(l.node, l.offset);
@@ -5443,15 +5443,15 @@
                         l.appendChild(s), s = l
                     }
                     s.contentEditable = "false", s.classList.add("ProseMirror-widget")
                 }
                 super(e, [], s, null), this.widget = t, this.widget = t, o = this
             }
             matchesWidget(e) {
-                return this.dirty == _ && e.type.eq(this.widget.type)
+                return this.dirty == U && e.type.eq(this.widget.type)
             }
             parseRule() {
                 return {
                     ignore: !0
                 }
             }
             stopEvent(e) {
@@ -5507,18 +5507,18 @@
                     contentElement: this.contentDOM
                 }
             }
             matchesMark(e) {
                 return this.dirty != le && this.mark.eq(e)
             }
             markDirty(e, t) {
-                if (super.markDirty(e, t), this.dirty != _) {
+                if (super.markDirty(e, t), this.dirty != U) {
                     let r = this.parent;
                     for (; !r.node;) r = r.parent;
-                    r.dirty < this.dirty && (r.dirty = this.dirty), this.dirty = _
+                    r.dirty < this.dirty && (r.dirty = this.dirty), this.dirty = U
                 }
             }
             slice(e, t, r) {
                 let i = n.create(this.parent, this.mark, !0, r),
                     o = this.children,
                     s = this.size;
                 t < s && (o = hr(o, t, s, r)), e > 0 && (o = hr(o, 0, e, r));
@@ -5566,15 +5566,15 @@
                         }
                     }
                     e.contentElement || (e.getContent = () => y.empty)
                 }
                 return e
             }
             matchesNode(e, t, r) {
-                return this.dirty == _ && e.eq(this.node) && cr(t, this.outerDeco) && r.eq(this.innerDeco)
+                return this.dirty == U && e.eq(this.node) && cr(t, this.outerDeco) && r.eq(this.innerDeco)
             }
             get size() {
                 return this.node.nodeSize
             }
             get border() {
                 return this.node.isLeaf ? 0 : 1
             }
@@ -5630,15 +5630,15 @@
                 let s = new sr(this, o, t, i);
                 e.input.compositionNodes.push(s), this.children = hr(this.children, r, r + i.length, e, s)
             }
             update(e, t, r, i) {
                 return this.dirty == le || !e.sameMarkup(this.node) ? !1 : (this.updateInner(e, t, r, i), !0)
             }
             updateInner(e, t, r, i) {
-                this.updateOuterDeco(t), this.node = e, this.innerDeco = r, this.contentDOM && this.updateChildren(i, this.posAtStart), this.dirty = _
+                this.updateOuterDeco(t), this.node = e, this.innerDeco = r, this.contentDOM && this.updateChildren(i, this.posAtStart), this.dirty = U
             }
             updateOuterDeco(e) {
                 if (cr(e, this.outerDeco)) return;
                 let t = this.nodeDOM.nodeType != 1,
                     r = this.dom;
                 this.dom = wo(this.dom, this.nodeDOM, ar(this.outerDeco, this.node, t), ar(e, this.node, t)), this.dom != r && (r.pmViewDesc = void 0, this.dom.pmViewDesc = this), this.outerDeco = e
             }
@@ -5666,15 +5666,15 @@
                 let e = this.nodeDOM.parentNode;
                 for (; e && e != this.dom && !e.pmIsDeco;) e = e.parentNode;
                 return {
                     skip: e || !0
                 }
             }
             update(e, t, r, i) {
-                return this.dirty == le || this.dirty != _ && !this.inParent() || !e.sameMarkup(this.node) ? !1 : (this.updateOuterDeco(t), (this.dirty != _ || e.text != this.node.text) && e.text != this.nodeDOM.nodeValue && (this.nodeDOM.nodeValue = e.text, i.trackWrites == this.nodeDOM && (i.trackWrites = null)), this.node = e, this.dirty = _, !0)
+                return this.dirty == le || this.dirty != U && !this.inParent() || !e.sameMarkup(this.node) ? !1 : (this.updateOuterDeco(t), (this.dirty != U || e.text != this.node.text) && e.text != this.nodeDOM.nodeValue && (this.nodeDOM.nodeValue = e.text, i.trackWrites == this.nodeDOM && (i.trackWrites = null)), this.node = e, this.dirty = U, !0)
             }
             inParent() {
                 let e = this.parent.contentDOM;
                 for (let t = this.nodeDOM; t; t = t.parentNode)
                     if (t == e) return !0;
                 return !1
             }
@@ -5708,15 +5708,15 @@
         sn = class extends Ke {
             parseRule() {
                 return {
                     ignore: !0
                 }
             }
             matchesHack(e) {
-                return this.dirty == _ && this.dom.nodeName == e
+                return this.dirty == U && this.dom.nodeName == e
             }
             get domAtom() {
                 return !0
             }
             get ignoreForCoords() {
                 return this.dom.nodeName == "IMG"
             }
@@ -5841,15 +5841,15 @@
 
     function ji(n) {
         let e = n.nextSibling;
         return n.parentNode.removeChild(n), e
     }
     var fr = class {
         constructor(e, t, r) {
-            this.lock = t, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = Ta(e.node.content, e)
+            this.lock = t, this.view = r, this.index = 0, this.stack = [], this.changed = !1, this.top = e, this.preMatch = Da(e.node.content, e)
         }
         destroyBetween(e, t) {
             if (e != t) {
                 for (let r = e; r < t; r++) this.top.children[r].destroy();
                 this.top.children.splice(e, t - e), this.changed = !0
             }
         }
@@ -5857,15 +5857,15 @@
             this.destroyBetween(this.index, this.top.children.length)
         }
         syncToMarks(e, t, r) {
             let i = 0,
                 o = this.stack.length >> 1,
                 s = Math.min(o, e.length);
             for (; i < s && (i == o - 1 ? this.top : this.stack[i + 1 << 1]).matchesMark(e[i]) && e[i].type.spec.spanning !== !1;) i++;
-            for (; i < o;) this.destroyRest(), this.top.dirty = _, this.index = this.stack.pop(), this.top = this.stack.pop(), o--;
+            for (; i < o;) this.destroyRest(), this.top.dirty = U, this.index = this.stack.pop(), this.top = this.stack.pop(), o--;
             for (; o < e.length;) {
                 this.stack.push(this.top, this.index + 1);
                 let l = -1;
                 for (let a = this.index; a < Math.min(this.index + 3, this.top.children.length); a++) {
                     let c = this.top.children[a];
                     if (c.matchesMark(e[o]) && !this.isLocked(c.dom)) {
                         l = a;
@@ -5918,15 +5918,15 @@
                 let a = this.top.children[l];
                 if (a instanceof we) {
                     let c = this.preMatch.matched.get(a);
                     if (c != null && c != o) return !1;
                     let f = a.dom,
                         h, d = this.isLocked(f) && !(e.isText && a.node && a.node.isText && a.nodeDOM.nodeValue == e.text && a.dirty != le && cr(t, a.outerDeco));
                     if (!d && a.update(e, t, r, i)) return this.destroyBetween(this.index, l), a.dom != f && (this.changed = !0), this.index++, !0;
-                    if (!d && (h = this.recreateWrapper(a, e, t, r, i, s))) return this.top.children[this.index] = h, h.contentDOM && (h.dirty = Fe, h.updateChildren(i, s + 1), h.dirty = _), this.changed = !0, this.index++, !0;
+                    if (!d && (h = this.recreateWrapper(a, e, t, r, i, s))) return this.top.children[this.index] = h, h.contentDOM && (h.dirty = Fe, h.updateChildren(i, s + 1), h.dirty = U), this.changed = !0, this.index++, !0;
                     break
                 }
             }
             return !1
         }
         recreateWrapper(e, t, r, i, o, s) {
             if (e.dirty || t.isAtom || !e.children.length || !e.node.content.eq(t.content)) return null;
@@ -5965,15 +5965,15 @@
             }
         }
         isLocked(e) {
             return this.lock && (e == this.lock || e.nodeType == 1 && e.contains(this.lock.parentNode))
         }
     };
 
-    function Ta(n, e) {
+    function Da(n, e) {
         let t = e,
             r = t.children.length,
             i = n.childCount,
             o = new Map,
             s = [];
         e: for (; i > 0;) {
             let l;
@@ -5997,15 +5997,15 @@
         return {
             index: i,
             matched: o,
             matches: s.reverse()
         }
     }
 
-    function Da(n, e) {
+    function Ta(n, e) {
         return n.type.side - e.type.side
     }
 
     function Ea(n, e, t, r) {
         let i = e.locals(n),
             o = 0;
         if (i.length == 0) {
@@ -6022,28 +6022,28 @@
             let f, h;
             for (; s < i.length && i[s].to == o;) {
                 let g = i[s++];
                 g.widget && (f ? (h || (h = [f])).push(g) : f = g)
             }
             if (f)
                 if (h) {
-                    h.sort(Da);
+                    h.sort(Ta);
                     for (let g = 0; g < h.length; g++) t(h[g], c, !!a)
                 } else t(f, c, !!a);
             let d, p;
             if (a) p = -1, d = a, a = null;
             else if (c < n.childCount) p = c, d = n.child(c++);
             else break;
             for (let g = 0; g < l.length; g++) l[g].to <= o && l.splice(g--, 1);
             for (; s < i.length && i[s].from <= o && i[s].to > o;) l.push(i[s++]);
             let u = o + d.nodeSize;
             if (d.isText) {
                 let g = u;
                 s < i.length && i[s].from < g && (g = i[s].from);
-                for (let k = 0; k < l.length; k++) l[k].to < g && (g = l[k].to);
+                for (let x = 0; x < l.length; x++) l[x].to < g && (g = l[x].to);
                 g < u && (a = d.cut(g - o), d = d.cut(0, g - o), u = g, p = -1)
             } else
                 for (; s < i.length && i[s].to < u;) s++;
             let m = d.isInline && !d.isLeaf ? l.filter(g => !g.inline) : l.slice();
             r(d, m, e.forChild(o, d), p), o = u
         }
     }
@@ -6096,52 +6096,52 @@
             s = n.docView.posFromDOM(t.focusNode, t.focusOffset, 1);
         if (s < 0) return null;
         let l = r.resolve(s),
             a, c;
         if (pn(t)) {
             for (a = l; i && !i.node;) i = i.parent;
             let f = i.node;
-            if (i && f.isAtom && x.isSelectable(f) && i.parent && !(f.isInline && oa(t.focusNode, t.focusOffset, i.dom))) {
+            if (i && f.isAtom && k.isSelectable(f) && i.parent && !(f.isInline && oa(t.focusNode, t.focusOffset, i.dom))) {
                 let h = i.posBefore;
-                c = new x(s == h ? l : r.resolve(h))
+                c = new k(s == h ? l : r.resolve(h))
             }
         } else {
             let f = n.docView.posFromDOM(t.anchorNode, t.anchorOffset, 1);
             if (f < 0) return null;
             a = r.resolve(f)
         }
         if (!c) {
             let f = e == "pointer" || n.state.selection.head < l.pos && !o ? 1 : -1;
             c = Cr(n, a, l, f)
         }
         return c
     }
 
-    function To(n) {
+    function Do(n) {
         return n.editable ? n.hasFocus() : Eo(n) && document.activeElement && document.activeElement.contains(n.dom)
     }
 
     function ge(n, e = !1) {
         let t = n.state.selection;
-        if (Do(n, t), !!To(n)) {
+        if (To(n, t), !!Do(n)) {
             if (!e && n.input.mouseDown && n.input.mouseDown.allowDefault && B) {
                 let r = n.domSelectionRange(),
                     i = n.domObserver.currentSelection;
                 if (r.anchorNode && i.anchorNode && qe(r.anchorNode, r.anchorOffset, i.anchorNode, i.anchorOffset)) {
                     n.input.mouseDown.delayedSelectionSync = !0, n.domObserver.setCurSelection();
                     return
                 }
             }
-            if (n.domObserver.disconnectSelection(), n.cursorWrapper) va(n);
+            if (n.domObserver.disconnectSelection(), n.cursorWrapper) Ra(n);
             else {
                 let {
                     anchor: r,
                     head: i
                 } = t, o, s;
-                _i && !(t instanceof w) && (t.$from.parent.inlineContent || (o = Ui(n, t.from)), !t.empty && !t.$from.parent.inlineContent && (s = Ui(n, t.to))), n.docView.setSelection(r, i, n.root, e), _i && (o && Gi(o), s && Gi(s)), t.visible ? n.dom.classList.remove("ProseMirror-hideselection") : (n.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && Ra(n))
+                _i && !(t instanceof w) && (t.$from.parent.inlineContent || (o = Ui(n, t.from)), !t.empty && !t.$from.parent.inlineContent && (s = Ui(n, t.to))), n.docView.setSelection(r, i, n.root, e), _i && (o && Gi(o), s && Gi(s)), t.visible ? n.dom.classList.remove("ProseMirror-hideselection") : (n.dom.classList.add("ProseMirror-hideselection"), "onselectionchange" in document && va(n))
             }
             n.domObserver.setCurSelection(), n.domObserver.connectSelection()
         }
     }
     var _i = F || B && aa < 63;
 
     function Ui(n, e) {
@@ -6160,37 +6160,37 @@
         return n.contentEditable = "true", F && n.draggable && (n.draggable = !1, n.wasDraggable = !0), n
     }
 
     function Gi(n) {
         n.contentEditable = "false", n.wasDraggable && (n.draggable = !0, n.wasDraggable = null)
     }
 
-    function Ra(n) {
+    function va(n) {
         let e = n.dom.ownerDocument;
         e.removeEventListener("selectionchange", n.input.hideSelectionGuard);
         let t = n.domSelectionRange(),
             r = t.anchorNode,
             i = t.anchorOffset;
         e.addEventListener("selectionchange", n.input.hideSelectionGuard = () => {
             (t.anchorNode != r || t.anchorOffset != i) && (e.removeEventListener("selectionchange", n.input.hideSelectionGuard), setTimeout(() => {
-                (!To(n) || n.state.selection.visible) && n.dom.classList.remove("ProseMirror-hideselection")
+                (!Do(n) || n.state.selection.visible) && n.dom.classList.remove("ProseMirror-hideselection")
             }, 20))
         })
     }
 
-    function va(n) {
+    function Ra(n) {
         let e = n.domSelection(),
             t = document.createRange(),
             r = n.cursorWrapper.dom,
             i = r.nodeName == "IMG";
         i ? t.setEnd(r.parentNode, I(r) + 1) : t.setEnd(r, 0), t.collapse(!1), e.removeAllRanges(), e.addRange(t), !i && !n.state.selection.visible && W && Oe <= 11 && (r.disabled = !0, r.disabled = !1)
     }
 
-    function Do(n, e) {
-        if (e instanceof x) {
+    function To(n, e) {
+        if (e instanceof k) {
             let t = n.docView.descAt(e.from);
             t != n.lastSelectedViewDesc && (Yi(n), t && t.selectNode(), n.lastSelectedViewDesc = t)
         } else Yi(n)
     }
 
     function Yi(n) {
         n.lastSelectedViewDesc && (n.lastSelectedViewDesc.parent && n.lastSelectedViewDesc.deselectNode(), n.lastSelectedViewDesc = void 0)
@@ -6241,26 +6241,26 @@
                 } = r, o = i.textOffset ? null : e < 0 ? i.nodeBefore : i.nodeAfter;
                 if (!o || o.isText || !o.isLeaf) return !1;
                 let s = n.state.doc.resolve(i.pos + o.nodeSize * (e < 0 ? -1 : 1));
                 return Me(n, new w(r.$anchor, s))
             } else if (r.empty) {
             if (n.endOfTextblock(e > 0 ? "forward" : "backward")) {
                 let i = dr(n.state, e);
-                return i && i instanceof x ? Me(n, i) : !1
-            } else if (!(j && t.indexOf("m") > -1)) {
+                return i && i instanceof k ? Me(n, i) : !1
+            } else if (!(_ && t.indexOf("m") > -1)) {
                 let i = r.$head,
                     o = i.textOffset ? null : e < 0 ? i.nodeBefore : i.nodeAfter,
                     s;
                 if (!o || o.isText) return !1;
                 let l = e < 0 ? i.pos - o.nodeSize : i.pos;
-                return o.isAtom || (s = n.docView.descAt(l)) && !s.contentDOM ? x.isSelectable(o) ? Me(n, new x(e < 0 ? n.state.doc.resolve(i.pos - o.nodeSize) : i)) : Et ? Me(n, new w(n.state.doc.resolve(e < 0 ? l : l + o.nodeSize))) : !1 : !1
+                return o.isAtom || (s = n.docView.descAt(l)) && !s.contentDOM ? k.isSelectable(o) ? Me(n, new k(e < 0 ? n.state.doc.resolve(i.pos - o.nodeSize) : i)) : Et ? Me(n, new w(n.state.doc.resolve(e < 0 ? l : l + o.nodeSize))) : !1 : !1
             }
         } else return !1;
         else {
-            if (r instanceof x && r.node.isInline) return Me(n, new w(e > 0 ? r.$to : r.$from));
+            if (r instanceof k && r.node.isInline) return Me(n, new w(e > 0 ? r.$to : r.$from));
             {
                 let i = dr(n.state, e);
                 return i ? Me(n, i) : !1
             }
         }
     }
 
@@ -6279,15 +6279,15 @@
 
     function za(n) {
         let e = n.domSelectionRange(),
             t = e.focusNode,
             r = e.focusOffset;
         if (!t) return;
         let i, o, s = !1;
-        for (X && t.nodeType == 1 && r < ln(t) && Ct(t.childNodes[r], -1) && (s = !0);;)
+        for (Z && t.nodeType == 1 && r < ln(t) && Ct(t.childNodes[r], -1) && (s = !0);;)
             if (r > 0) {
                 if (t.nodeType != 1) break;
                 {
                     let l = t.childNodes[r - 1];
                     if (Ct(l, -1)) i = t, o = --r;
                     else if (l.nodeType == 3) t = l, r = t.nodeValue.length;
                     else break
@@ -6335,25 +6335,25 @@
 
     function Ao(n) {
         let e = n.pmViewDesc;
         return e && e.node && e.node.isBlock
     }
 
     function Fa(n, e) {
-        for (; n && e == n.childNodes.length && !Dt(n);) e = I(n) + 1, n = n.parentNode;
+        for (; n && e == n.childNodes.length && !Tt(n);) e = I(n) + 1, n = n.parentNode;
         for (; n && e < n.childNodes.length;) {
             let t = n.childNodes[e];
             if (t.nodeType == 3) return t;
             if (t.nodeType == 1 && t.contentEditable == "false") break;
             n = t, e = 0
         }
     }
 
     function Va(n, e) {
-        for (; n && !e && !Dt(n);) e = I(n), n = n.parentNode;
+        for (; n && !e && !Tt(n);) e = I(n), n = n.parentNode;
         for (; n && e;) {
             let t = n.childNodes[e - 1];
             if (t.nodeType == 3) return t;
             if (t.nodeType == 1 && t.contentEditable == "false") break;
             n = t, e = n.childNodes.length
         }
     }
@@ -6393,22 +6393,22 @@
             }
         }
         return getComputedStyle(n.dom).direction == "rtl" ? "rtl" : "ltr"
     }
 
     function eo(n, e, t) {
         let r = n.state.selection;
-        if (r instanceof w && !r.empty || t.indexOf("s") > -1 || j && t.indexOf("m") > -1) return !1;
+        if (r instanceof w && !r.empty || t.indexOf("s") > -1 || _ && t.indexOf("m") > -1) return !1;
         let {
             $from: i,
             $to: o
         } = r;
         if (!i.parent.inlineContent || n.endOfTextblock(e < 0 ? "up" : "down")) {
             let s = dr(n.state, e);
-            if (s && s instanceof x) return Me(n, s)
+            if (s && s instanceof k) return Me(n, s)
         }
         if (!i.parent.inlineContent) {
             let s = e < 0 ? i : o,
                 l = r instanceof $ ? S.near(s, e) : S.findFrom(s, e);
             return l ? Me(n, l) : !1
         }
         return !1
@@ -6453,27 +6453,27 @@
         let e = "";
         return n.ctrlKey && (e += "c"), n.metaKey && (e += "m"), n.altKey && (e += "a"), n.shiftKey && (e += "s"), e
     }
 
     function Wa(n, e) {
         let t = e.keyCode,
             r = Ja(e);
-        if (t == 8 || j && t == 72 && r == "c") return to(n, -1) || Qe(n, -1);
-        if (t == 46 && !e.shiftKey || j && t == 68 && r == "c") return to(n, 1) || Qe(n, 1);
+        if (t == 8 || _ && t == 72 && r == "c") return to(n, -1) || Qe(n, -1);
+        if (t == 46 && !e.shiftKey || _ && t == 68 && r == "c") return to(n, 1) || Qe(n, 1);
         if (t == 13 || t == 27) return !0;
-        if (t == 37 || j && t == 66 && r == "c") {
+        if (t == 37 || _ && t == 66 && r == "c") {
             let i = t == 37 ? Zi(n, n.state.selection.from) == "ltr" ? -1 : 1 : -1;
             return Qi(n, i, r) || Qe(n, i)
-        } else if (t == 39 || j && t == 70 && r == "c") {
+        } else if (t == 39 || _ && t == 70 && r == "c") {
             let i = t == 39 ? Zi(n, n.state.selection.from) == "ltr" ? 1 : -1 : 1;
             return Qi(n, i, r) || Qe(n, i)
         } else {
-            if (t == 38 || j && t == 80 && r == "c") return eo(n, -1, r) || Qe(n, -1);
-            if (t == 40 || j && t == 78 && r == "c") return La(n) || eo(n, 1, r) || Qe(n, 1);
-            if (r == (j ? "m" : "c") && (t == 66 || t == 73 || t == 89 || t == 90)) return !0
+            if (t == 38 || _ && t == 80 && r == "c") return eo(n, -1, r) || Qe(n, -1);
+            if (t == 40 || _ && t == 78 && r == "c") return La(n) || eo(n, 1, r) || Qe(n, 1);
+            if (r == (_ ? "m" : "c") && (t == 66 || t == 73 || t == 89 || t == 90)) return !0
         }
         return !1
     }
 
     function Io(n, e) {
         n.someProp("transformCopied", p => {
             e = p(e, n)
@@ -6511,15 +6511,15 @@
 `);
         return {
             dom: a,
             text: d
         }
     }
 
-    function Ro(n, e, t, r, i) {
+    function vo(n, e, t, r, i) {
         let o = i.parent.type.spec.code,
             s, l;
         if (!t && !e) return null;
         let a = e && (r || o || !t);
         if (a) {
             if (n.someProp("transformPastedText", d => {
                     e = d(e, o || r, n)
@@ -6546,15 +6546,15 @@
         if (f && f[3])
             for (let h = +f[3]; h > 0; h--) {
                 let d = s.firstChild;
                 for (; d && d.nodeType != 1;) d = d.nextSibling;
                 if (!d) break;
                 s = d
             }
-        if (l || (l = (n.someProp("clipboardParser") || n.someProp("domParser") || ve.fromSchema(n.state.schema)).parseSlice(s, {
+        if (l || (l = (n.someProp("clipboardParser") || n.someProp("domParser") || Re.fromSchema(n.state.schema)).parseSlice(s, {
                 preserveWhitespace: !!(a || f),
                 context: i,
                 ruleFromNode(d) {
                     return d.nodeName == "BR" && !d.nextSibling && d.parentNode && !qa.test(d.parentNode.nodeName) ? {
                         ignore: !0
                     } : null
                 }
@@ -6581,32 +6581,32 @@
                     if (!s) return;
                     let a = i.findWrapping(l.type),
                         c;
                     if (!a) return s = null;
                     if (c = s.length && o.length && Po(a, o, l, s[s.length - 1], 0)) s[s.length - 1] = c;
                     else {
                         s.length && (s[s.length - 1] = zo(s[s.length - 1], o.length));
-                        let f = vo(l, a);
+                        let f = Ro(l, a);
                         s.push(f), i = i.matchType(f.type), o = a
                     }
                 }), s) return y.from(s)
         }
         return n
     }
 
-    function vo(n, e, t = 0) {
+    function Ro(n, e, t = 0) {
         for (let r = e.length - 1; r >= t; r--) n = e[r].create(null, y.from(n));
         return n
     }
 
     function Po(n, e, t, r, i) {
         if (i < n.length && i < e.length && n[i] == e[i]) {
             let o = Po(n, e, t, r.lastChild, i + 1);
             if (o) return r.copy(r.content.replaceChild(r.childCount - 1, o));
-            if (r.contentMatchAt(r.childCount).matchType(i == n.length - 1 ? t.type : n[i + 1])) return r.copy(r.content.append(y.from(vo(t, n, i + 1))))
+            if (r.contentMatchAt(r.childCount).matchType(i == n.length - 1 ? t.type : n[i + 1])) return r.copy(r.content.append(y.from(Ro(t, n, i + 1))))
         }
     }
 
     function zo(n, e) {
         if (e == 0) return n;
         let t = n.content.replaceChild(n.childCount - 1, zo(n.lastChild, e - 1)),
             r = n.contentMatchAt(n.childCount).fillBefore(y.empty, !0);
@@ -6740,28 +6740,28 @@
     }
 
     function Xa(n, e) {
         !Or(n, e) && V[e.type] && (n.editable || !(e.type in L)) && V[e.type](n, e)
     }
     L.keydown = (n, e) => {
         let t = e;
-        if (n.input.shiftKey = t.keyCode == 16 || t.shiftKey, !Lo(n, t) && (n.input.lastKeyCode = t.keyCode, n.input.lastKeyCodeTime = Date.now(), !(Y && B && t.keyCode == 13)))
+        if (n.input.shiftKey = t.keyCode == 16 || t.shiftKey, !Lo(n, t) && (n.input.lastKeyCode = t.keyCode, n.input.lastKeyCodeTime = Date.now(), !(Q && B && t.keyCode == 13)))
             if (t.keyCode != 229 && n.domObserver.forceFlush(), tt && t.keyCode == 13 && !t.ctrlKey && !t.altKey && !t.metaKey) {
                 let r = Date.now();
                 n.input.lastIOSEnter = r, n.input.lastIOSEnterFallbackTimeout = setTimeout(() => {
                     n.input.lastIOSEnter == r && (n.someProp("handleKeyDown", i => i(n, Be(13, "Enter"))), n.input.lastIOSEnter = 0)
                 }, 200)
             } else n.someProp("handleKeyDown", r => r(n, t)) || Wa(n, t) ? t.preventDefault() : Ce(n, "key")
     };
     L.keyup = (n, e) => {
         e.keyCode == 16 && (n.input.shiftKey = !1)
     };
     L.keypress = (n, e) => {
         let t = e;
-        if (Lo(n, t) || !t.charCode || t.ctrlKey && !t.altKey || j && t.metaKey) return;
+        if (Lo(n, t) || !t.charCode || t.ctrlKey && !t.altKey || _ && t.metaKey) return;
         if (n.someProp("handleKeyPress", i => i(n, t))) {
             t.preventDefault();
             return
         }
         let r = n.state.selection;
         if (!(r instanceof w) || !r.$from.sameParent(r.$to)) {
             let i = String.fromCharCode(t.charCode);
@@ -6796,31 +6796,31 @@
         t == "pointer" && r.setMeta("pointer", !0), n.dispatch(r)
     }
 
     function Za(n, e) {
         if (e == -1) return !1;
         let t = n.state.doc.resolve(e),
             r = t.nodeAfter;
-        return r && r.isAtom && x.isSelectable(r) ? (et(n, new x(t), "pointer"), !0) : !1
+        return r && r.isAtom && k.isSelectable(r) ? (et(n, new k(t), "pointer"), !0) : !1
     }
 
     function ec(n, e) {
         if (e == -1) return !1;
         let t = n.state.selection,
             r, i;
-        t instanceof x && (r = t.node);
+        t instanceof k && (r = t.node);
         let o = n.state.doc.resolve(e);
         for (let s = o.depth + 1; s > 0; s--) {
             let l = s > o.depth ? o.nodeAfter : o.node(s);
-            if (x.isSelectable(l)) {
+            if (k.isSelectable(l)) {
                 r && t.$from.depth > 0 && s >= t.$from.depth && o.before(t.$from.depth + 1) == t.$from.pos ? i = o.before(t.$from.depth) : i = o.before(s);
                 break
             }
         }
-        return i != null ? (et(n, x.create(n.state.doc, i), "pointer"), !0) : !1
+        return i != null ? (et(n, k.create(n.state.doc, i), "pointer"), !0) : !1
     }
 
     function tc(n, e, t, r, i) {
         return wr(n, "handleClickOn", e, t, r) || n.someProp("handleClick", o => o(n, e, r)) || (i ? ec(n, t) : Za(n, t))
     }
 
     function nc(n, e, t, r) {
@@ -6836,24 +6836,24 @@
         let r = n.state.doc;
         if (e == -1) return r.inlineContent ? (et(n, w.create(r, 0, r.content.size), "pointer"), !0) : !1;
         let i = r.resolve(e);
         for (let o = i.depth + 1; o > 0; o--) {
             let s = o > i.depth ? i.nodeAfter : i.node(o),
                 l = i.before(o);
             if (s.inlineContent) et(n, w.create(r, l + 1, l + 1 + s.content.size), "pointer");
-            else if (x.isSelectable(s)) et(n, x.create(r, l), "pointer");
+            else if (k.isSelectable(s)) et(n, k.create(r, l), "pointer");
             else continue;
             return !0
         }
     }
 
     function Nr(n) {
         return an(n)
     }
-    var Vo = j ? "metaKey" : "ctrlKey";
+    var Vo = _ ? "metaKey" : "ctrlKey";
     V.mousedown = (n, e) => {
         let t = e;
         n.input.shiftKey = t.shiftKey;
         let r = Nr(n),
             i = Date.now(),
             o = "singleClick";
         i - n.input.lastClick.time < 500 && Qa(t, n.input.lastClick) && !t[Vo] && (n.input.lastClick.type == "singleClick" ? o = "doubleClick" : n.input.lastClick.type == "doubleClick" && (o = "tripleClick")), n.input.lastClick = {
@@ -6876,19 +6876,19 @@
             }
             let l = i ? null : r.target,
                 a = l ? e.docView.nearestDesc(l, !0) : null;
             this.target = a ? a.dom : null;
             let {
                 selection: c
             } = e.state;
-            (r.button == 0 && o.type.spec.draggable && o.type.spec.selectable !== !1 || c instanceof x && c.from <= s && c.to > s) && (this.mightDrag = {
+            (r.button == 0 && o.type.spec.draggable && o.type.spec.selectable !== !1 || c instanceof k && c.from <= s && c.to > s) && (this.mightDrag = {
                 node: o,
                 pos: s,
                 addAttr: !!(this.target && !this.target.draggable),
-                setUneditable: !!(this.target && X && !this.target.hasAttribute("contentEditable"))
+                setUneditable: !!(this.target && Z && !this.target.hasAttribute("contentEditable"))
             }), this.target && this.mightDrag && (this.mightDrag.addAttr || this.mightDrag.setUneditable) && (this.view.domObserver.stop(), this.mightDrag.addAttr && (this.target.draggable = !0), this.mightDrag.setUneditable && setTimeout(() => {
                 this.view.input.mouseDown == this && this.target.setAttribute("contentEditable", "false")
             }, 20), this.view.domObserver.start()), e.root.addEventListener("mouseup", this.up = this.up.bind(this)), e.root.addEventListener("mousemove", this.move = this.move.bind(this)), Ce(e, "pointer")
         }
         done() {
             this.view.root.removeEventListener("mouseup", this.up), this.view.root.removeEventListener("mousemove", this.move), this.mightDrag && this.target && (this.view.domObserver.stop(), this.mightDrag.addAttr && this.target.removeAttribute("draggable"), this.mightDrag.setUneditable && this.target.removeAttribute("contentEditable"), this.view.domObserver.start()), this.delayedSelectionSync && setTimeout(() => ge(this.view)), this.view.input.mouseDown = null
         }
@@ -6911,23 +6911,23 @@
         n.input.lastTouch = Date.now(), Ce(n, "pointer")
     };
     V.contextmenu = n => Nr(n);
 
     function Lo(n, e) {
         return n.composing ? !0 : F && Math.abs(e.timeStamp - n.input.compositionEndedAt) < 500 ? (n.input.compositionEndedAt = -2e8, !0) : !1
     }
-    var oc = Y ? 5e3 : -1;
+    var oc = Q ? 5e3 : -1;
     L.compositionstart = L.compositionupdate = n => {
         if (!n.composing) {
             n.domObserver.flush();
             let {
                 state: e
             } = n, t = e.selection.$from;
             if (e.selection.empty && (e.storedMarks || !t.textOffset && t.parentOffset && t.nodeBefore.marks.some(r => r.type.spec.inclusive === !1))) n.markCursor = n.state.storedMarks || t.marks(), an(n, !0), n.markCursor = null;
-            else if (an(n), X && e.selection.empty && t.parentOffset && !t.textOffset && t.nodeBefore.marks.length) {
+            else if (an(n), Z && e.selection.empty && t.parentOffset && !t.textOffset && t.nodeBefore.marks.length) {
                 let r = n.domSelectionRange();
                 for (let i = r.focusNode, o = r.focusOffset; i && i.nodeType == 1 && o != 0;) {
                     let s = o < 0 ? i.lastChild : i.childNodes[o - 1];
                     if (!s) break;
                     if (s.nodeType == 3) {
                         n.domSelection().collapse(s, s.nodeValue.length);
                         break
@@ -6968,15 +6968,15 @@
 
     function lc() {
         let n = document.createEvent("Event");
         return n.initEvent("event", !0, !0), n.timeStamp
     }
 
     function an(n, e = !1) {
-        if (!(Y && n.domObserver.flushingSoon >= 0)) {
+        if (!(Q && n.domObserver.flushingSoon >= 0)) {
             if (n.domObserver.forceFlush(), Wo(n), e || n.docView && n.docView.dirty) {
                 let t = Mr(n);
                 return t && !t.eq(n.state.selection) ? n.dispatch(n.state.tr.setSelection(t)) : n.updateState(n.state), !0
             }
             return !1
         }
     }
@@ -7018,15 +7018,15 @@
         let i = n.input.shiftKey && n.input.lastKeyCode != 45;
         setTimeout(() => {
             n.focus(), r.parentNode && r.parentNode.removeChild(r), t ? Nt(n, r.value, null, i, e) : Nt(n, r.textContent, r.innerHTML, i, e)
         }, 50)
     }
 
     function Nt(n, e, t, r, i) {
-        let o = Ro(n, e, t, r, n.state.selection.$from);
+        let o = vo(n, e, t, r, n.state.selection.$from);
         if (n.someProp("handlePaste", a => a(n, i, o || b.empty))) return !0;
         if (!o) return !1;
         let s = cc(o),
             l = s ? n.state.tr.replaceSelectionWith(s, r) : n.state.tr.replaceSelection(o);
         return n.dispatch(l.scrollIntoView().setMeta("paste", !0).setMeta("uiEvent", "paste")), !0
     }
 
@@ -7034,37 +7034,37 @@
         let e = n.getData("text/plain") || n.getData("Text");
         if (e) return e;
         let t = n.getData("text/uri-list");
         return t ? t.replace(/\r?\n/g, " ") : ""
     }
     L.paste = (n, e) => {
         let t = e;
-        if (n.composing && !Y) return;
+        if (n.composing && !Q) return;
         let r = wt ? null : t.clipboardData,
             i = n.input.shiftKey && n.input.lastKeyCode != 45;
         r && Nt(n, qo(r), r.getData("text/html"), i, t) ? t.preventDefault() : fc(n, t)
     };
     var cn = class {
             constructor(e, t, r) {
                 this.slice = e, this.move = t, this.node = r
             }
         },
-        Ko = j ? "altKey" : "ctrlKey";
+        Ko = _ ? "altKey" : "ctrlKey";
     V.dragstart = (n, e) => {
         let t = e,
             r = n.input.mouseDown;
         if (r && r.done(), !t.dataTransfer) return;
         let i = n.state.selection,
             o = i.empty ? null : n.posAtCoords(mn(t)),
             s;
-        if (!(o && o.pos >= i.from && o.pos <= (i instanceof x ? i.to - 1 : i.to))) {
-            if (r && r.mightDrag) s = x.create(n.state.doc, r.mightDrag.pos);
+        if (!(o && o.pos >= i.from && o.pos <= (i instanceof k ? i.to - 1 : i.to))) {
+            if (r && r.mightDrag) s = k.create(n.state.doc, r.mightDrag.pos);
             else if (t.target && t.target.nodeType == 1) {
                 let f = n.docView.nearestDesc(t.target, !0);
-                f && f.node.type.spec.draggable && f != n.docView && (s = x.create(n.state.doc, f.posBefore))
+                f && f.node.type.spec.draggable && f != n.docView && (s = k.create(n.state.doc, f.posBefore))
             }
         }
         let l = (s || n.state.selection).content(),
             {
                 dom: a,
                 text: c
             } = Io(n, l);
@@ -7083,15 +7083,15 @@
         if (n.dragging = null, !t.dataTransfer) return;
         let i = n.posAtCoords(mn(t));
         if (!i) return;
         let o = n.state.doc.resolve(i.pos),
             s = r && r.slice;
         s ? n.someProp("transformPasted", u => {
             s = u(s, n)
-        }) : s = Ro(n, qo(t.dataTransfer), wt ? null : t.dataTransfer.getData("text/html"), !1, o);
+        }) : s = vo(n, qo(t.dataTransfer), wt ? null : t.dataTransfer.getData("text/html"), !1, o);
         let l = !!(r && !t[Ko]);
         if (n.someProp("handleDrop", u => u(n, t, s || b.empty, l))) {
             t.preventDefault();
             return
         }
         if (!s) return;
         t.preventDefault();
@@ -7105,32 +7105,32 @@
             u ? u.replace(c) : c.deleteSelection()
         }
         let f = c.mapping.map(a),
             h = s.openStart == 0 && s.openEnd == 0 && s.content.childCount == 1,
             d = c.doc;
         if (h ? c.replaceRangeWith(f, f, s.content.firstChild) : c.replaceRange(f, f, s), c.doc.eq(d)) return;
         let p = c.doc.resolve(f);
-        if (h && x.isSelectable(s.content.firstChild) && p.nodeAfter && p.nodeAfter.sameMarkup(s.content.firstChild)) c.setSelection(new x(p));
+        if (h && k.isSelectable(s.content.firstChild) && p.nodeAfter && p.nodeAfter.sameMarkup(s.content.firstChild)) c.setSelection(new k(p));
         else {
             let u = c.mapping.map(a);
-            c.mapping.maps[c.mapping.maps.length - 1].forEach((m, g, k, N) => u = N), c.setSelection(Cr(n, p, c.doc.resolve(u)))
+            c.mapping.maps[c.mapping.maps.length - 1].forEach((m, g, x, N) => u = N), c.setSelection(Cr(n, p, c.doc.resolve(u)))
         }
         n.focus(), n.dispatch(c.setMeta("uiEvent", "drop"))
     };
     V.focus = n => {
         n.input.lastFocus = Date.now(), n.focused || (n.domObserver.stop(), n.dom.classList.add("ProseMirror-focused"), n.domObserver.start(), n.focused = !0, setTimeout(() => {
             n.docView && n.hasFocus() && !n.domObserver.currentSelection.eq(n.domSelectionRange()) && ge(n)
         }, 20))
     };
     V.blur = (n, e) => {
         let t = e;
         n.focused && (n.domObserver.stop(), n.dom.classList.remove("ProseMirror-focused"), n.domObserver.start(), t.relatedTarget && n.dom.contains(t.relatedTarget) && n.domObserver.currentSelection.clear(), n.focused = !1)
     };
     V.beforeinput = (n, e) => {
-        if (B && Y && e.inputType == "deleteContentBackward") {
+        if (B && Q && e.inputType == "deleteContentBackward") {
             n.domObserver.flushSoon();
             let {
                 domChangeCount: r
             } = n.input;
             setTimeout(() => {
                 if (n.input.domChangeCount != r || (n.dom.blur(), n.focus(), n.someProp("handleKeyDown", o => o(n, Be(8, "Backspace"))))) return;
                 let {
@@ -7138,15 +7138,15 @@
                 } = n.state.selection;
                 i && i.pos > 0 && n.dispatch(n.state.tr.delete(i.pos - 1, i.pos).scrollIntoView())
             }, 50)
         }
     };
     for (let n in L) V[n] = L[n];
 
-    function Tt(n, e) {
+    function Dt(n, e) {
         if (n == e) return !0;
         for (let t in n)
             if (n[t] !== e[t]) return !1;
         for (let t in e)
             if (!(t in n)) return !1;
         return !0
     }
@@ -7161,15 +7161,15 @@
                 } = e.mapResult(t.from + i, this.side < 0 ? -1 : 1);
                 return s ? null : new ae(o - r, o - r, this)
             }
             valid() {
                 return !0
             }
             eq(e) {
-                return this == e || e instanceof n && (this.spec.key && this.spec.key == e.spec.key || this.toDOM == e.toDOM && Tt(this.spec, e.spec))
+                return this == e || e instanceof n && (this.spec.key && this.spec.key == e.spec.key || this.toDOM == e.toDOM && Dt(this.spec, e.spec))
             }
             destroy(e) {
                 this.spec.destroy && this.spec.destroy(e)
             }
         },
         Le = class n {
             constructor(e, t) {
@@ -7180,15 +7180,15 @@
                     s = e.map(t.to + i, this.spec.inclusiveEnd ? 1 : -1) - r;
                 return o >= s ? null : new ae(o, s, this)
             }
             valid(e, t) {
                 return t.from < t.to
             }
             eq(e) {
-                return this == e || e instanceof n && Tt(this.attrs, e.attrs) && Tt(this.spec, e.spec)
+                return this == e || e instanceof n && Dt(this.attrs, e.attrs) && Dt(this.spec, e.spec)
             }
             static is(e) {
                 return e.type instanceof n
             }
             destroy() {}
         },
         br = class n {
@@ -7205,15 +7205,15 @@
                 let {
                     index: r,
                     offset: i
                 } = e.content.findIndex(t.from), o;
                 return i == t.from && !(o = e.child(r)).isText && i + o.nodeSize == t.to
             }
             eq(e) {
-                return this == e || e instanceof n && Tt(this.attrs, e.attrs) && Tt(this.spec, e.spec)
+                return this == e || e instanceof n && Dt(this.attrs, e.attrs) && Dt(this.spec, e.spec)
             }
             destroy() {}
         },
         ae = class n {
             constructor(e, t, r) {
                 this.from = e, this.to = t, this.type = r
             }
@@ -7349,26 +7349,26 @@
                 for (let t = 0; t < this.local.length; t++)
                     if (!this.local[t].eq(e.local[t])) return !1;
                 for (let t = 0; t < this.children.length; t += 3)
                     if (this.children[t] != e.children[t] || this.children[t + 1] != e.children[t + 1] || !this.children[t + 2].eq(e.children[t + 2])) return !1;
                 return !0
             }
             locals(e) {
-                return Tr(this.localsInner(e))
+                return Dr(this.localsInner(e))
             }
             localsInner(e) {
                 if (this == P) return Ze;
                 if (e.inlineContent || !this.local.some(Le.is)) return this.local;
                 let t = [];
                 for (let r = 0; r < this.local.length; r++) this.local[r].type instanceof Le || t.push(this.local[r]);
                 return t
             }
         };
     q.empty = new q([], []);
-    q.removeOverlap = Tr;
+    q.removeOverlap = Dr;
     var P = q.empty,
         hn = class n {
             constructor(e) {
                 this.members = e
             }
             map(e, t) {
                 let r = this.members.map(i => i.map(e, t, Je));
@@ -7396,15 +7396,15 @@
                     if (o.length)
                         if (!t) t = o;
                         else {
                             r && (t = t.slice(), r = !1);
                             for (let s = 0; s < o.length; s++) t.push(o[s])
                         }
                 }
-                return t ? Tr(r ? t : t.sort(We)) : Ze
+                return t ? Dr(r ? t : t.sort(We)) : Ze
             }
             static from(e) {
                 switch (e.length) {
                     case 0:
                         return P;
                     case 1:
                         return e[0];
@@ -7416,19 +7416,19 @@
 
     function hc(n, e, t, r, i, o, s) {
         let l = n.slice();
         for (let c = 0, f = o; c < t.maps.length; c++) {
             let h = 0;
             t.maps[c].forEach((d, p, u, m) => {
                 let g = m - u - (p - d);
-                for (let k = 0; k < l.length; k += 3) {
-                    let N = l[k + 1];
+                for (let x = 0; x < l.length; x += 3) {
+                    let N = l[x + 1];
                     if (N < 0 || d > N + f - h) continue;
-                    let ee = l[k] + f - h;
-                    p >= ee ? l[k + 1] = d <= ee ? -2 : -1 : d >= f && g && (l[k] += g, l[k + 1] += g)
+                    let ee = l[x] + f - h;
+                    p >= ee ? l[x + 1] = d <= ee ? -2 : -1 : d >= f && g && (l[x] += g, l[x + 1] += g)
                 }
                 h += g
             }), f = t.maps[c].map(f, -1)
         }
         let a = !1;
         for (let c = 0; c < l.length; c += 3)
             if (l[c + 1] < 0) {
@@ -7446,16 +7446,16 @@
                     p = d - i,
                     {
                         index: u,
                         offset: m
                     } = r.content.findIndex(h),
                     g = r.maybeChild(u);
                 if (g && m == h && m + g.nodeSize == p) {
-                    let k = l[c + 2].mapInner(t, g, f + 1, n[c] + o + 1, s);
-                    k != P ? (l[c] = h, l[c + 1] = p, l[c + 2] = k) : (l[c + 1] = -2, a = !0)
+                    let x = l[c + 2].mapInner(t, g, f + 1, n[c] + o + 1, s);
+                    x != P ? (l[c] = h, l[c + 1] = p, l[c + 2] = x) : (l[c + 1] = -2, a = !0)
                 } else a = !0
             } if (a) {
             let c = dc(l, n, e, t, i, o, s),
                 f = dn(c, r, 0, s);
             e = f.local;
             for (let h = 0; h < l.length; h += 3) l[h + 1] < 0 && (l.splice(h, 3), h -= 3);
             for (let h = 0, d = 0; h < f.children.length; h += 3) {
@@ -7519,15 +7519,15 @@
         return s.length || i.length ? new q(s, i) : P
     }
 
     function We(n, e) {
         return n.from - e.from || n.to - e.to
     }
 
-    function Tr(n) {
+    function Dr(n) {
         let e = n;
         for (let t = 0; t < e.length - 1; t++) {
             let r = e[t];
             if (r.from != r.to)
                 for (let i = t + 1; i < e.length; i++) {
                     let o = e[i];
                     if (o.from == r.from) {
@@ -7559,31 +7559,31 @@
             characterData: !0,
             characterDataOldValue: !0,
             attributes: !0,
             attributeOldValue: !0,
             subtree: !0
         },
         pc = W && Oe <= 11,
-        kr = class {
+        xr = class {
             constructor() {
                 this.anchorNode = null, this.anchorOffset = 0, this.focusNode = null, this.focusOffset = 0
             }
             set(e) {
                 this.anchorNode = e.anchorNode, this.anchorOffset = e.anchorOffset, this.focusNode = e.focusNode, this.focusOffset = e.focusOffset
             }
             clear() {
                 this.anchorNode = this.focusNode = null
             }
             eq(e) {
                 return e.anchorNode == this.anchorNode && e.anchorOffset == this.anchorOffset && e.focusNode == this.focusNode && e.focusOffset == this.focusOffset
             }
         },
-        xr = class {
+        kr = class {
             constructor(e, t) {
-                this.view = e, this.handleDOMChange = t, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new kr, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
+                this.view = e, this.handleDOMChange = t, this.queue = [], this.flushingSoon = -1, this.observer = null, this.currentSelection = new xr, this.onCharData = null, this.suppressingSelectionUpdates = !1, this.observer = window.MutationObserver && new window.MutationObserver(r => {
                     for (let i = 0; i < r.length; i++) this.queue.push(r[i]);
                     W && Oe <= 11 && r.some(i => i.type == "childList" && i.removedNodes.length || i.type == "characterData" && i.oldValue.length > i.target.nodeValue.length) ? this.flushSoon() : this.flush()
                 }), pc && (this.onCharData = r => {
                     this.queue.push({
                         target: r.target,
                         type: "characterData",
                         oldValue: r.prevValue
@@ -7668,15 +7668,15 @@
                     l = !1,
                     a = [];
                 if (e.editable)
                     for (let f = 0; f < t.length; f++) {
                         let h = this.registerMutation(t[f], a);
                         h && (o = o < 0 ? h.from : Math.min(h.from, o), s = s < 0 ? h.to : Math.max(h.to, s), h.typeOver && (l = !0))
                     }
-                if (X && a.length > 1) {
+                if (Z && a.length > 1) {
                     let f = a.filter(h => h.nodeName == "BR");
                     if (f.length == 2) {
                         let h = f[0],
                             d = f[1];
                         h.parentNode && h.parentNode.parentNode == d.parentNode ? d.remove() : h.remove()
                     }
                 }
@@ -7722,15 +7722,15 @@
             }
         },
         so = new WeakMap,
         lo = !1;
 
     function mc(n) {
         if (!so.has(n) && (so.set(n, null), ["normal", "nowrap", "pre-line"].indexOf(getComputedStyle(n.dom).whiteSpace) !== -1)) {
-            if (n.requiresGeckoHackNode = X, lo) return;
+            if (n.requiresGeckoHackNode = Z, lo) return;
             console.warn("ProseMirror expects the CSS white-space property to be set, preferably to 'pre-wrap'. It is recommended to load style/prosemirror.css from the prosemirror-view package."), lo = !0
         }
     }
 
     function ao(n, e) {
         let t = e.startContainer,
             r = e.startOffset,
@@ -7770,24 +7770,24 @@
                 node: f,
                 offset: a.anchorOffset
             }], pn(a) || c.push({
                 node: a.focusNode,
                 offset: a.focusOffset
             })), B && n.input.lastKeyCode === 8)
             for (let g = o; g > i; g--) {
-                let k = r.childNodes[g - 1],
-                    N = k.pmViewDesc;
-                if (k.nodeName == "BR" && !N) {
+                let x = r.childNodes[g - 1],
+                    N = x.pmViewDesc;
+                if (x.nodeName == "BR" && !N) {
                     o = g;
                     break
                 }
                 if (!N || N.size) break
             }
         let h = n.state.doc,
-            d = n.someProp("domParser") || ve.fromSchema(n.state.schema),
+            d = n.someProp("domParser") || Re.fromSchema(n.state.schema),
             p = h.resolve(s),
             u = null,
             m = d.parse(r, {
                 topNode: p.parent,
                 topMatch: p.parent.contentMatchAt(p.index()),
                 topOpen: !0,
                 from: i,
@@ -7795,18 +7795,18 @@
                 preserveWhitespace: p.parent.type.whitespace == "pre" ? "full" : !0,
                 findPositions: c,
                 ruleFromNode: bc,
                 context: p
             });
         if (c && c[0].pos != null) {
             let g = c[0].pos,
-                k = c[1] && c[1].pos;
-            k == null && (k = g), u = {
+                x = c[1] && c[1].pos;
+            x == null && (x = g), u = {
                 anchor: g + s,
-                head: k + s
+                head: x + s
             }
         }
         return {
             doc: m,
             sel: u,
             from: s,
             to: l
@@ -7826,23 +7826,23 @@
                 ignore: !0
             }
         } else if (n.nodeName == "IMG" && n.getAttribute("mark-placeholder")) return {
             ignore: !0
         };
         return null
     }
-    var kc = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
+    var xc = /^(a|abbr|acronym|b|bd[io]|big|br|button|cite|code|data(list)?|del|dfn|em|i|ins|kbd|label|map|mark|meter|output|q|ruby|s|samp|small|span|strong|su[bp]|time|u|tt|var)$/i;
 
-    function xc(n, e, t, r, i) {
+    function kc(n, e, t, r, i) {
         let o = n.input.compositionPendingChanges || (n.composing ? n.input.compositionID : 0);
         if (n.input.compositionPendingChanges = 0, e < 0) {
             let M = n.input.lastSelectionTime > Date.now() - 50 ? n.input.lastSelectionOrigin : null,
                 be = Mr(n, M);
             if (be && !n.state.selection.eq(be)) {
-                if (B && Y && n.input.lastKeyCode === 13 && Date.now() - 100 < n.input.lastKeyCodeTime && n.someProp("handleKeyDown", Bs => Bs(n, Be(13, "Enter")))) return;
+                if (B && Q && n.input.lastKeyCode === 13 && Date.now() - 100 < n.input.lastKeyCodeTime && n.someProp("handleKeyDown", Bs => Bs(n, Be(13, "Enter")))) return;
                 let Pt = n.state.tr.setSelection(be);
                 M == "pointer" ? Pt.setMeta("pointer", !0) : M == "key" && Pt.scrollIntoView(), o && Pt.setMeta("composition", o), n.dispatch(Pt)
             }
             return
         }
         let s = n.state.doc.resolve(e),
             l = s.sharedDepth(t);
@@ -7850,15 +7850,15 @@
         let a = n.state.selection,
             c = yc(n, e, t),
             f = n.state.doc,
             h = f.slice(c.from, c.to),
             d, p;
         n.input.lastKeyCode === 8 && Date.now() - 100 < n.input.lastKeyCodeTime ? (d = n.state.selection.to, p = "end") : (d = n.state.selection.from, p = "start"), n.input.lastKeyCode = null;
         let u = Cc(h.content, c.doc.content, c.from, d, p);
-        if ((tt && n.input.lastIOSEnter > Date.now() - 225 || Y) && i.some(M => M.nodeType == 1 && !kc.test(M.nodeName)) && (!u || u.endA >= u.endB) && n.someProp("handleKeyDown", M => M(n, Be(13, "Enter")))) {
+        if ((tt && n.input.lastIOSEnter > Date.now() - 225 || Q) && i.some(M => M.nodeType == 1 && !xc.test(M.nodeName)) && (!u || u.endA >= u.endB) && n.someProp("handleKeyDown", M => M(n, Be(13, "Enter")))) {
             n.input.lastIOSEnter = 0;
             return
         }
         if (!u)
             if (r && a instanceof w && !a.empty && a.$head.sameParent(a.$anchor) && !n.composing && !(c.sel && c.sel.anchor != c.sel.head)) u = {
                 start: a.from,
                 endA: a.to,
@@ -7872,47 +7872,47 @@
                         o && be.setMeta("composition", o), n.dispatch(be)
                     }
                 }
                 return
             } n.input.domChangeCount++, n.state.selection.from < n.state.selection.to && u.start == u.endB && n.state.selection instanceof w && (u.start > n.state.selection.from && u.start <= n.state.selection.from + 2 && n.state.selection.from >= c.from ? u.start = n.state.selection.from : u.endA < n.state.selection.to && u.endA >= n.state.selection.to - 2 && n.state.selection.to <= c.to && (u.endB += n.state.selection.to - u.endA, u.endA = n.state.selection.to)), W && Oe <= 11 && u.endB == u.start + 1 && u.endA == u.start && u.start > c.from && c.doc.textBetween(u.start - c.from - 1, u.start - c.from + 1) == " \xA0" && (u.start--, u.endA--, u.endB--);
         let m = c.doc.resolveNoCache(u.start - c.from),
             g = c.doc.resolveNoCache(u.endB - c.from),
-            k = f.resolve(u.start),
-            N = m.sameParent(g) && m.parent.inlineContent && k.end() >= u.endA,
+            x = f.resolve(u.start),
+            N = m.sameParent(g) && m.parent.inlineContent && x.end() >= u.endA,
             ee;
         if ((tt && n.input.lastIOSEnter > Date.now() - 225 && (!N || i.some(M => M.nodeName == "DIV" || M.nodeName == "P")) || !N && m.pos < c.doc.content.size && !m.sameParent(g) && (ee = S.findFrom(c.doc.resolve(m.pos + 1), 1, !0)) && ee.head == g.pos) && n.someProp("handleKeyDown", M => M(n, Be(13, "Enter")))) {
             n.input.lastIOSEnter = 0;
             return
         }
         if (n.state.selection.anchor > u.start && Mc(f, u.start, u.endA, m, g) && n.someProp("handleKeyDown", M => M(n, Be(8, "Backspace")))) {
-            Y && B && n.domObserver.suppressSelectionUpdates();
+            Q && B && n.domObserver.suppressSelectionUpdates();
             return
         }
-        B && Y && u.endB == u.start && (n.input.lastAndroidDelete = Date.now()), Y && !N && m.start() != g.start() && g.parentOffset == 0 && m.depth == g.depth && c.sel && c.sel.anchor == c.sel.head && c.sel.head == u.endA && (u.endB -= 2, g = c.doc.resolveNoCache(u.endB - c.from), setTimeout(() => {
+        B && Q && u.endB == u.start && (n.input.lastAndroidDelete = Date.now()), Q && !N && m.start() != g.start() && g.parentOffset == 0 && m.depth == g.depth && c.sel && c.sel.anchor == c.sel.head && c.sel.head == u.endA && (u.endB -= 2, g = c.doc.resolveNoCache(u.endB - c.from), setTimeout(() => {
             n.someProp("handleKeyDown", function(M) {
                 return M(n, Be(13, "Enter"))
             })
         }, 20));
         let te = u.start,
-            U = u.endA,
-            C, H, ne;
+            Y = u.endA,
+            C, j, ne;
         if (N) {
-            if (m.pos == g.pos) W && Oe <= 11 && m.parentOffset == 0 && (n.domObserver.suppressSelectionUpdates(), setTimeout(() => ge(n), 20)), C = n.state.tr.delete(te, U), H = f.resolve(u.start).marksAcross(f.resolve(u.endA));
-            else if (u.endA == u.endB && (ne = Sc(m.parent.content.cut(m.parentOffset, g.parentOffset), k.parent.content.cut(k.parentOffset, u.endA - k.start())))) C = n.state.tr, ne.type == "add" ? C.addMark(te, U, ne.mark) : C.removeMark(te, U, ne.mark);
+            if (m.pos == g.pos) W && Oe <= 11 && m.parentOffset == 0 && (n.domObserver.suppressSelectionUpdates(), setTimeout(() => ge(n), 20)), C = n.state.tr.delete(te, Y), j = f.resolve(u.start).marksAcross(f.resolve(u.endA));
+            else if (u.endA == u.endB && (ne = Sc(m.parent.content.cut(m.parentOffset, g.parentOffset), x.parent.content.cut(x.parentOffset, u.endA - x.start())))) C = n.state.tr, ne.type == "add" ? C.addMark(te, Y, ne.mark) : C.removeMark(te, Y, ne.mark);
             else if (m.parent.child(m.index()).isText && m.index() == g.index() - (g.textOffset ? 0 : 1)) {
                 let M = m.parent.textBetween(m.parentOffset, g.parentOffset);
-                if (n.someProp("handleTextInput", be => be(n, te, U, M))) return;
-                C = n.state.tr.insertText(M, te, U)
+                if (n.someProp("handleTextInput", be => be(n, te, Y, M))) return;
+                C = n.state.tr.insertText(M, te, Y)
             }
         }
-        if (C || (C = n.state.tr.replace(te, U, c.doc.slice(u.start - c.from, u.endB - c.from))), c.sel) {
+        if (C || (C = n.state.tr.replace(te, Y, c.doc.slice(u.start - c.from, u.endB - c.from))), c.sel) {
             let M = co(n, C.doc, c.sel);
-            M && !(B && Y && n.composing && M.empty && (u.start != u.endB || n.input.lastAndroidDelete < Date.now() - 100) && (M.head == te || M.head == C.mapping.map(U) - 1) || W && M.empty && M.head == te) && C.setSelection(M)
+            M && !(B && Q && n.composing && M.empty && (u.start != u.endB || n.input.lastAndroidDelete < Date.now() - 100) && (M.head == te || M.head == C.mapping.map(Y) - 1) || W && M.empty && M.head == te) && C.setSelection(M)
         }
-        H && C.ensureMarks(H), o && C.setMeta("composition", o), n.dispatch(C.scrollIntoView())
+        j && C.ensureMarks(j), o && C.setMeta("composition", o), n.dispatch(C.scrollIntoView())
     }
 
     function co(n, e, t) {
         return Math.max(t.anchor, t.head) > e.content.size ? null : Cr(n, e.resolve(t.anchor), e.resolve(t.head))
     }
 
     function Sc(n, e) {
@@ -7986,15 +7986,15 @@
         if (n.length != 2) return !1;
         let e = n.charCodeAt(0),
             t = n.charCodeAt(1);
         return e >= 56320 && e <= 57343 && t >= 55296 && t <= 56319
     }
     var un = class {
         constructor(e, t) {
-            this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new mr, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = t, this.state = t.state, this.directPlugins = t.plugins || [], this.directPlugins.forEach(go), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = po(this), uo(this), this.nodeViews = mo(this), this.docView = Hi(this.state.doc, ho(this), er(this), this.dom, this), this.domObserver = new xr(this, (r, i, o, s) => xc(this, r, i, o, s)), this.domObserver.start(), Ua(this), this.updatePluginViews()
+            this._root = null, this.focused = !1, this.trackWrites = null, this.mounted = !1, this.markCursor = null, this.cursorWrapper = null, this.lastSelectedViewDesc = void 0, this.input = new mr, this.prevDirectPlugins = [], this.pluginViews = [], this.requiresGeckoHackNode = !1, this.dragging = null, this._props = t, this.state = t.state, this.directPlugins = t.plugins || [], this.directPlugins.forEach(go), this.dispatch = this.dispatch.bind(this), this.dom = e && e.mount || document.createElement("div"), e && (e.appendChild ? e.appendChild(this.dom) : typeof e == "function" ? e(this.dom) : e.mount && (this.mounted = !0)), this.editable = po(this), uo(this), this.nodeViews = mo(this), this.docView = Hi(this.state.doc, ho(this), er(this), this.dom, this), this.domObserver = new kr(this, (r, i, o, s) => kc(this, r, i, o, s)), this.domObserver.start(), Ua(this), this.updatePluginViews()
         }
         get composing() {
             return this.input.composing
         }
         get props() {
             if (this._props.state != this.state) {
                 let e = this._props;
@@ -8039,22 +8039,22 @@
             if (s) {
                 this.domObserver.stop();
                 let p = h && (W || B) && !this.composing && !i.selection.empty && !e.selection.empty && Oc(i.selection, e.selection);
                 if (h) {
                     let u = B ? this.trackWrites = this.domSelectionRange().focusNode : null;
                     this.composing && (this.input.compositionNode = sc(this)), (o || !this.docView.update(e.doc, c, a, this)) && (this.docView.updateOuterDeco(c), this.docView.destroy(), this.docView = Hi(e.doc, c, a, this.dom, this)), u && !this.trackWrites && (p = !0)
                 }
-                p || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && Pa(this)) ? ge(this, p) : (Do(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
+                p || !(this.input.mouseDown && this.domObserver.currentSelection.eq(this.domSelectionRange()) && Pa(this)) ? ge(this, p) : (To(this, e.selection), this.domObserver.setCurSelection()), this.domObserver.start()
             }
             this.updatePluginViews(i), !((r = this.dragging) === null || r === void 0) && r.node && !i.doc.eq(e.doc) && this.updateDraggedNode(this.dragging, i), f == "reset" ? this.dom.scrollTop = 0 : f == "to selection" ? this.scrollToSelection() : d && pa(d)
         }
         scrollToSelection() {
             let e = this.domSelectionRange().focusNode;
             if (!this.someProp("handleScrollToSelection", t => t(this)))
-                if (this.state.selection instanceof x) {
+                if (this.state.selection instanceof k) {
                     let t = this.docView.domAfterPos(this.state.selection.from);
                     t.nodeType == 1 && Li(this, t.getBoundingClientRect(), e)
                 } else Li(this, this.coordsAtPos(this.state.selection.head, 1), e)
         }
         destroyPluginViews() {
             let e;
             for (; e = this.pluginViews.pop();) e.destroy && e.destroy()
@@ -8080,15 +8080,15 @@
             let r = e.node,
                 i = -1;
             if (this.state.doc.nodeAt(r.from) == r.node) i = r.from;
             else {
                 let o = r.from + (this.state.doc.content.size - t.doc.content.size);
                 (o > 0 && this.state.doc.nodeAt(o)) == r.node && (i = o)
             }
-            this.dragging = new cn(e.slice, e.move, i < 0 ? void 0 : x.create(this.state.doc, i))
+            this.dragging = new cn(e.slice, e.move, i < 0 ? void 0 : k.create(this.state.doc, i))
         }
         someProp(e, t) {
             let r = this._props && this._props[e],
                 i;
             if (r != null && (i = t ? t(r) : r)) return i;
             for (let s = 0; s < this.directPlugins.length; s++) {
                 let l = this.directPlugins[s].props[e];
@@ -8125,15 +8125,15 @@
             }
             return e || document
         }
         updateRoot() {
             this._root = null
         }
         posAtCoords(e) {
-            return xa(this, e)
+            return ka(this, e)
         }
         coordsAtPos(e, t = 1) {
             return Mo(this, e, t)
         }
         domAtPos(e, t = 0) {
             return this.docView.domFromPos(e, t)
         }
@@ -8251,19 +8251,19 @@
             }
         }
         static fromJSON(e, t) {
             if (typeof t.pos != "number") throw new RangeError("Invalid input for GapCursor.fromJSON");
             return new n(e.resolve(t.pos))
         }
         getBookmark() {
-            return new Dr(this.anchor)
+            return new Tr(this.anchor)
         }
         static valid(e) {
             let t = e.parent;
-            if (t.isTextblock || !Nc(e) || !Tc(e)) return !1;
+            if (t.isTextblock || !Nc(e) || !Dc(e)) return !1;
             let r = t.type.spec.allowGapCursor;
             if (r != null) return r;
             let i = t.contentMatchAt(e.index()).defaultType;
             return i && i.isTextblock
         }
         static findGapCursorFrom(e, t, r = !1) {
             e: for (;;) {
@@ -8279,15 +8279,15 @@
                     i += t;
                     let a = e.doc.resolve(i);
                     if (n.valid(a)) return a
                 }
                 for (;;) {
                     let s = t > 0 ? o.firstChild : o.lastChild;
                     if (!s) {
-                        if (o.isAtom && !o.isText && !x.isSelectable(o)) {
+                        if (o.isAtom && !o.isText && !k.isSelectable(o)) {
                             e = e.doc.resolve(i + o.nodeSize * t), r = !1;
                             continue e
                         }
                         break
                     }
                     o = s, i += t;
                     let l = e.doc.resolve(i);
@@ -8296,15 +8296,15 @@
                 return null
             }
         }
     };
     z.prototype.visible = !1;
     z.findFrom = z.findGapCursorFrom;
     S.jsonID("gapcursor", z);
-    var Dr = class n {
+    var Tr = class n {
         constructor(e) {
             this.pos = e
         }
         map(e) {
             return new n(e.map(this.pos))
         }
         resolve(e) {
@@ -8325,15 +8325,15 @@
                 if (i.childCount == 0 && !i.inlineContent || i.isAtom || i.type.spec.isolating) return !0;
                 if (i.inlineContent) return !1
             }
         }
         return !0
     }
 
-    function Tc(n) {
+    function Dc(n) {
         for (let e = n.depth; e >= 0; e--) {
             let t = n.indexAfter(e),
                 r = n.node(e);
             if (t == r.childCount) {
                 if (r.type.spec.isolating) return !0;
                 continue
             }
@@ -8349,22 +8349,22 @@
         return new J({
             props: {
                 decorations: Ic,
                 createSelectionBetween(n, e, t) {
                     return e.pos == t.pos && z.valid(t) ? new z(t) : null
                 },
                 handleClick: Ec,
-                handleKeyDown: Dc,
+                handleKeyDown: Tc,
                 handleDOMEvents: {
                     beforeinput: Ac
                 }
             }
         })
     }
-    var Dc = Xn({
+    var Tc = Xn({
         ArrowLeft: gn("horiz", -1),
         ArrowRight: gn("horiz", 1),
         ArrowUp: gn("vert", -1),
         ArrowDown: gn("vert", 1)
     });
 
     function gn(n, e) {
@@ -8386,15 +8386,15 @@
         if (!n || !n.editable) return !1;
         let r = n.state.doc.resolve(e);
         if (!z.valid(r)) return !1;
         let i = n.posAtCoords({
             left: t.clientX,
             top: t.clientY
         });
-        return i && i.inside > -1 && x.isSelectable(n.state.doc.nodeAt(i.inside)) ? !1 : (n.dispatch(n.state.tr.setSelection(new z(r))), !0)
+        return i && i.inside > -1 && k.isSelectable(n.state.doc.nodeAt(i.inside)) ? !1 : (n.dispatch(n.state.tr.setSelection(new z(r))), !0)
     }
 
     function Ac(n, e) {
         if (e.inputType != "insertCompositionText" || !(n.state.selection instanceof z)) return !1;
         let {
             $from: t
         } = n.state.selection, r = t.parent.contentMatchAt(t.index()).findWrapping(n.state.schema.nodes.text);
@@ -8409,42 +8409,42 @@
         if (!(n.selection instanceof z)) return null;
         let e = document.createElement("div");
         return e.className = "ProseMirror-gapcursor", q.create(n.doc, [ae.widget(n.selection.head, e, {
             key: "gapcursor"
         })])
     }
     var yn = 200,
-        R = function() {};
-    R.prototype.append = function(e) {
-        return e.length ? (e = R.from(e), !this.length && e || e.length < yn && this.leafAppend(e) || this.length < yn && e.leafPrepend(this) || this.appendInner(e)) : this
+        v = function() {};
+    v.prototype.append = function(e) {
+        return e.length ? (e = v.from(e), !this.length && e || e.length < yn && this.leafAppend(e) || this.length < yn && e.leafPrepend(this) || this.appendInner(e)) : this
     };
-    R.prototype.prepend = function(e) {
-        return e.length ? R.from(e).append(this) : this
+    v.prototype.prepend = function(e) {
+        return e.length ? v.from(e).append(this) : this
     };
-    R.prototype.appendInner = function(e) {
-        return new Rc(this, e)
+    v.prototype.appendInner = function(e) {
+        return new vc(this, e)
     };
-    R.prototype.slice = function(e, t) {
-        return e === void 0 && (e = 0), t === void 0 && (t = this.length), e >= t ? R.empty : this.sliceInner(Math.max(0, e), Math.min(this.length, t))
+    v.prototype.slice = function(e, t) {
+        return e === void 0 && (e = 0), t === void 0 && (t = this.length), e >= t ? v.empty : this.sliceInner(Math.max(0, e), Math.min(this.length, t))
     };
-    R.prototype.get = function(e) {
+    v.prototype.get = function(e) {
         if (!(e < 0 || e >= this.length)) return this.getInner(e)
     };
-    R.prototype.forEach = function(e, t, r) {
+    v.prototype.forEach = function(e, t, r) {
         t === void 0 && (t = 0), r === void 0 && (r = this.length), t <= r ? this.forEachInner(e, t, r, 0) : this.forEachInvertedInner(e, t, r, 0)
     };
-    R.prototype.map = function(e, t, r) {
+    v.prototype.map = function(e, t, r) {
         t === void 0 && (t = 0), r === void 0 && (r = this.length);
         var i = [];
         return this.forEach(function(o, s) {
             return i.push(e(o, s))
         }, t, r), i
     };
-    R.from = function(e) {
-        return e instanceof R ? e : e && e.length ? new Uo(e) : R.empty
+    v.from = function(e) {
+        return e instanceof v ? e : e && e.length ? new Uo(e) : v.empty
     };
     var Uo = function(n) {
         function e(r) {
             n.call(this), this.values = r
         }
         n && (e.__proto__ = n), e.prototype = Object.create(n && n.prototype), e.prototype.constructor = e;
         var t = {
@@ -8472,17 +8472,17 @@
         }, e.prototype.leafPrepend = function(i) {
             if (this.length + i.length <= yn) return new e(i.flatten().concat(this.values))
         }, t.length.get = function() {
             return this.values.length
         }, t.depth.get = function() {
             return 0
         }, Object.defineProperties(e.prototype, t), e
-    }(R);
-    R.empty = new Uo([]);
-    var Rc = function(n) {
+    }(v);
+    v.empty = new Uo([]);
+    var vc = function(n) {
             function e(t, r) {
                 n.call(this), this.left = t, this.right = r, this.length = t.length + r.length, this.depth = Math.max(t.depth, r.depth) + 1
             }
             return n && (e.__proto__ = n), e.prototype = Object.create(n && n.prototype), e.prototype.constructor = e, e.prototype.flatten = function() {
                 return this.left.flatten().concat(this.right.flatten())
             }, e.prototype.getInner = function(r) {
                 return r < this.left.length ? this.left.get(r) : this.right.get(r - this.left.length)
@@ -8501,17 +8501,17 @@
                 if (i) return new e(this.left, i)
             }, e.prototype.leafPrepend = function(r) {
                 var i = this.left.leafPrepend(r);
                 if (i) return new e(i, this.right)
             }, e.prototype.appendInner = function(r) {
                 return this.left.depth >= Math.max(this.right.depth, r.depth) + 1 ? new e(this.left, new e(this.right, r)) : new e(this, r)
             }, e
-        }(R),
-        Er = R;
-    var vc = 500,
+        }(v),
+        Er = v;
+    var Rc = 500,
         He = class n {
             constructor(e, t) {
                 this.items = e, this.eventCount = t
             }
             popEvent(e, t) {
                 if (this.eventCount == 0) return null;
                 let r = this.items.length;
@@ -8588,15 +8588,15 @@
                         g && l++, r.push(new ce(u, m, g))
                     } else r.push(new ce(u))
                 }, i);
                 let c = [];
                 for (let d = t; d < s; d++) c.push(new ce(o.maps[d]));
                 let f = this.items.slice(0, i).append(c).append(r),
                     h = new n(f, l);
-                return h.emptyItemCount() > vc && (h = h.compress(this.items.length - r.length)), h
+                return h.emptyItemCount() > Rc && (h = h.compress(this.items.length - r.length)), h
             }
             emptyItemCount() {
                 let e = 0;
                 return this.items.forEach(t => {
                     t.step || e++
                 }), e
             }
@@ -8712,16 +8712,16 @@
                 if (e[t].spec.historyPreserveItems) {
                     Ir = !0;
                     break
                 }
         }
         return Ir
     }
-    var $e = new kt("history"),
-        Lc = new kt("closeHistory");
+    var $e = new xt("history"),
+        Lc = new xt("closeHistory");
 
     function Xo(n = {}) {
         return n = {
             depth: n.depth || 100,
             newGroupDelay: n.newGroupDelay || 500
         }, new J({
             key: $e,
@@ -8742,29 +8742,29 @@
                         return i ? (t.preventDefault(), i(e.state, e.dispatch)) : !1
                     }
                 }
             }
         })
     }
 
-    function kn(n, e) {
+    function xn(n, e) {
         return (t, r) => {
             let i = $e.getState(t);
             if (!i || (n ? i.undone : i.done).eventCount == 0) return !1;
             if (r) {
                 let o = Vc(i, t, n);
                 o && r(e ? o.scrollIntoView() : o)
             }
             return !0
         }
     }
-    var At = kn(!1, !0),
-        rt = kn(!0, !0),
-        Ph = kn(!1, !1),
-        zh = kn(!0, !1);
+    var At = xn(!1, !0),
+        rt = xn(!0, !0),
+        Ph = xn(!1, !1),
+        zh = xn(!0, !1);
     var Jc = ["p", 0],
         Wc = ["blockquote", 0],
         qc = ["hr"],
         Kc = ["pre", ["code", 0]],
         $c = ["br"],
         ye = {
             doc: {
@@ -8978,15 +8978,15 @@
                     tag: "code"
                 }],
                 toDOM() {
                     return _c
                 }
             }
         },
-        Vh = new ke({
+        Vh = new xe({
             nodes: ye,
             marks: It
         });
     var Uc = ["ol", 0],
         Gc = ["ul", 0],
         Yc = ["li", 0],
         Xc = {
@@ -9023,32 +9023,32 @@
             }],
             toDOM() {
                 return Yc
             },
             defining: !0
         };
 
-    function Rr(n, e) {
+    function vr(n, e) {
         let t = {};
         for (let r in n) t[r] = n[r];
         for (let r in e) t[r] = e[r];
         return t
     }
 
     function Qo(n, e, t) {
         return n.append({
-            ordered_list: Rr(Xc, {
+            ordered_list: vr(Xc, {
                 content: "list_item+",
                 group: t
             }),
-            bullet_list: Rr(Qc, {
+            bullet_list: vr(Qc, {
                 content: "list_item+",
                 group: t
             }),
-            list_item: Rr(Zc, {
+            list_item: vr(Zc, {
                 content: e
             })
         })
     }
 
     function it(n, e = null) {
         return function(t, r) {
@@ -9072,15 +9072,15 @@
         for (let f = t.length - 1; f >= 0; f--) o = y.from(t[f].type.create(t[f].attrs, o));
         n.step(new E(e.start - (r ? 2 : 0), e.end, e.start, e.end, new b(o, 0, 0), t.length, !0));
         let s = 0;
         for (let f = 0; f < t.length; f++) t[f].type == i && (s = f + 1);
         let l = t.length - s,
             a = e.start + t.length - (r ? 2 : 0),
             c = e.parent;
-        for (let f = e.startIndex, h = e.endIndex, d = !0; f < h; f++, d = !1) !d && xe(n.doc, a, l) && (n.split(a, l), a += 2 * l), a += c.child(f).nodeSize;
+        for (let f = e.startIndex, h = e.endIndex, d = !0; f < h; f++, d = !1) !d && ke(n.doc, a, l) && (n.split(a, l), a += 2 * l), a += c.child(f).nodeSize;
         return n
     }
 
     function Zo(n, e) {
         return function(t, r) {
             let {
                 $from: i,
@@ -9091,36 +9091,36 @@
             let l = i.node(-1);
             if (l.type != n) return !1;
             if (i.parent.content.size == 0 && i.node(-1).childCount == i.indexAfter(-1)) {
                 if (i.depth == 3 || i.node(-3).type != n || i.index(-2) != i.node(-2).childCount - 1) return !1;
                 if (r) {
                     let h = y.empty,
                         d = i.index(-1) ? 1 : i.index(-2) ? 2 : 3;
-                    for (let k = i.depth - d; k >= i.depth - 3; k--) h = y.from(i.node(k).copy(h));
+                    for (let x = i.depth - d; x >= i.depth - 3; x--) h = y.from(i.node(x).copy(h));
                     let p = i.indexAfter(-1) < i.node(-2).childCount ? 1 : i.indexAfter(-2) < i.node(-3).childCount ? 2 : 3;
                     h = h.append(y.from(n.createAndFill()));
                     let u = i.before(i.depth - (d - 1)),
                         m = t.tr.replace(u, i.after(-p), new b(h, 4 - d, 0)),
                         g = -1;
-                    m.doc.nodesBetween(u, m.doc.content.size, (k, N) => {
+                    m.doc.nodesBetween(u, m.doc.content.size, (x, N) => {
                         if (g > -1) return !1;
-                        k.isTextblock && k.content.size == 0 && (g = N + 1)
+                        x.isTextblock && x.content.size == 0 && (g = N + 1)
                     }), g > -1 && m.setSelection(S.near(m.doc.resolve(g))), r(m.scrollIntoView())
                 }
                 return !0
             }
             let a = o.pos == i.end() ? l.contentMatchAt(0).defaultType : null,
                 c = t.tr.delete(i.pos, o.pos),
                 f = a ? [e ? {
                     type: n,
                     attrs: e
                 } : null, {
                     type: a
                 }] : void 0;
-            return xe(c.doc, i.pos, 2, f) ? (r && r(c.split(i.pos, 2, f).scrollIntoView()), !0) : !1
+            return ke(c.doc, i.pos, 2, f) ? (r && r(c.split(i.pos, 2, f).scrollIntoView()), !0) : !1
         }
     }
 
     function es(n) {
         return function(e, t) {
             let {
                 $from: r,
@@ -9178,15 +9178,15 @@
                     d = o.start,
                     p = o.end;
                 t(e.tr.step(new E(d - (c ? 3 : 1), p, d, p, h, 1, !0)).scrollIntoView())
             }
             return !0
         }
     }
-    var Te = class {
+    var De = class {
         constructor(e, t, r = {}) {
             this.match = e, this.match = e, this.handler = typeof t == "string" ? rf(t) : t, this.undoable = r.undoable !== !1, this.inCode = r.inCode || !1
         }
     };
 
     function rf(n) {
         return function(e, t, r, i) {
@@ -9217,64 +9217,64 @@
                         e(s)
                     }
                     return !0
                 }
             }
             return !1
         },
-        $h = new Te(/--$/, "\u2014"),
-        Hh = new Te(/\.\.\.$/, "\u2026"),
-        jh = new Te(/(?:^|[\s\{\[\(\<'"\u2018\u201C])(")$/, "\u201C"),
-        _h = new Te(/"$/, "\u201D"),
-        Uh = new Te(/(?:^|[\s\{\[\(\<'"\u2018\u201C])(')$/, "\u2018"),
-        Gh = new Te(/'$/, "\u2019");
+        $h = new De(/--$/, "\u2014"),
+        Hh = new De(/\.\.\.$/, "\u2026"),
+        jh = new De(/(?:^|[\s\{\[\(\<'"\u2018\u201C])(")$/, "\u201C"),
+        _h = new De(/"$/, "\u201D"),
+        Uh = new De(/(?:^|[\s\{\[\(\<'"\u2018\u201C])(')$/, "\u2018"),
+        Gh = new De(/'$/, "\u2019");
 
     function of(n, e) {
         let t = Object.keys(e);
         return t.length ? !!t.filter(r => e[r] === n[r]).length : !0
     }
 
-    function vr(n, e, t = {}) {
+    function Rr(n, e, t = {}) {
         return n.find(r => r.type === e && of(r.attrs, t))
     }
 
     function sf(n, e, t = {}) {
-        return !!vr(n, e, t)
+        return !!Rr(n, e, t)
     }
 
     function Pr(n, e, t = {}) {
         if (!n || !e) return;
         let r = n.parent.childAfter(n.parentOffset);
         if (!r.node) return;
-        let i = vr(r.node.marks, e, t);
+        let i = Rr(r.node.marks, e, t);
         if (!i) return;
         let o = n.index(),
             s = n.start() + r.offset,
             l = o + 1,
             a = s + r.node.nodeSize;
-        for (vr(r.node.marks, e, t); o > 0 && i.isInSet(n.parent.child(o - 1).marks);) o -= 1, s -= n.parent.child(o).nodeSize;
+        for (Rr(r.node.marks, e, t); o > 0 && i.isInSet(n.parent.child(o - 1).marks);) o -= 1, s -= n.parent.child(o).nodeSize;
         for (; l < n.parent.childCount && sf(n.parent.child(l).marks, e, t);) a += n.parent.child(l).nodeSize, l += 1;
         return {
             from: s,
             to: a
         }
     }
 
     function lf(n) {
         var e = typeof n;
         return n != null && (e == "object" || e == "function")
     }
-    var Rt = lf;
+    var vt = lf;
     var af = typeof global == "object" && global && global.Object === Object && global,
         rs = af;
     var cf = typeof self == "object" && self && self.Object === Object && self,
         ff = rs || cf || Function("return this")(),
-        xn = ff;
+        kn = ff;
     var hf = function() {
-            return xn.Date.now()
+            return kn.Date.now()
         },
         Sn = hf;
     var df = /\s/;
 
     function uf(n) {
         for (var e = n.length; e-- && df.test(n.charAt(e)););
         return e
@@ -9282,34 +9282,34 @@
     var is = uf;
     var pf = /^\s+/;
 
     function mf(n) {
         return n && n.slice(0, is(n) + 1).replace(pf, "")
     }
     var ss = mf;
-    var gf = xn.Symbol,
+    var gf = kn.Symbol,
         ot = gf;
     var ls = Object.prototype,
         yf = ls.hasOwnProperty,
         bf = ls.toString,
-        vt = ot ? ot.toStringTag : void 0;
+        Rt = ot ? ot.toStringTag : void 0;
 
-    function kf(n) {
-        var e = yf.call(n, vt),
-            t = n[vt];
+    function xf(n) {
+        var e = yf.call(n, Rt),
+            t = n[Rt];
         try {
-            n[vt] = void 0;
+            n[Rt] = void 0;
             var r = !0
         } catch (o) {}
         var i = bf.call(n);
-        return r && (e ? n[vt] = t : delete n[vt]), i
+        return r && (e ? n[Rt] = t : delete n[Rt]), i
     }
-    var as = kf;
-    var xf = Object.prototype,
-        Sf = xf.toString;
+    var as = xf;
+    var kf = Object.prototype,
+        Sf = kf.toString;
 
     function Mf(n) {
         return Sf.call(n)
     }
     var cs = Mf;
     var Cf = "[object Null]",
         Of = "[object Undefined]",
@@ -9320,127 +9320,127 @@
     }
     var hs = wf;
 
     function Nf(n) {
         return n != null && typeof n == "object"
     }
     var ds = Nf;
-    var Tf = "[object Symbol]";
+    var Df = "[object Symbol]";
 
-    function Df(n) {
-        return typeof n == "symbol" || ds(n) && hs(n) == Tf
+    function Tf(n) {
+        return typeof n == "symbol" || ds(n) && hs(n) == Df
     }
-    var us = Df;
+    var us = Tf;
     var ps = NaN,
         Ef = /^[-+]0x[0-9a-f]+$/i,
         Af = /^0b[01]+$/i,
         If = /^0o[0-7]+$/i,
-        Rf = parseInt;
+        vf = parseInt;
 
-    function vf(n) {
+    function Rf(n) {
         if (typeof n == "number") return n;
         if (us(n)) return ps;
-        if (Rt(n)) {
+        if (vt(n)) {
             var e = typeof n.valueOf == "function" ? n.valueOf() : n;
-            n = Rt(e) ? e + "" : e
+            n = vt(e) ? e + "" : e
         }
         if (typeof n != "string") return n === 0 ? n : +n;
         n = ss(n);
         var t = Af.test(n);
-        return t || If.test(n) ? Rf(n.slice(2), t ? 2 : 8) : Ef.test(n) ? ps : +n
+        return t || If.test(n) ? vf(n.slice(2), t ? 2 : 8) : Ef.test(n) ? ps : +n
     }
-    var zr = vf;
+    var zr = Rf;
     var Pf = "Expected a function",
         zf = Math.max,
         Bf = Math.min;
 
     function Ff(n, e, t) {
         var r, i, o, s, l, a, c = 0,
             f = !1,
             h = !1,
             d = !0;
         if (typeof n != "function") throw new TypeError(Pf);
-        e = zr(e) || 0, Rt(t) && (f = !!t.leading, h = "maxWait" in t, o = h ? zf(zr(t.maxWait) || 0, e) : o, d = "trailing" in t ? !!t.trailing : d);
+        e = zr(e) || 0, vt(t) && (f = !!t.leading, h = "maxWait" in t, o = h ? zf(zr(t.maxWait) || 0, e) : o, d = "trailing" in t ? !!t.trailing : d);
 
         function p(C) {
-            var H = r,
+            var j = r,
                 ne = i;
-            return r = i = void 0, c = C, s = n.apply(ne, H), s
+            return r = i = void 0, c = C, s = n.apply(ne, j), s
         }
 
         function u(C) {
-            return c = C, l = setTimeout(k, e), f ? p(C) : s
+            return c = C, l = setTimeout(x, e), f ? p(C) : s
         }
 
         function m(C) {
-            var H = C - a,
+            var j = C - a,
                 ne = C - c,
-                M = e - H;
+                M = e - j;
             return h ? Bf(M, o - ne) : M
         }
 
         function g(C) {
-            var H = C - a,
+            var j = C - a,
                 ne = C - c;
-            return a === void 0 || H >= e || H < 0 || h && ne >= o
+            return a === void 0 || j >= e || j < 0 || h && ne >= o
         }
 
-        function k() {
+        function x() {
             var C = Sn();
             if (g(C)) return N(C);
-            l = setTimeout(k, m(C))
+            l = setTimeout(x, m(C))
         }
 
         function N(C) {
             return l = void 0, d && r ? p(C) : (r = i = void 0, s)
         }
 
         function ee() {
             l !== void 0 && clearTimeout(l), c = 0, r = a = i = l = void 0
         }
 
         function te() {
             return l === void 0 ? s : N(Sn())
         }
 
-        function U() {
+        function Y() {
             var C = Sn(),
-                H = g(C);
-            if (r = arguments, i = this, a = C, H) {
+                j = g(C);
+            if (r = arguments, i = this, a = C, j) {
                 if (l === void 0) return u(a);
-                if (h) return clearTimeout(l), l = setTimeout(k, e), p(a)
+                if (h) return clearTimeout(l), l = setTimeout(x, e), p(a)
             }
-            return l === void 0 && (l = setTimeout(k, e)), s
+            return l === void 0 && (l = setTimeout(x, e)), s
         }
-        return U.cancel = ee, U.flush = te, U
+        return Y.cancel = ee, Y.flush = te, Y
     }
     var ms = Ff;
-    var Q = (n, e = null) => {
+    var H = (n, e = null) => {
         let t = document.createElement(n);
         if (e)
             for (let [r, i] of Object.entries(e)) /^data-|^aria-|^role/.test(r) ? t.setAttribute(r, i) : t[r] = i;
         return t
     };
 
     function Mn(n, e) {
         let t = document.createElement("article");
-        return t.innerHTML = e, ve.fromSchema(n).parse(t)
+        return t.innerHTML = e, Re.fromSchema(n).parse(t)
     }
 
     function gs(n) {
         let {
             schema: e,
             doc: t
-        } = n, r = ie.fromSchema(e), i = Q("article");
+        } = n, r = ie.fromSchema(e), i = H("article");
         return i.appendChild(r.serializeFragment(t.content)), i.innerHTML
     }
     var ys = (n, e, t) => {
             let r = ie.fromSchema(n),
                 i = function() {
-                    let s = Q("article");
+                    let s = H("article");
                     return s.appendChild(r.serializeFragment(e.state.doc.content)), s.innerHTML
                 };
             return ms(() => {
                 let s = i();
                 t.value !== s && (t.value = s, t.dispatchEvent(new InputEvent("input", {
                     bubbles: !0,
                     cancelable: !0
@@ -9502,15 +9502,15 @@
                             e(n.tr.addMark(a, c, i.create(s)))
                         }
                     }
                 })
             }
             return !0
         },
-        ks = (n, e) => {
+        xs = (n, e) => {
             let t = n.schema.marks.link,
                 {
                     $from: r,
                     from: i,
                     to: o
                 } = n.selection,
                 s = Pr(r, t);
@@ -9533,15 +9533,15 @@
                 r.close()
             }), r.addEventListener("close", () => {
                 t.remove(), e(null)
             }), t.querySelector("button[type=submit]").addEventListener("click", o => {
                 o.preventDefault(), i.reportValidity() && (t.remove(), e(i.html.value))
             }), r.showModal()
         }),
-        xs = (n, e) => (e && Lf(gs(n)).then(t => {
+        ks = (n, e) => (e && Lf(gs(n)).then(t => {
             if (t) {
                 let r = Mn(n.schema, t);
                 e(n.tr.replaceWith(0, n.tr.doc.content.size, r))
             }
         }), !0),
         Ss = (n, e) => (e && e(n.tr.replaceSelectionWith(n.schema.nodes.horizontal_rule.create())), !0);
     var Ms = typeof navigator != "undefined" ? /Mac|iP(hone|[oa]d)/.test(navigator.platform) : !1,
@@ -9550,180 +9550,189 @@
         };
 
     function Os(n) {
         let e = {},
             t, r = Cs(e);
         if (r("Mod-z", At), r("Shift-Mod-z", rt), r("Backspace", ns), Ms || r("Mod-y", rt), t = n.nodes.hard_break) {
             let i = t,
-                o = xt(jn, (s, l) => (l && l(s.tr.replaceSelectionWith(i.create()).scrollIntoView()), !0));
+                o = kt(jn, (s, l) => (l && l(s.tr.replaceSelectionWith(i.create()).scrollIntoView()), !0));
             r("Mod-Enter", o), r("Shift-Enter", o), Ms && r("Ctrl-Enter", o)
         }
         return (t = n.nodes.bullet_list) && r("Shift-Ctrl-8", it(t)), (t = n.nodes.ordered_list) && r("Shift-Ctrl-9", it(t)), (t = n.nodes.blockquote) && r("Ctrl->", en(t)), (t = n.nodes.list_item) && (r("Enter", Zo(t)), r("Mod-[", es(t)), r("Mod-]", ts(t))), e
     }
 
     function ws(n) {
         let e = {},
             t, r = Cs(e);
-        return (t = n.marks.strong) && (r("Mod-b", G(t)), r("Mod-B", G(t))), (t = n.marks.em) && (r("Mod-i", G(t)), r("Mod-I", G(t))), (t = n.marks.underline) && (r("Mod-Shift-u", G(t)), r("Mod-Shift-U", G(t))), (t = n.marks.strikethrough) && (r("Mod-Shift-s", G(t)), r("Mod-Shift-S", G(t))), (t = n.marks.link) && (r("Mod-k", st), r("Mod-K", st)), e
+        return (t = n.marks.strong) && (r("Mod-b", X(t)), r("Mod-B", X(t))), (t = n.marks.em) && (r("Mod-i", X(t)), r("Mod-I", X(t))), (t = n.marks.underline) && (r("Mod-Shift-u", X(t)), r("Mod-Shift-U", X(t))), (t = n.marks.strikethrough) && (r("Mod-Shift-s", X(t)), r("Mod-Shift-S", X(t))), (t = n.marks.link) && (r("Mod-k", st), r("Mod-K", st)), e
     }
 
-    function Ns(n) {
+    function Ns(n, e) {
         return new J({
-            view(e) {
-                let t = new Br(n, e);
-                return e.dom.parentNode.insertBefore(t.dom, e.dom), t
+            view(t) {
+                let r = new Br(t, n, e);
+                return t.dom.parentNode.insertBefore(r.dom, t.dom), r
             }
         })
     }
 
-    function Ts(n, e) {
+    function Ds(n, e) {
         let {
             from: t,
             $from: r,
             to: i,
             empty: o
         } = n.selection;
         return o ? e.isInSet(n.storedMarks || r.marks()) : n.doc.rangeHasMark(t, i, e)
     }
 
     function Jf(n) {
-        let e = Q("span", {
+        let e = H("span", {
             className: "prose-menubar__button prose-menubar__button--heading"
         });
-        return e.append(Q("span", {
+        return e.append(H("span", {
             className: "material-icons",
             textContent: "title",
             title: `heading ${n}`
-        }), Q("span", {
+        }), H("span", {
             className: "level",
             textContent: `${n}`
         })), e
     }
 
-    function Z(n, e) {
-        return Q("span", {
+    function G(n, e) {
+        return H("span", {
             className: "prose-menubar__button material-icons",
             textContent: n,
             title: e
         })
     }
 
-    function Ds(n) {
+    function Ts(n) {
         if (!n.nodes.heading) return [];
         let e = t => ({
             command: _n(n.nodes.heading, {
                 level: t
             }),
             dom: Jf(t),
             active(r) {
                 return r.selection.$from.parent.hasMarkup(n.nodes.heading, {
                     level: t
                 })
             }
         });
-        return [e(1), e(2), e(3), {
+        return [e(1), e(2), e(3), e(4), e(5), {
             command: _n(n.nodes.paragraph),
-            dom: Z("notes", "paragraph"),
+            dom: G("notes", "paragraph"),
             active(t) {
                 return t.selection.$from.parent.hasMarkup(n.nodes.paragraph)
             }
         }]
     }
 
     function Es(n) {
         let e = [],
             t;
         return (t = n.nodes.bullet_list) && e.push({
             command: it(t),
-            dom: Z("format_list_bulleted", "unordered list"),
+            dom: G("format_list_bulleted", "unordered list"),
             active(r) {
                 return !1
             }
         }), (t = n.nodes.ordered_list) && e.push({
             command: it(t),
-            dom: Z("format_list_numbered", "ordered list"),
+            dom: G("format_list_numbered", "ordered list"),
             active(r) {
                 return !1
             }
         }), (t = n.nodes.blockquote) && e.push({
             command: en(t),
-            dom: Z("format_quote", "blockquote"),
+            dom: G("format_quote", "blockquote"),
             active(r) {
                 return !1
             }
         }), (t = n.nodes.horizontal_rule) && e.push({
             command: Ss,
-            dom: Z("horizontal_rule", "horizontal rule"),
+            dom: G("horizontal_rule", "horizontal rule"),
             active(r) {
                 return !1
             }
         }), e
     }
 
     function As(n) {
         let e = (t, r, i) => t ? {
-            command: G(t),
-            dom: Z(r, i),
-            active: o => Ts(o, t)
+            command: X(t),
+            dom: G(r, i),
+            active: o => Ds(o, t)
         } : null;
         return [e(n.marks.strong, "format_bold", "bold"), e(n.marks.em, "format_italic", "italic"), e(n.marks.underline, "format_underline", "underline"), e(n.marks.strikethrough, "format_strikethrough", "strikethrough"), e(n.marks.sub, "subscript", "subscript"), e(n.marks.sup, "superscript", "superscript")].filter(Boolean)
     }
 
     function Is(n) {
         return n.marks.link ? [{
             command: st,
-            dom: Z("insert_link", "insert link"),
+            dom: G("insert_link", "insert link"),
             active: st
         }, {
-            command: ks,
-            dom: Z("link_off", "remove link"),
-            active: e => Ts(e, n.marks.link)
+            command: xs,
+            dom: G("link_off", "remove link"),
+            active: e => Ds(e, n.marks.link)
         }] : []
     }
 
-    function Rs() {
+    function vs() {
         return [{
             command: At,
-            dom: Z("undo", "undo"),
+            dom: G("undo", "undo"),
             active(n) {
                 return !1
             }
         }, {
             command: rt,
-            dom: Z("redo", "redo"),
+            dom: G("redo", "redo"),
             active(n) {
                 return !1
             }
         }]
     }
 
-    function vs() {
+    function Rs() {
         return [{
-            command: xs,
-            dom: Z("code", "edit HTML"),
+            command: ks,
+            dom: G("code", "edit HTML"),
             active: () => !1
         }]
     }
     var Br = class {
-        constructor(e, t) {
-            this.items = e.flatMap(r => r), this.editorView = t, this.dom = Q("div", {
-                className: "prose-menubar"
-            }), e.filter(r => r.length).forEach(r => {
-                let i = Q("div", {
+        constructor(e, t, r) {
+            if (this.items = [t, ...r].flatMap(i => i), this.editorView = e, this.dom = H("div", {
+                    className: "prose-menubar"
+                }), t.length) {
+                let i = H("div", {
+                        className: "prose-menubar__dropdown"
+                    }),
+                    o = H("div");
+                this.dom.append(i), i.append(G("notes", "paragraph")), i.append(o), t.forEach(({
+                    dom: s
+                }) => o.append(s))
+            }
+            r.filter(i => i.length).forEach(i => {
+                let o = H("div", {
                     className: "prose-menubar__group"
                 });
-                this.dom.append(i), r.forEach(({
-                    dom: o
-                }) => i.append(o))
-            }), this.update(), this.dom.addEventListener("mousedown", r => {
-                r.preventDefault(), t.focus(), this.items.forEach(({
-                    command: i,
-                    dom: o
+                this.dom.append(o), i.forEach(({
+                    dom: s
+                }) => o.append(s))
+            }), this.update(), this.dom.addEventListener("mousedown", i => {
+                i.preventDefault(), e.focus(), this.items.forEach(({
+                    command: o,
+                    dom: s
                 }) => {
-                    o.contains(r.target) && i(t.state, t.dispatch, t)
+                    s.contains(i.target) && o(e.state, e.dispatch, e)
                 })
             })
         }
         update() {
             this.items.forEach(({
                 command: e,
                 dom: t,
@@ -9763,15 +9772,15 @@
             let t = ["doc", "paragraph", "text", ...e],
                 r = {},
                 i = {};
             return n.spec.nodes.forEach((o, s) => {
                 t.includes(o) && (r[o] = s)
             }), n.spec.marks.forEach((o, s) => {
                 t.includes(o) && (i[o] = s)
-            }), new ke({
+            }), new xe({
                 nodes: r,
                 marks: i
             })
         };
 
     function zs(n, e) {
         let t = {
@@ -9822,22 +9831,22 @@
                         }],
                         toDOM() {
                             return $f
                         }
                     }
                 }
             },
-            r = new ke(t);
-        r = new ke({
+            r = new xe(t);
+        r = new xe({
             nodes: Qo(r.spec.nodes, "paragraph block*", "block"),
             marks: r.spec.marks
         }), r = Hf(r, e.types);
         let i = Cn(Cn({}, Os(r)), ws(r)),
-            o = [Yn(i), Yn(Pi), zi(), _o(), Xo(), Ns([Ds(r), Es(r), Is(r), As(r), e.history ? Rs() : null, e.html ? vs() : null].filter(Boolean)), Ps()],
-            s = Q("div", {
+            o = [Yn(i), Yn(Pi), zi(), _o(), Xo(), Ns(Ts(r), [Es(r), Is(r), As(r), e.history ? vs() : null, e.html ? Rs() : null].filter(Boolean)), Ps()],
+            s = H("div", {
                 className: "prose-editor"
             });
         n.before(s);
         let l = new un(s, {
                 state: Zt.create({
                     doc: Mn(r, n.value),
                     plugins: o
```

### Comparing `django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/material-icons.css` & `django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/material-icons.css`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.4/django_prose_editor/static/django_prose_editor/material-icons.woff2` & `django_prose_editor-0.4.0/django_prose_editor/static/django_prose_editor/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.4/LICENSE` & `django_prose_editor-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.4/README.rst` & `django_prose_editor-0.4.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -98,7 +98,38 @@
     text = SanitizedProseEditorField(
         config={"types": ["strong", "em", "sub", "sup"]},
     )
 
 Paragraphs cannot be removed at the moment. Note that the backend doesn't
 sanitize the content to ensure that the HTML doesn't contain only the provided
 tags, that's out of scope for now.
+
+
+Usage outside the Django admin
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The prose editor can easily be used outside the Django admin. The form field
+respectively the widget includes the necessary CSS and JavaScript:
+
+.. code-block:: python
+
+    from django_prose_editor.fields import ProseEditorFormField
+
+    class Form(forms.Form):
+        text = ProseEditorFormField()
+
+Or maybe you want to use ``django_prose_editor.widgets.ProseEditorWidget``, but
+why make it more complicated than necessary.
+
+If you're rendering the form in a template you have to include the form media:
+
+.. code-block:: html+django
+
+    <form method="post">
+      {{ form.errors }} {# Always makes sense #}
+      {{ form.media }}  {# This is the important line! #}
+      {{ form.as_div }}
+      <button type="submit">send</button>
+    </form>
+
+Note that the form media isn't django-prose-editor specific, that's a Django
+feature.
```

### Comparing `django_prose_editor-0.3.4/pyproject.toml` & `django_prose_editor-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.4/PKG-INFO` & `django_prose_editor-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prose-editor
-Version: 0.3.4
+Version: 0.4.0
 Summary: Prose editor for the Django admin based on ProseMirror
 Project-URL: Homepage, https://github.com/matthiask/django-prose-editor/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -127,7 +127,38 @@
     text = SanitizedProseEditorField(
         config={"types": ["strong", "em", "sub", "sup"]},
     )
 
 Paragraphs cannot be removed at the moment. Note that the backend doesn't
 sanitize the content to ensure that the HTML doesn't contain only the provided
 tags, that's out of scope for now.
+
+
+Usage outside the Django admin
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The prose editor can easily be used outside the Django admin. The form field
+respectively the widget includes the necessary CSS and JavaScript:
+
+.. code-block:: python
+
+    from django_prose_editor.fields import ProseEditorFormField
+
+    class Form(forms.Form):
+        text = ProseEditorFormField()
+
+Or maybe you want to use ``django_prose_editor.widgets.ProseEditorWidget``, but
+why make it more complicated than necessary.
+
+If you're rendering the form in a template you have to include the form media:
+
+.. code-block:: html+django
+
+    <form method="post">
+      {{ form.errors }} {# Always makes sense #}
+      {{ form.media }}  {# This is the important line! #}
+      {{ form.as_div }}
+      <button type="submit">send</button>
+    </form>
+
+Note that the form media isn't django-prose-editor specific, that's a Django
+feature.
```

