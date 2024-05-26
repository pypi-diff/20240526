# Comparing `tmp/pydematel-0.1.0.tar.gz` & `tmp/pydematel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydematel-0.1.0.tar", last modified: Sun May 26 13:46:28 2024, max compression
+gzip compressed data, was "pydematel-0.1.1.tar", last modified: Sun May 26 14:43:05 2024, max compression
```

## Comparing `pydematel-0.1.0.tar` & `pydematel-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 13:46:28.759501 pydematel-0.1.0/
--rw-rw-rw-   0        0        0     1512 2024-05-26 11:51:08.000000 pydematel-0.1.0/LICENSE.md
--rw-rw-rw-   0        0        0     1585 2024-05-26 13:46:28.759501 pydematel-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-26 13:44:24.000000 pydematel-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 13:46:23.790744 pydematel-0.1.0/pyDEMATEL/
--rw-rw-rw-   0        0        0     7373 2024-05-26 12:24:19.000000 pydematel-0.1.0/pyDEMATEL/DEMATEL_Solver.py
--rw-rw-rw-   0        0        0    28327 2024-05-26 13:40:36.000000 pydematel-0.1.0/pyDEMATEL/DEMATEL_Window.py
--rw-rw-rw-   0        0        0    15162 2024-05-26 12:27:04.000000 pydematel-0.1.0/pyDEMATEL/Fuzzy_DEMATEL_Solver.py
--rw-rw-rw-   0        0        0        0 2024-05-26 09:58:28.000000 pydematel-0.1.0/pyDEMATEL/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 13:46:28.758032 pydematel-0.1.0/pyDEMATEL.egg-info/
--rw-rw-rw-   0        0        0     1585 2024-05-26 13:46:18.000000 pydematel-0.1.0/pyDEMATEL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-26 13:46:19.000000 pydematel-0.1.0/pyDEMATEL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 13:46:18.000000 pydematel-0.1.0/pyDEMATEL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-26 13:46:18.000000 pydematel-0.1.0/pyDEMATEL.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 13:46:28.762160 pydematel-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      851 2024-05-26 13:44:54.000000 pydematel-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:43:05.954806 pydematel-0.1.1/
+-rw-rw-rw-   0        0        0     1512 2024-05-26 11:51:08.000000 pydematel-0.1.1/LICENSE.md
+-rw-rw-rw-   0        0        0     1585 2024-05-26 14:43:05.952906 pydematel-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-26 13:44:24.000000 pydematel-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-26 14:43:05.678446 pydematel-0.1.1/pyDEMATEL/
+-rw-rw-rw-   0        0        0     7446 2024-05-26 14:28:07.000000 pydematel-0.1.1/pyDEMATEL/DEMATEL_Solver.py
+-rw-rw-rw-   0        0        0    25237 2024-05-26 14:34:38.000000 pydematel-0.1.1/pyDEMATEL/DEMATEL_Window.py
+-rw-rw-rw-   0        0        0    15239 2024-05-26 14:28:20.000000 pydematel-0.1.1/pyDEMATEL/Fuzzy_DEMATEL_Solver.py
+-rw-rw-rw-   0        0        0        0 2024-05-26 09:58:28.000000 pydematel-0.1.1/pyDEMATEL/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 14:43:05.950207 pydematel-0.1.1/pyDEMATEL.egg-info/
+-rw-rw-rw-   0        0        0     1585 2024-05-26 14:43:03.000000 pydematel-0.1.1/pyDEMATEL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-26 14:43:03.000000 pydematel-0.1.1/pyDEMATEL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 14:43:03.000000 pydematel-0.1.1/pyDEMATEL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-26 14:43:03.000000 pydematel-0.1.1/pyDEMATEL.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 14:43:05.954806 pydematel-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-05-26 14:25:49.000000 pydematel-0.1.1/setup.py
```

### Comparing `pydematel-0.1.0/LICENSE.md` & `pydematel-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydematel-0.1.0/PKG-INFO` & `pydematel-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDEMATEL
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyDematel a python-based tool implementing the Dematel and fuzzy Dematel methods for improved decision making
 Home-page: https://github.com/achekry/-Elsevier-SoftwareX-pyDEMATEL
 Author: Abderrahman CHEKRY, Jamal Bakkas, Mohamed Hanine
 Author-email: a.chekry@uca.ac.ma
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydematel-0.1.0/README.md` & `pydematel-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydematel-0.1.0/pyDEMATEL/DEMATEL_Solver.py` & `pydematel-0.1.1/pyDEMATEL/DEMATEL_Solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         return self.numberOfFactors  
 
     
     def getMatrix(self):
         return self.matrix
     def setMatrix(self, matrices):
         self.matrix=matrices
+    def AddMatrix(self, matrix):
+        self.matrix.append(matrix)   
     def setExperts(self, experts):
             self.experts=experts
     def getExperts(self):
         return self.experts            
     def addExpert(self, expert):
             self.experts.append(expert)
     def setFactors(self, factors):
```

### Comparing `pydematel-0.1.0/pyDEMATEL/DEMATEL_Window.py` & `pydematel-0.1.1/pyDEMATEL/DEMATEL_Window.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.window.attributes("-fullscreen", False)  # Ensure fullscreen is not set
         self.window.grid_columnconfigure(0, weight=1)
         self.MatrixX=[]         
         #self.noInfuence="No influence 0"     
         
         titre = tk.Label(self.window, text="pyDEMATEL : DEMATEL & Fuzzy DEMATEL Solver", font=('Helvetica', 20, 'bold'), fg='#2E4053')
         titre.grid(row=0, column=0, padx=10, pady=10, sticky="n")
-        # Création du frame input numbers of experts and factors & fill factors & experts
+        # frame input numbers of experts and factors & fill factors & experts
         self.createInputFrames()
 
         
     
         
     def usingDematel(self):
         self.MatrixX=[]         
@@ -49,53 +49,52 @@
         self.inputFrames = tk.Frame(self.window)
         self.inputFrames.grid(row=1, column=0, padx=10, pady=(0, 5), sticky="nsew")
         self.inputFrames.grid_columnconfigure((0, 1), weight=1)    
         self.createInputNumbersFrame()
         self.createInputNamesFrame()
         self.createButtonsDMATELFrame()
         
-     # Création du frame input numbers of experts and factors
+     # frame input numbers of experts and factors
     def createInputNumbersFrame(self):
         frmNumbers = tk.LabelFrame(self.inputFrames,text="Input Numbers", bg="#ECF0F1", padx=10, pady=10, relief='groove', bd=2)
         frmNumbers.grid(row=0, column=0, padx=10, pady=(0, 5), sticky="nsew")
         #défilement
         
         
-        # Label et zone de texte pour le nombre d'experts
+        
         label1 = tk.Label(frmNumbers, text="Number of experts:",font=('sans serif', 10, 'bold'))
         label1.grid(row=1, column=0, padx=10, pady=5, sticky="w")
         self.txtExperts = tk.Entry(frmNumbers,font=('sans serif', 10, 'bold'), bg='#D2D4CF')
         self.txtExperts.grid(row=1, column=1, padx=10, pady=5)    
    
-        # Label et zone de texte pour  le nombre des facteurs
+       
         label2 = tk.Label(frmNumbers, text="Number of factors:",font=('sans serif', 10, 'bold'))
         label2.grid(row=2, column=0, padx=10, pady=5, sticky="w")
         self.txtFactors = tk.Entry(frmNumbers,font=('sans serif', 10, 'bold'), bg='#D2D4CF')
         self.txtFactors.grid(row=2, column=1, padx=10, pady=5)
         
-        # Bouton "Add"
+       
         btnAdd = tk.Button(frmNumbers, text="           Add           ", font=("sans serif", 10, "bold"), command=self.on_btnAdd_click, bg="#CDD3C4", fg="black", relief="flat", padx=10, pady=5)
         btnAdd.grid(row=3, column=1, columnspan=2, padx=10, pady=(0, 5))
     
-    # Création du frame input experts and factors    
+    # frame input experts and factors    
     def createInputNamesFrame(self):
         self.frmNames = tk.LabelFrame(self.inputFrames,text="Input Names", bg="#ECF0F1", padx=10, pady=10, relief='groove', bd=2)
         self.frmNames.grid(row=0, column=1,padx=10, pady=(0, 5), sticky="nsew")
         
         scrollbar = ttk.Scrollbar( self.frmNames, orient="vertical")
         scrollbar.pack(side="right", fill="y")
         canvas = tk.Canvas( self.frmNames , yscrollcommand=scrollbar.set, height=100)
         canvas.pack(side="left", fill="both", expand=True)
         scrollbar.config(command=canvas.yview)
         self.frmInnerNames = ttk.Frame(canvas)
         canvas.create_window((0, 0), window=self.frmInnerNames, anchor="nw")
-        # Configurer le défilement du canevas lorsque son contenu change
         self.frmInnerNames.bind("<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all")))
  
-    # Création du frame boutons DMATEL And Fuzzy DEMATEL resolve  
+    # frame boutons DMATEL And Fuzzy DEMATEL resolve  
     def createButtonsDMATELFrame(self):
         self.frmButtons = tk.Frame(self.inputFrames,bg="#ECF0F1", padx=10, pady=10, relief='groove')
         self.frmButtons.grid(row=0, column=2,padx=10, pady=(0, 5), sticky="nsew")
         
                  
 
     def createInputValuesAndResaulsFrames(self):
@@ -116,15 +115,14 @@
         hScrollbar.pack(side="bottom", fill="x")     
         canvas = tk.Canvas( self.frmValues , yscrollcommand=vSscrollbar.set, xscrollcommand=hScrollbar.set, height=100)
         canvas.pack(side="left", fill="both", expand=True)
         vSscrollbar.config(command=canvas.yview)
         hScrollbar.config(command=canvas.xview)
         self.frmInnerValues = ttk.Frame(canvas)
         canvas.create_window((0, 0), window=self.frmInnerValues, anchor="nw")
-        # Configurer le défilement du canevas lorsque son contenu change
         self.frmInnerValues.bind("<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all")))
 
         
         
     def createResultsFrame(self):
         self.frmResults = tk.LabelFrame(self.InputValuesAndResaulsFrames,text="Results",height=400,width=400)
         self.frmResults.grid(row=0, column=1, padx=10, pady=(0, 5), sticky="nsew")
@@ -136,22 +134,20 @@
         hScrollbar.pack(side="bottom", fill="x")  
         canvas = tk.Canvas( self.frmResults ,  yscrollcommand=vSscrollbar.set, xscrollcommand=hScrollbar.set, height=100)
         canvas.pack(side="left", fill="both", expand=True)
         vSscrollbar.config(command=canvas.yview)
         hScrollbar.config(command=canvas.xview)
         self.frmInnerResults = ttk.Frame(canvas)
         canvas.create_window((0, 0), window=self.frmInnerResults, anchor="nw")
-        # Configurer le défilement du canevas lorsque son contenu change
         self.frmInnerResults.bind("<Configure>", lambda e: canvas.configure(scrollregion=canvas.bbox("all")))
         
     
        
  
     def generate_table(self, parent_frame, nbFactors,nCol):
-        # Création d'une grille de cadres pour simuler un tableau avec bordures
         table_frames = []
         for i in range(nbFactors + 1):  # +1 for titles
             row_frames = []
             for j in range(nCol + 1):  # +1 for titles
                 outer_frame = tk.Frame(parent_frame, highlightbackground="black", highlightcolor="black", highlightthickness=1, bd=0)
                 outer_frame.grid(row=i, column=j, sticky="nsew")
                 inner_frame = ttk.Frame(outer_frame)
@@ -160,49 +156,46 @@
             table_frames.append(row_frames)
         return table_frames
     
 
     def createExperts(self):
           self.expertNames=[]
           for i in range(self.num_experts):
-              # Label et zone de texte pour les dimensions du tableau
               lblNameExpert = tk.Label(self.frmInnerNames, text="Expert "+ str(i+1), font=('sans serif', 10, 'bold'))
               lblNameExpert.grid(row=1+i, column=0, padx=10, pady=5, sticky="w")
               self.expertNames.append(tk.Entry(self.frmInnerNames ,font=('sans serif', 10, 'bold'), bg='#D2D4CF'))
               self.expertNames[i].insert(0,"Expert"+str(i))
               self.expertNames[i].grid(row=1+i, column=1, padx=10, pady=5)
               
             
     def createFactors(self):
           self.FactorsNames=[]
           for i in range(self.num_factors):
-              # Label et zone de texte pour les dimensions du tableau
               lblNameFactor = tk.Label(self.frmInnerNames, text="Factor "+ str(i+1),font=('sans serif', 10, 'bold'))
               lblNameFactor.grid(row=1+i, column=2, padx=10, pady=5, sticky="w")
               self.FactorsNames.append(tk.Entry(self.frmInnerNames,font=('sans serif', 10, 'bold'), bg='#D2D4CF'))
               
               self.FactorsNames[i].insert(0,"Factor"+str(i))
               self.FactorsNames[i].grid(row=1+i, column=3, padx=10, pady=5)     
                     
-        # Creation des onglets         
+        # tabs        
     def createTabs(self):
-        # Bouton "Resolve"
+
         btnResolve = tk.Button(self.window, text="              Resolve              ", command=self.on_btnResolve_click, font=("sans serif", 10, "bold"), bg="#CDD3C4", fg="black", relief="flat", padx=10, pady=5)
         btnResolve.grid(row=4, column=0, columnspan=2, padx=10, pady=(0, 5))
         
-        # Notebook pour les onglets
+
         self.notebook = ttk.Notebook(self.frmInnerValues)
         self.notebook.grid(row=1, column=0, columnspan=5, padx=10, pady=10, sticky="nsew")
         
-        #Titres des onglets
+
         titlesTabs = [entry.get() for entry in self.expertNames]
         for i, title in enumerate(titlesTabs):
             frame = ttk.Frame(self.notebook)
             self.notebook.add(frame, text=title)
-            # Générer le tableau dans chaque onglet
             table_frames = self.generate_table(frame, self.num_factors, self.num_factors)
             self.matrixExpertTab(table_frames, self.num_factors)
         
     def fillFactors(self):
         titles = [entry.get() for entry in self.FactorsNames]
         for j, title in enumerate(titles):
             self.solver.factors.append(title)
@@ -226,15 +219,15 @@
                 j=0
                 for v in row:
                     self.solver.matrix[k][i][j]=self.influeceIndiceFactor[v.get()]
                     j+=1
                 i+=1
             k+=1
         
-    def fillMatrixZ(self, tab_name):                  #Remplissage de:  Direct-influence matrix Z
+    def fillMatrixZ(self, tab_name):                  #fillDirect-influence matrix Z
         tab_frame = self.tabsIDs.get(tab_name)
         
         # Générer le tableau
         if tab_frame:
             table_frames = self.generate_table(tab_frame, self.num_factors, self.num_factors)
             
             # Titres de la première ligne
@@ -244,27 +237,26 @@
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
         
             # Titres de la première colonne
             for i, title in enumerate(titles):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[i + 1][0], text=title)
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
           
-        # Ajout des labels avec les valeurs de self.solver.Z
         for i in range(1, self.num_factors + 1):
             for j in range(1, self.num_factors + 1):
-                value = self.solver.Z[i-1, j-1]  # Utilisez une seule valeur de self.solver.Z
+                value = self.solver.Z[i-1, j-1] 
                 if self.dim==3:
                     txt='('+str(f"{value[0]:.2f}") +','+str(f"{value[1]:.2f}")+',' +str(f"{value[2]:.2f}") +')'
                 else:
                     txt=f"{value:.2f}"
-                lblValue = ttk.Label(table_frames[i][j], text=txt)  # Formatez la valeur si nécessaire
+                lblValue = ttk.Label(table_frames[i][j], text=txt) 
                 lblValue.grid(row=0, column=0, padx=5, pady=5)
 
 
-    def fillMatrixX(self, tab_name):                  #Remplissage de:  Direct-influence matrix X
+    def fillMatrixX(self, tab_name):                  
 
         tab_frame = self.tabsIDs.get(tab_name)
         
         # Générer le tableau
         if tab_frame:
             table_frames = self.generate_table(tab_frame, self.num_factors, self.num_factors)
             
@@ -275,98 +267,91 @@
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
         
             # Titres de la première colonne
             for i, title in enumerate(titles):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[i + 1][0], text=title)
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
           
-        # Ajout des labels avec les valeurs de self.solver.X
         for i in range(1, self.num_factors + 1):
             for j in range(1, self.num_factors + 1):
-                value = self.solver.X[i-1, j-1]  # Utilisez une seule valeur de self.solver.X
+                value = self.solver.X[i-1, j-1]  
                 if self.dim==3:
                     txt='('+str(f"{value[0]:.2f}") +','+str(f"{value[1]:.2f}")+',' +str(f"{value[2]:.2f}") +')'
                 else:
                     txt=f"{value:.2f}"
-                lblValue = ttk.Label(table_frames[i][j], text=txt)  # Formatez la valeur si nécessaire
+                lblValue = ttk.Label(table_frames[i][j], text=txt)  
                 lblValue.grid(row=0, column=0, padx=5, pady=5)     
 
-    def fillMatrixT(self, tab_name):                  #Remplissage de:  Direct-influence matrix X
+    def fillMatrixT(self, tab_name):                  #fill Direct-influence matrix X
         tab_frame = self.tabsIDs.get(tab_name)
         
         # Générer le tableau
         if tab_frame:
             table_frames = self.generate_table(tab_frame, self.num_factors, self.num_factors)
             
-            # Titres de la première ligne
             titles = [entry.get() for entry in self.FactorsNames]
             for j, title in enumerate(titles):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[0][j + 1], text=title)
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
         
-            # Titres de la première colonne
             for i, title in enumerate(titles):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[i + 1][0], text=title)
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
           
-        # Ajout des labels avec les valeurs de self.solver.T
-        #j'ai un problème d'affichage a resoudre
+
         for i in range(1, self.num_factors + 1):
             for j in range(1, self.num_factors + 1):
-                value = self.solver.T[i-1][j-1]  # Accès à la valeur dans le tableau numpy multidimensionnel
+                value = self.solver.T[i-1][j-1]  
                 if self.dim==3:
                     txt='('+str(f"{value[0]:.2f}") +','+str(f"{value[1]:.2f}") +','+str(f"{value[2]:.2f}") +')'
                 else:
                     txt=f"{value:.2f}"
-                lblValue = ttk.Label(table_frames[i][j], text=txt)  # Formatez la valeur si nécessaire
+                lblValue = ttk.Label(table_frames[i][j], text=txt)  
                 lblValue.grid(row=0, column=0, padx=5, pady=5)
 
     
-    def fillMatrixIRM(self, tab_name):                  #Remplissage de:  Direct-influence matrix IRM
+    def fillMatrixIRM(self, tab_name):                  
         indicators = ["R","C","R+C","R-C"]
-        #self.solver.step4()
         tab_frame = self.tabsIDs.get(tab_name)
-        # Générer le tableau
+
         if tab_frame:
             table_frames = self.generate_table(tab_frame, self.num_factors,len(indicators))
-            # Titres de la première ligne
+
             titles = [entry.get() for entry in self.FactorsNames]
             for j, title in enumerate(titles):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[j + 1][0], text=title)
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
-              # Titres de la première colonne
+
             for i in range(len(indicators)):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[0][i + 1], text=indicators[i])
-                lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)# Titres de la première colonne
+                lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
             for i in range(1, self.num_factors + 1):
                     lblValueR = ttk.Label(table_frames[i][1], text=f"{self.solver.R[i-1]:.2f}")  
                     lblValueR.grid(row=0, column=0, padx=5, pady=5)
                     lblValueC = ttk.Label(table_frames[i][2], text=f"{self.solver.C[i-1]:.2f}")  
                     lblValueC.grid(row=0, column=1, padx=5, pady=5)
                     lblValueRelation = ttk.Label(table_frames[i][3], text=f"{self.solver.prominence[i-1]:.2f}")  
                     lblValueRelation.grid(row=0, column=3, padx=5, pady=5)
                     lblValueProminence = ttk.Label(table_frames[i][4], text=f"{self.solver.relation[i-1]:.2f}")  
                     lblValueProminence.grid(row=0, column=2, padx=5, pady=5)
        
-    def fillMatrixFuzzyIRM(self, tab_name):                  #Remplissage de:  Direct-influence matrix IRM
+    def fillMatrixFuzzyIRM(self, tab_name):                  #fill Direct-influence matrix IRM
         indicators = ["R","C","R+C","R-C"]
         #self.solver.step4()
         tab_frame = self.tabsIDs.get(tab_name)
         # Générer le tableau
         if tab_frame:
             table_frames = self.generate_table(tab_frame, self.num_factors,len(indicators))
-            # Titres de la première ligne
             titles = [entry.get() for entry in self.FactorsNames]
             for j, title in enumerate(titles):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[j + 1][0], text=title)
                 lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
-              # Titres de la première colonne
             for i in range(len(indicators)):
                 lblTitleFactorInTableTab = ttk.Label(table_frames[0][i + 1], text=indicators[i])
-                lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)# Titres de la première colonne
+                lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
             for i in range(1, self.num_factors + 1):
                     value = self.solver.FR[i-1] 
                     txt='('+str(f"{value[0]:.2f}") +','+str(f"{value[1]:.2f}") +','+str(f"{value[2]:.2f}") +')'
                     lblValueR = ttk.Label(table_frames[i][1], text=txt)  
                     lblValueR.grid(row=0, column=0, padx=5, pady=5)
                     
                     value = self.solver.FC[i-1] 
@@ -383,28 +368,24 @@
                     txt='('+str(f"{value[0]:.2f}") +','+str(f"{value[1]:.2f}") +','+str(f"{value[2]:.2f}") +')'
                     lblValueRelation = ttk.Label(table_frames[i][4], text=txt)  
                     lblValueRelation.grid(row=0, column=3, padx=5, pady=5)
         
     def drawCurve(self, tab_name):
         tab_frame = self.tabsIDs.get(tab_name)
         if tab_frame:
-            fig, ax = plt.subplots(figsize=(2, 2))  # Largeur: 6 pouces, Hauteur: 4 pouces
-            #ax.plot(self.solver.prominence,  self.solver.relation, marker='o')
+            fig, ax = plt.subplots(figsize=(2, 2))  
             ax.scatter(self.solver.prominence,  self.solver.relation, marker='o', s=50)  
             for name,p,r in zip(self.solver.factors, self.solver.prominence, self.solver.relation):
                 ax.text(p, r, name, ha='center', va='bottom')
             ax.set_xlabel('R+C')
             ax.set_ylabel('R-C')
-            #ax.set_title('Courbe de C en fonction de R')
 
-            # Afficher l'axe f(X) = 0
             ax.axhline(0, color='black', linestyle='--')
 
-            # Afficher les graphiques
-            plt.tight_layout()  # Ajuster les espacements entre les sous-figures
+            plt.tight_layout()  
 
             canvas = FigureCanvasTkAgg(fig, master=tab_frame)
             canvas.draw()
             canvas_widget = canvas.get_tk_widget()
             canvas_widget.pack(fill=tk.BOTH, expand=True)
             canvas_widget.config(width=350, height=450)
             canvas.get_tk_widget().pack(fill=tk.BOTH, expand=True)
@@ -414,45 +395,42 @@
     def matrixExpertTab(self, table_frames, nbFactors):
         # Titres de la première ligne
         titles = [entry.get() for entry in self.FactorsNames]
         for j, title in enumerate(titles):
             lblTitleFactorInTableTab = ttk.Label(table_frames[0][j + 1], text=title)
             lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
     
-        # Titres de la première colonne
+
         titles = [entry.get() for entry in self.FactorsNames]
         for i, title in enumerate(titles):
             lblTitleFactorInTableTab = ttk.Label(table_frames[i + 1][0], text=title)
             lblTitleFactorInTableTab.grid(row=0, column=0, padx=5, pady=5)
       
         
-        # Ajout des listes déroulantes dans le reste du tableau
         M=[]
         for i in range(1, nbFactors + 1):
             row=[]
             for j in range(1, nbFactors + 1):
                 if i == j:
                     combo_values = [self.noInfuence]
                     combo = ttk.Combobox(table_frames[i][j], values=combo_values, state="readonly")
-                    combo.current(0)  # Sélectionne le premier choix par défaut
+                    combo.current(0) 
                     combo.grid(row=0, column=0, padx=5, pady=5)
                     row.append(combo)
                 else:
                     row.append(ttk.Combobox(table_frames[i][j],  values=list(self.influeceIndiceFactor.keys()), state="readonly"))
                     row[j-1].grid(row=0, column=0, padx=5, pady=5)
-                    # combo_box.bind("<<ComboboxSelected>>", self.on_combobox_select)
+
             M.append(row)
         self.MatrixX.append(M)
     
-    # Creation des onglets de resultats      
+   
     def createResultTabs(self):
 
-        # Notebook pour les onglets
-        self.notebookResult = ttk.Notebook(self.frmInnerResults)
-        #***** Titres des onglets******        
+        self.notebookResult = ttk.Notebook(self.frmInnerResults)     
         values_ResultTabsTitles= [
             "Causal Diagram", "Influential Relation Map IRM", "Direct-influence matrix Z", 
             "Normalized direct-influence matrix X", "Total-influence matrix T" ]
         nb=5
         if self.dim==3:
             nb=6
             values_ResultTabsTitles+=["Fuzzy IRM"]
@@ -465,52 +443,44 @@
             self.frame = ttk.Frame(self.notebookResult)
             self.notebookResult.add(self.frame, text=title)
             self.tabsIDs[title] = self.frame
             
         for tab_name in values_ResultTabsTitles:
             self.tab_frame = self.tabsIDs.get(tab_name)
     
-        # Appel de la methode qui permet le Remplissage de Influential Relation Map IRM
+
         self.fillMatrixIRM("Influential Relation Map IRM")
-        # Appel de la methode qui permet la construction du graphe des causes
-        #self.buildCausalDiagram("Causal Diagram")
-        # Appel de la methode qui permet le Remplissage de Direct-influence matrix Z
         self.fillMatrixZ("Direct-influence matrix Z")
-        # Appel de la methode qui permet le Remplissage de Normalized direct-influence matrix X
         self.fillMatrixX("Normalized direct-influence matrix X")
-        # Appel de la methode qui permet le Remplissage de Total-influence matrix T
         self.fillMatrixT("Total-influence matrix T")
         self.fillMatrixFuzzyIRM("Fuzzy IRM")
         self.drawCurve("Causal Diagram")
         
         btnExport = tk.Button(self.window, text="   Export Results   ", command=self.on_btnExport_click, font=("sans serif", 10, "bold"), bg="#CDD3C4", fg="black", relief="flat", padx=10, pady=5)
         btnExport.grid(row=4, column=0, columnspan=2, padx=10, pady=(0, 5))
    
     def on_btnExport_click(self):
         folder_path = filedialog.askdirectory()
         self.solver.savexl(folder_path)
         msg = tk.Label(self.window, text="Your file has been saved at: "+folder_path+"/DEMATELAnalysis.xlsx", font=('Helvetica', 12, 'bold'), fg='#2E4053')
         msg.grid(row=6, column=0, columnspan=4, padx=10, pady=(0, 5))
-  
-    # Fonction appelée lors du clic sur le bouton "Add"
+
     def on_btnAdd_click(self):
         self.num_experts = int(self.txtExperts.get())
         self.num_factors = int(self.txtFactors.get())
         self.createExperts()
         self.createFactors()
             
-        # Bouton "Generate" 
         btnGenerate = tk.Button(self.frmButtons, text="      DEMATEL Solver    ", command=self.on_btnGenerate_click, font=("sans serif", 10, "bold"), bg="#CDD3C4", fg="black", relief="flat", padx=10, pady=5)
         btnGenerate.grid(row=0, column=0, columnspan=2, padx=10, pady=(0, 5)) 
         
         btnGenerate = tk.Button(self.frmButtons, text="Fuzzy DEMATEL Solver", command=self.on_btnGenerateFuzzy_click, font=("sans serif", 10, "bold"),  bg="#CDD3C4", fg="black", relief="flat", padx=10, pady=5)
         btnGenerate.grid(row=1, column=0, columnspan=2, padx=10, pady=(0, 5)) 
 
 
-    # Fonction appelée lors du clic sur le bouton "Generate"
     def on_btnGenerate_click(self):
         self.usingDematel()
         self.createInputValuesAndResaulsFrames()     
         self.createTabs() 
 
     def on_btnGenerateFuzzy_click(self):
         self.usingFuzzyDematel()
```

### Comparing `pydematel-0.1.0/pyDEMATEL/Fuzzy_DEMATEL_Solver.py` & `pydematel-0.1.1/pyDEMATEL/Fuzzy_DEMATEL_Solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         self.numberOfFactors=nb
     def getNumberOfFactors(self):
         return self.numberOfFactors  
 
     
     def getMatrix(self):
         return self.matrix
+    def AddMatrix(self, matrix):
+        self.matrix.append(matrix)       
     def setMatrix(self, matrices):
         self.matrix=matrices
     def setExperts(self, experts):
             self.experts=experts
     def getExperts(self):
         return self.experts            
     def addExpert(self, expert):
```

### Comparing `pydematel-0.1.0/pyDEMATEL.egg-info/PKG-INFO` & `pydematel-0.1.1/pyDEMATEL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDEMATEL
-Version: 0.1.0
+Version: 0.1.1
 Summary: pyDematel a python-based tool implementing the Dematel and fuzzy Dematel methods for improved decision making
 Home-page: https://github.com/achekry/-Elsevier-SoftwareX-pyDEMATEL
 Author: Abderrahman CHEKRY, Jamal Bakkas, Mohamed Hanine
 Author-email: a.chekry@uca.ac.ma
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydematel-0.1.0/setup.py` & `pydematel-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyDEMATEL",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[],  # Liste des dépendances
     author="Abderrahman CHEKRY, Jamal Bakkas, Mohamed Hanine",
     author_email="a.chekry@uca.ac.ma",
     description="pyDematel a python-based tool implementing the Dematel and fuzzy Dematel methods for improved decision making",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

