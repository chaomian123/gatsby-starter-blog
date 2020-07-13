---
title: 如何将bv转换为av号
date: "2020-07-14T19:50:03.284Z"
description: 前端看得懂的方法
---
#####缘由： 
    you-get下载bilibili视频需要av打头的视频编号地址
#####目的:
    转换
#####资料:
    https://zhuanlan.zhihu.com/p/117358823
```
1.去掉BV 长度10位

2.一个固定字符串 = 'fZodR9XQDSUm21yCkr6zBqiveYah8bt4xsWpHnJE7jL5VG3guMTKNPAwcF'

3.获得BV各字符在s中的index 分为 b1 b2 b3 b4 ... b10

4.bn 乘以58的n次方 (Array）n依次等于 = “6、2、4、8、5、9、3、7、1、0” 固定顺序不能打乱

例 b1 * 58 ^ n1 = o1

5.o1 + o2 + ... + o10 = oSum

6.oSum - 固定值 100618342136696320 = x

7.二进制化（x） 与十进制的177451812异或运算（使用在线工具，不需要了解什么叫做异或运算）  得 y

8.`AV${十进制化（y）}`

```

