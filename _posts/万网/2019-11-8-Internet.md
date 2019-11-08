---
layout:     post
title:      万网
subtitle:    "\" blog记录概要\""
date:       2019-11-8
author:     Jim
catalog: true
tags:
    - 万网
---
![mark](http://cdn.jokerjim.com/image/20191109/gVcegT28vdUq.png)
##对blog的简明概要记录
1.阿里云提供域名相关服务<br>
阿里云上注册的域名： www.jokerjim.com<br>
同样在上面也有一台轻量服务器 不过并没有托管代码和相关web服务，偶尔上云进Linux环境做些小实验<br>
①配置SSL证书并部署到域名上<br>
②在域名解析中设置CNAME类解析将主域名(www.jokerjim.com)解析到记录值（jim-carrey.github.o）上并在github pages的源码里添加CNAME文件并填入主域名（jokerjim.com）,同时确保在项目setting里设置开启域名解析并勾选https访问<br>
③设置A类解析，主机名@.jokerjim.com直接解析到IP地址上（美国github的IP）<br>


2.GitHub提供代码托管服务<br>
①代码托管在github上 使用github pages服务<br>


3.七牛云提供CDN加速及文件存储服务<br>
①创建图床并绑定二级域名(cdn.jokerjim.com)<br>
②在阿里云域名解析配置中新配置CNAME类解析，主机名填入前缀(cdn).jokerjim.com,解析值填入七牛平台上绑定二级域名对应的CNAME<br>
这样上传的文件就在二级域名(cdn.jokerjim.com)下，图片链到Markdown里就会转到七牛享受到CDN加速


