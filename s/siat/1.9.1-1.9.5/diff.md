# Comparing `tmp/siat-1.9.1-py3-none-any.whl.zip` & `tmp/siat-1.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1120883 bytes, number of entries: 117
+Zip file size: 1126842 bytes, number of entries: 117
 -rw-rw-rw-  2.0 fat      840 b- defN 23-Apr-10 11:29 siat/__init__.py
 -rw-rw-rw-  2.0 fat     2130 b- defN 23-Apr-10 11:29 siat/allin.py
 -rw-rw-rw-  2.0 fat      747 b- defN 23-Apr-10 11:29 siat/alpha_vantage_test.py
 -rw-rw-rw-  2.0 fat    28555 b- defN 23-Apr-10 11:29 siat/assets_liquidity.py
 -rw-rw-rw-  2.0 fat     1285 b- defN 23-Apr-10 11:29 siat/assets_liquidity_test.py
 -rw-rw-rw-  2.0 fat    10110 b- defN 23-Apr-10 11:29 siat/barrons_scraping_test.py
 -rw-rw-rw-  2.0 fat    36597 b- defN 23-Apr-10 11:29 siat/beta_adjustment.py
@@ -31,15 +31,15 @@
 -rw-rw-rw-  2.0 fat     2944 b- defN 23-Apr-10 11:29 siat/esg_test.py
 -rw-rw-rw-  2.0 fat    47177 b- defN 23-Apr-10 11:29 siat/fama_french.py
 -rw-rw-rw-  2.0 fat     4678 b- defN 23-Apr-10 11:29 siat/fama_french_test.py
 -rw-rw-rw-  2.0 fat    40695 b- defN 23-Apr-10 11:29 siat/financial_base.py
 -rw-rw-rw-  2.0 fat    21528 b- defN 23-Apr-10 11:29 siat/financial_statements.py
 -rw-rw-rw-  2.0 fat      716 b- defN 23-Apr-10 11:29 siat/financial_statements_test.py
 -rw-rw-rw-  2.0 fat    76676 b- defN 23-Apr-10 11:29 siat/financials.py
--rw-rw-rw-  2.0 fat   125365 b- defN 23-Apr-19 10:25 siat/financials_china.py
+-rw-rw-rw-  2.0 fat   148161 b- defN 23-Apr-21 14:04 siat/financials_china.py
 -rw-rw-rw-  2.0 fat    57998 b- defN 23-Apr-10 11:29 siat/financials_china2.py
 -rw-rw-rw-  2.0 fat     2722 b- defN 23-Apr-10 11:29 siat/financials_china2_test.py
 -rw-rw-rw-  2.0 fat     3507 b- defN 23-Apr-10 11:29 siat/financials_china2_test2.py
 -rw-rw-rw-  2.0 fat     3118 b- defN 23-Apr-10 11:29 siat/financials_china2_test3.py
 -rw-rw-rw-  2.0 fat    17549 b- defN 23-Apr-10 11:29 siat/financials_china_test.py
 -rw-rw-rw-  2.0 fat     5924 b- defN 23-Apr-19 09:54 siat/financials_china_test2.py
 -rw-rw-rw-  2.0 fat     5924 b- defN 23-Apr-19 09:55 siat/financials_china_test2_fin_indicator.py
@@ -108,12 +108,12 @@
 -rw-rw-rw-  2.0 fat   118133 b- defN 23-Apr-10 11:29 siat/translate-20230206.py
 -rw-rw-rw-  2.0 fat   121657 b- defN 23-Apr-10 11:29 siat/translate-20230215.py
 -rw-rw-rw-  2.0 fat   124748 b- defN 23-Apr-19 09:58 siat/translate.py
 -rw-rw-rw-  2.0 fat     3936 b- defN 23-Apr-10 11:29 siat/universal_test.py
 -rw-rw-rw-  2.0 fat    51268 b- defN 23-Apr-10 11:29 siat/valuation_china.py
 -rw-rw-rw-  2.0 fat     1571 b- defN 23-Apr-10 11:29 siat/valuation_market_china_test.py
 -rw-rw-rw-  2.0 fat    14859 b- defN 23-Apr-10 11:29 siat/var_model_validation.py
--rw-rw-rw-  2.0 fat     1399 b- defN 23-Apr-19 10:32 siat-1.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 10:32 siat-1.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-19 10:32 siat-1.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     9353 b- defN 23-Apr-19 10:33 siat-1.9.1.dist-info/RECORD
-117 files, 4407678 bytes uncompressed, 1106613 bytes compressed:  74.9%
+-rw-rw-rw-  2.0 fat     1399 b- defN 23-Apr-21 14:09 siat-1.9.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-21 14:09 siat-1.9.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Apr-21 14:09 siat-1.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     9353 b- defN 23-Apr-21 14:09 siat-1.9.5.dist-info/RECORD
+117 files, 4430474 bytes uncompressed, 1112572 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -333,20 +333,20 @@
 
 Filename: siat/valuation_market_china_test.py
 Comment: 
 
 Filename: siat/var_model_validation.py
 Comment: 
 
-Filename: siat-1.9.1.dist-info/METADATA
+Filename: siat-1.9.5.dist-info/METADATA
 Comment: 
 
-Filename: siat-1.9.1.dist-info/WHEEL
+Filename: siat-1.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: siat-1.9.1.dist-info/top_level.txt
+Filename: siat-1.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: siat-1.9.1.dist-info/RECORD
+Filename: siat-1.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## siat/financials_china.py

```diff
@@ -67,15 +67,15 @@
     
     #抓取三大报表
     try:
         fbs = ak.stock_financial_report_sina(stock=prefix, symbol="资产负债表")
         fis = ak.stock_financial_report_sina(stock=prefix, symbol="利润表")
         fcf = ak.stock_financial_report_sina(stock=prefix, symbol="现金流量表")
     except:
-        print("  #Error(get_fin_stmt_ak): some financial statements unavailable for",ticker)
+        print("  #Error(get_fin_stmt_ak): some financial statements unavailable yet for",ticker)
         return None        
     
     #若报表为空，则返回
     if fbs is None:
         print("  #Warning(get_fin_stmt_ak): balance sheets inaccessible for",ticker)
         return None 
     if fis is None:
@@ -585,15 +585,18 @@
         pd.set_option('display.unicode.ambiguous_as_wide', True)
         pd.set_option('display.unicode.east_asian_width', True)  
         
         print("===== 杜邦分析分项数据表 =====")
         print("*** 数据来源：sina/EM，"+str(today))
         """
         title_txt="杜邦分析分项数据表"
-        footnote="*** 数据来源：sina/EM，"+str(today)
+        footnote0="1、表中各个上市公司的财报日期可能存在差异，但均为可获得(已公布)的最新财报"
+        footnote1="2、表中数值基于期末数字直接计算，而非期初期末均值，可能与公告数字存在差异。"
+        footnote2="*** 数据来源：sina/EM，"+str(today)
+        footnote=footnote0+'\n'+footnote1+'\n'+footnote2
         df_directprint(df,title_txt,footnote)
         #print(df.to_string(index=False))
         
         
     #合并所有历史记录
     alldf=pd.concat(dpidflist)
     alldf.dropna(inplace=True)
@@ -610,15 +613,15 @@
 
 if __name__=='__main__':
     tickerlist=['600606.SS','600519.SS','000002.SZ'] 
     df=compare_dupont_china(tickerlist,fsdate='latest',scale1 = 100,scale2 = 10)   
 
 #==============================================================================
 #==============================================================================
-# 以上基于财报直接构造，以下基于获取的财务指标构造================================
+# 以上基于财报期末数字直接构造，以下基于获取的财务指标构造================================
 #==============================================================================
 #==============================================================================
 if __name__=='__main__':
     ticker="600606.SS" 
 
 def get_fin_abstract_ak(ticker):
     """
@@ -2594,15 +2597,15 @@
 
     #亿元
     yi=100000000
 
     company_name=codetranslate(ticker)
     # 定义杜邦分解项目变量
     
-    roe='【'+company_name+'】\n\n'+'净资产收益率'
+    roe='【'+company_name+'】\n('+fsdate+')\n'+'净资产收益率'
     try:
         totalOEValue=round(fs1['所有者权益(或股东权益)合计'].values[0] / yi,1)
     except:
         try:
             totalOEValue=round(fs1['股东权益合计'].values[0] / yi,1)
         except:
             totalOEValue=round(fs1['所有者权益合计'].values[0] / yi,1)
@@ -2995,19 +2998,512 @@
         print("1、为避免图示过大，这里未列出所有分解项目")
         print("2、金融机构报表与普通企业结构不同，此处仅为约算")
         print("3、应收款项包括应收账款、应收利息、应收保费以及应收票据等")
         print("4、递延资产为递延所得税资产或借项")
         print("5、税金包括营业税金及附加以及所得税费用")
         print("6、此处金融资产主要为交易性金融资产、衍生金融资产和买入返售金融资产")
         print("7、此处长期投资包括贷款及垫款、可供出售金融资产、持有至到期投资、长期股权投资、投资性房地产等")
+        print("8、注意：图中比率和比值均为基于财报期末数值直接计算，并非基于期初期末均值，可能与公告数字存在差异。")
 
     return g
 
 if __name__=='__main__':
     ticker="600519.SS" 
     fsdate='2022-12-31'
     
     g=dupont_decompose_china(ticker,fsdate)
 
 #==============================================================================
+if __name__=='__main__':
+    tickers=['000002.SZ','601398.SS']
+    fsdates=['2022-12-31','2021-12-31']
+    
+
+def get_fin_summary_china_original(tickers,fsdates):
+    """
+    功能：获得A股财报摘要，进行数据整理
+    输出：
+    1、项目列表：不带(元)、(次)、(%)等后缀括弧
+    2、数量级变换：(元)-->(亿元)，并相应修改字段名
+    
+    废弃！
+    """
+
+    import pandas as pd
+    df=pd.DataFrame()
+    # 获得股票
+    for t in tickers:
+        _,t1,_=split_prefix_suffix(t)
+        dft=ak.stock_financial_abstract(t1)
+        
+        dft['ticker']=t
+        
+        if len(df)==0:
+            df=dft
+        else:
+            df=pd.concat([df,dft])
+
+    # 遍历
+    collist=list(df)
+    colremove=['选项','指标','ticker']
+    for cr in colremove:
+        collist.remove(cr)
+    noamtlist=["率","每股","周转","乘数",'/']
+    yiyuan=100000000
+    
+    for index,row in df.iterrows():
+        #print(index,row)
+        # 金额变为亿元，不含"率"、"每股"、"周转"、"乘数"
+
+        if '率' in row['指标']:
+            if not ('周转率' in row['指标']):
+                df.at[index,'指标']=row['指标']+'(%)'
+                for d in collist:
+                    df.at[index,d] = round(row[d],2)
+                continue
+            
+        if '/' in row['指标']:
+            df.at[index,'指标']=row['指标']+'(%)'
+            for d in collist:
+                df.at[index,d] = round(row[d],2)
+            continue
+        
+        if '每股' in row['指标']:
+            df.at[index,d] = round(row[d],2)
+            continue
+     
+        # 元变换为亿元
+        for d in collist:
+            df.at[index,d] = round(row[d] / yiyuan,1)
+            df.at[index,'指标']=row['指标']+'(亿元)'
+    
+    # 填充nan为零
+    df.fillna('-',inplace=True)
+
+    # 改变日期格式
+    for c in collist:
+        try:
+            c1=pd.to_datetime(c)
+            c2=c1.strftime("%Y-%m-%d")
+        except:
+            continue
+        df.rename(columns={c:c2},inplace=True)
+        
+    # 过滤财报日期
+    fsdates2=[]
+    for d in fsdates:
+        d1=pd.to_datetime(d)
+        d2=d1.strftime("%Y-%m-%d")
+        fsdates2=fsdates2 + [d2]
+        
+    collistnew=colremove+fsdates2
+    fsdf=df[collistnew]
+    
+    return fsdf
+
+#==============================================================================
+if __name__=='__main__':
+    astr='存货周转天数'
+    substrlist=['乘数','每股','/','周转']
+    str_contain_any_substr(astr,substrlist)
+
+
+def str_contain_any_substr(astr,substrlist):
+    """
+    功能：判断astr是否含有子串列表substrlist之一
+    """
+    result=False
+    for sub in substrlist:
+        if sub in astr:
+            result=True
+            
+    return result
+
+
+if __name__=='__main__':
+    ticker='000002.SZ'
+    fsdates=['2022-12-31','2021-12-31','2020-12-31']
+    
+    fsdf1=get_fin_summary_1ticker_china(ticker,fsdates)
+
+def get_fin_summary_1ticker_china(ticker,fsdates):
+    """
+    功能：获得A股财报摘要，进行数据整理，单一股票
+    输出：
+    1、项目列表：不带(元)、(次)、(%)等后缀括弧
+    2、数量级变换：(元)-->(亿元)，并相应修改字段名
+    """
+
+    import pandas as pd
+    # 过滤财报日期
+    fsdates2=[]
+    for d in fsdates:
+        d1=pd.to_datetime(d)
+        d2=d1.strftime("%Y-%m-%d")
+        fsdates2=fsdates2 + [d2]
+    fsdates3=sorted(fsdates2,reverse=True)
+    
+    yiyuan=float(1e+08)
+    
+    # 获得股票所有财报数据
+    _,t1,_=split_prefix_suffix(ticker)
+    dft=ak.stock_financial_abstract(t1)
+    
+    # 处理金额单位和百分号字段
+    # 选项-指标对照表
+    option_indicator_df=dft[['选项','指标']]
+    option_indicator_df.set_index('指标',inplace=True)
+    
+    # 变换日期格式为YYYY-MM-DD
+    collist=list(dft)
+    for c in collist:
+        try:
+            c1=pd.to_datetime(c)
+            c2=c1.strftime("%Y-%m-%d")
+        except:
+            continue
+        dft.rename(columns={c:c2},inplace=True)
+    
+    # 过滤财报日期    
+    try:
+        dft2=dft[['选项','指标']+fsdates3]
+    except:
+        print("  #Warning(get_fin_summary_1ticker_china): fin stmt of",fsdates3[0],"unavailable for",ticker+'('+codetranslate(ticker)+')')
+        return None
+    
+    # 金额变换：元-->亿元，小数位截取
+    dft2=dft2.drop(labels=['选项'],axis=1)
+    # 去掉重复行，非常重要！！！
+    dft2b=dft2.drop_duplicates (keep='first')
+    
+    dft2b.set_index('指标',inplace=True)
+    
+    dft2t=dft2b.T
+    
+    noneamtlist=['乘数','每股','/','周转','率','天数']
+    collist2=list(dft2t)
+    
+    for c in collist2:
+        
+        if not str_contain_any_substr(c,noneamtlist):
+            dft2t[c]=dft2t[c] / yiyuan
+        
+        if ('/' in c) and ('现金' in c):
+            dft2t[c]=dft2t[c] * 100.0
+        
+        dft2t[c]=dft2t[c].apply(lambda x: round(x,2))    
+        
+    # 标记字段后缀
+    dft3=dft2t.T
+    dft3['指标2']=dft3.index
+    dft3t=dft3.T
+    collist3=list(dft3t)
+    for c in collist3:
+        # 判断顺序不可颠倒
+        if str_contain_any_substr(c,['乘数','周转']):
+            continue
+        if str_contain_any_substr(c,['率']):
+            dft3t.rename(columns={c:c+'%'},inplace=True)
+            continue
+        if str_contain_any_substr(c,['每股']):
+            dft3t.rename(columns={c:c+'(元)'},inplace=True)
+            continue
+        if str_contain_any_substr(c,['/']):
+            dft3t.rename(columns={c:c+'(%)'},inplace=True)
+            continue
+    
+        # 其余的字段：元变换为亿元
+        dft3t.rename(columns={c:c+'(亿元)'},inplace=True)
+        
+    # 检查字段改名情况
+    collist3t=list(dft3t)
+    
+    # 回填指标选项类型
+    dft4=dft3t.T
+    dft5=dft4.reset_index()
+    dft5.set_index('指标2',inplace=True)
+    dft6=dft5.merge(option_indicator_df,how='left',left_index=True, right_index=True) 
+     
+    dft7=dft6.reset_index(drop=True) 
+     
+    dft7['ticker']=ticker
+        
+    # 填充nan为零
+    dft7.fillna('-',inplace=True)
+    
+    return dft7
+
+#==============================================================================
+if __name__=='__main__':
+    tickers=['000002.SZ','601398.SS']
+    fsdates=['2022-12-31','2021-12-31','2020-12-31']
+    
+    fsdfm=get_fin_summary_china(tickers,fsdates)
+    
+
+def get_fin_summary_china(tickers,fsdates):
+    """
+    功能：获得A股财报摘要，进行数据整理
+    输出：
+    1、项目列表：不带(元)、(次)、(%)等后缀括弧
+    2、数量级变换：(元)-->(亿元)，并相应修改字段名
+    """
+
+    import pandas as pd
+    # 过滤财报日期
+    fsdates2=[]
+    for d in fsdates:
+        d1=pd.to_datetime(d)
+        d2=d1.strftime("%Y-%m-%d")
+        fsdates2=fsdates2 + [d2]
+    fsdates3=list(set(fsdates2))
+    fsdates4=sorted(fsdates3,reverse=True)
+    
+    df=pd.DataFrame()
+    
+    # 获得股票
+    for t in tickers:
+        # 抓取一只股票的财报
+        dft=get_fin_summary_1ticker_china(t,fsdates4)
+        if dft is None: 
+            continue
+        
+        if len(df)==0:
+            df=dft
+        else:
+            df=pd.concat([df,dft])
+    
+    return df
+
+if __name__=='__main__':
+    tickers=['000002.SZ','601398.SS']
+    fsdates=['2022-12-31','2021-12-31','2020-12-31']
+
+    tickers='000002.SZ'
+    fsdates=['2022-12-31','2021-12-31','2020-12-31']   
+    
+    tickers=['000002.SZ','600048.SS','001979.SZ','600325.SS','000069.SZ','600383.SS','600895.SS','601155.SS']
+    
+def compare_fin_summary_china(tickers,fsdates):
+    """
+    功能：分类别显示财报摘要中的指标
+    """        
+    
+    # 检查股票列表
+    if isinstance(tickers,str):
+        tickers=[tickers]
+    tickers=list(tickers) #强制转换
+    if len(tickers)==0:
+        print("  #Error(compare_fin_summary_china): need at least one stock in",tickers)
+        return None
+    
+    # 检查财报日期列表
+    if isinstance(fsdates,str):
+        fsdates=[fsdates]
+    if len(fsdates)==0:
+        print("  #Error(compare_fin_summary_china): need at least one date in",fsdates)
+        return None
+    
+    for d in fsdates:
+        result,_,_=check_period(d,d)
+        if not result:
+            print("  #Error(compare_fin_summary_china): invalid date",d)
+            return None
+        
+    # 获取财报数据
+    print("Searching for financial statements, please wait ...")
+    fsdf=get_fin_summary_china(tickers,fsdates)
+    
+    # 不改变列表顺序去重
+    tickerlist=list(fsdf['ticker'])
+    tickers_found=sorted(list(set(tickerlist)),key=tickerlist.index)
+    
+    #optionlist=list(fsdf['选项'])
+    #typelist=sorted(list(set(optionlist)),key=optionlist.index)
+    typelist=['常用指标','每股指标','营运能力','盈利能力','收益质量','成长能力','财务风险']
+    # 手工设定项目显示顺序，使其看起来更合理
+    typedict={'常用指标':
+              ['营业总收入(亿元)','营业成本(亿元)',
+               '净利润(亿元)','扣非净利润(亿元)','归母净利润(亿元)',
+               '毛利率%','销售净利率%','期间费用率%',  
+               '基本每股收益(元)','总资产报酬率(ROA)%','净资产收益率(ROE)%', 
+               '经营现金流量净额(亿元)','每股现金流(元)',
+               '股东权益合计(净资产)(亿元)','每股净资产(元)',
+               '资产负债率%','商誉(亿元)',],
+              
+              '每股指标':
+              ['每股营业总收入(元)','每股营业收入(元)',
+               '每股息税前利润(元)','基本每股收益(元)','稀释每股收益(元)',
+               '每股净资产_最新股数(元)','摊薄每股净资产_期末股数(元)','调整每股净资产_期末股数(元)', 
+               '每股未分配利润(元)','每股留存收益(元)','每股盈余公积金(元)','每股资本公积金(元)',
+               '每股现金流量净额(元)','每股经营现金流(元)','每股企业自由现金流量(元)','每股股东自由现金流量(元)',],
+              
+              '营运能力':
+              ['总资产周转率','总资产周转天数',
+               '流动资产周转天数','流动资产周转率', 
+               '存货周转率','存货周转天数',
+               '应收账款周转率','应收账款周转天数','应付账款周转率',],
+              
+              '盈利能力': 
+              ['毛利率%','营业利润率%','息税前利润率%','销售净利率%','成本费用利润率%',
+              '总资产净利率_平均%','总资产净利率_平均(含少数股东损益)%', 
+              '总资产报酬率%', '总资本回报率%','息前税后总资产报酬率_平均%', 
+              '净资产收益率(ROE)%','净资产收益率_平均%','净资产收益率_平均_扣除非经常损益%', 
+              '摊薄净资产收益率%','摊薄净资产收益率_扣除非经常损益%', 
+              '投入资本回报率%',],
+              
+              '收益质量':
+              ['销售成本率%','成本费用率%','期间费用率%','所得税/利润总额(%)',
+               '经营性现金净流量/营业总收入(%)','经营活动净现金/销售收入(%)', 
+               '经营活动净现金/归属母公司的净利润(%)',], 
+              
+              '成长能力':
+              ['营业总收入(亿元)','营业总收入增长率%',
+               '净利润(亿元)','扣非净利润(亿元)', 
+               '归母净利润(亿元)','归属母公司净利润增长率%',],
+              
+              '财务风险':
+              ['流动比率%','速动比率%','保守速动比率%','现金比率%','资产负债率%',
+               '权益乘数','权益乘数(含少数股权的净资产)','产权比率%',],
+              }
+
+    # 注释
+    notesdict={'常用指标': \
+               '\n注：\n'+ \
+               '1. 毛利率=毛利 / 营业(总)收入 ×100%，毛利=营业(总)收入-营业(总)成本 \n'+ \
+               '2. 销售净利率=净利润 / 营业(总)收入 ×100% \n'+ \
+               '3. 期间费用率=期间费用 / 营业(总)收入 ×100%，期间费用包括管理费用，销售费用和财务费用。 \n', \
+              
+              '每股指标': \
+               '\n注：\n'+ \
+               '1. 稀释每股指标:假设企业所有发行在外的稀释性潜在普通股期间内均转换为普通股，导致普通股股数增加 \n'+ \
+               '2. 潜在普通股：指赋予其持有者在报告期或以后期间享有取得普通股权利的金融工具或者其他合同，例如公司可转债、认股权证、股份期权等 \n'+ \
+               '3. 摊薄每股指标：使用扣非后净利润计算，而非净利润，扣非后净利润可持续性更强，可能大于、小于或等于净利润 \n'+ \
+               '4. 调整后的每股净资产：考虑了净资产的流动性和变现能力，更加稳健，缩小了报表的粉饰空间 \n'+ \
+               '5. 调整后的每股净资产=（年度末股东权益-三年以上的应收款项净额-待摊费用-长期待摊费用）/年度末普通股股份总数 \n'+ \
+               '6. 应收款项净额：包括应收帐款、其他应收款、预付帐款、应收股利、应收利息、应收补贴款 \n'+ \
+               '7. 未分配利润：指企业实现的净利润经过弥补亏损、提取盈余公积和向投资者分配利润后留存在企业的、历年结存的利润 \n'+ \
+               '8. 留存收益：指企业从历年实现的利润中提取或形成的留存于企业的内部积累，包括盈余公积和未分配利润两类 \n'+ \
+               '9. 法定盈余公积：指企业按照公司法等法律规定的比例从净利润中提取的盈余公积 \n'+ \
+               '10.任意盈余公积：指企业经股东大会或类似机构批准按照规定的比例从净利润中提取的盈余公积。任意盈余公积的提取比例由企业自行确定 \n'+ \
+               '11.资本公积金：指直接由资本原因形成的公积金，如发行股份溢价、资产重估增值、接受捐赠等，用于转增股本，不得用于弥补亏损 \n'+ \
+               '12.自由现金流=企业经营活动现金流-资本性支出，用来衡量实际持有的在不影响企业生存时可回报股东(债务人）的最大现金额。 \n', \
+
+              '营运能力': \
+               '\n注：\n'+ \
+               '1. 指标周转率/周转次数：营业(总)收入 / 指标的起初期末均值，一般来说越大越好 \n'+ \
+               '2. 指标周转天数：360/周转率(或周转次数)，一般来说越小越好 \n'+ \
+               '3. 注意：本表部分指标不适用于金融行业。 \n', \
+              
+              '盈利能力': 
+               '\n注：\n'+ \
+               '1. 营业利润率=营业利润 / 营业(总)收入 x100% \n'+ \
+               '2. 营业利润=营业(总)收入-营业(总)成本-营业税金及附加-期间费用-资产减值损失+公允价值变动损益+投资损益 \n'+ \
+               '3. 营业利润率是在不考虑营业外收支和所得税费用的情况下，反映企业经营业务创造利润能力，比毛利率更能反映企业的盈利能力 \n'+ \
+               '4. 成本费用利润率=利润总额 / 成本费用总额 ×100%，反映企业付出一单位成本可以获取多少利润，即企业获取利润的效率 \n'+ \
+               '5. 利润总额=营业利润+营业外收入-营业外支出 \n'+ \
+               '6. 成本费用总额=营业成本+营业税金及附加+期间费用+资产减值损失 \n'+ \
+               '7. 少数股东损益：指公司合并报表的子公司中其它非控股股东享有的损益，需要在利润表中予以扣除 \n'+ \
+               '8. 总资产净利率_平均(含少数股东损益)：即在扣除少数股东损益之前的总资产净利率 \n'+ \
+               '9. 总资产报酬率=息税前利润 / 总资产期初期末均值 ×100%，即（利润总额+利息支出） / 平均总资产 ×100% \n'+ \
+               '10.投入资本回报率(ROIC，Return Of Invested Capital)=息税前利润(EBIT) x (1-税率) / 投入资本 x100%， \n'+ \
+               '11.息税前利润(EBIT)=营业收入–营业成本–营业费用+营业外收入支出(或是税前净利+利息费用)， \n'+ \
+               '12.投入资本（Invested Capital）=流动资产–流动负债+不动产与厂房设备净额+无形资产及商誉， \n'+ \
+               '13.总资本回报率(收益率)（Return of Total Capital）=(利润总额+借入资本利息) / 总资本 x100%， \n'+ \
+               '14.总资本回报率(收益率)反映企业总资本的收益能力，从经营者的立场观察，自有资本和借入资本没有区分的必要 \n'+ \
+               '15.在借入资本利息中，除去利息支出、贴现费用、企业借债利息外，还应包括公司债券折价摊销数额在内。 \n', 
+              
+              '收益质量':
+               '\n注：\n'+ \
+               '1. 销售成本率=营业(总)成本 / 营业(总)收入 x100%，=1-毛利润 \n'+ \
+               '2. 成本费用率=(营业(总)成本+期间费用) / 营业(总)收入 x100%，=销售成本率+期间费用率，可评价企业对成本费用的控制能力 \n'+ \
+               '3. 期间费用率=期间费用 / 营业(总)收入 x100% \n',
+              
+              '成长能力':
+                '\n注：\n'+ \
+              '1. 扣费(后)净利润=净利润-非经常性损益，即扣除了偶然的不可持续或不常发生的收益，可持续性更强，可能大于或小于净利润 \n'+ \
+               '2. 归属母公司净利润：简称归母净利润，指企业合并报表中归属控股公司(母公司)的利润，不包括归属子公司中非控股股东的利润。 \n',
+              
+              '财务风险':
+               '\n注：\n'+ \
+               '1. 保守速动比率：又称超速动比率，=(现金+短期证券投资+应收账款净额) / 流动负债，比速动比能够更好地评价企业短期偿债能力 \n'+ \
+               '2. 应收账款净额:指应收账款和其他应收款减去备抵坏账的净额，实质即为信誉高客户的应收款净额 \n'+ \
+               '3. 产权比率(equity ratio)=负债总额 / 所有者权益总额(净资产) x100%，从一个方面说明企业长期偿债能力，越高越弱 \n'+ \
+               '4. 注意：本表部分指标不适用于金融行业。 \n\n'+ \
+               '*** 注意：表中数字并非基于财报期末数字计算，而是直接来源于财经网站和上市公司财报摘要（基于期初期末均值调整）。',
+              }        
+        
+    # 一只股票情形：多日期
+    if len(tickers_found) == 1:
+        ticker1=tickers[0]
+        titletxt="\n===== 上市公司财务报表摘要："+codetranslate(ticker1)+" ====="    
+        print(titletxt)    
+        
+        fsdf1=fsdf[fsdf['ticker']==ticker1]
+        for ty in typelist:
+            dft=fsdf1[fsdf1['选项']==ty]
+            #print(list(dft['指标']))
+            
+            # 自定义排序
+            dft["指标"]=dft["指标"].astype('category').cat.set_categories(typedict[ty])
+            dft.sort_values(by='指标',inplace=True)
+            
+            dft.reset_index(drop=True,inplace=True)
+            dft.index=dft.index + 1
+            dft2=dft.drop(labels=['选项','ticker'],axis=1)
+            
+            print("\n***",ty+'：')
+            colalign=['center','left']+['right']*(len(list(dft2)) - 2)
+            print(dft2.to_markdown(tablefmt='Simple',index=True,colalign=colalign))
+            print(notesdict[ty])
+            
+    
+    # 多只股票情形：单日期
+    import pandas as pd
+    fsdates2=[]
+    for fsd in fsdates:
+        fsd2=pd.to_datetime(fsd)
+        fsd3=fsd2.strftime("%Y-%m-%d")
+        fsdates2=fsdates2+[fsd3]
+    fsdates3=sorted(fsdates2,reverse=True)                
+    
+    if len(tickers_found) > 1:
+        titletxt="\n===== 上市公司财务报表摘要对比：报表日期"+fsdates3[0]+" ====="
+        print('\n'+titletxt)    
+    
+        mdf=pd.DataFrame()
+        for t in tickers_found:
+            dft=fsdf[fsdf['ticker']==t]
+            
+            try:
+                dft2=dft[['选项','指标',fsdates3[0]]]
+                dft2.rename(columns={fsdates3[0]:codetranslate(t)},inplace=True)
+            except:
+                print("  #Error(compare_fin_summary_china): fin stmt of",fsdates3[0],'not found for',t)
+                return None
+            
+            if len(mdf) == 0:
+                mdf=dft2
+            else:
+                mdf=mdf.merge(dft2,left_on=['选项','指标'], right_on=['选项','指标'])
+        
+        for ty in typelist:
+            dft=mdf[mdf['选项']==ty]
+            
+            # 自定义排序
+            dft["指标"]=dft["指标"].astype('category').cat.set_categories(typedict[ty])
+            dft.sort_values(by='指标',inplace=True)
+            
+            dft.reset_index(drop=True,inplace=True)
+            dft.index=dft.index + 1
+            dft2=dft.drop(labels=['选项'],axis=1)
+            
+            print("\n***",ty+'：')
+            colalign=['center','left']+['right']*(len(list(dft2)) - 2)
+            print(dft2.to_markdown(tablefmt='Simple',index=True,colalign=colalign))
+            print(notesdict[ty])
+    
+    return dft2
+
+#==============================================================================
 #==============================================================================
 #==============================================================================
```

## Comparing `siat-1.9.1.dist-info/METADATA` & `siat-1.9.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siat
-Version: 1.9.1
+Version: 1.9.5
 Summary: Securities Investment Analysis Tools (siat)
 Home-page: https://pypi.org/project/siat/
 Author: Prof. WANG Dehong, Business School, BFSU (北京外国语大学 国际商学院 王德宏 教授)
 Author-email: wdehong2000@163.com
 License: Copyright (C) WANG Dehong, 2023. For educational purpose only!
 Platform: UNKNOWN
 Requires-Dist: pandas-datareader
```

## Comparing `siat-1.9.1.dist-info/RECORD` & `siat-1.9.5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 siat/esg_test.py,sha256=Z9m6GUt8O7oHZSEG9aDYpGdvvrv2AiRJdHTiU6jqmZ0,2944
 siat/fama_french.py,sha256=qDpsZOj0BLuzXXdNwJ1IPhDyNVAnTJFHqn80Hkp85ZI,47177
 siat/fama_french_test.py,sha256=M4O23lBKsJxhWHRluwCb3l7HSEn3OFTjzGMpehcevRg,4678
 siat/financial_base.py,sha256=YxNVfhbgLQ4stLojI9nklB4sdQNuROcILcO3M2uz4Gs,40695
 siat/financial_statements.py,sha256=KDUl9b92EV5IseLLnEmG3czDHAaay2SWM2MpzZXPHpk,21528
 siat/financial_statements_test.py,sha256=FLhx8JD-tVVWSBGux6AMz1jioXX4U4bp9DmgFHYXb_w,716
 siat/financials.py,sha256=4b0fJAu1Mm5aX_zCIvF01CzzBokrprQpIk1N3za1FNA,76676
-siat/financials_china.py,sha256=bnr3x09X0xaRyB1ewe63maQ-0_CLPjKrFWC0WZGXCdU,125365
+siat/financials_china.py,sha256=bm4oc533Y-eV2y4V328zKrKYFDBLTFeGhIjlH4PqNZ0,148161
 siat/financials_china2.py,sha256=32--MBk7PBOSg7DUyxfjN63ZPEkmAsrYfuTHAenOphA,57998
 siat/financials_china2_test.py,sha256=Erz5k4LyOplBBvYls2MypuqHpVNJ3daiLdyeJezNPu0,2722
 siat/financials_china2_test2.py,sha256=C8CuYTMHN4Mhp-sTu-Bmg0zMXRCaYV6ezGDoYartRYQ,3507
 siat/financials_china2_test3.py,sha256=UXYSA80DNSPRhHpovc2MA9JkpILWMAQaRatbWCHBNPs,3118
 siat/financials_china_test.py,sha256=QS1SD_mXx4uH1Lg3gl2PmwLrvkLqkRs3e4x7SyFI_Xk,17549
 siat/financials_china_test2.py,sha256=WkNlVW_0hGegdw1rzg4BP_dKR-smdyUp9Fr00K7mPZY,5924
 siat/financials_china_test2_fin_indicator.py,sha256=WkNlVW_0hGegdw1rzg4BP_dKR-smdyUp9Fr00K7mPZY,5924
@@ -107,11 +107,11 @@
 siat/translate-20230206.py,sha256=-vtI125WyaJhmPotOpDAmclt_XnYVaWU9ByLWZ6FyYE,118133
 siat/translate-20230215.py,sha256=TJgtPE3n8IjljmZ4Pefy8dmHoNdFF-1zpML6BhA9FKE,121657
 siat/translate.py,sha256=Ed3H3G1BiMaWL1iKGiiE4YP92tgj23xhlIdsU42Uqlk,124748
 siat/universal_test.py,sha256=CDAOffW1Rvs-TcNN5giWVvHMlch1w4dp-w5SIV9jXL0,3936
 siat/valuation_china.py,sha256=J78FTnwyzOjNENq30MXaQdby6EtcBZi3AMeUKhGtuok,51268
 siat/valuation_market_china_test.py,sha256=gbJ0ioauuo4koTPH6WKUkqcXiQPafnbhU5eKJ6lpdLA,1571
 siat/var_model_validation.py,sha256=zB_Skk_tmzIR15l6oAW3am4HBGVIG-eZ8gJhCdXZ8Qw,14859
-siat-1.9.1.dist-info/METADATA,sha256=CD8o_91qonL7hUBaDfpVMvqqAQ9rP5de8yz8MwnNI80,1399
-siat-1.9.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-siat-1.9.1.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
-siat-1.9.1.dist-info/RECORD,,
+siat-1.9.5.dist-info/METADATA,sha256=THfCa4K9pKEO6Xz8Nq8rM7xgk1rk4Q6k_Czx0oWX704,1399
+siat-1.9.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+siat-1.9.5.dist-info/top_level.txt,sha256=r1cVyL7AIKqeAmEJjNR8FMT20OmEzufDstC2gv3NvEY,5
+siat-1.9.5.dist-info/RECORD,,
```

