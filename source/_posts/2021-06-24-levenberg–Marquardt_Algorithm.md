---
title: Levenberg–Marquardt Algorithm
date: 2021-06-24 15:14:39
tags: math
mathjax: true
---


## 问题背景
在使用Matlab或Python解决某些实际问题时，我们不免要求解非线性方程组，或解决一些优化问题。这时你就有可能遇到 **Levenberg–Marquardt 算法**。


## Levenberg–Marquardt 算法
Levenberg–Marquardt 算法是一种最小二乘（模型拟合）算法。它可以解决以下问题：

$$
\min_{x}f(x)= \min_{x} \\| F(x) \\|^2_2 = \min_{x} \sum_i F_i^2(x)
$$

即求一个 $x$ 使 $f(x)$ 最小。

1944年[Kenneth Levenberg]( https://doi.org/10.1090/qam/10666)首次提出该算法，1963年[Donald Marquardt](https://doi.org/10.1137/0111030)也发现了该算法，后来这种算法被称作Levenberg–Marquardt。



关于该算法的详细原理和实现可以参考 Flannery 等人的著作 [Numerical recipes in C](http://www.nrbook.com/a/bookcpdf.php)。



## Levenberg–Marquardt 算法与非线性方程组求根
求解非线性方程组即求解一组 $\bar{x}$ 令其满足 $\bar{F}(x)=0$。显然非线性方程组的根可以令上式成立。

因此，给定初始值，通过Levenberg–Marquardt 算法求得的 $\bar{x}$  就是非线性方程组 $\bar{x}$ 的一组近似根（初始值附近）。

非线性方程组的根显然不止一组，而通过该方法只能得到距离初始值较近的根，要想得到全部的根，需要配合其他算法。


## 参考文献
* Levenberg, K. (1944). A method for the solution of certain non-linear problems in least squares. *Quarterly of applied mathematics*, 2(2), 164-168.
* Mardquardt, D. W. (1963). An algorithm for least square estimation of parameters. *J. Soc. Ind. Appl. Math*, 11, 431-441.
* Flannery, B. P., Press, W. H., Teukolsky, S. A., & Vetterling, W. (1992). Numerical recipes in C. *Press Syndicate of the University of Cambridge, New York*, 24(78), 36.