<!--
author: vinnyzhao 
date: 2016-10-7
title: Putty组装及使用 
tags:  tools,ssh
category: tools 
status: publish
summary: Putty是Windows上远程登录的工具，支持常用的SSH和Telnet登录，是开源免费的软件。  
-->
## Putty 简单介绍
Putty是一个免费的、开源的telnet、rlogin和ssh客户端，功能丝毫不逊色于商业的远程登录类工具。在各种远程登录工具中，Putty是出色的工具之一,是SecureCRT商业软件的理想替代产品。

Putty拓展功能有限，但由于其开源的特性，目前有许多在Putty基础上二次封装的产品，例如PuttyCM、SuperPutty、PuttyTM等。主要针对putty本身一些功能进行扩展，例如不能分标签、不能自动登录等。


## Putty 下载

[Putty及封装工具下载地址：http://download.webtocn.com/index.html/Software/Putty/](http://download.webtocn.com/index.html/Software/Putty/)

在下载目录中有多个软件，每个工具都有其特性
```
SuperPutty_v1.3_special.zip                        06-Oct-2016 23:22    421K
putty-0.67.zip                                     06-Oct-2016 23:22      1M
puttycm-0.7.1-b-136.zip                            06-Oct-2016 23:22    461K
puttytm.zip                                        06-Oct-2016 23:22    112K
```
基础putty是`putty-0.67.zip`,他是其他封装类工具的内核，在使用其他类型工具前必须先安装基础putty。

- PuttyCM(Putty Connection Manager):在putty的基础上添加了多tab支持，添加了本地数据库保存用户名密码用于自动登录。但是有个bug，例如最小化后不能还原。

- PuttyTM(PuTTY Tab Manager):在putty的基础上添加多tab支持，添加了文件传输功能。不能保存密码自动登录。

- SuperPutty:在putty基础上添加了多tab支持。

## Putty 组装

1.下载并安装putty
这个下载最好到putty官网下载原版，但是由于伟大网络防火长城，你不得不爬上墙头翻过去。当然也可以在其他地方下载，比如download.webtocn.com。

2.下载封装工具包
上面给了3个建议的封装工具包，用户可以根据自己需求选择一个，也可以都下载体验一番在做选择。功能相对强大的是PuttyCM，主要是应为他能够保存密码自动登录。

3.安装封装工具包
在安装封装工具包时第一次打开都会让你指定putty的安装位置。

## Putty 使用
这里我选择的是PuttyCM，使用方法就以它为例。

基础内容就不介绍了，就那几个标签，点点就知道。主要说一些独有的特性。

- 自动登录功能使用 
创建一个数据库用以保存远程登录时的用户名和密码。   
创建一个登录session并保存在数据库中。   
设置这个session的属性，比如输入时的延迟。这里要注意的是，PuttyCM自动登录是模拟用户键盘输入，根据自己的网络延迟设置输入用户名和密码的时间，否则...你懂得。


