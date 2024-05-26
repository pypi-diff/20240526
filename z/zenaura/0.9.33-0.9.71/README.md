# Comparing `tmp/zenaura-0.9.33.tar.gz` & `tmp/zenaura-0.9.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenaura-0.9.33.tar", last modified: Wed May 15 21:54:24 2024, max compression
+gzip compressed data, was "zenaura-0.9.71.tar", last modified: Sun May 26 18:42:14 2024, max compression
```

## Comparing `zenaura-0.9.33.tar` & `zenaura-0.9.71.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 21:54:24.526305 zenaura-0.9.33/
--rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.33/LICENSE
--rw-rw-rw-   0        0        0     1557 2024-05-15 21:54:24.525305 zenaura-0.9.33/PKG-INFO
--rw-rw-rw-   0        0        0     1152 2024-05-13 18:21:23.000000 zenaura-0.9.33/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 21:54:24.526305 zenaura-0.9.33/setup.cfg
--rw-rw-rw-   0        0        0      709 2024-05-15 21:54:06.000000 zenaura-0.9.33/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 21:54:24.518805 zenaura-0.9.33/tests/
--rw-rw-rw-   0        0        0     7547 2024-05-15 17:30:31.000000 zenaura-0.9.33/tests/test_compiler.py
--rw-rw-rw-   0        0        0     4109 2024-05-13 16:55:02.000000 zenaura-0.9.33/tests/test_component_e2e.py
--rw-rw-rw-   0        0        0     1131 2024-05-11 17:44:57.000000 zenaura-0.9.33/tests/test_component_unit.py
--rw-rw-rw-   0        0        0     1435 2024-05-11 20:36:50.000000 zenaura-0.9.33/tests/test_observer.py
--rw-rw-rw-   0        0        0    15530 2024-05-14 16:04:33.000000 zenaura-0.9.33/tests/test_tags.py
--rw-rw-rw-   0        0        0    11805 2024-05-15 18:19:09.000000 zenaura-0.9.33/tests/test_zenaura_dom.py
-drwxrwxrwx   0        0        0        0 2024-05-15 21:54:24.519305 zenaura-0.9.33/zenaura/
--rw-rw-rw-   0        0        0        0 2024-05-11 11:31:00.000000 zenaura-0.9.33/zenaura/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 21:54:24.524804 zenaura-0.9.33/zenaura.egg-info/
--rw-rw-rw-   0        0        0     1557 2024-05-15 21:54:24.000000 zenaura-0.9.33/zenaura.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-05-15 21:54:24.000000 zenaura-0.9.33/zenaura.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 21:54:24.000000 zenaura-0.9.33/zenaura.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 21:54:24.000000 zenaura-0.9.33/zenaura.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-26 18:42:14.643483 zenaura-0.9.71/
+-rw-rw-rw-   0        0        0     1100 2024-05-11 11:29:30.000000 zenaura-0.9.71/LICENSE
+-rw-rw-rw-   0        0        0     2028 2024-05-26 18:42:14.642485 zenaura-0.9.71/PKG-INFO
+-rw-rw-rw-   0        0        0     1376 2024-05-26 16:54:28.000000 zenaura-0.9.71/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-26 18:42:14.643483 zenaura-0.9.71/setup.cfg
+-rw-rw-rw-   0        0        0      937 2024-05-26 18:42:04.000000 zenaura-0.9.71/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:42:14.637483 zenaura-0.9.71/tests/
+-rw-rw-rw-   0        0        0    33440 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_algorithm.py
+-rw-rw-rw-   0        0        0     6603 2024-05-26 18:05:15.000000 zenaura-0.9.71/tests/test_app.py
+-rw-rw-rw-   0        0        0     7595 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_compiler.py
+-rw-rw-rw-   0        0        0     4161 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_component_e2e.py
+-rw-rw-rw-   0        0        0     1415 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_component_unit.py
+-rw-rw-rw-   0        0        0     5301 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_node_properties.py
+-rw-rw-rw-   0        0        0     1435 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_observer.py
+-rw-rw-rw-   0        0        0     5710 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_rdom_adapter.py
+-rw-rw-rw-   0        0        0    15215 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_tags.py
+-rw-rw-rw-   0        0        0     3293 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_tasker.py
+-rw-rw-rw-   0        0        0     5456 2024-05-26 17:44:57.000000 zenaura-0.9.71/tests/test_zenaura_dom.py
+drwxrwxrwx   0        0        0        0 2024-05-26 18:42:14.641982 zenaura-0.9.71/zenaura.egg-info/
+-rw-rw-rw-   0        0        0     2028 2024-05-26 18:42:14.000000 zenaura-0.9.71/zenaura.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2024-05-26 18:42:14.000000 zenaura-0.9.71/zenaura.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:42:14.000000 zenaura-0.9.71/zenaura.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-26 18:42:14.000000 zenaura-0.9.71/zenaura.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 18:42:14.000000 zenaura-0.9.71/zenaura.egg-info/top_level.txt
```

### Comparing `zenaura-0.9.33/LICENSE` & `zenaura-0.9.71/LICENSE`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.33/PKG-INFO` & `zenaura-0.9.71/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.33
-Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
+Version: 0.9.71
+Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleach
 
 # Zenaura 
 
 <img title="a title" alt="Alt text" src="./assets/logo.png" width="300" height="300" />
 
-Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
+Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 
 ## Quick Example : 
 
 ```Python
 	    
 ```
```

### Comparing `zenaura-0.9.33/tests/test_compiler.py` & `zenaura-0.9.71/tests/test_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from zenaura.client.tags import Node, Attribute
 from zenaura.client.compiler import Compiler
 
 
 compiler = Compiler() 
 
 class CompilerTests(unittest.TestCase):
-    def test_compile_simple_node(self):
+    def test_compile_simple_render(self):
         elm = Node("div")
         result = compiler.compile(elm)
         self.assertEqual(result, "<div></div>")
 
     def test_compile_with_attributes(self):
         elm = Node("p")
-        elm.children.append(Attribute("styles", "my-paragraph"))
-        elm.children.append(Attribute("id", "main-content"))
+        elm.append_child(Attribute("styles", "my-paragraph"))
+        elm.append_child(Attribute("id", "main-content"))
         result = compiler.compile(elm, zenaura_dom_mode=False)
         self.assertEqual(result, '<p class="my-paragraph" id="main-content"></p>')
 
     
     def test_compile_with_attributes(self):
         elm = Node("p")
         elm.attributes.append(Attribute("styles", "my-paragraph"))
@@ -43,17 +43,17 @@
         #  note here space is important <div id=....
         self.assertEqual(result, ' id="my-node" class="important"')
 
     def test_compile_with_children(self):
         div = Node("div")
         span = Node("span")
         span.children = [
-            "Hello"
+            Node(text="Hello")
         ]
-        div.children.append(span)
+        div.append_child(span)
         result = compiler.compile(div, zenaura_dom_mode=False)
         self.assertEqual(result, "<div><span>Hello</span></div>")
     
     def test_sanitize_html(self):
         input_html = '<script>alert("XSS attack")</script>'
         result = compiler.sanitize(input_html)
         self.assertEqual(result, '&lt;script&gt;alert(&quot;XSS attack&quot;)&lt;/script&gt;')
@@ -63,16 +63,16 @@
         attrs = [Attribute("styles", "my-button"), Attribute("id", "btn-1")]
         result = compiler.process_attributes(attrs)
         self.assertEqual(result, ' class="my-button" id="btn-1"')
 
     def test_compile_with_nested_elements(self):
         div = Node("div")
         span = Node("span")
-        span.children = ["Hello"]
-        div.children.append(span)
+        span.children = [Node(text="Hello")]
+        div.append_child(span)
         result = compiler.compile(div, zenaura_dom_mode=False)
         self.assertEqual(result, "<div><span>Hello</span></div>")
 
 
     def test_sanitize_empty_input(self):
         input_html = ''
         result = compiler.sanitize(input_html)
@@ -101,38 +101,38 @@
     def test_compile_with_very_nested_complex_structure_and_attributes(self):
         root = Node("div")
         child1 = Node("div")
         child2 = Node("div")
         grandchild1 = Node("span")
         grandchild2 = Node("a")
         grandchild2.attributes.append(Attribute("href", "https://example.com"))
-        grandchild2.children = ["Link"]
+        grandchild2.children = [Node(text="Link")]
         grandchild3 = Node("img")
         grandchild3.attributes.append(Attribute("src", "image.jpg"))
         grandchild3.attributes.append(Attribute("alt", "Image"))
-        grandchild1.children = ["Hello"]
+        grandchild1.children = [Node(text="Hello")]
         child1.children.extend([grandchild1, grandchild2, grandchild3])
         root.children.extend([child1, child2])
         result = compiler.compile(root, zenaura_dom_mode=False)
         expected_output = '<div><div><span>Hello</span><a href="https://example.com">Link</a><img src="image.jpg" alt="Image"></div><div></div></div>'
         self.assertEqual(result, expected_output)
 
 
     def test_compile_with_even_more_nested_structure(self):
         root = Node("div")
         child1 = Node("div")
         child2 = Node("div")
         grandchild1 = Node("span")
         grandchild2 = Node("a")
         grandchild2.attributes.append(Attribute("href", "https://example.com"))
-        grandchild2.children = ["Link"]
+        grandchild2.children = [Node(text="Link")]
         grandchild3 = Node("img")
         grandchild3.attributes.append(Attribute("src", "image.jpg"))
         grandchild3.attributes.append(Attribute("alt", "Image"))
-        grandchild1.children = ["Hello"]
+        grandchild1.children = [Node(text="Hello")]
         child1.children.extend([grandchild1, grandchild2, grandchild3])
         root.children.extend([child1, child2])
 
         greatGrandchild1 = Node("div")
         greatGrandchild2 = Node("div")
         greatGrandchild3 = Node("div")
         greatGrandchild1.children.extend([greatGrandchild2, greatGrandchild3])
@@ -156,24 +156,24 @@
                 attributes.append(Attribute(key, value))
             return attributes
 
         # Create 10 levels of nested divs, each with 10 children, and attributes
         for level in range(10):
             for i in range(10):
                 child = Node("div", attributes=generate_attributes(3))  # 3 attributes per child
-                parent.children.append(child)
+                parent.append_child(child)
             parent = child
     
         # Add some content to the leaf nodes
         for child in parent.children:
-            child.children.append("Some content")
+            child.append_child("Some content")
 
         # Benchmark compilation time
         start_time = time.time()  # Start timer
         result = compiler.compile(root, zenaura_dom_mode=True)
         end_time = time.time()  # End timer
         compilation_time = end_time - start_time
 
         # Assert the size of the generated HTML
-        self.assertGreater(0.001, compilation_time)
+        self.assertGreater(0.1, compilation_time)
         self.assertLess(sys.getsizeof(result), 30000)  # Adjust the threshold as needed
```

#### html2text {}

```diff
@@ -1,41 +1,41 @@
 import unittest import time import sys import random import string from
 zenaura.client.tags import Node, Attribute from zenaura.client.compiler import
 Compiler compiler = Compiler() class CompilerTests(unittest.TestCase): def
-test_compile_simple_node(self): elm = Node("div") result = compiler.compile
+test_compile_simple_render(self): elm = Node("div") result = compiler.compile
 (elm) self.assertEqual(result, "
-") def test_compile_with_attributes(self): elm = Node("p") elm.children.append
-(Attribute("styles", "my-paragraph")) elm.children.append(Attribute("id",
-"main-content")) result = compiler.compile(elm, zenaura_dom_mode=False)
+") def test_compile_with_attributes(self): elm = Node("p") elm.append_child
+(Attribute("styles", "my-paragraph")) elm.append_child(Attribute("id", "main-
+content")) result = compiler.compile(elm, zenaura_dom_mode=False)
 self.assertEqual(result, '
 ') def test_compile_with_attributes(self): elm = Node("p")
 elm.attributes.append(Attribute("styles", "my-paragraph"))
 elm.attributes.append(Attribute("id", "main-content")) result =
 compiler.compile(elm, zenaura_dom_mode=False) self.assertEqual(result, '
 ') def test_compile_with_attributes(self): elm = Node("p")
 elm.attributes.append(Attribute("styles", "my-paragraph"))
 elm.attributes.append(Attribute("id", "main-content")) result =
 compiler.compile(elm, zenaura_dom_mode=False) self.assertEqual(result, '
 ') def test_process_attributes(self): attrs = [Attribute("id", "my-node"),
 Attribute("styles", "important")] result = compiler.process_attributes(attrs) #
 note here space is important
 id="my-node" class="important"') def test_compile_with_children(self): div =
-Node("div") span = Node("span") span.children = [ "Hello" ] div.children.append
-(span) result = compiler.compile(div, zenaura_dom_mode=False) self.assertEqual
-(result, "
+Node("div") span = Node("span") span.children = [ Node(text="Hello") ]
+div.append_child(span) result = compiler.compile(div, zenaura_dom_mode=False)
+self.assertEqual(result, "
 Hello
 ") def test_sanitize_html(self): input_html = '
 ' result = compiler.sanitize(input_html) self.assertEqual(result,
 '<script>alert("XSS attack")</script>') def
 test_process_attributes_with_keywords(self): attrs = [Attribute("styles", "my-
 button"), Attribute("id", "btn-1")] result = compiler.process_attributes(attrs)
 self.assertEqual(result, ' class="my-button" id="btn-1"') def
 test_compile_with_nested_elements(self): div = Node("div") span = Node("span")
-span.children = ["Hello"] div.children.append(span) result = compiler.compile
-(div, zenaura_dom_mode=False) self.assertEqual(result, "
+span.children = [Node(text="Hello")] div.append_child(span) result =
+compiler.compile(div, zenaura_dom_mode=False) self.assertEqual(result, "
 Hello
 ") def test_sanitize_empty_input(self): input_html = '' result =
 compiler.sanitize(input_html) self.assertEqual(result, '') def
 test_sanitize_input_with_special_characters(self): input_html = '<>&"' result =
 compiler.sanitize(input_html) self.assertEqual(result, '<>&"') def
 test_compile_node_with_no_attributes_or_children(self): elm = Node("div")
 result = compiler.compile(elm, zenaura_dom_mode=False) self.assertEqual(result,
@@ -43,31 +43,31 @@
 ") def test_process_attributes_with_no_attrs(self): attrs = [] result =
 compiler.process_attributes(attrs) self.assertEqual(result, '') def
 test_compile_with_no_children(self): elm = Node("div") result =
 compiler.compile(elm, zenaura_dom_mode=False) self.assertEqual(result, "
 ") def test_compile_with_very_nested_complex_structure_and_attributes(self):
 root = Node("div") child1 = Node("div") child2 = Node("div") grandchild1 = Node
 ("span") grandchild2 = Node("a") grandchild2.attributes.append(Attribute
-("href", "https://example.com")) grandchild2.children = ["Link"] grandchild3 =
-Node("img") grandchild3.attributes.append(Attribute("src", "image.jpg"))
-grandchild3.attributes.append(Attribute("alt", "Image")) grandchild1.children =
-["Hello"] child1.children.extend([grandchild1, grandchild2, grandchild3])
-root.children.extend([child1, child2]) result = compiler.compile(root,
-zenaura_dom_mode=False) expected_output = '
+("href", "https://example.com")) grandchild2.children = [Node(text="Link")]
+grandchild3 = Node("img") grandchild3.attributes.append(Attribute("src",
+"image.jpg")) grandchild3.attributes.append(Attribute("alt", "Image"))
+grandchild1.children = [Node(text="Hello")] child1.children.extend(
+[grandchild1, grandchild2, grandchild3]) root.children.extend([child1, child2])
+result = compiler.compile(root, zenaura_dom_mode=False) expected_output = '
 Hello_L_i_n_k[Image]
 ' self.assertEqual(result, expected_output) def
 test_compile_with_even_more_nested_structure(self): root = Node("div") child1 =
 Node("div") child2 = Node("div") grandchild1 = Node("span") grandchild2 = Node
 ("a") grandchild2.attributes.append(Attribute("href", "https://example.com"))
-grandchild2.children = ["Link"] grandchild3 = Node("img")
+grandchild2.children = [Node(text="Link")] grandchild3 = Node("img")
 grandchild3.attributes.append(Attribute("src", "image.jpg"))
 grandchild3.attributes.append(Attribute("alt", "Image")) grandchild1.children =
-["Hello"] child1.children.extend([grandchild1, grandchild2, grandchild3])
-root.children.extend([child1, child2]) greatGrandchild1 = Node("div")
-greatGrandchild2 = Node("div") greatGrandchild3 = Node("div")
+[Node(text="Hello")] child1.children.extend([grandchild1, grandchild2,
+grandchild3]) root.children.extend([child1, child2]) greatGrandchild1 = Node
+("div") greatGrandchild2 = Node("div") greatGrandchild3 = Node("div")
 greatGrandchild1.children.extend([greatGrandchild2, greatGrandchild3])
 grandchild2.children.extend([greatGrandchild1]) result = compiler.compile(root,
 zenaura_dom_mode=False) expected_output = '
 Hello
 _L_i_n_k
 [Image]
 ' self.assertEqual(result, expected_output) def
@@ -76,14 +76,14 @@
 attributes def generate_attributes(num_attributes): attributes = [] for _ in
 range(num_attributes): key = ''.join(random.choices(string.ascii_lowercase,
 k=5)) # Random 5-letter key value = ''.join(random.choices(string.ascii_letters
 + string.digits, k=10)) # Random 10-char value attributes.append(Attribute(key,
 value)) return attributes # Create 10 levels of nested divs, each with 10
 children, and attributes for level in range(10): for i in range(10): child =
 Node("div", attributes=generate_attributes(3)) # 3 attributes per child
-parent.children.append(child) parent = child # Add some content to the leaf
-nodes for child in parent.children: child.children.append("Some content") #
-Benchmark compilation time start_time = time.time() # Start timer result =
+parent.append_child(child) parent = child # Add some content to the leaf nodes
+for child in parent.children: child.append_child("Some content") # Benchmark
+compilation time start_time = time.time() # Start timer result =
 compiler.compile(root, zenaura_dom_mode=True) end_time = time.time() # End
 timer compilation_time = end_time - start_time # Assert the size of the
-generated HTML self.assertGreater(0.001, compilation_time) self.assertLess
+generated HTML self.assertGreater(0.1, compilation_time) self.assertLess
 (sys.getsizeof(result), 30000) # Adjust the threshold as needed
```

### Comparing `zenaura-0.9.33/tests/test_component_e2e.py` & `zenaura-0.9.71/tests/test_component_e2e.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 		self.counterState = CounterState
 
 	def test_initial_state(self):
 		state = self.counter.get_state()
 		self.assertEqual(state.count, 0)  # Ensure initial count is 0
 	
 
-	def test_increment(self):
-		self.counter.increment()
+	async def test_increment(self):
+		await self.counter.increment()
 		state = self.counter.get_state()
 		self.assertEqual(state.count, 1)
 	
 
 	def test_create_button(self):
 		button = self.counter.create_button("test", self.counter.increment)
 
@@ -39,23 +39,23 @@
 		self.assertEqual(len(button.attributes), 2)
 		self.assertEqual(len(button.children), 1)
 
 		self.assertEqual(self.btnstyles.btn, button.attributes[1].value)
 		self.assertEqual(self.counter.increment, button.attributes[0].value)
 		self.assertEqual(button.children[0].name , "label")
 
-	def test_decrease(self):
-		self.counter.decrease()
+	async def test_decrease(self):
+		await self.counter.decrease()
 		state = self.counter.get_state()
 		self.assertEqual(state.count, -1)
 	
 
 
 	def test_node_structure(self):
-		rendered_node = self.counter.node()
+		rendered_node = self.counter.render()
 		# Check for top-level container and attributes 
 		self.assertEqual(rendered_node.name, 'div')
 		# Ensure h1 header is present
 		header = rendered_node.children[0]
 		self.assertEqual(header.name, 'h1')
 
 		# Check controls div
@@ -74,15 +74,15 @@
 			for i in node.children:
 				if isinstance(i, Node):
 					curr.append(i)
 
 
 	def test_node_method_constructs_component_with_header_and_buttons(self):
 
-		result = self.counter.node()
+		result = self.counter.render()
 
 		# Assert
 		self.assertEqual(result.name, "div")
 		self.assertEqual(len(result.children), 2)
 		self.assertEqual(result.children[0].name, "h1")
 		self.assertEqual(len(result.children[0].children), 1)
 		self.assertEqual(result.children[0].children[0].name, "text")
@@ -98,24 +98,24 @@
 		button = self.counter.create_button("", self.counter.increment)
 		self.assertEqual(len(button.attributes), 2)
 		self.assertEqual(len(button.children), 1)
 		self.assertEqual(self.btnstyles.btn, button.attributes[1].value)
 		self.assertEqual(self.counter.increment, button.attributes[0].value)
 		self.assertEqual(button.children[0].name, "label")
 
-	def test_increment_multiple_times(self):
+	async def test_increment_multiple_times(self):
 		# Increment the count multiple times
 		for _ in range(5):
-			self.counter.increment()
+			await self.counter.increment()
 		state = self.counter.get_state()
 		self.assertEqual(state.count, 5)
 
-	def test_decrease_multiple_times(self):
+	async def test_decrease_multiple_times(self):
 		# Decrease the count multiple times
 		for _ in range(3):
-			self.counter.decrease()
+			await self.counter.decrease()
 		state = self.counter.get_state()
 		self.assertEqual(state.count, -3)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `zenaura-0.9.33/tests/test_component_unit.py` & `zenaura-0.9.71/tests/test_component_unit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import unittest
 from .mocks.component_mocks import Counter, Counter2, componentWIthInitState
-
+from zenaura.client.persistance import registry
+import hashlib
 c = Counter()
 c2 = Counter2()
 initState = componentWIthInitState()
 
 
 class TestComponent(unittest.TestCase):
     def setUp(self) -> None:
@@ -28,14 +29,22 @@
         state1 = {"test" : "test1"}
         state2 = {"test" : "test2"}
         self.c.set_state(state1)
         self.c2.set_state(state2) 
         self.assertNotEqual(self.c.get_state(), self.c2.get_state())
 
     def test_unique_comp_ids(self):
-        self.assertNotEqual(self.c2.componentId, self.c.componentId)
+        self.assertNotEqual(self.c2.id, self.c.id)
+
+    def test_uuid_presistance(self):
+        count = self.c.count
+        uuid = self.c.id 
+        hash = hashlib.md5(f"{self.c.__class__.__name__}{count}".encode()).hexdigest()[:8]
+        self.assertEqual(uuid, hash)
+        
+
```

### Comparing `zenaura-0.9.33/tests/test_observer.py` & `zenaura-0.9.71/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `zenaura-0.9.33/tests/test_tags.py` & `zenaura-0.9.71/tests/test_tags.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,26 +8,26 @@
         attribute = Attribute(key="test", value="test")
         self.assertEqual(attribute.key, "test")
         self.assertTrue(isinstance(attribute, Attribute))
 
     def test_node_creation(self):
         child = Node(name="test")
         node = Node(name="div")
-        node.children.append(child)
+        node.append_child(child)
         node.attributes.append(Attribute(key="test", value="test"))
         self.assertEqual(child.name, "test")
         self.assertEqual(len(node.children), 1)
         self.assertEqual(len(node.attributes), 1)
         self.assertTrue(isinstance(node.children[0], Node ))
         self.assertTrue(isinstance(node.attributes[0], Attribute))
 
     def test_node_has_nodeId(self):
         child = Node(name="test")
         parent = Node(name="div")
-        parent.children.append(child)
+        parent.append_child(child)
         self.assertTrue(child.nodeId)
         self.assertTrue(parent.nodeId)
 
     def test_node_builder(self):
         node = Builder('div') \
             .with_attribute("test", "test") \
             .with_child(
@@ -79,21 +79,21 @@
 
     def test_node_to_html_with_nested_nodes(self):
         # Create a nested node structure
         node1 = Node("div")
         node1.attributes.append(Attribute("class", "container"))
 
         node2 = Node("h1")
-        node2.children.append("Welcome to our website")
+        node2.append_child("Welcome to our website")
 
         node3 = Node("p")
-        node3.children.append("This is a paragraph")
+        node3.append_child("This is a paragraph")
 
-        node1.children.append(node2)
-        node1.children.append(node3)
+        node1.append_child(node2)
+        node1.append_child(node3)
 
         # Convert the node to HTML
         expected_html = (
             "<div class=\"container\">"
             "<h1>Welcome to our website</h1>"
             "<p>This is a paragraph</p>"
             "</div>"
@@ -103,22 +103,22 @@
     def test_node_to_html_with_nested_nodes_and_attributes(self):
         # Create a nested node structure with attributes
         node1 = Node("div")
         node1.attributes.append(Attribute("class", "container"))
 
         node2 = Node("h1")
         node2.attributes.append(Attribute("id", "title"))
-        node2.children.append("Welcome to our website")
+        node2.append_child("Welcome to our website")
 
         node3 = Node("p")
         node3.attributes.append(Attribute("class", "description"))
-        node3.children.append("This is a paragraph")
+        node3.append_child("This is a paragraph")
 
-        node1.children.append(node2)
-        node1.children.append(node3)
+        node1.append_child(node2)
+        node1.append_child(node3)
 
         # Convert the node to HTML
         expected_html = (
             "<div class=\"container\">"
             "<h1 id=\"title\">Welcome to our website</h1>"
             "<p class=\"description\">This is a paragraph</p>"
             "</div>"
@@ -127,26 +127,26 @@
 
     def test_node_to_html_with_nested_nodes_and_mixed_content(self):
         # Create a nested node structure with mixed content
         node1 = Node("div")
         node1.attributes.append(Attribute("class", "container"))
 
         node2 = Node("h1")
-        node2.children.append("Welcome to our website")
+        node2.append_child("Welcome to our website")
 
         node3 = Node("p")
-        node3.children.append("This is a paragraph")
+        node3.append_child("This is a paragraph")
 
         node4 = Node("img")
         node4.attributes.append(Attribute("src", "image.jpg"))
         node4.attributes.append(Attribute("alt", "Image"))
 
-        node1.children.append(node2)
-        node1.children.append(node3)
-        node1.children.append(node4)
+        node1.append_child(node2)
+        node1.append_child(node3)
+        node1.append_child(node4)
 
         # Convert the node to HTML
         expected_html = (
             "<div class=\"container\">"
             "<h1>Welcome to our website</h1>"
             "<p>This is a paragraph</p>"
             "<img src=\"image.jpg\" alt=\"Image\">"
@@ -156,128 +156,61 @@
 
     def test_node_to_html_with_nested_nodes_and_empty_children(self):
         # Create a nested node structure with empty children
         node1 = Node("div")
         node1.attributes.append(Attribute("class", "container"))
 
         node2 = Node("h1")
-        node2.children.append("Welcome to our website")
+        node2.append_child("Welcome to our website")
 
         node3 = Node("p")
-        node3.children.append("")
+        node3.append_child("")
 
-        node1.children.append(node2)
-        node1.children.append(node3)
+        node1.append_child(node2)
+        node1.append_child(node3)
 
         # Convert the node to HTML
         expected_html = (
             "<div class=\"container\">"
             "<h1>Welcome to our website</h1>"
             "<p></p>"
             "</div>"
         )
         self.assertEqual(node1.to_html(), expected_html)
 
 
 
-    def test_to_dict_with_children(self):
-        
-        child1 = Node("child1")
-        child2 = Node("child2")
-        node = Node("parent", children=[child1, child2])
-
-        
-        result = node.to_dict()
-        self.assertDictEqual(
-            result , 
-            {
-            "name": "parent",
-            "children": [
-                {
-                "name": "child1",
-                "children": []
-                },
-                {
-                "name": "child2",
-                "children": []
-                }
-            ]
-            }
-        )
        
         
     def test_to_dict_without_children(self):
         
         node = Node("parent")
 
         
         result = node.to_dict()
 
-
-        self.assertDictEqual(
-            result, {"name": "parent", "children": []}
-        )
-    def test_to_dict_with_children(self):
         
-        child1 = Node("child1")
-        node = Node("parent", children=[child1])
-
-        
-        result = node.to_dict()
-
 
         self.assertDictEqual(
-            result,
-            {
-            "name": "parent",
-            "children": [
-                {
-                "name": "child1",
-                "children": []
-                }
-            ]
-            }
+            result, {'name': 'parent', 'parent': 'none', 'level': 0, 'key': 0, 'path': '', 'children': []}
         )
         
     def test_to_dict_with_nested_children(self):
         
         child1 = Node("child1", children=[Node("grandchild1"), Node("grandchild2")])
         child2 = Node("child2")
         node = Node("parent", children=[child1, child2])
 
         
         result = node.to_dict()
-
-
+        
         self.assertDictEqual(
             result,
-            {
-                "name": "parent",
-                "children": [
-                    {
-                    "name": "child1",
-                    "children": [
-                        {
-                        "name": "grandchild1",
-                        "children": [],
-                        },
-                        {
-                        "name": "grandchild2",
-                        "children": [],
-                        }
-                    ]
-                    },
-                    {
-                    "name": "child2",
-                    "children": [],
-                    }
-                ]
-            }
+{'name': 'parent', 'parent': 'none', 'level': 0, 'key': 0, 'path': '', 'children': [{'name': 'child1', 'parent': 'child1', 'level': 1, 'key': 0, 'path': '00', 'children': [{'name': 'grandchild1', 'parent': 'grandchild1', 'level': 2, 'key': 0, 'path': '0010', 'children': []}, {'name': 'grandchild2', 'parent': 'grandchild2', 'level': 2, 'key': 1, 'path': '0011', 'children': []}]}, {'name': 'child2', 'parent': 'child2', 'level': 1, 'key': 1, 'path': '01', 'children': []}]}
         )
-
     def test_getAttributes(self):
 
         node = Node("div")
         node.attributes.append(Attribute("class", "container"))
         node.attributes.append(Attribute("id", "title"))
         node.attributes.append(Attribute("style", "color:blue;font-size:16px"))
 
@@ -285,173 +218,173 @@
 
         expected = " class=\"container\" id=\"title\" style=\"color:blue;font-size:16px\""
         self.assertEqual(attributes, expected)
 
 
     def test_findChildByName_found(self):
         node = Node("div")
-        node.children.append(Node("h1"))
+        node.append_child(Node("h1"))
 
         child = node.findChildByName("h1")
         self.assertEqual(child.name, "h1")
 
     def test_findChildByName_not_found(self):
         node = Node("div")
 
         child = node.findChildByName("h1")
         self.assertFalse(child)
 
     def test_findAllByName_found(self):
         node = Node("div")
-        node.children.append(Node("h1"))
-        node.children.append(Node("h1"))
-        node.children.append(Node("p"))
+        node.append_child(Node("h1"))
+        node.append_child(Node("h1"))
+        node.append_child(Node("p"))
 
         children = node.findAllByName("h1")
         self.assertEqual(len(children), 2)
 
     def test_findAllByName_not_found(self):
         node = Node("div")
-        node.children.append(Node("h1"))
-        node.children.append(Node("p"))
+        node.append_child(Node("h1"))
+        node.append_child(Node("p"))
 
         children = node.findAllByName("h2")
         self.assertEqual(len(children), 0)
 
     def test_findByAttribute_found(self):
         node = Node("div")
         child = Node("h1")
         child.attributes.append(Attribute("class", "container"))
-        node.children.append(child)
+        node.append_child(child)
 
         child = node.findByAttribute("class", "container")
         self.assertEqual(child.name, "h1")
 
     def test_findByAttribute_not_found(self):
         node = Node("div")
 
         child = node.findByAttribute("class", "container")
         self.assertFalse(child)
 
     def test_findAllChildrenByAttributeKey_found(self):
         node = Node("div")
-        node.children.append(Node("h1", attributes=[Attribute("class", "container")]))
-        node.children.append(Node("h1", attributes=[Attribute("class", "container")]))
-        node.children.append(Node("p"))
+        node.append_child(Node("h1", attributes=[Attribute("class", "container")]))
+        node.append_child(Node("h1", attributes=[Attribute("class", "container")]))
+        node.append_child(Node("p"))
 
         children = node.findAllChildrenByAttributeKey("class")
         self.assertEqual(len(children), 2)
 
     def test_findAllChildrenByAttributeKey_not_found(self):
         node = Node("div")
-        node.children.append(Node("p"))
+        node.append_child(Node("p"))
 
         children = node.findAllChildrenByAttributeKey("class")
         self.assertFalse(children)
 
     def test_findAllChildrenByAttributeValue_found(self):
         node = Node("div")
-        node.children.append(Node("h1", attributes=[Attribute("class", "container")]))
-        node.children.append(Node("h1", attributes=[Attribute("class", "container")]))
-        node.children.append(Node("p"))
+        node.append_child(Node("h1", attributes=[Attribute("class", "container")]))
+        node.append_child(Node("h1", attributes=[Attribute("class", "container")]))
+        node.append_child(Node("p"))
 
         children = node.findAllChildrenByAttributeValue("container")
         self.assertEqual(len(children), 2)
 
 
     def test_findAllChildrenByAttributeValue_not_found(self):
         node = Node("div")
 
         children = node.findAllChildrenByAttributeValue("container")
         self.assertFalse(children)
 
     def test_replace_children_found(self):
         node = Node("div")
         spe = Node("h1")
-        node.children.append(Node("h2"))
-        node.children.append(spe)
-        node.children.append(Node("p"))
+        node.append_child(Node("h2"))
+        node.append_child(spe)
+        node.append_child(Node("p"))
 
         node.replace(spe, Node("h2"))
         self.assertEqual(len(node.children), 3)
         self.assertEqual(node.children[0].name, "h2")
         self.assertEqual(node.children[1].name, "h2")
         self.assertEqual(node.children[2].name, "p")
 
     def test_replace_children_not_found(self):
         node = Node("div")
         spe = Node("h1")
-        node.children.append(Node("h2"))
-        node.children.append(Node("h1"))
-        node.children.append(Node("p"))
+        node.append_child(Node("h2"))
+        node.append_child(Node("h1"))
+        node.append_child(Node("p"))
 
         node.replace(spe, spe)
         self.assertEqual(len(node.children), 3)
         self.assertEqual(node.children[0].name, "h2")
         self.assertEqual(node.children[1].name, "h1")
         self.assertEqual(node.children[2].name, "p")
 
     def test_getChildIndex_found(self):
         node = Node("div")
         k = Node("h1")
-        node.children.append(k)
-        node.children.append(Node("h2"))
-        node.children.append(Node("p"))
+        node.append_child(k)
+        node.append_child(Node("h2"))
+        node.append_child(Node("p"))
 
         index = node.getChildIndex(k)
         self.assertEqual(index, 0)
 
     def test_insertAfter(self):
         node = Node("div")
         h2 = Node("h2")
-        node.children.append(Node("h1"))
-        node.children.append(h2)
-        node.children.append(Node("p"))
+        node.append_child(Node("h1"))
+        node.append_child(h2)
+        node.append_child(Node("p"))
 
         node.insertAfter(h2, Node("h3"))
         self.assertEqual(len(node.children), 4)
         self.assertEqual(node.children[0].name, "h1")
         self.assertEqual(node.children[1].name, "h2")
         self.assertEqual(node.children[2].name, "h3")
         self.assertEqual(node.children[3].name, "p")
 
     def test_insertBefore(self):
         node = Node("div")
         h2 = Node("h2")
-        node.children.append(Node("h1"))
-        node.children.append(h2)
-        node.children.append(Node("p"))
+        node.append_child(Node("h1"))
+        node.append_child(h2)
+        node.append_child(Node("p"))
 
         node.insertBefore(h2, Node("h3"))
         self.assertEqual(len(node.children), 4)
         self.assertEqual(node.children[0].name, "h1")
         self.assertEqual(node.children[1].name, "h3")
         self.assertEqual(node.children[2].name, "h2")
         self.assertEqual(node.children[3].name, "p")
 
 
     def test_remove(self):
         node = Node("div")
         h2 = Node("h2")
-        node.children.append(Node("h1"))
-        node.children.append(h2)
-        node.children.append(Node("p"))
+        node.append_child(Node("h1"))
+        node.append_child(h2)
+        node.append_child(Node("p"))
 
         node.remove(h2)
         self.assertEqual(len(node.children), 2)
         self.assertEqual(node.children[0].name, "h1")
         self.assertEqual(node.children[1].name, "p")
 
     def test_appendAttributeToChild(self):
 
         node = Node("div")
         h2 = Node("h2")
-        node.children.append(Node("h1"))
-        node.children.append(h2)
-        node.children.append(Node("p"))
+        node.append_child(Node("h1"))
+        node.append_child(h2)
+        node.append_child(Node("p"))
 
         h2.attributes.append(Attribute("class", "container"))
         h2.attributes.append(Attribute("id", "title"))
         h2.attributes.append(Attribute("style", "color:blue;font-size:16px"))
 
         node.appendAttributeToChild(h2, Attribute("class", "container2"))
 
@@ -460,8 +393,34 @@
         self.assertEqual(h2.attributes[0].value, "container")
         self.assertEqual(h2.attributes[1].key, "id")
         self.assertEqual(h2.attributes[1].value, "title")
         self.assertEqual(h2.attributes[2].key, "style")
         self.assertEqual(h2.attributes[2].value, "color:blue;font-size:16px")
         self.assertEqual(h2.attributes[3].key, "class")
         self.assertEqual(h2.attributes[3].value, "container2")
-        
+        
+
+    def test_with_attributes_with_children(self):
+        # Create a builder object with tag 'div'
+        node = Builder('div') \
+            .with_attribute("test", "test") \
+            .with_children(
+                Node(name="test_child1"),
+                Node(name="test_child2")
+            ) \
+            .with_attributes(
+                attr1="value1",
+                attr2="value2"
+            ).build()
+
+        # Assert attributes
+        self.assertEqual(node.attributes[0].key, "test")
+        self.assertEqual(node.attributes[0].value, "test")
+        self.assertEqual(node.attributes[1].key, "attr1")
+        self.assertEqual(node.attributes[1].value, "value1")
+        self.assertEqual(node.attributes[2].key, "attr2")
+        self.assertEqual(node.attributes[2].value, "value2")
+
+        # Assert children
+        self.assertEqual(len(node.children), 2)
+        self.assertEqual(node.children[0].name, "test_child1")
+        self.assertEqual(node.children[1].name, "test_child2")
```

### Comparing `zenaura-0.9.33/zenaura.egg-info/PKG-INFO` & `zenaura-0.9.71/zenaura.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: zenaura
-Version: 0.9.33
-Summary: Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
+Version: 0.9.71
+Summary: Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 Author: Ahmed Rakan
 Author-email: ar.aldhafeeri11@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: bleach
 
 # Zenaura 
 
 <img title="a title" alt="Alt text" src="./assets/logo.png" width="300" height="300" />
 
-Zenaura, light weight, super fast python full-stack development framework, in which every line of code emit the aura of python zen, build interactive SPA with pure Python, create secure and scalable endpoints.
+Zenaura is an experimental Python library built upon PyScript, designed to empower Python developers to create stateful, component-based Single Page Applications (SPAs). By leveraging a virtual DOM implementation, Zenaura optimizes the performance, reactivity, responsiveness, and interactivity of web applications. This allows developers to build high-performance, dynamic web applications using familiar Python concepts and syntax.
 
 ## Quick Example : 
 
 ```Python
 	    
 ```
```

