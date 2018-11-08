---
title: 'Unbiased Estimators'
date: 2018-11-08
permalink: /posts/2018/11/unbiased-estimators/
tags:
  - mathematics
  - statistics
  - problem
---

Let $X$ be a random variable with mean $\mu$ and variance $\sigma^2$. Given iid samples $X_1, \ldots, X_n$, one knows that the sample mean $\bar{X} := \frac{1}{n}(X_1+\cdots+X_n)$ and sample variance $S^2 := \frac{1}{n-1}\sum (X_i - \bar{X})^2$ are unbiased estimators for $\mu$ and $\sigma^2$ respectively, meaning that $\mathbb{E}[\bar{X}] = \mu$ and $\mathbb{E}[S^2] = \sigma^2$.

Now consider this more complicated situation: Let $X$ and $Y$ be random variables. One has iid samples $X_1, \ldots, X_n$, and for each $i\in[n]$, one has iid samples $Y_1^i, \ldots, Y_m^i\sim P(Y|X_i)$. Now the question is, how to build an unbiased estimator for $\mathrm{Var}(Y)$. One approach is to use the following famous formula:
$$\mathrm{Var}(Y) = \mathrm{Var}(\mathbb{E}(Y|X)) + \mathbb{E}(\mathrm{Var}(Y|X)),$$
but it's not so clear how to build an unbiased estimator out of this formula.

Any comments?
