---
layout: page
title: Research
---

### Context-Dependent Causal Influence

![Time-Varying Causality](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/causality5.png)

The problem of quantifying the causal influences between random entities is a non-trivial problem, even when there is a known causal graph and joint distribution over all variables. This work seeks to build an information theoretic framework for quantifying the extent to which one random variable (or process) influences another. The key feature of this framework is that the produced causal influences are *context-dependent*, meaning that the level of influence depends upon the *value* of a cause.

*Relevant Publications:*
- "Quantifying Context-Dependent Causal Influences", *NeurIPS Workshop on Causal Learning*, December 2018.
- "Measuring Sample Path Causal Influences with Relative Entropy", *Submitted*.
[[arXiv]](https://arxiv.org/abs/1810.05250)
- "A Sample Path Measure of Causal Influence", *IEEE International Symposium on Information Theory (ISIT)*, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8437627/)
[[arXiv]](https://arxiv.org/abs/1805.03333)

-----

### Non-Linear / Non-Markov Latent Time-Series Estimation

![Non-Linear/Non-Markov Problems](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/nonmarkov_nonlin_sig.png)

We consider the problem of estimating a latent multi-dimensional time-series given noisy measurements and knowledge of the dynamics of the signal. In the case of a Markov signal with linear dynamics and Gaussian measurements, the problem can be solved using the [Kalman filter](https://en.wikipedia.org/wiki/Kalman_filter).

We consider the class of problems where the underlying signal is non-Markov and/or the measurements obey and arbitrary log-concave likelihood model. We propose a framework that uses the [alternating direction method of multipliers](http://stanford.edu/~boyd/admm.html) to decompose problems of this nature into smaller, easy to solve subproblems.

*Relevant Publications:*
- “A Modularized Efficient Framework for
Non-Markov Time Series Estimation”, *IEEE Transactions on Signal Processing*, Volume 66, Issue 12, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8259364/)
[[arXiv]](https://arxiv.org/abs/1706.04685)
[[Code Ocean]](https://codeocean.com/2018/01/16/a-modularized-efficient-framework-for-non-markov-time-series-estimation/)
- “Efficient Low-Rank Spectrotemporal Decomposition using ADMM”, *IEEE Statistical Signal Processing Workshop*, June 2016.
[[IEEE Xplore]](http://ieeexplore.ieee.org/document/7551797/)

-----