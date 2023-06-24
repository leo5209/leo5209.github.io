---
layout: post
title: "斐波那契数列"
date: 2023-06-20
categories: jekyll update
---

斐波那契数列（Fibonacci Sequence）是指：1、1、2、3、5、8、13、21、34……每一项是前两项之和。这个数列在自然界中很常见，比如数学上的黄金分割、植物的叶子排列、蜂巢等等。

斐波那契数列可以用递归的方式实现，在代码中如下：
~~~
    def fibonacci(n):
        if n <= 1:
            return n
        else:
            return fibonacci(n-1) + fibonacci(n-2)
~~~