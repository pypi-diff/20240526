# Comparing `tmp/ADViewpy-0.6a0.tar.gz` & `tmp/ADViewpy-0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ADViewpy-0.6a0.tar", last modified: Fri May 24 05:51:58 2024, max compression
+gzip compressed data, was "ADViewpy-0.7a0.tar", last modified: Sun May 26 16:27:45 2024, max compression
```

## Comparing `ADViewpy-0.6a0.tar` & `ADViewpy-0.7a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 05:51:58.302763 ADViewpy-0.6a0/
-drwxrwxrwx   0        0        0        0 2024-05-24 05:51:58.294997 ADViewpy-0.6a0/ADViewpy/
--rw-rw-rw-   0        0        0    46666 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/ADViewpy.py
--rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.6a0/ADViewpy/__init__.py
--rw-rw-rw-   0        0        0    19348 2024-05-24 05:51:48.000000 ADViewpy-0.6a0/ADViewpy/myCanvas.py
--rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.6a0/ADViewpy/myUtils.py
--rw-rw-rw-   0        0        0    56104 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/pairwiseCanvas.py
--rw-rw-rw-   0        0        0    23713 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/rtCanvas.py
--rw-rw-rw-   0        0        0    65738 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/tcCanvas.py
--rw-rw-rw-   0        0        0    22310 2024-05-24 05:51:49.000000 ADViewpy-0.6a0/ADViewpy/treeDistributionView.py
-drwxrwxrwx   0        0        0        0 2024-05-24 05:51:58.301764 ADViewpy-0.6a0/ADViewpy.egg-info/
--rw-rw-rw-   0        0        0     6202 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-24 05:51:58.000000 ADViewpy-0.6a0/ADViewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6202 2024-05-24 05:51:58.303763 ADViewpy-0.6a0/PKG-INFO
--rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.6a0/README.md
--rw-rw-rw-   0        0        0      554 2024-05-24 05:51:48.000000 ADViewpy-0.6a0/pyproject.toml
--rw-rw-rw-   0        0        0       94 2024-05-24 05:51:58.303763 ADViewpy-0.6a0/setup.cfg
--rw-rw-rw-   0        0        0      904 2024-05-24 05:51:48.000000 ADViewpy-0.6a0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:27:45.216021 ADViewpy-0.7a0/
+drwxrwxrwx   0        0        0        0 2024-05-26 16:27:45.207617 ADViewpy-0.7a0/ADViewpy/
+-rw-rw-rw-   0        0        0    46666 2024-05-26 16:27:39.000000 ADViewpy-0.7a0/ADViewpy/ADViewpy.py
+-rw-rw-rw-   0        0        0      190 2024-05-04 05:39:18.000000 ADViewpy-0.7a0/ADViewpy/__init__.py
+-rw-rw-rw-   0        0        0    19348 2024-05-26 16:27:40.000000 ADViewpy-0.7a0/ADViewpy/myCanvas.py
+-rw-rw-rw-   0        0        0     3062 2024-05-21 03:27:21.000000 ADViewpy-0.7a0/ADViewpy/myUtils.py
+-rw-rw-rw-   0        0        0    56104 2024-05-26 16:27:39.000000 ADViewpy-0.7a0/ADViewpy/pairwiseCanvas.py
+-rw-rw-rw-   0        0        0    23715 2024-05-26 16:27:40.000000 ADViewpy-0.7a0/ADViewpy/rtCanvas.py
+-rw-rw-rw-   0        0        0    65815 2024-05-26 16:27:39.000000 ADViewpy-0.7a0/ADViewpy/tcCanvas.py
+-rw-rw-rw-   0        0        0    22310 2024-05-26 16:27:39.000000 ADViewpy-0.7a0/ADViewpy/treeDistributionView.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:27:45.215014 ADViewpy-0.7a0/ADViewpy.egg-info/
+-rw-rw-rw-   0        0        0     6202 2024-05-26 16:27:44.000000 ADViewpy-0.7a0/ADViewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-05-26 16:27:45.000000 ADViewpy-0.7a0/ADViewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:27:44.000000 ADViewpy-0.7a0/ADViewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-26 16:27:44.000000 ADViewpy-0.7a0/ADViewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-26 16:27:44.000000 ADViewpy-0.7a0/ADViewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6202 2024-05-26 16:27:45.216021 ADViewpy-0.7a0/PKG-INFO
+-rw-rw-rw-   0        0        0     5716 2024-05-21 03:16:52.000000 ADViewpy-0.7a0/README.md
+-rw-rw-rw-   0        0        0      554 2024-05-26 16:26:44.000000 ADViewpy-0.7a0/pyproject.toml
+-rw-rw-rw-   0        0        0       94 2024-05-26 16:27:45.217044 ADViewpy-0.7a0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2024-05-26 16:26:44.000000 ADViewpy-0.7a0/setup.py
```

### Comparing `ADViewpy-0.6a0/ADViewpy/ADViewpy.py` & `ADViewpy-0.7a0/ADViewpy/ADViewpy.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.6a0/ADViewpy/myCanvas.py` & `ADViewpy-0.7a0/ADViewpy/myCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.6a0/ADViewpy/myUtils.py` & `ADViewpy-0.7a0/ADViewpy/myUtils.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.6a0/ADViewpy/pairwiseCanvas.py` & `ADViewpy-0.7a0/ADViewpy/pairwiseCanvas.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.6a0/ADViewpy/rtCanvas.py` & `ADViewpy-0.7a0/ADViewpy/rtCanvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,29 +183,29 @@
 
                 if node.block.botR.y > node.parent_node.block.botR.y:
                     node.parent_node.block.botR = node.block.botR
             else:
                 node.parent_node.block = Block(node.block.topL,node.block.botR)
 
         if not node.is_leaf() and self.check_attribute_in_range(node):
-            self.draw_rec(node.pos.x, node.pos.y - RT_X_INTERVAL,RT_X_INTERVAL-2,RT_X_INTERVAL - 2, BEIGE,
+            self.draw_rec(node.pos.x, node.pos.y - RT_X_INTERVAL,RT_X_INTERVAL-2,RT_X_INTERVAL - 2, ORANGE,
                           layer_index=self.FILTER_NODE_LAYER)
 
 
         node.selected = False
         self.insert_node_section_list(node)
 
     def draw_filter_node(self,exact_match_range,support_value_range):
         self.support_value_interval = support_value_range
         self.exact_match_interval = exact_match_range
 
         self[self.FILTER_NODE_LAYER].clear()
         for node in self.rt.postorder_node_iter():
             if not node.is_leaf() and self.check_attribute_in_range(node):
-                self.draw_rec(node.pos.x, node.pos.y - RT_X_INTERVAL, RT_X_INTERVAL - 2, RT_X_INTERVAL - 2, BEIGE,
+                self.draw_rec(node.pos.x, node.pos.y - RT_X_INTERVAL, RT_X_INTERVAL - 2, RT_X_INTERVAL - 2, ORANGE,
                               layer_index=self.FILTER_NODE_LAYER)
 
     def check_attribute_in_range(self,node):
         exact_match_result = False
         support_value_result = False
 
         if self.support_value_interval:
```

### Comparing `ADViewpy-0.6a0/ADViewpy/tcCanvas.py` & `ADViewpy-0.7a0/ADViewpy/tcCanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -544,24 +544,25 @@
                     if first_subtree.root.corr[tree_index] == subtree.root.corr[tree_index]:
                         return True
 
     # Function to check whether current branch/node related with target subtree/taxa
     def check_relation(self,subtree,node,tree_index,nested_subtree_duplicate):
         # If node is subtree's root
         if node == subtree.root.corr[tree_index]:
-            result = self.check_subtree_combine(node,tree_index=tree_index)
-            if not self.subtree_independent and result == DUPLICATE_SUBTREE_ROOT:
-                return DUPLICATE_SUBTREE_ROOT
-            else:
-                return SUBTREE_ROOT
+            if not self.subtree_independent:
+                result = self.check_subtree_combine(node,tree_index=tree_index)
+                if result == DUPLICATE_SUBTREE_ROOT:
+                    return DUPLICATE_SUBTREE_ROOT
+
+            return SUBTREE_ROOT
 
         # If node from tc is target leaf node in this subtree
         if node.is_leaf():
             if node.taxon.label in subtree.leaf_set:
-                if not self.escape_taxa_as_context_block:
+                if not self.escape_taxa_as_context_block or self.subtree_independent:
                     return INDEPENDENT_LEAF
 
         if self.check_leaf_node_descendant(subtree,node) == IS_DESCENDANT:
             if self.escape_taxa_as_context_block:
                 if nested_subtree_duplicate or self.check_subtree_in_descendant(node,tree_index=tree_index):
                     return IS_DESCENDANT
             else:
@@ -743,23 +744,24 @@
         for index,subtree_block in enumerate(subtree_block_list):
             if subtree_block.nested_tree:
                 subtree_block.nested_tree.height = self.adjust_ad_block(subtree_block.nested_tree)
                 subtree_block.height = subtree_block.nested_tree.height
                 # print(f"{subtree_block.belong_subtree.label} height = "+str(subtree_block.height))
                 space_required += subtree_block.height + ad_tree.padding * self.scale
 
-                if index == len(subtree_block_list)-1:
+                if index == len(subtree_block_list) - 1:
                     if ad_tree.is_nested:
                         space_required += ad_tree.padding * self.scale
                     else:
                         free_space = ad_tree.height - space_required
                         subtree_block.height += free_space
-                        subtree_block.nested_tree.height = subtree_block.height
 
-                        self.allocate_remaining_space(subtree_block.nested_tree)
+                        if subtree_block.nested_tree:
+                            subtree_block.nested_tree.height = subtree_block.height
+                            self.allocate_remaining_space(subtree_block.nested_tree)
 
             elif ad_tree.is_nested:
                 subtree_block.height = self.nested_block_height
                 space_required += subtree_block.height + ad_tree.padding * self.scale
 
 
             else:
@@ -791,16 +793,18 @@
 
         if ad_tree.is_nested:
             return space_required
 
         return self.ad_height - space_required
 
     def allocate_remaining_space(self,ad_tree):
+        indv_block_list, subtree_block_list, taxa_total = ad_tree.individual_subtree_block_list()
+        if len(subtree_block_list) == 0:
+            return
 
-        indv_block_list, subtree_block_list,taxa_total = ad_tree.individual_subtree_block_list()
         block = subtree_block_list[-1]
         if ad_tree.is_nested and block.nested_tree:
             free_space = ad_tree.height - ad_tree.space_required
             block.height += free_space
 
             if block.nested_tree:
                 self.allocate_remaining_space(block.nested_tree)
@@ -831,15 +835,22 @@
             width = ad_tree.botR.x - ad_tree.x * self.scale - x
             ad_tree.missing_taxa_block = Block(Point(x,y),Point(x+width,y+self.missing_taxa_height))
 
             self.draw_missing_taxa_block(ad_tree)
 
     def draw_ad_tree(self,ad_tree=None,canvas=None,cluster=False):
         with hold_canvas(self):
-            ad_tree.y = 8 * self.scale
+            scale_tmp = self.scale
+
+            if self.scale > 1.0:
+                scale_tmp = 1.0
+            elif self.scale < 0.6:
+                scale_tmp = 0.6
+
+            ad_tree.y = 8 * scale_tmp
             for node in ad_tree.traverse_postorder():
                 if canvas and not ad_tree.is_nested:
                     if cluster:
                         ad_topL_x = 5
                         ad_topL_y = CLUSTER_NUMBER_BAR_HEIGHT + DEFAULT_PADDING_BETWEEN_BLOCK * 2 + 5
 
                         ad_tree.topL.x = ad_topL_x
@@ -856,29 +867,20 @@
                     ad_topL_y = ad_tree.topL.y
                     ad_botR_x = ad_tree.botR.x
                     ad_botR_y = ad_tree.botR.y
 
                 if node.type == LEAF:
                     block = node.node_or_block
 
-                    scale_tmp = self.scale
-
-                    if self.scale > 1.0:
-                        scale_tmp = 1.0
-                    elif self.scale < 0.6:
-                        scale_tmp = 0.6
-
-                    # scale_tmp = 0.7 if self.scale < 0.7 else self.scale
-
-                    x = ad_topL_x + (ad_tree.x * scale_tmp) + (
+                    x = ad_topL_x + (ad_tree.x * self.scale) + (
                             ad_tree.x * node.x_level * scale_tmp)  # ad_pos + padding
 
                     # Calculate block position
                     if ad_tree.is_nested:
-                        y = ad_topL_y + ad_tree.y + (12 * self.scale)
+                        y = ad_topL_y + ad_tree.y + (10 * self.scale)
                     else:
                         y = ad_topL_y + ad_tree.y
 
                     block.topL = Point(x, y)
 
                     block.botR = Point(ad_botR_x - ad_tree.x * self.scale, y + block.height)
 
@@ -1023,23 +1025,22 @@
 
             if height == 0:
                 height = self.get_color_segment_height(block.height,block.duplicate_subtree_taxa_count[i],block.subtree_taxa_count)
             else:
                 height = block.height - height
 
 
-            if block.exact_match[i]:
+            if block.exact_match[i] or not self.show_block_proportional:
                 self.draw_rec(x, y, block.width, height,
                               color=block.color[i],
                               layer_index=block.belong_ad_tree.located_layer,canvas=canvas)
                 self.draw_rec_edge_absent(side=side,exact_match=True,x=x,y=y,width=block.width,height=height,
                                           layer_index=block.belong_ad_tree.located_layer,canvas=canvas)
             else:
                 subtree_leaf = len(block.belong_subtree[i].leaf_set)
-
                 width = self.get_color_segment_width(block.width,block.duplicate_subtree_taxa_count[i],
                                                      len(block.taxa_list))
                 self.draw_rec(x, y, width, height,
                               color=block.color[i],
                               layer_index=block.belong_ad_tree.located_layer,canvas=canvas)
                 self.draw_rec_edge_absent(side=side,exact_match=False,x=x,y=y,width=block.width,height=height,layer_index=block.belong_ad_tree.located_layer,canvas=canvas)
```

### Comparing `ADViewpy-0.6a0/ADViewpy/treeDistributionView.py` & `ADViewpy-0.7a0/ADViewpy/treeDistributionView.py`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.6a0/ADViewpy.egg-info/PKG-INFO` & `ADViewpy-0.7a0/ADViewpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.6a0
+Version: 0.7a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.6a0/PKG-INFO` & `ADViewpy-0.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADViewpy
-Version: 0.6a0
+Version: 0.7a0
 Summary: ADViewpy is Python Library to visually compare phylogenetic trees
 Author: Ng Weng Shan
 Author-email: ngwengshan025@hotmail.com
 Project-URL: Homepage, https://github.com/Coralnws/ADViewpy-alpha.git
 Keywords: python,phylogenetic tree,aggregrated dendrogram,tree comparison
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `ADViewpy-0.6a0/README.md` & `ADViewpy-0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `ADViewpy-0.6a0/pyproject.toml` & `ADViewpy-0.7a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ADViewpy"
-version = '0.6.alpha'
+version = '0.7.alpha'
 description = "ADViewpy is Python Library to visually compare phylogenetic trees"
 readme = "README.md"
 #dependencies=[
 #        'dendropy',
 #        'ipycanvas',
 #        'ipywidgets',
 #        'scikit-learn',
```

### Comparing `ADViewpy-0.6a0/setup.py` & `ADViewpy-0.7a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import codecs
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.6.alpha'
+VERSION = '0.7.alpha'
 DESCRIPTION = ('ADViewpy is Python Library to visually compare phylogenetic trees')
 LONG_DESCRIPTION = 'ADViewpy is Python Library to visually compare phylogenetic trees, utilizing Aggregated Dendrogram for phylogenetic tree visualization. '
 
 
 setup(
     name="ADViewpy",
     version=VERSION,
```

