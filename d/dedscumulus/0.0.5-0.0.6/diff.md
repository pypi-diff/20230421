# Comparing `tmp/dedscumulus-0.0.5-py3-none-any.whl.zip` & `tmp/dedscumulus-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 24168 bytes, number of entries: 21
+Zip file size: 24242 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Feb-13 21:12 dedscumulus/RequestHandler.py
 -rw-rw-rw-  2.0 fat    14421 b- defN 23-Feb-13 13:17 dedscumulus/SharePointHandler.py
 -rw-rw-rw-  2.0 fat     2250 b- defN 23-Feb-20 20:06 dedscumulus/TableLogHandler.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-May-17 10:12 dedscumulus/__init__.py
 -rw-rw-rw-  2.0 fat     8815 b- defN 23-Feb-21 02:51 dedscumulus/brzGlobal.py
 -rw-rw-rw-  2.0 fat     4990 b- defN 23-Apr-18 16:46 dedscumulus/gbtGlobal.py
--rw-rw-rw-  2.0 fat    13474 b- defN 23-Apr-16 12:34 dedscumulus/mstAst.py
+-rw-rw-rw-  2.0 fat    14481 b- defN 23-Apr-21 02:00 dedscumulus/mstAst.py
 -rw-rw-rw-  2.0 fat      823 b- defN 23-Apr-20 21:56 dedscumulus/mstLog.py
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Feb-13 21:12 src/RequestHandler.py
 -rw-rw-rw-  2.0 fat    14421 b- defN 23-Feb-13 13:17 src/SharePointHandler.py
 -rw-rw-rw-  2.0 fat     2250 b- defN 23-Feb-20 20:06 src/TableLogHandler.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-May-17 10:12 src/__init__.py
 -rw-rw-rw-  2.0 fat     8815 b- defN 23-Feb-21 02:51 src/brzGlobal.py
 -rw-rw-rw-  2.0 fat     4990 b- defN 23-Apr-18 16:46 src/gbtGlobal.py
 -rw-rw-rw-  2.0 fat    13474 b- defN 23-Apr-16 12:34 src/mstAst.py
 -rw-rw-rw-  2.0 fat      823 b- defN 23-Apr-20 21:56 src/mstLog.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-21 01:51 dedscumulus-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      566 b- defN 23-Apr-21 01:51 dedscumulus-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 01:51 dedscumulus-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-21 01:51 dedscumulus-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1655 b- defN 23-Apr-21 01:51 dedscumulus-0.0.5.dist-info/RECORD
-21 files, 94006 bytes uncompressed, 21504 bytes compressed:  77.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-21 02:01 dedscumulus-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      566 b- defN 23-Apr-21 02:01 dedscumulus-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 02:01 dedscumulus-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-21 02:01 dedscumulus-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1655 b- defN 23-Apr-21 02:01 dedscumulus-0.0.6.dist-info/RECORD
+21 files, 95013 bytes uncompressed, 21578 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: src/mstAst.py
 Comment: 
 
 Filename: src/mstLog.py
 Comment: 
 
-Filename: dedscumulus-0.0.5.dist-info/LICENSE
+Filename: dedscumulus-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: dedscumulus-0.0.5.dist-info/METADATA
+Filename: dedscumulus-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: dedscumulus-0.0.5.dist-info/WHEEL
+Filename: dedscumulus-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: dedscumulus-0.0.5.dist-info/top_level.txt
+Filename: dedscumulus-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: dedscumulus-0.0.5.dist-info/RECORD
+Filename: dedscumulus-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dedscumulus/mstAst.py

```diff
@@ -5,258 +5,259 @@
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from azure.keyvault.secrets import SecretClient
 from azure.identity import ManagedIdentityCredential
 from sqlalchemy import create_engine
 import urllib
 
-def getAssetTypes(DB_CRED,logger):
-    current_row=''
-    assetTypes={}
-    try:
-        logger.debug("Starting getAssetTypes")
-        errors=0
-        while errors<3:
-            try:
-                with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
-                    with conn.cursor() as cursor:
-                        cursor.execute("SELECT [AssetTypeId],[ExternalName] FROM [dbo].[mstAssetType] WHERE [ExternalName] IS NOT NULL;")
-                        for row in cursor:
-                            current_row=str(row)
-                            assetTypes[row[1]]=row[0]
-                        return assetTypes
-            except Exception as pe:
-                errors+=1
-                time.sleep(0.05)
-        log_text="mstAst4.getAssetTypes Failed 3 times, stopping execution"
-        logger.error(log_text)
-        return None
-    except Exception as e1:
-        log_text=f"mstAst4.getAssetTypes Failed, error: {e1}, current_row: {current_row}"
-        logger.error(log_text)
-        return None
+class mstAst:
+    def getAssetTypes(DB_CRED,logger):
+        current_row=''
+        assetTypes={}
+        try:
+            logger.debug("Starting getAssetTypes")
+            errors=0
+            while errors<3:
+                try:
+                    with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
+                        with conn.cursor() as cursor:
+                            cursor.execute("SELECT [AssetTypeId],[ExternalName] FROM [dbo].[mstAssetType] WHERE [ExternalName] IS NOT NULL;")
+                            for row in cursor:
+                                current_row=str(row)
+                                assetTypes[row[1]]=row[0]
+                            return assetTypes
+                except Exception as pe:
+                    errors+=1
+                    time.sleep(0.05)
+            log_text="mstAst4.getAssetTypes Failed 3 times, stopping execution"
+            logger.error(log_text)
+            return None
+        except Exception as e1:
+            log_text=f"mstAst4.getAssetTypes Failed, error: {e1}, current_row: {current_row}"
+            logger.error(log_text)
+            return None
 
-def executeCommand(DB_CRED,sql,logger):
-    #this function returns negatie values in case of an error!!!
-    try:
-        #logger.debug(f"mstAst4.executeCommand / Executing an SQL command")
-        errors=0
-        while errors<3:
-            try:
-                with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
-                    with conn.cursor() as cursor:
-                        logger.debug(f"mstAst4.executeCommand / sql: {sql[:5000]}")
-                        cursor.execute(sql)
-                        rows=int("{}".format(cursor.rowcount))
-                        logger.debug(f"mstAst4.executeCommand / Received {rows} rows from cursor")
-            except Exception as s1:
-                if errors==0:
-                    logger.warning(f"mstAst4.executeCommand / first failure: "+str(s1)[:5000]+", command: "+str(sql[:2500]))
-                if "Violation of UNIQUE KEY constraint" in s1.args[1]:
-                    logger.warning(f"mstAst4.executeCommand / Violation of UNIQUE KEY constraint detected")
-                    return -2
-                if "The number of row value expressions in the INSERT statement exceeds the maximum allowed number of 1000" in s1.args[1]:
-                    logger.warning(f"mstAst4.executeCommand / INSERT statement exceeds the maximum allowed number of 1000")
-                    return -3
-                errors+=1
-                time.sleep(0.05)
-            if rows==0:
-                #logger.debug(f"mstAst4.executeCommand / 0 rows from cursor, returning 1")
-                return 1#so that we know that execution was successful
-            return rows
-        log_text=f"mstAst4.executeCommand Failed 3 times, stopping execution, last command: "+str(sql[:2500])
-        logger.error(log_text)
-        return -1
-    except Exception as e1:
-        #print(sql)
-        log_text=f"mstAst4.executeCommand Failed, error: {e1.args[1]}, sql: {sql[:2500]}"
-        logger.error(log_text)
-        return -1
-        
-def executeSelect(DB_CRED,sql,logger):
-    selectRows=[]
-    try:
-        logger.debug(f"mstAst4.executeSelect / Executing {sql}")
-        errors=0
-        error_text=None
-        while errors<3:
-            try:
-                with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
-                    with conn.cursor() as cursor:
-                        cursor.execute(sql)
-                        for row in cursor:
-                            selectRows.append(row)
-                        return selectRows
-            except Exception as pe:
-                error_text=str(pe)
-                errors+=1
-                time.sleep(0.05)
-        log_text="mstAst4.executeSelect Failed 3 times, stopping execution"
-        if error_text is not None:
-            log_text+=f". Last thrown error: {error_text}"
-        logger.error(log_text)
-        return None
-    except Exception as e1:
-        log_text=f"mstAst4.executeSelect Failed, error: "+str(e1)[:1000]
-        logger.error(log_text)
-        return selectRows
-        
-def getAssetParameter(DB_CRED,assetId,parameter,logger,subParameter=None):
-    try:
-        logger.debug("Starting getAssetParameter")
-        errors=0
-        while errors<3:
-            try:
-                if subParameter is None:
-                    sql=f"SELECT [{parameter}] FROM [dbo].[mstAssets] WHERE [AssetId]={assetId};"
-                else:
-                    sql=f"SELECT JSON_VALUE([{parameter}],'$.{subParameter}') FROM [dbo].[mstAssets] WHERE [AssetId]={assetId};"
-                #assetTypes={}
-                with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
-                    with conn.cursor() as cursor:
-                        cursor.execute(sql)
-                        for row in cursor:
-                            return row[0]
-                        return None#if no rows are returned, return none
-            except:
-                errors+=1
-                time.sleep(0.05)
-        log_text=f"mstAst4.getAssetParameter Failed 3 times, stopping execution"
-    except Exception as e1:
-        log_text=f"mstAst4.getAssetParameter Failed, error: {e1:[:1000]}"
-        logger.error(log_text)
-        
-def getColumnEntry(DB_CRED,getWhat,tableFrom,whereFilter,equalsWhat,string,logger):
-    try:
-        logger.debug(f"mstAst4.getColumnEntry / Getting {getWhat} from {tableFrom} on {DB_CRED['db_server']}.{DB_CRED['database']}")
-        errors=0
-        exc_text=""
-        while errors<3:
-            try:
-                if string==1:
-                    sql="SELECT "+getWhat+" FROM [dbo].["+tableFrom+"] WHERE ["+whereFilter+"]='"+equalsWhat+"';"
-                else:
-                    sql="SELECT "+getWhat+" FROM [dbo].["+tableFrom+"] WHERE ["+whereFilter+"]="+str(equalsWhat)+";"
-                logger.debug(f"mstAst4.getColumnEntry / SQL: {sql}")
-                #print(sql)
-                with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
-                    with conn.cursor() as cursor:
-                        cursor.execute(sql)
-                        for row in cursor:
-                            logger.debug(f"mstAst4.getColumnEntry OK, result: {row[0]}")
-                            return row[0]
-                        return None#if no rows are returned, return none
-            except Exception as e2:
-                log_text=f"mstAst4.getColumnEntry Failed, error2: {e2}"
-                exc_text=str(e2)[:500]
-                errors+=1
-                time.sleep(0.05)
-        log_text=f"mstAst4.getColumnEntry Failed 3 times, stopping execution, error: {exc_text}"
-        return None
-    except Exception as e1:
-        log_text=f"mstAst4.getColumnEntry Failed, error1: {e1}"
-        logger.error(log_text)
-        return None
+    def executeCommand(DB_CRED,sql,logger):
+        #this function returns negatie values in case of an error!!!
+        try:
+            #logger.debug(f"mstAst4.executeCommand / Executing an SQL command")
+            errors=0
+            while errors<3:
+                try:
+                    with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
+                        with conn.cursor() as cursor:
+                            logger.debug(f"mstAst4.executeCommand / sql: {sql[:5000]}")
+                            cursor.execute(sql)
+                            rows=int("{}".format(cursor.rowcount))
+                            logger.debug(f"mstAst4.executeCommand / Received {rows} rows from cursor")
+                except Exception as s1:
+                    if errors==0:
+                        logger.warning(f"mstAst4.executeCommand / first failure: "+str(s1)[:5000]+", command: "+str(sql[:2500]))
+                    if "Violation of UNIQUE KEY constraint" in s1.args[1]:
+                        logger.warning(f"mstAst4.executeCommand / Violation of UNIQUE KEY constraint detected")
+                        return -2
+                    if "The number of row value expressions in the INSERT statement exceeds the maximum allowed number of 1000" in s1.args[1]:
+                        logger.warning(f"mstAst4.executeCommand / INSERT statement exceeds the maximum allowed number of 1000")
+                        return -3
+                    errors+=1
+                    time.sleep(0.05)
+                if rows==0:
+                    #logger.debug(f"mstAst4.executeCommand / 0 rows from cursor, returning 1")
+                    return 1#so that we know that execution was successful
+                return rows
+            log_text=f"mstAst4.executeCommand Failed 3 times, stopping execution, last command: "+str(sql[:2500])
+            logger.error(log_text)
+            return -1
+        except Exception as e1:
+            #print(sql)
+            log_text=f"mstAst4.executeCommand Failed, error: {e1.args[1]}, sql: {sql[:2500]}"
+            logger.error(log_text)
+            return -1
+            
+    def executeSelect(DB_CRED,sql,logger):
+        selectRows=[]
+        try:
+            logger.debug(f"mstAst4.executeSelect / Executing {sql}")
+            errors=0
+            error_text=None
+            while errors<3:
+                try:
+                    with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
+                        with conn.cursor() as cursor:
+                            cursor.execute(sql)
+                            for row in cursor:
+                                selectRows.append(row)
+                            return selectRows
+                except Exception as pe:
+                    error_text=str(pe)
+                    errors+=1
+                    time.sleep(0.05)
+            log_text="mstAst4.executeSelect Failed 3 times, stopping execution"
+            if error_text is not None:
+                log_text+=f". Last thrown error: {error_text}"
+            logger.error(log_text)
+            return None
+        except Exception as e1:
+            log_text=f"mstAst4.executeSelect Failed, error: "+str(e1)[:1000]
+            logger.error(log_text)
+            return selectRows
+            
+    def getAssetParameter(DB_CRED,assetId,parameter,logger,subParameter=None):
+        try:
+            logger.debug("Starting getAssetParameter")
+            errors=0
+            while errors<3:
+                try:
+                    if subParameter is None:
+                        sql=f"SELECT [{parameter}] FROM [dbo].[mstAssets] WHERE [AssetId]={assetId};"
+                    else:
+                        sql=f"SELECT JSON_VALUE([{parameter}],'$.{subParameter}') FROM [dbo].[mstAssets] WHERE [AssetId]={assetId};"
+                    #assetTypes={}
+                    with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
+                        with conn.cursor() as cursor:
+                            cursor.execute(sql)
+                            for row in cursor:
+                                return row[0]
+                            return None#if no rows are returned, return none
+                except:
+                    errors+=1
+                    time.sleep(0.05)
+            log_text=f"mstAst4.getAssetParameter Failed 3 times, stopping execution"
+        except Exception as e1:
+            log_text=f"mstAst4.getAssetParameter Failed, error: {e1:[:1000]}"
+            logger.error(log_text)
+            
+    def getColumnEntry(DB_CRED,getWhat,tableFrom,whereFilter,equalsWhat,string,logger):
+        try:
+            logger.debug(f"mstAst4.getColumnEntry / Getting {getWhat} from {tableFrom} on {DB_CRED['db_server']}.{DB_CRED['database']}")
+            errors=0
+            exc_text=""
+            while errors<3:
+                try:
+                    if string==1:
+                        sql="SELECT "+getWhat+" FROM [dbo].["+tableFrom+"] WHERE ["+whereFilter+"]='"+equalsWhat+"';"
+                    else:
+                        sql="SELECT "+getWhat+" FROM [dbo].["+tableFrom+"] WHERE ["+whereFilter+"]="+str(equalsWhat)+";"
+                    logger.debug(f"mstAst4.getColumnEntry / SQL: {sql}")
+                    #print(sql)
+                    with pyodbc.connect('Driver='+DB_CRED['driver']+';Server=tcp:'+DB_CRED['db_server']+',1433;Database='+DB_CRED['database']+';Uid='+DB_CRED['db_user']+';Pwd={'+DB_CRED['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30') as conn:
+                        with conn.cursor() as cursor:
+                            cursor.execute(sql)
+                            for row in cursor:
+                                logger.debug(f"mstAst4.getColumnEntry OK, result: {row[0]}")
+                                return row[0]
+                            return None#if no rows are returned, return none
+                except Exception as e2:
+                    log_text=f"mstAst4.getColumnEntry Failed, error2: {e2}"
+                    exc_text=str(e2)[:500]
+                    errors+=1
+                    time.sleep(0.05)
+            log_text=f"mstAst4.getColumnEntry Failed 3 times, stopping execution, error: {exc_text}"
+            return None
+        except Exception as e1:
+            log_text=f"mstAst4.getColumnEntry Failed, error1: {e1}"
+            logger.error(log_text)
+            return None
 
-def buildMimeMessage(sender, subject, text, to_address, prio, text_type,cc_address,bcc_address):
-    msg = MIMEMultipart('html')
-    msg['From'] = sender
-    msg['To'] = to_address
-    msg['Cc'] = cc_address
-    msg['Bcc'] = bcc_address
-    msg['Subject'] = subject
-    body = text
-    msg['X-Priority'] = prio
-    msg.attach(MIMEText(body, text_type))
-    return msg
-    
-def sendEmail(CREDS, subject, text, to_address, prio, text_type, logger, cc_address=None, bcc_address=None):
-    try:
-        #text_type: 'html'
-        logger.debug("Starting sendEmail")
-        message = buildMimeMessage(CREDS["email_username"], subject, text, to_address, str(prio), text_type, cc_address, bcc_address)
-        exch=smtplib.SMTP(CREDS["email_server"], CREDS["email_port"])
-        exch.starttls()
-        exch.login(CREDS["email_username"], CREDS["email_password"])
-        exch.send_message(message)
-        exch.quit()
-        return 0
-    except Exception as e1:
-        log_text=f"mstAst4.sendEmail Failed, error: "+str(e1)[:1000]
-        logger.error(log_text)
-        return -1
-       
-def getSetting(CREDS,version,settingName,systemShortName,logger):
-    #this version of the function is using one mstSettings table instead of multiple ones like in the past
-    try:
-        logger.debug("Starting getSetting")
-        errors=0
-        while errors<3:
-            try:
-                sql=f"DECLARE @sysid INT=(SELECT [systemId] from [mstSystems] WHERE [shortName]='{systemShortName}');SELECT [Setting] FROM [dbo].[mstSettings] WHERE [settingVersion]={version} AND [settingName]='{settingName}' and [systemId]=@sysid;"
-                logger.debug(f"SQL: {sql}")
-                conn_string='Driver='+CREDS['driver']+';Server=tcp:'+CREDS['db_server']+',1433;Database='+CREDS['database']+';Uid='+CREDS['db_user']+';Pwd={'+CREDS['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30'
-                logger.debug(f"Connection: {conn_string}")
-                with pyodbc.connect(conn_string) as conn:
-                    with conn.cursor() as cursor:
-                        cursor.execute(sql)
-                        return cursor.fetchone()[0]
-            except Exception as pe:
-                logger.error(f"Failed getting setting: {pe}")
-                errors+=1
-                time.sleep(0.05)
-        log_text=f"mstAst4.getSetting Failed 3 times, stopping execution"
-        logger.error(log_text)
-        return None
-    except Exception as e1:
-        log_text=f"mstAst4.getSetting Failed, error: "+str(e1)[:1000]
-        logger.error(log_text)
-        return None
+    def buildMimeMessage(sender, subject, text, to_address, prio, text_type,cc_address,bcc_address):
+        msg = MIMEMultipart('html')
+        msg['From'] = sender
+        msg['To'] = to_address
+        msg['Cc'] = cc_address
+        msg['Bcc'] = bcc_address
+        msg['Subject'] = subject
+        body = text
+        msg['X-Priority'] = prio
+        msg.attach(MIMEText(body, text_type))
+        return msg
         
-def dfToDB2(CREDS,table,df,chunkSize,logger):
-    try:
-        #logger.debug(f"Starting mstAst4.dfToDB to table {table}")
-        #logger.debug(f"Creating connection")
-        conn_str=urllib.parse.quote_plus(r'Driver='+CREDS['driver']+';Server=tcp:'+CREDS['db_server']+',1433;Database='+CREDS['database']+';Uid='+CREDS['db_user']+';Pwd='+CREDS['db_password']+';Encrypt=yes;TrustServerCertificate=yes;Connection Timeout=30;')
-        conn='mssql+pyodbc:///?odbc_connect={}'.format(conn_str)
-        engine=create_engine(conn, fast_executemany=True, echo=False)
-        #engine=create_engine(conn, fast_executemany=False, echo=False)
-        #logger.debug(f"Executing df.to_sql")
-        #result=df.to_sql(table, engine, if_exists='append', chunksize=chunkSize, index=False, method='multi')
-        logger.debug(f"dfToDB2 executing")
-        timestampStart = datetime.now()
-        result=df.to_sql(table, engine, if_exists='append', chunksize=chunkSize, index=False)
-        timestampEnd=datetime.now()
-        runTime=str(timestampEnd-timestampStart)[:-7]
-        size=len(df.index)
-        logger.debug(f"mstAst4.dfToDB2 storing to table {table} ended with chunksize: {chunkSize}, result: {result}, size: {size} in {runTime}")
+    def sendEmail(CREDS, subject, text, to_address, prio, text_type, logger, cc_address=None, bcc_address=None):
+        try:
+            #text_type: 'html'
+            logger.debug("Starting sendEmail")
+            message = buildMimeMessage(CREDS["email_username"], subject, text, to_address, str(prio), text_type, cc_address, bcc_address)
+            exch=smtplib.SMTP(CREDS["email_server"], CREDS["email_port"])
+            exch.starttls()
+            exch.login(CREDS["email_username"], CREDS["email_password"])
+            exch.send_message(message)
+            exch.quit()
+            return 0
+        except Exception as e1:
+            log_text=f"mstAst4.sendEmail Failed, error: "+str(e1)[:1000]
+            logger.error(log_text)
+            return -1
+           
+    def getSetting(CREDS,version,settingName,systemShortName,logger):
+        #this version of the function is using one mstSettings table instead of multiple ones like in the past
+        try:
+            logger.debug("Starting getSetting")
+            errors=0
+            while errors<3:
+                try:
+                    sql=f"DECLARE @sysid INT=(SELECT [systemId] from [mstSystems] WHERE [shortName]='{systemShortName}');SELECT [Setting] FROM [dbo].[mstSettings] WHERE [settingVersion]={version} AND [settingName]='{settingName}' and [systemId]=@sysid;"
+                    logger.debug(f"SQL: {sql}")
+                    conn_string='Driver='+CREDS['driver']+';Server=tcp:'+CREDS['db_server']+',1433;Database='+CREDS['database']+';Uid='+CREDS['db_user']+';Pwd={'+CREDS['db_password']+'};Encrypt=yes;TrustServerCertificate=no;Connection Timeout=30'
+                    logger.debug(f"Connection: {conn_string}")
+                    with pyodbc.connect(conn_string) as conn:
+                        with conn.cursor() as cursor:
+                            cursor.execute(sql)
+                            return cursor.fetchone()[0]
+                except Exception as pe:
+                    logger.error(f"Failed getting setting: {pe}")
+                    errors+=1
+                    time.sleep(0.05)
+            log_text=f"mstAst4.getSetting Failed 3 times, stopping execution"
+            logger.error(log_text)
+            return None
+        except Exception as e1:
+            log_text=f"mstAst4.getSetting Failed, error: "+str(e1)[:1000]
+            logger.error(log_text)
+            return None
+            
+    def dfToDB2(CREDS,table,df,chunkSize,logger):
+        try:
+            #logger.debug(f"Starting mstAst4.dfToDB to table {table}")
+            #logger.debug(f"Creating connection")
+            conn_str=urllib.parse.quote_plus(r'Driver='+CREDS['driver']+';Server=tcp:'+CREDS['db_server']+',1433;Database='+CREDS['database']+';Uid='+CREDS['db_user']+';Pwd='+CREDS['db_password']+';Encrypt=yes;TrustServerCertificate=yes;Connection Timeout=30;')
+            conn='mssql+pyodbc:///?odbc_connect={}'.format(conn_str)
+            engine=create_engine(conn, fast_executemany=True, echo=False)
+            #engine=create_engine(conn, fast_executemany=False, echo=False)
+            #logger.debug(f"Executing df.to_sql")
+            #result=df.to_sql(table, engine, if_exists='append', chunksize=chunkSize, index=False, method='multi')
+            logger.debug(f"dfToDB2 executing")
+            timestampStart = datetime.now()
+            result=df.to_sql(table, engine, if_exists='append', chunksize=chunkSize, index=False)
+            timestampEnd=datetime.now()
+            runTime=str(timestampEnd-timestampStart)[:-7]
+            size=len(df.index)
+            logger.debug(f"mstAst4.dfToDB2 storing to table {table} ended with chunksize: {chunkSize}, result: {result}, size: {size} in {runTime}")
 
-        if isinstance(result, int) or result is None:
+            if isinstance(result, int) or result is None:
+                return 0
+            else:
+                logger.warning(f"mstAst4.dfToDB2 storing to table {table} ended with result: {result}, size: {size}, returning 0")
+            if size>chunkSize:
+                logger.debug(f"mstAst4.dfToDB2 storing to table {table} ended with result: {result}, size: {size}, returning 0")
             return 0
-        else:
-            logger.warning(f"mstAst4.dfToDB2 storing to table {table} ended with result: {result}, size: {size}, returning 0")
-        if size>chunkSize:
-            logger.debug(f"mstAst4.dfToDB2 storing to table {table} ended with result: {result}, size: {size}, returning 0")
-        return 0
-    except Exception as e1:
-        log_text=f"mstAst4.dfToDB2, storing to table {table} failed, error: "+str(e1)[:5000]
-        logger.error(log_text)
-        #logger.error(e1)
-        #raise
-        #raise error.with_traceback(sys.exc_info()[2])
-        return 1
-        
-def getVaultSecret(CREDS,vaultName,secretName,logger):
-    try:
-        logger.debug("Starting getVaultSecret")
-        #keyVaultName = "dv-kv-monsys"
-        #secretName="dv-sql"
-        KVUri = f"https://{vaultName}.vault.azure.net"
-        #credential = DefaultAzureCredential()
-        credential = ManagedIdentityCredential(client_id="031ce06f-fd5a-41a4-a62c-8ad477e71e98")
-        client = SecretClient(vault_url=KVUri, credential=credential)
-        secret = client.get_secret(secretName)
-        return secret.value
-    except Exception as e1:
-        log_text=f"mstAst4.getVaultSecret Failed, error: {e1}[:500]"
-        logger.error(log_text)
-        return None
+        except Exception as e1:
+            log_text=f"mstAst4.dfToDB2, storing to table {table} failed, error: "+str(e1)[:5000]
+            logger.error(log_text)
+            #logger.error(e1)
+            #raise
+            #raise error.with_traceback(sys.exc_info()[2])
+            return 1
+            
+    def getVaultSecret(CREDS,vaultName,secretName,logger):
+        try:
+            logger.debug("Starting getVaultSecret")
+            #keyVaultName = "dv-kv-monsys"
+            #secretName="dv-sql"
+            KVUri = f"https://{vaultName}.vault.azure.net"
+            #credential = DefaultAzureCredential()
+            credential = ManagedIdentityCredential(client_id="031ce06f-fd5a-41a4-a62c-8ad477e71e98")
+            client = SecretClient(vault_url=KVUri, credential=credential)
+            secret = client.get_secret(secretName)
+            return secret.value
+        except Exception as e1:
+            log_text=f"mstAst4.getVaultSecret Failed, error: {e1}[:500]"
+            logger.error(log_text)
+            return None
```

## Comparing `dedscumulus-0.0.5.dist-info/LICENSE` & `dedscumulus-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dedscumulus-0.0.5.dist-info/METADATA` & `dedscumulus-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.0.5
+Version: 0.0.6
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 License: UNKNOWN
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Platform: UNKNOWN
```

## Comparing `dedscumulus-0.0.5.dist-info/RECORD` & `dedscumulus-0.0.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 dedscumulus/RequestHandler.py,sha256=QHYYUg2veBvUlS4G-jVmImfc6hzsFuKMV5UrbmNFRCc,522
 dedscumulus/SharePointHandler.py,sha256=7-cmaaSqBB5-Y_huofCYVPMA9vcn8nQAtTCDzha---E,14421
 dedscumulus/TableLogHandler.py,sha256=i1jioOVCfK6PxDXPRLmJn20SkhVtGmpBvsTRw9rMDHg,2250
 dedscumulus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dedscumulus/brzGlobal.py,sha256=VB5Wb448lTocPGEoJGaqnTK96W95mmryaJoW0jGcSkA,8815
 dedscumulus/gbtGlobal.py,sha256=XmaY0rhRj2dzwh7LBKcILtb5i3UglmVG2o_aRWqSn5Y,4990
-dedscumulus/mstAst.py,sha256=U0hF7TJSRf01GXDE1tuI5f27LD_o01Z1XRfwJBOS3Xc,13474
+dedscumulus/mstAst.py,sha256=bcmEAa_SIu898mWUcEkgxk_aeu9l5H-Wjkk_EMOAUpE,14481
 dedscumulus/mstLog.py,sha256=0YOK8lkHIt7ma-xMZ7FCv23ERCFD0N5pLhLXy_FNuoA,823
 src/RequestHandler.py,sha256=QHYYUg2veBvUlS4G-jVmImfc6hzsFuKMV5UrbmNFRCc,522
 src/SharePointHandler.py,sha256=7-cmaaSqBB5-Y_huofCYVPMA9vcn8nQAtTCDzha---E,14421
 src/TableLogHandler.py,sha256=i1jioOVCfK6PxDXPRLmJn20SkhVtGmpBvsTRw9rMDHg,2250
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/brzGlobal.py,sha256=VB5Wb448lTocPGEoJGaqnTK96W95mmryaJoW0jGcSkA,8815
 src/gbtGlobal.py,sha256=XmaY0rhRj2dzwh7LBKcILtb5i3UglmVG2o_aRWqSn5Y,4990
 src/mstAst.py,sha256=U0hF7TJSRf01GXDE1tuI5f27LD_o01Z1XRfwJBOS3Xc,13474
 src/mstLog.py,sha256=0YOK8lkHIt7ma-xMZ7FCv23ERCFD0N5pLhLXy_FNuoA,823
-dedscumulus-0.0.5.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-dedscumulus-0.0.5.dist-info/METADATA,sha256=QQBtwko-SMBPe8V-qMH9VoGuvNolclpgQOx9j8EjQT4,566
-dedscumulus-0.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dedscumulus-0.0.5.dist-info/top_level.txt,sha256=dI9ZW3QNfFmeVCcUCLWTMkOMpHPqI6TTn4luigE8TrM,12
-dedscumulus-0.0.5.dist-info/RECORD,,
+dedscumulus-0.0.6.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+dedscumulus-0.0.6.dist-info/METADATA,sha256=PgVSdLt5BFNaZ1Uej1Un9CXfUdCAmqoWcMF65kNY6Kk,566
+dedscumulus-0.0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dedscumulus-0.0.6.dist-info/top_level.txt,sha256=dI9ZW3QNfFmeVCcUCLWTMkOMpHPqI6TTn4luigE8TrM,12
+dedscumulus-0.0.6.dist-info/RECORD,,
```

