# Comparing `tmp/gaussprot-0.0.1.tar.gz` & `tmp/gaussprot-0.0.2.tar.gz`

## Comparing `gaussprot-0.0.1.tar` & `gaussprot-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gaussprot-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/.gitignore
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/gkprot.iml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/vcs.xml
--rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/workspace.xml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gaussprot-0.0.1/gaussprot/__init__.py
--rw-r--r--   0        0        0     7712 2020-02-02 00:00:00.000000 gaussprot-0.0.1/gaussprot/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gaussprot-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 gaussprot-0.0.1/tests/data.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 gaussprot-0.0.1/tests/test_gaussprot.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gaussprot-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 gaussprot-0.0.1/LICENSE
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gaussprot-0.0.1/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 gaussprot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    41306 2020-02-02 00:00:00.000000 gaussprot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gaussprot-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/gkprot.iml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/vcs.xml
+-rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 gaussprot-0.0.2/gaussprot/__init__.py
+-rw-r--r--   0        0        0     8395 2020-02-02 00:00:00.000000 gaussprot-0.0.2/gaussprot/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gaussprot-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 gaussprot-0.0.2/tests/data.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 gaussprot-0.0.2/tests/test_gaussprot.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gaussprot-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 gaussprot-0.0.2/LICENSE
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gaussprot-0.0.2/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 gaussprot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    41306 2020-02-02 00:00:00.000000 gaussprot-0.0.2/PKG-INFO
```

### Comparing `gaussprot-0.0.1/.github/workflows/python-package.yml` & `gaussprot-0.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `gaussprot-0.0.1/.idea/workspace.xml` & `gaussprot-0.0.2/.idea/workspace.xml`

 * *Files 13% similar despite different names*

#### Comparing `gaussprot-0.0.1/.idea/workspace.xml` & `gaussprot-0.0.2/.idea/workspace.xml`

```diff
@@ -1,54 +1,61 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
-    <list default="true" id="9c7cb33f-4008-43f5-9936-57406dcec0ab" name="Changes" comment="update min python version"/>
+    <list default="true" id="9c7cb33f-4008-43f5-9936-57406dcec0ab" name="Changes" comment="bump version"/>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
+    <option name="RECENT_BRANCH_BY_REPOSITORY">
+      <map>
+        <entry key="$PROJECT_DIR$" value="master"/>
+      </map>
+    </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
     <option name="UPDATE_TYPE" value="REBASE"/>
   </component>
   <component name="ProjectColorInfo">{
   &quot;associatedIndex&quot;: 8
 }</component>
   <component name="ProjectId" id="2goRKxWsTv0J41TzUDSNoX73fao"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "Python tests.Python tests for tests.test_gaussprot.TestGaussProt.executor": "Run",
+    "Python tests.Python tests for tests.test_gaussprot.TestGaussProt.test_init_signature.executor": "Run",
+    "Python tests.Python tests for tests.test_gaussprot.TestGaussProt.test_simply_encode.executor": "Run",
     "Python.main.executor": "Run",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "git-widget-placeholder": "master",
     "last_opened_file_path": "/home/stefan/PycharmProjects/mhc",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "nodejs_package_manager_path": "npm",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
-  <component name="RunManager" selected="Python tests.Python tests for tests.test_gaussprot.TestGaussProt">
+  <component name="RunManager" selected="Python tests.Python tests for tests.test_gaussprot.TestGaussProt.test_simply_encode">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="gkprot"/>
       <option name="ENV_FILES" value=""/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
@@ -80,17 +87,51 @@
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;tests.test_gaussprot.TestGaussProt&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
+    <configuration name="Python tests for tests.test_gaussprot.TestGaussProt.test_init_signature" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+      <module name="gkprot"/>
+      <option name="ENV_FILES" value=""/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_gaussprot.TestGaussProt.test_init_signature&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <method v="2"/>
+    </configuration>
+    <configuration name="Python tests for tests.test_gaussprot.TestGaussProt.test_simply_encode" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+      <module name="gkprot"/>
+      <option name="ENV_FILES" value=""/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;tests.test_gaussprot.TestGaussProt.test_simply_encode&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <method v="2"/>
+    </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python tests.Python tests for tests.test_gaussprot.TestGaussProt.test_simply_encode"/>
         <item itemvalue="Python tests.Python tests for tests.test_gaussprot.TestGaussProt"/>
+        <item itemvalue="Python tests.Python tests for tests.test_gaussprot.TestGaussProt.test_init_signature"/>
         <item itemvalue="Python.main"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SharedIndexes">
     <attachedChunks>
       <set>
@@ -104,15 +145,16 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="9c7cb33f-4008-43f5-9936-57406dcec0ab" name="Changes" comment=""/>
       <created>1716361884168</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1716361884168</updated>
       <workItem from="1716361885387" duration="22309000"/>
-      <workItem from="1716466731223" duration="4772000"/>
+      <workItem from="1716466731223" duration="5462000"/>
+      <workItem from="1716637273604" duration="2570000"/>
     </task>
     <task id="LOCAL-00001" summary="add code blueprint">
       <option name="closed" value="true"/>
       <created>1716401711516</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
@@ -218,20 +260,55 @@
       <option name="closed" value="true"/>
       <created>1716532177115</created>
       <option name="number" value="00014"/>
       <option name="presentableId" value="LOCAL-00014"/>
       <option name="project" value="LOCAL"/>
       <updated>1716532177115</updated>
     </task>
-    <option name="localTasksCounter" value="15"/>
+    <task id="LOCAL-00015" summary="add test for class signature">
+      <option name="closed" value="true"/>
+      <created>1716705364879</created>
+      <option name="number" value="00015"/>
+      <option name="presentableId" value="LOCAL-00015"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716705364879</updated>
+    </task>
+    <task id="LOCAL-00016" summary="add encoding method; add unit test;">
+      <option name="closed" value="true"/>
+      <created>1716705945642</created>
+      <option name="number" value="00016"/>
+      <option name="presentableId" value="LOCAL-00016"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716705945642</updated>
+    </task>
+    <task id="LOCAL-00017" summary="bump version">
+      <option name="closed" value="true"/>
+      <created>1716706066153</created>
+      <option name="number" value="00017"/>
+      <option name="presentableId" value="LOCAL-00017"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1716706066153</updated>
+    </task>
+    <option name="localTasksCounter" value="18"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
+  <component name="Vcs.Log.Tabs.Properties">
+    <option name="TAB_STATES">
+      <map>
+        <entry key="MAIN">
+          <value>
+            <State/>
+          </value>
+        </entry>
+      </map>
+    </option>
+  </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="add code blueprint"/>
     <MESSAGE value="implement full sharding; finalize modeling function"/>
     <MESSAGE value="optimize auc"/>
     <MESSAGE value="finish validator and schema standardizer"/>
     <MESSAGE value="add docstrings;"/>
     <MESSAGE value="add toml file; add test files;"/>
@@ -239,14 +316,17 @@
     <MESSAGE value="optionally validate schema"/>
     <MESSAGE value="add discrete tests; fix discrete model type;"/>
     <MESSAGE value="add test for continuous models;"/>
     <MESSAGE value="update readme"/>
     <MESSAGE value="add requirements.txt"/>
     <MESSAGE value="raise exception when continuous model and discrete length set"/>
     <MESSAGE value="update min python version"/>
-    <option name="LAST_COMMIT_MESSAGE" value="update min python version"/>
+    <MESSAGE value="add test for class signature"/>
+    <MESSAGE value="add encoding method; add unit test;"/>
+    <MESSAGE value="bump version"/>
+    <option name="LAST_COMMIT_MESSAGE" value="bump version"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/gkprot$main.coverage" NAME="main Coverage Results" MODIFIED="1716400758958" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="false" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/gaussprot"/>
-    <SUITE FILE_PATH="coverage/gkprot$.coverage" NAME=" Coverage Results" MODIFIED="1716490194485" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="false" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
+    <SUITE FILE_PATH="coverage/gkprot$.coverage" NAME=" Coverage Results" MODIFIED="1716705910418" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="false" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
   </component>
 </project>
```

### Comparing `gaussprot-0.0.1/.idea/inspectionProfiles/Project_Default.xml` & `gaussprot-0.0.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `gaussprot-0.0.1/gaussprot/main.py` & `gaussprot-0.0.2/gaussprot/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -170,7 +170,23 @@
     def _standardize_schema(self):
         vals = list(self.schema.values())
         min_ = min(vals)
         max_ = max(vals)
         for k, v in self.schema.items():
             self.schema[k] = 2 * (v - min_) / (max_ - min_) - 1
 
+    def simply_encode(self, sequences: list[str]) -> list[np.ndarray]:
+        """
+        Encode sequences using the schema.
+        :param sequences: list of sequences
+        :return: list[np.ndarray]
+        """
+        if not self.padded:
+            return [np.array([self.schema[x] for x in seq]) for seq in sequences]
+        encoded_sequences = []
+        max_len = max([len(seq) for seq in sequences])
+        for seq in sequences:
+            enc_seq = [self.schema[x] for x in seq]
+            if len(enc_seq) < max_len:
+                enc_seq.extend([0]*(max_len - len(enc_seq)))
+            encoded_sequences.append(np.array(enc_seq))
+        return encoded_sequences
```

### Comparing `gaussprot-0.0.1/tests/data.py` & `gaussprot-0.0.2/tests/data.py`

 * *Files identical despite different names*

### Comparing `gaussprot-0.0.1/.gitignore` & `gaussprot-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gaussprot-0.0.1/LICENSE` & `gaussprot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussprot-0.0.1/pyproject.toml` & `gaussprot-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gaussprot"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Stefan Stojanovic", email="stefs304@gmail.com" },
 ]
 description = "Utility for generating Gaussian kernel models of proteins"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
```

### Comparing `gaussprot-0.0.1/PKG-INFO` & `gaussprot-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gaussprot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility for generating Gaussian kernel models of proteins
 Project-URL: Homepage, https://github.com/stefs304/gaussprot
 Project-URL: Issues, https://github.com/stefs304/gaussprot/issues
 Author-email: Stefan Stojanovic <stefs304@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

