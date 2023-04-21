# Comparing `tmp/HHLtools-1.0.8.1-py2.py3-none-any.whl.zip` & `tmp/HHLtools-1.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4183 bytes, number of entries: 7
--rw-r--r--  2.0 unx      364 b- defN 22-Nov-04 03:45 HHLtools/CN.py
--rw-r--r--  2.0 unx     4830 b- defN 22-Nov-04 03:44 HHLtools/__init__.py
--rwxrwxrwx  2.0 unx     1126 b- defN 22-Nov-04 03:55 HHLtools-1.0.8.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1166 b- defN 22-Nov-04 03:55 HHLtools-1.0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Nov-04 03:55 HHLtools-1.0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 22-Nov-04 03:55 HHLtools-1.0.8.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      552 b- defN 22-Nov-04 03:55 HHLtools-1.0.8.1.dist-info/RECORD
-7 files, 8157 bytes uncompressed, 3205 bytes compressed:  60.7%
+Zip file size: 5127 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      338 b- defN 23-Apr-21 03:35 HHLtools/CN.py
+-rw-r--r--  2.0 unx     9392 b- defN 23-Apr-21 05:52 HHLtools/__init__.py
+-rwxrwxrwx  2.0 unx     1126 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1266 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      542 b- defN 23-Apr-21 06:05 HHLtools-1.1.0.dist-info/RECORD
+7 files, 12783 bytes uncompressed, 4169 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: HHLtools/CN.py
 Comment: 
 
 Filename: HHLtools/__init__.py
 Comment: 
 
-Filename: HHLtools-1.0.8.1.dist-info/LICENSE.txt
+Filename: HHLtools-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: HHLtools-1.0.8.1.dist-info/METADATA
+Filename: HHLtools-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: HHLtools-1.0.8.1.dist-info/WHEEL
+Filename: HHLtools-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: HHLtools-1.0.8.1.dist-info/top_level.txt
+Filename: HHLtools-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: HHLtools-1.0.8.1.dist-info/RECORD
+Filename: HHLtools-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## HHLtools/CN.py

```diff
@@ -16,9 +16,7 @@
 绝对值 = abs
 字符 = chr
 执行 = exec
 是否属于 = isinstance
 编号 = ord
 保留小数 = round
 求和 = sum
-栈 = Stack
-队列 = Queue
```

## HHLtools/__init__.py

```diff
@@ -1,90 +1,129 @@
-import os
-import platform
-import sys
-import tkinter as tk
-
+from collections.abc import Iterable
 #CONSTANTS
-class fontstyle():
+class FontStyle:
     DEFAULT = 0
     BOLD = 1
     UNDERLINE = 4
     BLINK = 5
     REVERSE = 7
 
-class color():
+class FontColor:
     BLACK = 30
     RED = 31
     GREEN = 32
     YELLOW = 33
     BLUE = 34
     PURPLE = 35
     CYAN = 36
     WHITE = 37
 
-class backgroundcolor():
+class BackgroundColor:
+    DEFAULT = ''
     BLACK = 40
     RED = 41
     GREEN = 42
     YELLOW = 43
     BLUE = 44
     PURPLE = 45
     CYAN = 46
     WHITE = 47
 
 
-def fibonacci(n):
-    if n < 1 or int(n) != n:
+def fibonacci(n:int):
+    if type(n) != int:
+        raise TypeError
+    if n < 1:
         return "error, n should be a positive number which is greater than 1"
     if n < 3:
         return 1
     a, b = 1, 1
 
     for i in range(2, n):
         a = a + b if i % 2 == 0 else a
         b = a + b if i % 2 == 1 else b
     return a if a > b else b
 
 def fibonacci_list(n):
-    if n < 1 or int(n) != n:
+    if type(n) != int:
+        raise TypeError
+    if n < 1:
         return "error, n should be a positive number which is greater than 1"
     if n == 1:
         return [1]
     if n == 2:
         return [1, 1]
     list = [1, 1]
     for i in range(2, n):
         list.append(list[i - 2] + list[i - 1])
     return list
 
-class Queue():
+class Queue:
     def __init__(self,size:int = -1):
         if size > 0:
             self.__size = size
             self.__queue = [0] * size
             self.__head = 0
             self.__tail = 0
             self.__count = 0
         else:
             self.__size = size
             self.__queue = []
 
-    @property
-    def val(self):
-        return self.__queue
-
-    @property
-    def 值(self):
-        return self.__queue
-
-    @property
-    def count(self):
-        return self.__count
-
-    def push(self, content):
+    def __repr__(self):
+        return f'Queue({str(self.__queue)}, ' \
+               f'headPointer = {self.__head if self.__size != -1 else len(self.__queue) - 1}, ' \
+               f'tailPointer = {self.__tail if self.__size != -1 else 0})'
+
+    def __len__(self):
+        return self.__count if self.__size != -1 else len(self.__queue)
+
+    def __iter__(self):
+        return iter(self.getlist())
+
+    def __contains__(self, item):
+        return item in self.getlist()
+
+    def __getitem__(self, item):
+        return self.getlist()[int(item)]
+
+    def getlist(self):
+        contents = []
+        if self.__size == -1:
+            contents = self.__queue[:]
+        else:
+            head = self.__head
+            while 1:
+                contents.append(self.__queue[head])
+                head += 1
+                head = head % self.__size
+                if head == self.__tail:
+                    break
+        return contents
+
+    def show(self):
+        contents = self.getlist()
+        maxlen = 0
+        for c in contents:
+            if len(str(c)) > maxlen:
+                maxlen = len(str(c))
+        print('='*(15+maxlen+15))
+        for c in range(len(contents)):
+            front = ' '*15
+            end = ' '
+            if c == self.__head:
+                front = 'headPointer    '
+            if c == self.__tail:
+                end = (maxlen+4)*' ' +'tailPointer'
+            print(front+str(contents[c])+' '*(maxlen-len(str(contents[c])))+end)
+        print('=' * (15 + maxlen + 15))
+
+    def push(self, content: int|str|float):
+        if type(content) not in (int, str, float):
+            raise TypeError
         if self.__size > 0:
             if self.__count == self.__size:
                 print('the queue is full, try pop()')
                 return
             self.__queue[self.__tail] = content
             self.__tail = (self.__tail+1)%self.__size
             self.__count += 1
@@ -104,40 +143,52 @@
             self.__count -= 1
         else:
             try:
                 del self.__queue[0]
             except IndexError:
                 print('warning : no value in the queue,try push(content) to add one')
 
-    def 入列(self, content):
-        self.push(content)
-
-    def 出列(self):
-        self.pop()
-
 
 class Stack():
     def __init__(self,size:int=-1):
         self.a = 0
         if size > 0:
             self.__stack = [0]*size
         else:
             self.__stack = []
         self.__size = size
         self.__top = -1
 
-    @property
-    def val(self):
-        return self.__stack
-
-    @property
-    def 值(self):
-        return self.__stack
+    def __repr__(self):
+        return f'Stack({str(self.__stack)}, topPointer = {self.__top if self.__top != -1 else len(self.__stack)-1})'
 
-    def push(self, content):
+    def __len__(self):
+        return self.__top if self.__size != -1 else len(self.__stack)
+
+    def __iter__(self):
+        return iter(self.getlist())
+
+    def __contains__(self, item):
+        return item in self.getlist()
+
+    def __getitem__(self, item):
+        return self.getlist()[int(item)]
+
+    def getlist(self):
+        contents = []
+        if self.__size == -1:
+            contents = self.__stack[:]
+        else:
+            for i in range(0, self.__top):
+                contents.append(self.__stack[i])
+        return contents
+
+    def push(self, content: int|str|float):
+        if type(content) not in (int, str, float):
+            raise TypeError
         if self.__size > 0:
             if self.__top < self.__size - 1:
                 self.__top += 1
                 self.__stack[self.__top] = content
             else:
                 print('stack is full, try pop()')
         else:
@@ -152,41 +203,139 @@
                 print('warning : stack is empty ,try push(content)')
         else:
             try:
                 print(self.__stack[0])
                 del self.__stack[0]
             except IndexError:
                 print('warning : stack is empty ,try push(content)')
-    def 入栈(self, content):
-        self.push(content)
 
-    def 出栈(self):
-        self.pop()
-
-class Hmath():
-    class Functions():
+class Hmath:
+    class Functions:
         def __init__(self, expression: str, variable: str):
+            if type(expression) != str or type(variable) != str:
+                raise TypeError
             self.__expression = expression
             self.__var = variable
 
-        def evaluate(self, value: (int, float)):
+        def evaluate(self, value: int|float):
+            if type(value) not in (int, float):
+                raise TypeError
             expression = self.__expression.replace(self.__var, str(value))
             return eval(expression)
 
-        def gradient(self, accuracy, value: (int, float)):
+        def gradient(self, accuracy:float, value: int|float):
+            if type(value) not in (int, float) or type(accuracy) != float:
+                raise TypeError
             x1 = value
             x2 = value + 10 ** -accuracy
             y1 = self.evaluate(x1)
             y2 = self.evaluate(x2)
             res = (y2 - y1) / (x2 - x1)
             return round(res, 1) if res - int(res) > 0.999 or res - int(res) < 0.001 else round(res, 3)
 
 
-def prints(content,style=fontstyle.DEFAULT,fontColor=color.WHITE,back=''):
-    print("\033[{};{};{}m{}\033[0m".format(style,fontColor,back,content))
+def prints(content,fontStyle=FontStyle.DEFAULT,fontColor=FontColor.WHITE,backgroundColor=BackgroundColor.DEFAULT):
+    print("\033[{};{};{}m{}\033[0m".format(fontStyle,fontColor,backgroundColor,content))
+
+class LinkedListNode:
+    def __init__(self, val):
+        if type(val) not in (int, str, float):
+            raise TypeError
+        self.val = val
+        self.next = None
+
+    def __repr__(self):
+        result = ''
+        temp = self
+        while temp != None:
+            result += (str(temp.val) + ' --> ')
+            temp = temp.next
+        print(result[:-5])
+        return f'LinkedList({result})'
+
+    def __iter__(self):
+        return iter(self.getlist())
+
+    def __contains__(self, item):
+        return item in self.getlist()
+
+    def __getitem__(self, item):
+        return self.getlist()[int(item)]
+
+    def getlist(self):
+        content = []
+        temp = self
+        while temp != None:
+            content.append(temp.val)
+            temp = temp.next
+        return content
+
+def create_linkedlist_from_list(lst:list):
+    if type(lst) != list:
+        raise TypeError
+    if len(lst) == 0:
+        return LinkedListNode(None)
+    node = LinkedListNode(lst[0])
+    temp = node
+    for i in lst[1:]:
+        temp.next = LinkedListNode(i)
+        temp = temp.next
+    return node
+
+def create_stack_from_list(lst:list, Fixedlength:bool = True):
+    if type(lst) != list:
+        raise TypeError
+
+    if Fixedlength:
+        stack = Stack(len(lst))
+    else:
+        stack = Stack()
+    for i in lst:
+        stack.push(i)
+    return stack
+
+def create_queue_from_list(lst:list, Fixedlength:bool = True):
+    if type(lst) != list:
+        raise TypeError
+
+    if Fixedlength:
+        queue = Queue(len(lst))
+    else:
+        queue = Queue()
+    for i in lst:
+        queue.push(i)
+    return queue
+
+
+
+def BinarySearch(iterable, target):
+    if not isinstance(iterable, Iterable):
+        raise TypeError
+    found = False
+    highIndex = len(iterable)-1
+    lowIndex = 0
+    while not found and lowIndex <= highIndex:
+
+        mid = (highIndex + lowIndex) // 2
+        if iterable[mid] == target:
+            found = True
+            print(mid)
+        elif iterable[mid] > target:
+            highIndex = mid - 1
+        else:
+            lowIndex = mid + 1
+
+    if not found:
+        print("not found")
+
+
+
+
+
+
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `HHLtools-1.0.8.1.dist-info/LICENSE.txt` & `HHLtools-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `HHLtools-1.0.8.1.dist-info/METADATA` & `HHLtools-1.1.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: HHLtools
-Version: 1.0.8.1
-Summary: A test project
+Version: 1.1.0
+Summary: A tool for CAIE 9618 learner
 Author: hhaolin
 Author-email: 2813579566@qq.com
 License: MIT
 Keywords: HHLtools
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -39,9 +39,13 @@
     | 1.0.6 add Hmath
 
 2022/10/28
     | 1.0.7 add prints,python 3.11 available
 
 2022/11/4
     | 1.0.8 Chinese extension
-        | 1.0.8.1 debug
+    | 1.0.8.1 debug
+
+2023/4/21
+    | 1.1.0 add linked list, and some useful modifications to previous function
+
```

