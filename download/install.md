
# [<img src="https://www.hankmi.com/favicon.ico" width="60" height="60" align="center" />](https://www.hankmi.com) HankMi官方网站

## 安装抬腕系列应用
本教程将指导你逐步完成apk的安装操作。在我们正式开始之前，请先确保你已完成以下操作：  
1.在[抬腕应用商店](apps.md)下载了需要的安装包  
2.找到你下载的安装包文件  
3.确认手表和数据线在你身边  
我们将依次介绍如何使用Windows PC和Android手机完成操作。  

***

## 在Windows PC上安装
1.前往这个网址，安装安卓手表ADB实用工具箱  
~~~
https://vincent8623.lanzouw.com/AndroidWatch-ADB-ToolBox
~~~
2.打开安卓手表ADB实用工具箱  
3.在手表上打开“开发者选项”  
~~~
WearOS：设置>系统>关于>连续点击版本号>回到设置首页>开发者选项>ADB调试；
OPPO：设置>更多设置>关于>连续点击版本号>返回上一级>开发者选项>USB调试  
~~~
4.将手表连接到电脑，按程序提示操作即可

***

## 在Android手机上安装
1.前往这个网址，安装WearOS工具箱  
~~~
https://www.wearosbox.com/
~~~
2.打开WearOS工具箱APP  
3.在手表上打开“开发者选项”
~~~
WearOS：设置>系统>关于>连续点击版本号>回到设置首页>开发者选项>ADB调试（也要开启WLAN调试）；
OPPO：设置>更多设置>关于>连续点击版本号>返回上一级>开发者选项>USB调试
~~~
4.将手表连接到Android手机，按程序提示操作即可

***

## 在命令行中执行ADB
1.在Windows PC上，同时按下键盘`Windows` `R`以打开运行对话框  
2.输入cmd并轻点回车以打开命令提示符  
3.执行以下命令以安装
~~~
adb install -r [apk路径]
~~~
你需要提前部署ADB运行环境
