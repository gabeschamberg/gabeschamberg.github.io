---
layout: page
title: Research
---

### Measuring Context Dependent Causal Influences

![Time-Varying Causality](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/causality5.png)

How can we tell when one time series is having a *causal* effect on another time series?

We adopt a [Granger causality](http://www.scholarpedia.org/article/Granger_causality) philosophy, where $$X$$ is said to cause $$Y$$ if we can better predict $$Y$$ using all available information than we can using all information excluding $$X$$. Both Granger causality and information theoretic extensions such as directed information provide average measures of causal influence that depend solely on the underlying probabilistic model of the variables in question. We ask the question: *Does the causal influence between random variables change for different realizations of those variable? If so, what is the right way to measure those changes?*

*Relevant Publications:*
- "A Sample Path Measure of Causal Influence", *IEEE International Symposium on Information Theory (ISIT)*, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8437627/)
[[arXiv]](https://arxiv.org/abs/1805.03333)

-----

### Non-Linear / Non-Markov Latent Time-Series Estimation

![Non-Linear/Non-Markov Problems](https://raw.githubusercontent.com/gabeschamberg/gabeschamberg.github.io/master/imgs/nonmarkov_nonlin_sig.png)

We consider the problem of estimating a latent multi-dimensional time-series given noisy measurements and knowledge of the dynamics of the signal. In the case of a Markov signal with linear dynamics and Gaussian measurements, the problem can be solved using the [Kalman filter](https://en.wikipedia.org/wiki/Kalman_filter).

We consider the class of problems where the underlying signal is non-Markov and/or the measurements obey and arbitrary log-concave likelihood model. We propose a framework that uses the [Alternating Direction Method of Multipliers](http://stanford.edu/~boyd/admm.html) to decompose problems of this nature into smaller, easy to solve subproblems.

*Relevant Publications:*
- “A Modularized Efficient Framework for
Non-Markov Time Series Estimation”, *IEEE Transactions on Signal Processing*, Volume 66, Issue 12, June 2018.
[[IEEE Xplore]](https://ieeexplore.ieee.org/document/8259364/)
[[arXiv]](https://arxiv.org/abs/1706.04685)
[[Code Ocean]](https://codeocean.com/2018/01/16/a-modularized-efficient-framework-for-non-markov-time-series-estimation/)
- “Efficient Low-Rank Spectrotemporal Decomposition using ADMM”, *IEEE Statistical Signal Processing Workshop*, June 2016.
[[IEEE Xplore]](http://ieeexplore.ieee.org/document/7551797/)

-----