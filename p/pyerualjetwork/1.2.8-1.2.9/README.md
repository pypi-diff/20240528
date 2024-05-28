# Comparing `tmp/pyerualjetwork-1.2.8.tar.gz` & `tmp/pyerualjetwork-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerualjetwork-1.2.8.tar", last modified: Mon May 27 17:55:30 2024, max compression
+gzip compressed data, was "pyerualjetwork-1.2.9.tar", last modified: Tue May 28 20:35:49 2024, max compression
```

## Comparing `pyerualjetwork-1.2.8.tar` & `pyerualjetwork-1.2.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 17:55:30.763762 pyerualjetwork-1.2.8/
--rw-rw-rw-   0        0        0      446 2024-05-27 17:55:30.761766 pyerualjetwork-1.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-27 17:55:30.738264 pyerualjetwork-1.2.8/plan/
--rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.2.8/plan/__init__.py
--rw-rw-rw-   0        0        0    40457 2024-05-27 17:53:28.000000 pyerualjetwork-1.2.8/plan/plan.py
-drwxrwxrwx   0        0        0        0 2024-05-27 17:55:30.759764 pyerualjetwork-1.2.8/pyerualjetwork.egg-info/
--rw-rw-rw-   0        0        0      446 2024-05-27 17:55:30.000000 pyerualjetwork-1.2.8/pyerualjetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-27 17:55:30.000000 pyerualjetwork-1.2.8/pyerualjetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 17:55:30.000000 pyerualjetwork-1.2.8/pyerualjetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-27 17:55:30.000000 pyerualjetwork-1.2.8/pyerualjetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 17:55:30.763762 pyerualjetwork-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-05-27 17:55:02.000000 pyerualjetwork-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:35:49.753892 pyerualjetwork-1.2.9/
+-rw-rw-rw-   0        0        0      452 2024-05-28 20:35:49.752888 pyerualjetwork-1.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-28 20:35:49.698391 pyerualjetwork-1.2.9/plan/
+-rw-rw-rw-   0        0        0      352 2024-05-26 16:54:30.000000 pyerualjetwork-1.2.9/plan/__init__.py
+-rw-rw-rw-   0        0        0    42347 2024-05-28 20:20:20.000000 pyerualjetwork-1.2.9/plan/plan.py
+drwxrwxrwx   0        0        0        0 2024-05-28 20:35:49.748899 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/
+-rw-rw-rw-   0        0        0      452 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-28 20:35:49.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-28 20:35:48.000000 pyerualjetwork-1.2.9/pyerualjetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 20:35:49.754880 pyerualjetwork-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      864 2024-05-28 20:35:41.000000 pyerualjetwork-1.2.9/setup.py
```

### Comparing `pyerualjetwork-1.2.8/plan/plan.py` & `pyerualjetwork-1.2.9/plan/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import numpy as np
 import time
 from colorama import Fore,Style
 from typing import List, Union
 import math
 from scipy.special import expit, softmax
+import matplotlib.pyplot as plt
+import seaborn as sns
 
 # BUILD -----
 def TrainPLAN(
     TrainInputs: List[Union[int, float]], 
     TrainLabels: List[Union[int, float, str]], # At least two.. and one hot encoded
     ClassCount: int,
     Layers: List[str],
     Neurons: List[Union[int, float]],
     MembranThresholds: List[str],
     MembranPotentials: List[Union[int, float]],
     Normalizations: List[str],
-    Activations: List[str]
+    Activations: List[str],
+    Visualize: str
 ) -> str:
         
     infoPLAN = """
     Creates and configures a PLAN model.
     
     Args:
         TrainInputs (list[num]): List of input data.
@@ -27,20 +30,26 @@
         ClassCount (int): Number of classes.
         Layers (list[str]): List of layer names. (options: 'fex' (Feature Extraction), 'cat' (Catalyser))
         Neurons (list[num]): List of neuron counts for each layer.
         MembranThresholds (list[str]): List of MembranThresholds.
         MembranPotentials (list[num]): List of MembranPotentials.
         Normalizations (List[str]): Whether normalization will be performed at indexed layers ("y" or "n").
         Activations (list[str]): List of activation functions.
+        Visualize (str): Visualize Training procces or not visualize ('y' or 'n')
     
     Returns:
         list([num]): (Weight matrices list, TrainPredictions list, TrainAcc).
         error handled ?: Process status ('e')
 """
         
+    if Visualize != 'y' and Visualize != 'n':
+        print(Fore.RED + "ERROR109: Visualize parameter must be 'y' or 'n'. TrainPLAN",infoPLAN)
+        return 'e'
+        
+    
     LastNeuron = Neurons[-1:][0]
     if LastNeuron != ClassCount:
             print(Fore.RED + "ERROR108: Last layer of neuron count must be equal class count. from: TrainPLAN",infoPLAN)
             return 'e'
     
     if len(Normalizations) != len(MembranPotentials):
         
@@ -138,15 +147,15 @@
     TrainInputs[0] = TrainInputs[0].ravel()
     TrainInputsize = len(TrainInputs[0])
     
     W = WeightIdentification(len(Layers) - 1,ClassCount,Neurons,TrainInputsize)
     Divides = SynapticDividing(ClassCount,W)
     TrainedWs = [1] * len(W)
     print(Fore.GREEN + "Train Started with 0 ERROR" + Style.RESET_ALL,)
-    TrainPredictions = [1] * len(TrainLabels)
+    TrainPredictions = [None] * len(TrainLabels)
     true = 0
     StartTime = time.time()
     for index, inp in enumerate(TrainInputs):
         UniStartTime = time.time()
         inp = np.array(inp)
         inp = inp.ravel()
         
@@ -188,14 +197,32 @@
         RealOutput = np.argmax(TrainLabels[index])
         PredictedOutput = np.argmax(NeuralLayer)
         if RealOutput == PredictedOutput:
             true += 1
         Acc = true / len(TrainLabels)
         TrainPredictions[index] = PredictedOutput
         
+        if Visualize == 'y':
+        
+            TrainLabelsVisual = np.copy(TrainLabels) 
+            TrainLabelsVisual = np.argmax(TrainLabelsVisual, axis=1)
+            
+            plt.figure(figsize=(12, 6))
+            sns.kdeplot(TrainLabelsVisual, label='Real Outputs', shade=True)
+            sns.kdeplot(TrainPredictions, label='Predictions', shade=True)
+            plt.legend()
+            plt.xlabel('Class')
+            plt.ylabel('Data size')
+            plt.title('Predictions and Real Outputs for Training KDE Plot')
+            plt.show()
+            
+            if index + 1 != len(TrainInputs):
+            
+                plt.close('all')
+        
         if index == 0:
             for i, w in enumerate(W):
                 TrainedWs[i] = w
                      
         else:
             for i, w in enumerate(W):
                 TrainedWs[i] = TrainedWs[i] + w
@@ -533,15 +560,16 @@
 def TestPLAN(
     TestInputs,         # list[list[num]]: Test input data.
     TestLabels,         # list[num]: Test labels.
     Layers,             # list[str]: List of layer names.
     MembranThresholds,     # list[str]: List of MEMBRAN THRESHOLDS for each layer.
     MembranPotentials,    # list[num]: List of MEMBRAN POTENTIALS for each layer.
     Normalizations,    # str: Whether normalization will be performed ("y" or "n").
-    Activations,         # str: Activation function list for the neural network.
+    Activations,       # str: Activation function list for the neural network.
+    Visualize,         # Visualize Testing procces or not visualize ('y' or 'n')
     W                  # list[list[num]]: Weight matrix of the neural network.
 ) -> tuple:
     infoTestModel =  """
     Tests the neural network model with the given test data.
 
     Args:
         TestInputs (list[list[num]]): Test input data.
@@ -557,15 +585,15 @@
         tuple: A tuple containing the predicted labels and the accuracy of the model.
     """
 
 
     try:
         Wc = [0] * len(W)
         true = 0
-        TestPredictions = [1] * len(TestLabels)
+        TestPredictions = [None] * len(TestLabels)
         for i, w in enumerate(W):
             Wc[i] = np.copy(w)
             print('\rCopying weights.....',i+1,'/',len(W),end = "")
                 
         print(Fore.GREEN + "\n\nTest Started with 0 ERROR\n" + Style.RESET_ALL)
         StartTime = time.time()
         for inpIndex,Input in enumerate(TestInputs):
@@ -592,14 +620,33 @@
                 W[i] = np.copy(w)
             RealOutput = np.argmax(TestLabels[inpIndex])
             PredictedOutput = np.argmax(NeuralLayer)
             if RealOutput == PredictedOutput:
                 true += 1
             Acc = true / len(TestLabels)
             TestPredictions[inpIndex] = PredictedOutput
+            
+            if Visualize == 'y':
+            
+                TestLabelsVisual = np.copy(TestLabels) 
+                TestLabelsVisual = np.argmax(TestLabelsVisual, axis=1)
+                
+                plt.figure(figsize=(12, 6))
+                sns.kdeplot(TestLabelsVisual, label='Real Outputs', shade=True)
+                sns.kdeplot(TestPredictions, label='Predictions', shade=True)
+                plt.legend()
+                plt.xlabel('Class')
+                plt.ylabel('Data size')
+                plt.title('Predictions and Real Outputs for Testing KDE Plot')
+                plt.show()
+                
+                if inpIndex + 1 != len(TestInputs):
+                
+                    plt.close('all')
+            
             UniEndTime = time.time()
                 
             CalculatingEst = round((UniEndTime - UniStartTime) * (len(TestInputs) - inpIndex),3)
                 
             if CalculatingEst < 60:
                 print('\rest......(sec):',CalculatingEst,'\n',end= "")
                 print('\rTest Accuracy: ' ,Acc ,"\n", end="")
@@ -1041,8 +1088,8 @@
     
 def GetPreds():
         
     return 1
     
 def GetAcc():
         
-    return 2
+    return 2
```

