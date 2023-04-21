# Comparing `tmp/lsptrain-0.0.48.tar.gz` & `tmp/lsptrain-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.48.tar", last modified: Fri Apr 21 05:12:15 2023, max compression
+gzip compressed data, was "lsptrain-0.0.49.tar", last modified: Fri Apr 21 05:48:57 2023, max compression
```

## Comparing `lsptrain-0.0.48.tar` & `lsptrain-0.0.49.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 05:12:15.273447 lsptrain-0.0.48/
--rw-rw-rw-   0        0        0      492 2023-04-21 05:12:15.273447 lsptrain-0.0.48/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.48/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 05:12:15.256447 lsptrain-0.0.48/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.48/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:12:15.266448 lsptrain-0.0.48/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.48/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     6685 2023-04-21 04:59:31.000000 lsptrain-0.0.48/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:12:15.271448 lsptrain-0.0.48/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.48/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-04-21 04:59:31.000000 lsptrain-0.0.48/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.48/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-21 05:12:15.263447 lsptrain-0.0.48/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      492 2023-04-21 05:12:15.000000 lsptrain-0.0.48/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-04-21 05:12:15.000000 lsptrain-0.0.48/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 05:12:15.000000 lsptrain-0.0.48/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-21 05:12:15.000000 lsptrain-0.0.48/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 05:12:15.000000 lsptrain-0.0.48/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 05:12:15.274447 lsptrain-0.0.48/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-21 05:12:13.000000 lsptrain-0.0.48/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.222717 lsptrain-0.0.49/
+-rw-rw-rw-   0        0        0      492 2023-04-21 05:48:57.221716 lsptrain-0.0.49/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-21 05:10:24.000000 lsptrain-0.0.49/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.209715 lsptrain-0.0.49/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.49/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.216717 lsptrain-0.0.49/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.49/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     6974 2023-04-21 05:48:54.000000 lsptrain-0.0.49/lsptrain/nlp_classfication/model.py
+-rw-rw-rw-   0        0        0     1603 2023-04-21 05:47:19.000000 lsptrain-0.0.49/lsptrain/nlp_classfication/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.220716 lsptrain-0.0.49/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.49/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0     2418 2023-04-21 05:40:42.000000 lsptrain-0.0.49/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.49/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:48:57.214717 lsptrain-0.0.49/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      492 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 05:48:57.000000 lsptrain-0.0.49/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:48:57.222717 lsptrain-0.0.49/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-21 05:48:54.000000 lsptrain-0.0.49/setup.py
```

### Comparing `lsptrain-0.0.48/lsptrain/nlp_classfication/model.py` & `lsptrain-0.0.49/lsptrain/nlp_classfication/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # encoding: utf-8
 # @author: k
 
 import datetime
-import argparse
-import logging
 from tqdm import tqdm
 import os
 import time
 
 import numpy as np
 import torch
 from transformers import BertTokenizer, BertConfig, BertModel
 from torch.utils import data
 from sklearn.model_selection import train_test_split
 
 from ..utils.init_args import setup_classification_args
-from ..utils.init_logger import setup_logger
 
 args = setup_classification_args()
 
 if not os.path.exists(args.save_dir):
     os.mkdir(args.save_dir)
 
 if not os.path.exists(args.train_path):
     raise Exception(f"file:{args.train_path} does not exist.")
 
+
+def load_datas(data_file: str):
+    with open(data_file, "r", encoding=args.encoding) as f:
+        datas = f.readlines()
+    datas = [x.strip() for x in datas]
+    return datas
+
+
 print("开始读取数据")
-with open(args.train_path, "r", encoding=args.encoding) as f:
-    datas = f.readlines()
 
-datas = [x.strip() for x in datas]
+datas = load_datas(args.train_path)
+
 print("读取数据完成")
 
 info_labels = []
 
 # 加载预训练模型
 pretrained = args.pretrained_model
 tokenizer = BertTokenizer.from_pretrained(pretrained)
@@ -46,20 +50,26 @@
         if x not in info_labels:
             info_labels.append(x)
         return info_labels.index(x)
     else:
         return info_labels[x]
 
 
-def get_train_test_data(max_length=args.max_length, test_size=args.test_size):
+def get_train_test_data(datas, split_data="__", max_length=args.max_length, test_size=args.test_size):
+    """
+    :param datas: ["样本数据__标签",]
+    :param max_length: 样本最大长度，超过会自动截断
+    :param test_size: 测试集比率
+    :return: X_train, X_test, y_train, y_test
+    """
     texts = []
     labels = []
 
     for one in tqdm(datas):
-        result = one.split(args.split_data)
+        result = one.split(split_data)
         if len(result) != 2:
             continue
 
         text, label = result
         try:
             lebal_index = get_label(label.strip())
             text = tokenizer.encode(text.strip(), max_length=max_length, padding="max_length",
@@ -71,15 +81,15 @@
             continue
     X_train, X_test, y_train, y_test = train_test_split(texts, labels, test_size=test_size, random_state=0,
                                                         shuffle=True)
     return (X_train, y_train), (X_test, y_test)
 
 
 print("开始转换数据")
-(X_train, y_train), (X_test, y_test) = get_train_test_data(test_size=0.1)
+(X_train, y_train), (X_test, y_test) = get_train_test_data(datas=datas, test_size=0.1)
 print("完成转换数据")
 
 label_path = os.path.join(args.save_dir, args.label_file_name)
 
 with open(label_path, "w", encoding=args.encoding) as f:
     for label in info_labels:
         f.write(f"{label}\n")
@@ -117,40 +127,39 @@
 
     def forward(self, token_ids):
         bert_out = self.bert_model(token_ids)[1]  # 句向量 [batch_size,hidden_size]
         bert_out = self.dropout(bert_out)
         bert_out = self.fc1(bert_out)
         bert_out = self.relu(bert_out)
         bert_out = self.dropout(bert_out)
-        bert_out = self.fc2(bert_out)  #
+        bert_out = self.fc2(bert_out)
         return bert_out
 
 
 model = Model(bert_model, config, len(info_labels))
 if args.device and args.device.startswith("cuda"):
     device = torch.device(args.device) if torch.cuda.is_available() else 'cpu'
 elif args.device == "cpu":
     device = torch.device("cpu")
 else:
     device = torch.device(args.device)
 print(f"训练使用device:[{device}]")
 model.to(device)
 
 
-def get_optimizer():
-    select_optimizer = args.optimizer
-    if select_optimizer == "sgd":
-        optimizer = torch.optim.SGD(model.parameters(), lr=args.learning_rate, weight_decay=1e-4)
+def get_optimizer(select_optimizer: str = 'Adam', lr: float = 0.0001):
+    if select_optimizer.lower() == "sgd":
+        optimizer = torch.optim.SGD(model.parameters(), lr=lr, weight_decay=1e-4)
     else:
-        optimizer = torch.optim.Adam(model.parameters(), lr=args.learning_rate, weight_decay=1e-4)
+        optimizer = torch.optim.Adam(model.parameters(), lr=lr, weight_decay=1e-4)
     return optimizer
 
 
 criterion = torch.nn.CrossEntropyLoss()
-optimizer = get_optimizer()
+optimizer = get_optimizer(args.optimizer, args.learning_rate)
 
 
 def start_train():
     print("开始训练数据")
     best_accu = 0
     for epoch in range(args.num_epochs):
         print(f"epoch = {epoch}, datetime = {datetime.datetime.now()}")
```

### Comparing `lsptrain-0.0.48/lsptrain/utils/init_args.py` & `lsptrain-0.0.49/lsptrain/utils/init_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     parser.add_argument("-o", "--optimizer", choices=["adam", "sgd"], default="adam", type=str,
                         help="模型优化函数，默认adam")
     parser.add_argument("-b", "--batch_size", default=64, type=int,
                         help="训练批次大小，如果报错提示out of memory，可以适当调小")
     parser.add_argument("-s", "--save_dir", default="checkpoint", type=str,
                         help="训练checkpoint保存路径")
     parser.add_argument("--label_file_name", default="catalog_label.txt", type=str,
-                        help="保存标签路径")
+                        help="保存标签文件名")
     parser.add_argument("--save_best", default=False, type=bool,
                         help="是否只保存最优模型")
     parser.add_argument("--max_length", default=64, type=int,
                         help="默认序列最大长度64，超过部分会被自动截断")
     parser.add_argument("-e", "--num_epochs", default=25, type=int,
                         help="训练步数，默认25")
     parser.add_argument("-d", "--device", default="cuda:0",
```

### Comparing `lsptrain-0.0.48/setup.py` & `lsptrain-0.0.49/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.48',
+      version='0.0.49',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch>=1.11.0',
                         'transformers>=4.20.1',
```

