# Comparing `tmp/pyerualjetwork-1.2.0.tar.gz` & `tmp/pyerualjetwork-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.0.tar", last modified: Fri May 24 14:25:19 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.1.tar", last modified: Sun May 26 15:53:55 2024, max compression
```

## Comparing `pyerualjetwork-1.2.0.tar` & `pyerualjetwork-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 14:25:19.827287 pyerualjetwork-1.2.0/
--rw-rw-rw-   0        0        0      309 2024-05-24 14:25:19.825291 pyerualjetwork-1.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-24 14:25:19.805913 pyerualjetwork-1.2.0/plan/
--rw-rw-rw-   0        0        0      315 2024-05-23 00:45:28.000000 pyerualjetwork-1.2.0/plan/__init__.py
--rw-rw-rw-   0        0        0    40179 2024-05-24 14:21:37.000000 pyerualjetwork-1.2.0/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-24 14:25:19.824331 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      309 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-24 14:25:19.000000 pyerualjetwork-1.2.0/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 14:25:19.827287 pyerualjetwork-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      485 2024-05-24 14:24:44.000000 pyerualjetwork-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:53:55.592932 pyerualjetwork-1.2.1/
+-rw-rw-rw-   0        0        0      511 2024-05-26 15:53:55.591932 pyerualjetwork-1.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-26 15:53:55.570229 pyerualjetwork-1.2.1/plan/
+-rw-rw-rw-   0        0        0      315 2024-05-23 00:45:28.000000 pyerualjetwork-1.2.1/plan/__init__.py
+-rw-rw-rw-   0        0        0    40174 2024-05-26 15:20:16.000000 pyerualjetwork-1.2.1/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-26 15:53:55.590232 pyerualjetwork-1.2.1/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      511 2024-05-26 15:53:55.000000 pyerualjetwork-1.2.1/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-26 15:53:55.000000 pyerualjetwork-1.2.1/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 15:53:55.000000 pyerualjetwork-1.2.1/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-26 15:53:55.000000 pyerualjetwork-1.2.1/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-26 15:53:55.592932 pyerualjetwork-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-26 15:53:10.000000 pyerualjetwork-1.2.1/setup.py
```

### Comparing `pyerualjetwork-1.2.0/plan/plan.py` & `pyerualjetwork-1.2.1/plan/plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import numpy as np
 import time
 from colorama import Fore,Style
 from typing import List, Union
 import math
+from scipy.special import expit, softmax
+
 # BUILD -----
 def TrainPLAN(
-    Inputs: List[Union[int, float]], 
-    Labels: List[Union[int, float, str]], # At least two.. and one hot encoded
+    TrainInputs: List[Union[int, float]], 
+    TrainLabels: List[Union[int, float, str]], # At least two.. and one hot encoded
     ClassCount: int,
     Layers: List[str],
     Neurons: List[Union[int, float]],
     ThresholdSigns: List[str],
     ThresholdValues: List[Union[int, float]],
     Normalizations: List[str],
     Activations: List[str]
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
-        Inputs (list[num]): List of input data.
-        Labels (list[num]): List of labels. (one hot encoded)
+        TrainInputs (list[num]): List of input data.
+        TrainLabels (list[num]): List of TrainLabels. (one hot encoded)
         ClassCount (int): Number of classes.
         Layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
         Neurons (list[num]): List of neuron counts for each layer.
         ThresholdSigns (list[str]): List of threshold signs.
         ThresholdValues (list[num]): List of threshold values.
         Normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
         Activations (list[str]): List of activation functions.
@@ -41,16 +43,16 @@
             return 'e'
     
     if len(Normalizations) != len(ThresholdValues):
         
             print(Fore.RED + "ERROR307: Normalization list length must be equal to length of ThresholdSigns List,ThresholdValues List,Layers List,Neurons List. from: TrainPLAN",infoPLAN)
             return 'e'
     
-    if len(Inputs) != len(Labels):
-        print(Fore.RED + "ERROR301: Inputs list and Labels list must be same length.",infoPLAN)
+    if len(TrainInputs) != len(TrainLabels):
+        print(Fore.RED + "ERROR301: TrainInputs list and TrainLabels list must be same length.",infoPLAN)
         return 'e'
     
     for i, Value in enumerate(ThresholdValues):
         
         if Normalizations[i] != 'y' and Normalizations[i] != 'n':
                 print(Fore.RED + "ERROR105: Normalization list must be 'y' or 'n'.",infoPLAN)
                 return 'e'
@@ -113,53 +115,53 @@
             print(Fore.RED + "ERROR104: Threshold signs must be '>' or '<' or '==' or '!='. or 'none' from: TrainPLAN",infoPLAN)
             return 'e'
         
         if Layers[i] == 'fex' and Sign == 'none':
             print(Fore.RED + "ERROR109: at layer type 'fex', pairing with 'none' Threshold is not acceptlable. if you want to 'none' put '==' and make threshold value '0'. from: TrainPLAN ",infoPLAN)
             return 'e'
         
-    UniqueLabels = set()
-    for sublist in Labels:
+    UniqueTrainLabels = set()
+    for sublist in TrainLabels:
       
-        UniqueLabels.add(tuple(sublist))
+        UniqueTrainLabels.add(tuple(sublist))
     
     
-    UniqueLabels = list(UniqueLabels)
+    UniqueTrainLabels = list(UniqueTrainLabels)
     
-    Labels = [tuple(sublist) for sublist in Labels]
+    TrainLabels = [tuple(sublist) for sublist in TrainLabels]
     
     
-    if len(UniqueLabels) != ClassCount:
+    if len(UniqueTrainLabels) != ClassCount:
         print(Fore.RED + "ERROR106: Label variety length must be same Class Count. from: TrainPLAN",infoPLAN)
         return 'e'
     
-    Inputs[0] = np.array(Inputs[0])
-    Inputs[0] = Inputs[0].ravel()
-    InputSize = len(Inputs[0])
+    TrainInputs[0] = np.array(TrainInputs[0])
+    TrainInputs[0] = TrainInputs[0].ravel()
+    TrainInputsize = len(TrainInputs[0])
     
-    W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,InputSize)
+    W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,TrainInputsize)
     Divides = SynapticDividing(ClassCount,W)
     TrainedWs = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
-    TrainPredictions = [1] * len(Labels)
+    TrainPredictions = [1] * len(TrainLabels)
     true = 0
     StartTime = time.time()
-    for index, inp in enumerate(Inputs):
+    for index, inp in enumerate(TrainInputs):
         UniStartTime = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
-        if InputSize != len(inp):
-            print(Fore.RED +"ERROR304: All input matrices or vectors in inputs list, must be same size. from: TrainPLAN",infoPLAN + Style.RESET_ALL)
+        if TrainInputsize != len(inp):
+            print(Fore.RED +"ERROR304: All input matrices or vectors in TrainInputs list, must be same size. from: TrainPLAN",infoPLAN + Style.RESET_ALL)
             return 'e'
         
         
-        for Ulindex, Ul in enumerate(UniqueLabels):
+        for Ulindex, Ul in enumerate(UniqueTrainLabels):
             
-            if Ul == Labels[index]:
+            if Ul == TrainLabels[index]:
                 for Windex, w in enumerate(W):
                     for i, ul in enumerate(Ul):
                         if ul == 1.0:
                             k = i
                     Cs = Divides[int(k)][Windex][0]
        
                     W[Windex] = SynapticPruning(w, Cs, 'row', int(k),ClassCount)
@@ -179,36 +181,36 @@
                 NeuralLayer = Softmax(NeuralLayer)
                 
             if Layer == 'fex':
                 NeuralLayer,W[Lindex] = Fex(NeuralLayer, W[Lindex], ThresholdSigns[Lindex], ThresholdValues[Lindex])
             elif Layer == 'cat':
                 NeuralLayer,W[Lindex] = Cat(NeuralLayer, W[Lindex], ThresholdSigns[Lindex], ThresholdValues[Lindex],1)
                 
-        RealOutput = np.argmax(Labels[index])
+        RealOutput = np.argmax(TrainLabels[index])
         PredictedOutput = np.argmax(NeuralLayer)
         if RealOutput == PredictedOutput:
             true += 1
-        Acc = true / len(Labels)
-        TrainPredictions[index] = PredictedOutput+1
+        Acc = true / len(TrainLabels)
+        TrainPredictions[index] = PredictedOutput
         
         if index == 0:
             for i, w in enumerate(W):
                 TrainedWs[i] = w
                      
         else:
             for i, w in enumerate(W):
                 TrainedWs[i] = TrainedWs[i] + w
             
                 
-        W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,InputSize)
+        W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,TrainInputsize)
          
                
         UniEndTime = time.time()
         
-        CalculatingEst = round((UniEndTime - UniStartTime) * (len(Inputs) - index),3)
+        CalculatingEst = round((UniEndTime - UniStartTime) * (len(TrainInputs) - index),3)
         
         if CalculatingEst < 60:
             print('\rest......(sec):',CalculatingEst,'\n',end= "")
             print('\rTrain Accuracy: ' ,Acc ,"\n", end="")
         
         elif CalculatingEst > 60 and CalculatingEst < 3600:
             print('\rest......(min):',CalculatingEst/60,'\n',end= "")
@@ -249,33 +251,33 @@
         
 # FUNCTIONS -----
 
 def WeightIdentification(
     LayerCount,      # int: Number of layers in the neural network.
     ClassCount,      # int: Number of classes in the classification task.
     Neurons,         # list[num]: List of neuron counts for each layer.
-    InputSize        # int: Size of the input data.
+    TrainInputsize        # int: Size of the input data.
 ) -> str:
     """
     Identifies the weights for a neural network model.
 
     Args:
         LayerCount (int): Number of layers in the neural network.
         ClassCount (int): Number of classes in the classification task.
         Neurons (list[num]): List of neuron counts for each layer.
-        InputSize (int): Size of the input data.
+        TrainInputsize (int): Size of the input data.
 
     Returns:
         list([numpy_arrays],[...]): Weight matices of the model. .
     """
 
     
     Wlen = LayerCount + 1
     W = [None] * Wlen
-    W[0] = np.ones((Neurons[0],InputSize))
+    W[0] = np.ones((Neurons[0],TrainInputsize))
     ws = LayerCount - 1
     for w in range(ws):
         W[w + 1] = np.ones((Neurons[w + 1],Neurons[w]))
     W[LayerCount] = np.ones((ClassCount,Neurons[LayerCount - 1]))
     return W
 
 def SynapticPruning(
@@ -488,53 +490,31 @@
 
     Args:
         x (list[num]): Input data to be transformed using softmax function.
 
     Returns:
         list[num]: Transformed data after applying softmax function.
     """
-
-
-    MaxX = np.max(x)
-    
-    x -= MaxX
-    
-    ExpX = np.exp(x)
-    
-    SumExpX = np.sum(ExpX)
     
-    SoftmaxX = ExpX / SumExpX
-    
-    return SoftmaxX
+    return softmax(x)
 
 
 def Sigmoid(
     x  # list[num]: Input data to be transformed using sigmoid function.
 ):
     """
     Applies the sigmoid function to the input data.
 
     Args:
         x (list[num]): Input data to be transformed using sigmoid function.
 
     Returns:
         list[num]: Transformed data after applying sigmoid function.
     """
-
-    PositiveMask = x >= 0
-    NegativeMask = ~PositiveMask
-   
-    ExpXPositive = np.exp(-np.clip(x[PositiveMask], -709, None))
-    ExpXNegative = np.exp(np.clip(x[NegativeMask], None, 709))
-
-    SigmoidX = np.zeros_like(x, dtype=float)
-    SigmoidX[PositiveMask] = 1 / (1 + ExpXPositive)
-    SigmoidX[NegativeMask] = ExpXNegative / (1 + ExpXNegative)
-   
-    return SigmoidX
+    return expit(x)
 
 
 def Relu(
     x  # list[num]: Input data to be transformed using ReLU function.
 ):
     """
     Applies the Rectified Linear Unit (ReLU) function to the input data.
@@ -611,15 +591,15 @@
             for i, w in enumerate(Wc):
                 W[i] = np.copy(w)
             RealOutput = np.argmax(TestLabels[inpIndex])
             PredictedOutput = np.argmax(NeuralLayer)
             if RealOutput == PredictedOutput:
                 true += 1
             Acc = true / len(TestLabels)
-            TestPredictions[inpIndex] = PredictedOutput+1
+            TestPredictions[inpIndex] = PredictedOutput
             UniEndTime = time.time()
                 
             CalculatingEst = round((UniEndTime - UniStartTime) * (len(TestInputs) - inpIndex),3)
                 
             if CalculatingEst < 60:
                 print('\rest......(sec):',CalculatingEst,'\n',end= "")
                 print('\rTest Accuracy: ' ,Acc ,"\n", end="")
@@ -659,29 +639,29 @@
             print(Fore.RED+ '\nTotal Test Accuracy: ' ,Acc, '\n' + Style.RESET_ALL)   
     
     except:
         
         print(Fore.RED + "ERROR: Testing model parameters like 'Layers' 'ThresholdCounts' must be same as trained model. Check parameters. Are you sure weights are loaded ? from: TestPLAN" + infoTestModel + Style.RESET_ALL)
         return 'e'
    
-    return TestPredictions,Acc
+    return W,TestPredictions,Acc
 
 def SavePLAN(ModelName,
              ModelType,
              Layers,
              ClassCount,
              ThresholdSigns,
              ThresholdValues,
              Normalizations,
              Activations,
              TestAcc,
              LogType,
              WeightsType,
              WeightsFormat,
-             SavePath,
+             ModelPath,
              W
  ):
     
     infoSavePLAN = """
     Function to save a deep learning model.
 
     Arguments:
@@ -693,15 +673,15 @@
     ThresholdValues (list): List containing threshold values.
     DoNormalization (str): is that normalized data ? 'y' or 'n'.
     Activations (list): List containing activation functions for each layer.
     TestAcc (float): Test accuracy of the model.
     LogType (str): Type of log to save (options: 'csv', 'txt', 'hdf5').
     WeightsType (str): Type of weights to save (options: 'txt', 'npy', 'mat').
     WeightFormat (str): Format of the weights (options: 'd', 'f', 'raw').
-    SavePath (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
+    ModelPath (str): Path where the model will be saved. For example: C:/Users/beydili/Desktop/denemePLAN/
     W: Weights of the model.
     
     Returns:
     str: Message indicating if the model was saved successfully or encountered an error.
     """
     
     # Operations to be performed by the function will be written here
@@ -744,93 +724,93 @@
             'ACTIVATIONS': Activations,
             'NEURON COUNT': NeuronCount,
             'SYNAPSE COUNT': SynapseCount,
             'TEST ACCURACY': TestAcc,
             'SAVE DATE': datetime.now(),
             'WEIGHTS TYPE': WeightsType,
             'WEIGHTS FORMAT': WeightsFormat,
-            'SAVE PATH': SavePath
+            'SAVE PATH': ModelPath
             }
     try:
         
         df = pd.DataFrame(data)
         
         if  LogType == 'csv':
         
-            df.to_csv(SavePath + ModelName + '.csv', sep='\t', index=False)
+            df.to_csv(ModelPath + ModelName + '.csv', sep='\t', index=False)
             
         elif LogType == 'txt':
             
-            df.to_csv(SavePath + ModelName + '.txt', sep='\t', index=False)
+            df.to_csv(ModelPath + ModelName + '.txt', sep='\t', index=False)
             
         elif LogType == 'hdf5':
             
-            df.to_hdf(SavePath + ModelName + '.h5', key='data', mode='w')
+            df.to_hdf(ModelPath + ModelName + '.h5', key='data', mode='w')
             
     except:
         
         print(Fore.RED + "ERROR: Model log not saved. Check the log parameters from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     try:
         
         if WeightsType == 'txt' and WeightsFormat == 'd':
             
             for i, w in enumerate(W):
-                np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%d')
+                np.savetxt(ModelPath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%d')
                 
         if WeightsType == 'txt' and WeightsFormat == 'f':
              
             for i, w in enumerate(W):
-                 np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%f')
+                 np.savetxt(ModelPath + ModelName +  str(i+1) + 'w.txt' ,  w, fmt='%f')
         
         if WeightsType == 'txt' and WeightsFormat == 'raw':
             
             for i, w in enumerate(W):
-                np.savetxt(SavePath + ModelName +  str(i+1) + 'w.txt' ,  w)
+                np.savetxt(ModelPath + ModelName +  str(i+1) + 'w.txt' ,  w)
             
                 
         ###
         
         
         if WeightsType == 'npy' and WeightsFormat == 'd':
             
             for i, w in enumerate(W):
-                np.save(SavePath + ModelName + str(i+1) + 'w.npy', w.astype(int))
+                np.save(ModelPath + ModelName + str(i+1) + 'w.npy', w.astype(int))
         
         if WeightsType == 'npy' and WeightsFormat == 'f':
              
             for i, w in enumerate(W):
-                 np.save(SavePath + ModelName +  str(i+1) + 'w.npy' ,  w, w.astype(float))
+                 np.save(ModelPath + ModelName +  str(i+1) + 'w.npy' ,  w, w.astype(float))
         
         if WeightsType == 'npy' and WeightsFormat == 'raw':
             
             for i, w in enumerate(W):
-                np.save(SavePath + ModelName +  str(i+1) + 'w.npy' ,  w)
+                np.save(ModelPath + ModelName +  str(i+1) + 'w.npy' ,  w)
                 
            
         ###
         
          
         if WeightsType == 'mat' and WeightsFormat == 'd':
             
             for i, w in enumerate(W):
                 w = {'w': w.astype(int)}
-                io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
+                io.savemat(ModelPath + ModelName + str(i+1) + 'w.mat', w)
     
         if WeightsType == 'mat' and WeightsFormat == 'f':
              
             for i, w in enumerate(W):
                 w = {'w': w.astype(float)}
-                io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
+                io.savemat(ModelPath + ModelName + str(i+1) + 'w.mat', w)
         
         if WeightsType == 'mat' and WeightsFormat == 'raw':
             
             for i, w in enumerate(W):
                 w = {'w': w}
-                io.savemat(SavePath + ModelName + str(i+1) + 'w.mat', w)
+                io.savemat(ModelPath + ModelName + str(i+1) + 'w.mat', w)
             
     except:
         
         print(Fore.RED + "ERROR: Model Weights not saved. Check the Weight parameters. SaveFilePath expl: 'C:/Users/hasancanbeydili/Desktop/denemePLAN/' from: SavePLAN" + infoSavePLAN + Style.RESET_ALL)
         return 'e'
     print(df)
     message = (
@@ -880,28 +860,28 @@
 
    ModelName = str(df['MODEL NAME'].iloc[0])
    Layers = df['LAYERS'].tolist()
    LayerCount = int(df['LAYER COUNT'].iloc[0])
    ClassCount = int(df['CLASS COUNT'].iloc[0])
    ThresholdSigns = df['THRESHOLD SIGNS'].tolist()
    ThresholdValues = df['THRESHOLD VALUES'].tolist()
-   Normalization = df['NORMALIZATION'].tolist()
+   Normalizations = df['NORMALIZATION'].tolist()
    Activations = df['ACTIVATIONS'].tolist()
    NeuronCount = int(df['NEURON COUNT'].iloc[0])
    SynapseCount = int(df['SYNAPSE COUNT'].iloc[0])
    TestAcc = int(df['TEST ACCURACY'].iloc[0])
    ModelType = str(df['MODEL TYPE'].iloc[0])
    WeightType = str(df['WEIGHTS TYPE'].iloc[0])
    WeightFormat = str(df['WEIGHTS FORMAT'].iloc[0])
-   SavePath = str(df['SAVE PATH'].iloc[0])
+   ModelPath = str(df['MODEL PATH'].iloc[0])
 
    W = [0] * LayerCount
    
    if WeightType == 'txt':
-       for i in range(LayerCount):    
+       for i in range(LayerCount):
            W[i] = np.loadtxt(LoadPath + ModelName + str(i+1) + 'w.txt')
    elif WeightType == 'npy':
        for i in range(LayerCount):    
            W[i] = np.load(LoadPath + ModelName + str(i+1) + 'w.npy')
    elif WeightType == 'mat':
        for i in range(LayerCount):  
            W[i] = sio.loadmat(LoadPath + ModelName + str(i+1) + 'w.mat')
@@ -919,15 +899,15 @@
     ModelName (str): Name of the model.
     ModelPath (str): Path where the model is saved.
     LogType (str): Type of log to load (options: 'csv', 'txt', 'hdf5').
 
     Returns:
     ndarray: Output from the model.
     """
-    W,Layers,ThresholdSigns,ThresholdValues,Normalization,Activations = LoadPLAN(ModelName,ModelPath,
+    W,Layers,ThresholdSigns,ThresholdValues,Normalizations,Activations = LoadPLAN(ModelName,ModelPath,
                                                                                   LogType)[0:6]
     Wc = [0] * len(W)
     for i, w in enumerate(W):
         Wc[i] = np.copy(w)
     try:
         NeuralLayer = Input
         NeuralLayer = np.array(NeuralLayer)
@@ -1044,8 +1024,30 @@
         BalancedLabels = [TrainLabels[idx] for idx in BalancedIndices]
         
         print(Fore.GREEN + "All Training Data Succesfully Balanced from: " + str(len(TrainInputs)) + " to: " + str(len(BalancedInputs)) + ". from: AutoBalancer " + Style.RESET_ALL)
    except:
         print(Fore.RED + "ERROR: Inputs and labels must be same length check parameters" + infoAutoBalancer)
         return 'e'
         
-   return BalancedInputs, BalancedLabels
+   return BalancedInputs, BalancedLabels
+   
+   
+def GetWeights():
+        
+    return[0]
+    
+def GetDf():
+        
+    return[6]
+    
+def GetPreds():
+        
+    return[1]
+    
+def GetAcc():
+        
+    return[2]
+
+def GetAllFromLoad():
+    
+    return[0],[1],[2],[3],[4],[5]
+
```

