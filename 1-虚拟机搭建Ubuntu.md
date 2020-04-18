# 虚拟机搭建Ubuntu 19.10

本文将介绍使用Vmware虚拟机在Windows10上搭建Ubuntu，从下载到安装保姆级教程。

本文目录

1.[下载VMware15.5](#下载VMware15.5)

2.[安装Vmware](#安装Vmware)

3.[下载Ubuntu镜像文件](#下载Ubuntu镜像文件)

4.[创建虚拟机](#创建虚拟机)

5.[开启虚拟机](#开启虚拟机)



####下载VMware15.5

首先我们需要下载虚拟机VMware15.5

官网下载地址

`https://www.vmware.com/products/workstation-pro/workstation-pro-evaluation.html`

![image-20200322103928599](C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322103928599.png)

选择Workstation 15.5 Pro for Windows，点击Download Now就开始下载了，不要使用浏览器下载，建议使用迅雷下载

#### 安装VMware

这里要注意一点虚拟机最好安装在固态硬盘里，不要装在机械硬盘里。因为虚拟机是一个频繁读写硬盘的程序，放在机械硬盘里会影响速度，非常卡。有些小伙伴可能考虑占用磁盘空间大小的问题，单纯装一个Ubuntu用不到20GB的空间，所以这方面不用太担心。最后如果有的小伙伴固态硬盘没有空间了，那你就只好装在机械硬盘里吧。

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322111447643.png" alt="image-20200322111447643" style="zoom:80%;" />



![image-20200322111504188](C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322111504188.png)

![image-20200322112105686](C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322112105686.png)

选择安装位置，建议安装在c盘中



![image-20200322112152597](C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322112152597.png)





![image-20200322112207156](C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322112207156.png)



![image-20200322112218478](C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322112218478.png)



<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322112231539.png" alt="image-20200322112231539" style="zoom:80%;" />





####下载Ubuntu镜像文件

官网下载地址

`https://ubuntu.com/download/desktop`

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322114157373.png" alt="image-20200322114157373"  />

18.04.4 和19.10 都可以，这里我使用19.10，点击Download即开始下载



#### 创建虚拟机

点击 **创建新的虚拟机**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322114426262.png" alt="image-20200322114426262" style="zoom:80%;" />



选择 **典型**，下一步

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322114456466.png" alt="image-20200322114456466" style="zoom:80%;" />



选择 **稍后安装操作系统**，下一步

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322114602115.png" alt="image-20200322114602115" style="zoom:80%;" />



选择 **Linux** 版本选择 **Debian 10.x 64位**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322114648200.png" alt="image-20200322114648200" style="zoom:80%;" />



为虚拟机命名，位置建议选在固态硬盘，下一步

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322115720681.png" alt="image-20200322115720681" style="zoom:80%;" />



磁盘容量 20GB足以，即使不够后期也是可以扩容的，选择将**虚拟磁盘拆分为多个文件**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322115856940.png" alt="image-20200322115856940" style="zoom:80%;" />



点击 **完成**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322115913780.png" alt="image-20200322115913780" style="zoom:80%;" />



点击 **编辑虚拟机设置**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322115947709.png" alt="image-20200322115947709" style="zoom:80%;" />



内存2GB足以，电脑有8GB内存的可以选3GB左右，16GB内存的可以直接选择8GB，不过没有必要，我这里给了它4GB

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322120229150.png" alt="image-20200322120229150" style="zoom:80%;" />



处理器

一般的电脑处理器就一个，处理器内核可以根据自己电脑的CPU内核数量决定，以i7-9750H为例是6核心，所以给它三个核心，不会查内核数量的小伙伴可以去我的另一篇博客介绍Windows10如何查看cpu内核数量

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322121356846.png" alt="image-20200322121356846" style="zoom:80%;" />



选择 **CD/DVD(IDE)**，将之前下载的Ubuntu镜像文件导入，之后确定

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322121540560.png" alt="image-20200322121540560" style="zoom: 80%;" />



####开启虚拟机

选择 **中文简体**，**安裝Ubuntu**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322121817285.png" alt="image-20200322121817285" style="zoom:80%;" />



<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122011959.png" alt="image-20200322122011959" style="zoom:80%;" />



**正常安装** 取消 **安装Ubuntu时下载更新**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122157904.png" alt="image-20200322122157904" style="zoom:80%;" />



**现在安装**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122337040.png" alt="image-20200322122337040" style="zoom:80%;" />



**继续**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122355232.png" alt="image-20200322122355232" style="zoom:80%;" />



**继续**

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122545737.png" alt="image-20200322122545737" style="zoom:80%;" />



设置用户名和密码

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122617017.png" alt="image-20200322122617017" style="zoom:80%;" />



等待安装完毕

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122653520.png" alt="image-20200322122653520" style="zoom:80%;" />



下载文件可以跳过

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322122959144.png" alt="image-20200322122959144" style="zoom:80%;" />



安装完毕，重启

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322123240431.png" alt="image-20200322123240431" style="zoom:80%;" />



按下回车

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322123614843.png" alt="image-20200322123614843" style="zoom:80%;" />



登陆用户，大功告成

<img src="C:\Users\tangjian\AppData\Roaming\Typora\typora-user-images\image-20200322123700337.png" alt="image-20200322123700337" style="zoom:80%;" />



VMware Workstation Pro 15 序列号：

YG5H2-ANZ0H-M8ERY-TXZZZ-YKRV8

UG5J2-0ME12-M89WY-NPWXX-WQH88

UA5DR-2ZD4H-089FY-6YQ5T-YPRX6

GA590-86Y05-4806Y-X4PEE-ZV8E0

ZF582-0NW5N-H8D2P-0XZEE-Z22VA

YA18K-0WY8P-H85DY-L4NZG-X7RAD

CZ7WU-2MF01-488FZ-L6Z5T-PYAU4

CY1TH-0XZ5M-M85NY-MNXGG-ZZHU8

ZZ3EK-62W1P-H803P-4WN7T-Q7HT2

CY75U-ATW0P-H8EYZ-WDZE9-N68D6

GY7EH-DLY86-081EP-4GP59-WFRX0