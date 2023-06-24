---
layout: post
title: "最大公约数"
date: 2023-06-20
categories: jekyll update
---

最大公约数（Greatest Common Divisor，简称GCD）是指：两个数中所有公共约数中最大的那个数。比如，18和12的最大公约数是6。

最大公约数有多种求解方法，其中最常见的是欧几里得算法（Euclidean Algorithm）。其基本思想是利用两个数的差求最大公约数，如果两数相等，则这个数就是最大公约数，否则再把较大的数变为两数之差，重复上述操作，直至求出最大公约数。

欧几里得算法可以用递归或迭代方式实现，代码如下：
~~~
    def gcd(a, b):
        if b == 0:
            return a
        else:
            return gcd(b, a % b)
~~~