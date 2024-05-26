# Comparing `tmp/atlantic-1.1.5-py3-none-any.whl.zip` & `tmp/atlantic-1.1.50-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,23 @@
-Zip file size: 19288 bytes, number of entries: 13
+Zip file size: 28946 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 atlantic/__init__.py
--rw-rw-rw-  2.0 fat     5195 b- defN 23-Nov-05 00:48 atlantic/analysis.py
--rw-rw-rw-  2.0 fat    11817 b- defN 23-Nov-05 01:11 atlantic/evaluation.py
--rw-rw-rw-  2.0 fat     6233 b- defN 23-Oct-30 16:55 atlantic/imputation.py
--rw-rw-rw-  2.0 fat    11180 b- defN 23-Nov-05 01:09 atlantic/pattern.py
--rw-rw-rw-  2.0 fat     6181 b- defN 23-Nov-05 01:09 atlantic/pipeline.py
--rw-rw-rw-  2.0 fat     8271 b- defN 23-Oct-30 02:04 atlantic/processing.py
--rw-rw-rw-  2.0 fat     5230 b- defN 23-Nov-05 01:08 atlantic/selector.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Nov-05 01:18 atlantic-1.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    12367 b- defN 23-Nov-05 01:18 atlantic-1.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Nov-05 01:18 atlantic-1.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Nov-05 01:18 atlantic-1.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1011 b- defN 23-Nov-05 01:18 atlantic-1.1.5.dist-info/RECORD
-13 files, 68666 bytes uncompressed, 17620 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat    11495 b- defN 24-May-26 21:41 atlantic/pipeline.py
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 atlantic/feature_selection/__init__.py
+-rw-rw-rw-  2.0 fat    10030 b- defN 24-May-26 21:38 atlantic/feature_selection/selector.py
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 atlantic/imputers/__init__.py
+-rw-rw-rw-  2.0 fat     5255 b- defN 24-May-26 21:30 atlantic/imputers/imputation.py
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 atlantic/optimizer/__init__.py
+-rw-rw-rw-  2.0 fat    10379 b- defN 24-May-26 21:39 atlantic/optimizer/evaluation.py
+-rw-rw-rw-  2.0 fat     1860 b- defN 24-May-26 21:30 atlantic/optimizer/metrics.py
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 atlantic/processing/__init__.py
+-rw-rw-rw-  2.0 fat     8950 b- defN 24-May-26 21:30 atlantic/processing/analysis.py
+-rw-rw-rw-  2.0 fat    10768 b- defN 24-May-26 21:30 atlantic/processing/encoders.py
+-rw-rw-rw-  2.0 fat     8703 b- defN 24-May-26 21:30 atlantic/processing/scalers.py
+-rw-rw-rw-  2.0 fat     9610 b- defN 24-May-26 21:40 atlantic/processing/versions.py
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 atlantic/scheme/__init__.py
+-rw-rw-rw-  2.0 fat    13446 b- defN 24-May-26 21:40 atlantic/scheme/pattern.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-May-26 21:43 atlantic-1.1.50.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    12938 b- defN 24-May-26 21:43 atlantic-1.1.50.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-26 21:43 atlantic-1.1.50.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-26 21:43 atlantic-1.1.50.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1769 b- defN 24-May-26 21:43 atlantic-1.1.50.dist-info/RECORD
+21 files, 106394 bytes uncompressed, 26042 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,40 +1,64 @@
 Filename: atlantic/__init__.py
 Comment: 
 
-Filename: atlantic/analysis.py
+Filename: atlantic/pipeline.py
 Comment: 
 
-Filename: atlantic/evaluation.py
+Filename: atlantic/feature_selection/__init__.py
 Comment: 
 
-Filename: atlantic/imputation.py
+Filename: atlantic/feature_selection/selector.py
 Comment: 
 
-Filename: atlantic/pattern.py
+Filename: atlantic/imputers/__init__.py
 Comment: 
 
-Filename: atlantic/pipeline.py
+Filename: atlantic/imputers/imputation.py
+Comment: 
+
+Filename: atlantic/optimizer/__init__.py
+Comment: 
+
+Filename: atlantic/optimizer/evaluation.py
+Comment: 
+
+Filename: atlantic/optimizer/metrics.py
+Comment: 
+
+Filename: atlantic/processing/__init__.py
+Comment: 
+
+Filename: atlantic/processing/analysis.py
+Comment: 
+
+Filename: atlantic/processing/encoders.py
+Comment: 
+
+Filename: atlantic/processing/scalers.py
+Comment: 
+
+Filename: atlantic/processing/versions.py
 Comment: 
 
-Filename: atlantic/processing.py
+Filename: atlantic/scheme/__init__.py
 Comment: 
 
-Filename: atlantic/selector.py
+Filename: atlantic/scheme/pattern.py
 Comment: 
 
-Filename: atlantic-1.1.5.dist-info/LICENSE
+Filename: atlantic-1.1.50.dist-info/LICENSE
 Comment: 
 
-Filename: atlantic-1.1.5.dist-info/METADATA
+Filename: atlantic-1.1.50.dist-info/METADATA
 Comment: 
 
-Filename: atlantic-1.1.5.dist-info/WHEEL
+Filename: atlantic-1.1.50.dist-info/WHEEL
 Comment: 
 
-Filename: atlantic-1.1.5.dist-info/top_level.txt
+Filename: atlantic-1.1.50.dist-info/top_level.txt
 Comment: 
 
-Filename: atlantic-1.1.5.dist-info/RECORD
+Filename: atlantic-1.1.50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atlantic/pipeline.py

```diff
@@ -1,138 +1,278 @@
 import pandas as pd
-from atlantic.processing import AutoMinMaxScaler, AutoStandardScaler, AutoLabelEncoder, AutoIdfEncoder, Encoding_Version
-from atlantic.imputation import AutoSimpleImputer, AutoKNNImputer, AutoIterativeImputer
-from atlantic.analysis import Analysis
-from atlantic.selector import Selector
-from atlantic.pattern import Pattern
+from atlantic.processing.analysis import Analysis 
+from atlantic.processing.scalers import (AutoMinMaxScaler,
+                                         AutoStandardScaler,
+                                         AutoRobustScaler) 
+from atlantic.processing.encoders import (AutoLabelEncoder,
+                                          AutoIdfEncoder,
+                                          AutoOneHotEncoder) 
+from atlantic.processing.versions import Encoding_Version
+from atlantic.imputers.imputation import (AutoSimpleImputer,
+                                          AutoKNNImputer,
+                                          AutoIterativeImputer) 
+from atlantic.feature_selection.selector import Selector 
+from atlantic.scheme.pattern import Pattern 
 
-class ATLpipeline(Selector):
+class Atlantic(Selector):
+    """
+    The Atlantic class  provides comprehensive data preprocessing capabilities including feature engineering, feature selection, 
+    encoding, imputation, and transformation. It is designed to handle both classification and regression tasks
+    by automating the selection of optimal preprocessing strategies.
+
+    Attributes
+    ----------
+    X : pd.DataFrame
+        The input dataset to be processed.
+    target : str
+        The name of the target variable in the dataset.
+    enc_method : str
+        Selected encoding method.
+    imp_method : str
+        Selected imputation method.
+    encoder : object
+        Fitted encoder object.
+    scaler : object
+        Fitted scaler object.
+    imputer : object
+        Fitted imputer object.
+    n_cols : list
+        List of numerical columns.
+    c_cols : list
+        List of categorical columns.
+    cols : list
+        List of selected columns after preprocessing.
+    h2o_feature_importance : list
+        List of feature importances obtained from H2O feature selection.
+
+    Methods
+    -------
+    fit_processing(split_ratio, relevance=0.99, h2o_fs_models=7, encoding_fs=True, vif_ratio=10.0):
+        Fits the preprocessing steps on the input dataset.
+    data_processing(X):
+        Applies the fitted preprocessing steps to a new dataset.
+    """
     def __init__(self,
-                 X:pd.DataFrame=None,
-                 target:str=None):
+                 X : pd.DataFrame = None,
+                 target : str = None):
         super().__init__(X, target)
-        self.enc_method=None
-        self.imp_method=None
-        self.encoder=None
-        self.scaler=None
-        self.imputer=None
-        self.n_cols=None
-        self.c_cols=None
-        self.cols=None
-        self.h2o_feature_importance=None
+        self.enc_method = None
+        self.imp_method = None
+        self.encoder = None
+        self.scaler = None
+        self.imputer = None
+        self.n_cols = None
+        self.c_cols = None
+        self.cols = None
+        self.h2o_feature_importance = None
+        """
+        Initialize the Atlantic class with the input dataset and target variable.
+
+        Parameters
+        ----------
+        X : pd.DataFrame, optional
+            The input dataset to be processed, by default None.
+        target : str, optional
+            The name of the target variable, by default None.
+        """
 
     def fit_processing(self,
-                       split_ratio:float,
-                       relevance:float=0.99,
-                       h2o_fs_models:int=7,
-                       encoding_fs:bool=True,
-                       vif_ratio:float=10.0):
-    
-    ### Data Treatment
-        if self.pred_type=='Class': self.X[self.target]=self.X[self.target].astype(str)
+                       split_ratio : float,
+                       relevance : float = 0.99,
+                       h2o_fs_models : int = 7,
+                       encoding_fs : bool = True,
+                       vif_ratio : float = 10.0):
+        """
+        Fit the preprocessing steps on the input dataset.
+
+        This method performs a series of preprocessing steps including feature engineering, feature selection,
+        encoding method selection, imputation method selection, and VIF-based feature selection. The method
+        updates the attributes of the class with the fitted preprocessing objects and selected columns.
+
+        Parameters
+        ----------
+        split_ratio : float
+            The ratio for splitting the dataset into training and testing sets.
+        relevance : float, optional
+            The relevance threshold for H2O feature selection, by default 0.99.
+        h2o_fs_models : int, optional
+            The number of models to use for H2O feature selection, by default 7.
+        encoding_fs : bool, optional
+            Whether to use encoding during feature selection, by default True.
+        vif_ratio : float, optional
+            The VIF threshold for feature selection, by default 10.0.
+
+        Returns
+        -------
+        self
+            The fitted Atlantic object.
+        """
+        ### Data Treatment
+        if self.pred_type == 'Class':
+            self.X[self.target] = self.X[self.target].astype(str)
             
         X_ = self.X.copy()
-
-        X_ = super().remove_columns_by_nulls(X=X_,percentage=99.9)
         
-        X_ = X_[[col for col in X_.columns if col != self.target] + [self.target]] # target to last index
+        X_ = super().engin_date(X = X_, drop = True)
+        X_ = super().remove_columns_by_nulls(X = X_, percentage=99.9)
+        
+        X_ = X_.drop(columns=[col for col in X_.columns 
+                              if (X_[col].nunique() == len(X_) or X_[col].nunique() == 1) 
+                                                               and col != self.target])  
+        X_ = X_[[col for col in X_.columns if col != self.target] + [self.target]]       
         
-        X_ = super().engin_date(X=X_, drop=True)
-        dataset=X_.copy()
+        data = X_.copy()
         
-        train, test = super().split_dataset(X=X_,split_ratio=split_ratio)
+        train, test = super().split_dataset(X = X_, split_ratio = split_ratio)
         train, test = train.reset_index(drop=True), test.reset_index(drop=True)
         
-    ### Feature Selection 
-        fs=Selector(X=train,target=self.target)
-        sel_cols, self.h2o_feature_importance=fs.feature_selection_h2o(relevance=relevance,
-                                                                       h2o_fs_models=h2o_fs_models,
-                                                                       encoding_fs=encoding_fs)
-        train, test = train[sel_cols], test[sel_cols]
-    #### Encoding Method Selection    
-        pat=Pattern(train=train,test=test,target=self.target)          
-        self.enc_method,perf_ = pat.encoding_selection(),pat.perf
+        ### Feature Selection 
+        if relevance!=1:
+            fs = Selector(X = train, 
+                          target = self.target)
+            sel_cols, self.h2o_feature_importance = fs.feature_selection_h2o(relevance = relevance,
+                                                                             h2o_fs_models = h2o_fs_models,
+                                                                             encoding_fs = encoding_fs)
+            
+            train, test = train[sel_cols], test[sel_cols]
+            
+        #### Encoding Method Selection    
+        ptn = Pattern(train = train,
+                      test = test,
+                      target = self.target)          
+        self.enc_method, perf_ = ptn.encoding_selection(), ptn.perf
         
-    ### Null Imputation Selection 
+        ### Null Imputation Selection 
         if (train.isnull().sum().sum() or test.isnull().sum().sum()) != 0:
-            train, test = pat.imputation_selection()
-            self.imp_method,perf_=pat.imp_method,pat.perf
+            train, test = ptn.imputation_selection()
+            self.imp_method, perf_ = ptn.imp_method, ptn.perf
         else:
             self.imp_method='Undefined'
-            ev = Encoding_Version(train=train, test=test, target=self.target)
-            if self.enc_method=='Encoding Version 1':
-                train, test=ev.encoding_v1()
-            elif self.enc_method=='Encoding Version 2':
-                train, test=ev.encoding_v2()
-            elif self.enc_method=='Encoding Version 3':
-                train, test=ev.encoding_v3()
-            elif self.enc_method=='Encoding Version 4':
-                train, test=ev.encoding_v4()
+            ev = Encoding_Version(train = train,
+                                  test = test,
+                                  target = self.target)
+            if self.enc_method == 'Encoding Version 1':
+                train, test = ev.encoding_v1()
+            elif self.enc_method == 'Encoding Version 2':
+                train, test = ev.encoding_v2()
+            elif self.enc_method == 'Encoding Version 3':
+                train, test = ev.encoding_v3()
+            elif self.enc_method == 'Encoding Version 4':
+                train, test = ev.encoding_v4()
             print('There are no missing values in the Dataset')  
 
-    ### Variance Inflation Factor (VIF) Application 
-        train, test = Pattern(train=train,test=test,target=self.target).vif_performance(vif_threshold=vif_ratio,perf_=perf_)
-        self.cols=list(train.columns)
+        ### Variance Inflation Factor (VIF) Application 
+        train, test = Pattern(train = train,
+                              test = test,
+                              target = self.target).vif_performance(vif_threshold = vif_ratio,
+                                                                    perf_ = perf_)
+        self.cols = list(train.columns)
     
-    ### Fit Processors 
-        dataset=dataset[self.cols]
-        self.n_cols=list(super().num_cols(X=dataset))
-        self.c_cols=list(super().cat_cols(X=dataset))
+        ### Fit Processors 
+        data = data[self.cols]
+        self.n_cols = list(super().num_cols(X=data))
+        self.c_cols = list(super().cat_cols(X=data))
         
         ## Fit Encoding Version
-        if len(self.n_cols)>0:
-            if self.enc_method=='Encoding Version 1' or self.enc_method=='Encoding Version 3':
+        if len(self.n_cols) > 0:
+            
+            if self.enc_method == 'Encoding Version 1' or self.enc_method == 'Encoding Version 3':
                     self.scaler = AutoStandardScaler()
-                    self.scaler.fit(X=dataset[self.n_cols])
-                    dataset[self.n_cols]=self.scaler.transform(X=dataset[self.n_cols])
-            if self.enc_method=='Encoding Version 2' or self.enc_method=='Encoding Version 4':
+                    self.scaler.fit(X = data[self.n_cols])
+                    data[self.n_cols] = self.scaler.transform(X = data[self.n_cols])
+                    
+            if self.enc_method == 'Encoding Version 2' or self.enc_method == 'Encoding Version 4':
                     self.scaler = AutoMinMaxScaler()
-                    self.scaler.fit(X=dataset[self.n_cols])
-                    dataset[self.n_cols]=self.scaler.transform(X=dataset[self.n_cols])
-        if len(self.c_cols)>0:
-            if self.enc_method=='Encoding Version 1' or self.enc_method=='Encoding Version 2':
+                    self.scaler.fit(X=data[self.n_cols])
+                    data[self.n_cols] = self.scaler.transform(X = data[self.n_cols])
+                    
+        if len(self.c_cols) > 0:
+            
+            if self.enc_method == 'Encoding Version 1' or self.enc_method == 'Encoding Version 2':
                     self.encoder = AutoIdfEncoder()
-                    self.encoder.fit(dataset[self.c_cols])
-                    dataset=self.encoder.transform(X=dataset)
-            if self.enc_method=='Encoding Version 3' or self.enc_method=='Encoding Version 4':
+                    self.encoder.fit(data[self.c_cols])
+                    data = self.encoder.transform(X = data)
+                    
+            if self.enc_method == 'Encoding Version 3' or self.enc_method == 'Encoding Version 4':
                     self.encoder = AutoLabelEncoder()
-                    self.encoder.fit(dataset[self.c_cols])
-                    dataset=self.encoder.transform(X=dataset)
+                    self.encoder.fit(data[self.c_cols])
+                    data=self.encoder.transform(X = data)
             
         ## Fit Null Imputation
-        if self.imp_method=='Simple':
+        if self.imp_method == 'Simple':
             self.imputer = AutoSimpleImputer(strategy='mean')
-            self.imputer.fit(dataset)  # Fit on DataFrame
+            self.imputer.fit(data)  # Fit on DataFrame
         
-        elif self.imp_method=='KNN':
+        elif self.imp_method == 'KNN':
             self.imputer = AutoKNNImputer(n_neighbors=3,
                                           weights="uniform")
-            self.imputer.fit(dataset)  # Fit on DataFrame
+            self.imputer.fit(data)  # Fit on DataFrame
         
-        elif self.imp_method=='Iterative':
+        elif self.imp_method == 'Iterative':
             self.imputer = AutoIterativeImputer(max_iter=10,
                                                 random_state=42,
                                                 initial_strategy="mean",
                                                 imputation_order="ascending")
-            self.imputer.fit(dataset)  # Fit on DataFrame
+            self.imputer.fit(data)  # Fit on DataFrame
         
         return self
         
-    def data_processing(self,X:pd.DataFrame):
-        
-    ### Transformation Proceedment
-        X_=X.copy()
-        X_=Analysis.engin_date(X_)
-        X_=X_[self.cols]
-        
-        if len(self.n_cols)>0:
-            X_[self.n_cols] = self.scaler.transform(X_[self.n_cols])
-        if len(self.c_cols)>0:
-            X_=self.encoder.transform(X=X_)
-        if self.imp_method != "Undefined" and X_[self.c_cols+self.n_cols].isnull().sum().sum() != 0:
-            X_=self.imputer.transform(X_.copy())
-    
-        return X_
-    
+    def data_processing(self, X : pd.DataFrame):
+        """
+        Apply the fitted preprocessing steps to the loaded dataset.
+
+        This method transforms a new dataset using the preprocessing steps fitted in the `fit_processing` method.
+        It handles date feature engineering, encoding, scaling, and imputation based on the fitted objects and 
+        selected columns.
+
+        Parameters
+        ----------
+        X : pd.DataFrame
+            The new dataset to be processed.
+
+        Returns
+        -------
+        pd.DataFrame
+            The transformed dataset.
+        """
+        ### Transformation Proceedment
+        data = X.copy()
+        data = Analysis.engin_date(X = data,
+                                   drop = True)
+        
+        syntetic_target = False
+        if self.target not in list(data.columns):
+            data[self.target] = 0
+            syntetic_target = True
+        
+        data = data[self.cols]
+        
+        if len(self.n_cols) > 0:
+            data[self.n_cols] = self.scaler.transform(data[self.n_cols])
+        if len(self.c_cols) > 0:
+            data = self.encoder.transform(X = data)
+        if self.imp_method != "Undefined" and data[self.c_cols + self.n_cols].isnull().sum().sum() != 0:
+            data = self.imputer.transform(data.copy())
     
+        if syntetic_target:
+            data = data.drop(self.target, axis=1)
     
+        return data
+
+
+__all__ = [
+    'Analysis',
+    'AutoMinMaxScaler',
+    'AutoStandardScaler',
+    'AutoRobustScaler',
+    'AutoLabelEncoder',
+    'AutoIdfEncoder',
+    'AutoOneHotEncoder',
+    'Encoding_Version',
+    'AutoSimpleImputer',
+    'AutoKNNImputer',
+    'AutoIterativeImputer',
+    'Selector',
+    'Pattern'
+]
+
```

## Comparing `atlantic/evaluation.py` & `atlantic/optimizer/evaluation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,77 @@
 import pandas as pd
-from atlantic.analysis import Analysis
-from sklearn.ensemble import RandomForestRegressor, ExtraTreesRegressor, RandomForestClassifier, ExtraTreesClassifier
-from sklearn.metrics import *
+from atlantic.processing.analysis import Analysis
+from atlantic.optimizer.metrics import metrics_classification, metrics_regression
+from sklearn.ensemble import (RandomForestRegressor,
+                              ExtraTreesRegressor,
+                              RandomForestClassifier,
+                              ExtraTreesClassifier)
 import xgboost as xgb
 import optuna
 from tqdm import tqdm
 import warnings
 import logging
 
 class Evaluation(Analysis):
-    def __init__(self, train:pd.DataFrame, test:pd.DataFrame, target:str):
+    def __init__(self, 
+                 train : pd.DataFrame,
+                 test : pd.DataFrame,
+                 target : str):
+        """
+        Performs hyperparameter optimization and model evaluation for both regression and classification tasks.
+        It extends the Analysis class, leveraging its methods for data handling and prediction type identification.
+        
+        The main objective of the Evaluation class is to automate the process of selecting optimal 
+        hyperparameters for different machine learning models using the Optuna optimization framework. 
+        This class supports models such as Random Forest, Extra Trees, and XGBoost, and provides a 
+        systematic approach to evaluating their performance on a given dataset.
+    
+        Methods
+        -------
+        objective(trial, dim: str = "normal"):
+            Defines the objective function for hyperparameter optimization using Optuna. It configures 
+            the hyperparameters for various models, trains them, and evaluates their performance.
+            
+        auto_evaluate():
+            Automates the evaluation process by determining the appropriate optimization settings based 
+            on the dataset size and dimensions. It orchestrates the optimization trials and aggregates 
+            the evaluation metrics for comparison.
+        """
         # Constructor for the Evaluation class, inherits from Analysis and initializes class attributes.
         super().__init__(target)
-        self.train=train
-        self.test=test
-        self.metrics=None
-        self._tmetrics=None
-        self.hparameters_list,self.metrics_list=[],[]
-        self.pred_type,self.eval_metric=super().target_type(X=train)
-                
-    def objective(self,trial,dim:str="normal"): 
+        self.train = train
+        self.test = test
+        self.metrics = None
+        self._tmetrics = None
+        self.hparameters_list, self.metrics_list = [], []
+        self.pred_type, self.eval_metric = super().target_type(X = train)
+                
+    def objective(self,
+                  trial,
+                  dim : str = "normal"): 
+        """
+        Defines the objective function for hyperparameter optimization using Optuna.
+        
+        This method configures the hyperparameters for RandomForest, ExtraTrees, and XGBoost models 
+        for both regression and classification tasks. It trains these models on the training set and 
+        evaluates their performance on the test set using appropriate metrics. The results of each 
+        trial are stored for further analysis and comparison.
+
+        Parameters:
+        - trial: optuna.trial.Trial
+            An Optuna trial object used to suggest hyperparameter values.
+        - dim: str, optional (default = "normal")
+            A string indicating the dimensionality setting for the models, which can affect the 
+            hyperparameter configuration.
+
+        Returns:
+        - None
+        """
         
-        X_train,X_test,y_train,y_test=super().divide_dfs(self.train,self.test)
+        X_train, X_test, y_train, y_test = super().divide_dfs(self.train,self.test)
         
         # Configure logging to suppress Optuna's logs
         logging.getLogger('optuna').setLevel(logging.CRITICAL)
         
         # Define the regression and classification models
         rf_regressor = RandomForestRegressor()
         et_regressor = ExtraTreesRegressor()
@@ -35,200 +81,136 @@
         et_classifier = ExtraTreesClassifier()
         xgb_classifier = xgb.XGBClassifier()
             
         # Define hyperparameters for Random Forest regression
         rf_regressor_params = {
             "n_estimators": trial.suggest_int("rf_regressor_n_estimators", 50, 200),
             "max_depth": trial.suggest_int("rf_regressor_max_depth", 5, 32),
-            "min_samples_split": trial.suggest_int("rf_regressor_min_samples_split", 2, 20),
+            "min_samples_split": trial.suggest_int("rf_regressor_min_samples_split", 2, 25),
         }
         
         # Define hyperparameters for Random Forest classification
         rf_classifier_params = {
-            "n_estimators": trial.suggest_int("rf_classifier_n_estimators", 50, 200),
+            "n_estimators": trial.suggest_int("rf_classifier_n_estimators", 60, 250),
             "max_depth": trial.suggest_int("rf_classifier_max_depth", 10, 50),
             "min_samples_split": trial.suggest_int("rf_classifier_min_samples_split", 2, 20),
         }
         
         # Define hyperparameters for Extra Trees regression
         et_regressor_params = {
             "n_estimators": trial.suggest_int("et_regressor_n_estimators", 50, 200),
             "max_depth": trial.suggest_int("et_regressor_max_depth", 5, 32),
-            "min_samples_split": trial.suggest_int("et_regressor_min_samples_split", 2, 20),
+            "min_samples_split": trial.suggest_int("et_regressor_min_samples_split", 2, 25),
         }
         
         # Define hyperparameters for Extra Trees classification
         et_classifier_params = {
-            "n_estimators": trial.suggest_int("et_classifier_n_estimators", 50, 200),
+            "n_estimators": trial.suggest_int("et_classifier_n_estimators", 60, 250),
             "max_depth": trial.suggest_int("et_classifier_max_depth", 10, 50),
             "min_samples_split": trial.suggest_int("et_classifier_min_samples_split", 2, 20),
             }
         
         # Define hyperparameters for XGBoost regression
         xgb_regressor_params = {
             "n_estimators": trial.suggest_int("xgb_regressor_n_estimators", 50, 200),
-            "max_depth": trial.suggest_int("xgb_regressor_max_depth", 5, 10),
+            "max_depth": trial.suggest_int("xgb_regressor_max_depth", 5, 25),
             "learning_rate": trial.suggest_loguniform("xgb_regressor_learning_rate", 0.01, 0.1),
         }
         
         # Define hyperparameters for XGBoost classification
         xgb_classifier_params = {
-            "n_estimators": trial.suggest_int("xgb_classifier_n_estimators", 50, 200),
+            "n_estimators": trial.suggest_int("xgb_classifier_n_estimators", 60, 250),
             "max_depth": trial.suggest_int("xgb_classifier_max_depth", 10, 20),
             "learning_rate": trial.suggest_loguniform("xgb_classifier_learning_rate", 0.05, 0.1),  
         }
         
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
                     
-            if self.pred_type=="Reg":
-                # Initialize the regression models with the suggested hyperparameters
-                rf_regressor.set_params(**rf_regressor_params)
-                if dim!="high":et_regressor.set_params(**et_regressor_params)
-                xgb_regressor.set_params(**xgb_regressor_params)
-                
-                # Train the regression models on the training data
-                rf_regressor.fit(X_train, y_train)
-                if dim!="high":et_regressor.fit(X_train, y_train)
-                xgb_regressor.fit(X_train, y_train)
-                
-                # Make predictions on the test data for regression models
-                rf_r_preds = rf_regressor.predict(X_test)
-                if dim!="high":et_r_preds = et_regressor.predict(X_test)
-                xgb_r_preds = xgb_regressor.predict(X_test)
-                
-                m_reg=pd.DataFrame()
-                m_rf=pd.DataFrame(self.metrics_regression(y_test,rf_r_preds),index=[0])
-                if dim!="high":
-                    m_et=pd.DataFrame(self.metrics_regression(y_test,et_r_preds),index=[0])
-                    m_et["Model"]="ExtraTrees"
-                m_xgb=pd.DataFrame(self.metrics_regression(y_test,xgb_r_preds),index=[0])
-                m_rf["Model"],m_xgb["Model"]="RandomForest","XGBoost"
-                if dim!="high":m_reg=pd.concat([m_rf,m_et,m_xgb])
-                elif dim=="high":m_reg=pd.concat([m_rf,m_xgb])
-                m_reg["iteration"]=len(self.metrics_list) + 1
-                self.metrics_list.append(m_reg)
-                
-                self.hparameters_list.append({
-                    "rf_regressor_params": rf_regressor_params,
-                    "et_regressor_params": et_regressor_params,
-                    "xgb_regressor_params": xgb_regressor_params,
-                    "iteration": len(self.metrics_list) + 1,
-                })
-                
-            elif self.pred_type=="Class":
-                # Initialize the classification model with the suggested hyperparameters
-                rf_classifier.set_params(**rf_classifier_params)
-                if dim!="high":et_classifier.set_params(**et_classifier_params)
-                xgb_classifier.set_params(**xgb_classifier_params)
-                
-                # Train the classification model on the training data
-                rf_classifier.fit(X_train, y_train)
-                if dim!="high":et_classifier.fit(X_train, y_train)
-                xgb_classifier.fit(X_train, y_train)
-
-                # Make predictions on the test data for classification model
-                rf_c_preds = rf_classifier.predict(X_test)
-                if dim!="high":et_c_preds = et_classifier.predict(X_test)
-                xgb_c_preds = xgb_classifier.predict(X_test)
-                
-                m_class=pd.DataFrame()
-                m_rf=pd.DataFrame(self.metrics_classification(y_test,rf_c_preds),index=[0])
-                if dim!="high":
-                    m_et=pd.DataFrame(self.metrics_classification(y_test,et_c_preds),index=[0])
-                    m_et["Model"]="ExtraTrees"
-                m_xgb=pd.DataFrame(self.metrics_classification(y_test,xgb_c_preds),index=[0])
-                m_rf["Model"],m_xgb["Model"]="RandomForest","XGBoost"
-                if dim!="high":m_class=pd.concat([m_rf,m_et,m_xgb])
-                elif dim=="high":m_class=pd.concat([m_rf,m_xgb])
-                m_class["iteration"]=len(self.metrics_list)+1
-                self.metrics_list.append(m_class)
-                
-                self.hparameters_list.append({
-                    "rf_classifier_params": rf_classifier_params,
-                    "et_classifier_params": et_classifier_params,
-                    "xgb_classifier_params": xgb_classifier_params,
-                    "iteration": len(self.metrics_list)+1,
-                    })
-        
+            if self.pred_type in ["Reg", "Class"]:
+                # Define models and parameters
+                models = [rf_regressor, et_regressor, xgb_regressor] if self.pred_type == "Reg" else [rf_classifier, et_classifier, xgb_classifier]
+                params = [rf_regressor_params, et_regressor_params, xgb_regressor_params] if self.pred_type == "Reg" else [rf_classifier_params, et_classifier_params, xgb_classifier_params]
+                metrics_func = metrics_regression if self.pred_type == "Reg" else metrics_classification
+            
+                # Train models
+                for model, param in zip(models, params):
+                    if dim != "high" or model != et_regressor:
+                        model.set_params(**param)
+                        model.fit(X_train, y_train)
+            
+                # Make predictions
+                preds = [model.predict(X_test) if dim != "high" or model != et_regressor else None for model in models]
+            
+                # Calculate metrics
+                metrics = [metrics_func(y_test, pred) if pred is not None else None for pred in preds]
+            
+                # Concatenate metrics
+                m_df = pd.concat([m for m in metrics if m is not None])
+            
+                # Set model names
+                m_df["Model"] = ["RandomForest", "ExtraTrees", "XGBoost"] if dim != "high" else ["RandomForest", "XGBoost"]
+            
+                # Set iteration
+                m_df["iteration"] = len(self.metrics_list) + 1
+            
+                # Append to metrics list
+                self.metrics_list.append(m_df)
+            
+                # Append hyperparameters
+                hparams = {}
+                for model_name, param in zip(["rf", "et", "xgb"], params):
+                    hparams[model_name + "_" + self.pred_type.lower() + "_params"] = param
+                hparams["iteration"] = len(self.metrics_list) + 1
+                self.hparameters_list.append(hparams)
+    
     def auto_evaluate(self):
-        
+        """
+        Automates the evaluation process by determining the appropriate optimization settings based 
+        on the dataset size and dimensions.
+        
+        This method orchestrates the optimization trials using Optuna, dynamically adjusting the 
+        number of trials and dimensionality settings based on the characteristics of the dataset. 
+        It aggregates the evaluation metrics from all trials and identifies the best-performing models.
+
+        Returns:
+        - metrics: pd.DataFrame
+            A DataFrame containing the aggregated evaluation metrics for the best-performing models.
+        """
         optuna.logging.set_verbosity(optuna.logging.WARNING)
         
-        if len(self.train) <= 8000 and len(list(self.train.columns)) < 30: dim_, n_trials = "low", 8
-        elif len(self.train) <= 8000 and len(list(self.train.columns)) >= 30: dim_, n_trials = "medium", 6
-        elif len(self.train) > 8000 and len(list(self.train.columns)) < 30: dim_, n_trials = "mid_high", 5
-        elif len(self.train) > 8000 and len(list(self.train.columns)) >= 30: dim_, n_trials = "high", 5 # & Reduced Model Ensembles
-    
-        if self.pred_type=="Reg":
-            # Create an Optuna study
-            reg_study = optuna.create_study(direction="minimize", study_name="Reg Evaluation")
-            # Optimize the objective function with tqdm progress bar
-            with tqdm(total=n_trials, desc="",ncols=75) as pbar:
-                def trial_callback(study, trial):
-                    pbar.update(1)
-                reg_study.optimize(lambda trial: self.objective(trial,dim=dim_),
-                                   n_trials=n_trials,
-                                   callbacks=[trial_callback])
-            
-            self.metrics=pd.concat(self.metrics_list)
-            self.metrics=self.metrics.sort_values(["Model","Mean Absolute Error"], ascending=True)
-            self._tmetrics=self.metrics.copy()
-            self.metrics=self.metrics.groupby("Model").first().mean(axis=0).to_frame().T
-            del self.metrics['iteration']
-            
-        elif self.pred_type=="Class":
-            # Create an Optuna study for classification
-            class_study = optuna.create_study(direction="maximize", study_name="Class Evaluation")
-            # Optimize the objective function with tqdm progress bar
-            with tqdm(total=n_trials, desc="",ncols=75) as pbar:
-                def trial_callback(study, trial):
-                    pbar.update(1)
-                class_study.optimize(lambda trial: self.objective(trial,dim=dim_),
-                                     n_trials=n_trials,
-                                     callbacks=[trial_callback])
-                
-            self.metrics=pd.concat(self.metrics_list)
-            self.metrics=self.metrics.sort_values(["Model","Accuracy"], ascending=False)
-            self._tmetrics=self.metrics.copy()
-            self.metrics=self.metrics.groupby("Model").first().mean(axis=0).to_frame().T
-            del self.metrics['iteration']
-        
-        return self.metrics 
-    
-    @staticmethod
-    def metrics_regression(y_true, y_pred):
-        # Calculate various regression model evaluation metrics.
-        mae=mean_absolute_error(y_true, y_pred)
-        mape=mean_absolute_percentage_error(y_true, y_pred)
-        mse=mean_squared_error(y_true, y_pred)
-        evs=explained_variance_score(y_true, y_pred)
-        maximo_error=max_error(y_true, y_pred)
-        r2=r2_score(y_true, y_pred)
-        metrics_reg= {'Mean Absolute Error': mae,
-                      'Mean Absolute Percentage Error': mape,
-                      'Mean Squared Error': mse,
-                      'Explained Variance Score': evs,
-                      'Max Error': maximo_error,
-                      'R2 Score':r2}
-        
-        return metrics_reg
-    
-    @staticmethod
-    def metrics_classification(y_true, y_pred):
-        # Calculate various classification model evaluation metrics.
-        accuracy_metric=accuracy_score(y_true, y_pred)
-        precision_metric=precision_score(y_true, y_pred,average='micro')
-        f1_macro_metric=f1_score(y_true, y_pred,average='macro')
-        recall_score_metric=recall_score(y_true, y_pred, average='macro')
-        
-        metrics_class={'Accuracy': accuracy_metric,
-                       'Precision Micro': precision_metric,
-                       'F1 Score Macro':f1_macro_metric,
-                       'Recall Score Macro':recall_score_metric}
+        train_len, train_cols = self.train.shape[0], self.train.shape[1]
         
-        return metrics_class
+        if train_len <= 8000:
+            dim_, n_trials = ("low", 8) if train_cols < 30 else ("medium", 6)
+        else:
+            dim_, n_trials = ("mid_high", 5) if train_cols < 30 else ("high", 5)
+    
+        study_params = {
+            "direction": "minimize" if self.pred_type == "Reg" else "maximize",
+            "study_name": f"{self.pred_type} Evaluation"
+        }
+    
+        study = optuna.create_study(**study_params)
+    
+        with tqdm(total = n_trials, desc = "", ncols = 75) as pbar:
+            def trial_callback(study, trial):
+                pbar.update(1)
+    
+            study.optimize(lambda trial: self.objective(trial, dim = dim_), 
+                           n_trials = n_trials, 
+                           callbacks = [trial_callback])
+    
+        self.metrics = pd.concat(self.metrics_list)
+        sort_col = "Mean Absolute Error" if self.pred_type == "Reg" else "Accuracy"
+        self.metrics = self.metrics.sort_values(["Model", sort_col], ascending=self.pred_type == "Reg")
+        self._tmetrics = self.metrics.copy()
+        self.metrics = self.metrics.groupby("Model").first().mean(axis=0).to_frame().T
+        self.metrics.drop(columns = 'iteration', inplace=True)
+        
+        return self.metrics
+
```

## Comparing `atlantic/imputation.py` & `atlantic/imputers/imputation.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import pandas as pd
 from sklearn.experimental import enable_iterative_imputer
 from sklearn.impute import SimpleImputer, KNNImputer, IterativeImputer
 from sklearn.base import TransformerMixin
 
 class AutoSimpleImputer(TransformerMixin):
     def __init__(self, 
-                 strategy:str='mean', # {"mean", "median", "most_frequent", "constant"}
-                 target:str=None):
+                 strategy : str = 'mean', # {"mean", "median", "most_frequent", "constant"}
+                 target : str = None):
         self.strategy = strategy 
         self.target = target
         self.imputer = None
         self.numeric_columns = None  # Store the numeric columns here
 
     def fit(self, X, y=None):
         if self.target is not None:
@@ -34,41 +34,32 @@
         imputed_numeric = self.imputer.transform(X[self.numeric_columns])
         
         # Update the original DataFrame with imputed values
         X[self.numeric_columns] = imputed_numeric
         
         return X
     
-    def inverse_transform(self, X):
-        
-        if self.imputer is None:
-            raise ValueError("You must call 'fit' first to initialize the imputer.")
-        
-        # Reverse the imputation on numeric columns
-        X[self.numeric_columns] = self.imputer.inverse_transform(X[self.numeric_columns])
-    
-        return X
-    
     def impute(self,train:pd.DataFrame, test:pd.DataFrame, strategy:str="mean"):
         if strategy is not None:
             self.strategy = strategy  # Update the strategy if provided
         
         # Fit the AutoSimpleImputer instance on the training data
         self.fit(train)
         
         # Transform both the train and test data using the fitted imputer
         train = self.transform(train.copy())
         test = self.transform(test.copy())
         
         return train, test
 
 class AutoKNNImputer(TransformerMixin):
-    def __init__(self, n_neighbors:int=5,
-                 weights:str="uniform", #{"uniform", "distance"}
-                 target:str=None):
+    def __init__(self, 
+                 n_neighbors : int = 5,
+                 weights : str = "uniform", #{"uniform", "distance"}
+                 target : str = None):
         self.n_neighbors = n_neighbors
         self.weights = weights
         self.target = target
         self.imputer = None
         self.numeric_columns = None  # Store the numeric columns here
 
     def fit(self, X, y=None):
@@ -91,32 +82,23 @@
         # Transform only the numeric columns using the fitted imputer
         imputed_numeric = self.imputer.transform(X[self.numeric_columns])
         
         # Update the original DataFrame with imputed values
         X[self.numeric_columns] = imputed_numeric
         
         return X
-    
-    def inverse_transform(self, X):
-        
-        if self.imputer is None:
-            raise ValueError("You must call 'fit' first to initialize the imputer.")
-        
-        # Reverse the imputation on numeric columns
-        X[self.numeric_columns] = self.imputer.inverse_transform(X[self.numeric_columns])
-    
-        return X
 
 class AutoIterativeImputer(TransformerMixin):
 
-    def __init__(self, max_iter:int=10, 
-                 random_state:int=None, 
-                 initial_strategy:str="mean", # {"mean", "median", "most_frequent", "constant"}
-                 imputation_order:str="ascending", # {"ascending", "descending", "roman", "arabic", "random"}
-                 target:str=None):
+    def __init__(self,
+                 max_iter : int = 10, 
+                 random_state : int = None, 
+                 initial_strategy : str = "mean", # {"mean", "median", "most_frequent", "constant"}
+                 imputation_order : str = "ascending", # {"ascending", "descending", "roman", "arabic", "random"}
+                 target : str = None):
         self.max_iter = max_iter
         self.random_state = random_state
         self.initial_strategy = initial_strategy
         self.imputation_order = imputation_order
         self.target = target
         self.imputer = None
         self.numeric_columns = None  # Store the numeric columns here
@@ -145,21 +127,10 @@
         imputed_numeric = self.imputer.transform(X[self.numeric_columns])
         
         # Update the original DataFrame with imputed values
         X[self.numeric_columns] = imputed_numeric
         
         return X
     
-    def inverse_transform(self, X):
-        
-        if self.imputer is None:
-            raise ValueError("You must call 'fit' first to initialize the imputer.")
-        
-        # Reverse the imputation on numeric columns
-        X[self.numeric_columns] = self.imputer.inverse_transform(X[self.numeric_columns])
-    
-        return X
-    
-    
-    
     
+
```

## Comparing `atlantic/pattern.py` & `atlantic/scheme/pattern.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,221 +1,295 @@
 import pandas as pd
-from atlantic.evaluation import Evaluation
-from atlantic.imputation import AutoSimpleImputer, AutoKNNImputer, AutoIterativeImputer
-from atlantic.processing import Encoding_Version
-from atlantic.selector import Selector
+from atlantic.processing.versions import Encoding_Version 
+from atlantic.imputers.imputation import AutoSimpleImputer, AutoKNNImputer, AutoIterativeImputer 
+from atlantic.optimizer.evaluation import Evaluation 
+from atlantic.feature_selection.selector import Selector 
+from tqdm import tqdm
 
 class Pattern(Evaluation):
-    def __init__(self, train:pd.DataFrame, test:pd.DataFrame, target:str):
+    def __init__(self, 
+                 train : pd.DataFrame, 
+                 test : pd.DataFrame, 
+                 target : str):
         super().__init__(train,test,target)
-        self.enc_method=None
-        self.imp_method=None
-        self._imputer=None
-        self.perf=None
-        
+        self.enc_method = None
+        self.imp_method = None
+        self._imputer = None
+        self.perf = None
+        """
+        Provides a sequentially optimized application of methods for selecting optimal encoding and imputation strategies, 
+        as well as performing feature selection based on Variance Inflation Factor (VIF).
+    
+        Attributes
+        ----------
+        train : pd.DataFrame
+            Training dataset.
+        test : pd.DataFrame
+            Testing dataset.
+        target : str
+            The target variable name.
+        enc_method : str
+            Selected encoding method.
+        imp_method : str
+            Selected imputation method.
+        _imputer : object
+            Selected imputer object.
+        perf : float
+            Performance metric of the selected encoding or imputation method.
+    
+        Methods
+        -------
+        encoding_selection():
+            Selects the best encoding method based on predictive performance.
+        imputation_selection():
+            Selects the best imputation method based on predictive performance.
+        vif_performance(vif_threshold=10.0, perf_=None):
+            Evaluates the Variance Inflation Factor (VIF) and applies VIF-based feature selection.
+        """
     def encoding_selection(self):
-        # Select the encoding method and assess its performance.
-        
+        """
+        Select the optimal encoding method based on predictive performance.
+
+        This method generates different encoding versions of the training and testing datasets,
+        imputes missing values if necessary, and evaluates the performance of each encoding version.
+        The best-performing encoding method is selected and stored in the `enc_method` attribute.
+
+        Returns
+        -------
+        str
+            The selected encoding method.
+        """
         # Create an Encoding_Version instance and a SimpleImputer instance.
-        ev = Encoding_Version(train=self.train.copy(), test=self.test.copy(), target=self.target)
-        simple_imputer = AutoSimpleImputer(strategy='mean',target=self.target)
+        ev = Encoding_Version(train = self.train.copy(),
+                              test = self.test.copy(),
+                              target = self.target)
+        simple_imputer = AutoSimpleImputer(strategy = 'mean', target = self.target)
         
         # Generate different encoding versions and separate train and test data for each encoding version.
-        ds = [method() for method in [ev.encoding_v1, ev.encoding_v2, ev.encoding_v3, ev.encoding_v4]]
-        (train_v1, test_v1), (train_v2, test_v2), (train_v3, test_v3), (train_v4, test_v4) = [
-            (d[0], d[1]) if len(d) == 2 else (None, None) for i, d in enumerate(ds)]
+        # Initialize the progress bar
+        print('  ')        
+        encoding_versions = [ev.encoding_v1, ev.encoding_v2, ev.encoding_v3, ev.encoding_v4]
+        with tqdm(total=1, desc="Fitting Encoding Versions", ncols=75) as pbar:
+            (train_v1, test_v1), (train_v2, test_v2), (train_v3, test_v3), (train_v4, test_v4) = [method() for method in encoding_versions]
+            pbar.update(1)
             
         # Impute missing values if necessary.
         if (train_v1.isnull().sum().sum() or test_v1.isnull().sum().sum()) != 0:
-            train_v1, test_v1 = simple_imputer.impute(train=train_v1,test=test_v1)
-            
+            train_v1, test_v1 = simple_imputer.impute(train = train_v1,
+                                                      test = test_v1)
+        
         if (train_v2.isnull().sum().sum() or test_v2.isnull().sum().sum()) != 0:
-            train_v2, test_v2 = simple_imputer.impute(train=train_v2,test=test_v2)
+            train_v2, test_v2 = simple_imputer.impute(train = train_v2,
+                                                      test = test_v2)
             
         if (train_v3.isnull().sum().sum() or test_v3.isnull().sum().sum()) != 0:
-            train_v3, test_v3 = simple_imputer.impute(train=train_v3,test=test_v3)
+            train_v3, test_v3 = simple_imputer.impute(train = train_v3,
+                                                      test = test_v3)
             
         if (train_v4.isnull().sum().sum() or test_v4.isnull().sum().sum()) != 0:
-             train_v4, test_v4 = simple_imputer.impute(train=train_v4,test=test_v4)
+             train_v4, test_v4 = simple_imputer.impute(train = train_v4,
+                                                       test = test_v4)
             
         # Perform model evaluation for each encoding version.
         print('    ')
-        print('Encoding Version 1 Loading')
-        p_v1 = Evaluation(train=train_v1,
-                          test=test_v1,
-                          target=self.target).auto_evaluate()[self.eval_metric][0]
-        print('Encoding Version 2 Loading')
-        p_v2 = Evaluation(train=train_v2,
-                          test=test_v2,
-                          target=self.target).auto_evaluate()[self.eval_metric][0]
-        print('Encoding Version 3 Loading')
-        p_v3 = Evaluation(train=train_v3,
-                          test=test_v3,
-                          target=self.target).auto_evaluate()[self.eval_metric][0]
-        print('Encoding Version 4 Loading')
-        p_v4 = Evaluation(train=train_v4,
-                          test=test_v4,
-                          target=self.target).auto_evaluate()[self.eval_metric][0]
-        
-        if self.pred_type=='Reg':
-            print(' ')
-            print('Predictive Performance Encoding Versions:')
-            print('\n MAE Version 1 [IDF + StandardScaler] : ', round(p_v1, 4),
-                  '\n MAE Version 2 [IDF + MinMaxScaler] : ', round(p_v2, 4),
-                  '\n MAE Version 3 [Label + StandardScaler] : ', round(p_v3, 4),
-                  '\n MAE Version 4 [Label + MinMaxScaler] : ', round(p_v4, 4))
-            metric='MAE'
-        elif self.pred_type=='Class':
-            print(' ')
-            print('Predictive Performance Encoding Versions:')
-            print('\n ACC Version 1 [IDF + StandardScaler] : ', round(p_v1, 4),
-                  '\n ACC Version 2 [IDF + MinMaxScaler] : ', round(p_v2, 4),
-                  '\n ACC Version 3 [Label + StandardScaler] : ', round(p_v3, 4),
-                  '\n ACC Version 4 [Label + MinMaxScaler] : ', round(p_v4, 4))
-            metric='ACC'
+        encoding_versions = [
+            (train_v1, test_v1),
+            (train_v2, test_v2),
+            (train_v3, test_v3),
+            (train_v4, test_v4)
+        ]
+        
+        performances = []
+        for i, (train, test) in enumerate(encoding_versions, 1):
+            print(f'Encoding Version {i} Loading')
+            performance = Evaluation(train=train, test=test, target=self.target).auto_evaluate()[self.eval_metric][0]
+            performances.append(performance)
+        
+        p_v1, p_v2, p_v3, p_v4 = performances
+        
+        metric = 'MAE' if self.pred_type == 'Reg' else 'ACC'
+        
+        print('\nPredictive Performance Encoding Versions:')
+        print(f'\n Version 1 [IDF + StandardScaler] : {round(p_v1, 4)}',
+              f'\n Version 2 [IDF + MinMaxScaler] : {round(p_v2, 4)}',
+              f'\n Version 3 [Label + StandardScaler] : {round(p_v3, 4)}',
+              f'\n Version 4 [Label + MinMaxScaler] : {round(p_v4, 4)}')
         
         list_encoding=[p_v1,p_v2,p_v3,p_v4]
-        list_encoding.sort()
-        if self.pred_type=='Class': list_encoding.sort(reverse=True)
+        
+        if self.pred_type == 'Class':
+            list_encoding.sort(reverse=True)
+        else:
+            list_encoding.sort()
         
         # Select the encoding method with the best performance.
-        if list_encoding[0]==p_v1:
-            self.enc_method='Encoding Version 1'
-            print('Encoding Version 1 was choosen with an ', metric, ' of: ', round(p_v1, 4))
-            
-        elif list_encoding[0]==p_v2:
-            self.enc_method='Encoding Version 2'
-            print('Encoding Version 2 was choosen with an ', metric, ' of: ', round(p_v2, 4))    
-            
-        elif list_encoding[0]==p_v3:
-            self.enc_method='Encoding Version 3'
-            print('Encoding Version 3 was choosen with an ', metric, ' of: ', round(p_v3, 4))
-            
-        elif list_encoding[0]==p_v4:
-            self.enc_method='Encoding Version 4'
-            print('Encoding Version 4 was choosen with an ', metric, ' of: ', round(p_v4, 4))
-            print(' ')
-        self.perf=list_encoding[0]
+        if list_encoding[0] == p_v1:
+            self.enc_method = 'Encoding Version 1'
+        elif list_encoding[0] == p_v2:
+            self.enc_method = 'Encoding Version 2'
+        elif list_encoding[0] == p_v3:
+            self.enc_method = 'Encoding Version 3'
+        elif list_encoding[0] == p_v4:
+            self.enc_method = 'Encoding Version 4'  
+        self.perf = list_encoding[0]
+        
+        print(f'{self.enc_method} was choosen with an', metric, 'of: ', round(self.perf, 4))
         
         return self.enc_method
         
     def imputation_selection(self):
-        
+        """
+        Select the optimal imputation method based on predictive performance.
+
+        This method applies the selected encoding method to the training and testing datasets,
+        performs imputation using different imputation strategies, and evaluates their performance.
+        The best-performing imputation method is selected and stored in the `imp_method` attribute.
+
+        Returns
+        -------
+        tuple
+            The imputed training and testing imputated datasets.
+        """
         # Select the imputation method and assess its performance.
-        if self.pred_type=='Reg': metric='MAE' 
-        elif self.pred_type=='Class': metric='ACC'
+        metric = 'MAE' if self.pred_type == 'Reg' else 'ACC'
         
         ev = Encoding_Version(train=self.train.copy(), test=self.test.copy(), target=self.target)
         # Depending on the selected encoding method, apply the corresponding encoding function.
-        if self.enc_method=='Encoding Version 1':
-            self.train, self.test=ev.encoding_v1()
-        elif self.enc_method=='Encoding Version 2':
+        if self.enc_method == 'Encoding Version 1':
+            self.train, self.test = ev.encoding_v1()
+        elif self.enc_method == 'Encoding Version 2':
             self.train, self.test=ev.encoding_v2()
-        elif self.enc_method=='Encoding Version 3':
-            self.train, self.test=ev.encoding_v3()
-        elif self.enc_method=='Encoding Version 4':
-            self.train, self.test=ev.encoding_v4()
-        elif self.enc_method==None:
+        elif self.enc_method == 'Encoding Version 3':
+            self.train, self.test = ev.encoding_v3()
+        elif self.enc_method == 'Encoding Version 4':
+            self.train, self.test = ev.encoding_v4()
+        elif self.enc_method == None:
             print(" No Encoding Version Selected ")
-            self.train, self.test=ev.encoding_v4()
+            self.train, self.test = ev.encoding_v4()
             
         print('    ')
         print('Simple Imputation Loading')
         simple_imputer = AutoSimpleImputer(strategy='mean')
         simple_imputer.fit(self.train)  # Fit on the DataFrame
         train_s = simple_imputer.transform(self.train.copy())  # Transform the Train DataFrame
         test_s = simple_imputer.transform(self.test.copy()) # Transform the Test DataFrame
         
-        p_s = Evaluation(train=train_s,
-                         test=test_s,
-                         target=self.target).auto_evaluate()[self.eval_metric][0]
+        p_s = Evaluation(train = train_s,
+                         test = test_s,
+                         target = self.target).auto_evaluate()[self.eval_metric][0]
         
         print('KNN Imputation Loading')
         knn_imputer = AutoKNNImputer(n_neighbors=3)
         knn_imputer.fit(self.train)  # Fit on the DataFrame
         train_knn = knn_imputer.transform(self.train.copy())  # Transform the Train DataFrame
         test_knn = knn_imputer.transform(self.test.copy()) # Transform the Test DataFrame
         
-        p_knn = Evaluation(train=train_knn,
-                           test=test_knn,
-                           target=self.target).auto_evaluate()[self.eval_metric][0]
+        p_knn = Evaluation(train = train_knn,
+                           test = test_knn,
+                           target = self.target).auto_evaluate()[self.eval_metric][0]
         
         print('Iterative Imputation Loading')
         iter_imputer = AutoIterativeImputer(max_iter=10, random_state=42)
         iter_imputer.fit(self.train)  # Fit on the DataFrame
         train_iter = iter_imputer.transform(self.train.copy())  # Transform the Train DataFrame
         test_iter = iter_imputer.transform(self.test.copy()) # Transform the Test DataFrame
         
-        p_iter = Evaluation(train=train_iter,
-                            test=test_iter,
-                            target=self.target).auto_evaluate()[self.eval_metric][0]
+        p_iter = Evaluation(train = train_iter,
+                            test = test_iter,
+                            target = self.target).auto_evaluate()[self.eval_metric][0]
             
         print('    ')
         print('Predictive Performance Null Imputation Versions:')
         print('    ')
-        print(' KNN Performance: ', round(p_knn, 4), '\n Iterative Performance: ', 
-              round(p_iter, 4),'\n Simple Performance: ', round(p_s, 4))
+        print(' KNN Performance: ', round(p_knn, 4), 
+              '\n Iterative Performance: ', round(p_iter, 4),
+              '\n Simple Performance: ', round(p_s, 4))
         
         list_imp=[p_iter,p_knn,p_s]
         list_imp.sort()
-        if self.pred_type=='Class': list_imp.sort(reverse=True)
+        if self.pred_type == 'Class':
+            list_imp.sort(reverse=True)
         
         # Select the imputation method with the best performance.
-        if list_imp[0]==p_s:
-            self.imp_method='Simple'
-            self.train, self.test,self._imputer=train_s.copy(),test_s.copy(),simple_imputer
-            print('Simple Imputation Algorithm was chosen with an ', metric, ' of: ', round(p_s, 4))
-            
-        elif list_imp[0]==p_knn:
-            self.imp_method='KNN'
-            self.train, self.test,self._imputer=train_knn.copy(), test_knn.copy(),knn_imputer
-            print('KNN Imputation Algorithm was chosen with an ', metric, ' of: ', round(p_knn, 4))
-            
-        elif list_imp[0]==p_iter:
-            self.imp_method='Iterative'
+        if list_imp[0] == p_s:
+            self.imp_method = 'Simple'
+            self.train, self.test, self._imputer = train_s.copy(), test_s.copy(), simple_imputer
+            
+        elif list_imp[0] == p_knn:
+            self.imp_method = 'KNN'
+            self.train, self.test, self._imputer = train_knn.copy(), test_knn.copy(), knn_imputer
+
+        elif list_imp[0] == p_iter:
+            self.imp_method = 'Iterative'
             self.train, self.test,self._imputer=train_iter.copy(),test_iter.copy(),iter_imputer
-            print('Iterative Imputation Algorithm was chosen with an ', metric, ' of: ', round(p_iter, 4))
-        self.perf=list_imp[0]
+
+        self.perf = list_imp[0]
+        print(f'{self.imp_method} Imputation Algorithm was chosen with an', metric, 'of:', round(self.perf, 4))
         
         return self.train, self.test
     
-    def vif_performance(self,vif_threshold:float=10.0,perf_:float=None):
-        # Perform VIF-based feature selection on the train and test data.
-        # Evaluate and compare the performance before and after VIF-based feature selection.
+    def vif_performance(self,
+                        vif_threshold : float = 10.0,
+                        perf_ : float = None):
+        """
+        Evaluate and apply Variance Inflation Factor (VIF) based feature selection.
+
+        This method evaluates the performance before and after applying VIF-based feature selection.
+        It selects features with VIF below the specified threshold and compares performance.
+        If performance improves or remains stable, VIF-based feature selection is applied.
+
+        Parameters
+        ----------
+        vif_threshold : float, optional
+            The threshold for VIF to consider features for selection, by default 10.0.
+        perf_ : float, optional
+            The initial performance metric, by default None.
+
+        Returns
+        -------
+        tuple
+            The training and testing datasets after VIF-based feature selection.
+        """
+
         train_vif, test_vif = self.train.copy(), self.test.copy()
 
-        cols_vif = Selector(X=train_vif,target=self.target).feature_selection_vif(vif_threshold=vif_threshold)
+        cols_vif = Selector(X = train_vif,
+                            target = self.target).feature_selection_vif(vif_threshold = vif_threshold)
         print('    ')
-        print('Number of Selected VIF Columns: ', len(cols_vif),
-              '\nRemoved Columns with VIF :', len(list(train_vif.columns)) - len(cols_vif))
-        
-        train_vif,test_vif = train_vif[cols_vif],test_vif[cols_vif]
+        print('Selected VIF Columns: ', len(cols_vif),
+              '\nRemoved Columns by VIF :', train_vif.shape[1] - len(cols_vif))
         
-        if perf_!=None: self.perf=perf_
-        if self.perf==None:
-            self.perf = Evaluation(train=self.train.copy(),
-                                     test=self.test.copy(),
-                                     target=self.target).auto_evaluate()[self.eval_metric][0]
-            
-        perf_vif = Evaluation(train=train_vif,
-                              test=test_vif,
-                              target=self.target).auto_evaluate()[self.eval_metric][0]
+        train_vif, test_vif = train_vif[cols_vif], test_vif[cols_vif]
+        apply_vif = False
         
-        print('Default Performance:', round(self.perf, 4))
-        print('VIF Performance:', round(perf_vif, 4))
+        if self.train.shape[1] - len(cols_vif) == 0:
+            self.train = self.train[cols_vif]
+            self.test = self.test[cols_vif]
+            
+        else:
+            if perf_ != None: 
+                self.perf = perf_
+            if self.perf == None:
+                self.perf = Evaluation(train = self.train.copy(),
+                                       test = self.test.copy(),
+                                       target = self.target).auto_evaluate()[self.eval_metric][0]
+                
+            perf_vif = Evaluation(train = train_vif,
+                                  test = test_vif,
+                                  target = self.target).auto_evaluate()[self.eval_metric][0]
+            
+            print('Default Performance:', round(self.perf, 4))
+            print('VIF Performance:', round(perf_vif, 4))
     
-        if self.pred_type == 'Reg':
-            if perf_vif < self.perf:
-                print('The VIF filtering method was applied')
-                self.train = self.train[cols_vif]
-                self.test = self.test[cols_vif]
-            else:
-                print('The VIF filtering method was not applied')
-        elif self.pred_type == 'Class':
-            if perf_vif > self.perf:
+            if self.pred_type == 'Reg' and perf_vif < self.perf:
+                apply_vif = True
+            elif self.pred_type == 'Class' and perf_vif > self.perf:
+                apply_vif = True
+            
+            if apply_vif:
                 print('The VIF filtering method was applied')
                 self.train = self.train[cols_vif]
                 self.test = self.test[cols_vif]
             else:
                 print('The VIF filtering method was not applied')
     
         return self.train, self.test
```

## Comparing `atlantic-1.1.5.dist-info/LICENSE` & `atlantic-1.1.50.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atlantic-1.1.5.dist-info/METADATA` & `atlantic-1.1.50.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlantic
-Version: 1.1.5
+Version: 1.1.50
 Summary: Atlantic is an automated preprocessing framework for Supervised Machine Learning
 Home-page: https://github.com/TsLu1s/Atlantic
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,predictive modeling,data preprocessing,automated data preprocessing,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -15,14 +15,16 @@
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: numpy (>=1.19.5)
 Requires-Dist: cane (>=2.3.1)
 Requires-Dist: scikit-learn (>=1.2.2)
 Requires-Dist: h2o (>=3.44.0.1)
@@ -62,15 +64,15 @@
 
 <p align="center">
   <img src="https://i.ibb.co/C9dWJmk/ATL-Architecture-Final.png" align="center" width="700" height="680" />
 </p>    
 
 ## Where to get it <a name = "ta"></a>
 
-Binary installer for the latest released version is available at the Python Package Index [PyPI](https://pypi.org/project/atlantic/).  
+Binary installer for the latest released version is available at the Python Package Index [(PyPI)](https://pypi.org/project/atlantic/).  
 
 The source code is currently hosted on GitHub at: https://github.com/TsLu1s/Atlantic
 
 ## Installation  
 
 To install this package from Pypi repository run the following command:
 
@@ -79,54 +81,64 @@
 ```
 
 # Usage Examples
     
 ## 1. Atlantic - Automated Data Preprocessing Pipeline
 
 In order to be able to apply the automated preprocessing `atlantic` pipeline you need first to import the package. 
-The following needed step is to load a dataset and define your to be predicted target column name into the variable `target` and define split ratio for your Train and Validation subsets.
+The following needed step is to load a dataset, split it and define your to be predicted target column name into the variable `target`.
 You can customize the `fit_processing` method by altering the following running pipeline parameters:
-* split_ratio: Division ratio in which the preprocessing methods will be evaluated within the loaded Dataset.
-* relevance: Minimal value of the total sum of relative variable\feature importance percentage selected in the `H2O AutoML feature selection` step.
+* split_ratio: Division ratio (Train\Validation) in which the preprocessing methods will be evaluated within the loaded Dataset.
+* relevance: Minimal value of the total sum of relative feature importance percentage selected in the `H2O AutoML feature selection` step.
 * h2o_fs_models: Quantity of models generated for competition in step `H2O AutoML feature selection` to evaluate the relative importance of each feature (only leaderboard model is selected for evaluation).
-* encoding_fs: You can choose if you want to encond your features in order to reduce loading time in `H2O AutoML feature selection` step. If in `True` mode label encoding is applied to categorical features.
+* encoding_fs: You can choose if you want to enconde categorical features in order to reduce loading time in `H2O AutoML feature selection` step.
 * vif_ratio: This value defines the minimal `threshold` for Variance Inflation Factor filtering (default value=10).
+
+Once the data fitting process is complete, you can automaticaly optimize preprocessing transformations on all future dataframes with the same properties using the `data_processing` method.
  
 Importante Notes:
     
 * Default predictive evaluation metric for regression contexts is `Mean Absolute Error` and classification is `Accuracy`.
 * Although functional, `Atlantic` data processing is not optimized for big data purposes yet.
-* Major update is now available in **versions>=1.1.0**
     
 ```py
-    
-from atlantic.pipeline import ATLpipeline
 import pandas as pd
-from sklearn.model_selection import train_test_split 
+from sklearn.model_selection import train_test_split
+from atlantic.pipeline import Atlantic
+import warnings
+warnings.filterwarnings("ignore", category=Warning) # -> For a clean console
     
 data = pd.read_csv('csv_directory_path', encoding='latin', delimiter=',') # Dataframe Loading Example
 
-train,test = train_test_split(data, train_size=0.8)
-train,test = train.reset_index(drop=True), test.reset_index(drop=True) # Required 
+train,test = train_test_split(data, train_size = 0.8)
+test,future_data = train_test_split(test, train_size = 0.6)
+
+# Resetting Index is Required
+train = train.reset_index(drop=True)
+test = test.reset_index(drop=True)
+future_data = future_data.reset_index(drop=True)
+
+future_data.drop(columns=["Target_Column"], inplace=True) # Drop Target
 
 ### Fit Data Processing
 
-atl = ATLpipeline(X=train,              # X:pd.DataFrame, target:str="Target_Column"
-                  target="Target Column")    
+atl = Atlantic(X = train,                # X:pd.DataFrame, target:str="Target_Column"
+               target = "Target Column")    
 
-atl.fit_processing(split_ratio=0.75,   # split_ratio:float=0.75, relevance:float=0.99 [0.5,1]
-                   relevance=0.99,     # h2o_fs_models:int [1,50], encoding_fs:bool=True\False
-                   h2o_fs_models=7,    # vif_ratio:float=10.0 [3,30]
-                   encoding_fs=True,
-                   vif_ratio=10.0)
+atl.fit_processing(split_ratio = 0.75,   # split_ratio:float=0.75, relevance:float=0.99 [0.5,1]
+                   relevance = 0.99,     # h2o_fs_models:int [1,100], encoding_fs:bool=True\False
+                   h2o_fs_models = 7,    # vif_ratio:float=10.0 [3,30]
+                   encoding_fs = True,
+                   vif_ratio = 10.0)
 
 ### Transform Data Processing
 
-train = atl.data_processing(X=train)
-test = atl.data_processing(X=test)
+train = atl.data_processing(X = train)
+test = atl.data_processing(X = test)
+future_data = atl.data_processing(X = future_data)
 
 ### Export Atlantic Preprocessing Metadata
 
 import pickle 
 output = open("fit_atl.pkl", 'wb')
 pickle.dump(atl, output)
     
@@ -135,42 +147,42 @@
 ## 2. Atlantic - Preprocessing Data
     
 ### 2.1 Encoding Versions
  
 There are multiple preprocessing methods available to direct use. This package provides upgrated encoding `LabelEncoder`, `OneHotEncoder` and [IDF](https://pypi.org/project/cane/) methods with an automatic multicolumn application. 
  
 ```py
-from atlantic.processing import AutoLabelEncoder, AutoIdfEncoder, AutoOneHotEncoder
 import pandas as pd
 from sklearn.model_selection import train_test_split 
+from atlantic.processing.encoders import AutoLabelEncoder, AutoIdfEncoder, AutoOneHotEncoder
 
 train,test = train_test_split(data, train_size=0.8)
 train,test = train.reset_index(drop=True), test.reset_index(drop=True) # Required
 
 target = "Target_Column" # -> target feature name
     
-cat_cols=[col for col in data.select_dtypes(include=['object']).columns if col != target]
+cat_cols = [col for col in data.select_dtypes(include=['object']).columns if col != target]
 
 ### Encoders
 ## Create Label Encoder
 encoder = AutoLabelEncoder()
 ## Create IDF Encoder
 encoder = AutoIdfEncoder()
 ## Create One-hot Encoder
 encoder = AutoOneHotEncoder()
 
 ## Fit
 encoder.fit(train[cat_cols])
 
 # Transform the DataFrame using Label\IDF\One-hot Encoding
-train = encoder.transform(X=train)
-test = encoder.transform(X=test)
+train = encoder.transform(X = train)
+test = encoder.transform(X = test)
 
 # Label Encoding : Perform an inverse transform to convert it back the categorical columns values
-test = encoder.inverse_transform(X=test)
+test = encoder.inverse_transform(X = test)
 
 # IDF & One-hot Encoding : Perform an inverse transform to convert it back the categorical columns values
 # Note: Only decodes the last transformed Dataframe
 test = encoder.inverse_transform()
             
 ```    
    
@@ -179,57 +191,56 @@
 You can get filter your most valuable features from the dataset via this 2 feature selection methods:
     
 * [H2O AutoML Feature Selection](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/variable-importance.html) - This method is based of variable importance evaluation and calculation for tree-based models in H2Os AutoML and it can be customized by use of the following parameters: 
   * relevance: Minimal value of the total sum of relative variable\feature importance percentage selected.
   * h2o_fs_models: Quantity of models generated for competition to evaluate the relative importance of each feature (only leaderboard model will be selected for evaluation).
   * encoding_fs: You can choose if you want to encond your features in order to reduce loading time. If in `True` mode label encoding is applied to categorical features.
     
-    
 * [VIF Feature Selection (Variance Inflation Factor)](https://www.investopedia.com/terms/v/variance-inflation-factor.asp) - Variance inflation factor aims at measuring the amount of multicollinearity in a set of multiple regression variables or features, therefore for this filtering method to be applied all input variables need to be of numeric type. It can be customized by changing the column filtering treshold `vif_threshold` designated with a default value of 10.
     
     
 ```py    
-from atlantic.selector import Selector
+from atlantic.feature_selection.selector import Selector
 
-fs=Selector(X=train,target="Target_Column")
+fs = Selector(X = train, target = "Target_Column")
 
-cols_vif = fs.feature_selection_vif(vif_threshold=10.0)   # X: Only numerical values allowed & No nans allowed in VIF
+cols_vif = fs.feature_selection_vif(vif_threshold = 10.0)   # X: Only numerical values allowed & No nans allowed in VIF
 
-selected_cols, selected_importance = fs.feature_selection_h2o(relevance=0.99,     # relevance:float [0.5,1], h2o_fs_models:int [1,50]
-                                                              h2o_fs_models=7,    # encoding_fs:bool=True/False
-                                                              encoding_fs=True)
+selected_cols, selected_importance = fs.feature_selection_h2o(relevance = 0.99,     # relevance:float [0.5,1], h2o_fs_models:int [1,100]
+                                                              h2o_fs_models = 7,    # encoding_fs:bool=True/False
+                                                              encoding_fs = True)
 ```
     
 ### 2.3 Null Imputation Auxiliar Methods
     
 Simplified and automated multivariate null imputation methods based from [Sklearn](https://scikit-learn.org/stable/modules/impute.html) are also provided and applicable, as following:
     
 ```py  
 
 ## Simplified Null Imputation (Only numeric features)
-from atlantic.imputation import AutoSimpleImputer, AutoKNNImputer, AutoIterativeImputer
+from atlantic.imputers.imputation import AutoSimpleImputer, AutoKNNImputer, AutoIterativeImputer
 
 # Example usage of AutoSimpleImputer
-simple_imputer = AutoSimpleImputer(strategy='mean')
+simple_imputer = AutoSimpleImputer(strategy = 'mean')
 simple_imputer.fit(train)  # Fit on the Train DataFrame
 df_imputed = simple_imputer.transform(train.copy())  # Transform the Train DataFrame
 df_imputed_test = simple_imputer.transform(test.copy()) # Transform the Test DataFrame
 
 # Example usage of AutoKNNImputer
-knn_imputer = AutoKNNImputer(n_neighbors=3,
-                             weights="uniform")
+knn_imputer = AutoKNNImputer(n_neighbors = 3,
+                             weights = "uniform")
 knn_imputer.fit(train)  # Fit on the Train DataFrame
 df_imputed = knn_imputer.transform(train.copy())  # Transform the Train DataFrame
 df_imputed_test = knn_imputer.transform(test.copy()) # Transform the Test DataFrame
 
 # Example usage of AutoIterativeImputer
-iterative_imputer = AutoIterativeImputer(max_iter=10, 
-                                         random_state=0, 
-                                         initial_strategy="mean", 
-                                         imputation_order="ascending")
+iterative_imputer = AutoIterativeImputer(max_iter = 10, 
+                                         random_state = 0, 
+                                         initial_strategy = "mean", 
+                                         imputation_order = "ascending")
 iterative_imputer.fit(train)  # Fit on the Train DataFrame
 df_imputed = iterative_imputer.transform(train.copy())  # Transform the Train DataFrame
 df_imputed_test = iterative_imputer.transform(test.copy()) # Transform the Test DataFrame
 
 ```   
 
 ## Citation
```

