---
title: 读《深入React技术栈》
catalog: true
date: 2019-05-13 10:36:24
subtitle:
header-img:
tags:
- Skill
- Notes
---

CSS3、React底层原理、3D特效、设计模式等好多要补啊orz，块的学习从哪里开始呢？
这书是一个开始。

当你导出单例、函数库、空对象时使用帕斯卡式命名(一般的驼峰命名)

    const AirbnbStyleGuide = {
      es6: {
      }
    };

    export default AirbnbStyleGuide;


### memo

    ...
    const Foo = memo(function Foo (props) {
      console.log('Foo render');
      return <div>{props.person.age}</div>;
    })
    ...

![memo](https://user-gold-cdn.xitu.io/2019/6/12/16b49110278df11e?imageslim)


