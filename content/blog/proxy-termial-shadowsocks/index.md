---
title: 终端翻墙笔记
date: "2020-07-07T19:50:03.284Z"
description: ……
---
打开配置文件
```shell script
    code ~/.zshrc 
```
添加配置文件
```shell script
    # proxy list
    alias proxy='export all_proxy=socks5://127.0.0.1:1080'
    alias unproxy='unset all_proxy'
```
使用proxy前先查看下当前的ip地址：
```shell script
  curl cip.cc
```
执行代理和解除代理的方式
```shell script
    proxy
    unproxy
```

