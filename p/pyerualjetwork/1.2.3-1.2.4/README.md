# Comparing `tmp/pyerualjetwork-1.2.3.tar.gz` & `tmp/pyerualjetwork-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.3.tar", last modified: Sun May 26 16:05:01 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.4.tar", last modified: Sun May 26 16:13:30 2024, max compression
```

## Comparing `pyerualjetwork-1.2.3.tar` & `pyerualjetwork-1.2.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:05:01.759179 pyerualjetwork-1.2.3/
--rw-rw-rw-   0        0        0      511 2024-05-26 16:05:01.758179 pyerualjetwork-1.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-26 16:05:01.741397 pyerualjetwork-1.2.3/plan/
--rw-rw-rw-   0        0        0      368 2024-05-26 15:58:07.000000 pyerualjetwork-1.2.3/plan/__init__.py
--rw-rw-rw-   0        0        0    40159 2024-05-26 16:03:41.000000 pyerualjetwork-1.2.3/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:05:01.755954 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      511 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-26 16:05:01.000000 pyerualjetwork-1.2.3/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 16:05:01.759179 pyerualjetwork-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      687 2024-05-26 16:04:51.000000 pyerualjetwork-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:13:30.359182 pyerualjetwork-1.2.4/
+-rw-rw-rw-   0        0        0      511 2024-05-26 16:13:30.358185 pyerualjetwork-1.2.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 16:13:30.343646 pyerualjetwork-1.2.4/plan/
+-rw-rw-rw-   0        0        0      368 2024-05-26 15:58:07.000000 pyerualjetwork-1.2.4/plan/__init__.py
+-rw-rw-rw-   0        0        0    40168 2024-05-26 16:12:52.000000 pyerualjetwork-1.2.4/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-26 16:13:30.356189 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 16:13:30.000000 pyerualjetwork-1.2.4/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 16:13:30.359182 pyerualjetwork-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-26 16:13:21.000000 pyerualjetwork-1.2.4/setup.py
```

### Comparing `pyerualjetwork-1.2.3/plan/plan.py` & `pyerualjetwork-1.2.4/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -724,15 +724,15 @@
             'ACTIVATIONS': Activations,
             'NEURON COUNT': NeuronCount,
             'SYNAPSE COUNT': SynapseCount,
             'TEST ACCURACY': TestAcc,
             'SAVE DATE': datetime.now(),
             'WEIGHTS TYPE': WeightsType,
             'WEIGHTS FORMAT': WeightsFormat,
-            'SAVE PATH': ModelPath
+            'MODEL PATH': ModelPath
             }
     try:
         
         df = pd.DataFrame(data)
         
         if  LogType == 'csv':
         
@@ -819,46 +819,46 @@
         Style.RESET_ALL
         )
     
     return print(message)
 
 
 def LoadPLAN(ModelName,
-             LoadPath,
+             ModelPath,
              LogType,
 ):
    infoLoadPLAN = """
    Function to load a deep learning model.
 
    Arguments:
    ModelName (str): Name of the model.
-   LoadPath (str): Path where the model is saved.
+   ModelPath (str): Path where the model is saved.
    LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
    Returns:
    lists: W(list[num]), Layers, ThresholdSigns, ThresholdValues, Normalization,Activations
     """
    pass
 
     
    import pandas as pd
    import scipy.io as sio
    
    try:
    
        if LogType == 'csv':
-           df = pd.read_csv(LoadPath + ModelName + '.' + LogType)
+           df = pd.read_csv(ModelPath + ModelName + '.' + LogType)
         
     
        if LogType == 'txt':
-           df = pd.read_csv(LoadPath + ModelName + '.' + LogType, delimiter='\t')
+           df = pd.read_csv(ModelPath + ModelName + '.' + LogType, delimiter='\t')
         
     
        if LogType == 'hdf5':
-           df = pd.read_hdf(LoadPath + ModelName + '.' + LogType)
+           df = pd.read_hdf(ModelPath + ModelName + '.' + LogType)
    except:
        print(Fore.RED + "ERROR: Model Path error. Accaptable form: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: LoadPLAN" + infoLoadPLAN + Style.RESET_ALL)
 
    ModelName = str(df['MODEL NAME'].iloc[0])
    Layers = df['LAYERS'].tolist()
    LayerCount = int(df['LAYER COUNT'].iloc[0])
    ClassCount = int(df['CLASS COUNT'].iloc[0])
@@ -874,21 +874,21 @@
    WeightFormat = str(df['WEIGHTS FORMAT'].iloc[0])
    ModelPath = str(df['MODEL PATH'].iloc[0])
 
    W = [0] * LayerCount
    
    if WeightType == 'txt':
        for i in range(LayerCount):
-           W[i] = np.loadtxt(LoadPath + ModelName + str(i+1) + 'w.txt')
+           W[i] = np.loadtxt(ModelPath + ModelName + str(i+1) + 'w.txt')
    elif WeightType == 'npy':
        for i in range(LayerCount):    
-           W[i] = np.load(LoadPath + ModelName + str(i+1) + 'w.npy')
+           W[i] = np.load(ModelPath + ModelName + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
        for i in range(LayerCount):  
-           W[i] = sio.loadmat(LoadPath + ModelName + str(i+1) + 'w.mat')
+           W[i] = sio.loadmat(ModelPath + ModelName + str(i+1) + 'w.mat')
    else:
         raise ValueError(Fore.RED + "Incorrect weight type value. Value must be 'txt', 'npy' or 'mat' from: LoadPLAN."  + infoLoadPLAN + Style.RESET_ALL)
    print(Fore.GREEN + "Model loaded succesfully" + Style.RESET_ALL)     
    return W,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations,df
 
 def PredictFromDiscPLAN(Input,ModelName,ModelPath,LogType):
     infoPredictFromDİscPLAN = """
```

### Comparing `pyerualjetwork-1.2.3/setup.py` & `pyerualjetwork-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Setting Up
 
 setup(
       
       name = "pyerualjetwork",
-      version = "1.2.3",
+      version = "1.2.4",
       author = "Hasan Can Beydili",
       author_email = "tchasancan@gmail.com",
       description= "Advanced python deep learning library.UPDATED TO 1.2.2 NEW FEATURES: GetWeights() func for TrainPLAN, TestPLAN and LoadPLAN, GetPreds() and GetAcc() funcs for TrainPLAN and TestPLAN, GetAllFromLoad() func for LoadPLAN, GetDf() for LoadPLAN (Documentation in desc. Examples in GİTHUB: HCB06)",
       packages = find_packages(),
       keywords = ["model evaluation", "classifcation", 'pruning learning artficial neural networks']
       
       )
```

