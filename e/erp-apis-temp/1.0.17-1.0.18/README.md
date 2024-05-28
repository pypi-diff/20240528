# Comparing `tmp/erp_apis_temp-1.0.17-py3-none-any.whl.zip` & `tmp/erp_apis_temp-1.0.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 14789 bytes, number of entries: 15
+Zip file size: 14774 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     2347 b- defN 24-May-15 02:53 erp_apis_temp/config.py
 -rw-rw-rw-  2.0 fat     3636 b- defN 24-May-13 01:43 erp_apis_temp/erpRequest.py
 -rw-rw-rw-  2.0 fat     4710 b- defN 24-May-28 10:13 erp_apis_temp/apis/afterSales.py
 -rw-rw-rw-  2.0 fat     4471 b- defN 24-May-13 09:46 erp_apis_temp/apis/aftersale_test.py
 -rw-rw-rw-  2.0 fat     1538 b- defN 24-May-09 01:56 erp_apis_temp/apis/goods.py
 -rw-rw-rw-  2.0 fat     1013 b- defN 24-May-09 01:56 erp_apis_temp/apis/inventory.py
 -rw-rw-rw-  2.0 fat     4371 b- defN 24-May-13 01:43 erp_apis_temp/apis/order.py
--rw-rw-rw-  2.0 fat     3093 b- defN 24-May-12 12:12 erp_apis_temp/apis/refund.py
+-rw-rw-rw-  2.0 fat     3071 b- defN 24-May-28 10:28 erp_apis_temp/apis/refund.py
 -rw-rw-rw-  2.0 fat     2499 b- defN 24-May-13 01:44 erp_apis_temp/apis/test.py
 -rw-rw-rw-  2.0 fat     1139 b- defN 24-May-09 01:56 erp_apis_temp/apis/user.py
 -rw-rw-rw-  2.0 fat     2163 b- defN 24-May-13 07:20 erp_apis_temp/utils/util.py
--rw-rw-rw-  2.0 fat     1540 b- defN 24-May-28 10:16 erp_apis_temp-1.0.17.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 10:16 erp_apis_temp-1.0.17.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 24-May-28 10:16 erp_apis_temp-1.0.17.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1263 b- defN 24-May-28 10:16 erp_apis_temp-1.0.17.dist-info/RECORD
-15 files, 33928 bytes uncompressed, 12695 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 fat     1540 b- defN 24-May-28 10:28 erp_apis_temp-1.0.18.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 10:28 erp_apis_temp-1.0.18.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 24-May-28 10:28 erp_apis_temp-1.0.18.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1263 b- defN 24-May-28 10:28 erp_apis_temp-1.0.18.dist-info/RECORD
+15 files, 33906 bytes uncompressed, 12680 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: erp_apis_temp/apis/user.py
 Comment: 
 
 Filename: erp_apis_temp/utils/util.py
 Comment: 
 
-Filename: erp_apis_temp-1.0.17.dist-info/METADATA
+Filename: erp_apis_temp-1.0.18.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis_temp-1.0.17.dist-info/WHEEL
+Filename: erp_apis_temp-1.0.18.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis_temp-1.0.17.dist-info/top_level.txt
+Filename: erp_apis_temp-1.0.18.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis_temp-1.0.17.dist-info/RECORD
+Filename: erp_apis_temp-1.0.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis_temp/apis/refund.py

```diff
@@ -91,27 +91,27 @@
             }
         ),
     },
         method='Finishs'
     )
 
 # 确认退款订单
-def confirm(pay_id: Union[str, int]):
+def confirm(pay_ids):
     '''
     确认售后订单
     :param oid:  内部订单号
     :return: 执行结果
     '''
     return RefundRequest({
         'isCB': '0',
         '__CALLBACKID': 'ACall1',
         '__CALLBACKPARAM': dumps(
             {
                 "Method": "Confirms",
-                "Args": [str(pay_id)],
+                "Args": pay_ids,
              "CallControl": "{page}"
             }
         ),
     },
         method='Confirms',
         url='/app/order/refund/refund.aspx'
     )
```

## Comparing `erp_apis_temp-1.0.17.dist-info/METADATA` & `erp_apis_temp-1.0.18.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp_apis_temp
-Version: 1.0.17
+Version: 1.0.18
 Summary: erp_apis_temp
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
 Project-URL: Source Code, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis_temp-1.0.17.dist-info/RECORD` & `erp_apis_temp-1.0.18.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 erp_apis_temp/config.py,sha256=RVm2hs1j0J_Kb8sYbd-r29bzNRWSpR-gJcYnNc3RNPY,2347
 erp_apis_temp/erpRequest.py,sha256=b_6Z9glqi0wkvSG4LKgRx-Z53CXgK2ihycN61D8g20A,3636
 erp_apis_temp/apis/afterSales.py,sha256=f31n0Pv5RugB-CBrh4jOAqKQIjCk6lcy8R_sAzq-hms,4710
 erp_apis_temp/apis/aftersale_test.py,sha256=FjsYknNWL-It4otccyMtqNmcNqLgLIgXG3RqWxcgUdo,4471
 erp_apis_temp/apis/goods.py,sha256=3HplLv-feqNMiV46ANuzhRfL9RDiOovF8RAAvNydmdI,1538
 erp_apis_temp/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
 erp_apis_temp/apis/order.py,sha256=yCw8OhCJjvGjOMmI_gY9p4C_xROQWs062-iaJ9L7evw,4371
-erp_apis_temp/apis/refund.py,sha256=oUvhwQ3JOj-0XS2DZDPEfZWtJGVFtXty0CcpRMd9_B4,3093
+erp_apis_temp/apis/refund.py,sha256=pAzPpOoTzjWCl0QMpUVRHUQFnPHlZZK3qEkWjUoi7kU,3071
 erp_apis_temp/apis/test.py,sha256=XrWoVqJFoZxm1MTZcQ8h5kn341VWjPNGfvxg12mUXkE,2499
 erp_apis_temp/apis/user.py,sha256=vosgBp1QNesLIRMQyafe9y9PDFJyIjpPdmiE1jvVzOA,1139
 erp_apis_temp/utils/util.py,sha256=Jb9GOlGrYJDLuE8EjsjUbKb_L-VzdqTZkIN4Mgm18Yc,2163
-erp_apis_temp-1.0.17.dist-info/METADATA,sha256=lmu8hsuqsocFZjYv-oc9V3xcnODSlV8scgCmSR7S6Ms,1540
-erp_apis_temp-1.0.17.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis_temp-1.0.17.dist-info/top_level.txt,sha256=aTOkhDHreCOYKk-4ZEmPt3WkWpC71zChCYS9RykowuI,53
-erp_apis_temp-1.0.17.dist-info/RECORD,,
+erp_apis_temp-1.0.18.dist-info/METADATA,sha256=QFuVXixemVPKopakY6Y6dunWvfI_QIFY2rCCeMFhR08,1540
+erp_apis_temp-1.0.18.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis_temp-1.0.18.dist-info/top_level.txt,sha256=aTOkhDHreCOYKk-4ZEmPt3WkWpC71zChCYS9RykowuI,53
+erp_apis_temp-1.0.18.dist-info/RECORD,,
```

