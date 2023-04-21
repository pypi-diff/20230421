# Comparing `tmp/lsptrain-0.0.45.tar.gz` & `tmp/lsptrain-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.45.tar", last modified: Fri Apr 21 03:53:04 2023, max compression
+gzip compressed data, was "lsptrain-0.0.46.tar", last modified: Fri Apr 21 04:49:48 2023, max compression
```

## Comparing `lsptrain-0.0.45.tar` & `lsptrain-0.0.46.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:04.802290 lsptrain-0.0.45/
--rw-rw-rw-   0        0        0      434 2023-04-21 03:53:04.802290 lsptrain-0.0.45/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.45/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:04.790289 lsptrain-0.0.45/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.45/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:04.797289 lsptrain-0.0.45/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.45/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     6731 2023-04-21 03:51:19.000000 lsptrain-0.0.45/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:04.801289 lsptrain-0.0.45/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.45/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-04-21 02:59:24.000000 lsptrain-0.0.45/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0      406 2023-04-21 03:51:19.000000 lsptrain-0.0.45/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-21 03:53:04.795289 lsptrain-0.0.45/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      434 2023-04-21 03:53:04.000000 lsptrain-0.0.45/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-04-21 03:53:04.000000 lsptrain-0.0.45/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:53:04.000000 lsptrain-0.0.45/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-21 03:53:04.000000 lsptrain-0.0.45/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 03:53:04.000000 lsptrain-0.0.45/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 03:53:04.802290 lsptrain-0.0.45/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-21 03:53:03.000000 lsptrain-0.0.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.064926 lsptrain-0.0.46/
+-rw-rw-rw-   0        0        0      434 2023-04-21 04:49:48.064926 lsptrain-0.0.46/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.46/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.053926 lsptrain-0.0.46/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.46/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.059925 lsptrain-0.0.46/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.46/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     6712 2023-04-21 04:49:12.000000 lsptrain-0.0.46/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.063927 lsptrain-0.0.46/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.46/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0     2267 2023-04-21 04:49:12.000000 lsptrain-0.0.46/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0      172 2023-04-21 04:49:12.000000 lsptrain-0.0.46/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.058926 lsptrain-0.0.46/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:49:48.064926 lsptrain-0.0.46/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-21 04:49:46.000000 lsptrain-0.0.46/setup.py
```

### Comparing `lsptrain-0.0.45/lsptrain/nlp_classfication/model.py` & `lsptrain-0.0.46/lsptrain/nlp_classfication/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,31 +13,29 @@
 from transformers import BertTokenizer, BertConfig, BertModel
 from torch.utils import data
 from sklearn.model_selection import train_test_split
 
 from ..utils.init_args import setup_classification_args
 from ..utils.init_logger import setup_logger
 
-logger = setup_logger("sequence classification")
-
-
 args = setup_classification_args()
+logger = setup_logger(args)
 
 if not os.path.exists(args.save_dir):
     os.mkdir(args.save_dir)
 
 if not os.path.exists(args.train_path):
     raise Exception(f"file:{args.train_path} does not exist.")
 
-logger.info("开始读取数据")
+logger("开始读取数据")
 with open(args.train_path, "r", encoding=args.encoding) as f:
     datas = f.readlines()
 
 datas = [x.strip() for x in datas]
-logger.info("读取数据完成")
+logger("读取数据完成")
 
 info_labels = []
 
 # 加载预训练模型
 pretrained = args.pretrained_model
 tokenizer = BertTokenizer.from_pretrained(pretrained)
 bert_model = BertModel.from_pretrained(pretrained)
@@ -73,24 +71,24 @@
             print(e)
             continue
     X_train, X_test, y_train, y_test = train_test_split(texts, labels, test_size=test_size, random_state=0,
                                                         shuffle=True)
     return (X_train, y_train), (X_test, y_test)
 
 
-print("开始转换数据")
+logger("开始转换数据")
 (X_train, y_train), (X_test, y_test) = get_train_test_data(test_size=0.1)
-print("完成转换数据")
+logger("完成转换数据")
 
 label_path = os.path.join(args.save_dir, args.label_file_name)
 
 with open(label_path, "w", encoding=args.encoding) as f:
     for label in info_labels:
         f.write(f"{label}\n")
-logger.info(f"保存标签至:[{label_path}]")
+logger(f"保存标签至:[{label_path}]")
 
 
 # dataloader
 class DataGen(data.Dataset):
     def __init__(self, data, label):
         self.data = data
         self.label = label
@@ -131,15 +129,15 @@
 model = Model(bert_model, config, len(info_labels))
 if args.device and args.device.startswith("cuda"):
     device = torch.device(args.device) if torch.cuda.is_available() else 'cpu'
 elif args.device == "cpu":
     device = torch.device("cpu")
 else:
     device = torch.device(args.device)
-logger.info(f"训练使用device:[{device}]")
+logger(f"训练使用device:[{device}]")
 model.to(device)
 
 
 def get_optimizer():
     select_optimizer = args.optimizer
     if select_optimizer == "sgd":
         optimizer = torch.optim.SGD(model.parameters(), lr=args.learning_rate, weight_decay=1e-4)
@@ -149,17 +147,18 @@
 
 
 criterion = torch.nn.CrossEntropyLoss()
 optimizer = get_optimizer()
 
 
 def start_train():
+    logger("开始训练数据")
     best_accu = 0
     for epoch in range(args.num_epochs):
-        logger.info(f"epoch = {epoch}, datetime = {datetime.datetime.now()}")
+        logger(f"epoch = {epoch}, datetime = {datetime.datetime.now()}")
         start = time.time()
         loss_sum = 0.0
         accu = 0
         model.train()
         for token_ids, label in tqdm(train_dataloader):
             token_ids = token_ids.to(device).long()
             label = label.to(device).long()
@@ -179,15 +178,15 @@
             label = label.to(device).long()
             with torch.no_grad():
                 out = model(token_ids)
                 loss = criterion(out, label)
                 test_loss_sum += loss.cpu().data.numpy()
                 test_accu += (out.argmax(1) == label).sum().cpu().data.numpy()
         accuracy = test_accu / len(test_dataset)
-        logger.info("epoch %d, train loss:%f, train acc:%f, test loss:%f, test acc:%f, use time:" % (
+        logger("epoch %d, train loss:%f, train acc:%f, test loss:%f, test acc:%f, use time:" % (
             epoch, loss_sum / len(train_dataset), accu / len(train_dataset), test_loss_sum / len(test_dataset),
             test_accu / len(test_dataset)), int(time.time() - start))
         if args.save_best:
             # 如果只保存最优模型
             if best_accu < accuracy:
                 save_path = os.path.join(args.save_dir, f"{args.job_type}_model_best.pt")
                 best_accu = accuracy
```

### Comparing `lsptrain-0.0.45/lsptrain/utils/init_args.py` & `lsptrain-0.0.46/lsptrain/utils/init_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,10 +29,12 @@
                         help="序列最大长度，超过部分会被自动截断")
     parser.add_argument("-e", "--num_epochs", default=25, type=int,
                         help="训练步数")
     parser.add_argument("-d", "--device", default="cuda:0",
                         help="训练设备。如果可用，默认使用第一块显卡")
     parser.add_argument("-j", "--job_type", default="txt_classification", type=str,
                         help="任务名称，保存模型开头名称")
+    parser.add_argument("-sl", "--show_log", default=True, type=bool,
+                        help="是否打印日志")
     args = parser.parse_args()
 
     return args
```

### Comparing `lsptrain-0.0.45/setup.py` & `lsptrain-0.0.46/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.45',
+      version='0.0.46',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch>=1.11.0',
                         'transformers>=4.20.1',
```

