# saoma
 v1.0

 扫码枪(条码枪CCSP Scan)v1.0扫可以实现无焦点捕获输入，支持串口和USB接口、上传数据。 
  [github](https://github.com/chygfm/saoma)    小巧精悍，不到1M。  [下载](https://cdn.jsdelivr.net/gh/chygfm/saoma@master/saoma.zip)
   
  USB接口
  ![](https://img-blog.csdnimg.cn/20200824115821918.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NoeWczMQ==,size_16,color_FFFFFF,t_70#pic_center)

设置
![](https://img-blog.csdnimg.cn/20200824115912530.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NoeWczMQ==,size_16,color_FFFFFF,t_70#pic_center)


串口
![](https://img-blog.csdnimg.cn/20200824120101323.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NoeWczMQ==,size_16,color_FFFFFF,t_70#pic_center)


# 概述
1、 分为免费版和注册版：
    免费版上传数据有限制。每次可上传20条数据；每天可上传200条数据；总共可上传60000条数据
    免费版串口接口每次扫码50条数据
    注册版没有限制。
2、 本软件不记录保存上传任何信息。
3、 其它说明
  A、USB接口
   (1)打开软件，把鼠标点击输入框，扫码即可
   (2)不用考虑鼠标，直接监控扫码输入，若360卫士提示有键盘监控请通过
   (3)在设置中，可修改扫码的数据和上传功能。修改数据后要保存才立即生效。
   (4)扫码以回车13为结束，扫码的字符输入间隔可调整，一般60-80毫秒。
  B、串口接口
   (1)选择正确的串口，自动获取字符串,支持中文
 
#  原理
1、 有输入框，则直接通过判断结束符号（回车）来确定一条扫码记录完成。
2、无焦点扫码，通过判断字符输入间隔小于设定的阈值（一般60-80毫秒），判断为扫码输入，否则是正常的键盘输入，并以结束符号（回车）来确定一条扫码记录完成。
3、服务器使用restful接口
4、串口读取ASCII字符



#Overview

1. It is divided into free version and registration version:

The free version has restrictions on uploading data. 20 pieces of data can be uploaded each time; 200 pieces of data can be uploaded every day; a total of 60000 pieces of data can be uploaded

The free version serial interface scans 50 pieces of data each time

There are no restrictions on the registration version.

2. This software does not record, save and upload any information.

3. Other instructions

A. USB interface

(1) Open the software, click the mouse on the input box and scan the code

(2) Do not consider the mouse, directly monitor the scan code input, if 360 guard prompt keyboard monitoring, please click

(3) In the setting, the scan code data and upload function can be modified. After modifying the data, it must be saved before it takes effect immediately.

(4) Code scanning ends with carriage return 13. The character input interval of scanning code can be adjusted, generally 60-80 Ms.

B. Serial port interface

(1) Select the correct serial port, automatically get the string, support Chinese



#Principle

1. If there is an input box, a code scanning record can be determined by judging the end symbol (enter).

2. No focus code scanning, by judging that the character input interval is less than the set threshold (generally 60-80 MS), it is judged as code scanning input, otherwise, it is normal keyboard input, and a code scanning record is determined by the end symbol (enter).

3. The server uses restful interface

4. Reading ASCII characters through serial port
