---
title: 无聊的最终境界，写了一个卡牌游戏
date: "2020-07-31T19:50:03.284Z"
description: 因为mac os没有
---
#####缘由： 
    突然想玩卡牌游戏，然而我不是window os
    计时5个小时完成
#####思路:
    
```
1.了解规则
2.查找拖拽api 最后决定采用drag drop事件，封装便捷获取dom及兄弟祖父元素的函数。
3.了解MDN例子，20分钟完成页面主体 + 洗牌 + 卡牌数组制造
4. 40分钟补充单个体拖拽
5. 插入如何匹配规则，20分钟决定在drag & drop事件中判断
6. 多个卡牌拖拽，利用  ev.dataTransfer.setData('text/plain', [me, ...bros] api
7. 定时器轮询右上stacks是否匹配胜利条件
8. 拖拽落点瑕疵，把col - bros- 卡牌也加入落点判断条件


```



![最后是这样](https://s1.ax1x.com/2020/08/01/a1qLS1.gif)
