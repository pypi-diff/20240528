# Comparing `tmp/gwml-0.1.6-py3-none-any.whl.zip` & `tmp/gwml-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 98499 bytes, number of entries: 63
+Zip file size: 98012 bytes, number of entries: 63
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 08:56 gwml/__init__.py
 -rw-r--r--  2.0 unx     1521 b- defN 24-May-28 09:02 gwml/_command.py
 -rw-r--r--  2.0 unx      206 b- defN 24-May-28 09:02 gwml/_main.py
 -rw-r--r--  2.0 unx     6180 b- defN 24-May-28 09:02 gwml/command.py
 -rw-r--r--  2.0 unx      797 b- defN 24-May-28 09:02 gwml/main.py
 -rw-r--r--  2.0 unx      104 b- defN 24-May-28 08:56 gwml/mldump.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 09:02 gwml/cmdLib/__init__.py
@@ -52,14 +52,14 @@
 -rw-r--r--  2.0 unx     1181 b- defN 24-May-28 08:56 gwml/lib/common/sfds/reg/regModel.py
 -rw-r--r--  2.0 unx       22 b- defN 24-May-28 08:56 gwml/lib/common/trainer/__init__.py
 -rw-r--r--  2.0 unx    11894 b- defN 24-May-28 08:56 gwml/lib/common/trainer/customTrainer.py
 -rw-r--r--  2.0 unx    10834 b- defN 24-May-28 08:56 gwml/lib/common/trainer/regTrainer.py
 -rw-r--r--  2.0 unx     2317 b- defN 24-May-28 08:56 gwml/lib/common/utils/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-28 08:56 gwml/lib/reg/__init__.py
 -rw-r--r--  2.0 unx     5131 b- defN 24-May-28 08:56 gwml/lib/reg/regDecorator.py
--rw-r--r--  2.0 unx    24563 b- defN 24-May-28 08:56 gwml/lib/reg/regTrainer.py
--rw-r--r--  2.0 unx       49 b- defN 24-May-28 09:16 gwml-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-28 09:16 gwml-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 24-May-28 09:16 gwml-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-28 09:16 gwml-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5519 b- defN 24-May-28 09:16 gwml-0.1.6.dist-info/RECORD
-63 files, 321791 bytes uncompressed, 89623 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx    22656 b- defN 24-May-28 10:24 gwml/lib/reg/regTrainer.py
+-rw-r--r--  2.0 unx       49 b- defN 24-May-28 10:26 gwml-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 10:26 gwml-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 24-May-28 10:26 gwml-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-28 10:26 gwml-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     5519 b- defN 24-May-28 10:26 gwml-0.1.7.dist-info/RECORD
+63 files, 319884 bytes uncompressed, 89136 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -168,23 +168,23 @@
 
 Filename: gwml/lib/reg/regDecorator.py
 Comment: 
 
 Filename: gwml/lib/reg/regTrainer.py
 Comment: 
 
-Filename: gwml-0.1.6.dist-info/METADATA
+Filename: gwml-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: gwml-0.1.6.dist-info/WHEEL
+Filename: gwml-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: gwml-0.1.6.dist-info/entry_points.txt
+Filename: gwml-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: gwml-0.1.6.dist-info/top_level.txt
+Filename: gwml-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: gwml-0.1.6.dist-info/RECORD
+Filename: gwml-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwml/lib/reg/regTrainer.py

```diff
@@ -32,59 +32,40 @@
 import joblib
 import pickle
 import torch
 
 
 basePath = os.path.abspath(os.path.join(os.path.join(os.path.dirname(__file__), os.path.pardir)))
 commonPath = os.path.join((os.path.dirname(os.path.dirname(os.path.abspath(__file__)))),"common") # os.path.abspath("../common")
-modelPath = os.path.abspath(
-    os.path.join(
-        os.path.join(
-            os.path.join(os.path.dirname(__file__), os.path.pardir), os.path.pardir
-        ),
-        "modeldata/WEDA-Custom",
-    )
-)  # modeldata 위치
+# modelPath = "../../legacy" # modeldata 위치
 
-# sys.path.append(basePath)
+sys.path.append(basePath)
 sys.path.append(commonPath)
-# sys.path.append(os.path.join(basePath, "model"))
-# sys.path.append(os.path.join(basePath, "bin"))
-sys.path.append(os.path.join(commonPath, "graph"))
-sys.path.append(os.path.join(commonPath, "decorator"))
-sys.path.append(os.path.join(commonPath, "sender"))
-sys.path.append(os.path.join(commonPath, "datalib"))
-sys.path.append(os.path.join(commonPath, "utils"))
-
 
+from hyperopt import fmin, tpe, hp, STATUS_OK, Trials, STATUS_FAIL
 from sender.sender import sendMsg
 from graph.graph import graph
-from error.WedaErrorDecorator import WedaErrorDecorator
 from logger.WedaLogDecorator import WedaLogDecorator
-from hyperopt import fmin, tpe, hp, STATUS_OK, Trials, STATUS_FAIL
+from error.WedaErrorDecorator import WedaErrorDecorator
 from logger.Logger import Logger
-from dataLib import dataLib
+from datalib.dataLib import dataLib
 from utils.utils import utils
 
 # from wedaLib.reg import regDecorator
 
 
 class trainer:
     # @WedaLogDecorator(text="Train Start...", logLevel="info")
     def __init__(self, param, xTrain, xTest, yTrain, yTest, startTime, lm, log=None):
 
         self.param = param
         self.startTime = startTime
         self.dataInfo = param["dataInfo"] if "dataInfo" in param else None
         self.serverParam = param["serverParam"] if "serverParam" in param else None
-        self.selectedHyperParam = (
-            utils.getHyperParam(param["selectedHyperParam"], modelPath)
-            if param["selectedHyperParam"]
-            else param["selectedHyperParam"]
-        )
+        self.selectedHyperParam = param["selectedHyperParam"]
 
         self.timeColumn = self.dataInfo.get("timeColumn", "")
         self.purposeType = self.dataInfo["purposeType"]
         self.targetColumn = self.dataInfo["targetColumn"]
         self.classList = [
             i["className"] for i in param["dataInfo"].get("classInfo", [])
         ]
@@ -341,15 +322,16 @@
     @WedaLogDecorator(text="Running Trainer...", logLevel="info")
     def getTrainResult(self, startTime, hpoTf, sendResultUrl, log):
         output = {"status": 200, "massage": "", "result": {}}
 
         st = time.time()
 
         # custom model fit
-        lm = self.customLM(startTime=self.startTime, param=self.param)
+        param_grid = self.selectedHyperParam
+        lm = self.customLM(startTime=self.startTime, param=self.param, param_grid=param_grid)
         lm.model = lm.createModel()
 
         hyperParameter = {"hyperParammeter": []}
         for key in self.selectedHyperParam:
             hyperParam = {}
             if self.hyperscheme[key]["type"] == "int":
                 self.selectedHyperParam[key] = int(self.selectedHyperParam[key])
@@ -412,53 +394,14 @@
             output["xaiResult"] = xaiResult["result"]
             output["xaiExtTime"] = time.time() - st
             _ = sendMsg(sendResultUrl, output, "XAI", log)
 
         return output
 
 
-# opr에서 모델 입출력 스키마 정의
-def setModelInfo(scheme):
-    subList = []
-    for i in scheme["dataInfo"]["columnList"]:
-        subList.append(
-            {
-                "type": "string" if i["columnType"] == "string" else "number",
-                "name": i["columnName"],
-            }
-        )
-
-    inputScheme = [
-        {
-            "type": "object",
-            "name": "opData",
-            "subObject": [
-                {"type": "array", "name": "header", "subList": subList},
-                {"type": "array", "name": "xTest"},
-            ],
-        }
-    ]
-
-    # output 타입, 분류 등 다른 모델에서 OPR에서 다르게 나올 경우 수정 필요
-    subList.append({"type": "string", "name": "errMessage"})
-    subList.append({"type": "number", "name": "label"})
-    subList.append({"type": "number", "name": "accuracy"})
-
-    outputScheme = [
-        {"type": "array", "name": "opResult", "subList": subList},
-        {"type": "string", "name": "modelId"},
-    ]
-    with open(os.path.join(basePath, "modelInfo.json"), "r+") as jsonFile:
-        file_data = json.load(jsonFile)
-        file_data["ioScheme"] = {}
-        file_data["ioScheme"]["inputScheme"] = inputScheme
-        file_data["ioScheme"]["outputScheme"] = outputScheme
-        jsonFile.seek(0)
-        json.dump(file_data, jsonFile, indent=4)
-
 
 @WedaLogDecorator(text="Model Training...", logLevel="info")
 def runCustomHPO(params, df, startTime, hpoOption, sendResultUrl, lm, log):
 
     # 데이터 취득
     dl = dataLib(param=params, log=log)
     data = dl.getData(dataFrame=df, log=log)
@@ -477,32 +420,34 @@
         yTrain=yTrain,
         yTest=yTest,
         lm=lm,
         startTime=startTime,
     )
 
     space = {}
-    hyperparam = hpoOption["hyperParamScheme"]
-
+    hyperParamScheme = hpoOption["hyperParamScheme"]
+    space = lm.getSpace(hyperParamScheme) 
+    
+    
     # learningModel.getSpace() 대신
-    for key, value in hyperparam.items():
-        if value.get("q", "") != "":
-            if value["type"] == "int":
-                space[key] = hp.quniform(key, value["min"], value["max"], value["q"])
-            elif value["type"] == "float":
-                space[key] = hp.quniform(key, value["min"], value["max"], value["q"])
-        else:
-            if value["type"] == "int":
-                space[key] = hp.uniform(key, value["min"], value["max"])
+    # for key, value in hyperParamScheme.items():
+    #     if value.get("q", "") != "":
+    #         if value["type"] == "int":
+    #             space[key] = hp.quniform(key, value["min"], value["max"], value["q"])
+    #         elif value["type"] == "float":
+    #             space[key] = hp.quniform(key, value["min"], value["max"], value["q"])
+    #     else:
+    #         if value["type"] == "int":
+    #             space[key] = hp.uniform(key, value["min"], value["max"])
 
-            elif value["type"] == "float":
-                space[key] = hp.uniform(key, value["min"], value["max"])
+    #         elif value["type"] == "float":
+    #             space[key] = hp.uniform(key, value["min"], value["max"])
 
-            elif value["type"] == "str":
-                space[key] = hp.choice(key, value["value"])
+    #         elif value["type"] == "str":
+    #             space[key] = hp.choice(key, value["value"])
 
     if "trialCount" in t.param:
         trialCount = int(t.param["trialCount"])
     else:
         trialCount = 10
 
     # Trials 객체 선언합니다.
@@ -516,15 +461,15 @@
         max_evals=trialCount,  # 최대 반복 횟수를 지정합니다.
         trials=trials,
     )
 
     # convertParam 대신
     for i, v in best.items():
         if t.hyperscheme[i]["type"] == "str":
-            best[i] = hyperparam[i]["value"][v]
+            best[i] = hyperParamScheme[i]["value"][v]
 
     # 최적화된 결과를 int로 변환해야하는 파라미터는 타입 변환을 수행합니다.
     for key in best:
         if type(best[key]) == np.float64:
             best[key] = round(float(best[key]), 5)
         elif type(best[key]) == np.int64:
             best[key] = int(best[key])
@@ -544,17 +489,14 @@
     re.selectedHyperParam = best
     output = re.getTrainResult(
         startTime=startTime, hpoTf=True, sendResultUrl=sendResultUrl, log=log
     )
 
     print("re train done")
 
-    # opr에서 모델 입출력 스키마 정의 함수 호출
-    setModelInfo(re.param)
-
     with open(os.path.join(basePath, "param.json"), "w") as jsonFile:
         json.dump(re.param, jsonFile, ensure_ascii=False)
 
     return output
 
 
 def runCustomTrain(params, df, startTime, sendResultUrl, lm, log):
@@ -604,14 +546,15 @@
     df : 학습할 dataframe
     lm : 사용자가 정의한 lm 클래스
     target : 학습 타겟
     graph : 그래프 계산 유무
     xai : xai 계산 유무
     splitInfo : 학습, 테스트 비율
     hyperParams : 모델의 하이퍼 파라미터
+    hyperParamScheme: 파라미터 형태
     graphList: grapTf가 True일 떄 그릴 그래프 종류 (reg: regPlot, distribution Plot, Feature Importance)
     savePath: 모델, 그래프 등등 저장할 경로
     """
     validRatio = 100 - splitInfo
     splitInfo = {"validRatio": validRatio}
 
     startTime = datetime.datetime.now()
@@ -626,18 +569,18 @@
         {"columnName": col, "columnType": str(df[col].dtype)} for col in df.columns
     ]
 
     dataInfo["splitInfo"] = splitInfo
     dataInfo["hyperParam"] = hyperParams
     dataInfo["savePath"] = savePath
     dataInfo["graphList"] = graphList
+    
     data = {
         "runType": "custom",
         "dataInfo": dataInfo,
-        "splitInfo": splitInfo,
         "selectedHyperParam": hyperParams,
         "pathInfo": {},
         "selectedHyperParam": {},
         "hyperParamScheme": hyperParamScheme,
         "graphTf": graph,
         "xaiTf": xai,
     }
@@ -657,15 +600,15 @@
     return output
 
 
 def hpo(
     df,
     lm,
     hyperParamScheme={},
-    splitInfo=0.7,
+    splitInfo=70,
     target="",
     graph=False,
     xai=False,
     trialCount=10,
     savePath="./",
 ):
     """
@@ -676,19 +619,20 @@
     xai : xai 계산 유무
     splitInfo : 학습, 테스트 비율
     trialCount : 파라미터를 찾는 trial 횟수
     hyperParamScheme : 모델의 하이퍼 정보({"파라미터명": {"min": 0, "max": 100, "type":"float", "q":0.05, "defaultValue": 1.3},})
     graphList: grapTf가 True일 떄 그릴 그래프 종류 (reg: regPlot, distribution Plot, Feature Importance)
     savePath: 모델, 그래프 등등 저장할 경로
     """
-
+    validRatio = 100 - splitInfo
+    splitInfo = {"validRatio": validRatio}
+    
     hpoOption = {
         "graphTf": graph,
         "xaiTf": xai,
-        "splitInfo": splitInfo,
         "hyperParamScheme": hyperParamScheme,
         "savePath": savePath,
     }
 
     startTime = datetime.datetime.now()
 
     dataInfo = {}
@@ -698,19 +642,19 @@
 
     dataInfo["targetColumn"] = target
     dataInfo["purposeType"] = "regression"
     dataInfo["sourceType"] = "dataframe"
     dataInfo["columnList"] = [
         {"columnName": col, "columnType": str(df[col].dtype)} for col in df.columns
     ]
+    dataInfo["splitInfo"] = splitInfo
     
     data = {
         "runType": "custom",
         "dataInfo": dataInfo,
-        "splitInfo": hpoOption["splitInfo"],
         "trialCount": trialCount,
         "hyperParamScheme": hyperParamScheme,
         "selectedHyperParam": {},
         "pathInfo": {},
     }
 
     data = json.dumps(data)
```

## Comparing `gwml-0.1.6.dist-info/RECORD` & `gwml-0.1.7.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -51,13 +51,13 @@
 gwml/lib/common/sfds/reg/regModel.py,sha256=4ZnjqsGr8u0gEh6nnz8m47jexOlJZhJXIGuBkjDq-xM,1181
 gwml/lib/common/trainer/__init__.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 gwml/lib/common/trainer/customTrainer.py,sha256=05rWhPyD0xcbBV8FTkHBR2igBlEZPOfyyJhekcjuzUQ,11894
 gwml/lib/common/trainer/regTrainer.py,sha256=BXupe-vk72dLZ0Bp8NZq5O2bJ4sHVYQVeFg-SDQyOfw,10834
 gwml/lib/common/utils/utils.py,sha256=auXrdDqukRQnAOsRBAxioLvsocyniZeoh3eGjnZlrsA,2317
 gwml/lib/reg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwml/lib/reg/regDecorator.py,sha256=lkN5pxnutUvjWjk44Uz1w3QGCSVYuYZirSCrIL7VlSQ,5131
-gwml/lib/reg/regTrainer.py,sha256=6Qv1ploKZpGGCpEu4_7k4zLaEaAUOv8IrTuVMOoddvk,24563
-gwml-0.1.6.dist-info/METADATA,sha256=6_z4seRp5U8LKVt5ynyd5e_UlT7EvSdDAUTj_JNUd3M,49
-gwml-0.1.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-gwml-0.1.6.dist-info/entry_points.txt,sha256=imL6Gb7yRsNcKwqqUM7kpMULMW5smUSYZSX7i_BVdmo,40
-gwml-0.1.6.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
-gwml-0.1.6.dist-info/RECORD,,
+gwml/lib/reg/regTrainer.py,sha256=HUxT7UHvsS_1ZqmqU5d8Bqdw_3lYecOa88Bnl_muemE,22656
+gwml-0.1.7.dist-info/METADATA,sha256=TI-JvsGRoyCr0EF7phbR_jBc0UTutwenU9wxg45F27Y,49
+gwml-0.1.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+gwml-0.1.7.dist-info/entry_points.txt,sha256=imL6Gb7yRsNcKwqqUM7kpMULMW5smUSYZSX7i_BVdmo,40
+gwml-0.1.7.dist-info/top_level.txt,sha256=-Ib3RiOMqlhiZ_idfsP2Unxpw70_Lzk5xN0I7vWHuAQ,5
+gwml-0.1.7.dist-info/RECORD,,
```

