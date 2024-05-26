# Comparing `tmp/tablinum-0.1.3.tar.gz` & `tmp/tablinum-0.1.4.tar.gz`

## Comparing `tablinum-0.1.3.tar` & `tablinum-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 tablinum-0.1.3/t
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/__about__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/__init__.py
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tab_fun_dates.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tab_fun_maths.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tab_fun_useful.py
--rw-r--r--   0        0        0    59527 2020-02-02 00:00:00.000000 tablinum-0.1.3/src/tablinum/tablinum.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test-input.txt
--rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_calculation.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_command_line.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_contingency.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_filter.py
--rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_grouping.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_help.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_levels.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_makers.py
--rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_parsing.py
--rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_poppers_and_adders.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_roller.py
--rw-r--r--   0        0        0     9684 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_sort.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_text_manip.py
--rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tab_wrangler.py
--rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 tablinum-0.1.3/tests/test_tablinum.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tablinum-0.1.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tablinum-0.1.3/LICENSE
--rw-r--r--   0        0        0    60858 2020-02-02 00:00:00.000000 tablinum-0.1.3/README.md
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 tablinum-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    61853 2020-02-02 00:00:00.000000 tablinum-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tablinum-0.1.4/setup.cfg
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 tablinum-0.1.4/src/tablinum/__about__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tablinum-0.1.4/src/tablinum/__init__.py
+-rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 tablinum-0.1.4/src/tablinum/tab_fun_dates.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 tablinum-0.1.4/src/tablinum/tab_fun_maths.py
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tablinum-0.1.4/src/tablinum/tab_fun_useful.py
+-rw-r--r--   0        0        0    60313 2020-02-02 00:00:00.000000 tablinum-0.1.4/src/tablinum/tablinum.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test-input.txt
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_calculation.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_command_line.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_contingency.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_filter.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_grouping.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_help.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_levels.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_makers.py
+-rw-r--r--   0        0        0     9002 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_parsing.py
+-rw-r--r--   0        0        0     9593 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_poppers_and_adders.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_roller.py
+-rw-r--r--   0        0        0     9896 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_sort.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_text_manip.py
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tab_wrangler.py
+-rw-r--r--   0        0        0    14125 2020-02-02 00:00:00.000000 tablinum-0.1.4/tests/test_tablinum.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 tablinum-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tablinum-0.1.4/LICENSE
+-rw-r--r--   0        0        0    61650 2020-02-02 00:00:00.000000 tablinum-0.1.4/README.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 tablinum-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    62645 2020-02-02 00:00:00.000000 tablinum-0.1.4/PKG-INFO
```

### Comparing `tablinum-0.1.3/src/tablinum/tab_fun_dates.py` & `tablinum-0.1.4/src/tablinum/tab_fun_dates.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/src/tablinum/tab_fun_maths.py` & `tablinum-0.1.4/src/tablinum/tab_fun_maths.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/src/tablinum/tab_fun_useful.py` & `tablinum-0.1.4/src/tablinum/tab_fun_useful.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/src/tablinum/tablinum.py` & `tablinum-0.1.4/src/tablinum/tablinum.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,15 +168,16 @@
 
     try:
         return (float(x), x)
     except ValueError:
         pass
 
     try:
-        return (tab_fun_dates.parse_date(x).toordinal(), x)   # make parse date return epoch sec string
+        # try to parse the date and return an ordinal number
+        return (tab_fun_dates.parse_date(x).toordinal(), x)
     except ValueError:
         pass
 
     # is this a time?
     if (m := re.match(r'(\d+):([0-5]\d):([0-5]\d(\.\d+)?)\Z', x)) is not None:
         return (int(m.group(1)) * 3600 + int(m.group(2)) * 60 + float(m.group(3)), x)
 
@@ -272,15 +273,16 @@
     except (ValueError, SyntaxError):
         pass
 
     try:
         if trial_number.endswith('%'):
             return (True, decimal.Decimal(trial_number[:-1]) / 100)
         if trial_number[-1] in suffix:
-            return (True, decimal.Decimal(trial_number[:-1]) + decimal.Decimal(suffix.index(trial_number[-1])) / 4)
+            quarters = decimal.Decimal(suffix.index(trial_number[-1])) / 4
+            return (True, decimal.Decimal(trial_number[:-1]) + quarters)
         return (True, decimal.Decimal(trial_number))
     except ArithmeticError:
         pass
 
     return (False, sss)
 
 
@@ -592,17 +594,20 @@
     return [quantile(x, p) for p in pvalues]
 
 
 def statistical_summary(numbers):
     '''return a 4/6 field summary of a list of numbers
     >>> statistical_summary([])
     ''
-    >>> statistical_summary([decimal.Decimal(x) for x in '36.4 67.1 82.7 34.2 96.8 10.9 19.1 71.8 66.0 29.2'.split()])
+
+    >>> tdat = [decimal.Decimal(x) for x in '36.4 67.1 82.7 34.2 96.8 10.9 19.1 71.8 66.0 29.2'.split()]
+    >>> statistical_summary(tdat)
     'Min: 10.9  Mean: 51.42  Max: 96.8'
-    >>> statistical_summary([decimal.Decimal(x) for x in '0 1 2 3 4 5 6 8 9 36.4 67.1 82.7 34.2 96.8 10.9 29.2'.split()])
+    >>> tdat = [decimal.Decimal(x) for x in '0 1 2 3 4 5 6 8 9 36.4 67.1 82.7 34.2 96.8 10.9 29.2'.split()]
+    >>> statistical_summary(tdat)
     'Min: 0  Q25: 3.75  Median: 8.5  Mean: 24.70625  Q75: 34.750  Max: 96.8'
 
     '''
     if not numbers:
         return ''
 
     me = statistics.mean(numbers)
@@ -1517,71 +1522,97 @@
                         new_row.append(new_value)
                 except (ValueError, TypeError, NameError, AttributeError, decimal.InvalidOperation):
                     new_row.append(_replace_values(literal_code, values))
                 except ZeroDivisionError:
                     new_row.append("-")
             self.append(new_row)
 
-    def _fancy_col_index(self, col_spec):
+    def _fancy_col_index(self, column_letter):
         '''Find me an index, returns index + T/F to say if letter was upper case
+
+        >>> t = Table()
+        >>> a = (1, 2, 3, 4, 5, 6, 7, 8)
+        >>> b = (5, 23, 41, 2, 3, 4, 5, 6)
+        >>> t.parse_lol((a, b))
+        >>> t._fancy_col_index('a')
+        (0, False)
+        >>> t._fancy_col_index('B')
+        (1, True)
+        >>> t._fancy_col_index('Z')
+        (7, True)
+        >>> t._fancy_col_index('5')
+        (5, False)
+        >>> t._fancy_col_index('!!')
+        (None, False)
+
         '''
 
         flag = False
-        if col_spec in string.ascii_uppercase:
+        if column_letter in string.ascii_uppercase:
             flag = True
-            col_spec = col_spec.lower()
+            column_letter = column_letter.lower()
 
-        if col_spec in string.ascii_lowercase:
-            col_spec = ord(col_spec) - ord('a')
+        if column_letter in string.ascii_lowercase:
+            column_letter = ord(column_letter) - ord('a')
 
         try:
-            c = int(col_spec)
+            c = int(column_letter)
         except ValueError:
-            self.messages.append('?! colspec ' + col_spec)
+            self.messages.append('?! colspec ' + column_letter)
             return (None, flag)
 
         if c >= self.cols:
             c = self.cols - 1
         return (c, flag)
 
     def _sort_rows_by_col(self, col_spec=None):
         '''Sort the table
         By default sort by all columns left to right.
 
-        If the arg is a single number and abs(arg) < self.cols then sort on that column
+        Sort in groups where the col spec indicates the groups of cols
 
-        Otherwise sort in groups where the col spec indicates the groups of cols
+        a means use row[0] as the key
 
         abc means use the concatenation of row[0] + row[1] + row[2]
+
         upper case groups mean reverse sort
 
         groups are done right to left...
 
+        @ at the front of the colspec means pop first row, sort, then push row bacl
+        = at the front of the colspec means plain sort without smarts
+
         '''
         header = None
-        if '@' in col_spec:
+        want_smart = True
+
+        if col_spec.startswith('@'):
+            col_spec = col_spec[1:]
             header = self.pop(0)
-            col_spec = col_spec.replace('@', '')
+
+        if col_spec.startswith('='):
+            col_spec = col_spec[1:]
+            want_smart = False
 
         if col_spec is None or col_spec == '':
             col_spec = string.ascii_lowercase[:self.cols]
 
         if looks_like_formula(col_spec):
             self.do(f"arr ({col_spec})~ sort a arr -a")
 
         else:
-            try:
-                i = int(col_spec)
-            except ValueError:
-                for col in col_spec[::-1]:
-                    c, want_reverse = self._fancy_col_index(col)
-                    self.data.sort(key=lambda row: as_numeric_tuple(row[c], want_reverse), reverse=want_reverse)
-            else:
-                if -self.cols <= i < self.cols:
-                    self.data.sort(key=lambda row: as_numeric_tuple(row[i], False))
+            for col in col_spec[::-1]:
+                c, want_reverse = self._fancy_col_index(col)
+                if c is None:
+                    continue
+                if want_smart:
+                    self.data.sort(key=lambda row: as_numeric_tuple(row[c], want_reverse),
+                                   reverse=want_reverse)
+                else:
+                    self.data.sort(key=lambda row: row[c], reverse=want_reverse)
 
         if header is not None:
             self.insert(0, header)
 
     def _remove_duplicates_by_col(self, col_spec):
         '''like uniq, remove row if key cols match the row above
         '''
@@ -1738,17 +1769,18 @@
 
         # generate nicely lined up rows
         for i, row in enumerate(self.data):
             for ex in self.extras[i]:
                 if ex == 'rule' and ruler is not None:
                     if ruler == "plain":
                         yield ' ' * self.indent \
-                            + '-' * (sum(widths) + self.cols * len(separator) - len(separator) + len(eol_marker))
+                            + '-' * (sum(widths) + (self.cols - 1) * len(separator) + len(eol_marker))
                     elif ruler == "piped":
-                        yield ' ' * self.indent + separator.join(_pipe_rule(w, a) for w, a in zip(widths, aligns))
+                        yield ' ' * self.indent \
+                            + separator.join(_pipe_rule(w, a) for w, a in zip(widths, aligns))
                     else:
                         yield ruler
 
                 elif ex == 'blank' and blank_line is not None:
                     yield blank_line
 
                 elif ex.startswith('#') and comment_marker is not None:
@@ -1831,9 +1863,10 @@
 
     table.do(agenda)
     print(table)
 
     if args.file is not None:
         fh.close()
 
+
 if __name__ == "__main__":
     filter()
```

### Comparing `tablinum-0.1.3/tests/test_tab_calculation.py` & `tablinum-0.1.4/tests/test_tab_calculation.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_command_line.py` & `tablinum-0.1.4/tests/test_tab_command_line.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_contingency.py` & `tablinum-0.1.4/tests/test_tab_contingency.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_filter.py` & `tablinum-0.1.4/tests/test_tab_filter.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_grouping.py` & `tablinum-0.1.4/tests/test_tab_grouping.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_help.py` & `tablinum-0.1.4/tests/test_tab_help.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_levels.py` & `tablinum-0.1.4/tests/test_tab_levels.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_makers.py` & `tablinum-0.1.4/tests/test_tab_makers.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_parsing.py` & `tablinum-0.1.4/tests/test_tab_parsing.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_poppers_and_adders.py` & `tablinum-0.1.4/tests/test_tab_poppers_and_adders.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_roller.py` & `tablinum-0.1.4/tests/test_tab_roller.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_sort.py` & `tablinum-0.1.4/tests/test_tab_sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 Wednesday  0.91  0.17
 Thursday   0.22  0.94
 Friday     0.94  0.28
 Saturday   0.62  0.02
 Sunday     0.34  0.25
 '''.strip()
 
-
         self.addresses = '''
 Mac                IP
 00:01:E6:2C:42:1D  192.168.0.12
 3C:07:54:3D:3F:82  192.168.0.13
 60:C5:47:21:D7:E9  192.168.0.16
 2C:4D:54:74:A4:D8  192.168.0.4
 50:C7:BF:1C:88:66  192.168.0.3
@@ -59,20 +58,19 @@
 74:D0:2B:5D:CD:C0  192.168.0.2
 50:C7:BF:1C:88:66  192.168.0.3
 2C:4D:54:74:A4:D8  192.168.0.4
 00:01:E6:2C:42:1D  192.168.0.12
 3C:07:54:3D:3F:82  192.168.0.13
 60:C5:47:21:D7:E9  192.168.0.16
 '''.strip()
-        
 
     def test_filter(self):
         "Select matching rows"
         self.tab.parse_lines(self.rain.splitlines())
-        self.tab.do('sort')  # missing predicate does nothing because we start sorted
+        self.tab.do('sort')  # missing predicate does nothing here
         self.assertEqual(str(self.tab), self.rain)
         self.tab.do('sort j')
         expected = '''
 Date        Week  Mon  Tue  Wed  Thu  Fri  Sat   Sun  Total  Description
 ------------------------------------------------------------------------
 2019-12-30     1  0.0  0.2  0.0  0.0  1.2  0.0   0.0    1.4  Dry
 2020-01-20     4  0.0  0.0  0.0  0.0  0.0  0.1   2.3    2.4  Dry
@@ -218,15 +216,25 @@
 Wednesday  0.91  0.17
 Thursday   0.22  0.94
 Friday     0.94  0.28
 Saturday   0.62  0.02
 Sunday     0.34  0.25
 '''.strip())
 
+        self.tab.do('sort =a')
+        self.assertEqual(str(self.tab), '''
+Friday     0.94  0.28
+Monday     0.38  0.52
+Saturday   0.62  0.02
+Sunday     0.34  0.25
+Thursday   0.22  0.94
+Tuesday    0.41  0.14
+Wednesday  0.91  0.17
+'''.strip())
 
     def test_special_sorts(self):
         "Smart sorting"
         self.tab.parse_lines(self.addresses.splitlines())
-        self.tab.do('sort') 
+        self.tab.do('sort')
         self.assertEqual(str(self.tab), self.addresses_by_A)
         self.tab.do('sort b')
         self.assertEqual(str(self.tab), self.addresses_by_B)
```

### Comparing `tablinum-0.1.3/tests/test_tab_text_manip.py` & `tablinum-0.1.4/tests/test_tab_text_manip.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tab_wrangler.py` & `tablinum-0.1.4/tests/test_tab_wrangler.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/tests/test_tablinum.py` & `tablinum-0.1.4/tests/test_tablinum.py`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/.gitignore` & `tablinum-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/LICENSE` & `tablinum-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/README.md` & `tablinum-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1256,14 +1256,30 @@
     30 Sep 2021  The Tenant of Wildfell Hall    p780
     24 Sep 2020  Cave Art                       p904
     03 May 2018  The Almoravid Empire           p3972
     24 Nov 2016  Baltic Crusades                p5060
     20 Feb 2014  Social Darwinism               p5912
     11 Feb 2016  Rumi's Poetry                  p7019
 
+The smarts also recognize IP addresses, MAC addresses, and SI unit suffixes.
+If the smarts get your sorting wrong, then you can turn them off by adding "="
+to the front of the sort column specifier.  So you can do `sort =b` on the 
+table above to get this:
+
+    24 Nov 2016  Baltic Crusades                p5060
+    24 Sep 2020  Cave Art                       p904
+    04 Feb 2016  Chromatography                 p11
+    21 Sep 2017  Kant's Categorical Imperative  p265
+    11 Feb 2016  Rumi's Poetry                  p7019
+    20 Feb 2014  Social Darwinism               p5912
+    03 May 2018  The Almoravid Empire           p3972
+    29 Oct 2015  The Empire of Mali             p423
+    27 Feb 2020  The Evolution of Horses        p233
+    30 Sep 2021  The Tenant of Wildfell Hall    p780
+
 You can also sort on simple functions; essentially any function that you can use with `arr`.
 So given a table like this:
 
     tamarix     33  18
     tamasha     89  13
     tambac      57  72
     tambourine  48  46
```

### Comparing `tablinum-0.1.3/pyproject.toml` & `tablinum-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tablinum-0.1.3/PKG-INFO` & `tablinum-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tablinum
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tablinum is a Python library to make, manipulate, and neatly print tabular output to the console.
 Project-URL: Documentation, https://github.com/unknown/tablinum#readme
 Project-URL: Issues, https://github.com/unknown/tablinum/issues
 Project-URL: Source, https://github.com/unknown/tablinum
 Author-email: Toby Thurston <toby.thurston@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -1278,14 +1278,30 @@
     30 Sep 2021  The Tenant of Wildfell Hall    p780
     24 Sep 2020  Cave Art                       p904
     03 May 2018  The Almoravid Empire           p3972
     24 Nov 2016  Baltic Crusades                p5060
     20 Feb 2014  Social Darwinism               p5912
     11 Feb 2016  Rumi's Poetry                  p7019
 
+The smarts also recognize IP addresses, MAC addresses, and SI unit suffixes.
+If the smarts get your sorting wrong, then you can turn them off by adding "="
+to the front of the sort column specifier.  So you can do `sort =b` on the 
+table above to get this:
+
+    24 Nov 2016  Baltic Crusades                p5060
+    24 Sep 2020  Cave Art                       p904
+    04 Feb 2016  Chromatography                 p11
+    21 Sep 2017  Kant's Categorical Imperative  p265
+    11 Feb 2016  Rumi's Poetry                  p7019
+    20 Feb 2014  Social Darwinism               p5912
+    03 May 2018  The Almoravid Empire           p3972
+    29 Oct 2015  The Empire of Mali             p423
+    27 Feb 2020  The Evolution of Horses        p233
+    30 Sep 2021  The Tenant of Wildfell Hall    p780
+
 You can also sort on simple functions; essentially any function that you can use with `arr`.
 So given a table like this:
 
     tamarix     33  18
     tamasha     89  13
     tambac      57  72
     tambourine  48  46
```

