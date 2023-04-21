# Comparing `tmp/lsptrain-0.0.46.tar.gz` & `tmp/lsptrain-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.46.tar", last modified: Fri Apr 21 04:49:48 2023, max compression
+gzip compressed data, was "lsptrain-0.0.47.tar", last modified: Fri Apr 21 04:59:33 2023, max compression
```

## Comparing `lsptrain-0.0.46.tar` & `lsptrain-0.0.47.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.064926 lsptrain-0.0.46/
--rw-rw-rw-   0        0        0      434 2023-04-21 04:49:48.064926 lsptrain-0.0.46/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.46/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.053926 lsptrain-0.0.46/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.46/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.059925 lsptrain-0.0.46/lsptrain/nlp_classfication/
--rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.46/lsptrain/nlp_classfication/__init__.py
--rw-rw-rw-   0        0        0     6712 2023-04-21 04:49:12.000000 lsptrain-0.0.46/lsptrain/nlp_classfication/model.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.063927 lsptrain-0.0.46/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.46/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0     2267 2023-04-21 04:49:12.000000 lsptrain-0.0.46/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0      172 2023-04-21 04:49:12.000000 lsptrain-0.0.46/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-21 04:49:48.058926 lsptrain-0.0.46/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      434 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 04:49:48.000000 lsptrain-0.0.46/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 04:49:48.064926 lsptrain-0.0.46/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-04-21 04:49:46.000000 lsptrain-0.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:59:33.199360 lsptrain-0.0.47/
+-rw-rw-rw-   0        0        0      434 2023-04-21 04:59:33.199360 lsptrain-0.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-04-20 15:16:58.000000 lsptrain-0.0.47/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-21 04:59:33.186360 lsptrain-0.0.47/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.47/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:59:33.194360 lsptrain-0.0.47/lsptrain/nlp_classfication/
+-rw-rw-rw-   0        0        0       36 2023-04-21 03:31:26.000000 lsptrain-0.0.47/lsptrain/nlp_classfication/__init__.py
+-rw-rw-rw-   0        0        0     6685 2023-04-21 04:59:31.000000 lsptrain-0.0.47/lsptrain/nlp_classfication/model.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:59:33.197360 lsptrain-0.0.47/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.47/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0     2415 2023-04-21 04:59:31.000000 lsptrain-0.0.47/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.47/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-21 04:59:33.191361 lsptrain-0.0.47/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-04-21 04:59:33.000000 lsptrain-0.0.47/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-04-21 04:59:33.000000 lsptrain-0.0.47/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 04:59:33.000000 lsptrain-0.0.47/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-21 04:59:33.000000 lsptrain-0.0.47/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 04:59:33.000000 lsptrain-0.0.47/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 04:59:33.199360 lsptrain-0.0.47/setup.cfg
+-rw-rw-rw-   0        0        0      745 2023-04-21 04:57:43.000000 lsptrain-0.0.47/setup.py
```

### Comparing `lsptrain-0.0.46/lsptrain/nlp_classfication/model.py` & `lsptrain-0.0.47/lsptrain/nlp_classfication/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 from torch.utils import data
 from sklearn.model_selection import train_test_split
 
 from ..utils.init_args import setup_classification_args
 from ..utils.init_logger import setup_logger
 
 args = setup_classification_args()
-logger = setup_logger(args)
 
 if not os.path.exists(args.save_dir):
     os.mkdir(args.save_dir)
 
 if not os.path.exists(args.train_path):
     raise Exception(f"file:{args.train_path} does not exist.")
 
-logger("开始读取数据")
+print("开始读取数据")
 with open(args.train_path, "r", encoding=args.encoding) as f:
     datas = f.readlines()
 
 datas = [x.strip() for x in datas]
-logger("读取数据完成")
+print("读取数据完成")
 
 info_labels = []
 
 # 加载预训练模型
 pretrained = args.pretrained_model
 tokenizer = BertTokenizer.from_pretrained(pretrained)
 bert_model = BertModel.from_pretrained(pretrained)
@@ -52,15 +51,15 @@
 
 
 def get_train_test_data(max_length=args.max_length, test_size=args.test_size):
     texts = []
     labels = []
 
     for one in tqdm(datas):
-        result = one.split("__")
+        result = one.split(args.split_data)
         if len(result) != 2:
             continue
 
         text, label = result
         try:
             lebal_index = get_label(label.strip())
             text = tokenizer.encode(text.strip(), max_length=max_length, padding="max_length",
@@ -71,24 +70,24 @@
             print(e)
             continue
     X_train, X_test, y_train, y_test = train_test_split(texts, labels, test_size=test_size, random_state=0,
                                                         shuffle=True)
     return (X_train, y_train), (X_test, y_test)
 
 
-logger("开始转换数据")
+print("开始转换数据")
 (X_train, y_train), (X_test, y_test) = get_train_test_data(test_size=0.1)
-logger("完成转换数据")
+print("完成转换数据")
 
 label_path = os.path.join(args.save_dir, args.label_file_name)
 
 with open(label_path, "w", encoding=args.encoding) as f:
     for label in info_labels:
         f.write(f"{label}\n")
-logger(f"保存标签至:[{label_path}]")
+print(f"保存标签至:[{label_path}]")
 
 
 # dataloader
 class DataGen(data.Dataset):
     def __init__(self, data, label):
         self.data = data
         self.label = label
@@ -129,15 +128,15 @@
 model = Model(bert_model, config, len(info_labels))
 if args.device and args.device.startswith("cuda"):
     device = torch.device(args.device) if torch.cuda.is_available() else 'cpu'
 elif args.device == "cpu":
     device = torch.device("cpu")
 else:
     device = torch.device(args.device)
-logger(f"训练使用device:[{device}]")
+print(f"训练使用device:[{device}]")
 model.to(device)
 
 
 def get_optimizer():
     select_optimizer = args.optimizer
     if select_optimizer == "sgd":
         optimizer = torch.optim.SGD(model.parameters(), lr=args.learning_rate, weight_decay=1e-4)
@@ -147,18 +146,18 @@
 
 
 criterion = torch.nn.CrossEntropyLoss()
 optimizer = get_optimizer()
 
 
 def start_train():
-    logger("开始训练数据")
+    print("开始训练数据")
     best_accu = 0
     for epoch in range(args.num_epochs):
-        logger(f"epoch = {epoch}, datetime = {datetime.datetime.now()}")
+        print(f"epoch = {epoch}, datetime = {datetime.datetime.now()}")
         start = time.time()
         loss_sum = 0.0
         accu = 0
         model.train()
         for token_ids, label in tqdm(train_dataloader):
             token_ids = token_ids.to(device).long()
             label = label.to(device).long()
@@ -178,15 +177,15 @@
             label = label.to(device).long()
             with torch.no_grad():
                 out = model(token_ids)
                 loss = criterion(out, label)
                 test_loss_sum += loss.cpu().data.numpy()
                 test_accu += (out.argmax(1) == label).sum().cpu().data.numpy()
         accuracy = test_accu / len(test_dataset)
-        logger("epoch %d, train loss:%f, train acc:%f, test loss:%f, test acc:%f, use time:" % (
+        print("epoch %d, train loss:%f, train acc:%f, test loss:%f, test acc:%f, use time:" % (
             epoch, loss_sum / len(train_dataset), accu / len(train_dataset), test_loss_sum / len(test_dataset),
             test_accu / len(test_dataset)), int(time.time() - start))
         if args.save_best:
             # 如果只保存最优模型
             if best_accu < accuracy:
                 save_path = os.path.join(args.save_dir, f"{args.job_type}_model_best.pt")
                 best_accu = accuracy
```

### Comparing `lsptrain-0.0.46/lsptrain/utils/init_args.py` & `lsptrain-0.0.47/lsptrain/utils/init_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 
 def setup_classification_args():
     parser = argparse.ArgumentParser("预训练分类任务")
     parser.add_argument("--train_path", type=str,
                         help="训练集数据，应该为txt文件")
     parser.add_argument("--test_size", default=0.1, type=float,
-                        help="测试集比例")
+                        help="测试集比例，默认0.1")
     parser.add_argument("--encoding", default="utf-8", type=str,
                         help="打开数据字符集，默认为utf-8")
+    parser.add_argument("--split_data", default="__", type=str,
+                        help="切分数据与标签的分隔符， 默认'__'")
     parser.add_argument("-pm", "--pretrained_model", default="hfl/chinese-roberta-wwm-ext", type=str,
-                        help="预训练模型名称")
+                        help="预训练模型名称, 默认'hfl/chinese-roberta-wwm-ext'")
     parser.add_argument("-lr", "--learning_rate", default=0.0001,
-                        type=float, help="学习率")
+                        type=float, help="学习率，默认0.0001")
     parser.add_argument("-o", "--optimizer", choices=["adam", "sgd"], default="adam", type=str,
-                        help="模型优化函数")
+                        help="模型优化函数，默认adam")
     parser.add_argument("-b", "--batch_size", default=64, type=int,
                         help="训练批次大小，如果报错提示out of memory，可以适当调小")
     parser.add_argument("-s", "--save_dir", default="checkpoint", type=str,
                         help="训练checkpoint保存路径")
     parser.add_argument("--label_file_name", default="catalog_label.txt", type=str,
                         help="保存标签路径")
     parser.add_argument("--save_best", default=False, type=bool,
                         help="是否只保存最优模型")
     parser.add_argument("--max_length", default=64, type=int,
-                        help="序列最大长度，超过部分会被自动截断")
+                        help="默认序列最大长度64，超过部分会被自动截断")
     parser.add_argument("-e", "--num_epochs", default=25, type=int,
-                        help="训练步数")
+                        help="训练步数，默认25")
     parser.add_argument("-d", "--device", default="cuda:0",
                         help="训练设备。如果可用，默认使用第一块显卡")
     parser.add_argument("-j", "--job_type", default="txt_classification", type=str,
-                        help="任务名称，保存模型开头名称")
-    parser.add_argument("-sl", "--show_log", default=True, type=bool,
-                        help="是否打印日志")
+                        help="任务名称，保存模型开头名称，默认'txt_classification'")
     args = parser.parse_args()
 
     return args
```

### Comparing `lsptrain-0.0.46/setup.py` & `lsptrain-0.0.47/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.46',
+      version='0.0.47',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch>=1.11.0',
                         'transformers>=4.20.1',
```

