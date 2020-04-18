这篇文章将告诉大家如何查看CPU的**核心数**以及**线程数**

####1.win + r 打开 cmd



<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\win10查看核心数.1.png" alt="win10查看核心数.1" style="zoom:80%;" />

#### 2.输入命令查询

```
进入cpu查询
wmic

查询cpu名字
cpu get name

查看cpu核数
cpu get NumberOfCores

查看cpu线程数
cpu get NumberOfLogicalProcessors

查看cpu所有信息
cpu get*
```



#### 3.在cmd输入wmic时可能会出现下面的情况





这是因为环境变量没有配置好的原因，

win + s 输入 **查看高级系统设置** ，**选择环境变量**





选择 **Path** ，点击 **编辑**





点击 **新建**， 输入 `C:\Windows\System32\wbem`，之后确定结束，问题就解决啦

