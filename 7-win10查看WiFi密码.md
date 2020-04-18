本文介绍win10如何查看连接过的WiFi密码

本文将介绍两种方法

第一种是正常的[鼠标操作](#鼠标操作)

第二种是装X的[Dos操作](#Dos操作)



#### 鼠标操作

1. **win + s** 输入 **wlan** 选择 **WLAN设置**

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.1.png" alt="image-20200323092304445" style="zoom: 80%;" />



2.选择 **更改适配器选项**

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.2.png" alt="image-20200323092304445" style="zoom: 80%;" />



3.双击 **WLAN**

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.3.png" alt="image-20200323093449105" style="zoom:67%;" />



4.选择 **无限属性**

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.4.png" alt="image-20200323093404316" style="zoom:80%;" />



5.选择 **安全**，勾选 **选择字符** 即可查看当前wifi密码

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.5.png" alt="image-20200323093449105" style="zoom:67%;" />

#### Dos操作

1.先创建一个txt文本文档

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.6.png" alt="image-20200323093449105" style="zoom: 80%;" />



2.修改后缀 **.txt** 为 **.bat**，有的小伙伴可能没有办法修改后缀名，只是重命名了，可以去我的另一篇博客（win10如何修改文件后缀）

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.7.png" alt="image-20200323093449105" style="zoom: 80%;" />



---



<img src="D:\Typroa_wsp\img\win10查看WiFi密码.8.png" alt="image-20200323093449105" style="zoom: 80%;" />



3.右键选择 **编辑** 赋值以下代码

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.9.png" alt="image-20200323093449105" style="zoom: 80%;" />



```vbscript
@echo off
:main
echo 当前电脑连接过的WIFI有:
netsh wlan show profiles

set /p wifi_name=请输入您要查询的WIFI名称:

netsh wlan show profiles name=%wifi_name% key="clear"
echo 是否继续查询(Y/N)？
set /p input=输入:
cls
if %input%==Y goto main
if %input%==N goto exit

:exit
exit
pause>nul
```



4.此时要注意，你需要选择记事本的文件点击另存为，而不是直接ctrl + s 保存文件，因为记事本直接保存的文件编码为UTF-8，而bat文件使用的中文编码为ANSI，如果不修改编码会程序中文乱码现象

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.10.png" alt="image-20200323093449105" style="zoom: 80%;" />



---



<img src="D:\Typroa_wsp\img\win10查看WiFi密码.11.png" alt="image-20200323093449105" style="zoom: 80%;" />



5.保存之后，右键编辑好的bat文件，**以管理员身份运行**，输入你要查询的WiFi名称

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.12.png" alt="image-20200323093449105" style="zoom: 80%;" />



6.**关键内容**就是WiFi密码，是不是很装叉呢

<img src="D:\Typroa_wsp\img\win10查看WiFi密码.13.png" alt="image-20200323093449105" style="zoom: 80%;" />