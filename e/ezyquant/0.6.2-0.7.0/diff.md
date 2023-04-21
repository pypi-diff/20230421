# Comparing `tmp/ezyquant-0.6.2.tar.gz` & `tmp/ezyquant-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-0.6.2.tar", last modified: Thu Apr 20 12:13:28 2023, max compression
+gzip compressed data, was "ezyquant-0.7.0.tar", last modified: Fri Apr 21 06:29:51 2023, max compression
```

## Comparing `ezyquant-0.6.2.tar` & `ezyquant-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-20 12:13:05.000000 ezyquant-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 12:13:28.672164 ezyquant-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-20 12:13:05.000000 ezyquant-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/ezyquant/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/ezyquant/backtesting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/backtesting/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    81847 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-20 12:13:05.000000 ezyquant-0.6.2/ezyquant/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/ezyquant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 12:13:28.000000 ezyquant-0.6.2/ezyquant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-20 12:13:28.676164 ezyquant-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-20 12:13:05.000000 ezyquant-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:13:28.672164 ezyquant-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_indicators.py
--rw-r--r--   0 runner    (1001) docker     (123)    60298 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-04-20 12:13:06.000000 ezyquant-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-21 06:29:35.000000 ezyquant-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-21 06:29:51.577684 ezyquant-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-21 06:29:35.000000 ezyquant-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.573684 ezyquant-0.7.0/ezyquant/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/ezyquant/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/backtesting/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27943 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80441 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24832 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-21 06:29:35.000000 ezyquant-0.7.0/ezyquant/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/ezyquant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 06:29:51.000000 ezyquant-0.7.0/ezyquant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 06:29:51.577684 ezyquant-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-21 06:29:35.000000 ezyquant-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:29:51.577684 ezyquant-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_indicators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58450 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20083 2023-04-21 06:29:35.000000 ezyquant-0.7.0/tests/test_utils.py
```

### Comparing `ezyquant-0.6.2/LICENSE.txt` & `ezyquant-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/PKG-INFO` & `ezyquant-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.6.2
+Version: 0.7.0
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.6.2/README.md` & `ezyquant-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/backtesting/_backtesting.py` & `ezyquant-0.7.0/ezyquant/backtesting/_backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/backtesting/account.py` & `ezyquant-0.7.0/ezyquant/backtesting/account.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/backtesting/backtesting.py` & `ezyquant-0.7.0/ezyquant/backtesting/backtesting.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/backtesting/context.py` & `ezyquant-0.7.0/ezyquant/backtesting/context.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/backtesting/position.py` & `ezyquant-0.7.0/ezyquant/backtesting/position.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/backtesting/trade.py` & `ezyquant-0.7.0/ezyquant/backtesting/trade.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/connect.py` & `ezyquant-0.7.0/ezyquant/connect.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/creator.py` & `ezyquant-0.7.0/ezyquant/creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/fields.py` & `ezyquant-0.7.0/ezyquant/fields.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/indicators.py` & `ezyquant-0.7.0/ezyquant/indicators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/reader.py` & `ezyquant-0.7.0/ezyquant/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,33 +338,23 @@
         -------
         pd.DataFrame
             company info dataframe contain columns:
                 - company_id: int - I_COMPANY
                 - symbol: str - SECURITY.N_SECURITY
                 - company_name_t: str - N_COMPANY_T
                 - company_name_e: str - N_COMPANY_E
-                - address_t: str - A_COMPANY_T
-                - address_e: str - A_COMPANY_E
-                - zip: str - I_ZIP
-                - tel: str - E_TEL
-                - fax: str - E_FAX
-                - email: str - E_EMAIL
-                - url: str - E_URL
-                - establish: date - D_ESTABLISH
-                - dvd_policy_t: str - E_DVD_POLICY_T
-                - dvd_policy_e: str - E_DVD_POLICY_E
 
         Examples
         --------
         >>> from ezyquant import SETDataReader
         >>> sdr = SETDataReader()
         >>> sdr.get_company_info(symbol_list=["BBL", "PTT"])
-           company_id symbol               company_name_t  ...  establish                                       dvd_policy_t                                       dvd_policy_e
-        0           1    BBL  ธนาคารกรุงเทพ จำกัด (มหาชน)  ...  1/12/1944  เมื่อผลประกอบการของธนาคารมีกำไร (โดยมีเงื่อนไข...  Pays when company has profit (with additional ...
-        1         646    PTT    บริษัท ปตท. จำกัด (มหาชน)  ...  1/10/2001  ไม่ต่ำกว่าร้อยละ 25 ของกำไรสุทธิที่เหลือหลังหั...  Not less than 25% of net income after deductio...
+           company_id symbol               company_name_t                       company_name_e
+        0           1    BBL    ธนาคารกรุงเทพ จำกัด (มหาชน)  BANGKOK BANK PUBLIC COMPANY LIMITED
+        1         646    PTT     บริษัท ปตท. จำกัด (มหาชน)           PTT PUBLIC COMPANY LIMITED
         """
         warnings.warn(
             "This function will be deprecated in the future.", DeprecationWarning
         )
         company_t = self._table("COMPANY")
         security_t = self._table("SECURITY")
 
@@ -373,24 +363,14 @@
         )
         stmt = (
             select(
                 company_t.c.I_COMPANY.label("company_id"),
                 func.trim(security_t.c.N_SECURITY).label("symbol"),
                 company_t.c.N_COMPANY_T.label("company_name_t"),
                 company_t.c.N_COMPANY_E.label("company_name_e"),
-                company_t.c.A_COMPANY_T.label("address_t"),
-                company_t.c.A_COMPANY_E.label("address_e"),
-                company_t.c.I_ZIP.label("zip"),
-                company_t.c.E_TEL.label("tel"),
-                company_t.c.E_FAX.label("fax"),
-                company_t.c.E_EMAIL.label("email"),
-                company_t.c.E_URL.label("url"),
-                func.trim(company_t.c.D_ESTABLISH).label("establish"),
-                company_t.c.E_DVD_POLICY_T.label("dvd_policy_t"),
-                company_t.c.E_DVD_POLICY_E.label("dvd_policy_e"),
             )
             .select_from(from_clause)
             .order_by(company_t.c.I_COMPANY)
         )
 
         stmt = self._filter_str_in_list(
             stmt=stmt, column=security_t.c.N_SECURITY, values=symbol_list
```

### Comparing `ezyquant-0.6.2/ezyquant/report.py` & `ezyquant-0.7.0/ezyquant/report.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/utils.py` & `ezyquant-0.7.0/ezyquant/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant/validators.py` & `ezyquant-0.7.0/ezyquant/validators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/ezyquant.egg-info/PKG-INFO` & `ezyquant-0.7.0/ezyquant.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant
-Version: 0.6.2
+Version: 0.7.0
 Summary: Powerful backtest python library for Thai stocks
 Home-page: https://www.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-0.6.2/ezyquant.egg-info/SOURCES.txt` & `ezyquant-0.7.0/ezyquant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/setup.py` & `ezyquant-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/tests/test_creator.py` & `ezyquant-0.7.0/tests/test_creator.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/tests/test_indicators.py` & `ezyquant-0.7.0/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/tests/test_reader.py` & `ezyquant-0.7.0/tests/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,48 +372,16 @@
         # Test
         result = sdr.get_company_info(["PTT"])
 
         # Check
         self._check(result)
 
         expect = pd.DataFrame(
-            [
-                [
-                    646,
-                    "PTT",
-                    "บริษัท ปตท. จำกัด (มหาชน)",
-                    "PTT PUBLIC COMPANY LIMITED",
-                    "555 ถนนวิภาวดีรังสิต แขวงจตุจักร เขตจตุจักร กทม.",
-                    "555 VIBHAVADI RANGSIT ROAD, CHATUCHAK Bangkok",
-                    "10900",
-                    "0-2537-2000",
-                    "0-2537-3498-9",
-                    None,
-                    "http://www.pttplc.com",
-                    "1/10/2001",
-                    "ไม่ต่ำกว่าร้อยละ 25 ของกำไรสุทธิที่เหลือหลังหักเงินสำรองต่างๆ ทุกประเภทที่กฎหมายและบริษัทได้กำหนดไว้ (โดยมีเงื่อนไขเพิ่มเติม)",
-                    "Not less than 25% of net income after deduction of all specified reserves (with additional conditions)",
-                ]
-            ],
-            columns=[
-                "company_id",
-                "symbol",
-                "company_name_t",
-                "company_name_e",
-                "address_t",
-                "address_e",
-                "zip",
-                "tel",
-                "fax",
-                "email",
-                "url",
-                "establish",
-                "dvd_policy_t",
-                "dvd_policy_e",
-            ],
+            [[646, "PTT", "บริษัท ปตท. จำกัด (มหาชน)", "PTT PUBLIC COMPANY LIMITED"]],
+            columns=["company_id", "symbol", "company_name_t", "company_name_e"],
         )
         assert_frame_equal(result, expect)
 
     @pytest.mark.parametrize("symbol_list", [["ABCD"], []])
     def test_empty(self, sdr: SETDataReader, symbol_list: List[str]):
         # Test
         result = sdr.get_company_info(symbol_list)
@@ -424,32 +392,15 @@
 
     @staticmethod
     def _check(result):
         assert isinstance(result, pd.DataFrame)
 
         assert_index_equal(
             result.columns,
-            pd.Index(
-                [
-                    "company_id",
-                    "symbol",
-                    "company_name_t",
-                    "company_name_e",
-                    "address_t",
-                    "address_e",
-                    "zip",
-                    "tel",
-                    "fax",
-                    "email",
-                    "url",
-                    "establish",
-                    "dvd_policy_t",
-                    "dvd_policy_e",
-                ]
-            ),
+            pd.Index(["company_id", "symbol", "company_name_t", "company_name_e"]),
         )
 
         assert pd.notna(result["company_id"]).all()
         assert pd.notna(result["symbol"]).all()
 
         assert result["symbol"].is_unique
```

### Comparing `ezyquant-0.6.2/tests/test_test_utils.py` & `ezyquant-0.7.0/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-0.6.2/tests/test_utils.py` & `ezyquant-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

